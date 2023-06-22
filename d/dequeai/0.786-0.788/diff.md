# Comparing `tmp/dequeai-0.786.tar.gz` & `tmp/dequeai-0.788.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.786.tar", last modified: Thu Jun 22 16:17:12 2023, max compression
+gzip compressed data, was "dequeai-0.788.tar", last modified: Thu Jun 22 20:26:25 2023, max compression
```

## Comparing `dequeai-0.786.tar` & `dequeai-0.788.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:17:12.699135 dequeai-0.786/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 16:17:12.699135 dequeai-0.786/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:17:12.699135 dequeai-0.786/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.786/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.786/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.786/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.786/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.786/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    30994 2023-06-22 16:13:46.000000 dequeai-0.786/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.786/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.786/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.786/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.786/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:17:12.699135 dequeai-0.786/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 16:17:12.699135 dequeai-0.786/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-22 16:16:56.000000 dequeai-0.786/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:26:25.133119 dequeai-0.788/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 20:26:25.133119 dequeai-0.788/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:26:25.133119 dequeai-0.788/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.788/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.788/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.788/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.788/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.788/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    31683 2023-06-22 20:06:58.000000 dequeai-0.788/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.788/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.788/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.788/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.788/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:26:25.133119 dequeai-0.788/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 20:26:24.000000 dequeai-0.788/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 20:26:25.000000 dequeai-0.788/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:26:24.000000 dequeai-0.788/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 20:26:24.000000 dequeai-0.788/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 20:26:25.000000 dequeai-0.788/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:26:25.133119 dequeai-0.788/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      583 2023-06-22 20:26:11.000000 dequeai-0.788/setup.py
```

### Comparing `dequeai-0.786/dequeai/datatypes.py` & `dequeai-0.788/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.786/dequeai/dequeai.py` & `dequeai-0.788/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.786/dequeai/dequeai_run.py` & `dequeai-0.788/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import traceback
 import coolname
 from dequeai.rest_connect import RestConnect
 from dequeai.deque_environment import AGENT_API_SERVICE_URL
 import pickle
 import multiprocessing
 from dequeai.parsing_service import ParsingService
-from dequeai.datatypes import Image, Audio, Histogram, BoundingBox2D, Table  # , Plot
+from dequeai.datatypes import Image, Audio, Histogram, BoundingBox2D, Table, DEQUE_GRADIENT_HISTOGRAM
 from dequeai.util import MODEL, CODE, DATA, ENVIRONMENT, RESOURCES, TRACKING_ENDPOINT
 import requests
 import glob
 import time
 import psutil
 import GPUtil
 import socket
@@ -653,22 +653,24 @@
             return
 
         module_name = module.__class__.__name__
 
         # Handling multiple input gradients
         for idx, grad in enumerate(grad_input):
             if grad is not None:
-                self._log_histogram(f"{module_name}_input_{idx}_grad", grad.cpu().numpy())
+                self._log_histogram(name=f"{module_name}_input_{idx}_grad", values=grad.cpu().numpy())
 
         # Handling multiple output gradients
         for idx, grad in enumerate(grad_output):
             if grad is not None:
-                self._log_histogram(f"{module_name}_output_{idx}_grad", grad.cpu().numpy())
+                self._log_histogram(name=f"{module_name}_output_{idx}_grad", values=grad.cpu().numpy())
+
+    def _log_histogram(self, name, values, bins='auto', min_value=None, max_value=None, density=True):
+
 
-    def _log_histogram(self, values, bins, min_value=None, max_value=None, density=True):
         """
         Log histogram data from the given values.
 
         Args:
             values (list or np.array): The values to create the histogram from.
             bins (int): The number of bins to divide the data into.
             min_value (float, optional): The lower bound of the histogram range. Defaults to the minimum value in the dataset.
@@ -682,15 +684,26 @@
             min_value = np.min(values)
         if max_value is None:
             max_value = np.max(values)
 
         # Compute the histogram using numpy
         hist, bin_edges = np.histogram(values, bins=bins, range=(min_value, max_value), density=density)
 
-        return bin_edges, hist
+        # Log the histogram using the run logger
+
+
+
+        data = {"bin_edges": bin_edges, "hist": hist, "name": name, "min_value": min_value, "max_value": max_value,"datatype":DEQUE_GRADIENT_HISTOGRAM}
+        full_data = {"gradient_data": data}
+        full_data.update(
+            {"user_name": self.user_name, "run_id": self._run_id, "workload_type": self._workload_type,
+             "workload_id": self._workload_id, "submission_id": self._submission_id,
+             "project_name": self._project_name, "deque_log_time": datetime.datetime.now()})
+        resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/log/gradients/", json=full_data)
+
 
     def log_gradients(self, model, logging_frequency=1, layers_to_log="all"):
         try:
             import torch
         except ImportError:
             raise ImportError("PyTorch is required for logging gradients.")
```

### Comparing `dequeai-0.786/dequeai/parsing_service.py` & `dequeai-0.788/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.786/dequeai/rest_connect.py` & `dequeai-0.788/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.786/dequeai/util.py` & `dequeai-0.788/dequeai/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 DEQUE_HISTOGRAM = "deque_histogram"
 DEQUE_AUDIO="deque_audio"
 DEQUE_VIDEO="deque_video"
 DEQUE_TABLE="deque_table"
 DEQUE_TEXT="deque_text"
 DEQUE_BOUNDING_BOX="deque_bounding_box"
 DEQUE_PLOT="deque_plot"
+DEQUE_GRADIENT_HISTOGRAM="deque_gradient_histogram"
 MODEL="model"
 DATA="data"
 PYTORCH="pytorch"
 TENSORFLOW="tensorflow"
 ENVIRONMENT="environment"
 CODE="code"
 RESOURCES = "resources"
```

### Comparing `dequeai-0.786/setup.py` & `dequeai-0.788/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000786',
+    version='0.00000788',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
-    author="The Deque AI Team",
+    author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
           "coolname","requests","numpy","pillow","psutil","GPUtil","ipython","tabulate"
       ],
```

