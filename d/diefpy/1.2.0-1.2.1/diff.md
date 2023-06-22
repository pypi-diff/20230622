# Comparing `tmp/diefpy-1.2.0.tar.gz` & `tmp/diefpy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diefpy-1.2.0.tar", last modified: Thu Nov 24 15:19:45 2022, max compression
+gzip compressed data, was "diefpy-1.2.1.tar", last modified: Thu Jun 22 08:17:51 2023, max compression
```

## Comparing `diefpy-1.2.0.tar` & `diefpy-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 15:19:45.629025 diefpy-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2022-11-24 15:19:31.000000 diefpy-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2022-11-24 15:19:31.000000 diefpy-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2022-11-24 15:19:45.629025 diefpy-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2022-11-24 15:19:31.000000 diefpy-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2022-11-24 15:19:31.000000 diefpy-1.2.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 15:19:45.629025 diefpy-1.2.0/diefpy/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2022-11-24 15:19:31.000000 diefpy-1.2.0/diefpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 15:19:45.629025 diefpy-1.2.0/diefpy/data/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2022-11-24 15:19:31.000000 diefpy-1.2.0/diefpy/data/metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)   531277 2022-11-24 15:19:31.000000 diefpy-1.2.0/diefpy/data/traces.csv
--rw-r--r--   0 runner    (1001) docker     (123)    31386 2022-11-24 15:19:31.000000 diefpy-1.2.0/diefpy/dief.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2022-11-24 15:19:31.000000 diefpy-1.2.0/diefpy/radaraxes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-11-24 15:19:45.629025 diefpy-1.2.0/diefpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2022-11-24 15:19:45.000000 diefpy-1.2.0/diefpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2022-11-24 15:19:45.000000 diefpy-1.2.0/diefpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-11-24 15:19:45.000000 diefpy-1.2.0/diefpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2022-11-24 15:19:45.000000 diefpy-1.2.0/diefpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-11-24 15:19:45.000000 diefpy-1.2.0/diefpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2022-11-24 15:19:45.629025 diefpy-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2022-11-24 15:19:31.000000 diefpy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:17:51.200745 diefpy-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-22 08:17:37.000000 diefpy-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 08:17:37.000000 diefpy-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-22 08:17:51.200745 diefpy-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-22 08:17:37.000000 diefpy-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 08:17:37.000000 diefpy-1.2.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:17:51.200745 diefpy-1.2.1/diefpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-22 08:17:37.000000 diefpy-1.2.1/diefpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:17:51.200745 diefpy-1.2.1/diefpy/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-22 08:17:37.000000 diefpy-1.2.1/diefpy/data/metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   531277 2023-06-22 08:17:37.000000 diefpy-1.2.1/diefpy/data/traces.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    32272 2023-06-22 08:17:37.000000 diefpy-1.2.1/diefpy/dief.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-22 08:17:37.000000 diefpy-1.2.1/diefpy/radaraxes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 08:17:51.200745 diefpy-1.2.1/diefpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-06-22 08:17:51.000000 diefpy-1.2.1/diefpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-22 08:17:51.000000 diefpy-1.2.1/diefpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 08:17:51.000000 diefpy-1.2.1/diefpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 08:17:51.000000 diefpy-1.2.1/diefpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 08:17:51.000000 diefpy-1.2.1/diefpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-22 08:17:51.204745 diefpy-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-22 08:17:37.000000 diefpy-1.2.1/setup.py
```

### Comparing `diefpy-1.2.0/LICENSE` & `diefpy-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `diefpy-1.2.0/PKG-INFO` & `diefpy-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: diefpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for computing diefficiency metrics dief@t and dief@k.
 Home-page: https://github.com/SDM-TIB/diefpy
-Download-URL: https://github.com/SDM-TIB/diefpy/archive/refs/tags/v1.2.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/diefpy/archive/refs/tags/v1.2.1.tar.gz
 Author: Philipp D. Rohde, Nikoleta Themeliotou
 Author-email: philipp.rohde@tib.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SDM-TIB/diefpy/issues
 Keywords: metrics benchmarking efficiency diefficiency-metrics dief python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Matplotlib
```

### Comparing `diefpy-1.2.0/README.md` & `diefpy-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `diefpy-1.2.0/diefpy/__init__.py` & `diefpy-1.2.1/diefpy/__init__.py`

 * *Files identical despite different names*

### Comparing `diefpy-1.2.0/diefpy/data/traces.csv` & `diefpy-1.2.1/diefpy/data/traces.csv`

 * *Files identical despite different names*

