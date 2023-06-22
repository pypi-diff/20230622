# Comparing `tmp/readme_ai-0.0.65.tar.gz` & `tmp/readme_ai-0.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readme_ai-0.0.65.tar", max compression
+gzip compressed data, was "readme_ai-0.0.66.tar", max compression
```

## Comparing `readme_ai-0.0.65.tar` & `readme_ai-0.0.66.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.65/LICENSE
--rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.65/README.md
--rw-r--r--   0        0        0     2502 2023-06-22 15:25:00.667586 readme_ai-0.0.65/pyproject.toml
--rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.65/readme_ai/__init__.py
--rw-r--r--   0        0        0     5959 2023-06-22 15:10:09.973478 readme_ai-0.0.65/readme_ai/builder.py
--rw-r--r--   0        0        0     3912 2023-06-22 15:16:48.563642 readme_ai-0.0.65/readme_ai/conf.py
--rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.65/readme_ai/factory.py
--rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.65/readme_ai/logger.py
--rwxr-xr-x   0        0        0     4621 2023-06-22 15:09:56.999662 readme_ai-0.0.65/readme_ai/main.py
--rw-r--r--   0        0        0     7218 2023-06-22 15:11:02.062366 readme_ai-0.0.65/readme_ai/model.py
--rw-r--r--   0        0        0     7271 2023-06-22 15:11:06.893949 readme_ai-0.0.65/readme_ai/parse.py
--rw-r--r--   0        0        0     6703 2023-06-22 15:12:37.102550 readme_ai-0.0.65/readme_ai/preprocess.py
--rw-r--r--   0        0        0     3792 2023-06-22 15:10:45.871023 readme_ai-0.0.65/readme_ai/utils.py
--rw-r--r--   0        0        0    17716 1970-01-01 00:00:00.000000 readme_ai-0.0.65/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-02-24 21:00:05.269166 readme_ai-0.0.66/LICENSE
+-rw-r--r--   0        0        0    15959 2023-06-22 14:05:56.067804 readme_ai-0.0.66/README.md
+-rw-r--r--   0        0        0     6368 2023-06-21 20:44:11.043106 readme_ai-0.0.66/conf/conf.toml
+-rw-r--r--   0        0        0     1532 2023-05-28 14:39:03.433409 readme_ai-0.0.66/conf/dependency_files.toml
+-rw-r--r--   0        0        0     2178 2023-06-21 21:45:42.823961 readme_ai-0.0.66/conf/ignore_files.toml
+-rw-r--r--   0        0        0     1128 2023-06-21 00:53:09.500846 readme_ai-0.0.66/conf/language_names.toml
+-rw-r--r--   0        0        0     2854 2023-06-21 00:47:29.564628 readme_ai-0.0.66/conf/language_setup.toml
+-rw-r--r--   0        0        0  4519801 2023-06-01 07:23:32.901951 readme_ai-0.0.66/conf/svg/badges.json
+-rw-r--r--   0        0        0   337217 2023-06-21 20:04:14.971983 readme_ai-0.0.66/conf/svg/badges_compressed.json
+-rw-r--r--   0        0        0     2449 2023-06-22 15:27:24.309085 readme_ai-0.0.66/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-01-24 09:34:25.754949 readme_ai-0.0.66/readme_ai/__init__.py
+-rw-r--r--   0        0        0     5959 2023-06-22 15:10:09.973478 readme_ai-0.0.66/readme_ai/builder.py
+-rw-r--r--   0        0        0     3912 2023-06-22 15:16:48.563642 readme_ai-0.0.66/readme_ai/conf.py
+-rw-r--r--   0        0        0     3927 2023-06-20 00:23:27.565634 readme_ai-0.0.66/readme_ai/factory.py
+-rw-r--r--   0        0        0     1722 2023-06-18 00:28:07.197967 readme_ai-0.0.66/readme_ai/logger.py
+-rwxr-xr-x   0        0        0     4621 2023-06-22 15:09:56.999662 readme_ai-0.0.66/readme_ai/main.py
+-rw-r--r--   0        0        0     7218 2023-06-22 15:11:02.062366 readme_ai-0.0.66/readme_ai/model.py
+-rw-r--r--   0        0        0     7271 2023-06-22 15:11:06.893949 readme_ai-0.0.66/readme_ai/parse.py
+-rw-r--r--   0        0        0     6703 2023-06-22 15:12:37.102550 readme_ai-0.0.66/readme_ai/preprocess.py
+-rw-r--r--   0        0        0     3792 2023-06-22 15:10:45.871023 readme_ai-0.0.66/readme_ai/utils.py
+-rw-r--r--   0        0        0    17716 1970-01-01 00:00:00.000000 readme_ai-0.0.66/PKG-INFO
```

### Comparing `readme_ai-0.0.65/LICENSE` & `readme_ai-0.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/README.md` & `readme_ai-0.0.66/README.md`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/pyproject.toml` & `readme_ai-0.0.66/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
 readme-ai = "readme_ai.main:main"
 
 [tool.poetry]
 name = "readme-ai"
-version = "0.0.65"
+include = ["conf/*.toml", "conf/svg/*.json"]
+version = "0.0.66"
 description = "🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫"
 authors = ["Eli <43382407+eli64s@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/eli64s/README-AI"
 documentation = "https://github.com/eli64s/README-AI/blob/main/README.md"
 keywords = [
@@ -55,15 +56,14 @@
     "llms",
     "openai-python",
     "chatgpt-python",
     "llmops",
     "openai-chatbot",
     "gpt-35-turbo",
 ]
-include = ["readme_ai/*", "readme_ai.conf/*", "readme_ai.conf.svg", "readme_ai.conf.templates/*"]
 
 # Autoflake
 [tool.autoflake]
 ignore_pass_statements = true
 ignore-pass-after-docstring = true
 remove_all_unused_imports = true
 recursive = true
```

### Comparing `readme_ai-0.0.65/readme_ai/builder.py` & `readme_ai-0.0.66/readme_ai/builder.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/conf.py` & `readme_ai-0.0.66/readme_ai/conf.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/factory.py` & `readme_ai-0.0.66/readme_ai/factory.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/logger.py` & `readme_ai-0.0.66/readme_ai/logger.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/main.py` & `readme_ai-0.0.66/readme_ai/main.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/model.py` & `readme_ai-0.0.66/readme_ai/model.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/parse.py` & `readme_ai-0.0.66/readme_ai/parse.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/preprocess.py` & `readme_ai-0.0.66/readme_ai/preprocess.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/readme_ai/utils.py` & `readme_ai-0.0.66/readme_ai/utils.py`

 * *Files identical despite different names*

### Comparing `readme_ai-0.0.65/PKG-INFO` & `readme_ai-0.0.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readme-ai
-Version: 0.0.65
+Version: 0.0.66
 Summary: 🚀 Generate awesome README files from the terminal, powered by OpenAI's GPT language model APIs 💫
 Home-page: https://github.com/eli64s/README-AI
 License: MIT
 Keywords: markdown,readme,readme-badges,documentation-generator,markdown-generator,automated-documentation,awesome-readme,readme-generator,python-ai,gpt-3,openai-api,shieldsio-badges,gpt-4,llms,openai-python,chatgpt-python,llmops,openai-chatbot,gpt-35-turbo
 Author: Eli
 Author-email: 43382407+eli64s@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
```

