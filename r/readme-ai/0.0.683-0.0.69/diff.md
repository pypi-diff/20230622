# Comparing `tmp/readme_ai-0.0.683.tar.gz` & `tmp/readme_ai-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ai-0.0.683.tar", max compression
+gzip compressed data, was "readme_ai-0.0.69.tar", max compression
```

## Comparing `readme_ai-0.0.683.tar` & `readme_ai-0.0.69.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.683/LICENSE
--rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.683/README.md
--rw-r--r--   0        0        0     2457 2023-06-22 16:34:44.446009 readme_ai-0.0.683/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.683/readme_ai/__init__.py
--rw-r--r--   0        0        0     5959 2023-06-22 15:10:09.973478 readme_ai-0.0.683/readme_ai/builder.py
--rw-r--r--   0        0        0     3861 2023-06-22 16:15:35.759720 readme_ai-0.0.683/readme_ai/conf.py
--rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.683/readme_ai/factory.py
--rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.683/readme_ai/logger.py
--rwxr-xr-x   0        0        0     4621 2023-06-22 15:09:56.999662 readme_ai-0.0.683/readme_ai/main.py
--rw-r--r--   0        0        0     7218 2023-06-22 15:11:02.062366 readme_ai-0.0.683/readme_ai/model.py
--rw-r--r--   0        0        0     7271 2023-06-22 15:11:06.893949 readme_ai-0.0.683/readme_ai/parse.py
--rw-r--r--   0        0        0     6703 2023-06-22 15:12:37.102550 readme_ai-0.0.683/readme_ai/preprocess.py
--rw-r--r--   0        0        0     3792 2023-06-22 15:10:45.871023 readme_ai-0.0.683/readme_ai/utils.py
--rw-r--r--   0        0        0    17717 1970-01-01 00:00:00.000000 readme_ai-0.0.683/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.69/LICENSE
+-rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.69/README.md
+-rw-r--r--   0        0        0     2456 2023-06-22 16:45:41.280960 readme_ai-0.0.69/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.69/readme_ai/__init__.py
+-rw-r--r--   0        0        0     5959 2023-06-22 15:10:09.973478 readme_ai-0.0.69/readme_ai/builder.py
+-rw-r--r--   0        0        0     3861 2023-06-22 16:15:35.759720 readme_ai-0.0.69/readme_ai/conf.py
+-rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.69/readme_ai/factory.py
+-rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.69/readme_ai/logger.py
+-rwxr-xr-x   0        0        0     4621 2023-06-22 15:09:56.999662 readme_ai-0.0.69/readme_ai/main.py
+-rw-r--r--   0        0        0     7218 2023-06-22 15:11:02.062366 readme_ai-0.0.69/readme_ai/model.py
+-rw-r--r--   0        0        0     7271 2023-06-22 15:11:06.893949 readme_ai-0.0.69/readme_ai/parse.py
+-rw-r--r--   0        0        0     6703 2023-06-22 15:12:37.102550 readme_ai-0.0.69/readme_ai/preprocess.py
+-rw-r--r--   0        0        0     3792 2023-06-22 15:10:45.871023 readme_ai-0.0.69/readme_ai/utils.py
+-rw-r--r--   0        0        0    17716 1970-01-01 00:00:00.000000 readme_ai-0.0.69/PKG-INFO
```

### Comparing `readme_ai-0.0.683/LICENSE` & `readme_ai-0.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/README.md` & `readme_ai-0.0.69/README.md`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/pyproject.toml` & `readme_ai-0.0.69/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 readme-ai = "readme_ai.main:main"
 
 [build-system.sdist]
 include = ["pyproject.toml"]
 
 [tool.poetry]
 name = "readme-ai"
-version = "0.0.683"
+version = "0.0.69"
 description = "🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <43382407+eli64s@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/README-AI"
 documentation = "https://github.com/eli64s/README-AI/blob/main/README.md"
 keywords = [
```

### Comparing `readme_ai-0.0.683/readme_ai/builder.py` & `readme_ai-0.0.69/readme_ai/builder.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/conf.py` & `readme_ai-0.0.69/readme_ai/conf.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/factory.py` & `readme_ai-0.0.69/readme_ai/factory.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/logger.py` & `readme_ai-0.0.69/readme_ai/logger.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/main.py` & `readme_ai-0.0.69/readme_ai/main.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/model.py` & `readme_ai-0.0.69/readme_ai/model.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/parse.py` & `readme_ai-0.0.69/readme_ai/parse.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/preprocess.py` & `readme_ai-0.0.69/readme_ai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/readme_ai/utils.py` & `readme_ai-0.0.69/readme_ai/utils.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.683/PKG-INFO` & `readme_ai-0.0.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-ai
-Version: 0.0.683
+Version: 0.0.69
 Summary: 🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/README-AI
 License: MIT
 Keywords: markdown,readme,readme-badges,documentation-generator,markdown-generator,automated-documentation,awesome-readme,readme-generator,python-ai,gpt-3,openai-api,shieldsio-badges,gpt-4,llms,openai-python,chatgpt-python,llmops,openai-chatbot,gpt-35-turbo
 Author: Eli
 Author-email: 43382407+eli64s@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

