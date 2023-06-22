# Comparing `tmp/gpt-engineer-0.0.4.tar.gz` & `tmp/gpt-engineer-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-engineer-0.0.4.tar", last modified: Tue Jun 20 23:17:14 2023, max compression
+gzip compressed data, was "gpt-engineer-0.0.5.tar", last modified: Thu Jun 22 08:47:40 2023, max compression
```

## Comparing `gpt-engineer-0.0.4.tar` & `gpt-engineer-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/gpt_engineer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/gpt_engineer/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/gpt_engineer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 23:17:14.000000 gpt-engineer-0.0.4/gpt_engineer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 23:17:14.941167 gpt-engineer-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/tests/test_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/tests/test_chat_to_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-20 23:17:02.000000 gpt-engineer-0.0.4/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.797059 gpt-engineer-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 08:47:40.797059 gpt-engineer-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.793059 gpt-engineer-0.0.5/gpt_engineer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7901 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/gpt_engineer/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.793059 gpt-engineer-0.0.5/gpt_engineer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 08:47:40.000000 gpt-engineer-0.0.5/gpt_engineer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 08:47:40.797059 gpt-engineer-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:47:40.793059 gpt-engineer-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/tests/test_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/tests/test_chat_to_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-22 08:47:27.000000 gpt-engineer-0.0.5/tests/test_db.py
```

### Comparing `gpt-engineer-0.0.4/LICENSE` & `gpt-engineer-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.4/PKG-INFO` & `gpt-engineer-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,29 +25,19 @@
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-## Usage
-
-Choose either **stable** or **development**.
-
-For **stable** release:
-
-- `pip install gpt-engineer`
-
-For **development**:
+## Setup
 - `git clone git@github.com:AntonOsika/gpt-engineer.git`
 - `cd gpt-engineer`
-- `make install`
-- `source venv/bin/activate`
-
-**Setup**
+- `pip install -e .`
+  - (or: `make install && source venv/bin/activate` for a venv)
 
 With an api key that has GPT4 access run:
 
 - `export OPENAI_API_KEY=[your api key]`
 
 
 **Run**:
```

### Comparing `gpt-engineer-0.0.4/README.md` & `gpt-engineer-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -15,29 +15,19 @@
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-## Usage
-
-Choose either **stable** or **development**.
-
-For **stable** release:
-
-- `pip install gpt-engineer`
-
-For **development**:
+## Setup
 - `git clone git@github.com:AntonOsika/gpt-engineer.git`
 - `cd gpt-engineer`
-- `make install`
-- `source venv/bin/activate`
-
-**Setup**
+- `pip install -e .`
+  - (or: `make install && source venv/bin/activate` for a venv)
 
 With an api key that has GPT4 access run:
 
 - `export OPENAI_API_KEY=[your api key]`
 
 
 **Run**:
```

### Comparing `gpt-engineer-0.0.4/gpt_engineer/ai.py` & `gpt-engineer-0.0.5/gpt_engineer/ai.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.4/gpt_engineer/chat_to_files.py` & `gpt-engineer-0.0.5/gpt_engineer/chat_to_files.py`

 * *Files identical despite different names*

### Comparing `gpt-engineer-0.0.4/gpt_engineer/db.py` & `gpt-engineer-0.0.5/gpt_engineer/db.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     """A simple key-value store, where keys are filenames and values are file contents."""
 
     def __init__(self, path):
         self.path = Path(path).absolute()
 
         self.path.mkdir(parents=True, exist_ok=True)
 
+    def __contains__(self, key):
+        return (self.path / key).is_file()
+
     def __getitem__(self, key):
         full_path = self.path / key
 
         if not full_path.is_file():
             raise KeyError(key)
         with full_path.open("r", encoding="utf-8") as f:
             return f.read()
@@ -31,10 +34,10 @@
 
 
 # dataclass for all dbs:
 @dataclass
 class DBs:
     memory: DB
     logs: DB
-    identity: DB
+    preprompts: DB
     input: DB
     workspace: DB
