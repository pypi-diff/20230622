# Comparing `tmp/lightstreamer-client-lib-1.0.2.tar.gz` & `tmp/lightstreamer-client-lib-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightstreamer-client-lib-1.0.2.tar", last modified: Wed Apr  5 09:34:14 2023, max compression
+gzip compressed data, was "lightstreamer-client-lib-1.0.3.tar", last modified: Thu Jun 22 07:33:49 2023, max compression
```

## Comparing `lightstreamer-client-lib-1.0.2.tar` & `lightstreamer-client-lib-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-04-05 09:34:14.538424 lightstreamer-client-lib-1.0.2/
--rw-r--r--   0 acarioni   (501) staff       (20)    11357 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/LICENSE
--rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-04-05 09:34:14.537959 lightstreamer-client-lib-1.0.2/PKG-INFO
--rw-r--r--   0 acarioni   (501) staff       (20)     4517 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/README.md
--rw-r--r--   0 acarioni   (501) staff       (20)      783 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/pyproject.toml
--rw-r--r--   0 acarioni   (501) staff       (20)       38 2023-04-05 09:34:14.538542 lightstreamer-client-lib-1.0.2/setup.cfg
--rw-r--r--   0 acarioni   (501) staff       (20)       37 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/setup.py
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-04-05 09:34:14.516829 lightstreamer-client-lib-1.0.2/src/
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-04-05 09:34:14.516591 lightstreamer-client-lib-1.0.2/src/lightstreamer/
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-04-05 09:34:14.531917 lightstreamer-client-lib-1.0.2/src/lightstreamer/client/
--rw-r--r--   0 acarioni   (501) staff       (20)       75 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer/client/__init__.py
--rw-r--r--   0 acarioni   (501) staff       (20)     5499 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer/client/com_lightstreamer_net.py
--rw-r--r--   0 acarioni   (501) staff       (20)    43272 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer/client/ls_python_client_api.py
--rw-r--r--   0 acarioni   (501) staff       (20)   736212 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer/client/ls_python_client_haxe.py
--rw-r--r--   0 acarioni   (501) staff       (20)   107900 2023-04-05 07:49:11.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer/client/ls_python_client_wrapper.py
-drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-04-05 09:34:14.537419 lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/
--rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-04-05 09:34:14.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/PKG-INFO
--rw-r--r--   0 acarioni   (501) staff       (20)      539 2023-04-05 09:34:14.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/SOURCES.txt
--rw-r--r--   0 acarioni   (501) staff       (20)        1 2023-04-05 09:34:14.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/dependency_links.txt
--rw-r--r--   0 acarioni   (501) staff       (20)       31 2023-04-05 09:34:14.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/requires.txt
--rw-r--r--   0 acarioni   (501) staff       (20)       14 2023-04-05 09:34:14.000000 lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/top_level.txt
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.156802 lightstreamer-client-lib-1.0.3/
+-rw-r--r--   0 acarioni   (501) staff       (20)    11357 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/LICENSE
+-rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-06-22 07:33:49.156004 lightstreamer-client-lib-1.0.3/PKG-INFO
+-rw-r--r--   0 acarioni   (501) staff       (20)     4517 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/README.md
+-rw-r--r--   0 acarioni   (501) staff       (20)      783 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/pyproject.toml
+-rw-r--r--   0 acarioni   (501) staff       (20)       38 2023-06-22 07:33:49.157016 lightstreamer-client-lib-1.0.3/setup.cfg
+-rw-r--r--   0 acarioni   (501) staff       (20)       37 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/setup.py
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.115185 lightstreamer-client-lib-1.0.3/src/
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.114869 lightstreamer-client-lib-1.0.3/src/lightstreamer/
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.137976 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/
+-rw-r--r--   0 acarioni   (501) staff       (20)       75 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/__init__.py
+-rw-r--r--   0 acarioni   (501) staff       (20)     5499 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/com_lightstreamer_net.py
+-rw-r--r--   0 acarioni   (501) staff       (20)    43272 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_api.py
+-rw-r--r--   0 acarioni   (501) staff       (20)   749421 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_haxe.py
+-rw-r--r--   0 acarioni   (501) staff       (20)   107900 2023-06-22 07:30:28.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_wrapper.py
+drwxr-xr-x   0 acarioni   (501) staff       (20)        0 2023-06-22 07:33:49.155097 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/
+-rw-r--r--   0 acarioni   (501) staff       (20)     5121 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/PKG-INFO
+-rw-r--r--   0 acarioni   (501) staff       (20)      539 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 acarioni   (501) staff       (20)        1 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 acarioni   (501) staff       (20)       31 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/requires.txt
+-rw-r--r--   0 acarioni   (501) staff       (20)       14 2023-06-22 07:33:49.000000 lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/top_level.txt
```

### Comparing `lightstreamer-client-lib-1.0.2/LICENSE` & `lightstreamer-client-lib-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lightstreamer-client-lib-1.0.2/PKG-INFO` & `lightstreamer-client-lib-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightstreamer-client-lib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Lightstreamer Client SDK
 Author-email: Lightstreamer Srl <support@lightstreamer.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Lightstreamer/Lightstreamer-lib-client-haxe
 Keywords: lightstreamer,push,realtime,real-time
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -28,35 +28,35 @@
 python -m pip install lightstreamer-client-lib
 ```
 
 The sdk is supported on Python 3.7 and above.
 
 ## Quickstart
 
-To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
+To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
 A minimal version of the code that creates a LightstreamerClient and connects to the Lightstreamer Server on *https://push.lightstreamer.com* will look like this:
 
 ```python
 from lightstreamer.client import *
 
 client = LightstreamerClient("http://push.lightstreamer.com/","DEMO")
 client.connect()
 ```
 
-For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
+For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
 A simple Subscription containing three items and two fields to be subscribed in *MERGE* mode is easily created (see [Lightstreamer General Concepts](https://lightstreamer.com/docs/ls-server/latest/General%20Concepts.pdf)):
 
 ```python
 sub = Subscription("MERGE",["item1","item2","item3"],["stock_name","last_price"])
 sub.setDataAdapter("QUOTE_ADAPTER")
 sub.setRequestedSnapshot("yes")
 client.subscribe(sub)
 ```
 
-Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
+Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
 
 ```python
 class SubListener(SubscriptionListener):
   def onItemUpdate(self, update):
     print("UPDATE " + update.getValue("stock_name") + " " + update.getValue("last_price"))
 
   # other methods...
@@ -82,15 +82,15 @@
 client = LightstreamerClient("http://push.lightstreamer.com","DEMO")
 client.subscribe(sub)
 client.connect()
 ```
 
 ## Logging
 
-To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
+To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
 
 ```python
 import sys, logging
 
 logging.basicConfig(level=logging.DEBUG, format="%(message)s", stream=sys.stdout)
 
 loggerProvider = ConsoleLoggerProvider(ConsoleLogLevel.DEBUG)
