# Comparing `tmp/pythorhead-0.6.0.tar.gz` & `tmp/pythorhead-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythorhead-0.6.0.tar", last modified: Wed Jun 21 18:07:43 2023, max compression
+gzip compressed data, was "pythorhead-0.7.0.tar", last modified: Wed Jun 21 22:52:55 2023, max compression
```

## Comparing `pythorhead-0.6.0.tar` & `pythorhead-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:43.093744 pythorhead-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:43.089744 pythorhead-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:43.089744 pythorhead-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-21 18:07:26.000000 pythorhead-0.6.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-21 18:07:26.000000 pythorhead-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-21 18:07:32.000000 pythorhead-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-21 18:07:26.000000 pythorhead-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-21 18:07:43.093744 pythorhead-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-21 18:07:26.000000 pythorhead-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:43.089744 pythorhead-0.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-21 18:07:26.000000 pythorhead-0.6.0/examples/pm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-21 18:07:26.000000 pythorhead-0.6.0/examples/user.py
--rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-21 18:07:26.000000 pythorhead-0.6.0/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-21 18:07:32.000000 pythorhead-0.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:43.093744 pythorhead-0.6.0/pythorhead/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/lemmy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/post.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/private_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:43.093744 pythorhead-0.6.0/pythorhead/types/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/types/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/types/listing.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/types/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-21 18:07:26.000000 pythorhead-0.6.0/pythorhead/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:07:43.093744 pythorhead-0.6.0/pythorhead.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-21 18:07:43.000000 pythorhead-0.6.0/pythorhead.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 18:07:43.000000 pythorhead-0.6.0/pythorhead.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:07:43.000000 pythorhead-0.6.0/pythorhead.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 18:07:43.000000 pythorhead-0.6.0/pythorhead.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:07:26.000000 pythorhead-0.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:07:43.093744 pythorhead-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:52:55.324626 pythorhead-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:52:55.320625 pythorhead-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:52:55.320625 pythorhead-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-21 22:52:38.000000 pythorhead-0.7.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-06-21 22:52:38.000000 pythorhead-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-06-21 22:52:44.000000 pythorhead-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-21 22:52:38.000000 pythorhead-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-21 22:52:55.324626 pythorhead-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-21 22:52:38.000000 pythorhead-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:52:55.320625 pythorhead-0.7.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-21 22:52:38.000000 pythorhead-0.7.0/examples/pm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-21 22:52:38.000000 pythorhead-0.7.0/examples/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121595 2023-06-21 22:52:38.000000 pythorhead-0.7.0/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-21 22:52:44.000000 pythorhead-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:52:55.324626 pythorhead-0.7.0/pythorhead/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/lemmy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/post.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/private_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5737 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:52:55.324626 pythorhead-0.7.0/pythorhead/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/types/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/types/listing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-21 22:52:38.000000 pythorhead-0.7.0/pythorhead/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:52:55.324626 pythorhead-0.7.0/pythorhead.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    41109 2023-06-21 22:52:55.000000 pythorhead-0.7.0/pythorhead.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-21 22:52:55.000000 pythorhead-0.7.0/pythorhead.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:52:55.000000 pythorhead-0.7.0/pythorhead.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 22:52:55.000000 pythorhead-0.7.0/pythorhead.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:52:38.000000 pythorhead-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:52:55.324626 pythorhead-0.7.0/setup.cfg
```

### Comparing `pythorhead-0.6.0/.github/workflows/pypi.yml` & `pythorhead-0.7.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/.gitignore` & `pythorhead-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/CHANGELOG.md` & `pythorhead-0.7.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog
 
+## [v0.7.0](https://github.com/db0/pythorhead/tree/v0.7.0) (2023-06-21)
+
+[Full Changelog](https://github.com/db0/pythorhead/compare/v0.6.0...v0.7.0)
+
+**Merged pull requests:**
+
+- feat: nodeinfo [\#16](https://github.com/db0/pythorhead/pull/16) ([db0](https://github.com/db0))
+
 ## [v0.6.0](https://github.com/db0/pythorhead/tree/v0.6.0) (2023-06-21)
 
 [Full Changelog](https://github.com/db0/pythorhead/compare/v0.5.0...v0.6.0)
 
 **Merged pull requests:**
 
 - feat: Sending PM [\#15](https://github.com/db0/pythorhead/pull/15) ([db0](https://github.com/db0))
```

### Comparing `pythorhead-0.6.0/LICENSE` & `pythorhead-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/PKG-INFO` & `pythorhead-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.6.0
+Version: 0.7.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.6.0/README.md` & `pythorhead-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/examples/pm.py` & `pythorhead-0.7.0/examples/pm.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/examples/user.py` & `pythorhead-0.7.0/examples/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/logo.png` & `pythorhead-0.7.0/logo.png`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/pyproject.toml` & `pythorhead-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "pythorhead"
 description = "A python library for interacting with Lemmy API"
 authors = [
     {name = "db0", email = "mail@dbzer0.com"},
 ]
-version = "v0.6.0"
+version = "v0.7.0"
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file="LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
```

### Comparing `pythorhead-0.6.0/pythorhead/auth.py` & `pythorhead-0.7.0/pythorhead/auth.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/pythorhead/comment.py` & `pythorhead-0.7.0/pythorhead/comment.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/pythorhead/lemmy.py` & `pythorhead-0.7.0/pythorhead/lemmy.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,21 +15,25 @@
     post: Post
     comment: Comment
     _known_communities = {}
     _requestor: Requestor
 
     def __init__(self, api_base_url: str) -> None:
         self._requestor = Requestor()
-        self._requestor.set_api_base_url(f"{api_base_url}/api/v3")
+        self._requestor.set_domain(api_base_url)
         self.post = Post()
         self.comment = Comment()
         self.site = Site()
         self.user = User()
         self.private_message = PrivateMessage()
 
+    @property
+    def nodeinfo(self):
+        return self._requestor.nodeinfo
+
     def log_in(self, username_or_email: str, password: str) -> bool:
         return self._requestor.log_in(username_or_email, password)
 
     def discover_community(self, community_name: str) -> Optional[int]:
         if community_name in self._known_communities:
             return self._known_communities[community_name]
```

### Comparing `pythorhead-0.6.0/pythorhead/post.py` & `pythorhead-0.7.0/pythorhead/post.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/pythorhead/private_message.py` & `pythorhead-0.7.0/pythorhead/private_message.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/pythorhead/site.py` & `pythorhead-0.7.0/pythorhead/site.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/pythorhead/user.py` & `pythorhead-0.7.0/pythorhead/user.py`

 * *Files identical despite different names*

### Comparing `pythorhead-0.6.0/pythorhead.egg-info/PKG-INFO` & `pythorhead-0.7.0/pythorhead.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythorhead
-Version: 0.6.0
+Version: 0.7.0
 Summary: A python library for interacting with Lemmy API
 Author-email: db0 <mail@dbzer0.com>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pythorhead-0.6.0/pythorhead.egg-info/SOURCES.txt` & `pythorhead-0.7.0/pythorhead.egg-info/SOURCES.txt`

 * *Files identical despite different names*