```

### Comparing `gpt-engineer-0.0.4/gpt_engineer/main.py` & `gpt-engineer-0.0.5/gpt_engineer/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import json
 import logging
-import os
 import shutil
 
 from pathlib import Path
 
 import typer
 
 from gpt_engineer import steps
@@ -50,15 +49,15 @@
     )
 
     dbs = DBs(
         memory=DB(memory_path),
         logs=DB(memory_path / "logs"),
         input=DB(input_path),
         workspace=DB(workspace_path),
-        identity=DB(Path(os.path.curdir) / "identity"),
+        preprompts=DB(Path(__file__).parent / "preprompts"),
     )
 
     for step in STEPS[steps_config]:
         messages = step(ai, dbs)
         dbs.logs[step.__name__] = json.dumps(messages)
```

### Comparing `gpt-engineer-0.0.4/gpt_engineer/steps.py` & `gpt-engineer-0.0.5/gpt_engineer/steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 import json
 import re
 import subprocess
 
 from enum import Enum
+from typing import Callable, TypeVar
 
 from gpt_engineer.ai import AI
 from gpt_engineer.chat_to_files import to_files
 from gpt_engineer.db import DBs
 
 
 def setup_sys_prompt(dbs):
-    return dbs.identity["generate"] + "\nUseful to know:\n" + dbs.identity["philosophy"]
+    return (
+        dbs.preprompts["generate"] + "\nUseful to know:\n" + dbs.preprompts["philosophy"]
+    )
+
+
+Step = TypeVar("Step", bound=Callable[[AI, DBs], list[dict]])
 
 
 def simple_gen(ai: AI, dbs: DBs):
     """Run the AI on the main prompt and save the results"""
     messages = ai.start(
         setup_sys_prompt(dbs),
         dbs.input["main_prompt"],
@@ -23,15 +29,15 @@
     return messages
 
 
 def clarify(ai: AI, dbs: DBs):
     """
     Ask the user if they want to clarify anything and save the results to the workspace
     """
-    messages = [ai.fsystem(dbs.identity["qa"])]
+    messages = [ai.fsystem(dbs.preprompts["qa"])]
     user = dbs.input["main_prompt"]
     while True:
         messages = ai.next(messages, user)
 
         if messages[-1]["content"].strip().lower().startswith("no"):
             break
 
@@ -60,24 +66,24 @@
     the workspace
     """
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
         ai.fsystem(f"Instructions: {dbs.input['main_prompt']}"),
     ]
 
-    messages = ai.next(messages, dbs.identity["spec"])
+    messages = ai.next(messages, dbs.preprompts["spec"])
 
     dbs.memory["specification"] = messages[-1]["content"]
 
     return messages
 
 
 def respec(ai: AI, dbs: DBs):
     messages = json.loads(dbs.logs[gen_spec.__name__])
-    messages += [ai.fsystem(dbs.identity["respec"])]
+    messages += [ai.fsystem(dbs.preprompts["respec"])]
 
     messages = ai.next(messages)
     messages = ai.next(
         messages,
         (
             "Based on the conversation so far, please reiterate the specification for "
             "the program. "
@@ -98,15 +104,15 @@
     """
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
         ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
         ai.fuser(f"Specification:\n\n{dbs.memory['specification']}"),
     ]
 
-    messages = ai.next(messages, dbs.identity["unit_tests"])
+    messages = ai.next(messages, dbs.preprompts["unit_tests"])
 
     dbs.memory["unit_tests"] = messages[-1]["content"]
     to_files(dbs.memory["unit_tests"], dbs.workspace)
 
     return messages
 
 
@@ -114,30 +120,30 @@
     # get the messages from previous step
 
     messages = json.loads(dbs.logs[clarify.__name__])
 
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
     ] + messages[1:]
-    messages = ai.next(messages, dbs.identity["use_qa"])
+    messages = ai.next(messages, dbs.preprompts["use_qa"])
 
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
 def gen_code(ai: AI, dbs: DBs):
     # get the messages from previous step
 
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
         ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
         ai.fuser(f"Specification:\n\n{dbs.memory['specification']}"),
         ai.fuser(f"Unit tests:\n\n{dbs.memory['unit_tests']}"),
     ]
