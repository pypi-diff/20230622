# Comparing `tmp/dequeai-0.790.tar.gz` & `tmp/dequeai-0.792.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.790.tar", last modified: Thu Jun 22 20:30:51 2023, max compression
+gzip compressed data, was "dequeai-0.792.tar", last modified: Thu Jun 22 20:32:56 2023, max compression
```

## Comparing `dequeai-0.790.tar` & `dequeai-0.792.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:30:51.902624 dequeai-0.790/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 20:30:51.902624 dequeai-0.790/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:30:51.902624 dequeai-0.790/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.790/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.790/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.790/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.790/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-22 20:30:08.000000 dequeai-0.790/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    31683 2023-06-22 20:06:58.000000 dequeai-0.790/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.790/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.790/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.790/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.790/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:30:51.902624 dequeai-0.790/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 20:30:51.000000 dequeai-0.790/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 20:30:51.000000 dequeai-0.790/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:30:51.000000 dequeai-0.790/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 20:30:51.000000 dequeai-0.790/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 20:30:51.000000 dequeai-0.790/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:30:51.902624 dequeai-0.790/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-22 20:30:38.000000 dequeai-0.790/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:32:56.079324 dequeai-0.792/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:32:56.079324 dequeai-0.792/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:32:56.079324 dequeai-0.792/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-06-22 20:31:56.000000 dequeai-0.792/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.792/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.792/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.792/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-22 20:30:08.000000 dequeai-0.792/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    31683 2023-06-22 20:06:58.000000 dequeai-0.792/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.792/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.792/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.792/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.792/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:32:56.079324 dequeai-0.792/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 20:32:56.000000 dequeai-0.792/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:32:56.079324 dequeai-0.792/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-22 20:32:40.000000 dequeai-0.792/setup.py
```

### Comparing `dequeai-0.790/dequeai/datatypes.py` & `dequeai-0.792/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.790/dequeai/dequeai.py` & `dequeai-0.792/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.790/dequeai/dequeai_run.py` & `dequeai-0.792/dequeai/dequeai_run.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.790/dequeai/parsing_service.py` & `dequeai-0.792/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.790/dequeai/rest_connect.py` & `dequeai-0.792/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.790/dequeai/util.py` & `dequeai-0.792/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.790/setup.py` & `dequeai-0.792/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000790',
-    description='Python Experiment Tracking Package for Deque AI DLOps Platform',
+    version='0.00000792',
+    description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
           "coolname","requests","numpy","pillow","psutil","GPUtil","ipython","tabulate"
```

