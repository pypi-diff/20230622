# Comparing `tmp/icarus-bt-0.2.0.tar.gz` & `tmp/icarus-bt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icarus-bt-0.2.0.tar", last modified: Wed Jun 21 03:20:23 2023, max compression
+gzip compressed data, was "icarus-bt-0.2.1.tar", last modified: Thu Jun 22 19:39:09 2023, max compression
```

## Comparing `icarus-bt-0.2.0.tar` & `icarus-bt-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-21 03:20:23.538280 icarus-bt-0.2.0/
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-21 03:20:23.533341 icarus-bt-0.2.0/Icarus/
--rw-r--r--   0 devinthakker   (501) staff       (20)      184 2023-06-21 01:14:49.000000 icarus-bt-0.2.0/Icarus/__init__.py
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-21 03:20:23.533715 icarus-bt-0.2.0/Icarus/graphs/
--rw-r--r--   0 devinthakker   (501) staff       (20)       21 2023-06-21 00:21:04.000000 icarus-bt-0.2.0/Icarus/graphs/__init__.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     4932 2023-06-16 01:38:17.000000 icarus-bt-0.2.0/Icarus/graphs/graph.py
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-21 03:20:23.536035 icarus-bt-0.2.0/Icarus/indicators/
--rw-r--r--   0 devinthakker   (501) staff       (20)     5989 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/ADX.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3360 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/ATR.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2849 2023-06-19 03:45:16.000000 icarus-bt-0.2.0/Icarus/indicators/BOLLINGERBANDS.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3461 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/CCI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2752 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/EMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3194 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/MACD.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      998 2023-05-23 22:21:13.000000 icarus-bt-0.2.0/Icarus/indicators/OHLCV.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3030 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/RSI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2271 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/SMA.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     4217 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/STOCHOSCILLATOR.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3630 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/STOCHRSI.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     3454 2023-06-16 20:06:49.000000 icarus-bt-0.2.0/Icarus/indicators/VWAP.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      293 2023-06-16 20:09:40.000000 icarus-bt-0.2.0/Icarus/indicators/__init__.py
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-21 03:20:23.537245 icarus-bt-0.2.0/Icarus/metrics/
--rw-r--r--   0 devinthakker   (501) staff       (20)      898 2023-06-14 04:24:52.000000 icarus-bt-0.2.0/Icarus/metrics/__init__.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      564 2023-06-14 04:30:21.000000 icarus-bt-0.2.0/Icarus/metrics/annualizedreturns.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1600 2023-06-14 04:30:57.000000 icarus-bt-0.2.0/Icarus/metrics/calmar.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      655 2023-06-14 04:31:12.000000 icarus-bt-0.2.0/Icarus/metrics/maxdrawdown.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      883 2023-06-14 04:32:13.000000 icarus-bt-0.2.0/Icarus/metrics/sharperatio.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1254 2023-06-14 04:32:26.000000 icarus-bt-0.2.0/Icarus/metrics/sortinoratio.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      562 2023-06-14 04:32:45.000000 icarus-bt-0.2.0/Icarus/metrics/totalreturn.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      561 2023-06-21 01:19:08.000000 icarus-bt-0.2.0/Icarus/optimize.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     8694 2023-06-21 01:15:47.000000 icarus-bt-0.2.0/Icarus/riley.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     5739 2023-06-21 01:01:17.000000 icarus-bt-0.2.0/Icarus/runners.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     2857 2023-06-15 02:23:49.000000 icarus-bt-0.2.0/Icarus/source.py
--rw-r--r--   0 devinthakker   (501) staff       (20)      328 2023-06-15 02:24:00.000000 icarus-bt-0.2.0/Icarus/strategy.py
--rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-06-14 03:09:25.000000 icarus-bt-0.2.0/LICENSE
--rw-r--r--   0 devinthakker   (501) staff       (20)     7499 2023-06-21 03:20:23.538389 icarus-bt-0.2.0/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)     6132 2023-06-21 03:03:39.000000 icarus-bt-0.2.0/README.md
-drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-21 03:20:23.538121 icarus-bt-0.2.0/icarus_bt.egg-info/
--rw-r--r--   0 devinthakker   (501) staff       (20)     7499 2023-06-21 03:20:23.000000 icarus-bt-0.2.0/icarus_bt.egg-info/PKG-INFO
--rw-r--r--   0 devinthakker   (501) staff       (20)      928 2023-06-21 03:20:23.000000 icarus-bt-0.2.0/icarus_bt.egg-info/SOURCES.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-06-21 03:20:23.000000 icarus-bt-0.2.0/icarus_bt.egg-info/dependency_links.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)      861 2023-06-21 03:20:23.000000 icarus-bt-0.2.0/icarus_bt.egg-info/requires.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)        7 2023-06-21 03:20:23.000000 icarus-bt-0.2.0/icarus_bt.egg-info/top_level.txt
--rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-06-21 03:20:23.538776 icarus-bt-0.2.0/setup.cfg
--rw-r--r--   0 devinthakker   (501) staff       (20)     1842 2023-06-21 03:17:40.000000 icarus-bt-0.2.0/setup.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-22 19:39:09.873914 icarus-bt-0.2.1/
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-22 19:39:09.869079 icarus-bt-0.2.1/Icarus/
+-rw-r--r--   0 devinthakker   (501) staff       (20)      184 2023-06-21 01:14:49.000000 icarus-bt-0.2.1/Icarus/__init__.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-22 19:39:09.869453 icarus-bt-0.2.1/Icarus/graphs/
+-rw-r--r--   0 devinthakker   (501) staff       (20)       21 2023-06-21 00:21:04.000000 icarus-bt-0.2.1/Icarus/graphs/__init__.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     4932 2023-06-16 01:38:17.000000 icarus-bt-0.2.1/Icarus/graphs/graph.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-22 19:39:09.871648 icarus-bt-0.2.1/Icarus/indicators/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     5989 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/ADX.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3360 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/ATR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2849 2023-06-19 03:45:16.000000 icarus-bt-0.2.1/Icarus/indicators/BOLLINGERBANDS.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3461 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/CCI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2752 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/EMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3194 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/MACD.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      998 2023-05-23 22:21:13.000000 icarus-bt-0.2.1/Icarus/indicators/OHLCV.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3030 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/RSI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2271 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/SMA.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     4217 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/STOCHOSCILLATOR.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3630 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/STOCHRSI.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     3454 2023-06-16 20:06:49.000000 icarus-bt-0.2.1/Icarus/indicators/VWAP.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      293 2023-06-16 20:09:40.000000 icarus-bt-0.2.1/Icarus/indicators/__init__.py
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-22 19:39:09.872832 icarus-bt-0.2.1/Icarus/metrics/
+-rw-r--r--   0 devinthakker   (501) staff       (20)      898 2023-06-14 04:24:52.000000 icarus-bt-0.2.1/Icarus/metrics/__init__.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      564 2023-06-14 04:30:21.000000 icarus-bt-0.2.1/Icarus/metrics/annualizedreturns.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1600 2023-06-14 04:30:57.000000 icarus-bt-0.2.1/Icarus/metrics/calmar.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      655 2023-06-14 04:31:12.000000 icarus-bt-0.2.1/Icarus/metrics/maxdrawdown.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      883 2023-06-14 04:32:13.000000 icarus-bt-0.2.1/Icarus/metrics/sharperatio.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1254 2023-06-14 04:32:26.000000 icarus-bt-0.2.1/Icarus/metrics/sortinoratio.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      562 2023-06-14 04:32:45.000000 icarus-bt-0.2.1/Icarus/metrics/totalreturn.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      561 2023-06-21 01:19:08.000000 icarus-bt-0.2.1/Icarus/optimize.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     8694 2023-06-21 01:15:47.000000 icarus-bt-0.2.1/Icarus/riley.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     5739 2023-06-21 01:01:17.000000 icarus-bt-0.2.1/Icarus/runners.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     2857 2023-06-15 02:23:49.000000 icarus-bt-0.2.1/Icarus/source.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)      328 2023-06-15 02:24:00.000000 icarus-bt-0.2.1/Icarus/strategy.py
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1069 2023-06-14 03:09:25.000000 icarus-bt-0.2.1/LICENSE
+-rw-r--r--   0 devinthakker   (501) staff       (20)       24 2023-06-22 18:37:46.000000 icarus-bt-0.2.1/MANIFEST.in
+-rw-r--r--   0 devinthakker   (501) staff       (20)     7502 2023-06-22 19:39:09.874013 icarus-bt-0.2.1/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)     6133 2023-06-22 18:13:22.000000 icarus-bt-0.2.1/README.md
+drwxr-xr-x   0 devinthakker   (501) staff       (20)        0 2023-06-22 19:39:09.873738 icarus-bt-0.2.1/icarus_bt.egg-info/
+-rw-r--r--   0 devinthakker   (501) staff       (20)     7502 2023-06-22 19:39:09.000000 icarus-bt-0.2.1/icarus_bt.egg-info/PKG-INFO
+-rw-r--r--   0 devinthakker   (501) staff       (20)      957 2023-06-22 19:39:09.000000 icarus-bt-0.2.1/icarus_bt.egg-info/SOURCES.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        1 2023-06-22 19:39:09.000000 icarus-bt-0.2.1/icarus_bt.egg-info/dependency_links.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       49 2023-06-22 19:39:09.000000 icarus-bt-0.2.1/icarus_bt.egg-info/requires.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)        7 2023-06-22 19:39:09.000000 icarus-bt-0.2.1/icarus_bt.egg-info/top_level.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)      861 2023-06-21 03:04:22.000000 icarus-bt-0.2.1/requirements.txt
+-rw-r--r--   0 devinthakker   (501) staff       (20)       79 2023-06-22 19:39:09.874386 icarus-bt-0.2.1/setup.cfg
+-rw-r--r--   0 devinthakker   (501) staff       (20)     1862 2023-06-22 19:38:06.000000 icarus-bt-0.2.1/setup.py
```

### Comparing `icarus-bt-0.2.0/Icarus/graphs/graph.py` & `icarus-bt-0.2.1/Icarus/graphs/graph.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/ADX.py` & `icarus-bt-0.2.1/Icarus/indicators/ADX.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/ATR.py` & `icarus-bt-0.2.1/Icarus/indicators/ATR.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/BOLLINGERBANDS.py` & `icarus-bt-0.2.1/Icarus/indicators/BOLLINGERBANDS.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/CCI.py` & `icarus-bt-0.2.1/Icarus/indicators/CCI.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/EMA.py` & `icarus-bt-0.2.1/Icarus/indicators/EMA.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/MACD.py` & `icarus-bt-0.2.1/Icarus/indicators/MACD.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/OHLCV.py` & `icarus-bt-0.2.1/Icarus/indicators/OHLCV.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/RSI.py` & `icarus-bt-0.2.1/Icarus/indicators/RSI.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/SMA.py` & `icarus-bt-0.2.1/Icarus/indicators/SMA.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/STOCHOSCILLATOR.py` & `icarus-bt-0.2.1/Icarus/indicators/STOCHOSCILLATOR.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/STOCHRSI.py` & `icarus-bt-0.2.1/Icarus/indicators/STOCHRSI.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/indicators/VWAP.py` & `icarus-bt-0.2.1/Icarus/indicators/VWAP.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/metrics/__init__.py` & `icarus-bt-0.2.1/Icarus/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/metrics/annualizedreturns.py` & `icarus-bt-0.2.1/Icarus/metrics/annualizedreturns.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/metrics/calmar.py` & `icarus-bt-0.2.1/Icarus/metrics/calmar.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/metrics/maxdrawdown.py` & `icarus-bt-0.2.1/Icarus/metrics/maxdrawdown.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/metrics/sharperatio.py` & `icarus-bt-0.2.1/Icarus/metrics/sharperatio.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/metrics/sortinoratio.py` & `icarus-bt-0.2.1/Icarus/metrics/sortinoratio.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/metrics/totalreturn.py` & `icarus-bt-0.2.1/Icarus/metrics/totalreturn.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/optimize.py` & `icarus-bt-0.2.1/Icarus/optimize.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/riley.py` & `icarus-bt-0.2.1/Icarus/riley.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/runners.py` & `icarus-bt-0.2.1/Icarus/runners.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/Icarus/source.py` & `icarus-bt-0.2.1/Icarus/source.py`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/LICENSE` & `icarus-bt-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/PKG-INFO` & `icarus-bt-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: icarus-bt
-Version: 0.2.0
+Version: 0.2.1
 Summary: A backtesting framework for algorithmic trading
 Home-page: https://github.com/devthaakker/icarus-bt
-Download-URL: https://github.com/devthakker/Icarus-bt/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/devthakker/Icarus-bt/archive/refs/tags/v0.2.1.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: backtesting,trading,algorithmic trading,finance,stock market,stock,market,backtest,backtesting framework,backtesting library,backtesting tool,backtesting software,backtesting python,backtesting python library,backtesting python framework,backtesting python tool,backtesting python software,backtesting python library finance,backtesting python framework finance,backtesting python tool finance,backtesting python software finance,backtesting python library stock market,backtesting python framework stock market,backtesting python tool stock market,backtesting python software stock market
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # ICARUS-BT
 
 ![ICARUS-BT](./preview.jpg?raw=true)
 
 # Riley: Backtesting Engine for Trading Strategies
 
-[![Python](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/downloads/release/python-370/)
+[![Python](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/release/python-310/)
 [![PyPI](https://img.shields.io/pypi/v/icarus-bt?color=blue)](https://pypi.org/project/icarus-bt/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/icarus-bt?color=blue)](https://img.shields.io/github/downloads/devthakker/icarus-bt/total.svg)
 ![GitHub](https://img.shields.io/pypi/l/icarus-bt?color=blue)
 
 ## Overview
 Icarus is a Python package designed to facilitate the backtesting of trading strategies. It provides a framework to simulate and evaluate trading decisions based on historical data, calculate various performance metrics, and generate graphical representations of the results. Riley is equipped with features to compute metrics like Sharpe ratio and Sortino ratio, allowing traders and quantitative analysts to assess the risk-adjusted returns of their strategies.
```

