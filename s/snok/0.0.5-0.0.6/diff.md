# Comparing `tmp/snok-0.0.5.tar.gz` & `tmp/snok-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snok-0.0.5.tar", last modified: Thu Jun 22 03:54:27 2023, max compression
+gzip compressed data, was "snok-0.0.6.tar", last modified: Thu Jun 22 05:38:32 2023, max compression
```

## Comparing `snok-0.0.5.tar` & `snok-0.0.6.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 03:54:09.000000 snok-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:54:27.314362 snok-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 03:54:09.000000 snok-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-22 03:54:09.000000 snok-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:54:27.314362 snok-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.302362 snok-0.0.5/snok/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 03:54:09.000000 snok-0.0.5/snok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 03:54:09.000000 snok-0.0.5/snok/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 03:54:09.000000 snok-0.0.5/snok/const.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-22 03:54:09.000000 snok-0.0.5/snok/services/new.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.302362 snok-0.0.5/snok/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/templates/__app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/db.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/gunicorn_conf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/templates/__app/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok/templates/__app/routers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/routers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/routers/snok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__app/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app/services/snok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__app_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/_base.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/_head.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__app_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__app_tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.310362 snok-0.0.5/snok/templates/__package/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/snok/templates/__package_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__package_tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/snok/templates/__shared/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/_pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-22 03:54:09.000000 snok-0.0.5/snok/templates/__shared/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 03:54:09.000000 snok-0.0.5/snok/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.306362 snok-0.0.5/snok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 03:54:27.000000 snok-0.0.5/snok.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:54:27.314362 snok-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-22 03:54:09.000000 snok-0.0.5/tests/test_cli_new.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 03:54:09.000000 snok-0.0.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.632758 snok-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 05:38:05.000000 snok-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 05:38:32.632758 snok-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-22 05:38:05.000000 snok-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-06-22 05:38:05.000000 snok-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:38:32.632758 snok-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 05:38:05.000000 snok-0.0.6/snok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 05:38:05.000000 snok-0.0.6/snok/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 05:38:05.000000 snok-0.0.6/snok/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-22 05:38:05.000000 snok-0.0.6/snok/services/new.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok/templates/__app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/gunicorn_conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok/templates/__app/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok/templates/__app/routers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/routers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/routers/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok/templates/__app/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app/services/snok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.632758 snok-0.0.6/snok/templates/__app_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app_templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app_templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app_templates/_base.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app_templates/_head.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app_templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.632758 snok-0.0.6/snok/templates/__app_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__app_tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.632758 snok-0.0.6/snok/templates/__package/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__package/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.632758 snok-0.0.6/snok/templates/__package_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__package_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__package_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__package_tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__package_tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.632758 snok-0.0.6/snok/templates/__shared/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/_.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/_.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/_.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/_pyproject_toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-06-22 05:38:05.000000 snok-0.0.6/snok/templates/__shared/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 05:38:05.000000 snok-0.0.6/snok/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.628758 snok-0.0.6/snok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 05:38:32.000000 snok-0.0.6/snok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-22 05:38:32.000000 snok-0.0.6/snok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 05:38:32.000000 snok-0.0.6/snok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 05:38:32.000000 snok-0.0.6/snok.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 05:38:32.000000 snok-0.0.6/snok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 05:38:32.000000 snok-0.0.6/snok.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 05:38:32.632758 snok-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-22 05:38:05.000000 snok-0.0.6/tests/test_cli_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 05:38:05.000000 snok-0.0.6/tests/test_version.py
```

### Comparing `snok-0.0.5/LICENSE` & `snok-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `snok-0.0.5/PKG-INFO` & `snok-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: snok Version: 0.0.5 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.6 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.5/README.md` & `snok-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `snok-0.0.5/pyproject.toml` & `snok-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snok-0.0.5/snok/cli.py` & `snok-0.0.6/snok/cli.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.5/snok/services/new.py` & `snok-0.0.6/snok/services/new.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,18 +31,28 @@
     ) -> None:
         for root, dirs, files in os.walk(source_dir):
             if not ("__pycache__" in root or "_cache" in root):
                 for file in files:
                     file_path = os.path.join(root, file)
                     relative_path = os.path.relpath(file_path, source_dir)
                     output_path = os.path.join(output_dir, relative_path)
-                    if output_path.endswith("_pyproject.toml"):
+
+                    if output_path.endswith("_pyproject_toml"):
                         output_path = output_path.replace(
-                            "_pyproject.toml", "pyproject.toml"
+                            "_pyproject_toml", "pyproject.toml"
                         )
