# Comparing `tmp/clouding_server_manager-1.0.4.tar.gz` & `tmp/clouding_server_manager-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouding_server_manager-1.0.4.tar", max compression
+gzip compressed data, was "clouding_server_manager-1.0.5.tar", max compression
```

## Comparing `clouding_server_manager-1.0.4.tar` & `clouding_server_manager-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.4/LICENSE
--rw-r--r--   0        0        0     6956 2023-06-06 10:05:32.541615 clouding_server_manager-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.4/clouding_server_manager/__init__.py
--rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.4/clouding_server_manager/__main__.py
--rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.4/clouding_server_manager/commands.py
--rw-r--r--   0        0        0      782 2023-06-06 10:06:49.903304 clouding_server_manager-1.0.4/clouding_server_manager/constants.py
--rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.4/clouding_server_manager/helpers.py
--rw-r--r--   0        0        0      898 2023-06-06 10:06:22.916055 clouding_server_manager-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     7565 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-18 10:43:31.505631 clouding_server_manager-1.0.5/LICENSE
+-rw-r--r--   0        0        0     7039 2023-06-22 15:46:16.226441 clouding_server_manager-1.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-06-18 10:43:31.505631 clouding_server_manager-1.0.5/clouding_server_manager/__init__.py
+-rw-r--r--   0        0        0      590 2023-06-18 10:43:31.505631 clouding_server_manager-1.0.5/clouding_server_manager/__main__.py
+-rw-r--r--   0        0        0     3998 2023-06-18 10:43:31.505631 clouding_server_manager-1.0.5/clouding_server_manager/commands.py
+-rw-r--r--   0        0        0      782 2023-06-18 10:43:31.505631 clouding_server_manager-1.0.5/clouding_server_manager/constants.py
+-rw-r--r--   0        0        0     7418 2023-06-18 10:43:31.505631 clouding_server_manager-1.0.5/clouding_server_manager/helpers.py
+-rw-r--r--   0        0        0      898 2023-06-22 15:45:00.501531 clouding_server_manager-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     7648 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.5/PKG-INFO
```

### Comparing `clouding_server_manager-1.0.4/LICENSE` & `clouding_server_manager-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.4/README.md` & `clouding_server_manager-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Clouding Server Manager
-![Version](https://img.shields.io/badge/Version-1.0.4-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.5-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
@@ -130,31 +130,35 @@
 
 ## Development Setup
 If you want to contribute to the project or run the development environment, follow these additional steps:
 1. Install the development dependencies:
     ```bash
     poetry install --with dev
     ```
-2. Format the code:
+2. Install pre-commit hooks:
+    ```bash
+    poetry run pre-commit install
+    ```
+3. Format the code:
     ```bash
     poetry run black clouding_server_manager
     ```
-3. Lint the code:
+4. Lint the code:
     ```bash
     poetry run flake8 clouding_server_manager
     ```
-4. Run static type checking:
+5. Run static type checking:
     ```bash
     poetry run mypy clouding_server_manager
     ```
-5. Generate the documentation:
+6. Generate the documentation:
     ```bash
     cd docs && poetry run make html
     ```
-6. Do everything at once (except for generating the documentation):
+7. Do everything at once (except for generating the documentation):
     ```bash
     poetry run pre-commit run --all-files
     ```
 That's it! You now have the project set up and ready for development or execution.
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `clouding_server_manager-1.0.4/clouding_server_manager/__main__.py` & `clouding_server_manager-1.0.5/clouding_server_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.4/clouding_server_manager/commands.py` & `clouding_server_manager-1.0.5/clouding_server_manager/commands.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.4/clouding_server_manager/constants.py` & `clouding_server_manager-1.0.5/clouding_server_manager/constants.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.4/clouding_server_manager/helpers.py` & `clouding_server_manager-1.0.5/clouding_server_manager/helpers.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.4/pyproject.toml` & `clouding_server_manager-1.0.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clouding-server-manager"
-version = "1.0.4"
+version = "1.0.5"
 description = "A Python project to easily manage Clouding servers from the command line."
 authors = ["dmarts05 <dmarts05@estudiantes.unileon.es>"]
 readme = "README.md"
 packages = [{include = "clouding_server_manager"}]
 
 [tool.poetry.scripts]
 clouding-sm = "clouding_server_manager.__main__:main"
```

### Comparing `clouding_server_manager-1.0.4/PKG-INFO` & `clouding_server_manager-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: clouding-server-manager
-Version: 1.0.4
+Version: 1.0.5
 Summary: A Python project to easily manage Clouding servers from the command line.
 Author: dmarts05
 Author-email: dmarts05@estudiantes.unileon.es
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Clouding Server Manager
-![Version](https://img.shields.io/badge/Version-1.0.4-brightgreen.svg)
+![Version](https://img.shields.io/badge/Version-1.0.5-brightgreen.svg)
 ![Python](https://img.shields.io/badge/Python-3.9-brightgreen.svg)
 ![License](https://img.shields.io/badge/License-MIT-blue.svg)
 
 Clouding Server Manager is a Python project that allows you to manage your Clouding servers from the command line. It is designed to list, archive, and unarchive servers in your Clouding account. It uses the [Clouding API](https://api.clouding.io/docs) to perform the actions.
 
 ## Table of Contents
 * [Features](#features)
@@ -146,31 +146,35 @@
 
 ## Development Setup
 If you want to contribute to the project or run the development environment, follow these additional steps:
 1. Install the development dependencies:
     ```bash
     poetry install --with dev
     ```
-2. Format the code:
+2. Install pre-commit hooks:
+    ```bash
+    poetry run pre-commit install
+    ```
+3. Format the code:
     ```bash
     poetry run black clouding_server_manager
     ```
-3. Lint the code:
+4. Lint the code:
     ```bash
     poetry run flake8 clouding_server_manager
     ```
-4. Run static type checking:
+5. Run static type checking:
     ```bash
     poetry run mypy clouding_server_manager
     ```
-5. Generate the documentation:
+6. Generate the documentation:
     ```bash
     cd docs && poetry run make html
     ```
-6. Do everything at once (except for generating the documentation):
+7. Do everything at once (except for generating the documentation):
     ```bash
     poetry run pre-commit run --all-files
     ```
 That's it! You now have the project set up and ready for development or execution.
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

