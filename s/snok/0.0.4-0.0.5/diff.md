# Comparing `tmp/snok-0.0.4.tar.gz` & `tmp/snok-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snok-0.0.4.tar", last modified: Thu Jun 22 03:19:27 2023, max compression
+gzip compressed data, was "snok-0.0.5.tar", last modified: Thu Jun 22 03:54:27 2023, max compression
```

## Comparing `snok-0.0.4.tar` & `snok-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:19:27.703660 snok-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 03:19:07.000000 snok-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:19:27.703660 snok-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 03:19:07.000000 snok-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-22 03:19:07.000000 snok-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-22 03:19:27.703660 snok-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:19:27.699660 snok-0.0.4/snok/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 03:19:07.000000 snok-0.0.4/snok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 03:19:07.000000 snok-0.0.4/snok/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 03:19:07.000000 snok-0.0.4/snok/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:19:07.000000 snok-0.0.4/snok/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:19:27.699660 snok-0.0.4/snok/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:19:07.000000 snok-0.0.4/snok/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-22 03:19:07.000000 snok-0.0.4/snok/services/new.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 03:19:07.000000 snok-0.0.4/snok/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:19:27.699660 snok-0.0.4/snok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:19:27.000000 snok-0.0.4/snok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-22 03:19:27.000000 snok-0.0.4/snok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:19:27.000000 snok-0.0.4/snok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:19:27.000000 snok-0.0.4/snok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 03:19:27.000000 snok-0.0.4/snok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 03:19:27.000000 snok-0.0.4/snok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:19:27.703660 snok-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-22 03:19:07.000000 snok-0.0.4/tests/test_cli_new.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 03:19:07.000000 snok-0.0.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 03:54:09.000000 snok-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:54:27.314362 snok-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 03:54:09.000000 snok-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-22 03:54:09.000000 snok-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:54:27.314362 snok-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.302362 snok-0.0.5/snok/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 03:54:09.000000 snok-0.0.5/snok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 03:54:09.000000 snok-0.0.5/snok/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 03:54:09.000000 snok-0.0.5/snok/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-22 03:54:09.000000 snok-0.0.5/snok/services/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.302362 snok-0.0.5/snok/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/templates/__app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/gunicorn_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/templates/__app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/templates/__app/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/routers/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/services/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__app_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__app_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__package/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/snok/templates/__package_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/snok/templates/__shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/_pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 03:54:09.000000 snok-0.0.5/snok/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-22 03:54:09.000000 snok-0.0.5/tests/test_cli_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 03:54:09.000000 snok-0.0.5/tests/test_version.py
```

### Comparing `snok-0.0.4/LICENSE` & `snok-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `snok-0.0.4/PKG-INFO` & `snok-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: snok Version: 0.0.4 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.5 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.4/README.md` & `snok-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `snok-0.0.4/pyproject.toml` & `snok-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,23 @@
 [project.urls]
 Home = "https://github.com/anthonycorletti/snok"
 Documentation = "https://snok.corletti.xyz"
 
 [project.scripts]
 snok = "snok.cli:app"
 
+[tool.setuptools.package-data]
+snok = ["py.typed", "templates/**/*"]
+
+[tool.setuptools.dynamic]
+version = {attr = "snok.__version__"}
+
+[tool.setuptools.packages.find]
+exclude = ["tests"]
+
 [tool.ruff]
 line-length = 88
 ignore = [
     "D10",
 ]
 include = [
     "*.py",
@@ -164,10 +173,7 @@
 ]
 
 [tool.coverage.html]
 directory = "htmlcov"
 
 [tool.coverage.xml]
 output = "coverage.xml"
-
-[tool.setuptools.dynamic.version]
-attr = "snok.__version__"
```

### Comparing `snok-0.0.4/snok/cli.py` & `snok-0.0.5/snok/cli.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.4/snok/services/new.py` & `snok-0.0.5/snok/services/new.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.4/snok.egg-info/PKG-INFO` & `snok-0.0.5/snok.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.4
+Version: 0.0.5
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
-Metadata-Version: 2.1 Name: snok Version: 0.0.4 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.5 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.4/tests/test_cli_new.py` & `snok-0.0.5/tests/test_cli_new.py`

 * *Files identical despite different names*

