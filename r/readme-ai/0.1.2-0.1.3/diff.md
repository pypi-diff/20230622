# Comparing `tmp/readme_ai-0.1.2.tar.gz` & `tmp/readme_ai-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ai-0.1.2.tar", max compression
+gzip compressed data, was "readme_ai-0.1.3.tar", max compression
```

## Comparing `readme_ai-0.1.2.tar` & `readme_ai-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.1.2/LICENSE
--rw-r--r--   0        0        0    15980 2023-06-22 12:25:52.523548 readme_ai-0.1.2/README.md
--rw-r--r--   0        0        0     2491 2023-06-22 12:59:04.459018 readme_ai-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.1.2/src/readme_ai/__init__.py
--rw-r--r--   0        0        0     5949 2023-06-22 12:52:04.858638 readme_ai-0.1.2/src/readme_ai/builder.py
--rw-r--r--   0        0        0     3858 2023-06-22 10:55:41.792898 readme_ai-0.1.2/src/readme_ai/conf.py
--rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.1.2/src/readme_ai/factory.py
--rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.1.2/src/readme_ai/logger.py
--rwxr-xr-x   0        0        0     4606 2023-06-22 12:57:00.708512 readme_ai-0.1.2/src/readme_ai/main.py
--rw-r--r--   0        0        0     7392 2023-06-22 12:21:52.188140 readme_ai-0.1.2/src/readme_ai/model.py
--rw-r--r--   0        0        0     7258 2023-06-22 12:21:52.279983 readme_ai-0.1.2/src/readme_ai/parse.py
--rw-r--r--   0        0        0     6620 2023-06-22 12:21:52.087982 readme_ai-0.1.2/src/readme_ai/preprocess.py
--rw-r--r--   0        0        0     3769 2023-06-22 12:21:52.244679 readme_ai-0.1.2/src/readme_ai/utils.py
--rw-r--r--   0        0        0    17736 1970-01-01 00:00:00.000000 readme_ai-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.1.3/LICENSE
+-rw-r--r--   0        0        0    15980 2023-06-22 12:25:52.523548 readme_ai-0.1.3/README.md
+-rw-r--r--   0        0        0     2483 2023-06-22 13:03:36.810357 readme_ai-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.1.3/src/readme_ai/__init__.py
+-rw-r--r--   0        0        0     5949 2023-06-22 12:52:04.858638 readme_ai-0.1.3/src/readme_ai/builder.py
+-rw-r--r--   0        0        0     3858 2023-06-22 10:55:41.792898 readme_ai-0.1.3/src/readme_ai/conf.py
+-rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.1.3/src/readme_ai/factory.py
+-rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.1.3/src/readme_ai/logger.py
+-rwxr-xr-x   0        0        0     4606 2023-06-22 12:57:00.708512 readme_ai-0.1.3/src/readme_ai/main.py
+-rw-r--r--   0        0        0     7392 2023-06-22 12:21:52.188140 readme_ai-0.1.3/src/readme_ai/model.py
+-rw-r--r--   0        0        0     7258 2023-06-22 12:21:52.279983 readme_ai-0.1.3/src/readme_ai/parse.py
+-rw-r--r--   0        0        0     6620 2023-06-22 12:21:52.087982 readme_ai-0.1.3/src/readme_ai/preprocess.py
+-rw-r--r--   0        0        0     3769 2023-06-22 12:21:52.244679 readme_ai-0.1.3/src/readme_ai/utils.py
+-rw-r--r--   0        0        0    17736 1970-01-01 00:00:00.000000 readme_ai-0.1.3/PKG-INFO
```

### Comparing `readme_ai-0.1.2/LICENSE` & `readme_ai-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/README.md` & `readme_ai-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/pyproject.toml` & `readme_ai-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readme-ai"
-version = "0.1.2"
+version = "0.1.3"
 description = "🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <43382407+eli64s@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/README-AI"
 documentation = "https://github.com/eli64s/README-AI/blob/main/README.md"
 keywords = [
@@ -25,18 +25,14 @@
     "openai-python",
     "chatgpt-python",
     "llmops",
     "openai-chatbot",
     "gpt-35-turbo",
 ]
 
-[build-system.packages]
-readme_ai = {include = "src/readme_ai"}
-readme_ai_subpackages = {include = "src/readme_ai/**"}
-
 [tool.poetry.dependencies]
 python = "^3.8"
 pandas = "^1.4.0"
 black = "21.9b0"
 click = "8.0.1"
 colorlog = "^6.7.0"
 cachetools = "^5.3.1"
@@ -51,21 +47,25 @@
 responses = "^0.23.1"
 setuptools = "^68.0.0"
 tabulate = "^0.9.0"
 tenacity = "^8.2.2"
 tiktoken = "^0.4.0"
 openai = "^0.27.8"
 
-[tool.poetry.scripts]
-readme-ai = "readme_ai.main:main"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
+[build-system.scripts]
+readme-ai = "readme_ai.main:main"
+
+[build-system.packages]
+readme_ai = {include = "readme_ai"}
+readme_ai_subpackages = {include = "readme_ai.*"}
+
 # Autoflake
 [tool.autoflake]
 ignore_pass_statements = true
 ignore-pass-after-docstring = true
 remove_all_unused_imports = true
 recursive = true
```

### Comparing `readme_ai-0.1.2/src/readme_ai/builder.py` & `readme_ai-0.1.3/src/readme_ai/builder.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/conf.py` & `readme_ai-0.1.3/src/readme_ai/conf.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/factory.py` & `readme_ai-0.1.3/src/readme_ai/factory.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/logger.py` & `readme_ai-0.1.3/src/readme_ai/logger.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/main.py` & `readme_ai-0.1.3/src/readme_ai/main.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/model.py` & `readme_ai-0.1.3/src/readme_ai/model.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/parse.py` & `readme_ai-0.1.3/src/readme_ai/parse.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/preprocess.py` & `readme_ai-0.1.3/src/readme_ai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/src/readme_ai/utils.py` & `readme_ai-0.1.3/src/readme_ai/utils.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.1.2/PKG-INFO` & `readme_ai-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-ai
-Version: 0.1.2
+Version: 0.1.3
 Summary: 🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/README-AI
 License: MIT
 Keywords: markdown,readme,readme-badges,documentation-generator,markdown-generator,automated-documentation,awesome-readme,readme-generator,python-ai,gpt-3,openai-api,shieldsio-badges,gpt-4,llms,openai-python,chatgpt-python,llmops,openai-chatbot,gpt-35-turbo
 Author: Eli
 Author-email: 43382407+eli64s@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