-    messages = ai.next(messages, dbs.identity["use_qa"])
+    messages = ai.next(messages, dbs.preprompts["use_qa"])
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
 def execute_entrypoint(ai, dbs):
     command = dbs.workspace["run.sh"]
 
@@ -187,28 +193,28 @@
 
 
 def use_feedback(ai: AI, dbs: DBs):
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
         ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
         ai.fassistant(dbs.workspace["all_output.txt"]),
-        ai.fsystem(dbs.identity["use_feedback"]),
+        ai.fsystem(dbs.preprompts["use_feedback"]),
     ]
     messages = ai.next(messages, dbs.input["feedback"])
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
 def fix_code(ai: AI, dbs: DBs):
-    code_ouput = json.loads(dbs.logs[gen_code.__name__])[-1]["content"]
+    code_output = json.loads(dbs.logs[gen_code.__name__])[-1]["content"]
     messages = [
         ai.fsystem(setup_sys_prompt(dbs)),
         ai.fuser(f"Instructions: {dbs.input['main_prompt']}"),
-        ai.fuser(code_ouput),
-        ai.fsystem(dbs.identity["fix_code"]),
+        ai.fuser(code_output),
+        ai.fsystem(dbs.preprompts["fix_code"]),
     ]
     messages = ai.next(messages, "Please fix any errors in the code above.")
     to_files(messages[-1]["content"], dbs.workspace)
     return messages
 
 
 class Config(str, Enum):
@@ -255,14 +261,15 @@
         execute_entrypoint,
     ],
     Config.RESPEC: [
         gen_spec,
         respec,
         gen_unit_tests,
         gen_code,
+        fix_code,
         gen_entrypoint,
         execute_entrypoint,
     ],
     Config.USE_FEEDBACK: [use_feedback, gen_entrypoint, execute_entrypoint],
     Config.EXECUTE_ONLY: [gen_entrypoint, execute_entrypoint],
 }
```

### Comparing `gpt-engineer-0.0.4/gpt_engineer.egg-info/PKG-INFO` & `gpt-engineer-0.0.5/gpt_engineer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-engineer
-Version: 0.0.4
+Version: 0.0.5
 Summary: Specify what you want it to build, the AI asks for clarification, and then builds it.
 Project-URL: Homepage, https://github.com/AntonOsika/gpt-engineer
 Project-URL: Bug Tracker, https://github.com/AntonOsika/gpt-engineer/issues
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -25,29 +25,19 @@
 - Flexible and easy to add new own "AI steps". See `steps.py`.
 - Incrementally build towards a user experience of:
   1. high level prompting
   2. giving feedback to the AI that it will remember over time
 - Fast handovers back and forth between AI and human
 - Simplicity, all computation is "resumable" and persisted to the filesystem
 
-## Usage
-
-Choose either **stable** or **development**.
-
-For **stable** release:
-
-- `pip install gpt-engineer`
-
-For **development**:
+## Setup
 - `git clone git@github.com:AntonOsika/gpt-engineer.git`
 - `cd gpt-engineer`
-- `make install`
-- `source venv/bin/activate`
-
-**Setup**
+- `pip install -e .`
+  - (or: `make install && source venv/bin/activate` for a venv)
 
 With an api key that has GPT4 access run:
 
 - `export OPENAI_API_KEY=[your api key]`
 
 
 **Run**:
```

### Comparing `gpt-engineer-0.0.4/pyproject.toml` & `gpt-engineer-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "gpt-engineer"
-version = "0.0.4"
+version = "0.0.5"
 description = "Specify what you want it to build, the AI asks for clarification, and then builds it."
 readme = "README.md"
 requires-python = ">=3"
 dependencies = [
   'black == 23.3.0',
   'mypy == 1.3.0',
   'openai == 0.27.8',
```

### Comparing `gpt-engineer-0.0.4/tests/test_chat_to_files.py` & `gpt-engineer-0.0.5/tests/test_chat_to_files.py`

 * *Files identical despite different names*

