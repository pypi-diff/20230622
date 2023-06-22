# Comparing `tmp/sparrow-cvat-0.3.2.dev1679080043.tar.gz` & `tmp/sparrow-cvat-0.3.2.dev1687448436.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrow-cvat-0.3.2.dev1679080043.tar", last modified: Fri Mar 17 19:07:34 2023, max compression
+gzip compressed data, was "sparrow-cvat-0.3.2.dev1687448436.tar", last modified: Thu Jun 22 15:40:48 2023, max compression
```

## Comparing `sparrow-cvat-0.3.2.dev1679080043.tar` & `sparrow-cvat-0.3.2.dev1687448436.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:07:34.899889 sparrow-cvat-0.3.2.dev1679080043/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-17 19:07:34.899889 sparrow-cvat-0.3.2.dev1679080043/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-17 19:07:34.899889 sparrow-cvat-0.3.2.dev1679080043/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:07:34.895889 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:07:34.899889 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-17 19:06:01.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 19:07:34.895889 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-17 19:07:34.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-03-17 19:07:34.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 19:07:34.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-17 19:07:34.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-17 19:07:34.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-17 19:07:34.000000 sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:40:48.362513 sparrow-cvat-0.3.2.dev1687448436/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 15:40:48.362513 sparrow-cvat-0.3.2.dev1687448436/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-22 15:40:48.366513 sparrow-cvat-0.3.2.dev1687448436/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:40:48.362513 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:40:48.362513 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 15:39:11.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:40:48.362513 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 15:40:48.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 15:40:48.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:40:48.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 15:40:48.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 15:40:48.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 15:40:48.000000 sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/top_level.txt
```

### Comparing `sparrow-cvat-0.3.2.dev1679080043/LICENSE` & `sparrow-cvat-0.3.2.dev1687448436/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/setup.cfg` & `sparrow-cvat-0.3.2.dev1687448436/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sparrow-cvat
-version = 0.3.2.dev1679080043
+version = 0.3.2.dev1687448436
 author = Sparrow Computing
 author_email = ben@sparrow.dev
 
 [options]
 install_requires = 
 	av
 	datumaro<1.0.0
```

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/__main__.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/__main__.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/annotations.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/annotations.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/auth.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/auth.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/core.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/core.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/create.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/create.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/dataset_manifest/utils.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/dataset_manifest/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/jobs.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/jobs.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat/tasks.py` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat/tasks.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.3.2.dev1679080043/sparrow_cvat.egg-info/SOURCES.txt` & `sparrow-cvat-0.3.2.dev1687448436/sparrow_cvat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 LICENSE
+README.md
 setup.cfg
 setup.py
 sparrow_cvat/__init__.py
 sparrow_cvat/__main__.py
 sparrow_cvat/annotations.py
 sparrow_cvat/auth.py
 sparrow_cvat/jobs.py
```

