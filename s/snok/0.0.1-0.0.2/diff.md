# Comparing `tmp/snok-0.0.1.tar.gz` & `tmp/snok-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snok-0.0.1.tar", last modified: Thu Jun 22 02:26:49 2023, max compression
+gzip compressed data, was "snok-0.0.2.tar", last modified: Thu Jun 22 02:33:13 2023, max compression
```

## Comparing `snok-0.0.1.tar` & `snok-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:26:49.222503 snok-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 02:26:31.000000 snok-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 02:26:49.222503 snok-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 02:26:31.000000 snok-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-22 02:26:31.000000 snok-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-22 02:26:49.222503 snok-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:26:49.218503 snok-0.0.1/snok/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 02:26:31.000000 snok-0.0.1/snok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-22 02:26:31.000000 snok-0.0.1/snok/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 02:26:31.000000 snok-0.0.1/snok/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:26:31.000000 snok-0.0.1/snok/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:26:49.222503 snok-0.0.1/snok/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:26:31.000000 snok-0.0.1/snok/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-22 02:26:31.000000 snok-0.0.1/snok/services/new.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:26:49.222503 snok-0.0.1/snok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 02:26:49.000000 snok-0.0.1/snok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 02:26:49.000000 snok-0.0.1/snok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:26:49.000000 snok-0.0.1/snok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:26:49.000000 snok-0.0.1/snok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-22 02:26:49.000000 snok-0.0.1/snok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 02:26:49.000000 snok-0.0.1/snok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:26:49.222503 snok-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-22 02:26:31.000000 snok-0.0.1/tests/test_cli_new.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 02:26:31.000000 snok-0.0.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.126236 snok-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 02:32:55.000000 snok-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 02:33:13.126236 snok-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 02:32:55.000000 snok-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-22 02:32:55.000000 snok-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-22 02:33:13.126236 snok-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.122236 snok-0.0.2/snok/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 02:32:55.000000 snok-0.0.2/snok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-22 02:32:55.000000 snok-0.0.2/snok/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 02:32:55.000000 snok-0.0.2/snok/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:32:55.000000 snok-0.0.2/snok/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.122236 snok-0.0.2/snok/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:32:55.000000 snok-0.0.2/snok/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-22 02:32:55.000000 snok-0.0.2/snok/services/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.122236 snok-0.0.2/snok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 02:33:13.000000 snok-0.0.2/snok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:33:13.126236 snok-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-06-22 02:32:55.000000 snok-0.0.2/tests/test_cli_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 02:32:55.000000 snok-0.0.2/tests/test_version.py
```

### Comparing `snok-0.0.1/LICENSE` & `snok-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `snok-0.0.1/PKG-INFO` & `snok-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.1
+Version: 0.0.2
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
-Metadata-Version: 2.1 Name: snok Version: 0.0.1 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.2 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.1/README.md` & `snok-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `snok-0.0.1/pyproject.toml` & `snok-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 requires-python = ">=3.11"
 dependencies = [
     "black>=21.10",
     "coverage>=6.1.1",
     "fastapi>=0.97.0",
     "gunicorn>=20.1.0",
     "invoke>=2.0.0",
+    "jinja2>=3.1.2",
     "mypy>=0.910",
     "packaging>=21.0",
     "pre-commit>=2.17.0",
     "pydantic>=1.8.2",
     "pytest-cov>=3.0.0",
     "pytest-xdist>=3.3.1",
     "pytest>=6.2.5",
@@ -123,15 +124,15 @@
     "snok",
     "tests",
 ]
 exclude = [
     "dist",
     "build",
     ".venv",
-    "snok/templates/*"
+    "snok/templates/*",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.pytest.ini_options]
 addopts = [
```

### Comparing `snok-0.0.1/snok/cli.py` & `snok-0.0.2/snok/cli.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.1/snok/services/new.py` & `snok-0.0.2/snok/services/new.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.1/snok.egg-info/PKG-INFO` & `snok-0.0.2/snok.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.1
+Version: 0.0.2
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
-Metadata-Version: 2.1 Name: snok Version: 0.0.1 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.2 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.1/tests/test_cli_new.py` & `snok-0.0.2/tests/test_cli_new.py`

 * *Files identical despite different names*

