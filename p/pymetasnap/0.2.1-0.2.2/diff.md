# Comparing `tmp/pymetasnap-0.2.1.tar.gz` & `tmp/pymetasnap-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymetasnap-0.2.1.tar", max compression
+gzip compressed data, was "pymetasnap-0.2.2.tar", max compression
```

## Comparing `pymetasnap-0.2.1.tar` & `pymetasnap-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/LICENSE
--rw-r--r--   0        0        0     2927 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/__init__.py
--rw-r--r--   0        0        0     1724 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/checks.py
--rw-r--r--   0        0        0     3278 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/core.py
--rw-r--r--   0        0        0      227 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/logger.py
--rw-r--r--   0        0        0     1287 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/main.py
--rw-r--r--   0        0        0     2619 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/render.py
--rw-r--r--   0        0        0     1669 2023-06-22 14:43:34.896235 pymetasnap-0.2.1/extractor/utils.py
--rw-r--r--   0        0        0      845 2023-06-22 14:43:34.900235 pymetasnap-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2927 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/__init__.py
+-rw-r--r--   0        0        0     2492 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/checks.py
+-rw-r--r--   0        0        0     2998 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/core.py
+-rw-r--r--   0        0        0      227 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/logger.py
+-rw-r--r--   0        0        0     1253 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/main.py
+-rw-r--r--   0        0        0     3262 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/render.py
+-rw-r--r--   0        0        0     1669 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/extractor/utils.py
+-rw-r--r--   0        0        0      845 2023-06-22 20:05:35.815502 pymetasnap-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 pymetasnap-0.2.2/PKG-INFO
```

### Comparing `pymetasnap-0.2.1/LICENSE` & `pymetasnap-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.1/README.md` & `pymetasnap-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.1/extractor/checks.py` & `pymetasnap-0.2.2/extractor/checks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from typing import Dict
 
 from extractor.logger import logger
 
 
 class StandardCheck:
     def gh_pattern(self, pattern: str, url: str, custom_error: str = None):
         try:
@@ -19,22 +20,42 @@
             "Source Code",
             "Source code",
             "Source",
             "Homepage",
             "Home",
             "Repository",
             "repository",
+            "Download",
+            "download",
         ]
         for title, url in urls:
             if _ := self.gh_pattern(pattern, url) and title in possible_keys:
                 return url
 
