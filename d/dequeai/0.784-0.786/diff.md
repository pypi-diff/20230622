# Comparing `tmp/dequeai-0.784.tar.gz` & `tmp/dequeai-0.786.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.784.tar", last modified: Wed Jun 14 22:38:21 2023, max compression
+gzip compressed data, was "dequeai-0.786.tar", last modified: Thu Jun 22 16:17:12 2023, max compression
```

## Comparing `dequeai-0.784.tar` & `dequeai-0.786.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:38:21.405068 dequeai-0.784/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-14 22:38:21.405068 dequeai-0.784/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:38:21.405068 dequeai-0.784/dequeai/
--rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.784/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.784/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.784/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.784/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.784/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    30266 2023-05-12 17:14:03.000000 dequeai-0.784/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.784/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.784/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.784/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.784/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 22:38:21.405068 dequeai-0.784/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      408 2023-06-14 22:38:20.000000 dequeai-0.784/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-14 22:38:21.000000 dequeai-0.784/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 22:38:21.405068 dequeai-0.784/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      583 2023-06-14 22:38:06.000000 dequeai-0.784/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:17:12.699135 dequeai-0.786/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 16:17:12.699135 dequeai-0.786/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:17:12.699135 dequeai-0.786/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      370 2023-04-21 15:01:14.000000 dequeai-0.786/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.786/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.786/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.786/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)      955 2023-04-26 15:26:45.000000 dequeai-0.786/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    30994 2023-06-22 16:13:46.000000 dequeai-0.786/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.786/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.786/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.786/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2483 2023-03-27 20:38:54.000000 dequeai-0.786/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:17:12.699135 dequeai-0.786/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 16:17:12.000000 dequeai-0.786/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 16:17:12.699135 dequeai-0.786/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      583 2023-06-22 16:16:56.000000 dequeai-0.786/setup.py
```

### Comparing `dequeai-0.784/dequeai/datatypes.py` & `dequeai-0.786/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.784/dequeai/dequeai.py` & `dequeai-0.786/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.784/dequeai/dequeai_run.py` & `dequeai-0.786/dequeai/dequeai_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import GPUtil
 import socket
 import types
 from IPython.display import display, HTML
 from tabulate import tabulate
 import numpy as np
 
+
 _RESOURCE_MONITORING_INTERVAL = 60
 
 
 class Run:
 
     def __init__(self):
         self.user_name = None
@@ -44,14 +45,15 @@
         self._model_logged = False
         self._code_logged = False
         self._running = False
         self._environment_logged = False
         self._resources_logged = False
         self._res_monitor = None
         self._run_start_time = None
+        self._gradient_logging_frequency = 1
 
     def init(self, user_name, api_key, project_name=None):
 
         os.environ["running"] = "yes"
         is_authenticated = self._authenticate(user_name=user_name, api_key=api_key)
         if is_authenticated:
             self.user_name = user_name
@@ -642,14 +644,18 @@
                 current_dict = current_dict[k]
             else:
                 return None
 
         return current_dict
 
     def _gradient_hook(self, module, grad_input, grad_output):
+
+        if self._step % self._gradient_logging_frequency != 0:
+            return
+
         module_name = module.__class__.__name__
 
         # Handling multiple input gradients
         for idx, grad in enumerate(grad_input):
             if grad is not None:
                 self._log_histogram(f"{module_name}_input_{idx}_grad", grad.cpu().numpy())
 
@@ -678,17 +684,31 @@
             max_value = np.max(values)
 
         # Compute the histogram using numpy
         hist, bin_edges = np.histogram(values, bins=bins, range=(min_value, max_value), density=density)
 
         return bin_edges, hist
 
-    def log_gradients(self, model):
+    def log_gradients(self, model, logging_frequency=1, layers_to_log="all"):
+        try:
+            import torch
+        except ImportError:
+            raise ImportError("PyTorch is required for logging gradients.")
+
+            # Check if the model is a PyTorch model
+        if not isinstance(model, torch.nn.Module):
+            raise TypeError('Model should be an instance of a PyTorch nn.Module.')
+
+        self._gradient_logging_frequency = logging_frequency
+        if layers_to_log in [None, "all"]:
+            layers_to_log = [name for name, _ in model.named_modules()]
         for module_name, module in model.named_modules():
-            module.register_backward_hook(self._gradient_hook)
+            if module_name in layers_to_log:
+                module.register_backward_hook(self._gradient_hook)
+
 
 
 
 
 if __name__ == "__main__":
     deque = Run()
     deque._validate_hyperparams({"train": {"accuracy": "1.3", "loss": "2.2"}})
```

### Comparing `dequeai-0.784/dequeai/parsing_service.py` & `dequeai-0.786/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.784/dequeai/rest_connect.py` & `dequeai-0.786/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.784/dequeai/util.py` & `dequeai-0.786/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.784/setup.py` & `dequeai-0.786/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000784',
+    version='0.00000786',
     description='Python Experiment Tracking Package for Deque AI DLOps Platform',
     author="The Deque AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

