# Comparing `tmp/micro_orch-0.1.1.tar.gz` & `tmp/micro_orch-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micro_orch-0.1.1.tar", last modified: Thu Jun 22 11:32:06 2023, max compression
+gzip compressed data, was "micro_orch-0.1.2.tar", last modified: Thu Jun 22 11:37:13 2023, max compression
```

## Comparing `micro_orch-0.1.1.tar` & `micro_orch-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:32:06.625857 micro_orch-0.1.1/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 micro_orch-0.1.1/LICENSE
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1302 2023-06-22 11:32:06.625857 micro_orch-0.1.1/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      662 2023-06-17 11:49:33.000000 micro_orch-0.1.1/README.md
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:32:06.625857 micro_orch-0.1.1/micro_orch.egg-info/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1302 2023-06-22 11:32:06.000000 micro_orch-0.1.1/micro_orch.egg-info/PKG-INFO
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      578 2023-06-22 11:32:06.000000 micro_orch-0.1.1/micro_orch.egg-info/SOURCES.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-06-22 11:32:06.000000 micro_orch-0.1.1/micro_orch.egg-info/dependency_links.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       10 2023-06-22 11:32:06.000000 micro_orch-0.1.1/micro_orch.egg-info/top_level.txt
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      671 2023-06-22 11:32:06.625857 micro_orch-0.1.1/setup.cfg
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      927 2023-06-22 11:31:57.000000 micro_orch-0.1.1/setup.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:32:06.625857 micro_orch-0.1.1/src/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 10:56:07.000000 micro_orch-0.1.1/src/__init__.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:32:06.625857 micro_orch-0.1.1/src/helpers/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      117 2023-06-22 10:06:30.000000 micro_orch-0.1.1/src/helpers/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 10:33:30.000000 micro_orch-0.1.1/src/helpers/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-19 07:46:44.000000 micro_orch-0.1.1/src/helpers/celery_utils.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 10:07:58.000000 micro_orch-0.1.1/src/helpers/handlers.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2009 2023-06-22 10:33:30.000000 micro_orch-0.1.1/src/helpers/repository.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 10:33:30.000000 micro_orch-0.1.1/src/helpers/status.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-19 07:46:44.000000 micro_orch-0.1.1/src/helpers/utils.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:32:06.625857 micro_orch-0.1.1/src/saga/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 10:06:30.000000 micro_orch-0.1.1/src/saga/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 10:31:23.000000 micro_orch-0.1.1/src/saga/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 10:29:34.000000 micro_orch-0.1.1/src/saga/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     5357 2023-06-22 10:31:23.000000 micro_orch-0.1.1/src/saga/stateful.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:32:06.625857 micro_orch-0.1.1/src/steps/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-19 07:46:44.000000 micro_orch-0.1.1/src/steps/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 10:31:23.000000 micro_orch-0.1.1/src/steps/asynch.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 10:29:59.000000 micro_orch-0.1.1/src/steps/base.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-19 07:46:44.000000 micro_orch-0.1.1/src/steps/sync.py
-drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:32:06.625857 micro_orch-0.1.1/tests/
--rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 micro_orch-0.1.1/tests/__init__.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     6633 2023-06-22 10:45:12.000000 micro_orch-0.1.1/tests/test_async_saga.py
--rw-rw-r--   0 saeed     (1000) saeed     (1000)     2084 2023-06-22 10:09:05.000000 micro_orch-0.1.1/tests/test_sync_saga.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:37:13.196879 micro_orch-0.1.2/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1086 2023-06-17 07:10:20.000000 micro_orch-0.1.2/LICENSE
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1302 2023-06-22 11:37:13.196879 micro_orch-0.1.2/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      662 2023-06-17 11:49:33.000000 micro_orch-0.1.2/README.md
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:37:13.196879 micro_orch-0.1.2/micro_orch/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      126 2023-06-22 10:56:07.000000 micro_orch-0.1.2/micro_orch/__init__.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:37:13.196879 micro_orch-0.1.2/micro_orch/helpers/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      117 2023-06-22 10:06:30.000000 micro_orch-0.1.2/micro_orch/helpers/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2259 2023-06-22 10:33:30.000000 micro_orch-0.1.2/micro_orch/helpers/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      640 2023-06-19 07:46:44.000000 micro_orch-0.1.2/micro_orch/helpers/celery_utils.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2119 2023-06-22 10:07:58.000000 micro_orch-0.1.2/micro_orch/helpers/handlers.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2009 2023-06-22 10:33:30.000000 micro_orch-0.1.2/micro_orch/helpers/repository.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      145 2023-06-22 10:33:30.000000 micro_orch-0.1.2/micro_orch/helpers/status.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1007 2023-06-19 07:46:44.000000 micro_orch-0.1.2/micro_orch/helpers/utils.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:37:13.196879 micro_orch-0.1.2/micro_orch/saga/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       66 2023-06-22 10:06:30.000000 micro_orch-0.1.2/micro_orch/saga/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     3687 2023-06-22 10:31:23.000000 micro_orch-0.1.2/micro_orch/saga/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5218 2023-06-22 10:29:34.000000 micro_orch-0.1.2/micro_orch/saga/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     5357 2023-06-22 10:31:23.000000 micro_orch-0.1.2/micro_orch/saga/stateful.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:37:13.196879 micro_orch-0.1.2/micro_orch/steps/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       62 2023-06-19 07:46:44.000000 micro_orch-0.1.2/micro_orch/steps/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      563 2023-06-22 10:31:23.000000 micro_orch-0.1.2/micro_orch/steps/asynch.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      361 2023-06-22 10:29:59.000000 micro_orch-0.1.2/micro_orch/steps/base.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       88 2023-06-19 07:46:44.000000 micro_orch-0.1.2/micro_orch/steps/sync.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:37:13.196879 micro_orch-0.1.2/micro_orch.egg-info/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     1302 2023-06-22 11:37:13.000000 micro_orch-0.1.2/micro_orch.egg-info/PKG-INFO
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      690 2023-06-22 11:37:13.000000 micro_orch-0.1.2/micro_orch.egg-info/SOURCES.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        1 2023-06-22 11:37:13.000000 micro_orch-0.1.2/micro_orch.egg-info/dependency_links.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)       17 2023-06-22 11:37:13.000000 micro_orch-0.1.2/micro_orch.egg-info/top_level.txt
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      671 2023-06-22 11:37:13.196879 micro_orch-0.1.2/setup.cfg
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)      927 2023-06-22 11:37:10.000000 micro_orch-0.1.2/setup.py
+drwxrwxr-x   0 saeed     (1000) saeed     (1000)        0 2023-06-22 11:37:13.196879 micro_orch-0.1.2/tests/
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)        0 2023-06-19 07:46:44.000000 micro_orch-0.1.2/tests/__init__.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     6620 2023-06-22 11:36:48.000000 micro_orch-0.1.2/tests/test_async_saga.py
+-rw-rw-r--   0 saeed     (1000) saeed     (1000)     2091 2023-06-22 11:36:48.000000 micro_orch-0.1.2/tests/test_sync_saga.py
```

### Comparing `micro_orch-0.1.1/LICENSE` & `micro_orch-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/PKG-INFO` & `micro_orch-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro_orch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/micro-orch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/micro-orch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
```

### Comparing `micro_orch-0.1.1/README.md` & `micro_orch-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/micro_orch.egg-info/PKG-INFO` & `micro_orch-0.1.2/micro_orch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micro-orch
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Microservice Orchestrator
 Home-page: https://github.com/hasanisaeed/micro-orch
 Author: Saeed Hasani Borzadaran
 Author-email: hassanisaeed19@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/hasanisaeed/micro-orch/issues/new
 Keywords: microservice,saga,patterns,microservice patterns,saga pattern