### Comparing `diefpy-1.2.0/diefpy/dief.py` & `diefpy-1.2.1/diefpy/dief.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 Python library for computing diefficiency metrics **dief@t** and **dief@k**.
 
 The metrics **dief@t** and **dief@k** allow for measuring the diefficiency during
 an elapsed time period *t* or while *k* answers are produced, respectively.
 **dief@t** and **dief@k** rely on the computation of the area under the curve (AUC) of
 answer traces, and thus capturing the answer rate concentration over a time interval.
 """
+import re
+
 import matplotlib.lines as mlines
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticker
 import numpy as np
 from matplotlib.figure import Figure
 
 from diefpy.radaraxes import radar_factory
 
-
 DEFAULT_COLORS = ("#ECC30B", "#D56062", "#84BCDA")
 """Default colors for printing plots: yellow, red, blue"""
 
 
 def dieft(inputtrace: np.ndarray, inputtest: str, t: float = -1.0, continue_to_end: bool = True) -> np.ndarray:
     """
     Computes the **dief@t** metric for a specific test at a given time point *t*.
@@ -239,14 +240,37 @@
     # Plot the answer traces for each test.
     for t in tests:
         plots.append(plot_answer_trace(inputtrace, t, colors))
 
     return plots
 
 
+def sorted_alphanumeric(list_):
+    """
+    Sorts a list alphanumerically.
+
+    The given list is sorted alphanumerically. This is done using two lambda expressions for the sorting key.
+
+    :param list_: The list to be sorted.
+    :return: The alphanumerically sorted list.
+
+    **Examples**
+
+    >>> sorted_alphanumeric(['Q1', 'Q3', 'Q10', 'Q2'])
+    ['Q1', 'Q2', 'Q3', 'Q10']
+    >>> sorted_alphanumeric(['A', '1', '10', '2', '100', 'B', 'a', 'Hello', 'Q1', 'Q2'])
+    ['1', '2', '10', '100', 'A', 'a', 'B', 'Hello', 'Q1', Q2']
+    >>> sorted_alphanumeric(['1.0.0', '0.9.0', '1.2.1', '1.2.0'])
+    ['0.9.0', '1.0.0', '1.2.0', '1.2.1']
+    """
+    digit2int = lambda text: int(text) if text.isdigit() else text
+    alphanumeric_key = lambda key: [digit2int(c) for c in re.split('([0-9]+)', key.lower())]
+    return sorted(list_, key=alphanumeric_key)
+
+
 def plot_execution_time(metrics: np.ndarray, colors: list = DEFAULT_COLORS, log_scale: bool = False) -> Figure:
     """
     Creates a bar chart with the overall *execution time* for all the tests and approaches in the metrics data.
 
     Bar chart presenting the conventional performance measure *execution time*.
     Each test is represented as a group of bars representing the approaches.
 
@@ -260,15 +284,15 @@
     >>> plot_execution_time(metrics)
     >>> plot_execution_time(metrics, ["#ECC30B","#D56062","#84BCDA"])
     >>> plot_execution_time(metrics, log_scale=True)
     >>> plot_execution_time(metrics, ["#ECC30B","#D56062","#84BCDA"], log_scale=True)
     """
     # Obtain test and approaches to compare.
     approaches = np.unique(metrics['approach'])
-    tests = np.unique(metrics['test'])
+    tests = sorted_alphanumeric(np.unique(metrics['test']))
 
     color_map = dict(zip(approaches, colors))
 
     fig, ax = plt.subplots(figsize=(0.95*len(tests), 5), dpi=100)
     fig.subplots_adjust(top=0.85, bottom=0.25, left=0.08)
 
     index = np.arange(len(tests))
```

### Comparing `diefpy-1.2.0/diefpy/radaraxes.py` & `diefpy-1.2.1/diefpy/radaraxes.py`

 * *Files identical despite different names*

### Comparing `diefpy-1.2.0/diefpy.egg-info/PKG-INFO` & `diefpy-1.2.1/diefpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: diefpy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for computing diefficiency metrics dief@t and dief@k.
 Home-page: https://github.com/SDM-TIB/diefpy
-Download-URL: https://github.com/SDM-TIB/diefpy/archive/refs/tags/v1.2.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/diefpy/archive/refs/tags/v1.2.1.tar.gz
 Author: Philipp D. Rohde, Nikoleta Themeliotou
 Author-email: philipp.rohde@tib.eu
 License: MIT
 Project-URL: Bug Tracker, https://github.com/SDM-TIB/diefpy/issues
 Keywords: metrics benchmarking efficiency diefficiency-metrics dief python
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Matplotlib
```

### Comparing `diefpy-1.2.0/setup.py` & `diefpy-1.2.1/setup.py`

 * *Files identical despite different names*

