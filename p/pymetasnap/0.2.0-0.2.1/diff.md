# Comparing `tmp/pymetasnap-0.2.0.tar.gz` & `tmp/pymetasnap-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.2.0.tar", max compression
+gzip compressed data, was "pymetasnap-0.2.1.tar", max compression
```

## Comparing `pymetasnap-0.2.0.tar` & `pymetasnap-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/LICENSE
--rw-r--r--   0        0        0     2927 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/__init__.py
--rw-r--r--   0        0        0     1724 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/checks.py
--rw-r--r--   0        0        0     3278 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/core.py
--rw-r--r--   0        0        0      227 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/logger.py
--rw-r--r--   0        0        0     1287 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/main.py
--rw-r--r--   0        0        0     2550 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/render.py
--rw-r--r--   0        0        0     1926 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/utils.py
--rw-r--r--   0        0        0      845 2023-06-21 23:13:33.784785 pymetasnap-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/__init__.py
+-rw-r--r--   0        0        0     1724 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/checks.py
+-rw-r--r--   0        0        0     3278 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/core.py
+-rw-r--r--   0        0        0      227 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/logger.py
+-rw-r--r--   0        0        0     1287 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/main.py
+-rw-r--r--   0        0        0     2619 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/render.py
+-rw-r--r--   0        0        0     1669 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/utils.py
+-rw-r--r--   0        0        0      845 2023-06-22 14:43:34.900235 pymetasnap-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.2.1/PKG-INFO
```

### Comparing `pymetasnap-0.2.0/LICENSE` & `pymetasnap-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.0/README.md` & `pymetasnap-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.0/extractor/checks.py` & `pymetasnap-0.2.1/extractor/checks.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.0/extractor/core.py` & `pymetasnap-0.2.1/extractor/core.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.0/extractor/main.py` & `pymetasnap-0.2.1/extractor/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typer
 from rich import print
 from typing_extensions import Annotated
 
 from extractor.core import extract_data, save_data
 
 app = typer.Typer()
-VERSION = "0.2.0"
+VERSION = "0.2.1"
 
 
 class RequirementsFormat(str, Enum):
     pip_list = "pip_list"
     pip_freeze = "pip_freeze"
```

### Comparing `pymetasnap-0.2.0/extractor/render.py` & `pymetasnap-0.2.1/extractor/render.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         Args:
             data: The pip freeze formatted data to be parsed.
 
         Returns:
             A list of tuples containing package names and versions.
         """
         lines = data.strip().split("\n")
+        lines = [line for line in lines if not line.startswith("#")]
         pattern = r"(==|<=|>=|<|>)"
         package_data = [re.split(pattern, line) for line in lines]
         return [
             (package[0], package[2]) if len(package) > 1 else package
             for package in package_data
         ]
```

### Comparing `pymetasnap-0.2.0/extractor/utils.py` & `pymetasnap-0.2.1/extractor/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 import pandas as pd
-import toml
 from rich import print
 from rich.progress import track
 
 from extractor.core import filter_data, get_raw_data
 from extractor.logger import logger
 from extractor.render import Requirements
 
 
-def get_version_from_pyproject():
-    with open("pyproject.toml") as f:
-        pyproject_data = toml.load(f)
-        version = (
-            pyproject_data.get("tool", {}).get("poetry", {}).get("version")
-        )  # noqa
-    return version
-
-
 def filter_requirements(requirements_file_data, installed_requirements_data):
     base_reqs = [req[0] for req in requirements_file_data]
     return [
         ireq for ireq in installed_requirements_data if ireq[0] in base_reqs
     ]  # noqa
```

### Comparing `pymetasnap-0.2.0/pyproject.toml` & `pymetasnap-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.2.0"
+version = "0.2.1"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
```

### Comparing `pymetasnap-0.2.0/PKG-INFO` & `pymetasnap-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.2.0
+Version: 0.2.1
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

