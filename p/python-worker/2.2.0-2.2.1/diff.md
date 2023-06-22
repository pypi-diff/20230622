# Comparing `tmp/python-worker-2.2.0.tar.gz` & `tmp/python-worker-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-worker-2.2.0.tar", last modified: Thu Jun 22 08:55:23 2023, max compression
+gzip compressed data, was "python-worker-2.2.1.tar", last modified: Thu Jun 22 09:16:35 2023, max compression
```

## Comparing `python-worker-2.2.0.tar` & `python-worker-2.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 08:55:23.050560 python-worker-2.2.0/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     8314 2023-06-22 08:55:23.050560 python-worker-2.2.0/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7882 2023-06-22 08:54:57.000000 python-worker-2.2.0/README.md
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 08:55:23.050560 python-worker-2.2.0/python_worker.egg-info/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     8314 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/PKG-INFO
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      256 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/SOURCES.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/dependency_links.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        9 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/requires.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        7 2023-06-22 08:55:22.000000 python-worker-2.2.0/python_worker.egg-info/top_level.txt
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-22 08:55:23.050560 python-worker-2.2.0/setup.cfg
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1253 2023-06-22 08:53:37.000000 python-worker-2.2.0/setup.py
-drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 08:55:23.050560 python-worker-2.2.0/worker/
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     4424 2023-06-22 08:53:21.000000 python-worker-2.2.0/worker/__init__.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     3509 2023-06-22 08:52:13.000000 python-worker-2.2.0/worker/process.py
--rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    19813 2022-12-27 10:45:46.000000 python-worker-2.2.0/worker/worker.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 09:16:35.103967 python-worker-2.2.1/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     8314 2023-06-22 09:16:35.103967 python-worker-2.2.1/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     7882 2023-06-22 08:54:57.000000 python-worker-2.2.1/README.md
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 09:16:35.099967 python-worker-2.2.1/python_worker.egg-info/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     8314 2023-06-22 09:16:35.000000 python-worker-2.2.1/python_worker.egg-info/PKG-INFO
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)      256 2023-06-22 09:16:35.000000 python-worker-2.2.1/python_worker.egg-info/SOURCES.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        1 2023-06-22 09:16:35.000000 python-worker-2.2.1/python_worker.egg-info/dependency_links.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        9 2023-06-22 09:16:35.000000 python-worker-2.2.1/python_worker.egg-info/requires.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)        7 2023-06-22 09:16:35.000000 python-worker-2.2.1/python_worker.egg-info/top_level.txt
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)       38 2023-06-22 09:16:35.103967 python-worker-2.2.1/setup.cfg
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     1253 2023-06-22 09:16:31.000000 python-worker-2.2.1/setup.py
+drwxrwxr-x   0 danangjoyoo  (1000) danangjoyoo  (1000)        0 2023-06-22 09:16:35.103967 python-worker-2.2.1/worker/
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     4418 2023-06-22 09:16:18.000000 python-worker-2.2.1/worker/__init__.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)     3512 2023-06-22 09:16:24.000000 python-worker-2.2.1/worker/process.py
+-rw-rw-r--   0 danangjoyoo  (1000) danangjoyoo  (1000)    19813 2022-12-27 10:45:46.000000 python-worker-2.2.1/worker/worker.py
```

### Comparing `python-worker-2.2.0/PKG-INFO` & `python-worker-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-worker
-Version: 2.2.0
+Version: 2.2.1
 Summary: Simplify and master control (run and stop) the python threads (workers)
 Home-page: https://github.com/Danangjoyoo/python-worker
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: python,threading,worker,async worker,async thread,abort thread,thread stopper,thread manager,simple thread,thread monitor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-worker-2.2.0/README.md` & `python-worker-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `python-worker-2.2.0/python_worker.egg-info/PKG-INFO` & `python-worker-2.2.1/python_worker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-worker
-Version: 2.2.0
+Version: 2.2.1
 Summary: Simplify and master control (run and stop) the python threads (workers)
 Home-page: https://github.com/Danangjoyoo/python-worker
 Author: danangjoyoo (Agus Danangjoyo)
 Author-email: <agus.danangjoyo.blog@gmail.com>
 Keywords: python,threading,worker,async worker,async thread,abort thread,thread stopper,thread manager,simple thread,thread monitor
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `python-worker-2.2.0/setup.py` & `python-worker-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '2.2.0'
+VERSION = '2.2.1'
 DESCRIPTION = 'Simplify and master control (run and stop) the python threads (workers)'
 
 # Setting up
 setup(
     name="python-worker",
     version=VERSION,
     author="danangjoyoo (Agus Danangjoyo)",
```

### Comparing `python-worker-2.2.0/worker/__init__.py` & `python-worker-2.2.1/worker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,12 +124,12 @@
 def process(function: FunctionType):
     """
     Create a process worker. This function will run your function in a separate GIL
     """
     return ProcessConnector.create_process(function)
 
 
-async def async_process(function: FunctionType):
+def async_process(function: FunctionType):
     """
     Create an async process worker. This function will run your function in a separate GIL
     """
     return ProcessConnector.create_process(function)
```

### Comparing `python-worker-2.2.0/worker/process.py` & `python-worker-2.2.1/worker/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     @property
     def ret(self):
         if self.parent_con and not self.parent_con.closed and self.child_con.closed:
             self.result = self.parent_con.recv()
             self.parent_con.close()
         return self.result
 
-    def wait(self, timeout):
+    def wait(self, timeout=10):
         self.proc.join(timeout)
 
     def receive(self):
         return self.parent_con.recv()
 
     @staticmethod
     def create_process(function: FunctionType):
```

### Comparing `python-worker-2.2.0/worker/worker.py` & `python-worker-2.2.1/worker/worker.py`

 * *Files identical despite different names*

