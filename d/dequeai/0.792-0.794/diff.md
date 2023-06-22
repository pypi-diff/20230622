# Comparing `tmp/dequeai-0.792.tar.gz` & `tmp/dequeai-0.794.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.792.tar", last modified: Thu Jun 22 20:32:56 2023, max compression
+gzip compressed data, was "dequeai-0.794.tar", last modified: Thu Jun 22 20:38:01 2023, max compression
```

## Comparing `dequeai-0.792.tar` & `dequeai-0.794.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:32:56.079324 dequeai-0.792/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:32:56.079324 dequeai-0.792/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:32:56.079324 dequeai-0.792/dequeai/
--rw-r--r--   0 root         (0) root         (0)      401 2023-06-22 20:31:56.000000 dequeai-0.792/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.792/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.792/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.792/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-22 20:30:08.000000 dequeai-0.792/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    31683 2023-06-22 20:06:58.000000 dequeai-0.792/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.792/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.792/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.792/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.792/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:32:56.079324 dequeai-0.792/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 20:32:56.000000 dequeai-0.792/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 20:32:55.000000 dequeai-0.792/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:32:56.079324 dequeai-0.792/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      557 2023-06-22 20:32:40.000000 dequeai-0.792/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:38:01.841046 dequeai-0.794/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:38:01.841046 dequeai-0.794/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:38:01.841046 dequeai-0.794/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-06-22 20:31:56.000000 dequeai-0.794/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.794/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.794/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.794/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-22 20:30:08.000000 dequeai-0.794/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    31744 2023-06-22 20:37:40.000000 dequeai-0.794/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.794/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.794/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.794/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.794/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:38:01.841046 dequeai-0.794/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:38:01.000000 dequeai-0.794/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 20:38:01.000000 dequeai-0.794/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:38:01.000000 dequeai-0.794/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 20:38:01.000000 dequeai-0.794/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 20:38:01.000000 dequeai-0.794/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:38:01.841046 dequeai-0.794/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-22 20:37:48.000000 dequeai-0.794/setup.py
```

### Comparing `dequeai-0.792/dequeai/datatypes.py` & `dequeai-0.794/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.792/dequeai/dequeai.py` & `dequeai-0.794/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.792/dequeai/dequeai_run.py` & `dequeai-0.794/dequeai/dequeai_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,26 +695,27 @@
         data = {"bin_edges": bin_edges, "hist": hist, "name": name, "min_value": min_value, "max_value": max_value,"datatype":DEQUE_GRADIENT_HISTOGRAM}
         full_data = {"gradient_data": data}
         full_data.update(
             {"user_name": self.user_name, "run_id": self._run_id, "workload_type": self._workload_type,
              "workload_id": self._workload_id, "submission_id": self._submission_id,
              "project_name": self._project_name, "deque_log_time": datetime.datetime.now()})
         resp = requests.post(url=AGENT_API_SERVICE_URL + "/fex/project/run/log/gradients/", json=full_data)
+        print(resp.json())
 
 
     def log_gradients(self, model, logging_frequency=1, layers_to_log="all"):
         try:
             import torch
         except ImportError:
             raise ImportError("PyTorch is required for logging gradients.")
 
             # Check if the model is a PyTorch model
         if not isinstance(model, torch.nn.Module):
             raise TypeError('Model should be an instance of a PyTorch nn.Module.')
-
+        print("Logging gradients")
         self._gradient_logging_frequency = logging_frequency
         if layers_to_log in [None, "all"]:
             layers_to_log = [name for name, _ in model.named_modules()]
         for module_name, module in model.named_modules():
             if module_name in layers_to_log:
                 module.register_backward_hook(self._gradient_hook)
```

### Comparing `dequeai-0.792/dequeai/parsing_service.py` & `dequeai-0.794/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.792/dequeai/rest_connect.py` & `dequeai-0.794/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.792/dequeai/util.py` & `dequeai-0.794/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.792/setup.py` & `dequeai-0.794/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000792',
+    version='0.00000794',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

