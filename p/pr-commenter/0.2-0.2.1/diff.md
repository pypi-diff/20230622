# Comparing `tmp/pr_commenter-0.2.tar.gz` & `tmp/pr_commenter-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_commenter-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pr_commenter-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pr_commenter-0.2.tar` & `pr_commenter-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3807 2023-06-21 16:06:32.861657 pr_commenter-0.2/README.md
--rw-r--r--   0        0        0     6237 2023-06-21 16:06:32.861657 pr_commenter-0.2/pr_commenter.py
--rw-r--r--   0        0        0     1156 2023-06-21 16:06:32.861657 pr_commenter-0.2/pyproject.toml
--rw-r--r--   0        0        0     4773 1970-01-01 00:00:00.000000 pr_commenter-0.2/PKG-INFO
+-rw-r--r--   0        0        0     3807 2023-06-22 00:47:17.131961 pr_commenter-0.2.1/README.md
+-rw-r--r--   0        0        0     7180 2023-06-22 00:47:17.131961 pr_commenter-0.2.1/pr_commenter.py
+-rw-r--r--   0        0        0     1156 2023-06-22 00:47:17.131961 pr_commenter-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pr_commenter-0.2.1/PKG-INFO
```

### Comparing `pr_commenter-0.2/README.md` & `pr_commenter-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pr_commenter-0.2/pr_commenter.py` & `pr_commenter-0.2.1/pr_commenter.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   --token=<token>               Github token. Default to the envvar PR_COMMENTER_GITHUB_TOKEN.
   --label=<label>               Add label/s if there were a comment
   --build=<build>               Identifier. If a comment for the template and build exist the 
                                 new message will be appended.
   --debug                       Show the final comment but don't post it to Github
 """
 
-__version__ = "0.2"
+__version__ = "0.2.1"
 
 logger = logging.getLogger(__file__)
 
 
 def setup_logger(debug=False):
     # setup loggin
     logger.setLevel(logging.DEBUG if debug else logging.INFO)
@@ -53,41 +53,62 @@
         user = gh.get_user()
         pr = gh.get_repo(repo).get_pull(int(pr_number))
         return pr, user
     except (KeyError, GithubException):
         raise ValueError("Repo or PR not found")
 
 
-def minimize_comment(comment, token, reason="OUTDATED"):
-    """
-    Minimize (hide) a comment on GitHub using the api v4
-    (as pygithub only cover the api rest v3 and this feature is not there)
-
-    This will hide the comment from view, but not delete it.
-    Valid reasons are: ABUSE, OFF_TOPIC, OUTDATED, RESOLVED, SPAM
-    """
-    minimize_comment = """
-        mutation MinimizeComment($commentId: ID!, $minimizeReason: ReportedContentClassifiers!) {
-            minimizeComment(input: {subjectId: $commentId, classifier: $minimizeReason}) {
+class GraphqlClient:
+    def __init__(self, token):
+        self.token = token
+
+    def _post(self, query_or_mutation, variables=None):
+        response = requests.post(
+            "https://api.github.com/graphql",
+            headers={
+                "Authorization": f"token {self.token}",
+                "Content-Type": "application/json",
+            },
+            json={"query": query_or_mutation, "variables": variables},
+        )
+        return response.json()
+
+    def minimize_comment(self, comment, reason="OUTDATED"):
+        """
+        Minimize (hide) a comment on GitHub using the api v4
+        (as pygithub only cover the api rest v3 and this feature is not there)
+
+        This will hide the comment from view, but not delete it.
+        Valid reasons are: ABUSE, OFF_TOPIC, OUTDATED, RESOLVED, SPAM
+        """
+        mutation = """
+            mutation MinimizeComment($commentId: ID!, $minimizeReason: ReportedContentClassifiers!) {
+                minimizeComment(input: {subjectId: $commentId, classifier: $minimizeReason}) {
                 clientMutationId
             }
-    }"""
-
-    response = requests.post(
-        "https://api.github.com/graphql",
-        headers={
-            "Authorization": f"token {token}",
-            "Content-Type": "application/json",
-        },
-        json={
-            "query": minimize_comment,
-            "variables": {"commentId": comment.raw_data["node_id"], "minimizeReason": reason},
-        },
-    )
-    logger.info(response.json())
+        }"""
+        variables = {"commentId": comment.raw_data["node_id"], "minimizeReason": reason}
+        return self._post(mutation, variables)
+
+    def is_minimized(self, comment) -> bool:
+        """
+        Check if a comment is minimized (hidden) on GitHub using the api v4
+        """
+        query = """
+         query CheckMinimizedComment($commentID: ID!) {
+          node(id: $commentID) {
+            ... on Minimizable {
+              isMinimized
+            }
+          }
+         }
+        """
+        variables = {'commentID': comment.raw_data["node_id"]}
+        result = self._post(query, variables)
+        return result["data"]["node"]['isMinimized']
 
 
 def render(lines, template=None, build="", is_append=False):
     """
     Render the comment template passing environment variables and the lines as input_lines
     """
     if template:
@@ -113,40 +134,43 @@
         raise DocoptExit("Token not found. Pass --token or set the environment variable PR_COMMENTER_GITHUB_TOKEN")
 
     try:
         pr, user = get_pr_and_user(token, repo=args["<repo>"], pr_number=args["<pr>"].strip("pr/"))
     except ValueError as e:
         raise DocoptExit(str(e))
 
+    graphql_client = GraphqlClient(token)
     labels = args["--label"]
     template = args["--template"]
     build = args["--build"]
     lines = []
     files = args["<file>"]
     if files:
         with fileinput.input(files=files) as f:
             for line in f:
                 lines.append(line.strip())
 
     # update or create a comment
     comment = None
+
     for previous_comment in pr.get_issue_comments():
-        if previous_comment.user.login != user.login:
-            # only consider comments from the same user
+        if previous_comment.user.login != user.login or graphql_client.is_minimized(previous_comment):
+            # we do not consider already minimized comments
             continue
 
+        # previous comment is a candidate to be minimized or updated
         first_line = previous_comment.body.split("\n")[0]
 
         match = re.search(r"<!-- pr-commenter: (\S+) (\S+)?\s*-->", first_line)
         if match:
             prev_template, prev_build = match.groups()
             if prev_template == template and prev_build != build:
                 logger.info("Found a previous comment for a different build. Minimizing it...")
                 if not debug:
-                    minimize_comment(previous_comment, token=token)
+                    graphql_client.minimize_comment(previous_comment)
                 break
             elif prev_template == template and prev_build == build:
                 logger.info("Found a previous comment for the same build. Appending...")
                 new_comment = render(lines, template, build, is_append=True)
                 comment = f"{previous_comment.body}\n{new_comment}"
 
                 logger.debug(f"Updated comment: {comment}")
```

### Comparing `pr_commenter-0.2/pyproject.toml` & `pr_commenter-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pr_commenter-0.2/PKG-INFO` & `pr_commenter-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-commenter
-Version: 0.2
+Version: 0.2.1
 Summary: Create and manage automatic comments in a Github PR
 Author-email: Martín Gaitán <marting@shiphero.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

