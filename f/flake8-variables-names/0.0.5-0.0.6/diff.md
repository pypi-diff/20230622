# Comparing `tmp/flake8_variables_names-0.0.5.tar.gz` & `tmp/flake8_variables_names-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_variables_names-0.0.5.tar", last modified: Thu Feb 24 12:39:54 2022, max compression
+gzip compressed data, was "flake8_variables_names-0.0.6.tar", last modified: Thu Jun 22 12:43:19 2023, max compression
```

## Comparing `flake8_variables_names-0.0.5.tar` & `flake8_variables_names-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 12:39:54.540612 flake8_variables_names-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-24 12:39:30.000000 flake8_variables_names-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-02-24 12:39:54.540612 flake8_variables_names-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2566 2022-02-24 12:39:30.000000 flake8_variables_names-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 12:39:54.540612 flake8_variables_names-0.0.5/flake8_variables_names/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-24 12:39:30.000000 flake8_variables_names-0.0.5/flake8_variables_names/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1915 2022-02-24 12:39:30.000000 flake8_variables_names-0.0.5/flake8_variables_names/ast_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-02-24 12:39:30.000000 flake8_variables_names-0.0.5/flake8_variables_names/checker.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-02-24 12:39:30.000000 flake8_variables_names-0.0.5/flake8_variables_names/list_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 12:39:54.540612 flake8_variables_names-0.0.5/flake8_variables_names.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-02-24 12:39:54.000000 flake8_variables_names-0.0.5/flake8_variables_names.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-02-24 12:39:54.000000 flake8_variables_names-0.0.5/flake8_variables_names.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 12:39:54.000000 flake8_variables_names-0.0.5/flake8_variables_names.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-02-24 12:39:54.000000 flake8_variables_names-0.0.5/flake8_variables_names.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 12:39:54.000000 flake8_variables_names-0.0.5/flake8_variables_names.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-02-24 12:39:54.000000 flake8_variables_names-0.0.5/flake8_variables_names.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      571 2022-02-24 12:39:54.544612 flake8_variables_names-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-02-24 12:39:30.000000 flake8_variables_names-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:43:19.702527 flake8_variables_names-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 12:42:29.000000 flake8_variables_names-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-22 12:43:19.702527 flake8_variables_names-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-22 12:42:29.000000 flake8_variables_names-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:43:19.698526 flake8_variables_names-0.0.6/flake8_variables_names/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 12:42:29.000000 flake8_variables_names-0.0.6/flake8_variables_names/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-22 12:42:29.000000 flake8_variables_names-0.0.6/flake8_variables_names/ast_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-06-22 12:42:29.000000 flake8_variables_names-0.0.6/flake8_variables_names/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 12:42:29.000000 flake8_variables_names-0.0.6/flake8_variables_names/list_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:43:19.698526 flake8_variables_names-0.0.6/flake8_variables_names.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-22 12:43:19.000000 flake8_variables_names-0.0.6/flake8_variables_names.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-22 12:43:19.000000 flake8_variables_names-0.0.6/flake8_variables_names.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:43:19.000000 flake8_variables_names-0.0.6/flake8_variables_names.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 12:43:19.000000 flake8_variables_names-0.0.6/flake8_variables_names.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:43:19.000000 flake8_variables_names-0.0.6/flake8_variables_names.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 12:43:19.000000 flake8_variables_names-0.0.6/flake8_variables_names.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-22 12:43:19.702527 flake8_variables_names-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-22 12:42:29.000000 flake8_variables_names-0.0.6/setup.py
```

### Comparing `flake8_variables_names-0.0.5/LICENSE` & `flake8_variables_names-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_variables_names-0.0.5/PKG-INFO` & `flake8_variables_names-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: flake8_variables_names
-Version: 0.0.5
+Version: 0.0.6
 Summary: A flake8 extension that helps to make more readable variables names
 Home-page: https://github.com/best-doctor/flake8-variables-names
 Author: Ilya Lebedev
 Author-email: melevir@gmail.com
 License: MIT
 Keywords: flake8 naming
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -87,9 +86,7 @@
 Here are useful tips:
 
 - You can run all checks and tests with `make check`.
   Please do it before CI does.
 - We use [BestDoctor python styleguide](https://github.com/best-doctor/guides/blob/master/guides/en/python_styleguide.md).
 - We respect [Django CoC](https://www.djangoproject.com/conduct/).
   Make soft, not bullshit.
-
-
```

### Comparing `flake8_variables_names-0.0.5/README.md` & `flake8_variables_names-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `flake8_variables_names-0.0.5/flake8_variables_names/checker.py` & `flake8_variables_names-0.0.6/flake8_variables_names/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from optparse import OptionParser
 from typing import Generator, Tuple, List
 
 from flake8_variables_names import __version__ as version
 from flake8_variables_names.ast_helpers import extract_all_variable_names
 
+
 ErrorTuple = Tuple[int, int, str, type]
 
 
 class VariableNamesChecker:
     name = 'flake8-variables-names'
     version = version
 
@@ -71,14 +72,15 @@
             return self._variable_names_blacklist
 
     @classmethod
     def add_options(cls, parser: OptionParser) -> None:
         parser.add_option(
             '--use-varnames-strict-mode',
             action='store_true',
+            parse_from_config=True,
         )
 
     @classmethod
     def parse_options(cls, options) -> None:
         cls.use_strict_mode = bool(options.use_varnames_strict_mode)
 
     def run(self) -> Generator[ErrorTuple, None, None]:
```

### Comparing `flake8_variables_names-0.0.5/flake8_variables_names.egg-info/PKG-INFO` & `flake8_variables_names-0.0.6/flake8_variables_names.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: flake8-variables-names
-Version: 0.0.5
+Version: 0.0.6
 Summary: A flake8 extension that helps to make more readable variables names
 Home-page: https://github.com/best-doctor/flake8-variables-names
 Author: Ilya Lebedev
 Author-email: melevir@gmail.com
 License: MIT
 Keywords: flake8 naming
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -87,9 +86,7 @@
 Here are useful tips:
 
 - You can run all checks and tests with `make check`.
   Please do it before CI does.
 - We use [BestDoctor python styleguide](https://github.com/best-doctor/guides/blob/master/guides/en/python_styleguide.md).
 - We respect [Django CoC](https://www.djangoproject.com/conduct/).
   Make soft, not bullshit.
-
-
```

### Comparing `flake8_variables_names-0.0.5/setup.cfg` & `flake8_variables_names-0.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `flake8_variables_names-0.0.5/setup.py` & `flake8_variables_names-0.0.6/setup.py`

 * *Files identical despite different names*

