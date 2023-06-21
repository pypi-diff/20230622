# Comparing `tmp/pymetasnap-0.1.4.tar.gz` & `tmp/pymetasnap-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.1.4.tar", max compression
+gzip compressed data, was "pymetasnap-0.2.0.tar", max compression
```

## Comparing `pymetasnap-0.1.4.tar` & `pymetasnap-0.2.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/LICENSE
--rw-r--r--   0        0        0     2927 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/__init__.py
--rw-r--r--   0        0        0      684 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/checks.py
--rw-r--r--   0        0        0     3118 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/core.py
--rw-r--r--   0        0        0     1276 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/main.py
--rw-r--r--   0        0        0     2550 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/render.py
--rw-r--r--   0        0        0     1916 2023-06-21 19:37:29.977801 pymetasnap-0.1.4/extractor/utils.py
--rw-r--r--   0        0        0      845 2023-06-21 19:37:29.981801 pymetasnap-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/__init__.py
+-rw-r--r--   0        0        0     1724 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/checks.py
+-rw-r--r--   0        0        0     3278 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/core.py
+-rw-r--r--   0        0        0      227 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/logger.py
+-rw-r--r--   0        0        0     1287 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/main.py
+-rw-r--r--   0        0        0     2550 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/render.py
+-rw-r--r--   0        0        0     1926 2023-06-21 23:13:33.780785 pymetasnap-0.2.0/extractor/utils.py
+-rw-r--r--   0        0        0      845 2023-06-21 23:13:33.784785 pymetasnap-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.2.0/PKG-INFO
```

### Comparing `pymetasnap-0.1.4/LICENSE` & `pymetasnap-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.4/README.md` & `pymetasnap-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.4/extractor/core.py` & `pymetasnap-0.2.0/extractor/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from pathlib import Path
 from typing import Dict
 
 import pandas as pd
 import requests
-from loguru import logger
-from rich import print
 from rich.progress import track
 
 from extractor.checks import StandardCheck
+from extractor.logger import logger
 from extractor.render import Requirements
 
 URLBASE = "https://pypi.org/pypi"
 
 
 def get_raw_data(project: str) -> Dict[str, str]:
     """
@@ -49,61 +48,62 @@
     project_urls = raw_data["project_urls"]
     gh_url_pattern = r"(https:\/\/|http:\/\/)github\.com"
     filtered_data = {
         "name": project_name,
         "version": version or raw_data["version"],
         "license": raw_data["license"],
         "homepage": raw_data["home_page"],
+        "release_url": raw_data["release_url"],
     }
     check = StandardCheck()
-    print(f"Searching GitHub url for: {project_name}")
+    logger.info(f"Searching GitHub url for: {project_name}")
+
+    # logger.info(f"Searching GitHub url for: {project_name}")
     if project_url != "" and check.gh_pattern(gh_url_pattern, project_url):
         filtered_data["project_url"] = project_url
 
     if project_urls:
-        print("Nested metadata found")
+        logger.debug("Nested metadata found")
         filtered_data["project_url"] = check.additional_urls(
             gh_url_pattern, project_urls
         )
+    if project_name == "pandas":
+        version = f"v{filtered_data['version']}"
+        filtered_data["version"] = version
 
-    filtered_data["version_url"] = (
-        f"{filtered_data['project_url']}/tree/{version}/"
-        if version
-        else filtered_data["release_url"]
-    )
-
+    filtered_data = check.version(version, gh_url_pattern, raw_data, filtered_data)
     return filtered_data
 
 
 def extract_data(source_path: Path, format: str) -> None:
     """
     Extract data based on the specified requirements format.
 
     Args:
         source_path: The path to the requirements file.
         format: The format of the requirements file.
 
     Returns:
         pd.DataFrame
     """
-    print("Starting process")
-    print(f"Retrieving: {source_path}")
+    logger.info("Starting process")
+    logger.debug(f"Retrieving: {source_path}")
     result = Requirements().render(source_path, format)
     pkgs_raw_metadata = []
-    for pkg in track(result, description="Processing..."):
+    for pkg in track(result):
         filtered_data = filter_data(
             get_raw_data(pkg[0]), pkg[1] if len(pkg) > 1 else None
         )
         pkgs_raw_metadata.append(filtered_data)
     return pd.DataFrame(pkgs_raw_metadata)
 
 
 def save_data(data: pd.DataFrame, output: Path):
-    print(f"Storing into: {output}")
+    logger.info(f"Storing into: {output}")
     if str(output).endswith(".csv"):
         data.to_csv(output, index=False)
-        print("All done! Have a Great day")
+        logger.info("All done! Have a Great day")
     elif str(output).endswith(".xlsx"):
         data.to_excel(output, index=False)
-        print("All done! Have a Great day")
+        logger.info("All done! Have a Great day")
     else:
         logger.error("Not supported format.")
```

### Comparing `pymetasnap-0.1.4/extractor/main.py` & `pymetasnap-0.2.0/extractor/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from enum import Enum
 from pathlib import Path
 
 import typer
+from rich import print
 from typing_extensions import Annotated
 
 from extractor.core import extract_data, save_data
 
 app = typer.Typer()
+VERSION = "0.2.0"
 
 
 class RequirementsFormat(str, Enum):
     pip_list = "pip_list"
     pip_freeze = "pip_freeze"
 
 
-# @app.command(name="version")
-# def version():
-#     return print(get_version_from_pyproject())
+@app.command(name="version")
+def version():
+    return print(VERSION)
 
 
 @app.command(name="extract")
-def extract(
+def main(
     source_path: Annotated[
         Path,
         typer.Option(
             exists=True,
             file_okay=True,
             dir_okay=False,
             writable=False,
```

### Comparing `pymetasnap-0.1.4/extractor/render.py` & `pymetasnap-0.2.0/extractor/render.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.1.4/extractor/utils.py` & `pymetasnap-0.2.0/extractor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import toml
-from loguru import logger
 from rich import print
 from rich.progress import track
 
 from extractor.core import filter_data, get_raw_data
+from extractor.logger import logger
 from extractor.render import Requirements
 
 
 def get_version_from_pyproject():
     with open("pyproject.toml") as f:
         pyproject_data = toml.load(f)
         version = (
```

### Comparing `pymetasnap-0.1.4/pyproject.toml` & `pymetasnap-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.1.4"
+version = "0.2.0"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
```

### Comparing `pymetasnap-0.1.4/PKG-INFO` & `pymetasnap-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.1.4
+Version: 0.2.0
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

