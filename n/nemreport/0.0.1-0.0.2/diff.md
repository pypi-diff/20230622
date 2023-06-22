# Comparing `tmp/nemreport-0.0.1.tar.gz` & `tmp/nemreport-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nemreport-0.0.1.tar", last modified: Fri Jun 16 23:25:22 2023, max compression
+gzip compressed data, was "nemreport-0.0.2.tar", last modified: Thu Jun 22 10:30:47 2023, max compression
```

## Comparing `nemreport-0.0.1.tar` & `nemreport-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rwxr-xr-x   0        0        0     1836 2023-06-15 10:33:44.765933 nemreport-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2023-04-13 01:26:35.356696 nemreport-0.0.1/LICENSE
--rw-r--r--   0        0        0       30 2023-06-15 10:36:18.254519 nemreport-0.0.1/MANIFEST.in
--rwxr-xr-x   0        0        0      652 2023-06-16 23:16:51.756079 nemreport-0.0.1/README.md
--rw-r--r--   0        0        0      126 2023-06-15 10:11:36.097013 nemreport-0.0.1/nemreport/__init__.py
--rw-r--r--   0        0        0       28 2022-10-22 23:26:41.883203 nemreport-0.0.1/nemreport/__main__.py
--rw-r--r--   0        0        0      842 2023-06-15 10:28:35.464673 nemreport-0.0.1/nemreport/cli.py
--rw-r--r--   0        0        0     2426 2023-06-16 23:19:59.660765 nemreport-0.0.1/nemreport/model.py
--rw-r--r--   0        0        0      568 2023-06-16 23:24:00.686508 nemreport-0.0.1/nemreport/prepare_db.py
--rwxr-xr-x   0        0        0     7839 2023-06-16 23:21:21.105281 nemreport-0.0.1/nemreport/report.py
--rw-r--r--   0        0        0   163873 2023-04-13 01:26:35.356696 nemreport-0.0.1/nemreport/templates/bootstrap.min.css
--rw-r--r--   0        0        0      735 2023-04-19 10:22:38.621358 nemreport-0.0.1/nemreport/templates/index.html
--rwxr-xr-x   0        0        0    11094 2023-06-16 10:34:56.714032 nemreport-0.0.1/nemreport/templates/nmi-report.html
--rw-r--r--   0        0        0       22 2023-06-15 10:09:42.378648 nemreport-0.0.1/nemreport/version.py
--rwxr-xr-x   0        0        0     1427 2023-06-16 23:05:16.185954 nemreport-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-16 23:01:01.582028 nemreport-0.0.1/requirements.txt
--rw-r--r--   0        0        0   285444 2023-06-16 23:15:18.935529 nemreport-0.0.1/screenshot.png
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 nemreport-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1836 2023-06-15 10:33:44.765933 nemreport-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1069 2023-04-13 01:26:35.356696 nemreport-0.0.2/LICENSE
+-rw-r--r--   0        0        0       30 2023-06-15 10:36:18.254519 nemreport-0.0.2/MANIFEST.in
+-rwxr-xr-x   0        0        0      652 2023-06-16 23:16:51.756079 nemreport-0.0.2/README.md
+-rw-r--r--   0        0        0      126 2023-06-15 10:11:36.097013 nemreport-0.0.2/nemreport/__init__.py
+-rw-r--r--   0        0        0       28 2022-10-22 23:26:41.883203 nemreport-0.0.2/nemreport/__main__.py
+-rw-r--r--   0        0        0      916 2023-06-22 10:25:53.156068 nemreport-0.0.2/nemreport/cli.py
+-rw-r--r--   0        0        0     2426 2023-06-22 10:21:33.221684 nemreport-0.0.2/nemreport/model.py
+-rw-r--r--   0        0        0      612 2023-06-22 10:28:30.895126 nemreport-0.0.2/nemreport/prepare_db.py
+-rwxr-xr-x   0        0        0     7853 2023-06-22 10:21:47.042078 nemreport-0.0.2/nemreport/report.py
+-rw-r--r--   0        0        0   163873 2023-04-13 01:26:35.356696 nemreport-0.0.2/nemreport/templates/bootstrap.min.css
+-rw-r--r--   0        0        0      735 2023-04-19 10:22:38.621358 nemreport-0.0.2/nemreport/templates/index.html
+-rwxr-xr-x   0        0        0    11094 2023-06-16 10:34:56.714032 nemreport-0.0.2/nemreport/templates/nmi-report.html
+-rw-r--r--   0        0        0       22 2023-06-22 10:08:41.553442 nemreport-0.0.2/nemreport/version.py
+-rwxr-xr-x   0        0        0     1426 2023-06-22 10:08:33.957250 nemreport-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2875 2023-06-22 10:11:26.616749 nemreport-0.0.2/requirements.txt
+-rw-r--r--   0        0        0   285444 2023-06-16 23:15:18.935529 nemreport-0.0.2/screenshot.png
+-rw-r--r--   0        0        0        0 2022-10-22 23:26:41.883203 nemreport-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-22 10:29:36.060259 nemreport-0.0.2/tests/test_cli.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 nemreport-0.0.2/PKG-INFO
```

### Comparing `nemreport-0.0.1/.gitignore` & `nemreport-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/LICENSE` & `nemreport-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/README.md` & `nemreport-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/nemreport/cli.py` & `nemreport-0.0.2/nemreport/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,13 +31,15 @@
     Generate energy report from NEM meter data files
     """
     pass
 
 
 @app.command()
 def update_db() -> None:
-    update_nem_database()
+    fp = update_nem_database()
+    typer.echo(f"Updated {fp}")
 
 
 @app.command()
 def build() -> None:
-    build_reports()
+    fp = build_reports()
+    typer.echo(f"Created {fp}")
```

### Comparing `nemreport-0.0.1/nemreport/model.py` & `nemreport-0.0.2/nemreport/model.py`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/nemreport/report.py` & `nemreport-0.0.2/nemreport/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import plotly.express as px
 from jinja2 import Environment, FileSystemLoader
 from nemreader.output_db import get_nmis
 
 from .model import (
     DB_PATH,
     db,
+    get_annual_data,
     get_date_range,
     get_day_data,
     get_season_data,
     get_usage_df,
-    get_annual_data,
 )
 from .prepare_db import update_nem_database
 
 log = logging.getLogger(__name__)
 this_dir = Path(__file__).parent
 template_dir = this_dir / "templates"
 env = Environment(loader=FileSystemLoader(template_dir))
@@ -268,7 +268,8 @@
         update_nem_database()
     copy_static_data()
     nmis = get_nmis(DB_PATH)
     for nmi in nmis:
         build_report(nmi)
     fp = Path(build_index(nmis)).resolve()
     webbrowser.open(fp.as_uri())
+    return fp
```

### Comparing `nemreport-0.0.1/nemreport/templates/bootstrap.min.css` & `nemreport-0.0.2/nemreport/templates/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/nemreport/templates/index.html` & `nemreport-0.0.2/nemreport/templates/index.html`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/nemreport/templates/nmi-report.html` & `nemreport-0.0.2/nemreport/templates/nmi-report.html`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/pyproject.toml` & `nemreport-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.8",
     "Operating System :: OS Independent",
 ]
 keywords = ["energy", "NEM12", "NEM13"]
 requires-python = ">=3.8"
 dynamic = ["version", "description"]
 dependencies = [
-    "nemreader>=v0.8.7",
+    "nemreader>=0.8.7",
     "jinja2",
     "pandas",
     "plotly",
     "calplot",
     "sqlite_utils",
     "pydantic",
     "typer",
@@ -34,15 +34,15 @@
 test = ["pytest >=2.7.3", "pytest-cov", "mypy"]
 dev = ["black", "flake8", "flake8-bugbear", "pep8-naming", "flake8-builtins"]
 
 [project.urls]
 Source = "https://github.com/aguinane/energy-report"
 
 [project.scripts]
-nemreader = "nemreport.cli:app"
+nemreport = "nemreport.cli:app"
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "-ra --failed-first --showlocals --durations=3 --cov=nemreport"
```

### Comparing `nemreport-0.0.1/screenshot.png` & `nemreport-0.0.2/screenshot.png`

 * *Files identical despite different names*

### Comparing `nemreport-0.0.1/PKG-INFO` & `nemreport-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nemreport
-Version: 0.0.1
+Version: 0.0.2
 Summary: Generate energy report from NEM meter data files
 Keywords: energy,NEM12,NEM13
 Author-email: Alex Guinman <alex@guinman.id.au>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
-Requires-Dist: nemreader>=v0.8.7
+Requires-Dist: nemreader>=0.8.7
 Requires-Dist: jinja2
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: calplot
 Requires-Dist: sqlite_utils
 Requires-Dist: pydantic
 Requires-Dist: typer
```

