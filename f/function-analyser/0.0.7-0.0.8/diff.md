# Comparing `tmp/function-analyser-0.0.7.tar.gz` & `tmp/function-analyser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "function-analyser-0.0.7.tar", last modified: Thu Jun 22 10:06:48 2023, max compression
+gzip compressed data, was "function-analyser-0.0.8.tar", last modified: Thu Jun 22 10:54:27 2023, max compression
```

## Comparing `function-analyser-0.0.7.tar` & `function-analyser-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 10:06:38.000000 function-analyser-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:06:48.025287 function-analyser-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 10:06:38.000000 function-analyser-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-22 10:06:41.000000 function-analyser-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 10:06:48.025287 function-analyser-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/src/function_analyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 10:06:48.000000 function-analyser-0.0.7/src/function_analyser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/missing_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/parse_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 10:06:38.000000 function-analyser-0.0.7/src/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:06:48.025287 function-analyser-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_missing_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_parse_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-06-22 10:06:38.000000 function-analyser-0.0.7/tests/test_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 10:53:55.000000 function-analyser-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:54:26.994257 function-analyser-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 10:53:55.000000 function-analyser-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-06-22 10:54:16.000000 function-analyser-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 10:54:26.994257 function-analyser-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/src/function_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/missing_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/parse_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 10:53:55.000000 function-analyser-0.0.8/src/function_analyser/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/src/function_analyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 10:54:26.000000 function-analyser-0.0.8/src/function_analyser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:26.994257 function-analyser-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_missing_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_parse_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-06-22 10:53:55.000000 function-analyser-0.0.8/tests/test_statistics.py
```

### Comparing `function-analyser-0.0.7/LICENSE.txt` & `function-analyser-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.7/PKG-INFO` & `function-analyser-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-analyser
-Version: 0.0.7
+Version: 0.0.8
 Summary: Identify long functions to refactor with this function analyser
 Author-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 Maintainer-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 License: Copyright 2023, Nicholas Hemley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `function-analyser-0.0.7/README.md` & `function-analyser-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.7/pyproject.toml` & `function-analyser-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "function-analyser"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = '0.0.7'  # Required
+version = '0.0.8'  # Required
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "Identify long functions to refactor with this function analyser"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `function-analyser-0.0.7/src/function_analyser.egg-info/PKG-INFO` & `function-analyser-0.0.8/src/function_analyser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: function-analyser
-Version: 0.0.7
+Version: 0.0.8
 Summary: Identify long functions to refactor with this function analyser
 Author-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 Maintainer-email: Nicholas Hemley <nicholas.oliver.hemley@gmail.com>
 License: Copyright 2023, Nicholas Hemley
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

### Comparing `function-analyser-0.0.7/src/main.py` & `function-analyser-0.0.8/src/function_analyser/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 import argparse
-import pathlib
+import os
 
 from parse_function import parse_files
-from statistics import get_statistics, apply_thresholds, filter_by_percentile
+from function_analyser.statistics import get_statistics, filter_by_percentile
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description='Function analysis')
     parser.add_argument('-f', '--filepath', help='Source file path to analyse', required=False)
     args = vars(parser.parse_args())
     return args
 
 
 def main():
     args = parse_args()
     if args["filepath"]:
         file_path = args["filepath"]
     else:
-        file_path = pathlib.Path(__file__).parent
+        file_path = os.getcwd()
 
     series_list = parse_files(file_path)
-    for series in series_list:
-        print(get_statistics(series))
-
-    # use percentiles over specific thresholds ...
-    series_list2 = filter_by_percentile(series_list)
-    for series in series_list2:
-        # note - we want the function names (i.e. index) as well ...
-        print(get_statistics(series, include_index=True))
-
-    # extract main offender (-1 being last in list) ...
-    worst_offender = series_list2[0].index[-1]
-    print(f"Best contender / Worst offender is {worst_offender}")
+    if len(series_list) > 0:
+        for series in series_list:
+            print(get_statistics(series))
+
+        # use percentiles over specific thresholds ...
+        series_list2 = filter_by_percentile(series_list)
+        for series in series_list2:
+            # note - we want the function names (i.e. index) as well ...
+            print(get_statistics(series, include_index=True))
+
+        # extract main offender (-1 being last in list) ...
+        worst_offender = series_list2[0].index[-1]
+        print(f"Best contender / Worst offender is {worst_offender}")
+    else:
+        print("No source files found.")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `function-analyser-0.0.7/src/parse_function.py` & `function-analyser-0.0.8/src/function_analyser/parse_function.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.7/src/statistics.py` & `function-analyser-0.0.8/src/function_analyser/statistics.py`

 * *Files identical despite different names*

