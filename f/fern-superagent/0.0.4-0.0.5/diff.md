# Comparing `tmp/fern_superagent-0.0.4.tar.gz` & `tmp/fern_superagent-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fern_superagent-0.0.4.tar", max compression
+gzip compressed data, was "fern_superagent-0.0.5.tar", max compression
```

## Comparing `fern_superagent-0.0.4.tar` & `fern_superagent-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        0 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/README.md
--rw-r--r--   0        0        0      380 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      517 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/__init__.py
--rw-r--r--   0        0        0     2378 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/py.typed
--rw-r--r--   0        0        0      236 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14819 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5901 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    10039 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0     9019 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-06-22 14:23:35.390052 fern_superagent-0.0.4/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 fern_superagent-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2274 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/README.md
+-rw-r--r--   0        0        0      380 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      517 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/__init__.py
+-rw-r--r--   0        0        0     2378 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-22 14:31:34.537184 fern_superagent-0.0.5/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/py.typed
+-rw-r--r--   0        0        0      236 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14819 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    10039 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0     9019 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-06-22 14:31:34.541183 fern_superagent-0.0.5/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     2715 1970-01-01 00:00:00.000000 fern_superagent-0.0.5/PKG-INFO
```

### Comparing `fern_superagent-0.0.4/src/superagent/__init__.py` & `fern_superagent-0.0.5/src/superagent/__init__.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/client.py` & `fern_superagent-0.0.5/src/superagent/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/core/datetime_utils.py` & `fern_superagent-0.0.5/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/core/jsonable_encoder.py` & `fern_superagent-0.0.5/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/agent/client.py` & `fern_superagent-0.0.5/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/api_token/client.py` & `fern_superagent-0.0.5/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/auth/client.py` & `fern_superagent-0.0.5/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/documents/client.py` & `fern_superagent-0.0.5/src/superagent/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/prompts/client.py` & `fern_superagent-0.0.5/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/tools/client.py` & `fern_superagent-0.0.5/src/superagent/resources/tools/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/traces/client.py` & `fern_superagent-0.0.5/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/resources/user/client.py` & `fern_superagent-0.0.5/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/types/http_validation_error.py` & `fern_superagent-0.0.5/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `fern_superagent-0.0.4/src/superagent/types/validation_error.py` & `fern_superagent-0.0.5/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

