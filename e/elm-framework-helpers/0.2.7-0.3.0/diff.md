# Comparing `tmp/elm_framework_helpers-0.2.7.tar.gz` & `tmp/elm_framework_helpers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm_framework_helpers-0.2.7.tar", max compression
+gzip compressed data, was "elm_framework_helpers-0.3.0.tar", max compression
```

## Comparing `elm_framework_helpers-0.2.7.tar` & `elm_framework_helpers-0.3.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
--rw-r--r--   0        0        0      422 2023-02-22 05:45:01.637717 elm_framework_helpers-0.2.7/README.md
--rw-r--r--   0        0        0        0 2023-01-20 07:35:05.428027 elm_framework_helpers-0.2.7/elm_framework_helpers/__init__.py
--rw-r--r--   0        0        0      216 2023-01-20 09:37:21.214396 elm_framework_helpers-0.2.7/elm_framework_helpers/ccxt/__init__.py
--rw-r--r--   0        0        0      280 2023-02-25 04:57:26.776325 elm_framework_helpers-0.2.7/elm_framework_helpers/ccxt/models/orderbook.py
--rw-r--r--   0        0        0      702 2023-01-27 07:21:57.204998 elm_framework_helpers-0.2.7/elm_framework_helpers/ccxt/orderbook/extract.py
--rw-r--r--   0        0        0      303 2023-02-11 02:14:42.708856 elm_framework_helpers-0.2.7/elm_framework_helpers/config.py
--rw-r--r--   0        0        0        0 2023-02-22 05:45:01.637717 elm_framework_helpers-0.2.7/elm_framework_helpers/http/__init__.py
--rw-r--r--   0        0        0      609 2023-02-22 05:45:01.637717 elm_framework_helpers-0.2.7/elm_framework_helpers/http/threaded_server.py
--rw-r--r--   0        0        0      232 2023-02-22 05:45:01.637717 elm_framework_helpers-0.2.7/elm_framework_helpers/json/__init__.py
--rw-r--r--   0        0        0      140 2023-02-22 05:45:01.637717 elm_framework_helpers-0.2.7/elm_framework_helpers/logging.py
--rw-r--r--   0        0        0      248 2023-03-23 07:35:43.494903 elm_framework_helpers-0.2.7/elm_framework_helpers/operators/__init__.py
--rw-r--r--   0        0        0      114 2023-01-27 07:21:57.204998 elm_framework_helpers-0.2.7/elm_framework_helpers/operators/ignore_errors_.py
--rw-r--r--   0        0        0      243 2023-01-23 09:07:09.378554 elm_framework_helpers-0.2.7/elm_framework_helpers/operators/item_at_index_.py
--rw-r--r--   0        0        0     1229 2023-03-23 08:02:14.524660 elm_framework_helpers-0.2.7/elm_framework_helpers/operators/manual_value_or.py
--rw-r--r--   0        0        0     2919 2023-03-12 05:47:22.415439 elm_framework_helpers-0.2.7/elm_framework_helpers/operators/retry_with_delay.py
--rw-r--r--   0        0        0     2305 2023-02-22 05:45:01.647717 elm_framework_helpers-0.2.7/elm_framework_helpers/output/__init__.py
--rw-r--r--   0        0        0      396 2023-02-22 05:44:33.006180 elm_framework_helpers-0.2.7/elm_framework_helpers/schedulers/__init__.py
--rw-r--r--   0        0        0     2365 2023-03-05 07:12:13.951311 elm_framework_helpers-0.2.7/elm_framework_helpers/strategies/binance_tester.py
--rw-r--r--   0        0        0     1877 2023-01-27 08:37:22.897847 elm_framework_helpers-0.2.7/elm_framework_helpers/strategies/grid/orders.py
--rw-r--r--   0        0        0      443 2023-03-12 06:18:21.261532 elm_framework_helpers-0.2.7/elm_framework_helpers/testing/__init__.py
--rw-r--r--   0        0        0     2193 2023-03-12 06:33:19.455778 elm_framework_helpers-0.2.7/elm_framework_helpers/testing/log_to_observable.py
--rw-r--r--   0        0        0      137 2023-03-12 05:53:54.169432 elm_framework_helpers-0.2.7/elm_framework_helpers/testing/pytest/test_scheduler.py
--rw-r--r--   0        0        0      656 2023-03-12 06:21:46.729895 elm_framework_helpers-0.2.7/elm_framework_helpers/testing/reactivex_assertion.py
--rw-r--r--   0        0        0      192 2023-02-25 04:57:35.666325 elm_framework_helpers-0.2.7/elm_framework_helpers/unified/models/book.py
--rw-r--r--   0        0        0     1259 2023-02-25 02:54:19.534869 elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/__init__.py
--rw-r--r--   0        0        0      473 2023-02-25 02:38:35.310463 elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/bundle.py
--rw-r--r--   0        0        0     1762 2023-03-05 03:52:38.378403 elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/enhanced_websocket.py
--rw-r--r--   0        0        0      245 2023-02-25 02:38:35.310463 elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/message_types.py
--rw-r--r--   0        0        0      782 2023-02-25 02:52:49.680984 elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/status.py
--rw-r--r--   0        0        0        0 2023-02-25 02:54:45.426117 elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/operators/__init__.py
--rw-r--r--   0        0        0     2012 2023-02-25 03:01:41.660181 elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/operators/connection_operators.py
--rw-r--r--   0        0        0     1401 2023-03-23 08:02:34.765883 elm_framework_helpers-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 elm_framework_helpers-0.2.7/setup.py
--rw-r--r--   0        0        0     1421 1970-01-01 00:00:00.000000 elm_framework_helpers-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      422 2023-02-22 05:45:01.637717 elm_framework_helpers-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-01-20 07:35:05.428027 elm_framework_helpers-0.3.0/elm_framework_helpers/__init__.py
+-rw-r--r--   0        0        0      216 2023-01-20 09:37:21.214396 elm_framework_helpers-0.3.0/elm_framework_helpers/ccxt/__init__.py
+-rw-r--r--   0        0        0      280 2023-02-25 04:57:26.776325 elm_framework_helpers-0.3.0/elm_framework_helpers/ccxt/models/orderbook.py
+-rw-r--r--   0        0        0      702 2023-01-27 07:21:57.204998 elm_framework_helpers-0.3.0/elm_framework_helpers/ccxt/orderbook/extract.py
+-rw-r--r--   0        0        0      303 2023-02-11 02:14:42.708856 elm_framework_helpers-0.3.0/elm_framework_helpers/config.py
+-rw-r--r--   0        0        0        0 2023-02-22 05:45:01.637717 elm_framework_helpers-0.3.0/elm_framework_helpers/http/__init__.py
+-rw-r--r--   0        0        0      609 2023-02-22 05:45:01.637717 elm_framework_helpers-0.3.0/elm_framework_helpers/http/threaded_server.py
+-rw-r--r--   0        0        0      232 2023-02-22 05:45:01.637717 elm_framework_helpers-0.3.0/elm_framework_helpers/json/__init__.py
+-rw-r--r--   0        0        0      140 2023-02-22 05:45:01.637717 elm_framework_helpers-0.3.0/elm_framework_helpers/logging.py
+-rw-r--r--   0        0        0      248 2023-03-23 07:35:43.494903 elm_framework_helpers-0.3.0/elm_framework_helpers/operators/__init__.py
+-rw-r--r--   0        0        0      114 2023-01-27 07:21:57.204998 elm_framework_helpers-0.3.0/elm_framework_helpers/operators/ignore_errors_.py
+-rw-r--r--   0        0        0      243 2023-01-23 09:07:09.378554 elm_framework_helpers-0.3.0/elm_framework_helpers/operators/item_at_index_.py
+-rw-r--r--   0        0        0     1229 2023-03-23 08:02:14.524660 elm_framework_helpers-0.3.0/elm_framework_helpers/operators/manual_value_or.py
+-rw-r--r--   0        0        0     2919 2023-03-12 05:47:22.415439 elm_framework_helpers-0.3.0/elm_framework_helpers/operators/retry_with_delay.py
+-rw-r--r--   0        0        0     2305 2023-02-22 05:45:01.647717 elm_framework_helpers-0.3.0/elm_framework_helpers/output/__init__.py
+-rw-r--r--   0        0        0      396 2023-02-22 05:44:33.006180 elm_framework_helpers-0.3.0/elm_framework_helpers/schedulers/__init__.py
+-rw-r--r--   0        0        0     2365 2023-03-05 07:12:13.951311 elm_framework_helpers-0.3.0/elm_framework_helpers/strategies/binance_tester.py
+-rw-r--r--   0        0        0     1877 2023-01-27 08:37:22.897847 elm_framework_helpers-0.3.0/elm_framework_helpers/strategies/grid/orders.py
+-rw-r--r--   0        0        0      443 2023-03-12 06:18:21.261532 elm_framework_helpers-0.3.0/elm_framework_helpers/testing/__init__.py
+-rw-r--r--   0        0        0     2193 2023-03-12 06:33:19.455778 elm_framework_helpers-0.3.0/elm_framework_helpers/testing/log_to_observable.py
+-rw-r--r--   0        0        0      137 2023-03-12 05:53:54.169432 elm_framework_helpers-0.3.0/elm_framework_helpers/testing/pytest/test_scheduler.py
+-rw-r--r--   0        0        0      656 2023-03-12 06:21:46.729895 elm_framework_helpers-0.3.0/elm_framework_helpers/testing/reactivex_assertion.py
+-rw-r--r--   0        0        0      192 2023-02-25 04:57:35.666325 elm_framework_helpers-0.3.0/elm_framework_helpers/unified/models/book.py
+-rw-r--r--   0        0        0      383 2023-06-22 02:04:38.596995 elm_framework_helpers-0.3.0/elm_framework_helpers/websocket_server/__init__.py
+-rw-r--r--   0        0        0      357 2023-06-22 01:59:34.307678 elm_framework_helpers-0.3.0/elm_framework_helpers/websocket_server/models.py
+-rw-r--r--   0        0        0     2038 2023-06-22 02:01:13.430322 elm_framework_helpers-0.3.0/elm_framework_helpers/websocket_server/server.py
+-rw-r--r--   0        0        0     1086 2023-06-22 02:04:14.976406 elm_framework_helpers-0.3.0/elm_framework_helpers/websocket_server/view.py
+-rw-r--r--   0        0        0     1259 2023-02-25 02:54:19.534869 elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/__init__.py
+-rw-r--r--   0        0        0      473 2023-02-25 02:38:35.310463 elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/bundle.py
+-rw-r--r--   0        0        0     1762 2023-03-05 03:52:38.378403 elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/enhanced_websocket.py
+-rw-r--r--   0        0        0      245 2023-02-25 02:38:35.310463 elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/message_types.py
+-rw-r--r--   0        0        0      782 2023-02-25 02:52:49.680984 elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/status.py
+-rw-r--r--   0        0        0        0 2023-02-25 02:54:45.426117 elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/operators/__init__.py
+-rw-r--r--   0        0        0     2012 2023-02-25 03:01:41.660181 elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/operators/connection_operators.py
+-rw-r--r--   0        0        0     1429 2023-06-22 02:04:45.906995 elm_framework_helpers-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1470 1970-01-01 00:00:00.000000 elm_framework_helpers-0.3.0/PKG-INFO
```

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/ccxt/orderbook/extract.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/ccxt/orderbook/extract.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/http/threaded_server.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/http/threaded_server.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/operators/manual_value_or.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/operators/manual_value_or.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/operators/retry_with_delay.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/operators/retry_with_delay.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/output/__init__.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/output/__init__.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/strategies/binance_tester.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/strategies/binance_tester.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/strategies/grid/orders.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/strategies/grid/orders.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/testing/log_to_observable.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/testing/log_to_observable.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/testing/reactivex_assertion.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/testing/reactivex_assertion.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/__init__.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/__init__.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/enhanced_websocket.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/enhanced_websocket.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/models/status.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/models/status.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/elm_framework_helpers/websockets/operators/connection_operators.py` & `elm_framework_helpers-0.3.0/elm_framework_helpers/websockets/operators/connection_operators.py`

 * *Files identical despite different names*

