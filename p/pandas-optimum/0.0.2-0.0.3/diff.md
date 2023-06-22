# Comparing `tmp/pandas-optimum-0.0.2.tar.gz` & `tmp/pandas-optimum-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-optimum-0.0.2.tar", last modified: Thu Jun 22 19:16:35 2023, max compression
+gzip compressed data, was "pandas-optimum-0.0.3.tar", last modified: Thu Jun 22 19:25:37 2023, max compression
```

## Comparing `pandas-optimum-0.0.2.tar` & `pandas-optimum-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:16:35.015344 pandas-optimum-0.0.2/
--rw-r--r--   0 rajan      (501) staff       (20)     3078 2023-06-22 17:49:44.000000 pandas-optimum-0.0.2/.gitignore
--rw-r--r--   0 rajan      (501) staff       (20)     1498 2023-06-22 17:49:44.000000 pandas-optimum-0.0.2/LICENSE
--rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:16:35.015441 pandas-optimum-0.0.2/PKG-INFO
--rw-r--r--   0 rajan      (501) staff       (20)       63 2023-06-22 17:49:44.000000 pandas-optimum-0.0.2/README.md
--rw-r--r--   0 rajan      (501) staff       (20)       95 2023-06-22 19:00:29.000000 pandas-optimum-0.0.2/pyproject.toml
--rw-r--r--   0 rajan      (501) staff       (20)      733 2023-06-22 19:16:35.015767 pandas-optimum-0.0.2/setup.cfg
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:16:35.013304 pandas-optimum-0.0.2/src/
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:16:35.014242 pandas-optimum-0.0.2/src/pandas-optimum/
--rw-r--r--   0 rajan      (501) staff       (20)        0 2023-06-22 18:36:36.000000 pandas-optimum-0.0.2/src/pandas-optimum/__init__.py
--rw-r--r--   0 rajan      (501) staff       (20)       20 2023-06-22 18:37:59.000000 pandas-optimum-0.0.2/src/pandas-optimum/p_op.py
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:16:35.015224 pandas-optimum-0.0.2/src/pandas_optimum.egg-info/
--rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:16:34.000000 pandas-optimum-0.0.2/src/pandas_optimum.egg-info/PKG-INFO
--rw-r--r--   0 rajan      (501) staff       (20)      320 2023-06-22 19:16:35.000000 pandas-optimum-0.0.2/src/pandas_optimum.egg-info/SOURCES.txt
--rw-r--r--   0 rajan      (501) staff       (20)        1 2023-06-22 19:16:34.000000 pandas-optimum-0.0.2/src/pandas_optimum.egg-info/dependency_links.txt
--rw-r--r--   0 rajan      (501) staff       (20)       30 2023-06-22 19:16:34.000000 pandas-optimum-0.0.2/src/pandas_optimum.egg-info/requires.txt
--rw-r--r--   0 rajan      (501) staff       (20)       15 2023-06-22 19:16:34.000000 pandas-optimum-0.0.2/src/pandas_optimum.egg-info/top_level.txt
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:25:37.560908 pandas-optimum-0.0.3/
+-rw-r--r--   0 rajan      (501) staff       (20)     3078 2023-06-22 17:49:44.000000 pandas-optimum-0.0.3/.gitignore
+-rw-r--r--   0 rajan      (501) staff       (20)     1498 2023-06-22 17:49:44.000000 pandas-optimum-0.0.3/LICENSE
+-rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:25:37.561006 pandas-optimum-0.0.3/PKG-INFO
+-rw-r--r--   0 rajan      (501) staff       (20)       63 2023-06-22 17:49:44.000000 pandas-optimum-0.0.3/README.md
+-rw-r--r--   0 rajan      (501) staff       (20)       95 2023-06-22 19:00:29.000000 pandas-optimum-0.0.3/pyproject.toml
+-rw-r--r--   0 rajan      (501) staff       (20)      733 2023-06-22 19:25:37.561332 pandas-optimum-0.0.3/setup.cfg
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:25:37.559229 pandas-optimum-0.0.3/src/
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:25:37.560100 pandas-optimum-0.0.3/src/pandas-optimum/
+-rw-r--r--   0 rajan      (501) staff       (20)        0 2023-06-22 18:36:36.000000 pandas-optimum-0.0.3/src/pandas-optimum/__init__.py
+-rw-r--r--   0 rajan      (501) staff       (20)       20 2023-06-22 19:23:19.000000 pandas-optimum-0.0.3/src/pandas-optimum/panda_optimum.py
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:25:37.560749 pandas-optimum-0.0.3/src/pandas_optimum.egg-info/
+-rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:25:37.000000 pandas-optimum-0.0.3/src/pandas_optimum.egg-info/PKG-INFO
+-rw-r--r--   0 rajan      (501) staff       (20)      329 2023-06-22 19:25:37.000000 pandas-optimum-0.0.3/src/pandas_optimum.egg-info/SOURCES.txt
+-rw-r--r--   0 rajan      (501) staff       (20)        1 2023-06-22 19:25:37.000000 pandas-optimum-0.0.3/src/pandas_optimum.egg-info/dependency_links.txt
+-rw-r--r--   0 rajan      (501) staff       (20)       30 2023-06-22 19:25:37.000000 pandas-optimum-0.0.3/src/pandas_optimum.egg-info/requires.txt
+-rw-r--r--   0 rajan      (501) staff       (20)       15 2023-06-22 19:25:37.000000 pandas-optimum-0.0.3/src/pandas_optimum.egg-info/top_level.txt
```

### Comparing `pandas-optimum-0.0.2/.gitignore` & `pandas-optimum-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pandas-optimum-0.0.2/LICENSE` & `pandas-optimum-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-optimum-0.0.2/PKG-INFO` & `pandas-optimum-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-optimum
-Version: 0.0.2
+Version: 0.0.3
 Summary: Optimised pandas, Best practices in-built
 Home-page: https://github.com/irajankumar/pandas-optimum
 Author: Rajan Kumar
 Project-URL: Bug Tracker, https://github.com/irajankumar/pandas-optimum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandas-optimum-0.0.2/setup.cfg` & `pandas-optimum-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pandas-optimum
-version = 0.0.2
+version = 0.0.3
 author = Rajan Kumar
 description = Optimised pandas, Best practices in-built
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/irajankumar/pandas-optimum
 project_urls = 
 	Bug Tracker = https://github.com/irajankumar/pandas-optimum/issues
```

### Comparing `pandas-optimum-0.0.2/src/pandas_optimum.egg-info/PKG-INFO` & `pandas-optimum-0.0.3/src/pandas_optimum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-optimum
-Version: 0.0.2
+Version: 0.0.3
 Summary: Optimised pandas, Best practices in-built
 Home-page: https://github.com/irajankumar/pandas-optimum
 Author: Rajan Kumar
 Project-URL: Bug Tracker, https://github.com/irajankumar/pandas-optimum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

