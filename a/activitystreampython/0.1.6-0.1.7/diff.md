# Comparing `tmp/activitystreampython-0.1.6.tar.gz` & `tmp/activitystreampython-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitystreampython-0.1.6.tar", max compression
+gzip compressed data, was "activitystreampython-0.1.7.tar", max compression
```

## Comparing `activitystreampython-0.1.6.tar` & `activitystreampython-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      562 2023-05-26 15:14:34.843418 activitystreampython-0.1.6/LICENSE
--rw-r--r--   0        0        0     3000 2023-05-26 15:14:34.844068 activitystreampython-0.1.6/README.md
--rw-r--r--   0        0        0       46 2023-05-26 13:03:57.815792 activitystreampython-0.1.6/activitystreampython/__init__.py
--rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.6/activitystreampython/activitystream.py
--rw-r--r--   0        0        0      609 2023-05-26 15:51:14.781976 activitystreampython-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 activitystreampython-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      562 2023-05-26 15:14:34.843418 activitystreampython-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3000 2023-05-26 15:14:34.844068 activitystreampython-0.1.7/README.md
+-rw-r--r--   0        0        0       46 2023-05-26 13:03:57.815792 activitystreampython-0.1.7/activitystreampython/__init__.py
+-rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.7/activitystreampython/activitystream.py
+-rw-r--r--   0        0        0      607 2023-06-22 16:27:08.134986 activitystreampython-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3811 1970-01-01 00:00:00.000000 activitystreampython-0.1.7/PKG-INFO
```

### Comparing `activitystreampython-0.1.6/LICENSE` & `activitystreampython-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.6/README.md` & `activitystreampython-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.6/activitystreampython/activitystream.py` & `activitystreampython-0.1.7/activitystreampython/activitystream.py`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.6/pyproject.toml` & `activitystreampython-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "activitystreampython"
-version = "0.1.6"
+version = "0.1.7"
 description = "A convenience library to make retrieving data from the Activity Stream Data Service API easier"
 authors = ["Hugh Topping <hugh@crowdengage.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/crowdengage/activitystreampython/"
 repository = "https://github.com/crowdengage/activitystreampython/"
 
 [tool.poetry.dependencies]
-python = "^3.9.5"
+python = "^3.8"
 requests = "^2.31.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `activitystreampython-0.1.6/PKG-INFO` & `activitystreampython-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: activitystreampython
-Version: 0.1.6
+Version: 0.1.7
 Summary: A convenience library to make retrieving data from the Activity Stream Data Service API easier
 Home-page: https://github.com/crowdengage/activitystreampython/
 License: Apache-2.0
 Author: Hugh Topping
 Author-email: hugh@crowdengage.com
-Requires-Python: >=3.9.5,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/crowdengage/activitystreampython/
 Description-Content-Type: text/markdown
 
 # activitystreampython
```

