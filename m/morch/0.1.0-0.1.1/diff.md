# Comparing `tmp/morch-0.1.0.tar.gz` & `tmp/morch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morch-0.1.0.tar", last modified: Thu Jun 22 11:41:02 2023, max compression
+gzip compressed data, was "morch-0.1.1.tar", last modified: Thu Jun 22 11:55:07 2023, max compression
```

## Comparing `morch-0.1.0.tar` & `morch-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:41:02.178967 morch-0.1.0/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 morch-0.1.0/LICENSE
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1292 2023-06-22 11:41:02.178967 morch-0.1.0/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      662 2023-06-17 11:49:33.000000 morch-0.1.0/README.md
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:41:02.178967 morch-0.1.0/morch/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 10:56:07.000000 morch-0.1.0/morch/__init__.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:41:02.178967 morch-0.1.0/morch/helpers/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      117 2023-06-22 10:06:30.000000 morch-0.1.0/morch/helpers/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 10:33:30.000000 morch-0.1.0/morch/helpers/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-19 07:46:44.000000 morch-0.1.0/morch/helpers/celery_utils.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 10:07:58.000000 morch-0.1.0/morch/helpers/handlers.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2009 2023-06-22 10:33:30.000000 morch-0.1.0/morch/helpers/repository.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 10:33:30.000000 morch-0.1.0/morch/helpers/status.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-19 07:46:44.000000 morch-0.1.0/morch/helpers/utils.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:41:02.178967 morch-0.1.0/morch/saga/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 10:06:30.000000 morch-0.1.0/morch/saga/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 10:31:23.000000 morch-0.1.0/morch/saga/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 10:29:34.000000 morch-0.1.0/morch/saga/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5357 2023-06-22 10:31:23.000000 morch-0.1.0/morch/saga/stateful.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:41:02.178967 morch-0.1.0/morch/steps/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-19 07:46:44.000000 morch-0.1.0/morch/steps/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 10:31:23.000000 morch-0.1.0/morch/steps/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 10:29:59.000000 morch-0.1.0/morch/steps/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-19 07:46:44.000000 morch-0.1.0/morch/steps/sync.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:41:02.178967 morch-0.1.0/morch.egg-info/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1292 2023-06-22 11:41:02.000000 morch-0.1.0/morch.egg-info/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      590 2023-06-22 11:41:02.000000 morch-0.1.0/morch.egg-info/SOURCES.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-06-22 11:41:02.000000 morch-0.1.0/morch.egg-info/dependency_links.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       12 2023-06-22 11:41:02.000000 morch-0.1.0/morch.egg-info/top_level.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      656 2023-06-22 11:41:02.178967 morch-0.1.0/setup.cfg
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      917 2023-06-22 11:40:45.000000 morch-0.1.0/setup.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:41:02.178967 morch-0.1.0/tests/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 morch-0.1.0/tests/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     6615 2023-06-22 11:40:45.000000 morch-0.1.0/tests/test_async_saga.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2086 2023-06-22 11:40:45.000000 morch-0.1.0/tests/test_sync_saga.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:55:07.344347 morch-0.1.1/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 morch-0.1.1/LICENSE
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1292 2023-06-22 11:55:07.344347 morch-0.1.1/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      662 2023-06-17 11:49:33.000000 morch-0.1.1/README.md
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:55:07.344347 morch-0.1.1/morch/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 10:56:07.000000 morch-0.1.1/morch/__init__.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:55:07.344347 morch-0.1.1/morch/helpers/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      117 2023-06-22 10:06:30.000000 morch-0.1.1/morch/helpers/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 10:33:30.000000 morch-0.1.1/morch/helpers/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-19 07:46:44.000000 morch-0.1.1/morch/helpers/celery_utils.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 10:07:58.000000 morch-0.1.1/morch/helpers/handlers.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2009 2023-06-22 10:33:30.000000 morch-0.1.1/morch/helpers/repository.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 10:33:30.000000 morch-0.1.1/morch/helpers/status.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-19 07:46:44.000000 morch-0.1.1/morch/helpers/utils.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:55:07.344347 morch-0.1.1/morch/saga/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 10:06:30.000000 morch-0.1.1/morch/saga/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 10:31:23.000000 morch-0.1.1/morch/saga/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 10:29:34.000000 morch-0.1.1/morch/saga/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5357 2023-06-22 10:31:23.000000 morch-0.1.1/morch/saga/stateful.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:55:07.344347 morch-0.1.1/morch/steps/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-19 07:46:44.000000 morch-0.1.1/morch/steps/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 10:31:23.000000 morch-0.1.1/morch/steps/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 10:29:59.000000 morch-0.1.1/morch/steps/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-19 07:46:44.000000 morch-0.1.1/morch/steps/sync.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:55:07.344347 morch-0.1.1/morch.egg-info/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1292 2023-06-22 11:55:07.000000 morch-0.1.1/morch.egg-info/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      618 2023-06-22 11:55:07.000000 morch-0.1.1/morch.egg-info/SOURCES.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-06-22 11:55:07.000000 morch-0.1.1/morch.egg-info/dependency_links.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       45 2023-06-22 11:55:07.000000 morch-0.1.1/morch.egg-info/requires.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       12 2023-06-22 11:55:07.000000 morch-0.1.1/morch.egg-info/top_level.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      656 2023-06-22 11:55:07.344347 morch-0.1.1/setup.cfg
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1099 2023-06-22 11:54:11.000000 morch-0.1.1/setup.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:55:07.344347 morch-0.1.1/tests/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 morch-0.1.1/tests/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     6615 2023-06-22 11:40:45.000000 morch-0.1.1/tests/test_async_saga.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2086 2023-06-22 11:40:45.000000 morch-0.1.1/tests/test_sync_saga.py
```

### Comparing `morch-0.1.0/LICENSE` & `morch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/PKG-INFO` & `morch-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morch
-Version: 0.1.0
+Version: 0.1.1
 Summary: SAGA Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/morch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/morch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
