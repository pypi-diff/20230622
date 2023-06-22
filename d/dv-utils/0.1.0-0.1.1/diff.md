# Comparing `tmp/dv_utils-0.1.0.tar.gz` & `tmp/dv_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dv_utils-0.1.0.tar", max compression
+gzip compressed data, was "dv_utils-0.1.1.tar", max compression
```

## Comparing `dv_utils-0.1.0.tar` & `dv_utils-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      622 2022-09-23 12:38:21.911471 dv_utils-0.1.0/README.md
--rw-r--r--   0        0        0      378 2023-04-26 12:10:23.887056 dv_utils-0.1.0/dv_utils/__init__.py
--rw-r--r--   0        0        0      452 2023-04-26 10:45:42.041117 dv_utils-0.1.0/dv_utils/__main__.py
--rw-r--r--   0        0        0     3239 2023-02-20 08:24:19.300581 dv_utils-0.1.0/dv_utils/client.py
--rw-r--r--   0        0        0     1657 2023-06-20 13:55:12.304286 dv_utils-0.1.0/dv_utils/listener.py
--rw-r--r--   0        0        0     1932 2023-04-26 12:04:07.208975 dv_utils-0.1.0/dv_utils/log_utils.py
--rw-r--r--   0        0        0     1521 2022-08-05 13:05:56.151683 dv_utils-0.1.0/dv_utils/process.py
--rw-r--r--   0        0        0     2813 2023-06-20 13:29:43.364033 dv_utils-0.1.0/dv_utils/redis.py
--rw-r--r--   0        0        0     1413 2022-08-05 13:04:09.726787 dv_utils-0.1.0/dv_utils/settings.py
--rw-r--r--   0        0        0     1186 2023-06-20 13:55:34.100458 dv_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 dv_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      622 2022-09-23 12:38:21.911471 dv_utils-0.1.1/README.md
+-rw-r--r--   0        0        0      378 2023-04-26 12:10:23.887056 dv_utils-0.1.1/dv_utils/__init__.py
+-rw-r--r--   0        0        0      452 2023-04-26 10:45:42.041117 dv_utils-0.1.1/dv_utils/__main__.py
+-rw-r--r--   0        0        0     3239 2023-02-20 08:24:19.300581 dv_utils-0.1.1/dv_utils/client.py
+-rw-r--r--   0        0        0     1664 2023-06-22 09:39:59.081720 dv_utils-0.1.1/dv_utils/listener.py
+-rw-r--r--   0        0        0     1932 2023-04-26 12:04:07.208975 dv_utils-0.1.1/dv_utils/log_utils.py
+-rw-r--r--   0        0        0     1521 2022-08-05 13:05:56.151683 dv_utils-0.1.1/dv_utils/process.py
+-rw-r--r--   0        0        0     2813 2023-06-20 13:29:43.364033 dv_utils-0.1.1/dv_utils/redis.py
+-rw-r--r--   0        0        0     1413 2022-08-05 13:04:09.726787 dv_utils-0.1.1/dv_utils/settings.py
+-rw-r--r--   0        0        0     1186 2023-06-22 09:40:09.149811 dv_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1514 1970-01-01 00:00:00.000000 dv_utils-0.1.1/PKG-INFO
```

### Comparing `dv_utils-0.1.0/README.md` & `dv_utils-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.0/dv_utils/client.py` & `dv_utils-0.1.1/dv_utils/client.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.0/dv_utils/listener.py` & `dv_utils-0.1.1/dv_utils/listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         redis_queue = RedisQueue()
         redis_queue.create_consummer_group()
 
         if(daemon):
            audit_log(log="Algo Event Listener started", app="algo")
 
         while True:
-           evt = self.listen_once(timeout)
+           evt = redis_queue.listen_once(timeout)
            if evt:
                start = time.time()
                evt_type =evt.get("type", "MISSING_TYPE")
                if(log_events):
                   audit_log("Event processing started", evt=evt_type, state="STARTED", app="algo")
 
                try:
```

### Comparing `dv_utils-0.1.0/dv_utils/log_utils.py` & `dv_utils-0.1.1/dv_utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.0/dv_utils/process.py` & `dv_utils-0.1.1/dv_utils/process.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.0/dv_utils/redis.py` & `dv_utils-0.1.1/dv_utils/redis.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.0/dv_utils/settings.py` & `dv_utils-0.1.1/dv_utils/settings.py`

 * *Files identical despite different names*

### Comparing `dv_utils-0.1.0/pyproject.toml` & `dv_utils-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry>=0.12", "setuptools>=40.8.0"]
 build-backend = "poetry.masonry.api"
 
 [tool]
 [tool.poetry]
 name = "dv-utils"
-version = "0.1.0"
+version = "0.1.1"
 description = "DataVillage Python utils for interaction with the middleware and building algo processing code"
 authors = ["Loic Quertenmont <loic@deeperanalytics.be>"]
 readme = "README.md"
 repository = "https://github.com/datavillage-me/dv-utils"
 
 [tool.poetry.dependencies]
 python = ">=3.10.4,<4"
```

### Comparing `dv_utils-0.1.0/PKG-INFO` & `dv_utils-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dv-utils
-Version: 0.1.0
+Version: 0.1.1
 Summary: DataVillage Python utils for interaction with the middleware and building algo processing code
 Home-page: https://github.com/datavillage-me/dv-utils
 Author: Loic Quertenmont
 Author-email: loic@deeperanalytics.be
 Requires-Python: >=3.10.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