+
+                    _basename = os.path.basename(relative_path)
+                    if _basename.startswith("_.") and not _basename.endswith(".py"):
+                        _newbasename = _basename.replace("_.", ".")
+                        output_path = os.path.join(
+                            output_dir,
+                            relative_path.replace(_basename, _newbasename),
+                        )
+
                     self._render_content_file(
                         name=name,
                         desc=desc,
                         source_path=file_path,
                         output_path=output_path,
                         type=type,
                     )
```

### Comparing `snok-0.0.5/snok/templates/__shared/CONTRIBUTING.md` & `snok-0.0.6/snok/templates/__shared/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `snok-0.0.5/snok/templates/__shared/_pyproject.toml` & `snok-0.0.6/snok/templates/__shared/_pyproject_toml`

 * *Files 11% similar despite different names*

```diff
@@ -26,14 +26,26 @@
     "pytest-xdist>=3.3.1",
     "pytest>=6.2.5",
     "ruff>=0.0.98",
     "setuptools>=67.8.0",
     "wheel>=0.36",
 ]
 
+[tool.setuptools.dynamic.version]
+attr = "{{ __template_name }}.__version__"
+
+[tool.setuptools.package-data]
+{{ __template_name }} = ["py.typed"]
+
+[tool.setuptools.dynamic]
+version = {attr = "{{ __template_name }}.__version__"}
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
@@ -122,10 +134,7 @@
 ]
 
 [tool.coverage.html]
 directory = "htmlcov"
 
 [tool.coverage.xml]
 output = "coverage.xml"
-
-[tool.setuptools.dynamic.version]
-attr = "{{ __template_name }}.__version__"
```

### Comparing `snok-0.0.5/snok/templates/__shared/tasks.py` & `snok-0.0.6/snok/templates/__shared/tasks.py`

 * *Files identical despite different names*

### Comparing `snok-0.0.5/snok.egg-info/PKG-INFO` & `snok-0.0.6/snok.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snok
-Version: 0.0.5
+Version: 0.0.6
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
-Metadata-Version: 2.1 Name: snok Version: 0.0.5 Summary: ð A simple, modern,
+Metadata-Version: 2.1 Name: snok Version: 0.0.6 Summary: ð A simple, modern,
 full-stack toolkit for Python ð Author-email: Anthony Corletti
 snok@gmail.com> License: MIT Project-URL: Home, https://github.com/
 anthonycorletti/snok Project-URL: Documentation, https://snok.corletti.xyz
 Requires-Python: >=3.11 Description-Content-Type: text/markdown Provides-Extra:
 dev License-File: LICENSE
                                     [Snok]
            ð A simple, modern, full-stack toolkit for Python ð
```

### Comparing `snok-0.0.5/snok.egg-info/SOURCES.txt` & `snok-0.0.6/snok.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -34,13 +34,15 @@
 snok/templates/__package/main.py
 snok/templates/__package_tests/__init__.py
 snok/templates/__package_tests/conftest.py
 snok/templates/__package_tests/test_main.py
 snok/templates/__package_tests/test_version.py
 snok/templates/__shared/CONTRIBUTING.md
 snok/templates/__shared/README.md
-snok/templates/__shared/_pyproject.toml
+snok/templates/__shared/_.editorconfig
+snok/templates/__shared/_.gitignore
+snok/templates/__shared/_.pre-commit-config.yaml
+snok/templates/__shared/_pyproject_toml
 snok/templates/__shared/py.typed
-snok/templates/__shared/setup.cfg
 snok/templates/__shared/tasks.py
 tests/test_cli_new.py
 tests/test_version.py
```

### Comparing `snok-0.0.5/tests/test_cli_new.py` & `snok-0.0.6/tests/test_cli_new.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 
 def test_new_package(cli_runner: CliRunner, setup_test_project_dir: str) -> None:
     response = cli_runner.invoke(
         app,
         ["new", "test_package", "-o", setup_test_project_dir],
     )
     assert response.exit_code == 0
+    print(os.listdir(setup_test_project_dir))
     # assert the output directory exists
     for path in [
         f"{setup_test_project_dir}/test_package",
         f"{setup_test_project_dir}/tests",
         f"{setup_test_project_dir}/.git",
         f"{setup_test_project_dir}/README.md",
-        f"{setup_test_project_dir}/setup.cfg",
         f"{setup_test_project_dir}/pyproject.toml",
+        f"{setup_test_project_dir}/.gitignore",
         f"{setup_test_project_dir}/test_package/__init__.py",
         f"{setup_test_project_dir}/test_package/main.py",
         f"{setup_test_project_dir}/tests/__init__.py",
         f"{setup_test_project_dir}/tests/conftest.py",
         f"{setup_test_project_dir}/tests/test_main.py",
         f"{setup_test_project_dir}/tests/test_version.py",
     ]:
```

