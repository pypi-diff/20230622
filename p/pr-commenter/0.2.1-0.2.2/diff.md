# Comparing `tmp/pr_commenter-0.2.1.tar.gz` & `tmp/pr_commenter-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_commenter-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pr_commenter-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pr_commenter-0.2.1.tar` & `pr_commenter-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3807 2023-06-22 00:47:17.131961 pr_commenter-0.2.1/README.md
--rw-r--r--   0        0        0     7180 2023-06-22 00:47:17.131961 pr_commenter-0.2.1/pr_commenter.py
--rw-r--r--   0        0        0     1156 2023-06-22 00:47:17.131961 pr_commenter-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pr_commenter-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3807 2023-06-22 01:35:19.719389 pr_commenter-0.2.2/README.md
+-rw-r--r--   0        0        0     7181 2023-06-22 01:35:19.719389 pr_commenter-0.2.2/pr_commenter.py
+-rw-r--r--   0        0        0     1156 2023-06-22 01:35:19.719389 pr_commenter-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pr_commenter-0.2.2/PKG-INFO
```

### Comparing `pr_commenter-0.2.1/README.md` & `pr_commenter-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pr_commenter-0.2.1/pr_commenter.py` & `pr_commenter-0.2.2/pr_commenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   --token=<token>               Github token. Default to the envvar PR_COMMENTER_GITHUB_TOKEN.
   --label=<label>               Add label/s if there were a comment
   --build=<build>               Identifier. If a comment for the template and build exist the 
                                 new message will be appended.
   --debug                       Show the final comment but don't post it to Github
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 logger = logging.getLogger(__file__)
 
 
 def setup_logger(debug=False):
     # setup loggin
     logger.setLevel(logging.DEBUG if debug else logging.INFO)
@@ -98,25 +98,25 @@
           node(id: $commentID) {
             ... on Minimizable {
               isMinimized
             }
           }
          }
         """
-        variables = {'commentID': comment.raw_data["node_id"]}
+        variables = {"commentID": comment.raw_data["node_id"]}
         result = self._post(query, variables)
-        return result["data"]["node"]['isMinimized']
+        return result["data"]["node"]["isMinimized"]
 
 
 def render(lines, template=None, build="", is_append=False):
     """
     Render the comment template passing environment variables and the lines as input_lines
     """
     if template:
-        env = Environment(autoescape=True)
+        env = Environment(autoescape=False)
         t = env.from_string(Path(template).read_text())
         comment = t.render({"input_lines": lines, "is_append": is_append, **environ})
         if not is_append:
             comment = f"<!-- pr-commenter: {template} {build or ''} -->\n{comment}"
     else:
         comment = "\n".join(lines)
     logger.debug("Comment:\n%s", comment)
```

### Comparing `pr_commenter-0.2.1/pyproject.toml` & `pr_commenter-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pr_commenter-0.2.1/PKG-INFO` & `pr_commenter-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-commenter
-Version: 0.2.1
+Version: 0.2.2
 Summary: Create and manage automatic comments in a Github PR
 Author-email: Martín Gaitán <marting@shiphero.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

