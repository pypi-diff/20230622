# Comparing `tmp/gpt-engineer-0.0.5.tar.gz` & `tmp/gpt-engineer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-engineer-0.0.5.tar", last modified: Thu Jun 22 08:47:40 2023, max compression
+gzip compressed data, was "gpt-engineer-0.0.6.tar", last modified: Thu Jun 22 09:31:36 2023, max compression
```

## Comparing `gpt-engineer-0.0.5.tar` & `gpt-engineer-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.797059 gpt-engineer-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 08:47:40.797059 gpt-engineer-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.793059 gpt-engineer-0.0.5/gpt_engineer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.793059 gpt-engineer-0.0.5/gpt_engineer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:47:40.797059 gpt-engineer-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.793059 gpt-engineer-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/tests/test_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/tests/test_chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.446110 gpt-engineer-0.0.6/gpt_engineer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/gpt_engineer/preprompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/fix_code
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/generate
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/philosophy
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/qa
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/respec
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/spec
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/unit_tests
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/use_feedback
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/preprompts/use_qa
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/gpt_engineer/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/gpt_engineer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 09:31:36.000000 gpt-engineer-0.0.6/gpt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:31:36.450110 gpt-engineer-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/tests/test_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/tests/test_chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 09:31:25.000000 gpt-engineer-0.0.6/tests/test_db.py
```

### Comparing `gpt-engineer-0.0.5/LICENSE` & `gpt-engineer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.5/PKG-INFO` & `gpt-engineer-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gpt-engineer-0.0.5/README.md` & `gpt-engineer-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.5/gpt_engineer/ai.py` & `gpt-engineer-0.0.6/gpt_engineer/ai.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.5/gpt_engineer/chat_to_files.py` & `gpt-engineer-0.0.6/gpt_engineer/chat_to_files.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.5/gpt_engineer/db.py` & `gpt-engineer-0.0.6/gpt_engineer/db.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.5/gpt_engineer/main.py` & `gpt-engineer-0.0.6/gpt_engineer/main.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.5/gpt_engineer/steps.py` & `gpt-engineer-0.0.6/gpt_engineer/steps.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.5/gpt_engineer.egg-info/PKG-INFO` & `gpt-engineer-0.0.6/gpt_engineer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.5
+Version: 0.0.6
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `gpt-engineer-0.0.5/pyproject.toml` & `gpt-engineer-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "gpt-engineer"
-version = "0.0.5"
+version = "0.0.6"
 description = "Specify what you want it to build, the AI asks for clarification, and then builds it."
 readme = "README.md"
 requires-python = ">=3"
 dependencies = [
   'black == 23.3.0',
   'mypy == 1.3.0',
   'openai == 0.27.8',
```

### Comparing `gpt-engineer-0.0.5/tests/test_chat_to_files.py` & `gpt-engineer-0.0.6/tests/test_chat_to_files.py`

 * *Files identical despite different names*

