# Comparing `tmp/plottah-0.1.0.tar.gz` & `tmp/plottah-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plottah-0.1.0.tar", max compression
+gzip compressed data, was "plottah-0.1.1.tar", max compression
```

## Comparing `plottah-0.1.0.tar` & `plottah-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      796 2023-06-22 11:27:07.932712 plottah-0.1.0/README.md
--rw-r--r--   0        0        0       22 2023-06-22 11:30:53.499061 plottah-0.1.0/plottah/__init__.py
--rw-r--r--   0        0        0     1012 2023-06-22 12:44:11.607614 plottah-0.1.0/plottah/__main__.py
--rw-r--r--   0        0        0     1339 2023-06-19 19:34:19.357898 plottah-0.1.0/plottah/colors.py
--rw-r--r--   0        0        0     3056 2023-06-22 09:19:12.089888 plottah-0.1.0/plottah/config.py
--rw-r--r--   0        0        0      988 2023-06-22 09:55:14.056657 plottah-0.1.0/plottah/main.py
--rw-r--r--   0        0        0       24 2023-06-20 17:12:04.651705 plottah-0.1.0/plottah/plot_builder/__init__.py
--rw-r--r--   0        0        0     2720 2023-06-22 12:44:18.230172 plottah-0.1.0/plottah/plot_builder/builders.py
--rw-r--r--   0        0        0     7488 2023-06-22 12:44:18.976051 plottah-0.1.0/plottah/plot_handler/PlotHandler.py
--rw-r--r--   0        0        0       37 2023-06-20 17:27:02.673177 plottah-0.1.0/plottah/plot_handler/__init__.py
--rw-r--r--   0        0        0     7530 2023-06-22 12:44:22.633547 plottah-0.1.0/plottah/plots/BinEventRatePlot.py
--rw-r--r--   0        0        0     3987 2023-06-22 12:44:23.133501 plottah-0.1.0/plottah/plots/DistPlot.py
--rw-r--r--   0        0        0     1927 2023-06-22 07:41:05.603043 plottah-0.1.0/plottah/plots/PlotProtocol.py
--rw-r--r--   0        0        0     3578 2023-06-22 12:44:24.105798 plottah-0.1.0/plottah/plots/RocCurvePlot.py
--rw-r--r--   0        0        0      117 2023-06-16 12:50:48.680563 plottah-0.1.0/plottah/plots/__init__.py
--rw-r--r--   0        0        0     4050 2023-06-16 12:25:45.788578 plottah-0.1.0/plottah/utils.py
--rw-r--r--   0        0        0      506 2023-06-22 12:43:26.480856 plottah-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 plottah-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      780 2023-06-22 12:45:01.689438 plottah-0.1.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-22 11:30:53.499061 plottah-0.1.1/plottah/__init__.py
+-rw-r--r--   0        0        0     1012 2023-06-22 12:44:11.607614 plottah-0.1.1/plottah/__main__.py
+-rw-r--r--   0        0        0     1339 2023-06-19 19:34:19.357898 plottah-0.1.1/plottah/colors.py
+-rw-r--r--   0        0        0     3056 2023-06-22 09:19:12.089888 plottah-0.1.1/plottah/config.py
+-rw-r--r--   0        0        0      988 2023-06-22 09:55:14.056657 plottah-0.1.1/plottah/main.py
+-rw-r--r--   0        0        0       24 2023-06-20 17:12:04.651705 plottah-0.1.1/plottah/plot_builder/__init__.py
+-rw-r--r--   0        0        0     2720 2023-06-22 12:44:18.230172 plottah-0.1.1/plottah/plot_builder/builders.py
+-rw-r--r--   0        0        0     7488 2023-06-22 12:44:18.976051 plottah-0.1.1/plottah/plot_handler/PlotHandler.py
+-rw-r--r--   0        0        0       37 2023-06-20 17:27:02.673177 plottah-0.1.1/plottah/plot_handler/__init__.py
+-rw-r--r--   0        0        0     7530 2023-06-22 12:44:22.633547 plottah-0.1.1/plottah/plots/BinEventRatePlot.py
+-rw-r--r--   0        0        0     3987 2023-06-22 12:44:23.133501 plottah-0.1.1/plottah/plots/DistPlot.py
+-rw-r--r--   0        0        0     1927 2023-06-22 07:41:05.603043 plottah-0.1.1/plottah/plots/PlotProtocol.py
+-rw-r--r--   0        0        0     3578 2023-06-22 12:44:24.105798 plottah-0.1.1/plottah/plots/RocCurvePlot.py
+-rw-r--r--   0        0        0      117 2023-06-16 12:50:48.680563 plottah-0.1.1/plottah/plots/__init__.py
+-rw-r--r--   0        0        0     4050 2023-06-16 12:25:45.788578 plottah-0.1.1/plottah/utils.py
+-rw-r--r--   0        0        0      506 2023-06-22 12:46:19.964832 plottah-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1570 1970-01-01 00:00:00.000000 plottah-0.1.1/PKG-INFO
```

### Comparing `plottah-0.1.0/README.md` & `plottah-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-# Ota-Template
-
 *Copyright © 2023 by Boston Consulting Group. All rights reserved*
-# SmartBanking PLotting tool
+# SmartBanking Plotting tool
 
 ## Setup
 
 ### Requirements
 
 * Python (>=3.6)
```

### Comparing `plottah-0.1.0/plottah/__main__.py` & `plottah-0.1.1/plottah/__main__.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/colors.py` & `plottah-0.1.1/plottah/colors.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/config.py` & `plottah-0.1.1/plottah/config.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/main.py` & `plottah-0.1.1/plottah/main.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/plot_builder/builders.py` & `plottah-0.1.1/plottah/plot_builder/builders.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/plot_handler/PlotHandler.py` & `plottah-0.1.1/plottah/plot_handler/PlotHandler.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/plots/BinEventRatePlot.py` & `plottah-0.1.1/plottah/plots/BinEventRatePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/plots/DistPlot.py` & `plottah-0.1.1/plottah/plots/DistPlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/plots/PlotProtocol.py` & `plottah-0.1.1/plottah/plots/PlotProtocol.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/plots/RocCurvePlot.py` & `plottah-0.1.1/plottah/plots/RocCurvePlot.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/plottah/utils.py` & `plottah-0.1.1/plottah/utils.py`

 * *Files identical despite different names*

### Comparing `plottah-0.1.0/PKG-INFO` & `plottah-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plottah
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Niels Ota
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jupyter (>=1.0.0,<2.0.0)
@@ -17,18 +17,16 @@
 Requires-Dist: pytest (>=7.3.2,<8.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Description-Content-Type: text/markdown
 
-# Ota-Template
-
 *Copyright © 2023 by Boston Consulting Group. All rights reserved*
-# SmartBanking PLotting tool
+# SmartBanking Plotting tool
 
 ## Setup
 
 ### Requirements
 
 * Python (>=3.6)
```