+    def licenses(self, raw_data: Dict) -> str:
+        licenses = raw_data["license"]
+        if licenses != "" and licenses is not None:
+            return licenses
+        licenses_pattern = r"^[lL]icense.*"
+
+        for lic in raw_data["classifiers"]:
+            if license_found := re.search(licenses_pattern, lic):
+                return license_found.group()
+
+    def project_url(self, pattern: str, project_url: str, project_urls: Dict) -> str:
+        if project_url != "" and self.gh_pattern(pattern, project_url):
+            return project_url
+
+        if project_urls:
+            logger.debug("Nested metadata found")
+            return self.additional_urls(pattern, project_urls)
+
     def version(
-        self, version: str, pattern: str, raw_data: dict, filtered_data: dict
-    ) -> dict:
+        self, version: str, pattern: str, raw_data: Dict, filtered_data: Dict
+    ) -> Dict:
         project_default_error = "No project url found, please check manually"
         version_default_error = "No version url found, please check manually"
         if version and self.gh_pattern(
             pattern, filtered_data.get("project_url"), project_default_error
         ):
             filtered_data[
                 "version_url"
```

### Comparing `pymetasnap-0.2.1/extractor/core.py` & `pymetasnap-0.2.2/extractor/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,34 +42,27 @@
 
     Returns:
         A dictionary containing filtered metadata.
     """
     project_name = raw_data["name"]
     project_url = raw_data["project_url"]
     project_urls = raw_data["project_urls"]
+    check = StandardCheck()
     gh_url_pattern = r"(https:\/\/|http:\/\/)github\.com"
     filtered_data = {
         "name": project_name,
         "version": version or raw_data["version"],
-        "license": raw_data["license"],
+        "license": check.licenses(raw_data),
         "homepage": raw_data["home_page"],
         "release_url": raw_data["release_url"],
+        "project_url": check.project_url(gh_url_pattern, project_url, project_urls),
     }
-    check = StandardCheck()
-    logger.info(f"Searching GitHub url for: {project_name}")
 
-    # logger.info(f"Searching GitHub url for: {project_name}")
-    if project_url != "" and check.gh_pattern(gh_url_pattern, project_url):
-        filtered_data["project_url"] = project_url
+    logger.info(f"Searching GitHub url for: {project_name}")
 
-    if project_urls:
-        logger.debug("Nested metadata found")
-        filtered_data["project_url"] = check.additional_urls(
-            gh_url_pattern, project_urls
-        )
     if project_name == "pandas":
         version = f"v{filtered_data['version']}"
         filtered_data["version"] = version
 
     filtered_data = check.version(version, gh_url_pattern, raw_data, filtered_data)
     return filtered_data
```

### Comparing `pymetasnap-0.2.1/extractor/main.py` & `pymetasnap-0.2.2/extractor/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,38 @@
-from enum import Enum
 from pathlib import Path
 
 import typer
 from rich import print
 from typing_extensions import Annotated
 
 from extractor.core import extract_data, save_data
+from extractor.render import RequirementsFormat
 
 app = typer.Typer()
-VERSION = "0.2.1"
-
-
-class RequirementsFormat(str, Enum):
-    pip_list = "pip_list"
-    pip_freeze = "pip_freeze"
+VERSION = "0.2.2"
 
 
 @app.command(name="version")
 def version():
     return print(VERSION)
 
 
 @app.command(name="extract")
 def main(
     source_path: Annotated[
         Path,
         typer.Option(
             exists=True,
             file_okay=True,
-            dir_okay=False,
-            writable=False,
+            dir_okay=True,
+            writable=True,
             readable=True,
             resolve_path=True,
             prompt=True,
-            help="Requirements file path",
+            help="Requirements files paths. Can be a single file, or a folder",
         ),
     ] = "",
     output: Annotated[
         Path,
         typer.Option(
             file_okay=True,
             dir_okay=False,
```

### Comparing `pymetasnap-0.2.1/extractor/render.py` & `pymetasnap-0.2.2/extractor/render.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,74 @@
 """This module contains Requirements class, which is the core of the current process."""
-
+import os
 import re
+from enum import Enum
 from typing import List, Tuple
 
 
+class RequirementsFormat(str, Enum):
+    pip_list = "pip_list"
+    pip_freeze = "pip_freeze"
+
+
 class Requirements:
     """
     A class that handles parsing and rendering requirements data.
 
     Attributes:
         None
 
     Methods:
         _read_file_contents: Read the contents of a file.
         _from_pip_freeze: Parse data in the pip freeze format.
         _from_pip_list: Parse data in the pip list format.
         render: Render the requirements data based on the specified format.
     """
 
+    def _merge_multiple_requirements(self, source_path: str) -> set:
+        requirements = set()
+        paths = os.listdir(source_path)
+        paths = [
+            os.path.join(source_path, path) for path in paths if path.endswith(".txt")
+        ]
+
+        for file in paths:
+            with open(file, "r") as src:
+                requirements.update(src.read().splitlines())
+
+        return requirements
+
     def _read_file_contents(self, source_path: str) -> str:
         """
         Read the contents of a file.
 
         Args:
             source_path: The path to the file to be read.
 
         Returns:
             The contents of the file as a string.
         """
-        return open(source_path, "r").read()
+        basepath = os.path.abspath(source_path)
+        if os.path.isdir(basepath):
+            return self._merge_multiple_requirements(basepath)
+        with open(basepath, "r") as src:
+            return src.read().splitlines()
 
     def _from_pip_freeze(self, data: str) -> List[Tuple[str, str]]:
         """
         Parse data in the pip freeze format.
 
         Args:
             data: The pip freeze formatted data to be parsed.
 
         Returns:
             A list of tuples containing package names and versions.
         """
-        lines = data.strip().split("\n")
-        lines = [line for line in lines if not line.startswith("#")]
+
+        lines = [line for line in data if not line.startswith("#")]
         pattern = r"(==|<=|>=|<|>)"
         package_data = [re.split(pattern, line) for line in lines]
         return [
             (package[0], package[2]) if len(package) > 1 else package
             for package in package_data
         ]
 
@@ -55,16 +78,16 @@
 
         Args:
             data: The pip list formatted data to be parsed.
 
         Returns:
             A list of tuples containing package names and versions.
         """
-        lines = data.strip().split("\n")
-        package_data = [tuple(line.split()) for line in lines[2:]]
+
+        package_data = [tuple(line.split()) for line in data[2:]]
         return [(package[0], package[1]) for package in package_data]  # pylint
 
     def render(self, source_path: str, format: str) -> List[Tuple[str, str]]:
         """
         Render the requirements data based on the specified format.
 
         Args:
```

### Comparing `pymetasnap-0.2.1/extractor/utils.py` & `pymetasnap-0.2.2/extractor/utils.py`

 * *Files identical despite different names*

### Comparing `pymetasnap-0.2.1/pyproject.toml` & `pymetasnap-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pymetasnap"
-version = "0.2.1"
+version = "0.2.2"
 description = "This package allows you to scrape metadata from the Python Package Index"
 authors = ["cristian-rincon <cristian.o.rincon.b@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "extractor"}]
 
 [tool.poetry.scripts]
```

### Comparing `pymetasnap-0.2.1/PKG-INFO` & `pymetasnap-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymetasnap
-Version: 0.2.1
+Version: 0.2.2
 Summary: This package allows you to scrape metadata from the Python Package Index
 License: MIT
 Author: cristian-rincon
 Author-email: cristian.o.rincon.b@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