```

### Comparing `micro_orch-0.1.1/micro_orch.egg-info/SOURCES.txt` & `micro_orch-0.1.2/micro_orch.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
+micro_orch/__init__.py
 micro_orch.egg-info/PKG-INFO
 micro_orch.egg-info/SOURCES.txt
 micro_orch.egg-info/dependency_links.txt
 micro_orch.egg-info/top_level.txt
-src/__init__.py
-src/helpers/__init__.py
-src/helpers/asynch.py
-src/helpers/celery_utils.py
-src/helpers/handlers.py
-src/helpers/repository.py
-src/helpers/status.py
-src/helpers/utils.py
-src/saga/__init__.py
-src/saga/asynch.py
-src/saga/base.py
-src/saga/stateful.py
-src/steps/__init__.py
-src/steps/asynch.py
-src/steps/base.py
-src/steps/sync.py
+micro_orch/helpers/__init__.py
+micro_orch/helpers/asynch.py
+micro_orch/helpers/celery_utils.py
+micro_orch/helpers/handlers.py
+micro_orch/helpers/repository.py
+micro_orch/helpers/status.py
+micro_orch/helpers/utils.py
+micro_orch/saga/__init__.py
+micro_orch/saga/asynch.py
+micro_orch/saga/base.py
+micro_orch/saga/stateful.py
+micro_orch/steps/__init__.py
+micro_orch/steps/asynch.py
+micro_orch/steps/base.py
+micro_orch/steps/sync.py
 tests/__init__.py
 tests/test_async_saga.py
 tests/test_sync_saga.py
