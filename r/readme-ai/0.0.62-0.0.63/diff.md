# Comparing `tmp/readme_ai-0.0.62.tar.gz` & `tmp/readme_ai-0.0.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ai-0.0.62.tar", max compression
+gzip compressed data, was "readme_ai-0.0.63.tar", max compression
```

## Comparing `readme_ai-0.0.62.tar` & `readme_ai-0.0.63.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.62/LICENSE
--rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.62/README.md
--rw-r--r--   0        0        0     2372 2023-06-22 15:11:19.094754 readme_ai-0.0.62/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.62/readme_ai/__init__.py
--rw-r--r--   0        0        0     5959 2023-06-22 15:10:09.973478 readme_ai-0.0.62/readme_ai/builder.py
--rw-r--r--   0        0        0     3859 2023-06-22 15:10:14.257801 readme_ai-0.0.62/readme_ai/conf.py
--rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.62/readme_ai/factory.py
--rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.62/readme_ai/logger.py
--rwxr-xr-x   0        0        0     4621 2023-06-22 15:09:56.999662 readme_ai-0.0.62/readme_ai/main.py
--rw-r--r--   0        0        0     7218 2023-06-22 15:11:02.062366 readme_ai-0.0.62/readme_ai/model.py
--rw-r--r--   0        0        0     7271 2023-06-22 15:11:06.893949 readme_ai-0.0.62/readme_ai/parse.py
--rw-r--r--   0        0        0     6682 2023-06-22 14:07:31.092576 readme_ai-0.0.62/readme_ai/preprocess.py
--rw-r--r--   0        0        0     3792 2023-06-22 15:10:45.871023 readme_ai-0.0.62/readme_ai/utils.py
--rw-r--r--   0        0        0    17716 1970-01-01 00:00:00.000000 readme_ai-0.0.62/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.63/LICENSE
+-rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.63/README.md
+-rw-r--r--   0        0        0     2372 2023-06-22 15:12:56.977605 readme_ai-0.0.63/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.63/readme_ai/__init__.py
+-rw-r--r--   0        0        0     5959 2023-06-22 15:10:09.973478 readme_ai-0.0.63/readme_ai/builder.py
+-rw-r--r--   0        0        0     3859 2023-06-22 15:10:14.257801 readme_ai-0.0.63/readme_ai/conf.py
+-rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.63/readme_ai/factory.py
+-rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.63/readme_ai/logger.py
+-rwxr-xr-x   0        0        0     4621 2023-06-22 15:09:56.999662 readme_ai-0.0.63/readme_ai/main.py
+-rw-r--r--   0        0        0     7218 2023-06-22 15:11:02.062366 readme_ai-0.0.63/readme_ai/model.py
+-rw-r--r--   0        0        0     7271 2023-06-22 15:11:06.893949 readme_ai-0.0.63/readme_ai/parse.py
+-rw-r--r--   0        0        0     6703 2023-06-22 15:12:37.102550 readme_ai-0.0.63/readme_ai/preprocess.py
+-rw-r--r--   0        0        0     3792 2023-06-22 15:10:45.871023 readme_ai-0.0.63/readme_ai/utils.py
+-rw-r--r--   0        0        0    17716 1970-01-01 00:00:00.000000 readme_ai-0.0.63/PKG-INFO
```

### Comparing `readme_ai-0.0.62/LICENSE` & `readme_ai-0.0.63/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/README.md` & `readme_ai-0.0.63/README.md`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/pyproject.toml` & `readme_ai-0.0.63/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readme-ai"
-version = "0.0.62"
+version = "0.0.63"
 description = "🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <43382407+eli64s@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/README-AI"
 documentation = "https://github.com/eli64s/README-AI/blob/main/README.md"
 keywords = [
```

### Comparing `readme_ai-0.0.62/readme_ai/builder.py` & `readme_ai-0.0.63/readme_ai/builder.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/readme_ai/conf.py` & `readme_ai-0.0.63/readme_ai/conf.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/readme_ai/factory.py` & `readme_ai-0.0.63/readme_ai/factory.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/readme_ai/logger.py` & `readme_ai-0.0.63/readme_ai/logger.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/readme_ai/main.py` & `readme_ai-0.0.63/readme_ai/main.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/readme_ai/model.py` & `readme_ai-0.0.63/readme_ai/model.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/readme_ai/parse.py` & `readme_ai-0.0.63/readme_ai/parse.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/readme_ai/preprocess.py` & `readme_ai-0.0.63/readme_ai/preprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import tempfile
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
 import tiktoken
 
-import conf
-import parse
-import utils
+from . import conf
+from . import parse
+from . import utils
 
 
 class RepositoryParserWrapper:
     """Wrapper class for the RepositoryParser."""
 
     def __init__(self, conf: conf.AppConfig, conf_helper: conf.ConfigHelper):
         self.parser = RepositoryParser(
```

### Comparing `readme_ai-0.0.62/readme_ai/utils.py` & `readme_ai-0.0.63/readme_ai/utils.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.62/PKG-INFO` & `readme_ai-0.0.63/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-ai
-Version: 0.0.62
+Version: 0.0.63
 Summary: 🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/README-AI
 License: MIT
 Keywords: markdown,readme,readme-badges,documentation-generator,markdown-generator,automated-documentation,awesome-readme,readme-generator,python-ai,gpt-3,openai-api,shieldsio-badges,gpt-4,llms,openai-python,chatgpt-python,llmops,openai-chatbot,gpt-35-turbo
 Author: Eli
 Author-email: 43382407+eli64s@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