### Comparing `icarus-bt-0.2.0/README.md` & `icarus-bt-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # ICARUS-BT
 
 ![ICARUS-BT](./preview.jpg?raw=true)
 
 # Riley: Backtesting Engine for Trading Strategies
 
-[![Python](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/downloads/release/python-370/)
+[![Python](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/release/python-310/)
 [![PyPI](https://img.shields.io/pypi/v/icarus-bt?color=blue)](https://pypi.org/project/icarus-bt/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/icarus-bt?color=blue)](https://img.shields.io/github/downloads/devthakker/icarus-bt/total.svg)
 ![GitHub](https://img.shields.io/pypi/l/icarus-bt?color=blue)
 
 ## Overview
 Icarus is a Python package designed to facilitate the backtesting of trading strategies. It provides a framework to simulate and evaluate trading decisions based on historical data, calculate various performance metrics, and generate graphical representations of the results. Riley is equipped with features to compute metrics like Sharpe ratio and Sortino ratio, allowing traders and quantitative analysts to assess the risk-adjusted returns of their strategies.
```

### Comparing `icarus-bt-0.2.0/icarus_bt.egg-info/PKG-INFO` & `icarus-bt-0.2.1/icarus_bt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: icarus-bt
-Version: 0.2.0
+Version: 0.2.1
 Summary: A backtesting framework for algorithmic trading
 Home-page: https://github.com/devthaakker/icarus-bt
-Download-URL: https://github.com/devthakker/Icarus-bt/archive/refs/tags/v0.2.0.tar.gz
+Download-URL: https://github.com/devthakker/Icarus-bt/archive/refs/tags/v0.2.1.tar.gz
 Author: Devin Thakker
 Author-email: devin.thakker@outlook.com
 License: MIT
 Keywords: backtesting,trading,algorithmic trading,finance,stock market,stock,market,backtest,backtesting framework,backtesting library,backtesting tool,backtesting software,backtesting python,backtesting python library,backtesting python framework,backtesting python tool,backtesting python software,backtesting python library finance,backtesting python framework finance,backtesting python tool finance,backtesting python software finance,backtesting python library stock market,backtesting python framework stock market,backtesting python tool stock market,backtesting python software stock market
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # ICARUS-BT
 
 ![ICARUS-BT](./preview.jpg?raw=true)
 
 # Riley: Backtesting Engine for Trading Strategies
 
-[![Python](https://img.shields.io/badge/python-3.7%2B-blue)](https://www.python.org/downloads/release/python-370/)
+[![Python](https://img.shields.io/badge/python-3.10%2B-blue)](https://www.python.org/downloads/release/python-310/)
 [![PyPI](https://img.shields.io/pypi/v/icarus-bt?color=blue)](https://pypi.org/project/icarus-bt/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/icarus-bt?color=blue)](https://img.shields.io/github/downloads/devthakker/icarus-bt/total.svg)
 ![GitHub](https://img.shields.io/pypi/l/icarus-bt?color=blue)
 
 ## Overview
 Icarus is a Python package designed to facilitate the backtesting of trading strategies. It provides a framework to simulate and evaluate trading decisions based on historical data, calculate various performance metrics, and generate graphical representations of the results. Riley is equipped with features to compute metrics like Sharpe ratio and Sortino ratio, allowing traders and quantitative analysts to assess the risk-adjusted returns of their strategies.
```

### Comparing `icarus-bt-0.2.0/icarus_bt.egg-info/SOURCES.txt` & `icarus-bt-0.2.1/icarus_bt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 LICENSE
+MANIFEST.in
 README.md
+requirements.txt
 setup.cfg
 setup.py
 Icarus/__init__.py
 Icarus/optimize.py
 Icarus/riley.py
 Icarus/runners.py
 Icarus/source.py
```

### Comparing `icarus-bt-0.2.0/icarus_bt.egg-info/requires.txt` & `icarus-bt-0.2.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `icarus-bt-0.2.0/setup.py` & `icarus-bt-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='icarus-bt',
-    version='0.2.0',
+    version='0.2.1',
     description='A backtesting framework for algorithmic trading',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires=[n for n in open('requirements.txt').readlines()],
+    install_requires=['numpy', 'matplotlib', 'yfinance', 'pandas', 'tqdm', 'mplfinance'],
     author='Devin Thakker',
     author_email='devin.thakker@outlook.com',
     url='https://github.com/devthaakker/icarus-bt',
     license='MIT',
-    download_url='https://github.com/devthakker/Icarus-bt/archive/refs/tags/v0.2.0.tar.gz',
+    download_url='https://github.com/devthakker/Icarus-bt/archive/refs/tags/v0.2.1.tar.gz',
     keywords=['backtesting', 'trading', 'algorithmic trading', 'finance', 'stock market', 'stock', 'market', 'backtest', 'backtesting framework', 'backtesting library', 'backtesting tool', 'backtesting software', 'backtesting python', 'backtesting python library', 'backtesting python framework', 'backtesting python tool', 'backtesting python software', 'backtesting python library finance', 'backtesting python framework finance', 'backtesting python tool finance', 'backtesting python software finance', 'backtesting python library stock market', 'backtesting python framework stock market', 'backtesting python tool stock market', 'backtesting python software stock market'],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Office/Business :: Financial :: Investment',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Utilities'
     ],
-    python_requires='>=3.7'
+    python_requires='>=3.10'
 )
```

