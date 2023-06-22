# Comparing `tmp/kegstand-0.3.5.tar.gz` & `tmp/kegstand-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kegstand-0.3.5.tar", max compression
+gzip compressed data, was "kegstand-0.3.6.tar", max compression
```

## Comparing `kegstand-0.3.5.tar` & `kegstand-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.5/LICENSE
--rw-r--r--   0        0        0     1141 2023-06-20 23:30:32.094298 kegstand-0.3.5/pyproject.toml
--rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.5/src/kegstand/__init__.py
--rw-r--r--   0        0        0     3139 2023-06-20 23:29:29.942870 kegstand-0.3.5/src/kegstand/api.py
--rw-r--r--   0        0        0     9982 2023-06-20 21:54:06.742326 kegstand-0.3.5/src/kegstand/decorators.py
--rw-r--r--   0        0        0     1891 2023-06-20 17:35:15.952831 kegstand-0.3.5/src/kegstand/utils.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.5/setup.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-05 20:27:51.475886 kegstand-0.3.6/LICENSE
+-rw-r--r--   0        0        0     1141 2023-06-22 19:49:12.658333 kegstand-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      360 2023-06-20 17:35:04.354740 kegstand-0.3.6/src/kegstand/__init__.py
+-rw-r--r--   0        0        0     3139 2023-06-20 23:29:29.942870 kegstand-0.3.6/src/kegstand/api.py
+-rw-r--r--   0        0        0     9982 2023-06-20 21:54:06.742326 kegstand-0.3.6/src/kegstand/decorators.py
+-rw-r--r--   0        0        0     1960 2023-06-22 19:48:53.634934 kegstand-0.3.6/src/kegstand/utils.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 kegstand-0.3.6/setup.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 kegstand-0.3.6/PKG-INFO
```

### Comparing `kegstand-0.3.5/LICENSE` & `kegstand-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.5/pyproject.toml` & `kegstand-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kegstand"
-version = "0.3.5"
+version = "0.3.6"
 description = "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS"
 authors = ["JensRoland <mail@jensroland.com>"]
 license = "MIT"
 repository = "https://github.com/jensroland/kegstand-framework-python"
 homepage = "https://kegstand.dev"
 #readme = "README.md"
 # Keywords description https://python-poetry.org/docs/pyproject/#keywords
```

### Comparing `kegstand-0.3.5/src/kegstand/api.py` & `kegstand-0.3.6/src/kegstand/api.py`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.5/src/kegstand/decorators.py` & `kegstand-0.3.6/src/kegstand/decorators.py`

 * *Files identical despite different names*

### Comparing `kegstand-0.3.5/src/kegstand/utils.py` & `kegstand-0.3.6/src/kegstand/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,17 @@
         {"name": "api", "resources_are_public": False},
         {"name": "api/public", "resources_are_public": True},
     ]
 
     # Loop over folders in api_src_dir and list the resource modules
     for api_folder in api_folders:
         api_folder_full = os.path.join(api_src_dir, api_folder["name"])
+        if not os.path.isdir(api_folder_full):
+            continue
+
         for file_descriptor in os.listdir(api_folder_full):
             # Ignore folders, only look at files
             if os.path.isdir(os.path.join(api_folder_full, file_descriptor)):
                 continue
             # Skip dotfiles and special files
             if (
                 file_descriptor.startswith(".")
```

### Comparing `kegstand-0.3.5/setup.py` & `kegstand-0.3.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aws-lambda-powertools[aws-sdk]>=2.10.0,<3.0.0', 'pyjwt>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'kegstand',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': "The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS",
     'long_description': 'None',
     'author': 'JensRoland',
     'author_email': 'mail@jensroland.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://kegstand.dev',
```

### Comparing `kegstand-0.3.5/PKG-INFO` & `kegstand-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kegstand
-Version: 0.3.5
+Version: 0.3.6
 Summary: The Developer's Toolbelt For Accelerating Mean-Time-To-Party on AWS
 Home-page: https://kegstand.dev
 License: MIT
 Author: JensRoland
 Author-email: mail@jensroland.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

