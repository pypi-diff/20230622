# Comparing `tmp/snok-0.0.2.tar.gz` & `tmp/snok-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snok-0.0.2.tar", last modified: Thu Jun 22 02:33:13 2023, max compression
+gzip compressed data, was "snok-0.0.3.tar", last modified: Thu Jun 22 03:10:55 2023, max compression
```

## Comparing `snok-0.0.2.tar` & `snok-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.126236 snok-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 02:32:55.000000 snok-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 02:33:13.126236 snok-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 02:32:55.000000 snok-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-22 02:32:55.000000 snok-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-22 02:33:13.126236 snok-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.122236 snok-0.0.2/snok/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 02:32:55.000000 snok-0.0.2/snok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-22 02:32:55.000000 snok-0.0.2/snok/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 02:32:55.000000 snok-0.0.2/snok/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:32:55.000000 snok-0.0.2/snok/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.122236 snok-0.0.2/snok/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:32:55.000000 snok-0.0.2/snok/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-22 02:32:55.000000 snok-0.0.2/snok/services/new.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.122236 snok-0.0.2/snok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.126236 snok-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-22 02:32:55.000000 snok-0.0.2/tests/test_cli_new.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 02:32:55.000000 snok-0.0.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:10:55.062278 snok-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 03:10:27.000000 snok-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:10:55.062278 snok-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 03:10:27.000000 snok-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-22 03:10:27.000000 snok-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 03:10:55.062278 snok-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:10:55.058278 snok-0.0.3/snok/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 03:10:27.000000 snok-0.0.3/snok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 03:10:27.000000 snok-0.0.3/snok/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 03:10:27.000000 snok-0.0.3/snok/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:10:27.000000 snok-0.0.3/snok/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:10:55.058278 snok-0.0.3/snok/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:10:27.000000 snok-0.0.3/snok/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-22 03:10:27.000000 snok-0.0.3/snok/services/new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 03:10:27.000000 snok-0.0.3/snok/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:10:55.058278 snok-0.0.3/snok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:10:55.000000 snok-0.0.3/snok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 03:10:55.000000 snok-0.0.3/snok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:10:55.000000 snok-0.0.3/snok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:10:55.000000 snok-0.0.3/snok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 03:10:55.000000 snok-0.0.3/snok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 03:10:55.000000 snok-0.0.3/snok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:10:55.062278 snok-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-22 03:10:27.000000 snok-0.0.3/tests/test_cli_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 03:10:27.000000 snok-0.0.3/tests/test_version.py
```

### Comparing `snok-0.0.2/LICENSE` & `snok-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `snok-0.0.2/PKG-INFO` & `snok-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.2
+Version: 0.0.3
 Summary: 🚀 A simple, modern, full-stack toolkit for Python 🐍
 Author-email: Anthony Corletti <anthcor+snok@gmail.com>
 License: MIT
 Project-URL: Home, https://github.com/anthonycorletti/snok
 Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snok Version: 0.0.2 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.3 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.2/README.md` & `snok-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `snok-0.0.2/pyproject.toml` & `snok-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snok-0.0.2/snok/cli.py` & `snok-0.0.3/snok/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import os
-
 from typer import Argument, Option, Typer, echo
 
 from snok import __version__
 from snok.const import APP_DESC, APP_NAME, ProjectType
 from snok.services.new import NewPackageService
+from snok.utils import _get_default_output_dir
 
 app = Typer(
     name=APP_NAME,
     help=APP_DESC,
     no_args_is_help=True,
 )
 
@@ -39,30 +38,28 @@
     ),
     description: str = Option(
         "A new Python project.",
         "-d",
         "--description",
         help="The description of the project. Defaults to 'A new Python project.'",
     ),
-    output_dir: str = Option(
-        os.getcwd(),
-        "-o",
-        "--output-dir",
-        help="The output directory of the project. Defaults to the current directory.",
-    ),
     type: ProjectType = Option(
         "package",
         "-t",
         "--type",
         help="The type of project to create. Defaults to 'package'",
     ),
+    output_dir: str = Option(
+        _get_default_output_dir(),
+        "-o",
+        "--output-dir",
+        help="The output directory of the project. "
+        "Defaults to the same directory of the current virtual environment.",
+    ),
 ) -> None:
     new_project_service_dispatcher = {
         ProjectType.package: NewPackageService,
     }
     new_project_service = new_project_service_dispatcher[type]()
     new_project_service.create(
-        name=name,
-        desc=description,
-        type=type,
-        output_dir=output_dir,
+        name=name, desc=description, type=type, output_dir=output_dir
     )
```

### Comparing `snok-0.0.2/snok/services/new.py` & `snok-0.0.3/snok/services/new.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import importlib.resources as resources
 import os
 
 from jinja2 import Template
 
 from snok.const import ProjectType
 
 
 class BaseNewService:
     def __init__(self) -> None:
