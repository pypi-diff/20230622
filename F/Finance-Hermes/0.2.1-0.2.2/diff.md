# Comparing `tmp/Finance-Hermes-0.2.1.tar.gz` & `tmp/Finance-Hermes-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Hermes-0.2.1.tar", last modified: Mon Dec  5 09:10:18 2022, max compression
+gzip compressed data, was "dist/Finance-Hermes-0.2.2.tar", last modified: Thu Jun 22 00:39:44 2023, max compression
```

## Comparing `Finance-Hermes-0.2.1.tar` & `Finance-Hermes-0.2.2.tar`

### file list

```diff
@@ -1,65 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/
--rw-r--r--   0 root         (0) root         (0)      222 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1703 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       70 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-12-05 09:10:17.000000 Finance-Hermes-0.2.1/Finance_Hermes.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      114 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      222 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/Izador/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/Izador/__init__.py
--rw-r--r--   0 root         (0) root         (0)      657 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/Izador/calculater.py
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-05 09:09:49.000000 Finance-Hermes-0.2.1/hermes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7484 2022-12-03 08:36:51.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/alpha101.py
--rw-r--r--   0 root         (0) root         (0)    15211 2022-12-03 07:41:04.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/core/alpha191.py
--rw-r--r--   0 root         (0) root         (0)     7523 2022-12-03 08:19:08.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/factor_alpha101.py
--rw-r--r--   0 root         (0) root         (0)    13226 2022-12-03 07:37:08.000000 Finance-Hermes-0.2.1/hermes/factors/alphax/factor_alpha191.py
--rw-r--r--   0 root         (0) root         (0)     1744 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/factors/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-10 07:28:19.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-13 12:40:33.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1673 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/core/basis.py
--rw-r--r--   0 root         (0) root         (0)     2241 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/fundamentals/factor_basis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/macroeconmic/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-10 07:28:19.000000 Finance-Hermes-0.2.1/hermes/factors/macroeconmic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/technical/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-10 07:28:19.000000 Finance-Hermes-0.2.1/hermes/factors/technical/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4925 2022-11-13 12:40:33.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/maturity.py
--rw-r--r--   0 root         (0) root         (0)    36381 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/momentum.py
--rw-r--r--   0 root         (0) root         (0)    14993 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/overlap.py
--rw-r--r--   0 root         (0) root         (0)     5954 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/statistics.py
--rw-r--r--   0 root         (0) root         (0)    16208 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/trend.py
--rw-r--r--   0 root         (0) root         (0)     5106 2022-11-06 15:36:30.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/utilities.py
--rw-r--r--   0 root         (0) root         (0)    16264 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/volatility.py
--rw-r--r--   0 root         (0) root         (0)    15946 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/core/volume.py
--rw-r--r--   0 root         (0) root         (0)     4608 2022-11-13 12:40:33.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_maturity.py
--rw-r--r--   0 root         (0) root         (0)    26641 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_momentum.py
--rw-r--r--   0 root         (0) root         (0)     9240 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_overlap.py
--rw-r--r--   0 root         (0) root         (0)     3907 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_statistics.py
--rw-r--r--   0 root         (0) root         (0)     6867 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_trend.py
--rw-r--r--   0 root         (0) root         (0)    11005 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_volatility.py
--rw-r--r--   0 root         (0) root         (0)    12352 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/factors/technical/factor_volume.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/kdutils/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/kdutils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2338 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/kdutils/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/fixes.py
--rw-r--r--   0 root         (0) root         (0)     7825 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.1/hermes/kdutils/core/helper.py
--rw-r--r--   0 root         (0) root         (0)     1578 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.1/hermes/kdutils/lazy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/requirements/
--rw-r--r--   0 root         (0) root         (0)       69 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/requirements/py3.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-05 09:10:18.000000 Finance-Hermes-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1964 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/Finance_Hermes.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/Finance_Hermes.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/Finance_Hermes.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/Finance_Hermes.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/Finance_Hermes.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/Finance_Hermes.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-01 07:48:09.000000 Finance-Hermes-0.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      327 2023-06-22 00:38:52.000000 Finance-Hermes-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      233 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      195 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/hermes/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-22 00:13:26.000000 Finance-Hermes-0.2.2/hermes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/hermes/factors/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.2/hermes/factors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-06-21 22:52:56.000000 Finance-Hermes-0.2.2/hermes/factors/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/hermes/kdutils/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.2/hermes/kdutils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.2/hermes/kdutils/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/hermes/kdutils/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.2/hermes/kdutils/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.2/hermes/kdutils/core/fixes.py
+-rw-r--r--   0 root         (0) root         (0)     7825 2022-11-11 12:13:52.000000 Finance-Hermes-0.2.2/hermes/kdutils/core/helper.py
+-rw-r--r--   0 root         (0) root         (0)      870 2023-06-21 21:57:15.000000 Finance-Hermes-0.2.2/hermes/kdutils/create_id.py
+-rw-r--r--   0 root         (0) root         (0)     1578 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.2/hermes/kdutils/lazy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/hermes/lzador/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.2/hermes/lzador/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      657 2022-11-06 15:36:04.000000 Finance-Hermes-0.2.2/hermes/lzador/calculater.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/requirements/
+-rw-r--r--   0 root         (0) root         (0)       69 2022-11-20 16:24:38.000000 Finance-Hermes-0.2.2/requirements/py3.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 00:39:44.000000 Finance-Hermes-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1964 2023-06-22 00:28:55.000000 Finance-Hermes-0.2.2/setup.py
```

### Comparing `Finance-Hermes-0.2.1/hermes/Izador/calculater.py` & `Finance-Hermes-0.2.2/hermes/lzador/calculater.py`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/base.py` & `Finance-Hermes-0.2.2/hermes/kdutils/base.py`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/core/fixes.py` & `Finance-Hermes-0.2.2/hermes/kdutils/core/fixes.py`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/core/helper.py` & `Finance-Hermes-0.2.2/hermes/kdutils/core/helper.py`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/hermes/kdutils/lazy.py` & `Finance-Hermes-0.2.2/hermes/kdutils/lazy.py`

 * *Files identical despite different names*

### Comparing `Finance-Hermes-0.2.1/setup.py` & `Finance-Hermes-0.2.2/setup.py`

 * *Files identical despite different names*

