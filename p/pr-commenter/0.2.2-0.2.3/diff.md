# Comparing `tmp/pr_commenter-0.2.2.tar.gz` & `tmp/pr_commenter-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pr_commenter-0.2.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pr_commenter-0.2.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pr_commenter-0.2.2.tar` & `pr_commenter-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3807 2023-06-22 01:35:19.719389 pr_commenter-0.2.2/README.md
--rw-r--r--   0        0        0     7181 2023-06-22 01:35:19.719389 pr_commenter-0.2.2/pr_commenter.py
--rw-r--r--   0        0        0     1156 2023-06-22 01:35:19.719389 pr_commenter-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pr_commenter-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3807 2023-06-22 18:35:15.736351 pr_commenter-0.2.3/README.md
+-rw-r--r--   0        0        0     7185 2023-06-22 18:35:15.736351 pr_commenter-0.2.3/pr_commenter.py
+-rw-r--r--   0        0        0     1156 2023-06-22 18:35:15.736351 pr_commenter-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     4775 1970-01-01 00:00:00.000000 pr_commenter-0.2.3/PKG-INFO
```

### Comparing `pr_commenter-0.2.2/README.md` & `pr_commenter-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pr_commenter-0.2.2/pr_commenter.py` & `pr_commenter-0.2.3/pr_commenter.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   --token=<token>               Github token. Default to the envvar PR_COMMENTER_GITHUB_TOKEN.
   --label=<label>               Add label/s if there were a comment
   --build=<build>               Identifier. If a comment for the template and build exist the 
                                 new message will be appended.
   --debug                       Show the final comment but don't post it to Github
 """
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 logger = logging.getLogger(__file__)
 
 
 def setup_logger(debug=False):
     # setup loggin
     logger.setLevel(logging.DEBUG if debug else logging.INFO)
@@ -143,15 +143,15 @@
     template = args["--template"]
     build = args["--build"]
     lines = []
     files = args["<file>"]
     if files:
         with fileinput.input(files=files) as f:
             for line in f:
-                lines.append(line.strip())
+                lines.append(line.rstrip("\n"))
 
     # update or create a comment
     comment = None
 
     for previous_comment in pr.get_issue_comments():
         if previous_comment.user.login != user.login or graphql_client.is_minimized(previous_comment):
             # we do not consider already minimized comments
@@ -178,15 +178,14 @@
                     previous_comment.edit(comment)
                     logger.info(f"Comment updated: {previous_comment.html_url}")
                 break
 
     is_empty = False
     if not comment:
         comment = render(lines, template, args["--build"])
-
         is_empty = re.sub(r"<!-- pr-commenter[^>]*-->", "", comment).strip() == ""
         if is_empty:
             logger.info("New comment is empty. Skipping...")
             for label in labels:
                 pr.remove_from_labels(label)
             if labels:
                 logger.info(f"Labels removed: {', '.join(labels)}")
```

### Comparing `pr_commenter-0.2.2/pyproject.toml` & `pr_commenter-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pr_commenter-0.2.2/PKG-INFO` & `pr_commenter-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pr-commenter
-Version: 0.2.2
+Version: 0.2.3
 Summary: Create and manage automatic comments in a Github PR
 Author-email: Martín Gaitán <marting@shiphero.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