```

### Comparing `morch-0.1.0/README.md` & `morch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/helpers/asynch.py` & `morch-0.1.1/morch/helpers/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/helpers/celery_utils.py` & `morch-0.1.1/morch/helpers/celery_utils.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/helpers/handlers.py` & `morch-0.1.1/morch/helpers/handlers.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/helpers/repository.py` & `morch-0.1.1/morch/helpers/repository.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/helpers/utils.py` & `morch-0.1.1/morch/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/saga/asynch.py` & `morch-0.1.1/morch/saga/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/saga/base.py` & `morch-0.1.1/morch/saga/base.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/saga/stateful.py` & `morch-0.1.1/morch/saga/stateful.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch/steps/asynch.py` & `morch-0.1.1/morch/steps/asynch.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/morch.egg-info/PKG-INFO` & `morch-0.1.1/morch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morch
-Version: 0.1.0
+Version: 0.1.1
 Summary: SAGA Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/morch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/morch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
```

### Comparing `morch-0.1.0/morch.egg-info/SOURCES.txt` & `morch-0.1.1/morch.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 setup.cfg
 setup.py
 morch/__init__.py
 morch.egg-info/PKG-INFO
 morch.egg-info/SOURCES.txt
 morch.egg-info/dependency_links.txt
+morch.egg-info/requires.txt
 morch.egg-info/top_level.txt
 morch/helpers/__init__.py
 morch/helpers/asynch.py
 morch/helpers/celery_utils.py
 morch/helpers/handlers.py
 morch/helpers/repository.py
 morch/helpers/status.py
```

### Comparing `morch-0.1.0/setup.cfg` & `morch-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = morch
-version = 0.1.0
+version = 0.1.1
 author = Saeed Hasani Borzadaran
 author_email = hassanisaeed19@gmail.com
 description = Python Microservice Orchestrator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hasanisaeed/morch
 project_urls =
```

### Comparing `morch-0.1.0/tests/test_async_saga.py` & `morch-0.1.1/tests/test_async_saga.py`

 * *Files identical despite different names*

### Comparing `morch-0.1.0/tests/test_sync_saga.py` & `morch-0.1.1/tests/test_sync_saga.py`

 * *Files identical despite different names*

