# Comparing `tmp/obsws_python-1.5.0.tar.gz` & `tmp/obsws_python-1.5.1.tar.gz`

## Comparing `obsws_python-1.5.0.tar` & `obsws_python-1.5.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/__init__.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/baseclient.py
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/callback.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/error.py
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/events.py
--rw-r--r--   0        0        0    57952 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/reqs.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/subs.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/util.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 obsws_python-1.5.0/obsws_python/version.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 obsws_python-1.5.0/.gitignore
--rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 obsws_python-1.5.0/LICENSE
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 obsws_python-1.5.0/README.md
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 obsws_python-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     4702 2020-02-02 00:00:00.000000 obsws_python-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/__init__.py
+-rw-r--r--   0        0        0     4485 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/baseclient.py
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/callback.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/error.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/events.py
+-rw-r--r--   0        0        0    58004 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/reqs.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/subs.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/util.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 obsws_python-1.5.1/obsws_python/version.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 obsws_python-1.5.1/.gitignore
+-rw-r--r--   0        0        0    35821 2020-02-02 00:00:00.000000 obsws_python-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 obsws_python-1.5.1/README.md
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 obsws_python-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     4702 2020-02-02 00:00:00.000000 obsws_python-1.5.1/PKG-INFO
```

### Comparing `obsws_python-1.5.0/obsws_python/baseclient.py` & `obsws_python-1.5.1/obsws_python/baseclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,19 +7,20 @@
 from typing import Optional
 
 import websocket
 from websocket import WebSocketTimeoutException
 
 from .error import OBSSDKError, OBSSDKTimeoutError
 
+logger = logging.getLogger(__name__)
 
-class ObsClient:
-    logger = logging.getLogger("baseclient.obsclient")
 
+class ObsClient:
     def __init__(self, **kwargs):
+        self.logger = logger.getChild(self.__class__.__name__)
         defaultkwargs = {
             "host": "localhost",
             "port": 4455,
             "password": "",
             "subs": 0,
             "timeout": None,
         }
```

### Comparing `obsws_python-1.5.0/obsws_python/callback.py` & `obsws_python-1.5.1/obsws_python/callback.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.0/obsws_python/events.py` & `obsws_python-1.5.1/obsws_python/events.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 
 """
 A class to interact with obs-websocket events
 defined in official github repo
 https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md#events
 """
 
+logger = logging.getLogger(__name__)
+
 
 class EventClient:
-    logger = logging.getLogger("events.eventclient")
     DELAY = 0.001
 
     def __init__(self, **kwargs):
+        self.logger = logger.getChild(self.__class__.__name__)
         defaultkwargs = {"subs": Subs.LOW_VOLUME}
         kwargs = defaultkwargs | kwargs
         self.base_client = ObsClient(**kwargs)
         if self.base_client.authenticate():
             self.logger.info(f"Successfully identified {self} with the server")
         self.callback = Callback()
         self.subscribe()
```

### Comparing `obsws_python-1.5.0/obsws_python/reqs.py` & `obsws_python-1.5.1/obsws_python/reqs.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,20 @@
 
 """
 A class to interact with obs-websocket requests
 defined in official github repo
 https://github.com/obsproject/obs-websocket/blob/master/docs/generated/protocol.md#Requests
 """
 
+logger = logging.getLogger(__name__)
 
-class ReqClient:
-    logger = logging.getLogger("reqs.reqclient")
 
+class ReqClient:
     def __init__(self, **kwargs):
+        self.logger = logger.getChild(self.__class__.__name__)
         self.base_client = ObsClient(**kwargs)
         if self.base_client.authenticate():
             self.logger.info(f"Successfully identified {self} with the server")
 
     def __enter__(self):
         return self
```

### Comparing `obsws_python-1.5.0/obsws_python/subs.py` & `obsws_python-1.5.1/obsws_python/subs.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.0/obsws_python/util.py` & `obsws_python-1.5.1/obsws_python/util.py`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.0/.gitignore` & `obsws_python-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.0/LICENSE` & `obsws_python-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.0/README.md` & `obsws_python-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.0/pyproject.toml` & `obsws_python-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `obsws_python-1.5.0/PKG-INFO` & `obsws_python-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsws-python
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Python SDK for OBS Studio WebSocket v5.0
 Project-URL: Homepage, https://github.com/aatikturk/obsws-python
 Author-email: Adem Atikturk <aatikturk@gmail.com>
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: tomli>=2.0.1; python_version < '3.11'
 Requires-Dist: websocket-client
```