### Comparing `elm_framework_helpers-0.2.7/pyproject.toml` & `elm_framework_helpers-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elm-framework-helpers"
-version = "0.2.7"
+version = "0.3.0"
 description = ""
 authors = ["Mat <mathieu@redapesolutions.com>"]
 readme = "README.md"
 packages = [{ include = "elm_framework_helpers" }]
 homepage = "https://github.com/TechSpaceAsia/elm-framework-helpers"
 repository = "https://github.com/TechSpaceAsia/elm-framework-helpers"
 license = "MIT"
@@ -46,7 +46,8 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 reactivex = "^4.0.4"
 fastapi = "^0.92.0"
 uvicorn = "^0.20.0"
 orjson = "^3.8.6"
 websocket-client = "^1.5.1"
+websocket-server = "^0.6.4"
```

### Comparing `elm_framework_helpers-0.2.7/PKG-INFO` & `elm_framework_helpers-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elm-framework-helpers
-Version: 0.2.7
+Version: 0.3.0
 Summary: 
 Home-page: https://github.com/TechSpaceAsia/elm-framework-helpers
 License: MIT
 Author: Mat
 Author-email: mathieu@redapesolutions.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,15 @@
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: orjson (>=3.8.6,<4.0.0)
 Requires-Dist: reactivex (>=4.0.4,<5.0.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
 Requires-Dist: websocket-client (>=1.5.1,<2.0.0)
+Requires-Dist: websocket-server (>=0.6.4,<0.7.0)
 Project-URL: Repository, https://github.com/TechSpaceAsia/elm-framework-helpers
 Description-Content-Type: text/markdown
 
 # Helpers for the ELM framework scripts
 
 ## Logging
```

