# Comparing `tmp/hayloft-0.2.0a1.tar.gz` & `tmp/hayloft-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.2.0a1.tar", max compression
+gzip compressed data, was "hayloft-0.2.0a2.tar", max compression
```

## Comparing `hayloft-0.2.0a1.tar` & `hayloft-0.2.0a2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.0a1/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.0a1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.0a1/hayloft/__init__.py
--rw-r--r--   0        0        0     3268 2023-06-22 09:38:40.225479 hayloft-0.2.0a1/hayloft/app-old.py
--rw-r--r--   0        0        0     3410 2023-06-22 09:49:41.116144 hayloft-0.2.0a1/hayloft/app.py
--rw-r--r--   0        0        0      673 2023-06-22 09:01:21.737742 hayloft-0.2.0a1/hayloft/cors.py
--rw-r--r--   0        0        0      863 2023-06-20 13:55:34.742760 hayloft-0.2.0a1/hayloft/llama_index.py
--rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.2.0a1/hayloft/logger.py
--rw-r--r--   0        0        0   175448 2023-06-22 09:16:49.415090 hayloft-0.2.0a1/hayloft/public/assets/index-0cc0a4d1.js
--rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.0a1/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0      384 2023-06-22 09:16:45.491685 hayloft-0.2.0a1/hayloft/public/index.html
--rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.2.0a1/hayloft/schema-old.py
--rw-r--r--   0        0        0      575 2023-06-22 10:12:56.000756 hayloft-0.2.0a1/hayloft/schema.py
--rw-r--r--   0        0        0      554 2023-06-21 14:45:37.279127 hayloft-0.2.0a1/hayloft/sse.py
--rw-r--r--   0        0        0      543 2023-06-22 10:13:52.057719 hayloft-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 hayloft-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.0a2/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.0a2/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.0a2/hayloft/__init__.py
+-rw-r--r--   0        0        0     3268 2023-06-22 09:38:40.225479 hayloft-0.2.0a2/hayloft/app-old.py
+-rw-r--r--   0        0        0     3410 2023-06-22 09:49:41.116144 hayloft-0.2.0a2/hayloft/app.py
+-rw-r--r--   0        0        0      673 2023-06-22 09:01:21.737742 hayloft-0.2.0a2/hayloft/cors.py
+-rw-r--r--   0        0        0      863 2023-06-20 13:55:34.742760 hayloft-0.2.0a2/hayloft/llama_index.py
+-rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.2.0a2/hayloft/logger.py
+-rw-r--r--   0        0        0   175448 2023-06-22 09:16:49.415090 hayloft-0.2.0a2/hayloft/public/assets/index-0cc0a4d1.js
+-rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.0a2/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0      384 2023-06-22 09:16:45.491685 hayloft-0.2.0a2/hayloft/public/index.html
+-rw-r--r--   0        0        0     1367 2023-06-13 15:26:48.605765 hayloft-0.2.0a2/hayloft/schema-old.py
+-rw-r--r--   0        0        0      816 2023-06-22 10:34:29.676305 hayloft-0.2.0a2/hayloft/schema.py
+-rw-r--r--   0        0        0      554 2023-06-21 14:45:37.279127 hayloft-0.2.0a2/hayloft/sse.py
+-rw-r--r--   0        0        0      543 2023-06-22 10:35:00.229129 hayloft-0.2.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 hayloft-0.2.0a2/PKG-INFO
```

### Comparing `hayloft-0.2.0a1/LICENSE` & `hayloft-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/README.md` & `hayloft-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/app-old.py` & `hayloft-0.2.0a2/hayloft/app-old.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/app.py` & `hayloft-0.2.0a2/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/cors.py` & `hayloft-0.2.0a2/hayloft/cors.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/llama_index.py` & `hayloft-0.2.0a2/hayloft/llama_index.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/logger.py` & `hayloft-0.2.0a2/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/public/assets/index-0cc0a4d1.js` & `hayloft-0.2.0a2/hayloft/public/assets/index-0cc0a4d1.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/public/assets/index-7630e259.css` & `hayloft-0.2.0a2/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/schema-old.py` & `hayloft-0.2.0a2/hayloft/schema-old.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/hayloft/sse.py` & `hayloft-0.2.0a2/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.0a1/pyproject.toml` & `hayloft-0.2.0a2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.2.0a1"
+version = "0.2.0a2"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.2.0a1/PKG-INFO` & `hayloft-0.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.2.0a1
+Version: 0.2.0a2
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

