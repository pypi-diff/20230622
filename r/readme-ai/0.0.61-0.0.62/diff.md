# Comparing `tmp/readme_ai-0.0.61.tar.gz` & `tmp/readme_ai-0.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ai-0.0.61.tar", max compression
+gzip compressed data, was "readme_ai-0.0.62.tar", max compression
```

## Comparing `readme_ai-0.0.61.tar` & `readme_ai-0.0.62.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.61/LICENSE
--rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.61/README.md
--rw-r--r--   0        0        0     2372 2023-06-22 15:07:43.349860 readme_ai-0.0.61/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.61/readme_ai/__init__.py
--rw-r--r--   0        0        0     5949 2023-06-22 14:06:59.973481 readme_ai-0.0.61/readme_ai/builder.py
--rw-r--r--   0        0        0     3858 2023-06-22 10:55:41.792898 readme_ai-0.0.61/readme_ai/conf.py
--rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.61/readme_ai/factory.py
--rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.61/readme_ai/logger.py
--rwxr-xr-x   0        0        0     4621 2023-06-22 15:07:10.056439 readme_ai-0.0.61/readme_ai/main.py
--rw-r--r--   0        0        0     7203 2023-06-22 14:07:31.084456 readme_ai-0.0.61/readme_ai/model.py
--rw-r--r--   0        0        0     7270 2023-06-22 14:07:31.102910 readme_ai-0.0.61/readme_ai/parse.py
--rw-r--r--   0        0        0     6682 2023-06-22 14:07:31.092576 readme_ai-0.0.61/readme_ai/preprocess.py
--rw-r--r--   0        0        0     3785 2023-06-22 14:07:31.064818 readme_ai-0.0.61/readme_ai/utils.py
--rw-r--r--   0        0        0    17716 1970-01-01 00:00:00.000000 readme_ai-0.0.61/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.62/LICENSE
+-rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.62/README.md
+-rw-r--r--   0        0        0     2372 2023-06-22 15:11:19.094754 readme_ai-0.0.62/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.62/readme_ai/__init__.py
+-rw-r--r--   0        0        0     5959 2023-06-22 15:10:09.973478 readme_ai-0.0.62/readme_ai/builder.py
+-rw-r--r--   0        0        0     3859 2023-06-22 15:10:14.257801 readme_ai-0.0.62/readme_ai/conf.py
+-rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.62/readme_ai/factory.py
+-rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.62/readme_ai/logger.py
+-rwxr-xr-x   0        0        0     4621 2023-06-22 15:09:56.999662 readme_ai-0.0.62/readme_ai/main.py
+-rw-r--r--   0        0        0     7218 2023-06-22 15:11:02.062366 readme_ai-0.0.62/readme_ai/model.py
+-rw-r--r--   0        0        0     7271 2023-06-22 15:11:06.893949 readme_ai-0.0.62/readme_ai/parse.py
+-rw-r--r--   0        0        0     6682 2023-06-22 14:07:31.092576 readme_ai-0.0.62/readme_ai/preprocess.py
+-rw-r--r--   0        0        0     3792 2023-06-22 15:10:45.871023 readme_ai-0.0.62/readme_ai/utils.py
+-rw-r--r--   0        0        0    17716 1970-01-01 00:00:00.000000 readme_ai-0.0.62/PKG-INFO
```

### Comparing `readme_ai-0.0.61/LICENSE` & `readme_ai-0.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.61/README.md` & `readme_ai-0.0.62/README.md`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.61/pyproject.toml` & `readme_ai-0.0.62/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readme-ai"
-version = "0.0.61"
+version = "0.0.62"
 description = "🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <43382407+eli64s@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/README-AI"
 documentation = "https://github.com/eli64s/README-AI/blob/main/README.md"
 keywords = [
```

### Comparing `readme_ai-0.0.61/readme_ai/builder.py` & `readme_ai-0.0.62/readme_ai/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import subprocess
 import tempfile
 from pathlib import Path
 
 import pandas as pd
 
-import utils
-from conf import AppConfig, ConfigHelper
-from factory import FileHandler
-from logger import Logger
+from . import utils
+from .conf import AppConfig, ConfigHelper
+from .factory import FileHandler
+from .logger import Logger
 
 LOGGER = Logger(__name__)
 
 
 def build_markdown(
     conf: AppConfig,
     conf_helper: ConfigHelper,
```

### Comparing `readme_ai-0.0.61/readme_ai/conf.py` & `readme_ai-0.0.62/readme_ai/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, List, Union
 from urllib.parse import urlsplit
 
 import dacite
 
-from factory import FileHandler
+from .factory import FileHandler
 
 
 @dataclass
 class ApiConfig:
     """OpenAI API configuration."""
 
     endpoint: str
```

### Comparing `readme_ai-0.0.61/readme_ai/factory.py` & `readme_ai-0.0.62/readme_ai/factory.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.61/readme_ai/logger.py` & `readme_ai-0.0.62/readme_ai/logger.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.61/readme_ai/main.py` & `readme_ai-0.0.62/readme_ai/main.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.61/readme_ai/model.py` & `readme_ai-0.0.62/readme_ai/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from tenacity import (
     retry,
     retry_if_exception_type,
     stop_after_attempt,
     wait_exponential,
 )
 
-import conf
-import utils
-from logger import Logger
+from . import conf
+from . import utils
+from .logger import Logger
 
 
 class OpenAIHandler:
     """OpenAI API handler for generating text for the README.md file."""
 
     LOGGER = Logger(__name__)
```

### Comparing `readme_ai-0.0.61/readme_ai/parse.py` & `readme_ai-0.0.62/readme_ai/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import re
 from typing import List
 
 import toml
 import yaml
 
-from logger import Logger
+from .logger import Logger
 
 LOGGER = Logger(__name__)
 
 
 def parse_docker_compose(content: str) -> List[str]:
     """Extracts services from a docker-compose.yaml file."""
     try:
```

### Comparing `readme_ai-0.0.61/readme_ai/preprocess.py` & `readme_ai-0.0.62/readme_ai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.61/readme_ai/utils.py` & `readme_ai-0.0.62/readme_ai/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import tempfile
 from pathlib import Path
 from typing import List
 
 import git
 from tiktoken import get_encoding
 
-import conf
+from . import conf
 
 
 def is_valid_git_repo(url: str) -> bool:
     """Check if a given URL is a valid git repository."""
     with tempfile.TemporaryDirectory() as temp_dir:
         try:
             git.Repo.clone_from(url, temp_dir, depth=1)
```

### Comparing `readme_ai-0.0.61/PKG-INFO` & `readme_ai-0.0.62/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-ai
-Version: 0.0.61
+Version: 0.0.62
 Summary: 🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/README-AI
 License: MIT
 Keywords: markdown,readme,readme-badges,documentation-generator,markdown-generator,automated-documentation,awesome-readme,readme-generator,python-ai,gpt-3,openai-api,shieldsio-badges,gpt-4,llms,openai-python,chatgpt-python,llmops,openai-chatbot,gpt-35-turbo
 Author: Eli
 Author-email: 43382407+eli64s@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

