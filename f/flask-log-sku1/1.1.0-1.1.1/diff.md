# Comparing `tmp/flask_log_sku1-1.1.0.tar.gz` & `tmp/flask_log_sku1-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_log_sku1-1.1.0.tar", last modified: Fri Mar 10 12:54:02 2023, max compression
+gzip compressed data, was "flask_log_sku1-1.1.1.tar", last modified: Thu Jun 22 06:18:32 2023, max compression
```

## Comparing `flask_log_sku1-1.1.0.tar` & `flask_log_sku1-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:54:02.229917 flask_log_sku1-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-10 12:53:52.000000 flask_log_sku1-1.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:54:02.225917 flask_log_sku1-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:54:02.225917 flask_log_sku1-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-03-10 12:53:52.000000 flask_log_sku1-1.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-03-10 12:53:52.000000 flask_log_sku1-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-10 12:54:02.229917 flask_log_sku1-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-10 12:53:52.000000 flask_log_sku1-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-10 12:53:52.000000 flask_log_sku1-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-10 12:54:02.229917 flask_log_sku1-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:54:02.225917 flask_log_sku1-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:54:02.229917 flask_log_sku1-1.1.0/src/flask_log_sku1/
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-03-10 12:53:52.000000 flask_log_sku1-1.1.0/src/flask_log_sku1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 12:54:02.229917 flask_log_sku1-1.1.0/src/flask_log_sku1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-03-10 12:54:02.000000 flask_log_sku1-1.1.0/src/flask_log_sku1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-10 12:54:02.000000 flask_log_sku1-1.1.0/src/flask_log_sku1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 12:54:02.000000 flask_log_sku1-1.1.0/src/flask_log_sku1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-10 12:54:02.000000 flask_log_sku1-1.1.0/src/flask_log_sku1.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-10 12:54:02.000000 flask_log_sku1-1.1.0/src/flask_log_sku1.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:18:32.532721 flask_log_sku1-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 06:18:22.000000 flask_log_sku1-1.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:18:32.528721 flask_log_sku1-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:18:32.532721 flask_log_sku1-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-22 06:18:22.000000 flask_log_sku1-1.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 06:18:22.000000 flask_log_sku1-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-22 06:18:32.532721 flask_log_sku1-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 06:18:22.000000 flask_log_sku1-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 06:18:22.000000 flask_log_sku1-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-22 06:18:32.536721 flask_log_sku1-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:18:32.528721 flask_log_sku1-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:18:32.532721 flask_log_sku1-1.1.1/src/flask_log_sku1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-22 06:18:22.000000 flask_log_sku1-1.1.1/src/flask_log_sku1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:18:32.532721 flask_log_sku1-1.1.1/src/flask_log_sku1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-22 06:18:32.000000 flask_log_sku1-1.1.1/src/flask_log_sku1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 06:18:32.000000 flask_log_sku1-1.1.1/src/flask_log_sku1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:18:32.000000 flask_log_sku1-1.1.1/src/flask_log_sku1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 06:18:32.000000 flask_log_sku1-1.1.1/src/flask_log_sku1.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 06:18:32.000000 flask_log_sku1-1.1.1/src/flask_log_sku1.egg-info/top_level.txt
```

### Comparing `flask_log_sku1-1.1.0/.github/workflows/python-publish.yml` & `flask_log_sku1-1.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `flask_log_sku1-1.1.0/LICENSE` & `flask_log_sku1-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_log_sku1-1.1.0/PKG-INFO` & `flask_log_sku1-1.1.1/src/flask_log_sku1.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: flask_log_sku1
-Version: 1.1.0
+Name: flask-log-sku1
+Version: 1.1.1
 Summary: Flask log output
 Home-page: https://github.com/Skulldorom/flask_log_sku1
 Author: Skulldorom
 Author-email: Skulldorom@gmail.com
 Project-URL: Bug Tracker, https://github.com/Skulldorom/flask_log_sku1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flask_log_sku1
 
 Simple print formatter
 
@@ -25,14 +25,17 @@
 
 example:
 
 ```
 from flask_log_sku1 import log
 
 log("Hello world").success()
+log("INFO").info()
+log("WARNING").warning()
+log("ERROR").error()
 ```
 
 options for log() are:
 success()
 info()
 warning()
 error()
```

### Comparing `flask_log_sku1-1.1.0/setup.cfg` & `flask_log_sku1-1.1.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.11
+python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	gha_python_packaging_demo = gha_python_packaging_demo.app:entry_point
```

### Comparing `flask_log_sku1-1.1.0/src/flask_log_sku1/__init__.py` & `flask_log_sku1-1.1.1/src/flask_log_sku1/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_log_sku1-1.1.0/src/flask_log_sku1.egg-info/PKG-INFO` & `flask_log_sku1-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
-Name: flask-log-sku1
-Version: 1.1.0
+Name: flask_log_sku1
+Version: 1.1.1
 Summary: Flask log output
 Home-page: https://github.com/Skulldorom/flask_log_sku1
 Author: Skulldorom
 Author-email: Skulldorom@gmail.com
 Project-URL: Bug Tracker, https://github.com/Skulldorom/flask_log_sku1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flask_log_sku1
 
 Simple print formatter
 
@@ -25,14 +25,17 @@
 
 example:
 
 ```
 from flask_log_sku1 import log
 
 log("Hello world").success()
+log("INFO").info()
+log("WARNING").warning()
+log("ERROR").error()
 ```
 
 options for log() are:
 success()
 info()
 warning()
 error()
```

