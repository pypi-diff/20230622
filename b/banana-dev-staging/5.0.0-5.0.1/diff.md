# Comparing `tmp/banana_dev_staging-5.0.0.tar.gz` & `tmp/banana_dev_staging-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "banana_dev_staging-5.0.0.tar", last modified: Thu May 25 22:41:14 2023, max compression
+gzip compressed data, was "banana_dev_staging-5.0.1.tar", last modified: Thu Jun 22 03:28:49 2023, max compression
```

## Comparing `banana_dev_staging-5.0.0.tar` & `banana_dev_staging-5.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:41:14.951409 banana_dev_staging-5.0.0/
--rw-r--r--   0 erik       (501) staff       (20)     1869 2023-05-25 22:41:14.951465 banana_dev_staging-5.0.0/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)     1220 2023-04-25 00:43:43.000000 banana_dev_staging-5.0.0/README.md
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:41:14.950521 banana_dev_staging-5.0.0/banana_dev/
--rw-r--r--   0 erik       (501) staff       (20)       26 2023-04-25 02:04:09.000000 banana_dev_staging-5.0.0/banana_dev/__init__.py
--rw-r--r--   0 erik       (501) staff       (20)     3976 2023-05-25 22:35:07.000000 banana_dev_staging-5.0.0/banana_dev/client.py
-drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-05-25 22:41:14.951312 banana_dev_staging-5.0.0/banana_dev_staging.egg-info/
--rw-r--r--   0 erik       (501) staff       (20)     1869 2023-05-25 22:41:14.000000 banana_dev_staging-5.0.0/banana_dev_staging.egg-info/PKG-INFO
--rw-r--r--   0 erik       (501) staff       (20)      298 2023-05-25 22:41:14.000000 banana_dev_staging-5.0.0/banana_dev_staging.egg-info/SOURCES.txt
--rw-r--r--   0 erik       (501) staff       (20)        1 2023-05-25 22:41:14.000000 banana_dev_staging-5.0.0/banana_dev_staging.egg-info/dependency_links.txt
--rw-r--r--   0 erik       (501) staff       (20)       24 2023-05-25 22:41:14.000000 banana_dev_staging-5.0.0/banana_dev_staging.egg-info/requires.txt
--rw-r--r--   0 erik       (501) staff       (20)       11 2023-05-25 22:41:14.000000 banana_dev_staging-5.0.0/banana_dev_staging.egg-info/top_level.txt
--rw-r--r--   0 erik       (501) staff       (20)       79 2023-05-25 22:41:14.951659 banana_dev_staging-5.0.0/setup.cfg
--rw-r--r--   0 erik       (501) staff       (20)     1235 2023-05-25 22:37:32.000000 banana_dev_staging-5.0.0/setup.py
--rw-r--r--   0 erik       (501) staff       (20)     1224 2023-05-25 22:41:12.000000 banana_dev_staging-5.0.0/setup_staging.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-22 03:28:49.968648 banana_dev_staging-5.0.1/
+-rw-r--r--   0 erik       (501) staff       (20)     1869 2023-06-22 03:28:49.968707 banana_dev_staging-5.0.1/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)     1220 2023-04-25 00:43:43.000000 banana_dev_staging-5.0.1/README.md
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-22 03:28:49.967916 banana_dev_staging-5.0.1/banana_dev/
+-rw-r--r--   0 erik       (501) staff       (20)       26 2023-04-25 02:04:09.000000 banana_dev_staging-5.0.1/banana_dev/__init__.py
+-rw-r--r--   0 erik       (501) staff       (20)     4026 2023-06-22 03:13:37.000000 banana_dev_staging-5.0.1/banana_dev/client.py
+drwxr-xr-x   0 erik       (501) staff       (20)        0 2023-06-22 03:28:49.968560 banana_dev_staging-5.0.1/banana_dev_staging.egg-info/
+-rw-r--r--   0 erik       (501) staff       (20)     1869 2023-06-22 03:28:49.000000 banana_dev_staging-5.0.1/banana_dev_staging.egg-info/PKG-INFO
+-rw-r--r--   0 erik       (501) staff       (20)      298 2023-06-22 03:28:49.000000 banana_dev_staging-5.0.1/banana_dev_staging.egg-info/SOURCES.txt
+-rw-r--r--   0 erik       (501) staff       (20)        1 2023-06-22 03:28:49.000000 banana_dev_staging-5.0.1/banana_dev_staging.egg-info/dependency_links.txt
+-rw-r--r--   0 erik       (501) staff       (20)       24 2023-06-22 03:28:49.000000 banana_dev_staging-5.0.1/banana_dev_staging.egg-info/requires.txt
+-rw-r--r--   0 erik       (501) staff       (20)       11 2023-06-22 03:28:49.000000 banana_dev_staging-5.0.1/banana_dev_staging.egg-info/top_level.txt
+-rw-r--r--   0 erik       (501) staff       (20)       79 2023-06-22 03:28:49.968892 banana_dev_staging-5.0.1/setup.cfg
+-rw-r--r--   0 erik       (501) staff       (20)     1235 2023-05-25 22:37:32.000000 banana_dev_staging-5.0.1/setup.py
+-rw-r--r--   0 erik       (501) staff       (20)     1224 2023-06-22 03:28:47.000000 banana_dev_staging-5.0.1/setup_staging.py
```

### Comparing `banana_dev_staging-5.0.0/PKG-INFO` & `banana_dev_staging-5.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banana_dev_staging
-Version: 5.0.0
+Version: 5.0.1
 Summary: The banana package is a python client to interact with your Potassium servers hosted on Banana
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: MIT
 Keywords: Banana client,API wrapper,Banana,SDK
 Classifier: Development Status :: 4 - Beta
