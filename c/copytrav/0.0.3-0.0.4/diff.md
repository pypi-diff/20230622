# Comparing `tmp/copytrav-0.0.3.tar.gz` & `tmp/copytrav-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copytrav-0.0.3.tar", last modified: Wed Jun 21 17:42:18 2023, max compression
+gzip compressed data, was "copytrav-0.0.4.tar", last modified: Thu Jun 22 14:39:08 2023, max compression
```

## Comparing `copytrav-0.0.3.tar` & `copytrav-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 17:42:00.000000 copytrav-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-21 17:42:18.279693 copytrav-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-21 17:42:00.000000 copytrav-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-21 17:42:00.000000 copytrav-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:42:18.279693 copytrav-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.275693 copytrav-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.275693 copytrav-0.0.3/src/copytrav/
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.275693 copytrav-0.0.3/src/copytrav/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav/data/one/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/one/data1.rst
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/one/data1.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav/data/two/
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/data2.rst
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/data2.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav/data/two/even_more_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/even_more_data/data3.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:00.000000 copytrav-0.0.3/src/copytrav/data/two/even_more_data/data3.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/src/copytrav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-21 17:42:18.000000 copytrav-0.0.3/src/copytrav.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:42:18.279693 copytrav-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-21 17:42:00.000000 copytrav-0.0.3/tests/test_copy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.448860 copytrav-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 14:38:42.000000 copytrav-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-22 14:39:08.448860 copytrav-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-22 14:38:42.000000 copytrav-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-22 14:38:42.000000 copytrav-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:39:08.448860 copytrav-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.444860 copytrav-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.448860 copytrav-0.0.4/src/copytrav/
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-22 14:38:42.000000 copytrav-0.0.4/src/copytrav/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.444860 copytrav-0.0.4/src/copytrav/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.448860 copytrav-0.0.4/src/copytrav/data/one/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-22 14:38:42.000000 copytrav-0.0.4/src/copytrav/data/one/data1.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-22 14:38:42.000000 copytrav-0.0.4/src/copytrav/data/one/data1.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.448860 copytrav-0.0.4/src/copytrav/data/two/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-22 14:38:42.000000 copytrav-0.0.4/src/copytrav/data/two/data2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-22 14:38:42.000000 copytrav-0.0.4/src/copytrav/data/two/data2.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.448860 copytrav-0.0.4/src/copytrav/data/two/even_more_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:38:42.000000 copytrav-0.0.4/src/copytrav/data/two/even_more_data/data3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:38:42.000000 copytrav-0.0.4/src/copytrav/data/two/even_more_data/data3.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.448860 copytrav-0.0.4/src/copytrav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-06-22 14:39:08.000000 copytrav-0.0.4/src/copytrav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-22 14:39:08.000000 copytrav-0.0.4/src/copytrav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:39:08.000000 copytrav-0.0.4/src/copytrav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 14:39:08.000000 copytrav-0.0.4/src/copytrav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 14:39:08.000000 copytrav-0.0.4/src/copytrav.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:39:08.448860 copytrav-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-22 14:38:42.000000 copytrav-0.0.4/tests/test_copy.py
```

### Comparing `copytrav-0.0.3/LICENSE` & `copytrav-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `copytrav-0.0.3/PKG-INFO` & `copytrav-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: copytrav
-Version: 0.0.3
+Version: 0.0.4
 Summary: Copy traversables as directories.
 Author-email: Owen Shepherd <oshepengineering@gmail.com>
 Project-URL: Homepage, https://github.com/OwenShepherd/copytrav
+Project-URL: Documentation, https://OwenShepherd.github.io/copytrav
 Project-URL: Bug Tracker, https://github.com/OwenShepherd/copytrav/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `copytrav-0.0.3/README.md` & `copytrav-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `copytrav-0.0.3/pyproject.toml` & `copytrav-0.0.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "copytrav"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name="Owen Shepherd", email="oshepengineering@gmail.com" },
 ]
 description = "Copy traversables as directories."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -17,14 +17,15 @@
     "sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-mdinclude",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/OwenShepherd/copytrav"
+"Documentation" = "https://OwenShepherd.github.io/copytrav"
 "Bug Tracker" = "https://github.com/OwenShepherd/copytrav/issues"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.package-data]
```

### Comparing `copytrav-0.0.3/src/copytrav/__init__.py` & `copytrav-0.0.4/src/copytrav/__init__.py`

 * *Files identical despite different names*

### Comparing `copytrav-0.0.3/src/copytrav.egg-info/PKG-INFO` & `copytrav-0.0.4/src/copytrav.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: copytrav
-Version: 0.0.3
+Version: 0.0.4
 Summary: Copy traversables as directories.
 Author-email: Owen Shepherd <oshepengineering@gmail.com>
 Project-URL: Homepage, https://github.com/OwenShepherd/copytrav
+Project-URL: Documentation, https://OwenShepherd.github.io/copytrav
 Project-URL: Bug Tracker, https://github.com/OwenShepherd/copytrav/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `copytrav-0.0.3/tests/test_copy.py` & `copytrav-0.0.4/tests/test_copy.py`

 * *Files identical despite different names*

