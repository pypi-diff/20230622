# Comparing `tmp/function-analyser-0.0.5.tar.gz` & `tmp/function-analyser-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-analyser-0.0.5.tar", last modified: Thu Jun 22 09:38:44 2023, max compression
+gzip compressed data, was "function-analyser-0.0.7.tar", last modified: Thu Jun 22 10:06:48 2023, max compression
```

## Comparing `function-analyser-0.0.5.tar` & `function-analyser-0.0.7.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:44.896296 function-analyser-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 09:38:31.000000 function-analyser-0.0.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-22 09:38:44.896296 function-analyser-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-22 09:38:31.000000 function-analyser-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-22 09:38:37.000000 function-analyser-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:38:44.896296 function-analyser-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:44.892296 function-analyser-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:44.892296 function-analyser-0.0.5/src/function_analyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-06-22 09:38:44.000000 function-analyser-0.0.5/src/function_analyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 09:38:44.000000 function-analyser-0.0.5/src/function_analyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:38:44.000000 function-analyser-0.0.5/src/function_analyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 09:38:44.000000 function-analyser-0.0.5/src/function_analyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 09:38:44.000000 function-analyser-0.0.5/src/function_analyser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 09:38:31.000000 function-analyser-0.0.5/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 09:38:31.000000 function-analyser-0.0.5/src/missing_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-22 09:38:31.000000 function-analyser-0.0.5/src/parse_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 09:38:31.000000 function-analyser-0.0.5/src/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:44.896296 function-analyser-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 09:38:31.000000 function-analyser-0.0.5/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 09:38:31.000000 function-analyser-0.0.5/tests/test_missing_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-22 09:38:31.000000 function-analyser-0.0.5/tests/test_parse_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-22 09:38:31.000000 function-analyser-0.0.5/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 10:06:38.000000 function-analyser-0.0.7/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:06:48.025287 function-analyser-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 10:06:38.000000 function-analyser-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-22 10:06:41.000000 function-analyser-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 10:06:48.025287 function-analyser-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/src/function_analyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/missing_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/parse_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_missing_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_parse_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_statistics.py
```

### Comparing `function-analyser-0.0.5/LICENSE.txt` & `function-analyser-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.5/PKG-INFO` & `function-analyser-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-analyser
-Version: 0.0.5
+Version: 0.0.7
 Summary: Identify long functions to refactor with this function analyser
 Author-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 Maintainer-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 License: Copyright 2023, Nicholas Hemley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -28,14 +28,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # function-analyser
 
+TL;DR;
+```commandline
+pip install function-analyser
+
+```
 There is much debate about the ideal length of a function or method.
 
 E.g.
 ```
 The first rule of functions is that they should be small.
 The second rule of functions is that they should be smaller than that.
 Functions should not be 100 lines long.
```

### Comparing `function-analyser-0.0.5/README.md` & `function-analyser-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # function-analyser
 
+TL;DR;
+```commandline
+pip install function-analyser
+
+```
 There is much debate about the ideal length of a function or method.
 
 E.g.
 ```
 The first rule of functions is that they should be small.
 The second rule of functions is that they should be smaller than that.
 Functions should not be 100 lines long.
```

### Comparing `function-analyser-0.0.5/pyproject.toml` & `function-analyser-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "function-analyser"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = '0.0.5'  # Required
+version = '0.0.7'  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Identify long functions to refactor with this function analyser"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `function-analyser-0.0.5/src/function_analyser.egg-info/PKG-INFO` & `function-analyser-0.0.7/src/function_analyser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-analyser
-Version: 0.0.5
+Version: 0.0.7
 Summary: Identify long functions to refactor with this function analyser
 Author-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 Maintainer-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 License: Copyright 2023, Nicholas Hemley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -28,14 +28,19 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
 
 # function-analyser
 
+TL;DR;
+```commandline
+pip install function-analyser
+
+```
 There is much debate about the ideal length of a function or method.
 
 E.g.
 ```
 The first rule of functions is that they should be small.
 The second rule of functions is that they should be smaller than that.
 Functions should not be 100 lines long.
```

### Comparing `function-analyser-0.0.5/src/main.py` & `function-analyser-0.0.7/src/main.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.5/src/parse_function.py` & `function-analyser-0.0.7/src/parse_function.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.5/src/statistics.py` & `function-analyser-0.0.7/src/statistics.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.5/tests/test_missing_docstring.py` & `function-analyser-0.0.7/tests/test_missing_docstring.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.5/tests/test_parse_function.py` & `function-analyser-0.0.7/tests/test_parse_function.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.5/tests/test_statistics.py` & `function-analyser-0.0.7/tests/test_statistics.py`

 * *Files identical despite different names*