### Comparing `function-analyser-0.0.7/tests/test_missing_docstring.py` & `function-analyser-0.0.8/tests/test_missing_docstring.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import inspect
 import unittest
 
-import parse_function
 from missing_docstring import has_docstring
+from function_analyser import parse_function
 
 
 class TestMissingDocString(unittest.TestCase):
 
   def test_0(self):
     """
     test with docstring
     :return:
     """
     def function():
       pass
     bool = has_docstring(function)
-    self.assertTrue(bool)
+    self.assertFalse(bool)
 
     def function2():
       """
       With doc string
       :return:
       """
       pass
     bool = has_docstring(function2)
-    self.assertFalse(bool)
+    self.assertTrue(bool)
 
   def test_1(self):
     functions = inspect.getmembers(parse_function, inspect.isfunction)
     for function in functions:
         print(f"function {function[0]} {has_docstring(function)}")
```

### Comparing `function-analyser-0.0.7/tests/test_parse_function.py` & `function-analyser-0.0.8/tests/test_parse_function.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import pathlib
 import unittest
 import pandas
 from pandas import Series
 
-from parse_function import parse_file, parse_files, FUNCTION_LENGTHS, PARAMETER_COUNT, create_series
+from function_analyser.parse_function import parse_file, parse_files, FUNCTION_LENGTHS, PARAMETER_COUNT, create_series
 
 
 class TestParseFunctions(unittest.TestCase):
 
     def test_0(self):
         """
         Test for custom series attribute
@@ -35,15 +35,15 @@
     def test_4(self):
         """
         Tests for parse_file
         No thresholds
         :return:
         """
         base_dir = pathlib.Path(__file__).parent
-        file = os.path.join(base_dir, "..", "src", "parse_function.py")
+        file = os.path.join(base_dir, "..", "src", "function_analyser", "parse_function.py")
         with open(file) as file:
             series_list = parse_file(file)
             self.assertEqual(6, len(series_list[0]))
             self.assertTrue(isinstance(series_list[0].filename, str))
 
     def test_5(self):
         """
@@ -66,10 +66,21 @@
         series_list = parse_files(base_dir)
         self.assertEqual(2, len(series_list))
         self.assertEqual(FUNCTION_LENGTHS, series_list[0].type)
         self.assertTrue(len(series_list[0]) > 0)
         self.assertEqual(PARAMETER_COUNT, series_list[1].type)
         self.assertTrue(len(series_list[1]) > 0)
 
+    def test_7(self):
+        """
+        Test for parse_files
+
+        No source files
+        :return:
+        """
+        base_dir = pathlib.Path(__file__).parent.parent
+        series_list = parse_files(base_dir)
+        self.assertEqual(0, len(series_list))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `function-analyser-0.0.7/tests/test_statistics.py` & `function-analyser-0.0.8/tests/test_statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 import unittest
 
 import numpy as np
 import pandas
 
 from parse_function import FUNCTION_LENGTHS, PARAMETER_COUNT, parse_files
-from statistics import get_statistics, filter_series_by_threshold, get_function_lengths_over_threshold, \
+from function_analyser.statistics import get_statistics, filter_series_by_threshold, get_function_lengths_over_threshold, \
     get_parameter_count_over_threshold, apply_thresholds, filter_by_percentile
 
 
 class TestStatistics(unittest.TestCase):
     def test_0(self):
         """
         Test for get_statistics
@@ -108,15 +108,15 @@
     def test_5(self):
         """
         Test for filter_by_percentile
         80%
         :return:
         """
         base_dir = pathlib.Path(__file__).parent
-        file_path = os.path.join(base_dir, "..", "src")
+        file_path = os.path.join(base_dir, "..", "src", "function_analyser")
 
         series_list = parse_files(file_path)
         series_list2 = filter_by_percentile(series_list, percentile=80)
         for series in series_list2:
             print(get_statistics(series, include_index=True))
 
         worst_offender = series_list2[0].index[-1]
```

