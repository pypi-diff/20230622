# Comparing `tmp/autodistill_detic-0.1.3.tar.gz` & `tmp/autodistill_detic-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_detic-0.1.3.tar", last modified: Tue Jun 20 15:58:49 2023, max compression
+gzip compressed data, was "autodistill_detic-0.1.4.tar", last modified: Thu Jun 22 21:56:17 2023, max compression
```

## Comparing `autodistill_detic-0.1.3.tar` & `autodistill_detic-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/
--rw-r--r--   0 arty      (1019) arty      (1020)     1055 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/LICENSE.md
--rw-r--r--   0 arty      (1019) arty      (1020)     2297 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/PKG-INFO
--rw-r--r--   0 arty      (1019) arty      (1020)     1821 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/README.md
-drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.590548 autodistill_detic-0.1.3/autodistill_detic/
--rw-r--r--   0 arty      (1019) arty      (1020)       71 2023-06-20 15:57:28.000000 autodistill_detic-0.1.3/autodistill_detic/__init__.py
--rw-r--r--   0 arty      (1019) arty      (1020)     3841 2023-06-14 10:46:00.000000 autodistill_detic-0.1.3/autodistill_detic/detic_model.py
-drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/autodistill_detic.egg-info/
--rw-r--r--   0 arty      (1019) arty      (1020)     2297 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/PKG-INFO
--rw-r--r--   0 arty      (1019) arty      (1020)      344 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/SOURCES.txt
--rw-r--r--   0 arty      (1019) arty      (1020)        1 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/dependency_links.txt
--rw-r--r--   0 arty      (1019) arty      (1020)       89 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/requires.txt
--rw-r--r--   0 arty      (1019) arty      (1020)       22 2023-06-20 15:58:49.000000 autodistill_detic-0.1.3/autodistill_detic.egg-info/top_level.txt
--rw-r--r--   0 arty      (1019) arty      (1020)       38 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/setup.cfg
--rw-r--r--   0 arty      (1019) arty      (1020)     1975 2023-06-14 10:49:59.000000 autodistill_detic-0.1.3/setup.py
-drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/src/
--rw-r--r--   0 arty      (1019) arty      (1020)       22 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/src/__init__.py
--rw-r--r--   0 arty      (1019) arty      (1020)       39 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/src/hello.py
-drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-20 15:58:49.594548 autodistill_detic-0.1.3/test/
--rw-r--r--   0 arty      (1019) arty      (1020)       91 2023-06-08 22:41:53.000000 autodistill_detic-0.1.3/test/test_hello.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-22 21:56:17.730375 autodistill_detic-0.1.4/
+-rw-r--r--   0 arty      (1019) arty      (1020)     1055 2023-06-08 22:41:53.000000 autodistill_detic-0.1.4/LICENSE.md
+-rw-r--r--   0 arty      (1019) arty      (1020)     2297 2023-06-22 21:56:17.730375 autodistill_detic-0.1.4/PKG-INFO
+-rw-r--r--   0 arty      (1019) arty      (1020)     1821 2023-06-22 19:19:21.000000 autodistill_detic-0.1.4/README.md
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-22 21:56:17.730375 autodistill_detic-0.1.4/autodistill_detic/
+-rw-r--r--   0 arty      (1019) arty      (1020)       71 2023-06-22 21:55:31.000000 autodistill_detic-0.1.4/autodistill_detic/__init__.py
+-rw-r--r--   0 arty      (1019) arty      (1020)     5035 2023-06-22 19:06:41.000000 autodistill_detic-0.1.4/autodistill_detic/detic_model.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-22 21:56:17.730375 autodistill_detic-0.1.4/autodistill_detic.egg-info/
+-rw-r--r--   0 arty      (1019) arty      (1020)     2297 2023-06-22 21:56:17.000000 autodistill_detic-0.1.4/autodistill_detic.egg-info/PKG-INFO
+-rw-r--r--   0 arty      (1019) arty      (1020)      344 2023-06-22 21:56:17.000000 autodistill_detic-0.1.4/autodistill_detic.egg-info/SOURCES.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)        1 2023-06-22 21:56:17.000000 autodistill_detic-0.1.4/autodistill_detic.egg-info/dependency_links.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)       89 2023-06-22 21:56:17.000000 autodistill_detic-0.1.4/autodistill_detic.egg-info/requires.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)       22 2023-06-22 21:56:17.000000 autodistill_detic-0.1.4/autodistill_detic.egg-info/top_level.txt
+-rw-r--r--   0 arty      (1019) arty      (1020)       38 2023-06-22 21:56:17.730375 autodistill_detic-0.1.4/setup.cfg
+-rw-r--r--   0 arty      (1019) arty      (1020)     1169 2023-06-22 18:40:39.000000 autodistill_detic-0.1.4/setup.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-22 21:56:17.730375 autodistill_detic-0.1.4/src/
+-rw-r--r--   0 arty      (1019) arty      (1020)       22 2023-06-08 22:41:53.000000 autodistill_detic-0.1.4/src/__init__.py
+-rw-r--r--   0 arty      (1019) arty      (1020)       39 2023-06-08 22:41:53.000000 autodistill_detic-0.1.4/src/hello.py
+drwxr-xr-x   0 arty      (1019) arty      (1020)        0 2023-06-22 21:56:17.730375 autodistill_detic-0.1.4/test/
+-rw-r--r--   0 arty      (1019) arty      (1020)       91 2023-06-08 22:41:53.000000 autodistill_detic-0.1.4/test/test_hello.py
```

### Comparing `autodistill_detic-0.1.3/LICENSE.md` & `autodistill_detic-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autodistill_detic-0.1.3/PKG-INFO` & `autodistill_detic-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill_detic
-Version: 0.1.3
+Version: 0.1.4
 Summary: DETIC module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-detic
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_detic-0.1.3/README.md` & `autodistill_detic-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_detic-0.1.3/autodistill_detic.egg-info/PKG-INFO` & `autodistill_detic-0.1.4/autodistill_detic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-detic
-Version: 0.1.3
+Version: 0.1.4
 Summary: DETIC module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-detic
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