```

### Comparing `micro_orch-0.1.1/setup.cfg` & `micro_orch-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = micro_orch
-version = 0.1.1
+version = 0.1.2
 author = Saeed Hasani Borzadaran
 author_email = hassanisaeed19@gmail.com
 description = Python Microservice Orchestrator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/hasanisaeed/micro-orch
 project_urls =
```

### Comparing `micro_orch-0.1.1/setup.py` & `micro_orch-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 setuptools.setup(name="micro_orch",
-                 version="0.1.1",
+                 version="0.1.2",
                  author="Saeed Hasani Borzadaran",
                  author_email="hassanisaeed19@gmail.com",
                  description="Python Microservice Orchestrator",
                  long_description_content_type="text/markdown",
                  url="https://github.com/hasanisaeed/micro-orch",
                  keywords='microservice, saga, patterns, microservice patterns, saga pattern',
                  python_requires='>=3.9',
```

### Comparing `micro_orch-0.1.1/src/helpers/asynch.py` & `micro_orch-0.1.2/micro_orch/helpers/asynch.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/helpers/celery_utils.py` & `micro_orch-0.1.2/micro_orch/helpers/celery_utils.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/helpers/handlers.py` & `micro_orch-0.1.2/micro_orch/helpers/handlers.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/helpers/repository.py` & `micro_orch-0.1.2/micro_orch/helpers/repository.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/helpers/utils.py` & `micro_orch-0.1.2/micro_orch/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/saga/asynch.py` & `micro_orch-0.1.2/micro_orch/saga/asynch.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/saga/base.py` & `micro_orch-0.1.2/micro_orch/saga/base.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/saga/stateful.py` & `micro_orch-0.1.2/micro_orch/saga/stateful.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/src/steps/asynch.py` & `micro_orch-0.1.2/micro_orch/steps/asynch.py`

 * *Files identical despite different names*

### Comparing `micro_orch-0.1.1/tests/test_async_saga.py` & `micro_orch-0.1.2/tests/test_async_saga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Dict
 from unittest.mock import MagicMock
 
-from src import SyncStep, AsyncStep
-from src.saga import AsyncSaga
+from micro_orch import AsyncSaga, SyncStep, AsyncStep
 
 
 def test_run_success_many_step():
     start_step_compensation_mock = MagicMock()
 
     step_2_success_mock = MagicMock()
     step_2_failure_mock = MagicMock()
```

### Comparing `micro_orch-0.1.1/tests/test_sync_saga.py` & `micro_orch-0.1.2/tests/test_sync_saga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest.mock import MagicMock
 
-from src import SyncStep, BaseSaga
+from micro_orch import SyncStep, BaseSaga
 
 
 def test_run_success():
     start_step_action_mock = MagicMock()
     start_step_compensation_mock = MagicMock()
 
     fake_action_mock = MagicMock()
```