-        self.root_template_dir = "snok/templates"
+        import snok
+
+        self.root_template_dir = str(resources.files(snok)) + "/templates"
 
     def create(
         self,
         name: str,
         desc: str,
         output_dir: str,
         type: ProjectType = ProjectType.package,
@@ -72,36 +75,35 @@
         desc: str,
         output_dir: str,
         type: ProjectType = ProjectType.package,
     ) -> None:
         shared_template_dir = f"{self.root_template_dir}/__shared"
         package_template_dir = f"{self.root_template_dir}/__{type.value}"
         tests_template_dir = f"{self.root_template_dir}/__{type.value}_tests"
-        root_output_dir = f"{output_dir}/{name}"
-        os.makedirs(root_output_dir, exist_ok=True)
+        os.makedirs(output_dir, exist_ok=True)
         self._render_content_directory(
             name=name,
             desc=desc,
             source_dir=shared_template_dir,
-            output_dir=root_output_dir,
+            output_dir=output_dir,
             type=type,
         )
-        package_root = f"{root_output_dir}/{name}"
+        package_root = f"{output_dir}/{name}"
         os.makedirs(package_root, exist_ok=True)
         self._render_content_directory(
             name=name,
             desc=desc,
             source_dir=package_template_dir,
             output_dir=package_root,
             type=type,
         )
-        package_test_root = f"{root_output_dir}/tests"
+        package_test_root = f"{output_dir}/tests"
         os.makedirs(package_test_root, exist_ok=True)
         self._render_content_directory(
             name=name,
             desc=desc,
             source_dir=tests_template_dir,
             output_dir=package_test_root,
             type=type,
         )
-        if not os.path.exists(f"{root_output_dir}/.git"):
-            os.system(f"git init {root_output_dir} > /dev/null 2>&1")
+        if not os.path.exists(f"{output_dir}/.git"):
+            os.system(f"git init {output_dir} > /dev/null 2>&1")
```

### Comparing `snok-0.0.2/snok.egg-info/PKG-INFO` & `snok-0.0.3/snok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.2
+Version: 0.0.3
 Summary: 🚀 A simple, modern, full-stack toolkit for Python 🐍
 Author-email: Anthony Corletti <anthcor+snok@gmail.com>
 License: MIT
 Project-URL: Home, https://github.com/anthonycorletti/snok
 Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: snok Version: 0.0.2 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.3 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.2/tests/test_cli_new.py` & `snok-0.0.3/tests/test_cli_new.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,35 +2,34 @@
 
 from typer.testing import CliRunner
 
 from snok import __version__
 from snok.cli import app
 
 
-def test_new_package(cli_runner: CliRunner, setup_test_content_output_dir: str) -> None:
+def test_new_package(cli_runner: CliRunner, setup_test_project_dir: str) -> None:
     response = cli_runner.invoke(
         app,
-        ["new", "test_package", "-o", setup_test_content_output_dir],
+        ["new", "test_package", "-o", setup_test_project_dir],
     )
     assert response.exit_code == 0
     # assert the output directory exists
     for path in [
-        f"{setup_test_content_output_dir}/test_package",
-        f"{setup_test_content_output_dir}/test_package/test_package",
-        f"{setup_test_content_output_dir}/test_package/tests",
-        f"{setup_test_content_output_dir}/test_package/.git",
-        f"{setup_test_content_output_dir}/test_package/README.md",
-        f"{setup_test_content_output_dir}/test_package/setup.cfg",
-        f"{setup_test_content_output_dir}/test_package/pyproject.toml",
-        f"{setup_test_content_output_dir}/test_package/test_package/__init__.py",
-        f"{setup_test_content_output_dir}/test_package/test_package/main.py",
-        f"{setup_test_content_output_dir}/test_package/tests/__init__.py",
-        f"{setup_test_content_output_dir}/test_package/tests/conftest.py",
-        f"{setup_test_content_output_dir}/test_package/tests/test_main.py",
-        f"{setup_test_content_output_dir}/test_package/tests/test_version.py",
+        f"{setup_test_project_dir}/test_package",
+        f"{setup_test_project_dir}/tests",
+        f"{setup_test_project_dir}/.git",
+        f"{setup_test_project_dir}/README.md",
+        f"{setup_test_project_dir}/setup.cfg",
+        f"{setup_test_project_dir}/pyproject.toml",
+        f"{setup_test_project_dir}/test_package/__init__.py",
+        f"{setup_test_project_dir}/test_package/main.py",
+        f"{setup_test_project_dir}/tests/__init__.py",
+        f"{setup_test_project_dir}/tests/conftest.py",
+        f"{setup_test_project_dir}/tests/test_main.py",
+        f"{setup_test_project_dir}/tests/test_version.py",
     ]:
         assert os.path.exists(path)
 
 
 def test_version(cli_runner: CliRunner) -> None:
     response = cli_runner.invoke(app, ["version"])
     assert response.exit_code == 0
```