```

### Comparing `banana_dev_staging-5.0.0/README.md` & `banana_dev_staging-5.0.1/README.md`

 * *Files identical despite different names*

### Comparing `banana_dev_staging-5.0.0/banana_dev/client.py` & `banana_dev_staging-5.0.1/banana_dev/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Union
+from typing import Union, Tuple
 import requests, time
 
 class ClientException(Exception):
     "Raised on errors from Banana client"
     def __init__(self, message = "" , res: requests.Response = None):
         if res != None:
             self.message = res.text
         else:
             self.message = message
         self.message = "\n" + self.message
         super().__init__(self.message)
 
 class Client():
+    "The Banana client class is for interracting with a specific model on Banana."
     def __init__(self, api_key, model_key, url, verbose = True):
         self.api_key = api_key
         self.model_key = model_key
         self.url = url
         self.verbose = verbose
 
-    def call(self, route: str, json: dict = {}, headers: dict = {}, use_replica: Union[str, None] = None, retry=True, retry_timeout = 300):
+    "Call a route on the Banana server with a POST request"
+    def call(self, route: str, json: dict = {}, headers: dict = {}, retry=True, retry_timeout = 300) -> Tuple[dict, dict]:
         headers["Content-Type"] = "application/json"
         headers['X-BANANA-API-KEY'] = self.api_key
         headers['X-BANANA-MODEL-KEY'] = self.model_key
-        if use_replica != None:
-            headers["X-USE-REPLICA"] = use_replica
         endpoint = self.url.rstrip("/") + "/" + route.lstrip("/")
 
         backoff_interval = 0.1 # seed for exponential backoff
         start = time.time()
         first_call = True
 
         # start retry loop
```

### Comparing `banana_dev_staging-5.0.0/banana_dev_staging.egg-info/PKG-INFO` & `banana_dev_staging-5.0.1/banana_dev_staging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: banana-dev-staging
-Version: 5.0.0
+Version: 5.0.1
 Summary: The banana package is a python client to interact with your Potassium servers hosted on Banana
 Home-page: https://www.banana.dev
 Author: Erik Dunteman
 Author-email: erik@banana.dev
 License: MIT
 Keywords: Banana client,API wrapper,Banana,SDK
 Classifier: Development Status :: 4 - Beta
```

### Comparing `banana_dev_staging-5.0.0/setup.py` & `banana_dev_staging-5.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `banana_dev_staging-5.0.0/setup_staging.py` & `banana_dev_staging-5.0.1/setup_staging.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='banana_dev_staging',
     packages=['banana_dev'],
-    version='5.0.0',
+    version='5.0.1',
     license='MIT',
     # Give a short description about your library
     description='The banana package is a python client to interact with your Potassium servers hosted on Banana',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Erik Dunteman',
     author_email='erik@banana.dev',
```