@@ -101,15 +101,15 @@
 
 Compatible with Lightstreamer Server since version 7.3.2.
 
 ## Documentation
 
 - [Live demos](https://demos.lightstreamer.com/?p=lightstreamer&t=client&lclient=python)
 
-- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.2/index.html)
+- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.3/index.html)
 
 ## Support
 
 For questions and support please use the [Official Forum](https://forums.lightstreamer.com/). The issue list of this page is **exclusively** for bug reports and feature requests.
 
 ## License
```

### Comparing `lightstreamer-client-lib-1.0.2/README.md` & `lightstreamer-client-lib-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,35 +12,35 @@
 python -m pip install lightstreamer-client-lib
 ```
 
 The sdk is supported on Python 3.7 and above.
 
 ## Quickstart
 
-To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
+To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
 A minimal version of the code that creates a LightstreamerClient and connects to the Lightstreamer Server on *https://push.lightstreamer.com* will look like this:
 
 ```python
 from lightstreamer.client import *
 
 client = LightstreamerClient("http://push.lightstreamer.com/","DEMO")
 client.connect()
 ```
 
-For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
+For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
 A simple Subscription containing three items and two fields to be subscribed in *MERGE* mode is easily created (see [Lightstreamer General Concepts](https://lightstreamer.com/docs/ls-server/latest/General%20Concepts.pdf)):
 
 ```python
 sub = Subscription("MERGE",["item1","item2","item3"],["stock_name","last_price"])
 sub.setDataAdapter("QUOTE_ADAPTER")
 sub.setRequestedSnapshot("yes")
 client.subscribe(sub)
 ```
 
-Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
+Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
 
 ```python
 class SubListener(SubscriptionListener):
   def onItemUpdate(self, update):
     print("UPDATE " + update.getValue("stock_name") + " " + update.getValue("last_price"))
 
   # other methods...
@@ -66,15 +66,15 @@
 client = LightstreamerClient("http://push.lightstreamer.com","DEMO")
 client.subscribe(sub)
 client.connect()
 ```
 
 ## Logging
 
-To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
+To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
 
 ```python
 import sys, logging
 
 logging.basicConfig(level=logging.DEBUG, format="%(message)s", stream=sys.stdout)
 
 loggerProvider = ConsoleLoggerProvider(ConsoleLogLevel.DEBUG)
@@ -85,15 +85,15 @@
 
 Compatible with Lightstreamer Server since version 7.3.2.
 
 ## Documentation
 
 - [Live demos](https://demos.lightstreamer.com/?p=lightstreamer&t=client&lclient=python)
 
-- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.2/index.html)
+- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.3/index.html)
 
 ## Support
 
 For questions and support please use the [Official Forum](https://forums.lightstreamer.com/). The issue list of this page is **exclusively** for bug reports and feature requests.
 
 ## License
```

### Comparing `lightstreamer-client-lib-1.0.2/pyproject.toml` & `lightstreamer-client-lib-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lightstreamer-client-lib"
-version = "1.0.2"
+version = "1.0.3"
 description = "Lightstreamer Client SDK"
 readme = "README.md"
 authors = [{ name = "Lightstreamer Srl", email = "support@lightstreamer.com" }]
 license = { text = "Apache-2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3",
```

### Comparing `lightstreamer-client-lib-1.0.2/src/lightstreamer/client/com_lightstreamer_net.py` & `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/com_lightstreamer_net.py`

 * *Files identical despite different names*

### Comparing `lightstreamer-client-lib-1.0.2/src/lightstreamer/client/ls_python_client_api.py` & `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_api.py`

 * *Files identical despite different names*

### Comparing `lightstreamer-client-lib-1.0.2/src/lightstreamer/client/ls_python_client_haxe.py` & `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_haxe.py`

 * *Files 2% similar despite different names*

```diff
@@ -11082,14 +11082,21 @@
 class com_lightstreamer_internal__MacroTools_MacroTools_Fields_:
     _hx_class_name = "com.lightstreamer.internal._MacroTools.MacroTools_Fields_"
     _hx_is_interface = "False"
     __slots__ = ()
 com_lightstreamer_internal__MacroTools_MacroTools_Fields_._hx_class = com_lightstreamer_internal__MacroTools_MacroTools_Fields_
 
 
+class com_lightstreamer_internal__Macros_Macros_Fields_:
+    _hx_class_name = "com.lightstreamer.internal._Macros.Macros_Fields_"
+    _hx_is_interface = "False"
+    __slots__ = ()
+com_lightstreamer_internal__Macros_Macros_Fields_._hx_class = com_lightstreamer_internal__Macros_Macros_Fields_
+
+
 class com_lightstreamer_internal__MyList_MyList_Impl_:
     _hx_class_name = "com.lightstreamer.internal._MyList.MyList_Impl_"
     _hx_is_interface = "False"
     __slots__ = ()
     _hx_statics = ["_new", "push", "exists", "find", "contains", "removeIf"]
 
     @staticmethod
@@ -12422,30 +12429,40 @@
         return hx_concurrent_executor_Schedule("WEEKLY", 5, (day,hour,minute,second))
 hx_concurrent_executor_Schedule._hx_class = hx_concurrent_executor_Schedule
 
 
 class hx_concurrent_executor_Executor(hx_concurrent_ServiceBase):
     _hx_class_name = "hx.concurrent.executor.Executor"
     _hx_is_interface = "False"
-    __slots__ = ("onResult",)
-    _hx_fields = ["onResult"]
-    _hx_methods = ["submit", "stop"]
+    __slots__ = ("completionListeners",)
+    _hx_fields = ["completionListeners"]
+    _hx_methods = ["notifyResult", "onCompletion", "submit", "stop"]
     _hx_statics = ["NOW_ONCE", "create"]
     _hx_interfaces = []
     _hx_super = hx_concurrent_ServiceBase
 
 
     def __init__(self):
-        def _hx_local_0(result):
-            pass
-        self.onResult = _hx_local_0
+        self.completionListeners = hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArray_Impl_._new()
         super().__init__()
 
-    def submit(self,task,schedule = None):
-        raise haxe_Exception.thrown("Not implemented")
+    def notifyResult(self,result):
+        _this = self.completionListeners._items
+        listener_current = 0
+        while (listener_current < len(_this)):
+            listener = listener_current
+            listener_current = (listener_current + 1)
+            listener1 = (_this[listener] if listener >= 0 and listener < len(_this) else None)
+            try:
+                listener1(result)
+            except BaseException as _g:
+                pass
+
+    def onCompletion(self,listener):
+        self.completionListeners.add(listener)
 
     def stop(self):
         super().stop()
 
     @staticmethod
     def create(maxConcurrent = None,autostart = None):
         if (maxConcurrent is None):
@@ -12473,15 +12490,14 @@
 
     @staticmethod
     def get_isSupported():
         try:
             from threading import Thread
             return True
         except BaseException as _g:
-            None
             return False
 
     @staticmethod
     def _hx_await(condition,timeoutMS,waitLoopSleepMS = None):
         if (waitLoopSleepMS is None):
             waitLoopSleepMS = 10
         if (timeoutMS < -1):
@@ -12603,35 +12619,30 @@
                 if (t1 is None):
                     break
                 t1.cancel()
             def _hx_local_8():
                 return (_gthis._threadPool.state == hx_concurrent_ServiceState.STOPPED)
             hx_concurrent_thread_Threads._hx_await(_hx_local_8,-1)
             _gthis.set_state(hx_concurrent_ServiceState.STOPPED)
-        t = python_lib_threading_Thread(**python__KwArgs_KwArgs_Impl_.fromT(_hx_AnonObject({'target': _hx_local_9})))
-        t.daemon = True
-        t.start()
+        hx_concurrent_thread_Threads.spawn(_hx_local_9)
 
     def submit(self,task,schedule = None):
         _gthis = self
+        schedule1 = (hx_concurrent_executor_Executor.NOW_ONCE if ((schedule is None)) else schedule)
         def _hx_local_2():
             def _hx_local_1():
-                nonlocal schedule
                 if (_gthis.state != hx_concurrent_ServiceState.RUNNING):
                     raise haxe_Exception.thrown((("Cannot accept new tasks. Executor is not in state [RUNNING] but [" + Std.string(_gthis.state)) + "]."))
-                if (schedule is None):
-                    schedule = hx_concurrent_executor_Executor.NOW_ONCE
-                future = hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl(_gthis,task,schedule)
-                if (schedule is not None):
-                    if (schedule.index == 0):
-                        if future.isDue():
-                            def _hx_local_0(ctx):
-                                future.run()
-                            _gthis._threadPool.submit(_hx_local_0)
-                            return future
+                future = hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl(_gthis,task,schedule1)
+                if (schedule1.index == 0):
+                    if future.isDue():
+                        def _hx_local_0(ctx):
+                            future.run()
+                        _gthis._threadPool.submit(_hx_local_0)
+                        return future
                 _gthis._newScheduledTasks.push(future)
                 return future
             return self._stateLock.execute(_hx_local_1)
         return _hx_local_2()
 
     def stop(self):
         _gthis = self
@@ -12643,36 +12654,47 @@
 
 hx_concurrent_executor_ThreadPoolExecutor._hx_class = hx_concurrent_executor_ThreadPoolExecutor
 
 
 class hx_concurrent_thread_ThreadPool(hx_concurrent_ServiceBase):
     _hx_class_name = "hx.concurrent.thread.ThreadPool"
     _hx_is_interface = "False"
-    __slots__ = ("_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount")
-    _hx_fields = ["_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount"]
-    _hx_methods = ["get_executingTasks", "get_pendingTasks", "awaitCompletion", "cancelPendingTasks", "onStart", "submit", "stop"]
-    _hx_statics = ["_threadIDs"]
+    __slots__ = ("_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount", "pollPeriod")
+    _hx_fields = ["_spawnedThreadCount", "_workingThreadCount", "_workQueue", "threadCount", "pollPeriod"]
+    _hx_methods = ["set_pollPeriod", "get_executingTasks", "get_pendingTasks", "awaitCompletion", "cancelPendingTasks", "onStart", "submit", "stop"]
+    _hx_statics = ["DEFAULT_POLL_PERIOD", "_threadIDs"]
     _hx_interfaces = []
     _hx_super = hx_concurrent_ServiceBase
 
 
     def __init__(self,numThreads,autostart = None):
         if (autostart is None):
             autostart = True
         self.threadCount = None
+        self.pollPeriod = hx_concurrent_thread_ThreadPool.DEFAULT_POLL_PERIOD
         self._workQueue = hx_concurrent_collection_Queue()
         self._workingThreadCount = hx_concurrent_atomic__AtomicInt_AtomicIntImpl(0)
         self._spawnedThreadCount = hx_concurrent_atomic__AtomicInt_AtomicIntImpl(0)
         if (numThreads < 1):
             raise haxe_Exception.thrown("[numThreads] must be > 0")
         super().__init__()
         self.threadCount = numThreads
         if autostart:
             self.start()
 
+    def set_pollPeriod(self,value):
+        if (value <= 0):
+            raise haxe_Exception.thrown("[value] must be >= 0")
+        def _hx_local_1():
+            def _hx_local_0():
+                self.pollPeriod = value
+                return self.pollPeriod
+            return _hx_local_0()
+        return _hx_local_1()
+
     def get_executingTasks(self):
         return self._workingThreadCount.get_value()
 
     def get_pendingTasks(self):
         return self._workQueue._length.get_value()
 
     def awaitCompletion(self,timeoutMS):
@@ -12703,30 +12725,28 @@
                 _gthis._spawnedThreadCount.getAndIncrement()
                 context = hx_concurrent_thread_ThreadContext(hx_concurrent_thread_ThreadPool._threadIDs.incrementAndGet())
                 while True:
                     task = _gthis._workQueue.pop()
                     if (task is None):
                         if (_gthis.state != hx_concurrent_ServiceState.RUNNING):
                             break
-                        Sys.sleep(0.001)
+                        Sys.sleep(_gthis.pollPeriod)
                     else:
                         try:
                             _gthis._workingThreadCount.getAndIncrement()
                             task(context)
                         except BaseException as _g:
-                            None
+                            pass
                         _gthis._workingThreadCount.getAndIncrement(-1)
                 _gthis._spawnedThreadCount.getAndIncrement(-1)
                 if (_gthis._spawnedThreadCount.get_value() == 0):
                     def _hx_local_1():
                         return _gthis.set_state(hx_concurrent_ServiceState.STOPPED)
                     _gthis._stateLock.execute(_hx_local_1)
-            t = python_lib_threading_Thread(**python__KwArgs_KwArgs_Impl_.fromT(_hx_AnonObject({'target': _hx_local_2})))
-            t.daemon = True
-            t.start()
+            hx_concurrent_thread_Threads.spawn(_hx_local_2)
 
     def submit(self,task):
         _gthis = self
         if (task is None):
             raise haxe_Exception.thrown("[task] must not be null")
         def _hx_local_0():
             if (_gthis.state != hx_concurrent_ServiceState.RUNNING):
@@ -12761,14 +12781,15 @@
         self._scheduledTasks = []
         super().__init__()
         if autostart:
             self.start()
 
     def submit(self,task,schedule = None):
         _gthis = self
+        schedule1 = (hx_concurrent_executor_Executor.NOW_ONCE if ((schedule is None)) else schedule)
         def _hx_local_1():
             def _hx_local_0():
                 if (_gthis.state != hx_concurrent_ServiceState.RUNNING):
                     raise haxe_Exception.thrown((("Cannot accept new tasks. Executor is not in state [RUNNING] but [" + Std.string(_gthis.state)) + "]."))
                 i = len(_gthis._scheduledTasks)
                 while True:
                     tmp = i
@@ -12780,19 +12801,17 @@
                         pos = i
                         if (pos < 0):
                             pos = (len(_this) + pos)
                         if (pos < 0):
                             pos = 0
                         _this[pos:(pos + 1)]
                         del _this[pos:(pos + 1)]
-                future = hx_concurrent_executor__TimerExecutor_TaskFutureImpl(_gthis,task,(hx_concurrent_executor_Executor.NOW_ONCE if ((schedule is None)) else schedule))
-                if (schedule is None):
-                    _gthis._scheduledTasks.append(future)
-                elif (schedule.index == 0):
-                    _g = schedule.params[0]
+                future = hx_concurrent_executor__TimerExecutor_TaskFutureImpl(_gthis,task,schedule1)
+                if (schedule1.index == 0):
+                    _g = schedule1.params[0]
                     if (_g is None):
                         _gthis._scheduledTasks.append(future)
                     elif (_g != 0):
                         _gthis._scheduledTasks.append(future)
                 else:
                     _gthis._scheduledTasks.append(future)
                 return future
@@ -13415,15 +13434,15 @@
         else:
             return -1
 
     @staticmethod
     def allValidNames(names):
         def _hx_local_1():
             def _hx_local_0(item):
-                _this = EReg("^$| |^\\d","")
+                _this = EReg("^$| |^\\d+$","")
                 _this.matchObj = python_lib_Re.search(_this.pattern,item)
                 return (_this.matchObj is not None)
             return (not Lambda.exists(names,_hx_local_0))
         return _hx_local_1()
 
     @staticmethod
     def fromArray(array):
@@ -14092,16 +14111,15 @@
             swallowExceptions = False
         ex = None
         result = None
         self.acquire()
         try:
             result = func()
         except BaseException as _g:
-            None
-            ex = hx_concurrent_ConcurrentException(haxe_Exception.caught(_g).unwrap())
+            ex = hx_concurrent_ConcurrentException(haxe_Exception.caught(_g))
         self.release()
         if ((not swallowExceptions) and ((ex is not None))):
             ex.rethrow()
         return result
 
 hx_concurrent_lock_AbstractAcquirable._hx_class = hx_concurrent_lock_AbstractAcquirable
 
@@ -15332,81 +15350,142 @@
 
 hx_concurrent_ConcurrentException._hx_class = hx_concurrent_ConcurrentException
 
 
 class hx_concurrent_Future:
     _hx_class_name = "hx.concurrent.Future"
     _hx_is_interface = "True"
-    __slots__ = ("result", "onResult")
-    _hx_fields = ["result", "onResult"]
-    _hx_methods = ["set_onResult"]
+    __slots__ = ("result",)
+    _hx_fields = ["result"]
+    _hx_methods = ["isComplete", "onCompletion"]
 hx_concurrent_Future._hx_class = hx_concurrent_Future
 
 class hx_concurrent_FutureResult(Enum):
     __slots__ = ()
     _hx_class_name = "hx.concurrent.FutureResult"
-    _hx_constructs = ["SUCCESS", "FAILURE", "NONE"]
+    _hx_constructs = ["VALUE", "FAILURE", "PENDING"]
 
     @staticmethod
-    def SUCCESS(result,time,future):
-        return hx_concurrent_FutureResult("SUCCESS", 0, (result,time,future))
+    def VALUE(result,time,future):
+        return hx_concurrent_FutureResult("VALUE", 0, (result,time,future))
 
     @staticmethod
     def FAILURE(ex,time,future):
         return hx_concurrent_FutureResult("FAILURE", 1, (ex,time,future))
 
     @staticmethod
-    def NONE(future):
-        return hx_concurrent_FutureResult("NONE", 2, (future,))
+    def PENDING(future):
+        return hx_concurrent_FutureResult("PENDING", 2, (future,))
 hx_concurrent_FutureResult._hx_class = hx_concurrent_FutureResult
 
 
-class hx_concurrent_FutureBase:
-    _hx_class_name = "hx.concurrent.FutureBase"
+class hx_concurrent_AbstractFuture:
+    _hx_class_name = "hx.concurrent.AbstractFuture"
     _hx_is_interface = "False"
-    __slots__ = ("result", "onResult")
-    _hx_fields = ["result", "onResult"]
-    _hx_methods = ["set_onResult"]
+    __slots__ = ("completionListeners", "sync", "result")
+    _hx_fields = ["completionListeners", "sync", "result"]
+    _hx_methods = ["isComplete", "onCompletion"]
     _hx_interfaces = [hx_concurrent_Future]
 
     def __init__(self):
-        self.onResult = None
         self.result = None
-        self.result = hx_concurrent_FutureResult.NONE(self)
+        self.sync = hx_concurrent_lock_RLock()
+        self.completionListeners = list()
+        self.result = hx_concurrent_FutureResult.PENDING(self)
 
-    def set_onResult(self,fn):
-        if (fn is not None):
-            result = self.result
-            if (result.index != 2):
-                fn(result)
-        def _hx_local_1():
-            def _hx_local_0():
-                self.onResult = fn
-                return self.onResult
-            return _hx_local_0()
-        return _hx_local_1()
+    def isComplete(self):
+        if (self.result.index == 2):
+            return False
+        else:
+            return True
+
+    def onCompletion(self,listener):
+        _gthis = self
+        def _hx_local_0():
+            if (_gthis.result.index != 2):
+                listener(_gthis.result)
+            _this = _gthis.completionListeners
+            _this.append(listener)
+            return len(_this)
+        self.sync.execute(_hx_local_0)
 
-hx_concurrent_FutureBase._hx_class = hx_concurrent_FutureBase
+hx_concurrent_AbstractFuture._hx_class = hx_concurrent_AbstractFuture
 
 
-class hx_concurrent_ConstantFuture(hx_concurrent_FutureBase):
-    _hx_class_name = "hx.concurrent.ConstantFuture"
+class hx_concurrent_CompletableFuture(hx_concurrent_AbstractFuture):
+    _hx_class_name = "hx.concurrent.CompletableFuture"
     _hx_is_interface = "False"
     __slots__ = ()
     _hx_fields = []
-    _hx_methods = []
+    _hx_methods = ["complete"]
     _hx_statics = []
     _hx_interfaces = []
-    _hx_super = hx_concurrent_FutureBase
+    _hx_super = hx_concurrent_AbstractFuture
 
 
-    def __init__(self,result):
+    def __init__(self):
         super().__init__()
-        self.result = hx_concurrent_FutureResult.SUCCESS(result,(python_lib_Time.time() * 1000),self)
-hx_concurrent_ConstantFuture._hx_class = hx_concurrent_ConstantFuture
+
+    def complete(self,result,overwriteResult = None):
+        if (overwriteResult is None):
+            overwriteResult = False
+        _gthis = self
+        def _hx_local_3():
+            def _hx_local_2():
+                if (overwriteResult or (not _gthis.isComplete())):
+                    _g = result
+                    tmp = _g.index
+                    if (tmp == 0):
+                        tmp = (python_lib_Time.time() * 1000)
+                        _gthis.result = hx_concurrent_FutureResult.VALUE(_g.params[0],tmp,_gthis)
+                    elif (tmp == 1):
+                        tmp = (python_lib_Time.time() * 1000)
+                        _gthis.result = hx_concurrent_FutureResult.FAILURE(_g.params[0],tmp,_gthis)
+                    else:
+                        pass
+                    _g = 0
+                    _g1 = _gthis.completionListeners
+                    while (_g < len(_g1)):
+                        def _hx_local_1():
+                            nonlocal _g
+                            _hx_local_0 = _g
+                            _g = (_g + 1)
+                            return _hx_local_0
+                        listener = python_internal_ArrayImpl._get(_g1, _hx_local_1())
+                        try:
+                            listener(_gthis.result)
+                        except BaseException as _g2:
+                            pass
+                    return True
+                return False
+            return self.sync.execute(_hx_local_2)
+        return _hx_local_3()
+
+hx_concurrent_CompletableFuture._hx_class = hx_concurrent_CompletableFuture
+
+
+class hx_concurrent_CompletedFuture:
+    _hx_class_name = "hx.concurrent.CompletedFuture"
+    _hx_is_interface = "False"
+    __slots__ = ("result",)
+    _hx_fields = ["result"]
+    _hx_methods = ["isComplete", "onCompletion"]
+    _hx_interfaces = [hx_concurrent_Future]
+
+    def __init__(self,value):
+        self.result = None
+        self.result = hx_concurrent_FutureResult.VALUE(value,(python_lib_Time.time() * 1000),self)
+
+    def isComplete(self):
+        return True
+
+    def onCompletion(self,listener):
+        listener(self.result)
+
+hx_concurrent_CompletedFuture._hx_class = hx_concurrent_CompletedFuture
 
 class hx_concurrent_ServiceState(Enum):
     __slots__ = ()
     _hx_class_name = "hx.concurrent.ServiceState"
     _hx_constructs = ["STARTING", "RUNNING", "STOPPING", "STOPPED"]
 hx_concurrent_ServiceState.STARTING = hx_concurrent_ServiceState("STARTING", 0, ())
 hx_concurrent_ServiceState.RUNNING = hx_concurrent_ServiceState("RUNNING", 1, ())
@@ -15565,14 +15644,273 @@
 
     @staticmethod
     def toString(this1):
         return Std.string(this1.get_value())
 hx_concurrent_atomic__AtomicInt_AtomicInt_Impl_._hx_class = hx_concurrent_atomic__AtomicInt_AtomicInt_Impl_
 
 
+class hx_concurrent_collection_Collection:
+    _hx_class_name = "hx.concurrent.collection.Collection"
+    _hx_is_interface = "True"
+    __slots__ = ()
+    _hx_methods = ["get_length", "add", "addIfAbsent", "addAll", "clear", "remove", "contains", "isEmpty", "iterator", "filter", "map", "copy", "toArray", "toString", "join"]
+hx_concurrent_collection_Collection._hx_class = hx_concurrent_collection_Collection
+
+
+class hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArray_Impl_:
+    _hx_class_name = "hx.concurrent.collection._CopyOnWriteArray.CopyOnWriteArray_Impl_"
+    _hx_is_interface = "False"
+    __slots__ = ()
+    _hx_statics = ["_new", "_get", "_set"]
+
+    @staticmethod
+    def _new(initialValues = None):
+        this1 = hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArrayImpl()
+        if (initialValues is not None):
+            this1.addAll(initialValues)
+        return this1
+
+    @staticmethod
+    def _get(this1,idx):
+        return this1.get(idx)
+
+    @staticmethod
+    def _set(this1,idx,x):
+        this1._set(idx,x)
+        return x
+hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArray_Impl_._hx_class = hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArray_Impl_
+
+
+class hx_concurrent_collection_OrderedCollection:
+    _hx_class_name = "hx.concurrent.collection.OrderedCollection"
+    _hx_is_interface = "True"
+    __slots__ = ()
+    _hx_methods = ["get_first", "get_last", "insertAt", "removeAt", "removeFirst", "removeLast", "get", "indexOf", "lastIndexOf"]
+    _hx_interfaces = [hx_concurrent_collection_Collection]
+hx_concurrent_collection_OrderedCollection._hx_class = hx_concurrent_collection_OrderedCollection
+
+
+class hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArrayImpl:
+    _hx_class_name = "hx.concurrent.collection._CopyOnWriteArray.CopyOnWriteArrayImpl"
+    _hx_is_interface = "False"
+    __slots__ = ("_items", "_sync")
+    _hx_fields = ["_items", "_sync"]
+    _hx_methods = ["_set", "get_first", "get_last", "get_length", "add", "addIfAbsent", "addAll", "clear", "insertAt", "remove", "removeAt", "removeFirst", "removeLast", "copy", "contains", "isEmpty", "get", "indexOf", "lastIndexOf", "filter", "map", "join", "iterator", "toArray", "toString"]
+    _hx_interfaces = [hx_concurrent_collection_OrderedCollection]
+
+    def __init__(self):
+        self._sync = hx_concurrent_lock_RLock()
+        self._items = list()
+
+    def _set(self,idx,x):
+        _gthis = self
+        def _hx_local_0():
+            items = list(_gthis._items)
+            python_internal_ArrayImpl._set(items, idx, x)
+            _gthis._items = items
+        self._sync.execute(_hx_local_0)
+
+    def get_first(self):
+        items = self._items
+        if (len(items) == 0):
+            return None
+        else:
+            return (items[0] if 0 < len(items) else None)
+
+    def get_last(self):
+        items = self._items
+        if (len(items) == 0):
+            return None
+        else:
+            return python_internal_ArrayImpl._get(items, (len(items) - 1))
+
+    def get_length(self):
+        return len(self._items)
+
+    def add(self,x):
+        _gthis = self
+        def _hx_local_0():
+            items = list(_gthis._items)
+            items.append(x)
+            _gthis._items = items
+        self._sync.execute(_hx_local_0)
+
+    def addIfAbsent(self,x):
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                if (python_internal_ArrayImpl.indexOf(_gthis._items,x,None) > -1):
+                    return False
+                items = list(_gthis._items)
+                items.append(x)
+                _gthis._items = items
+                return True
+            return self._sync.execute(_hx_local_0)
+        return _hx_local_1()
+
+    def addAll(self,coll):
+        _gthis = self
+        def _hx_local_0():
+            items = None
+            _g = coll
+            tmp = _g.index
+            if (tmp == 0):
+                items = list(_gthis._items)
+                i = _g.params[0].iterator()
+                while i.hasNext():
+                    i1 = i.next()
+                    items.append(i1)
+            elif (tmp == 1):
+                items = (_gthis._items + _g.params[0])
+            elif (tmp == 2):
+                items = list(_gthis._items)
+                _g_head = _g.params[0].h
+                while (_g_head is not None):
+                    val = _g_head.item
+                    _g_head = _g_head.next
+                    items.append(val)
+            else:
+                pass
+            _gthis._items = items
+        self._sync.execute(_hx_local_0)
+
+    def clear(self):
+        self._items = []
+
+    def insertAt(self,idx,x):
+        _gthis = self
+        def _hx_local_0():
+            items = list(_gthis._items)
+            items.insert(idx, x)
+            return items
+        self._items = self._sync.execute(_hx_local_0)
+
+    def remove(self,x):
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                if (python_internal_ArrayImpl.indexOf(_gthis._items,x,None) == -1):
+                    return False
+                items = list(_gthis._items)
+                removed = python_internal_ArrayImpl.remove(items,x)
+                _gthis._items = items
+                return removed
+            return self._sync.execute(_hx_local_0)
+        return _hx_local_1()
+
+    def removeAt(self,idx,throwIfOutOfRange = None):
+        if (throwIfOutOfRange is None):
+            throwIfOutOfRange = False
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                if ((idx < 0) or ((idx >= len(_gthis._items)))):
+                    if throwIfOutOfRange:
+                        raise haxe_Exception.thrown("Index out of range.")
+                    return None
+                items = list(_gthis._items)
+                pos = idx
+                if (pos < 0):
+                    pos = (len(items) + pos)
+                if (pos < 0):
+                    pos = 0
+                res = items[pos:(pos + 1)]
+                del items[pos:(pos + 1)]
+                _gthis._items = items
+                if (len(res) == 0):
+                    return None
+                else:
+                    return (res[0] if 0 < len(res) else None)
+            return self._sync.execute(_hx_local_0)
+        return _hx_local_1()
+
+    def removeFirst(self,throwIfEmpty = None):
+        if (throwIfEmpty is None):
+            throwIfEmpty = False
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                if (len(_gthis._items) == 0):
+                    if throwIfEmpty:
+                        raise haxe_Exception.thrown("This collection is empty.")
+                    return None
+                items = list(_gthis._items)
+                removed = (None if ((len(items) == 0)) else items.pop(0))
+                _gthis._items = items
+                return removed
+            return self._sync.execute(_hx_local_0)
+        return _hx_local_1()
+
+    def removeLast(self,throwIfEmpty = None):
+        if (throwIfEmpty is None):
+            throwIfEmpty = False
+        _gthis = self
+        def _hx_local_1():
+            def _hx_local_0():
+                if (len(_gthis._items) == 0):
+                    if throwIfEmpty:
+                        raise haxe_Exception.thrown("This collection is empty.")
+                    return None
+                items = list(_gthis._items)
+                removed = (None if ((len(items) == 0)) else items.pop())
+                _gthis._items = items
+                return removed
+            return self._sync.execute(_hx_local_0)
+        return _hx_local_1()
+
+    def copy(self):
+        return hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArray_Impl_._new(hx_concurrent_internal__Either3__Either3.b(list(self._items)))
+
+    def contains(self,x):
+        return (python_internal_ArrayImpl.indexOf(self._items,x,0) > -1)
+
+    def isEmpty(self):
+        return (len(self._items) == 0)
+
+    def get(self,idx,throwIfOutOfRange = None):
+        if (throwIfOutOfRange is None):
+            throwIfOutOfRange = False
+        items = self._items
+        if ((idx < 0) or ((idx >= len(items)))):
+            if throwIfOutOfRange:
+                raise haxe_Exception.thrown("Index out of range.")
+            return None
+        return (items[idx] if idx >= 0 and idx < len(items) else None)
+
+    def indexOf(self,x,startAt = None):
+        if (startAt is None):
+            startAt = 0
+        return python_internal_ArrayImpl.indexOf(self._items,x,startAt)
+
+    def lastIndexOf(self,x,startAt = None):
+        return python_internal_ArrayImpl.lastIndexOf(self._items,x,startAt)
+
+    def filter(self,fn):
+        return hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArray_Impl_._new(hx_concurrent_internal__Either3__Either3.b(list(filter(fn,self._items))))
+
+    def map(self,fn):
+        return hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArray_Impl_._new(hx_concurrent_internal__Either3__Either3.b(list(map(fn,self._items))))
+
+    def join(self,sep):
+        _this = self._items
+        return sep.join([python_Boot.toString1(x1,'') for x1 in _this])
+
+    def iterator(self):
+        return haxe_iterators_ArrayIterator(self._items)
+
+    def toArray(self):
+        return list(self._items)
+
+    def toString(self):
+        _this = self._items
+        return (("[" + HxOverrides.stringOrNull(",".join([python_Boot.toString1(x1,'') for x1 in _this]))) + "]")
+
+hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArrayImpl._hx_class = hx_concurrent_collection__CopyOnWriteArray_CopyOnWriteArrayImpl
+
+
 class hx_concurrent_collection_Queue:
     _hx_class_name = "hx.concurrent.collection.Queue"
     _hx_is_interface = "False"
     __slots__ = ("_queue", "_length")
     _hx_fields = ["_queue", "_length"]
     _hx_methods = ["get_length", "pop", "pushHead", "push"]
 
@@ -15595,24 +15933,22 @@
         msg = None
         if (timeoutMS < -1):
             raise haxe_Exception.thrown("[timeoutMS] must be >= -1")
         if (timeoutMS == 0):
             try:
                 msg = Reflect.field(self._queue,"pop")()
             except BaseException as _g:
-                None
                 msg = None
         else:
             def _hx_local_0():
                 nonlocal msg
                 nonlocal msg
                 try:
                     msg = Reflect.field(_gthis._queue,"pop")()
                 except BaseException as _g:
-                    None
                     msg = None
                 return (msg is not None)
             hx_concurrent_thread_Threads._hx_await(_hx_local_0,timeoutMS)
         if (msg is not None):
             self._length.getAndIncrement(-1)
         return msg
 
@@ -15632,28 +15968,28 @@
 
 
 class hx_concurrent_executor_TaskFuture:
     _hx_class_name = "hx.concurrent.executor.TaskFuture"
     _hx_is_interface = "True"
     __slots__ = ("schedule", "isStopped")
     _hx_fields = ["schedule", "isStopped"]
-    _hx_methods = ["cancel", "waitAndGet"]
+    _hx_methods = ["cancel", "awaitCompletion"]
     _hx_interfaces = [hx_concurrent_Future]
 hx_concurrent_executor_TaskFuture._hx_class = hx_concurrent_executor_TaskFuture
 
 
-class hx_concurrent_executor_TaskFutureBase(hx_concurrent_FutureBase):
-    _hx_class_name = "hx.concurrent.executor.TaskFutureBase"
+class hx_concurrent_executor_AbstractTaskFuture(hx_concurrent_CompletableFuture):
+    _hx_class_name = "hx.concurrent.executor.AbstractTaskFuture"
     _hx_is_interface = "False"
     __slots__ = ("schedule", "isStopped", "_executor", "_task")
     _hx_fields = ["schedule", "isStopped", "_executor", "_task"]
-    _hx_methods = ["cancel", "waitAndGet"]
+    _hx_methods = ["cancel", "awaitCompletion"]
     _hx_statics = []
     _hx_interfaces = [hx_concurrent_executor_TaskFuture]
-    _hx_super = hx_concurrent_FutureBase
+    _hx_super = hx_concurrent_CompletableFuture
 
 
     def __init__(self,executor,task,schedule):
         self._task = None
         self._executor = None
         self.schedule = None
         self.isStopped = False
@@ -15661,25 +15997,22 @@
         self._executor = executor
         self._task = task
         self.schedule = hx_concurrent_executor_ScheduleTools.assertValid(schedule)
 
     def cancel(self):
         self.isStopped = True
 
-    def waitAndGet(self,timeoutMS):
+    def awaitCompletion(self,timeoutMS):
         _gthis = self
         def _hx_local_0():
-            if (_gthis.result.index == 2):
-                return False
-            else:
-                return True
+            return _gthis.isComplete()
         hx_concurrent_thread_Threads._hx_await(_hx_local_0,timeoutMS,10)
         return self.result
 
-hx_concurrent_executor_TaskFutureBase._hx_class = hx_concurrent_executor_TaskFutureBase
+hx_concurrent_executor_AbstractTaskFuture._hx_class = hx_concurrent_executor_AbstractTaskFuture
 
 
 class hx_concurrent_executor_ScheduleTools:
     _hx_class_name = "hx.concurrent.executor.ScheduleTools"
     _hx_is_interface = "False"
     __slots__ = ()
     _hx_statics = ["HOUR_IN_MS", "DAY_IN_MS", "WEEK_IN_MS", "applyDefaults", "assertValid", "firstRunAt"]
@@ -15802,23 +16135,23 @@
             else:
                 return ((nowMS + ((((runAtSecondOfDay - elapsedSecondsToday)) * 1000))) + ((86400000 * ((7 - ((dayIndex - now.date.day)))))))
         else:
             pass
 hx_concurrent_executor_ScheduleTools._hx_class = hx_concurrent_executor_ScheduleTools
 
 
-class hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl(hx_concurrent_executor_TaskFutureBase):
+class hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl(hx_concurrent_executor_AbstractTaskFuture):
     _hx_class_name = "hx.concurrent.executor._ThreadPoolExecutor.TaskFutureImpl"
     _hx_is_interface = "False"
     __slots__ = ("_nextRunAt",)
     _hx_fields = ["_nextRunAt"]
     _hx_methods = ["isDue", "run"]
     _hx_statics = []
     _hx_interfaces = []
-    _hx_super = hx_concurrent_executor_TaskFutureBase
+    _hx_super = hx_concurrent_executor_AbstractTaskFuture
 
 
     def __init__(self,executor,task,schedule):
         self._nextRunAt = None
         super().__init__(executor,task,schedule)
         self._nextRunAt = hx_concurrent_executor_ScheduleTools.firstRunAt(self.schedule)
 
@@ -15856,64 +16189,50 @@
                 pass
             return True
         return False
 
     def run(self):
         if self.isStopped:
             return
-        result = hx_concurrent_FutureResult.NONE(self)
+        fnResult = None
         try:
-            resultValue = None
             _g = self._task
-            resultValue1 = _g.index
-            if (resultValue1 == 0):
-                resultValue = _g.params[0]()
-            elif (resultValue1 == 1):
+            fnResult1 = _g.index
+            if (fnResult1 == 0):
+                fnResult = hx_concurrent_internal__Either2__Either2.a(_g.params[0]())
+            elif (fnResult1 == 1):
                 _g.params[0]()
-                resultValue = None
+                fnResult = None
             else:
                 pass
-            result = hx_concurrent_FutureResult.SUCCESS(resultValue,(python_lib_Time.time() * 1000),self)
         except BaseException as _g:
-            None
-            result = hx_concurrent_FutureResult.FAILURE(hx_concurrent_ConcurrentException(haxe_Exception.caught(_g).unwrap()),(python_lib_Time.time() * 1000),self)
+            fnResult = hx_concurrent_internal__Either2__Either2.b(hx_concurrent_ConcurrentException(haxe_Exception.caught(_g)))
         _g = self.schedule
         tmp = _g.index
         if (tmp == 0):
             self.isStopped = True
         elif (tmp == 1):
             self._nextRunAt = ((python_lib_Time.time() * 1000) + _g.params[0])
         else:
             pass
-        self.result = result
-        fn = self.onResult
-        if (fn is not None):
-            try:
-                fn(result)
-            except BaseException as _g:
-                None
-        fn = self._executor.onResult
-        if (fn is not None):
-            try:
-                fn(result)
-            except BaseException as _g:
-                None
+        self.complete(fnResult,True)
+        self._executor.notifyResult(self.result)
 
 hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl._hx_class = hx_concurrent_executor__ThreadPoolExecutor_TaskFutureImpl
 
 
-class hx_concurrent_executor__TimerExecutor_TaskFutureImpl(hx_concurrent_executor_TaskFutureBase):
+class hx_concurrent_executor__TimerExecutor_TaskFutureImpl(hx_concurrent_executor_AbstractTaskFuture):
     _hx_class_name = "hx.concurrent.executor._TimerExecutor.TaskFutureImpl"
     _hx_is_interface = "False"
     __slots__ = ("_timer",)
     _hx_fields = ["_timer"]
     _hx_methods = ["run", "cancel"]
     _hx_statics = []
     _hx_interfaces = []
-    _hx_super = hx_concurrent_executor_TaskFutureBase
+    _hx_super = hx_concurrent_executor_AbstractTaskFuture
 
 
     def __init__(self,executor,task,schedule):
         self._timer = None
         super().__init__(executor,task,schedule)
         x = (hx_concurrent_executor_ScheduleTools.firstRunAt(self.schedule) - ((python_lib_Time.time() * 1000)))
         initialDelay = None
@@ -15944,51 +16263,37 @@
                 t.run = self.run
             elif (tmp == 5):
                 t = haxe_Timer(604800000)
                 t.run = self.run
             else:
                 pass
             self._timer = t
-        result = hx_concurrent_FutureResult.NONE(self)
+        fnResult = None
         try:
-            resultValue = None
             _g = self._task
-            resultValue1 = _g.index
-            if (resultValue1 == 0):
-                resultValue = _g.params[0]()
-            elif (resultValue1 == 1):
+            fnResult1 = _g.index
+            if (fnResult1 == 0):
+                fnResult = hx_concurrent_internal__Either2__Either2.a(_g.params[0]())
+            elif (fnResult1 == 1):
                 _g.params[0]()
-                resultValue = None
+                fnResult = None
             else:
                 pass
-            result = hx_concurrent_FutureResult.SUCCESS(resultValue,(python_lib_Time.time() * 1000),self)
         except BaseException as _g:
-            None
-            result = hx_concurrent_FutureResult.FAILURE(hx_concurrent_ConcurrentException(haxe_Exception.caught(_g).unwrap()),(python_lib_Time.time() * 1000),self)
+            fnResult = hx_concurrent_internal__Either2__Either2.b(hx_concurrent_ConcurrentException(haxe_Exception.caught(_g)))
         _g = self.schedule
         tmp = _g.index
         if (tmp == 0):
             self.isStopped = True
         elif (tmp == 1):
             self._timer = haxe_Timer.delay(self.run,_g.params[0])
         else:
             pass
-        self.result = result
-        fn = self.onResult
-        if (fn is not None):
-            try:
-                fn(result)
-            except BaseException as _g:
-                None
-        fn = self._executor.onResult
-        if (fn is not None):
-            try:
-                fn(result)
-            except BaseException as _g:
-                None
+        self.complete(fnResult,True)
+        self._executor.notifyResult(self.result)
 
     def cancel(self):
         t = self._timer
         if (t is not None):
             t.stop()
         super().cancel()
 
@@ -16046,14 +16351,61 @@
 
     @staticmethod
     def b(v):
         return hx_concurrent_internal__Either2__Either2("b", 1, (v,))
 hx_concurrent_internal__Either2__Either2._hx_class = hx_concurrent_internal__Either2__Either2
 
 
+class hx_concurrent_internal__Either3_Either3_Impl_:
+    _hx_class_name = "hx.concurrent.internal._Either3.Either3_Impl_"
+    _hx_is_interface = "False"
+    __slots__ = ()
+    _hx_statics = ["_new", "get_value", "fromA", "fromB", "fromC"]
+    value = None
+
+    @staticmethod
+    def _new(value):
+        return value
+
+    @staticmethod
+    def get_value(this1):
+        return this1
+
+    @staticmethod
+    def fromA(value):
+        return hx_concurrent_internal__Either3__Either3.a(value)
+
+    @staticmethod
+    def fromB(value):
+        return hx_concurrent_internal__Either3__Either3.b(value)
+
+    @staticmethod
+    def fromC(value):
+        return hx_concurrent_internal__Either3__Either3.c(value)
+hx_concurrent_internal__Either3_Either3_Impl_._hx_class = hx_concurrent_internal__Either3_Either3_Impl_
+
+class hx_concurrent_internal__Either3__Either3(Enum):
+    __slots__ = ()
+    _hx_class_name = "hx.concurrent.internal._Either3._Either3"
+    _hx_constructs = ["a", "b", "c"]
+
+    @staticmethod
+    def a(v):
+        return hx_concurrent_internal__Either3__Either3("a", 0, (v,))
+
+    @staticmethod
+    def b(v):
+        return hx_concurrent_internal__Either3__Either3("b", 1, (v,))
+
+    @staticmethod
+    def c(v):
+        return hx_concurrent_internal__Either3__Either3("c", 2, (v,))
+hx_concurrent_internal__Either3__Either3._hx_class = hx_concurrent_internal__Either3__Either3
+
+
 class hx_concurrent_thread_ThreadContext:
     _hx_class_name = "hx.concurrent.thread.ThreadContext"
     _hx_is_interface = "False"
     __slots__ = ("id", "vars")
     _hx_fields = ["id", "vars"]
 
     def __init__(self,id):
@@ -16427,16 +16779,16 @@
 sys_thread__Thread_HxThread.threadsMutex = sys_thread_Mutex()
 sys_thread__Thread_HxThread.mainThread = sys_thread__Thread_HxThread(python_lib_Threading.current_thread())
 sys_thread__Thread_HxThread.mainThread.events = sys_thread_EventLoop()
 
 com_lightstreamer_client__ConnectionDetails_ConnectionDetails_Fields_.DEFAULT_SERVER = None
 com_lightstreamer_internal__Constants_Constants_Fields_.TLCP_VERSION = "TLCP-2.4.0"
 com_lightstreamer_internal__Constants_Constants_Fields_.FULL_TLCP_VERSION = (HxOverrides.stringOrNull(com_lightstreamer_internal__Constants_Constants_Fields_.TLCP_VERSION) + ".lightstreamer.com")
-com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_VERSION = (("1.0.2" + " build ") + "20230405")
-com_lightstreamer_internal__Constants_Constants_Fields_.LS_CID = "v Wntytg4pkpW36AK3O4hwLri8M4OA66fBv"
+com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_VERSION = (("1.0.3" + " build ") + "20230622")
+com_lightstreamer_internal__Constants_Constants_Fields_.LS_CID = "v Wntytg4pkpW36AK3P4hwLri8M4OA68h8x"
 com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_NAME = "python_client"
 com_lightstreamer_internal__Constants_Constants_Fields_.LS_CREATE_REALM = ""
 LSLightstreamerClient.LIB_NAME = com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_NAME
 LSLightstreamerClient.LIB_VERSION = com_lightstreamer_internal__Constants_Constants_Fields_.LS_LIB_VERSION
 com_lightstreamer_client__Proxy_ProxyType_Impl_.HTTP = "HTTP"
 com_lightstreamer_client__Proxy_ProxyType_Impl_.SOCKS4 = "SOCKS4"
 com_lightstreamer_client__Proxy_ProxyType_Impl_.SOCKS5 = "SOCKS5"
@@ -16448,14 +16800,15 @@
 python_Boot.keywords = set(["and", "del", "from", "not", "with", "as", "elif", "global", "or", "yield", "assert", "else", "if", "pass", "None", "break", "except", "import", "raise", "True", "class", "exec", "in", "return", "False", "continue", "finally", "is", "try", "def", "for", "lambda", "while"])
 python_Boot.prefixLength = len("_hx_")
 python_Lib.lineEnd = ("\r\n" if ((Sys.systemName() == "Windows")) else "\n")
 hx_concurrent_ServiceBase._ids = hx_concurrent_atomic__AtomicInt_AtomicIntImpl(0)
 hx_concurrent_executor_Executor.NOW_ONCE = hx_concurrent_executor_Schedule.ONCE(0)
 hx_concurrent_executor_ThreadPoolExecutor.SCHEDULER_RESOLUTION_MS = 10
 hx_concurrent_executor_ThreadPoolExecutor.SCHEDULER_RESOLUTION_SEC = 0.01
+hx_concurrent_thread_ThreadPool.DEFAULT_POLL_PERIOD = 0.001
 hx_concurrent_thread_ThreadPool._threadIDs = hx_concurrent_atomic__AtomicInt_AtomicIntImpl(0)
 com_lightstreamer_internal__Threads_Threads_Fields_.userThread = com_lightstreamer_internal__Threads_Threads_Fields_.createExecutor()
 com_lightstreamer_internal__Threads_Threads_Fields_.sessionThread = com_lightstreamer_internal__Threads_Threads_Fields_.createExecutor()
 com_lightstreamer_internal__Types_Millis_Impl_.ZERO = 0
 com_lightstreamer_internal__Types_TransportSelection_Impl_.WS = "WS"
 com_lightstreamer_internal__Types_TransportSelection_Impl_.WS_STREAMING = "WS-STREAMING"
 com_lightstreamer_internal__Types_TransportSelection_Impl_.WS_POLLING = "WS-POLLING"
```

### Comparing `lightstreamer-client-lib-1.0.2/src/lightstreamer/client/ls_python_client_wrapper.py` & `lightstreamer-client-lib-1.0.3/src/lightstreamer/client/ls_python_client_wrapper.py`

 * *Files identical despite different names*

### Comparing `lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/PKG-INFO` & `lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightstreamer-client-lib
-Version: 1.0.2
+Version: 1.0.3
 Summary: Lightstreamer Client SDK
 Author-email: Lightstreamer Srl <support@lightstreamer.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Lightstreamer/Lightstreamer-lib-client-haxe
 Keywords: lightstreamer,push,realtime,real-time
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -28,35 +28,35 @@
 python -m pip install lightstreamer-client-lib
 ```
 
 The sdk is supported on Python 3.7 and above.
 
 ## Quickstart
 
-To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
+To connect to a Lightstreamer Server, a [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient) object has to be created, configured, and instructed to connect to the Lightstreamer Server. 
 A minimal version of the code that creates a LightstreamerClient and connects to the Lightstreamer Server on *https://push.lightstreamer.com* will look like this:
 
 ```python
 from lightstreamer.client import *
 
 client = LightstreamerClient("http://push.lightstreamer.com/","DEMO")
 client.connect()
 ```
 
-For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
+For each subscription to be subscribed to a Lightstreamer Server a [Subscription](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.Subscription) instance is needed.
 A simple Subscription containing three items and two fields to be subscribed in *MERGE* mode is easily created (see [Lightstreamer General Concepts](https://lightstreamer.com/docs/ls-server/latest/General%20Concepts.pdf)):
 
 ```python
 sub = Subscription("MERGE",["item1","item2","item3"],["stock_name","last_price"])
 sub.setDataAdapter("QUOTE_ADAPTER")
 sub.setRequestedSnapshot("yes")
 client.subscribe(sub)
 ```
 
-Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
+Before sending the subscription to the server, usually at least one [SubscriptionListener](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.SubscriptionListener) is attached to the Subscription instance in order to consume the real-time updates. The following code shows the values of the fields *stock_name* and *last_price* each time a new update is received for the subscription:
 
 ```python
 class SubListener(SubscriptionListener):
   def onItemUpdate(self, update):
     print("UPDATE " + update.getValue("stock_name") + " " + update.getValue("last_price"))
 
   # other methods...
@@ -82,15 +82,15 @@
 client = LightstreamerClient("http://push.lightstreamer.com","DEMO")
 client.subscribe(sub)
 client.connect()
 ```
 
 ## Logging
 
-To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.2/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
+To enable the internal client logger, create a [LoggerProvider](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_api.LoggerProvider) and set it as the default provider of [LightstreamerClient](https://lightstreamer.com/api/ls-python-client/1.0.3/lightstreamer.html#lightstreamer.client.ls_python_client_wrapper.LightstreamerClient.setLoggerProvider).
 
 ```python
 import sys, logging
 
 logging.basicConfig(level=logging.DEBUG, format="%(message)s", stream=sys.stdout)
 
 loggerProvider = ConsoleLoggerProvider(ConsoleLogLevel.DEBUG)
@@ -101,15 +101,15 @@
 
 Compatible with Lightstreamer Server since version 7.3.2.
 
 ## Documentation
 
 - [Live demos](https://demos.lightstreamer.com/?p=lightstreamer&t=client&lclient=python)
 
-- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.2/index.html)
+- [API Reference](https://lightstreamer.com/api/ls-python-client/1.0.3/index.html)
 
 ## Support
 
 For questions and support please use the [Official Forum](https://forums.lightstreamer.com/). The issue list of this page is **exclusively** for bug reports and feature requests.
 
 ## License
```

### Comparing `lightstreamer-client-lib-1.0.2/src/lightstreamer_client_lib.egg-info/SOURCES.txt` & `lightstreamer-client-lib-1.0.3/src/lightstreamer_client_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

