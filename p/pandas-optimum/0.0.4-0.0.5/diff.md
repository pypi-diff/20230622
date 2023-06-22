# Comparing `tmp/pandas-optimum-0.0.4.tar.gz` & `tmp/pandas-optimum-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-optimum-0.0.4.tar", last modified: Thu Jun 22 19:29:29 2023, max compression
+gzip compressed data, was "pandas-optimum-0.0.5.tar", last modified: Thu Jun 22 19:32:50 2023, max compression
```

## Comparing `pandas-optimum-0.0.4.tar` & `pandas-optimum-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:29:29.300589 pandas-optimum-0.0.4/
--rw-r--r--   0 rajan      (501) staff       (20)     3078 2023-06-22 17:49:44.000000 pandas-optimum-0.0.4/.gitignore
--rw-r--r--   0 rajan      (501) staff       (20)     1498 2023-06-22 17:49:44.000000 pandas-optimum-0.0.4/LICENSE
--rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:29:29.300683 pandas-optimum-0.0.4/PKG-INFO
--rw-r--r--   0 rajan      (501) staff       (20)       63 2023-06-22 17:49:44.000000 pandas-optimum-0.0.4/README.md
--rw-r--r--   0 rajan      (501) staff       (20)       95 2023-06-22 19:00:29.000000 pandas-optimum-0.0.4/pyproject.toml
--rw-r--r--   0 rajan      (501) staff       (20)      733 2023-06-22 19:29:29.301010 pandas-optimum-0.0.4/setup.cfg
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:29:29.298297 pandas-optimum-0.0.4/src/
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:29:29.299520 pandas-optimum-0.0.4/src/pandas_optimum/
--rw-r--r--   0 rajan      (501) staff       (20)        0 2023-06-22 18:36:36.000000 pandas-optimum-0.0.4/src/pandas_optimum/__init__.py
--rw-r--r--   0 rajan      (501) staff       (20)       20 2023-06-22 19:23:19.000000 pandas-optimum-0.0.4/src/pandas_optimum/panda_optimum.py
-drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:29:29.300449 pandas-optimum-0.0.4/src/pandas_optimum.egg-info/
--rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:29:29.000000 pandas-optimum-0.0.4/src/pandas_optimum.egg-info/PKG-INFO
--rw-r--r--   0 rajan      (501) staff       (20)      329 2023-06-22 19:29:29.000000 pandas-optimum-0.0.4/src/pandas_optimum.egg-info/SOURCES.txt
--rw-r--r--   0 rajan      (501) staff       (20)        1 2023-06-22 19:29:29.000000 pandas-optimum-0.0.4/src/pandas_optimum.egg-info/dependency_links.txt
--rw-r--r--   0 rajan      (501) staff       (20)       30 2023-06-22 19:29:29.000000 pandas-optimum-0.0.4/src/pandas_optimum.egg-info/requires.txt
--rw-r--r--   0 rajan      (501) staff       (20)       15 2023-06-22 19:29:29.000000 pandas-optimum-0.0.4/src/pandas_optimum.egg-info/top_level.txt
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:32:50.583678 pandas-optimum-0.0.5/
+-rw-r--r--   0 rajan      (501) staff       (20)     3078 2023-06-22 17:49:44.000000 pandas-optimum-0.0.5/.gitignore
+-rw-r--r--   0 rajan      (501) staff       (20)     1498 2023-06-22 17:49:44.000000 pandas-optimum-0.0.5/LICENSE
+-rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:32:50.583761 pandas-optimum-0.0.5/PKG-INFO
+-rw-r--r--   0 rajan      (501) staff       (20)       63 2023-06-22 17:49:44.000000 pandas-optimum-0.0.5/README.md
+-rw-r--r--   0 rajan      (501) staff       (20)       95 2023-06-22 19:00:29.000000 pandas-optimum-0.0.5/pyproject.toml
+-rw-r--r--   0 rajan      (501) staff       (20)      733 2023-06-22 19:32:50.584078 pandas-optimum-0.0.5/setup.cfg
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:32:50.581659 pandas-optimum-0.0.5/src/
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:32:50.582705 pandas-optimum-0.0.5/src/pandas_optimum/
+-rw-r--r--   0 rajan      (501) staff       (20)        0 2023-06-22 18:36:36.000000 pandas-optimum-0.0.5/src/pandas_optimum/__init__.py
+-rw-r--r--   0 rajan      (501) staff       (20)       20 2023-06-22 19:32:00.000000 pandas-optimum-0.0.5/src/pandas_optimum/pandas_optimum.py
+drwxr-xr-x   0 rajan      (501) staff       (20)        0 2023-06-22 19:32:50.583536 pandas-optimum-0.0.5/src/pandas_optimum.egg-info/
+-rw-r--r--   0 rajan      (501) staff       (20)      560 2023-06-22 19:32:50.000000 pandas-optimum-0.0.5/src/pandas_optimum.egg-info/PKG-INFO
+-rw-r--r--   0 rajan      (501) staff       (20)      330 2023-06-22 19:32:50.000000 pandas-optimum-0.0.5/src/pandas_optimum.egg-info/SOURCES.txt
+-rw-r--r--   0 rajan      (501) staff       (20)        1 2023-06-22 19:32:50.000000 pandas-optimum-0.0.5/src/pandas_optimum.egg-info/dependency_links.txt
+-rw-r--r--   0 rajan      (501) staff       (20)       30 2023-06-22 19:32:50.000000 pandas-optimum-0.0.5/src/pandas_optimum.egg-info/requires.txt
+-rw-r--r--   0 rajan      (501) staff       (20)       15 2023-06-22 19:32:50.000000 pandas-optimum-0.0.5/src/pandas_optimum.egg-info/top_level.txt
```

### Comparing `pandas-optimum-0.0.4/.gitignore` & `pandas-optimum-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `pandas-optimum-0.0.4/LICENSE` & `pandas-optimum-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-optimum-0.0.4/PKG-INFO` & `pandas-optimum-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-optimum
-Version: 0.0.4
+Version: 0.0.5
 Summary: Optimised pandas, Best practices in-built
 Home-page: https://github.com/irajankumar/pandas-optimum
 Author: Rajan Kumar
 Project-URL: Bug Tracker, https://github.com/irajankumar/pandas-optimum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `pandas-optimum-0.0.4/setup.cfg` & `pandas-optimum-0.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pandas-optimum
-version = 0.0.4
+version = 0.0.5
 author = Rajan Kumar
 description = Optimised pandas, Best practices in-built
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/irajankumar/pandas-optimum
 project_urls = 
 	Bug Tracker = https://github.com/irajankumar/pandas-optimum/issues
```

### Comparing `pandas-optimum-0.0.4/src/pandas_optimum.egg-info/PKG-INFO` & `pandas-optimum-0.0.5/src/pandas_optimum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-optimum
-Version: 0.0.4
+Version: 0.0.5
 Summary: Optimised pandas, Best practices in-built
 Home-page: https://github.com/irajankumar/pandas-optimum
 Author: Rajan Kumar
 Project-URL: Bug Tracker, https://github.com/irajankumar/pandas-optimum/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

