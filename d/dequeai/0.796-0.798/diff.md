# Comparing `tmp/dequeai-0.796.tar.gz` & `tmp/dequeai-0.798.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dequeai-0.796.tar", last modified: Thu Jun 22 20:40:57 2023, max compression
+gzip compressed data, was "dequeai-0.798.tar", last modified: Thu Jun 22 20:42:16 2023, max compression
```

## Comparing `dequeai-0.796.tar` & `dequeai-0.798.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:40:57.722143 dequeai-0.796/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:40:57.722143 dequeai-0.796/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:40:57.722143 dequeai-0.796/dequeai/
--rw-r--r--   0 root         (0) root         (0)      401 2023-06-22 20:31:56.000000 dequeai-0.796/dequeai/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.796/dequeai/datatypes.py
--rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.796/dequeai/deque_config.py
--rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.796/dequeai/deque_environment.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-06-22 20:30:08.000000 dequeai-0.796/dequeai/dequeai.py
--rw-r--r--   0 root         (0) root         (0)    31882 2023-06-22 20:40:35.000000 dequeai-0.796/dequeai/dequeai_run.py
--rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.796/dequeai/parsing_service.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.796/dequeai/redis_services.py
--rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.796/dequeai/rest_connect.py
--rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.796/dequeai/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:40:57.722143 dequeai-0.796/dequeai.egg-info/
--rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:40:57.000000 dequeai-0.796/dequeai.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 20:40:57.000000 dequeai-0.796/dequeai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:40:57.000000 dequeai-0.796/dequeai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 20:40:57.000000 dequeai-0.796/dequeai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 20:40:57.000000 dequeai-0.796/dequeai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:40:57.722143 dequeai-0.796/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      557 2023-06-22 20:40:44.000000 dequeai-0.796/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:42:16.486746 dequeai-0.798/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:42:16.486746 dequeai-0.798/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:42:16.486746 dequeai-0.798/dequeai/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-06-22 20:31:56.000000 dequeai-0.798/dequeai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14712 2023-06-14 22:37:55.000000 dequeai-0.798/dequeai/datatypes.py
+-rw-r--r--   0 root         (0) root         (0)      256 2022-04-22 17:52:12.000000 dequeai-0.798/dequeai/deque_config.py
+-rw-r--r--   0 root         (0) root         (0)      350 2023-04-11 17:28:02.000000 dequeai-0.798/dequeai/deque_environment.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-06-22 20:30:08.000000 dequeai-0.798/dequeai/dequeai.py
+-rw-r--r--   0 root         (0) root         (0)    31800 2023-06-22 20:41:52.000000 dequeai-0.798/dequeai/dequeai_run.py
+-rw-r--r--   0 root         (0) root         (0)     3242 2023-03-27 20:38:54.000000 dequeai-0.798/dequeai/parsing_service.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-08-26 18:22:25.000000 dequeai-0.798/dequeai/redis_services.py
+-rw-r--r--   0 root         (0) root         (0)     1888 2022-05-04 21:23:01.000000 dequeai-0.798/dequeai/rest_connect.py
+-rw-r--r--   0 root         (0) root         (0)     2535 2023-06-22 19:21:57.000000 dequeai-0.798/dequeai/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:42:16.486746 dequeai-0.798/dequeai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      382 2023-06-22 20:42:16.000000 dequeai-0.798/dequeai.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-22 20:42:16.000000 dequeai-0.798/dequeai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:42:16.000000 dequeai-0.798/dequeai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-22 20:42:16.000000 dequeai-0.798/dequeai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 20:42:16.000000 dequeai-0.798/dequeai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:42:16.486746 dequeai-0.798/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-22 20:42:03.000000 dequeai-0.798/setup.py
```

### Comparing `dequeai-0.796/dequeai/datatypes.py` & `dequeai-0.798/dequeai/datatypes.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.796/dequeai/dequeai.py` & `dequeai-0.798/dequeai/dequeai.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.796/dequeai/dequeai_run.py` & `dequeai-0.798/dequeai/dequeai_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -645,16 +645,14 @@
             else:
                 return None
 
         return current_dict
 
     def _gradient_hook(self, module, grad_input, grad_output):
         print("Gradient hook called")
-        if self._step % self._gradient_logging_frequency != 0:
-            return
 
         module_name = module.__class__.__name__
 
         # Handling multiple input gradients
         for idx, grad in enumerate(grad_input):
             if grad is not None:
                 self._log_histogram(name=f"{module_name}_input_{idx}_grad", values=grad.cpu().numpy())
```

### Comparing `dequeai-0.796/dequeai/parsing_service.py` & `dequeai-0.798/dequeai/parsing_service.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.796/dequeai/rest_connect.py` & `dequeai-0.798/dequeai/rest_connect.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.796/dequeai/util.py` & `dequeai-0.798/dequeai/util.py`

 * *Files identical despite different names*

### Comparing `dequeai-0.796/setup.py` & `dequeai-0.798/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, Extension
 
 
 setup(
     name='dequeai',
-    version='0.00000796',
+    version='0.00000798',
     description='Python Package for DEQUE AI Platform',
     author="The DEQUE AI Team",
     author_email='team@deque.app',
     packages=["dequeai"],
     url='https://dequeapp-deque.gitbook.io/deque-docs/getting-started/dequeai-experiment-tracking',
     keywords='deque client for experiment tracking, sweep and other deep learning tooling',
     install_requires=[
```

