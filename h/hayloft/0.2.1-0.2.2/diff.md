# Comparing `tmp/hayloft-0.2.1.tar.gz` & `tmp/hayloft-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hayloft-0.2.1.tar", max compression
+gzip compressed data, was "hayloft-0.2.2.tar", max compression
```

## Comparing `hayloft-0.2.1.tar` & `hayloft-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.1/LICENSE
--rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.1/hayloft/__init__.py
--rw-r--r--   0        0        0     3365 2023-06-22 12:28:57.584359 hayloft-0.2.1/hayloft/app.py
--rw-r--r--   0        0        0      673 2023-06-22 09:01:21.737742 hayloft-0.2.1/hayloft/cors.py
--rw-r--r--   0        0        0      863 2023-06-20 13:55:34.742760 hayloft-0.2.1/hayloft/llama_index.py
--rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.2.1/hayloft/logger.py
--rw-r--r--   0        0        0   175448 2023-06-22 09:16:49.415090 hayloft-0.2.1/hayloft/public/assets/index-0cc0a4d1.js
--rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.1/hayloft/public/assets/index-7630e259.css
--rw-r--r--   0        0        0      384 2023-06-22 09:16:45.491685 hayloft-0.2.1/hayloft/public/index.html
--rw-r--r--   0        0        0      575 2023-06-22 10:39:00.726417 hayloft-0.2.1/hayloft/schema.py
--rw-r--r--   0        0        0      554 2023-06-21 14:45:37.279127 hayloft-0.2.1/hayloft/sse.py
--rw-r--r--   0        0        0      541 2023-06-22 12:29:39.301564 hayloft-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-13 15:27:24.809402 hayloft-0.2.2/LICENSE
+-rw-r--r--   0        0        0      908 2023-06-18 15:56:02.291486 hayloft-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-13 15:23:56.017734 hayloft-0.2.2/hayloft/__init__.py
+-rw-r--r--   0        0        0     3365 2023-06-22 12:28:57.584359 hayloft-0.2.2/hayloft/app.py
+-rw-r--r--   0        0        0      673 2023-06-22 09:01:21.737742 hayloft-0.2.2/hayloft/cors.py
+-rw-r--r--   0        0        0      860 2023-06-22 12:36:35.898085 hayloft-0.2.2/hayloft/llama_index.py
+-rw-r--r--   0        0        0      669 2023-06-19 12:12:50.488202 hayloft-0.2.2/hayloft/logger.py
+-rw-r--r--   0        0        0   175448 2023-06-22 09:16:49.415090 hayloft-0.2.2/hayloft/public/assets/index-0cc0a4d1.js
+-rw-r--r--   0        0        0    18224 2023-06-22 09:16:49.415090 hayloft-0.2.2/hayloft/public/assets/index-7630e259.css
+-rw-r--r--   0        0        0      384 2023-06-22 09:16:45.491685 hayloft-0.2.2/hayloft/public/index.html
+-rw-r--r--   0        0        0      575 2023-06-22 10:39:00.726417 hayloft-0.2.2/hayloft/schema.py
+-rw-r--r--   0        0        0      554 2023-06-21 14:45:37.279127 hayloft-0.2.2/hayloft/sse.py
+-rw-r--r--   0        0        0      541 2023-06-22 12:37:01.934935 hayloft-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 hayloft-0.2.2/PKG-INFO
```

### Comparing `hayloft-0.2.1/LICENSE` & `hayloft-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/README.md` & `hayloft-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/hayloft/app.py` & `hayloft-0.2.2/hayloft/app.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/hayloft/cors.py` & `hayloft-0.2.2/hayloft/cors.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/hayloft/llama_index.py` & `hayloft-0.2.2/hayloft/llama_index.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,10 +15,10 @@
         elif record.name.startswith("llama_index.llm_predictor"):
             type = "completion"
         elif record.name.startswith("llama_index.indices.response"):
             type = "completion" if record.msg.find(" response: ") != -1 else "prompt"
 
         self.log(title=record.name, message=record.msg, type=type)
 
-def load_hayloft():
+def grab_logs():
     logging.getLogger("llama_index").setLevel(logging.DEBUG)
     logging.getLogger().addHandler(HayloftLogger())
```

### Comparing `hayloft-0.2.1/hayloft/logger.py` & `hayloft-0.2.2/hayloft/logger.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/hayloft/public/assets/index-0cc0a4d1.js` & `hayloft-0.2.2/hayloft/public/assets/index-0cc0a4d1.js`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/hayloft/public/assets/index-7630e259.css` & `hayloft-0.2.2/hayloft/public/assets/index-7630e259.css`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/hayloft/schema.py` & `hayloft-0.2.2/hayloft/schema.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/hayloft/sse.py` & `hayloft-0.2.2/hayloft/sse.py`

 * *Files identical despite different names*

### Comparing `hayloft-0.2.1/pyproject.toml` & `hayloft-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hayloft"
-version = "0.2.1"
+version = "0.2.2"
 description = "UI tool for LLM frameworks"
 authors = []
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eturchenkov/hayloft"
 keywords = ["llm framework", "llm app tracking", "ui for llm app"]
```

### Comparing `hayloft-0.2.1/PKG-INFO` & `hayloft-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hayloft
-Version: 0.2.1
+Version: 0.2.2
 Summary: UI tool for LLM frameworks
 Home-page: https://github.com/eturchenkov/hayloft
 License: MIT
 Keywords: llm framework,llm app tracking,ui for llm app
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

