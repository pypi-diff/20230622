# Comparing `tmp/theboringlibrary-0.1.0.tar.gz` & `tmp/theboringlibrary-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "theboringlibrary-0.1.0.tar", max compression
+gzip compressed data, was "theboringlibrary-0.2.0.tar", max compression
```

## Comparing `theboringlibrary-0.1.0.tar` & `theboringlibrary-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2023-06-20 21:53:04.566889 theboringlibrary-0.1.0/LICENSE
--rw-r--r--   0        0        0       36 2023-06-20 21:53:04.566889 theboringlibrary-0.1.0/README.md
--rw-r--r--   0        0        0      526 2023-06-20 21:53:04.566889 theboringlibrary-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       11 2023-06-20 21:53:04.566889 theboringlibrary-0.1.0/src/theboringlibrary/__init__.py
--rw-r--r--   0        0        0      121 2023-06-20 21:53:04.566889 theboringlibrary-0.1.0/src/theboringlibrary/core.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 theboringlibrary-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-22 19:02:17.898404 theboringlibrary-0.2.0/LICENSE
+-rw-r--r--   0        0        0       36 2023-06-22 19:02:17.898404 theboringlibrary-0.2.0/README.md
+-rw-r--r--   0        0        0      526 2023-06-22 19:02:17.898404 theboringlibrary-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-06-22 19:02:17.898404 theboringlibrary-0.2.0/src/theboringlibrary/__init__.py
+-rw-r--r--   0        0        0      121 2023-06-22 19:02:17.898404 theboringlibrary-0.2.0/src/theboringlibrary/core.py
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 theboringlibrary-0.2.0/PKG-INFO
```

### Comparing `theboringlibrary-0.1.0/LICENSE` & `theboringlibrary-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `theboringlibrary-0.1.0/pyproject.toml` & `theboringlibrary-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "theboringlibrary"
-version = "0.1.0"
+version = "0.2.0"
 description = "It does nothing!"
 authors = ["Stefano Frassetto <frassetto.stefano@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "theboringlibrary", from = "src" }
 ]
```

### Comparing `theboringlibrary-0.1.0/PKG-INFO` & `theboringlibrary-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: theboringlibrary
-Version: 0.1.0
+Version: 0.2.0
 Summary: It does nothing!
 Author: Stefano Frassetto
 Author-email: frassetto.stefano@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

