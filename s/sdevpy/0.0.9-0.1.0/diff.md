# Comparing `tmp/sdevpy-0.0.9.tar.gz` & `tmp/sdevpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevpy-0.0.9.tar", last modified: Sun Jun 18 08:28:58 2023, max compression
+gzip compressed data, was "sdevpy-0.1.0.tar", last modified: Thu Jun 22 00:50:49 2023, max compression
```

## Comparing `sdevpy-0.0.9.tar` & `sdevpy-0.1.0.tar`

### file list

```diff
@@ -1,68 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.105496 sdevpy-0.0.9/
--rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.0.9/LICENSE
--rw-rw-rw-   0        0        0     1725 2023-06-18 08:28:58.104497 sdevpy-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.0.9/README.md
--rw-rw-rw-   0        0        0      643 2023-06-18 08:25:52.000000 sdevpy-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 08:28:58.105496 sdevpy-0.0.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:57.942550 sdevpy-0.0.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:57.956544 sdevpy-0.0.9/src/sdevpy/
--rw-rw-rw-   0        0        0       21 2023-06-18 08:28:32.000000 sdevpy-0.0.9/src/sdevpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.030521 sdevpy-0.0.9/src/sdevpy/analytics/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.9/src/sdevpy/analytics/__init__.py
--rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.0.9/src/sdevpy/analytics/bachelier.py
--rw-rw-rw-   0        0        0     2838 2023-05-06 08:46:10.000000 sdevpy-0.0.9/src/sdevpy/analytics/black.py
--rw-rw-rw-   0        0        0     6244 2023-05-30 05:18:38.000000 sdevpy-0.0.9/src/sdevpy/analytics/fbsabr.py
--rw-rw-rw-   0        0        0     6791 2023-06-04 08:07:50.000000 sdevpy-0.0.9/src/sdevpy/analytics/mcheston.py
--rw-rw-rw-   0        0        0     7636 2023-06-03 14:15:41.000000 sdevpy-0.0.9/src/sdevpy/analytics/mcsabr.py
--rw-rw-rw-   0        0        0     8413 2023-06-04 03:56:13.000000 sdevpy-0.0.9/src/sdevpy/analytics/mczabr.py
--rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.0.9/src/sdevpy/analytics/sabr.py
--rw-rw-rw-   0        0        0       45 2023-06-17 01:57:09.000000 sdevpy-0.0.9/src/sdevpy/example.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.043517 sdevpy-0.0.9/src/sdevpy/machinelearning/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/__init__.py
--rw-rw-rw-   0        0        0     4339 2023-05-01 03:27:12.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/callbacks.py
--rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/datasets.py
--rw-rw-rw-   0        0        0     6098 2023-06-10 07:48:52.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/learningmodel.py
--rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/learningschedules.py
--rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.0.9/src/sdevpy/machinelearning/topology.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.051514 sdevpy-0.0.9/src/sdevpy/maths/
--rw-rw-rw-   0        0        0        0 2023-06-17 01:56:05.000000 sdevpy-0.0.9/src/sdevpy/maths/__init__.py
--rw-rw-rw-   0        0        0      676 2023-04-16 02:45:25.000000 sdevpy-0.0.9/src/sdevpy/maths/interpolations.py
--rw-rw-rw-   0        0        0      415 2023-04-30 13:53:34.000000 sdevpy-0.0.9/src/sdevpy/maths/metrics.py
--rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.0.9/src/sdevpy/maths/optimization.py
--rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.0.9/src/sdevpy/maths/rand.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.052513 sdevpy-0.0.9/src/sdevpy/projects/
--rw-rw-rw-   0        0        0      888 2023-06-18 05:26:29.000000 sdevpy-0.0.9/src/sdevpy/projects/datafiles.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.064510 sdevpy-0.0.9/src/sdevpy/projects/pinns/
--rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.0.9/src/sdevpy/projects/pinns/ernst_pinns.py
--rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns.py
--rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns_worst_of.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.081505 sdevpy-0.0.9/src/sdevpy/projects/stovol/
--rw-rw-rw-   0        0        0     2508 2023-06-18 05:56:21.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolgen.py
--rw-rw-rw-   0        0        0     4907 2023-06-16 02:55:53.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolplot.py
--rw-rw-rw-   0        0        0     9986 2023-06-16 08:39:59.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/stovoltrain.py
--rw-rw-rw-   0        0        0    10465 2023-06-09 00:39:24.000000 sdevpy-0.0.9/src/sdevpy/projects/stovol/xsabrfit.py
--rw-rw-rw-   0        0        0      400 2023-04-09 03:41:51.000000 sdevpy-0.0.9/src/sdevpy/settings.py
--rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.0.9/src/sdevpy/test.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.091502 sdevpy-0.0.9/src/sdevpy/tools/
--rw-rw-rw-   0        0        0     1070 2023-05-06 02:22:05.000000 sdevpy-0.0.9/src/sdevpy/tools/clipboard.py
--rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.0.9/src/sdevpy/tools/constants.py
--rw-rw-rw-   0        0        0     1529 2023-05-28 10:08:05.000000 sdevpy-0.0.9/src/sdevpy/tools/filemanager.py
--rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.0.9/src/sdevpy/tools/jsonmanager.py
--rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.0.9/src/sdevpy/tools/timegrids.py
--rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.0.9/src/sdevpy/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.101498 sdevpy-0.0.9/src/sdevpy/volsurfacegen/
--rw-rw-rw-   0        0        0     2489 2023-06-16 06:09:33.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/fbsabrgenerator.py
--rw-rw-rw-   0        0        0     8576 2023-06-10 04:04:58.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/mchestongenerator.py
--rw-rw-rw-   0        0        0     9196 2023-06-16 12:59:49.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/mcsabrgenerator.py
--rw-rw-rw-   0        0        0     9119 2023-06-10 04:05:12.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/mczabrgenerator.py
--rw-rw-rw-   0        0        0    11493 2023-06-16 06:02:08.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/sabrgenerator.py
--rw-rw-rw-   0        0        0     4777 2023-06-16 01:47:35.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/smilegenerator.py
--rw-rw-rw-   0        0        0     2118 2023-06-18 08:25:27.000000 sdevpy-0.0.9/src/sdevpy/volsurfacegen/stovolfactory.py
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.003530 sdevpy-0.0.9/src/sdevpy.egg-info/
--rw-rw-rw-   0        0        0     1725 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1753 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 08:28:57.000000 sdevpy-0.0.9/src/sdevpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 08:28:58.103497 sdevpy-0.0.9/tests/
--rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.0.9/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.236625 sdevpy-0.1.0/
+-rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1725 2023-06-22 00:50:49.235625 sdevpy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.1.0/README.md
+-rw-rw-rw-   0        0        0      643 2023-06-22 00:44:59.000000 sdevpy-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 00:50:49.236625 sdevpy-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:48.877741 sdevpy-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:48.913730 sdevpy-0.1.0/src/sdevpy/
+-rw-rw-rw-   0        0        0       23 2023-06-19 11:53:52.000000 sdevpy-0.1.0/src/sdevpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:48.984707 sdevpy-0.1.0/src/sdevpy/analytics/
+-rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.1.0/src/sdevpy/analytics/bachelier.py
+-rw-rw-rw-   0        0        0     2810 2023-06-20 03:38:43.000000 sdevpy-0.1.0/src/sdevpy/analytics/black.py
+-rw-rw-rw-   0        0        0     6308 2023-06-20 03:41:05.000000 sdevpy-0.1.0/src/sdevpy/analytics/fbsabr.py
+-rw-rw-rw-   0        0        0     6911 2023-06-20 03:42:55.000000 sdevpy-0.1.0/src/sdevpy/analytics/mcheston.py
+-rw-rw-rw-   0        0        0     7657 2023-06-20 03:43:39.000000 sdevpy-0.1.0/src/sdevpy/analytics/mcsabr.py
+-rw-rw-rw-   0        0        0     8745 2023-06-20 03:49:45.000000 sdevpy-0.1.0/src/sdevpy/analytics/mczabr.py
+-rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.1.0/src/sdevpy/analytics/sabr.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.035692 sdevpy-0.1.0/src/sdevpy/machinelearning/
+-rw-rw-rw-   0        0        0     4350 2023-06-19 11:59:56.000000 sdevpy-0.1.0/src/sdevpy/machinelearning/callbacks.py
+-rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.1.0/src/sdevpy/machinelearning/datasets.py
+-rw-rw-rw-   0        0        0     6101 2023-06-20 09:15:35.000000 sdevpy-0.1.0/src/sdevpy/machinelearning/learningmodel.py
+-rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.1.0/src/sdevpy/machinelearning/learningschedules.py
+-rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.1.0/src/sdevpy/machinelearning/topology.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.051685 sdevpy-0.1.0/src/sdevpy/maths/
+-rw-rw-rw-   0        0        0      840 2023-06-20 06:44:09.000000 sdevpy-0.1.0/src/sdevpy/maths/interpolations.py
+-rw-rw-rw-   0        0        0      413 2023-06-20 08:24:06.000000 sdevpy-0.1.0/src/sdevpy/maths/metrics.py
+-rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.1.0/src/sdevpy/maths/optimization.py
+-rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.1.0/src/sdevpy/maths/rand.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.059682 sdevpy-0.1.0/src/sdevpy/projects/
+-rw-rw-rw-   0        0        0      893 2023-06-19 11:54:24.000000 sdevpy-0.1.0/src/sdevpy/projects/datafiles.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.092672 sdevpy-0.1.0/src/sdevpy/projects/pinns/
+-rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.1.0/src/sdevpy/projects/pinns/ernst_pinns.py
+-rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.1.0/src/sdevpy/projects/pinns/pinns.py
+-rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.1.0/src/sdevpy/projects/pinns/pinns_worst_of.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.123662 sdevpy-0.1.0/src/sdevpy/projects/stovol/
+-rw-rw-rw-   0        0        0     2513 2023-06-21 13:29:16.000000 sdevpy-0.1.0/src/sdevpy/projects/stovol/stovolgen.py
+-rw-rw-rw-   0        0        0     5033 2023-06-21 13:31:09.000000 sdevpy-0.1.0/src/sdevpy/projects/stovol/stovolplot.py
+-rw-rw-rw-   0        0        0    10181 2023-06-21 13:31:58.000000 sdevpy-0.1.0/src/sdevpy/projects/stovol/stovoltrain.py
+-rw-rw-rw-   0        0        0    10577 2023-06-21 13:33:49.000000 sdevpy-0.1.0/src/sdevpy/projects/stovol/xsabrfit.py
+-rw-rw-rw-   0        0        0      400 2023-06-19 11:47:07.000000 sdevpy-0.1.0/src/sdevpy/settings.py
+-rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.1.0/src/sdevpy/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.169647 sdevpy-0.1.0/src/sdevpy/tools/
+-rw-rw-rw-   0        0        0     1048 2023-06-20 09:17:04.000000 sdevpy-0.1.0/src/sdevpy/tools/clipboard.py
+-rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.1.0/src/sdevpy/tools/constants.py
+-rw-rw-rw-   0        0        0     1546 2023-06-20 09:18:04.000000 sdevpy-0.1.0/src/sdevpy/tools/filemanager.py
+-rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.1.0/src/sdevpy/tools/jsonmanager.py
+-rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.1.0/src/sdevpy/tools/timegrids.py
+-rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.1.0/src/sdevpy/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.232627 sdevpy-0.1.0/src/sdevpy/volsurfacegen/
+-rw-rw-rw-   0        0        0     2529 2023-06-21 13:34:01.000000 sdevpy-0.1.0/src/sdevpy/volsurfacegen/fbsabrgenerator.py
+-rw-rw-rw-   0        0        0     8773 2023-06-20 09:22:19.000000 sdevpy-0.1.0/src/sdevpy/volsurfacegen/mchestongenerator.py
+-rw-rw-rw-   0        0        0     9366 2023-06-21 13:33:57.000000 sdevpy-0.1.0/src/sdevpy/volsurfacegen/mcsabrgenerator.py
+-rw-rw-rw-   0        0        0     9324 2023-06-21 13:23:45.000000 sdevpy-0.1.0/src/sdevpy/volsurfacegen/mczabrgenerator.py
+-rw-rw-rw-   0        0        0    11547 2023-06-21 13:33:58.000000 sdevpy-0.1.0/src/sdevpy/volsurfacegen/sabrgenerator.py
+-rw-rw-rw-   0        0        0     4789 2023-06-21 13:33:59.000000 sdevpy-0.1.0/src/sdevpy/volsurfacegen/smilegenerator.py
+-rw-rw-rw-   0        0        0     2118 2023-06-21 13:34:03.000000 sdevpy-0.1.0/src/sdevpy/volsurfacegen/stovolfactory.py
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:48.938722 sdevpy-0.1.0/src/sdevpy.egg-info/
+-rw-rw-rw-   0        0        0     1725 2023-06-22 00:50:48.000000 sdevpy-0.1.0/src/sdevpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1630 2023-06-22 00:50:48.000000 sdevpy-0.1.0/src/sdevpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 00:50:48.000000 sdevpy-0.1.0/src/sdevpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-22 00:50:48.000000 sdevpy-0.1.0/src/sdevpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 00:50:48.000000 sdevpy-0.1.0/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 00:50:49.234626 sdevpy-0.1.0/tests/
+-rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.1.0/tests/test.py
```

### Comparing `sdevpy-0.0.9/LICENSE` & `sdevpy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/PKG-INFO` & `sdevpy-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.0.9/README.md` & `sdevpy-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/pyproject.toml` & `sdevpy-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdevpy"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Sebastien Gurrieri", email="sebgur@gmail.com" },
 ]
 description = "Python package for Machine Learning in Finance"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `sdevpy-0.0.9/src/sdevpy/analytics/bachelier.py` & `sdevpy-0.1.0/src/sdevpy/analytics/bachelier.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/analytics/black.py` & `sdevpy-0.1.0/src/sdevpy/analytics/black.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,9 +73,9 @@
     f_space = np.linspace(100, 120, NUM_POINTS)
     k_space = np.linspace(20, 2180, NUM_POINTS)
     prices = price(EXPIRY, k_space, IS_CALL, f_space, VOL)
     # print(prices)
     implied_vols = []
     for i, k in enumerate(k_space):
         implied_vols.append(implied_vol(EXPIRY, k, IS_CALL, f_space[i], prices[i]))
-                            
+
     # print(implied_vols)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/analytics/fbsabr.py` & `sdevpy-0.1.0/src/sdevpy/analytics/fbsabr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Monte-Carlo simulation for Free-Boundary SABR model (vanillas) """
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy.stats as sp
 # from analytics.sabr import calculate_alpha
-from tools.timegrids import SimpleTimeGridBuilder
-from tools import timer
+from sdevpy.tools.timegrids import SimpleTimeGridBuilder
+from sdevpy.tools import timer
 
 
 def price(expiries, strikes, are_calls, fwd, parameters, num_mc=10000, points_per_year=10,
           scheme='Andersen'):
     """ Calculate vanilla prices under Free-Boundary SABR model by Monte-Carlo simulation"""
     floor = 0.00001
 
@@ -147,22 +147,23 @@
                       scheme=SCHEME)
     mc_timer.stop()
     mc_timer.print()
 
     # print(MC_PRICES)
 
     # Convert to IV and compare against approximate closed-form
-    import black
+    # import black
     import bachelier
     mc_ivs = []
     for a, expiry in enumerate(EXPIRIES):
         mc_iv = []
         for j, sstrike in enumerate(SSTRIKES[a]):
             # mc_iv.append(black.implied_vol(expiry, sstrike, IS_CALL, SFWD, MC_PRICES[a, j]))
-            mc_iv.append(bachelier.implied_vol(expiry, STRIKES[a, j], IS_CALL, FWD, MC_PRICES[a, j]))
+            mc_iv.append(bachelier.implied_vol(expiry, STRIKES[a, j], IS_CALL, FWD,
+                                               MC_PRICES[a, j]))
         mc_ivs.append(mc_iv)
 
     plt.figure(figsize=(10, 8))
     plt.subplots_adjust(hspace=0.40)
     plt.subplot(2, 2, 1)
     plt.plot(XAXIS[0], mc_ivs[0], label='MC')
     plt.legend(loc='best')
```

### Comparing `sdevpy-0.0.9/src/sdevpy/analytics/mcheston.py` & `sdevpy-0.1.0/src/sdevpy/analytics/mcheston.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
     dS = sqrt(v) * S * dW
     dv = kappa * (theta - v) * dt + xi * sqrt(v) * dZ with <dW, dZ> = rho
     """
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy.stats as sp
 # from analytics.sabr import calculate_alpha
-from tools.timegrids import SimpleTimeGridBuilder
-from tools import timer
+from sdevpy.tools.timegrids import SimpleTimeGridBuilder
+from sdevpy.tools import timer
 
 
 def price(expiries, strikes, are_calls, fwd, parameters, num_mc=10000, points_per_year=10):
     """ Calculate vanilla prices under Heston model by Monte-Carlo simulation"""
     scale = fwd
     if scale < 0.0:
         raise ValueError("Negative forward")
@@ -97,14 +97,16 @@
             payoff_count += 1
 
     np.seterr(divide='warn')
 
     return np.asarray(mc_prices)
 
 def calculate_v0(lnvol):
+    """ Calculate approximated v0 parameter from lognormal vol (for order of magnitude
+        only)"""
     return lnvol**2
 
 
 if __name__ == "__main__":
     EXPIRIES = [0.5, 1.0, 5.0, 10.0]
     NSTRIKES = 50
     FWD = -0.005
```

### Comparing `sdevpy-0.0.9/src/sdevpy/analytics/mcsabr.py` & `sdevpy-0.1.0/src/sdevpy/analytics/mcsabr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ Monte-Carlo simulation for SABR models (vanillas) """
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy.stats as sp
-from analytics.sabr import calculate_alpha
-from tools.timegrids import SimpleTimeGridBuilder
-from tools import timer
+from sdevpy.analytics.sabr import calculate_alpha
+from sdevpy.tools.timegrids import SimpleTimeGridBuilder
+from sdevpy.tools import timer
 
 
 def price(expiries, strikes, are_calls, fwd, parameters, num_mc=10000, points_per_year=10,
           scheme='LogAndersen'):
     """ Calculate vanilla prices under SABR model by Monte-Carlo simulation"""
     scale = fwd
     if scale < 0.0:
```

### Comparing `sdevpy-0.0.9/src/sdevpy/analytics/mczabr.py` & `sdevpy-0.1.0/src/sdevpy/analytics/mczabr.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """ Monte-Carlo simulation for ZABR model (vanillas). The model is defined as
     dF = alpha x sigma x F^beta dW
     dsigma = nu x sigma^gamma dZ
     with sigma(0) = 1.0 and <dW, dZ> = rho. SABR is the gamma = 1 case. """
 import numpy as np
 import matplotlib.pyplot as plt
 import scipy.stats as sp
-import analytics.mcsabr as mcsabr
-from tools.timegrids import SimpleTimeGridBuilder
-from tools import timer
+from sdevpy.analytics import mcsabr
+from sdevpy.tools.timegrids import SimpleTimeGridBuilder
+from sdevpy.tools import timer
+from sdevpy.tools import clipboard
 
 
 def price(expiries, strikes, are_calls, fwd, parameters, num_mc=10000, points_per_year=10):
     """ Calculate vanilla prices under ZABR model by Monte-Carlo simulation"""
     scale = fwd
     if scale < 0.0:
         raise ValueError("Negative forward")
@@ -154,55 +155,61 @@
     MC_PRICES4 = price(EXPIRIES, SSTRIKES, ARE_CALLS, SFWD, PARAMS4, NUM_MC, POINTS_PER_YEAR)
     MC_PRICES5 = price(EXPIRIES, SSTRIKES, ARE_CALLS, SFWD, PARAMS5, NUM_MC, POINTS_PER_YEAR)
     mc_timer.stop()
     mc_timer.print()
 
     # Convert to IV and compare against approximate closed-form
     import black
-    import bachelier
+    # import bachelier
     mc_ivs1 = []
     mc_ivs2 = []
     mc_ivs3 = []
     mc_ivs4 = []
     mc_ivs5 = []
     sb_ivs = []
     for a, expiry in enumerate(EXPIRIES):
         mc_iv1 = []
         mc_iv2 = []
         mc_iv3 = []
         mc_iv4 = []
         mc_iv5 = []
         sb_iv = []
         for j, sstrike in enumerate(SSTRIKES[a]):
-            mc_iv1.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD, MC_PRICES1[a, j]))
-            mc_iv2.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD, MC_PRICES2[a, j]))
-            mc_iv3.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD, MC_PRICES3[a, j]))
-            mc_iv4.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD, MC_PRICES4[a, j]))
-            mc_iv5.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD, MC_PRICES5[a, j]))
-            sb_iv.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD, SB_PRICES[a, j]))
+            mc_iv1.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD,
+                                            MC_PRICES1[a, j]))
+            mc_iv2.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD,
+                                            MC_PRICES2[a, j]))
+            mc_iv3.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD,
+                                            MC_PRICES3[a, j]))
+            mc_iv4.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD,
+                                            MC_PRICES4[a, j]))
+            mc_iv5.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD,
+                                            MC_PRICES5[a, j]))
+            sb_iv.append(black.implied_vol(expiry, SSTRIKES[a, j], IS_CALL, SFWD,
+                                           SB_PRICES[a, j]))
         mc_ivs1.append(mc_iv1)
         mc_ivs2.append(mc_iv2)
         mc_ivs3.append(mc_iv3)
         mc_ivs4.append(mc_iv4)
         mc_ivs5.append(mc_iv5)
         sb_ivs.append(sb_iv)
 
     label1 = f'gam={PARAMS1["Gamma"]}'
     label2 = f'gam={PARAMS2["Gamma"]}'
     label3 = f'gam={PARAMS3["Gamma"]}'
     label4 = f'gam={PARAMS4["Gamma"]}'
     label5 = f'gam={PARAMS5["Gamma"]}'
 
-    xport = np.column_stack((STRIKES[0, :], sb_ivs[0], mc_ivs1[0], mc_ivs2[0], mc_ivs3[0], mc_ivs4[0],
-                             mc_ivs5[0]))
-    from tools import clipboard
+    xport = np.column_stack((STRIKES[0, :], sb_ivs[0], mc_ivs1[0], mc_ivs2[0], mc_ivs3[0],
+                             mc_ivs4[0], mc_ivs5[0]))
     clipboard.export2d(xport)
 
 
     def plot_zabr(idx):
+        """ Plot a slice of ZABR vols"""
         plt.subplot(2, 2, idx + 1)
         plt.plot(XAXIS[idx], mc_ivs1[idx], label=label1, color='blue')
         plt.plot(XAXIS[idx], mc_ivs2[idx], label=label2, color='red')
         plt.plot(XAXIS[idx], mc_ivs3[idx], label=label3, color='green')
         plt.plot(XAXIS[idx], mc_ivs4[idx], label=label4, color='purple')
         plt.plot(XAXIS[idx], mc_ivs5[idx], label=label5, color='cyan')
         plt.plot(XAXIS[idx], sb_ivs[idx], label="SABR", color='black')
```

### Comparing `sdevpy-0.0.9/src/sdevpy/analytics/sabr.py` & `sdevpy-0.1.0/src/sdevpy/analytics/sabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/machinelearning/callbacks.py` & `sdevpy-0.1.0/src/sdevpy/machinelearning/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Custom callbacks for Keras training """
-import numpy as np
+# import numpy as np
 import keras
 from sklearn.preprocessing import MinMaxScaler
-from maths.metrics import rmse
+# from sdevpy.maths.metrics import rmse
 
 
 class SDevPyCallback(keras.callbacks.Callback):
     """ SDevPy's base class for callbacks. Compared to Keras's base, it also keeps track of 
         the learning rate and displays it at each period """
     def __init__(self, epoch_sampling=1, optimizer=None):
         keras.callbacks.Callback.__init__(self)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/machinelearning/datasets.py` & `sdevpy-0.1.0/src/sdevpy/machinelearning/datasets.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/machinelearning/learningmodel.py` & `sdevpy-0.1.0/src/sdevpy/machinelearning/learningmodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Wrapper class for machine learning models, including scalers, and simplifying
     evaluation, history tracking, exporting to/importing from files, etc. """
 import os
 from sklearn.preprocessing import StandardScaler
 # from keras.models import load_model
 import tensorflow as tf
 import joblib
-from tools import jsonmanager
 import absl.logging
+from sdevpy.tools import jsonmanager
 
 class LearningModel:
     """ Wrapper class for machine learning models, including scalers, and simplifying
         evaluation, history tracking, exporting to/importing from files, etc. """
     def __init__(self, model, is_scaled=False,
                  x_scaler=StandardScaler(copy=True), y_scaler=StandardScaler(copy=True)):
         self.model = model
@@ -124,15 +124,15 @@
     """ Load learning model from files. Note that for now, we set compile=False when loading
         the keras model as we do not know how to save and load custom components such as
         the scheduler or the callback. To restart the training after loading the model from
         file, we would have to be able to properly save and load those custom components.
          
         One possibility could be to implement additional custom saving, recreate those components
         by hand, and then compile again. """
-    
+
     if os.path.exists(path) is False:
         raise RuntimeError("Model folder does not exist: " + path)
 
     keras_model = tf.keras.models.load_model(path, compile=compile_)
 
     x_scaler_file, y_scaler_file = scaler_files(path)
     if os.path.exists(x_scaler_file) and os.path.exists(y_scaler_file):
```

### Comparing `sdevpy-0.0.9/src/sdevpy/machinelearning/learningschedules.py` & `sdevpy-0.1.0/src/sdevpy/machinelearning/learningschedules.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/machinelearning/topology.py` & `sdevpy-0.1.0/src/sdevpy/machinelearning/topology.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/maths/interpolations.py` & `sdevpy-0.1.0/src/sdevpy/maths/interpolations.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+""" Various interpolations and parametric forms """
 import numpy as np
 from scipy.interpolate import CubicSpline
 import matplotlib.pyplot as plt
 
 
 def rebonato(v):
+    """ Parametric funtion in Rebonato's book, convenient to fit yield and volatility
+        curves """
     a0 = 0.5
     ainf = 2.0
     b = -0.01
     tau = 5.0
     return ainf + (b * v + a0 - ainf) * np.exp(-v / tau)
 
 
 if __name__ == "__main__":
-    n_points = 5
-    x = np.linspace(0.0, 4.0, num=n_points)
+    NUM_POINTS = 5
+    x = np.linspace(0.0, 4.0, num=NUM_POINTS)
     y = rebonato(x)
     spline = CubicSpline(x, y, bc_type='natural')
 
     k = np.linspace(-1.0, 5.0, num=10)
     func = rebonato(k)
     inter = spline(k)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/maths/rand.py` & `sdevpy-0.1.0/src/sdevpy/maths/rand.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/datafiles.py` & `sdevpy-0.1.0/src/sdevpy/projects/datafiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Operations on data files e.g. merging, etc. """
 import os
 import pandas as pd
 from sdevpy.tools import filemanager
-import sdevpy.settings
+from sdevpy import settings
 
 
 def merge_tsv(path, shuffle=False):
     """ Merge all .tsv files into one, assuming they all have the same structure """
     merged_file = os.path.join(path, "merged.tsv")
     if os.path.exists(merged_file):
         print("removing file: " + merged_file)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/pinns/ernst_pinns.py` & `sdevpy-0.1.0/src/sdevpy/projects/pinns/ernst_pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns.py` & `sdevpy-0.1.0/src/sdevpy/projects/pinns/pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/pinns/pinns_worst_of.py` & `sdevpy-0.1.0/src/sdevpy/projects/pinns/pinns_worst_of.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolgen.py` & `sdevpy-0.1.0/src/sdevpy/projects/stovol/stovolgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Generate training data for Stochastic Local Vol models. We implement the direct map here.
     Datasets of parameters (inputs) vs prices/implied vols (outputs) are generated to later train
     a network that learns the so-called 'direct' calculation, i.e. prices from parameter. """
 import os
 from sdevpy.volsurfacegen import stovolfactory
-import sdevpy.settings
+from sdevpy import settings
 from sdevpy.tools.filemanager import check_directory
 from sdevpy.tools.timer import Stopwatch
 
 
 # ################ Runtime configuration ##########################################################
 # MODEL_TYPE = "SABR"
 # MODEL_TYPE = "ShiftedSABR"
```

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/stovol/stovolplot.py` & `sdevpy-0.1.0/src/sdevpy/projects/stovol/stovolplot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Plot helpers for XSABR project """
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mtick
-from analytics import bachelier
-from analytics import black
+from sdevpy.analytics import bachelier
+from sdevpy.analytics import black
 
 
 def plot_transform_surface(expiries, strikes, are_calls, fwd, ref_prices, mod_prices, title_,
                            transform='ShiftedBlackScholes'):
     """ Calculate quantities to display for the surface and display them in charts. Transformed
         quantities available are: Price, ShiftedBlackScholes (3%) and Bachelier (normal vols). """
     # Transform prices
@@ -14,15 +14,15 @@
     mod_disp = transform_surface(expiries, strikes, are_calls, fwd, mod_prices, transform)
 
     # Display transformed prices
     num_charts = expiries.shape[0]
     num_cols = 2
     num_rows = int(num_charts / num_cols)
     # print("num_rows: " + str(num_rows))
-    ylabel = 'Price' if transform is 'Price' else 'Vol'
+    ylabel = 'Price' if transform == 'Price' else 'Vol'
 
     fig, axs = plt.subplots(num_rows, num_cols, layout="constrained")
     fig.suptitle(title_, size='x-large', weight='bold')
     fig.set_size_inches(12, 8)
     for i in range(num_rows):
         for j in range(num_cols):
             k = num_cols * i + j
@@ -38,38 +38,40 @@
     plt.show()
 
 
 def transform_surface(expiries, strikes, are_calls, fwd, prices, transform='ShiftedBlackScholes'):
     """ Tranform prices into: Price, ShiftedBlackScholes (3%) and Bachelier (normal vols). """
     # Transform prices
     trans_prices = []
-    if transform is 'Price':
+    if transform == 'Price':
         trans_prices = prices
-    elif transform is 'ShiftedBlackScholes':
+    elif transform == 'ShiftedBlackScholes':
         shift = 0.03
         sfwd = fwd + shift
         for i, expiry in enumerate(expiries):
             strikes_ = strikes[i]
             are_calls_ = are_calls[i]
             trans_prices_ = []
             for j, strike in enumerate(strikes_):
                 sstrike = strike + shift
-                trans_prices_.append(black.implied_vol(expiry, sstrike, are_calls_[j], sfwd, prices[i, j]))
+                trans_prices_.append(black.implied_vol(expiry, sstrike, are_calls_[j], sfwd,
+                                                       prices[i, j]))
             trans_prices.append(trans_prices_)
-    elif transform is 'Bachelier':
+    elif transform == 'Bachelier':
         for i, expiry in enumerate(expiries):
             strikes_ = strikes[i]
             are_calls_ = are_calls[i]
             trans_prices_ = []
             for j, strike in enumerate(strikes_):
-                trans_prices_.append(bachelier.implied_vol(expiry, strike, are_calls_[j], fwd, prices[i, j]))
+                trans_prices_.append(bachelier.implied_vol(expiry, strike, are_calls_[j], fwd,
+                                                           prices[i, j]))
             trans_prices.append(trans_prices_)
     else:
         raise ValueError("Unknown transform type: " + transform)
-    
+
     return trans_prices
 
 
 # def strike_ladder(expiry, spread_ladder, fwd, test_params, generator, model,
 #                   transform='ShiftedBlackScholes'):
 #     """ Plot volatilities along a ladder of strike spreads """
 #     is_call = generator.is_call
```

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/stovol/stovoltrain.py` & `sdevpy-0.1.0/src/sdevpy/projects/stovol/stovoltrain.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,51 +4,51 @@
     pre-trained state or trained from scratch. Pre-trained models can be loaded and training
     resumed. """
 import os
 from datetime import datetime
 import numpy as np
 import tensorflow as tf
 import matplotlib.pyplot as plt
-import settings
-from machinelearning.topology import compose_model
-from machinelearning.learningmodel import LearningModel, load_learning_model
-from machinelearning.learningschedules import FlooredExponentialDecay
-from machinelearning.callbacks import RefCallback
-from machinelearning.datasets import prepare_sets
-from tools.filemanager import check_directory
-from tools.timer import Stopwatch
-from tools import clipboard
-from maths.metrics import rmse, tf_rmse
-from volsurfacegen.stovolfactory import set_generator
-from projects.stovol import stovolplot as xplt
+from sdevpy import settings
+from sdevpy.machinelearning.topology import compose_model
+from sdevpy.machinelearning.learningmodel import LearningModel, load_learning_model
+from sdevpy.machinelearning.learningschedules import FlooredExponentialDecay
+from sdevpy.machinelearning.callbacks import RefCallback
+from sdevpy.machinelearning.datasets import prepare_sets
+from sdevpy.tools.filemanager import check_directory
+from sdevpy.tools.timer import Stopwatch
+from sdevpy.tools import clipboard
+from sdevpy.maths.metrics import rmse, tf_rmse
+from sdevpy.volsurfacegen.stovolfactory import set_generator
+from sdevpy.projects.stovol import stovolplot as xplt
 
-# Create generator that samples/prices from a trained model
 # Fine-train models
+# Use type in json to know which type to instantiate
 # Lazy instantiation from remote/name code
 # Store data in Kaggle
 
 # ################ Runtime configuration ##########################################################
 # MODEL_TYPE = "SABR"
-MODEL_TYPE = "ShiftedSABR"
+# MODEL_TYPE = "ShiftedSABR"
 # MODEL_TYPE = "McShiftedSABR"
-# MODEL_TYPE = "FbSABR"
+MODEL_TYPE = "FbSABR"
 # MODEL_TYPE = "McShiftedZABR"
 # MODEL_TYPE = "McShiftedHeston"
 USE_TRAINED = True
 TRAIN = False
 if USE_TRAINED is False and TRAIN is False:
     raise RuntimeError("When not using pre-trained models, a new model must be trained")
 
 TRAIN_PERCENT = 0.90 # Proportion of dataset used for training (rest used for test)
-EPOCHS = 400
+EPOCHS = 100
 BATCH_SIZE = 1000
 SHOW_VOL_CHARTS = True # Show smile section charts
 # For comparison to reference values (accuracy of reference)
-NUM_MC = 50 * 1000 # 100 * 1000
-POINTS_PER_YEAR = 20 # 25
+NUM_MC = 100 * 1000 # 100 * 1000
+POINTS_PER_YEAR = 25 # 25
 
 print(">> Set up runtime configuration")
 project_folder = os.path.join(settings.WORKFOLDER, "stovol")
 print("> Project folder: " + project_folder)
 data_folder = os.path.join(project_folder, "samples")
 print("> Data folder: " + data_folder)
 check_directory(data_folder)
@@ -120,16 +120,16 @@
 print(f"> Hidden layer structure: {HIDDEN_LAYERS}")
 print(f"> Number of neurons per layer: {NUM_NEURONS}")
 print(f"> Drop-out rate: {DROP_OUT:.2f}")
 
 # ################ Train the model ################################################################
 if TRAIN:
     # Learning rate scheduler
-    INIT_LR = 1.0e-2
-    FINAL_LR = 1.0e-4
+    INIT_LR = 1.0e-1
+    FINAL_LR = 1.0e-3
     DECAY = 0.97
     STEPS = 250
     lr_schedule = FlooredExponentialDecay(INIT_LR, FINAL_LR, DECAY, STEPS)
 
     # Optimizer
     optimizer = tf.keras.optimizers.Adam(learning_rate=lr_schedule)
     model.optimizer_ = optimizer.get_config()
@@ -182,45 +182,47 @@
 test_pred = model.predict(x_test)
 test_rmse = bps_rmse(test_pred, y_test)
 print(f"RMSE(nvol) on test set: {test_rmse:,.2f}")
 
 # Generate strike spread axis
 if SHOW_VOL_CHARTS:
     NUM_STRIKES = 100
-    PARAMS = { 'LnVol': 0.20, 'Beta': 0.5, 'Nu': 0.55, 'Rho': 0.25, 'Gamma': 0.7, 'Kappa': 1.0,
+    PARAMS = { 'LnVol': 0.20, 'Beta': 0.5, 'Nu': 0.55, 'Rho': -0.25, 'Gamma': 0.7, 'Kappa': 1.0,
                 'Theta': 0.05, 'Xi': 0.50 }
     FWD = 0.028
 
     # Any number of expiries can be calculated, but for optimum display choose no more than 6
-    EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.00, 10.0, 30.0]).reshape(-1, 1)
+    EXPIRIES = np.asarray([0.125, 0.250, 0.5, 1.00, 2.0, 5.0]).reshape(-1, 1)
+    # EXPIRIES = np.asarray([0.25, 0.50, 1.0, 5.00, 10.0, 30.0]).reshape(-1, 1)
     NUM_EXPIRIES = EXPIRIES.shape[0]
     METHOD = 'Percentiles'
     PERCENTS = np.linspace(0.01, 0.99, num=NUM_STRIKES)
     PERCENTS = np.asarray([PERCENTS] * NUM_EXPIRIES)
 
     strikes = generator.convert_strikes(EXPIRIES, PERCENTS, FWD, PARAMS, METHOD)
+    clipboard.export2d(strikes)
     ARE_CALLS = [[False] * NUM_STRIKES] * NUM_EXPIRIES # All puts
     # ARE_CALLS = [[False if s < FWD else True for s in expks] for expks in strikes] # Puts/calls
     # print(ARE_CALLS)
-    
+
     print("Calculating chart surface with reference model")
     ref_prices = generator.price_surface_ref(EXPIRIES, strikes, ARE_CALLS, FWD, PARAMS)
     # print(ref_prices.shape)
     # clipboard.export2d(ref_prices)
     print("Calculating chart surface with trained model")
     mod_prices = generator.price_surface_mod(model, EXPIRIES, strikes, ARE_CALLS, FWD, PARAMS)
     # print(mod_prices.shape)
     # clipboard.export2d(mod_prices)
     print(f"Ref-Mod RMSE(price): {bps_rmse(ref_prices, mod_prices):.2f}")
 
     # Available tranforms: Price, ShiftedBlackScholes, Bachelier
     TITLE = f"{MODEL_TYPE} smile sections, forward={FWD*100:.2f}"#,%\n parameters={PARAMS}"
-    TRANSFORM = "Bachelier"
+    # TRANSFORM = "Bachelier"
     # TRANSFORM = "Price"
-    #TRANSFORM = "ShiftedBlackScholes"
+    TRANSFORM = "ShiftedBlackScholes"
     xplt.plot_transform_surface(EXPIRIES, strikes, ARE_CALLS, FWD, ref_prices, mod_prices,
                                 TITLE, transform=TRANSFORM)
 
 
 # Show training history
 if TRAIN:
     hist_epochs = callback.epochs
```

### Comparing `sdevpy-0.0.9/src/sdevpy/projects/stovol/xsabrfit.py` & `sdevpy-0.1.0/src/sdevpy/projects/stovol/xsabrfit.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,29 @@
     (inputs) vs prices/implied vols (outputs) are generated (or read from tsv) to train a network that
     learns the so-called 'direct' calculation, i.e. prices from parameter. """
 import os
 from datetime import datetime
 import numpy as np
 import tensorflow as tf
 import matplotlib.pyplot as plt
-from volsurfacegen.sabrgenerator import SabrGenerator, ShiftedSabrGenerator
-from volsurfacegen.mcsabrgenerator import McShiftedSabrGenerator
-from volsurfacegen.fbsabrgenerator import FbSabrGenerator
-from volsurfacegen.mczabrgenerator import McShiftedZabrGenerator
-from volsurfacegen.mchestongenerator import McShiftedHestonGenerator
-import settings
-from machinelearning.topology import compose_model
-from machinelearning.learningmodel import LearningModel, load_learning_model
-from machinelearning.learningschedules import FlooredExponentialDecay
-from machinelearning.callbacks import RefCallback
-from machinelearning.datasets import prepare_sets
-from tools.filemanager import check_directory
-from tools.timer import Stopwatch
-from maths.metrics import rmse, tf_rmse
-from projects.xsabr import xsabrplot as xplt
+from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator, ShiftedSabrGenerator
+from sdevpy.volsurfacegen.mcsabrgenerator import McShiftedSabrGenerator
+from sdevpy.volsurfacegen.fbsabrgenerator import FbSabrGenerator
+from sdevpy.volsurfacegen.mczabrgenerator import McShiftedZabrGenerator
+from sdevpy.volsurfacegen.mchestongenerator import McShiftedHestonGenerator
+from sdevpy import settings
+from sdevpy.machinelearning.topology import compose_model
+from sdevpy.machinelearning.learningmodel import LearningModel, load_learning_model
+from sdevpy.machinelearning.learningschedules import FlooredExponentialDecay
+from sdevpy.machinelearning.callbacks import RefCallback
+from sdevpy.machinelearning.datasets import prepare_sets
+from sdevpy.tools.filemanager import check_directory
+from sdevpy.tools.timer import Stopwatch
+from sdevpy.maths.metrics import rmse, tf_rmse
+from sdevpy.projects.stovol import stovolplot as xplt
 
 # Re-training from saved model
 # Implement new class over LearningModel that gives prices directly, having stored
 #   the model. Implement inversions to shifted BS and Bachelier as well.
 # Possibility to test only without training
 # Utility to merge sample data files into 1
 # Finalize and fine-train models on extended parameter range
```

### Comparing `sdevpy-0.0.9/src/sdevpy/test.py` & `sdevpy-0.1.0/src/sdevpy/test.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/tools/clipboard.py` & `sdevpy-0.1.0/src/sdevpy/tools/clipboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Export data to clipboard/Excel (vectors and matrices) """
 import pyperclip
-# import numpy as np
 
 
 def concat_1dlist(data, sep='\n'):
     """ Concatenate a 1d list into a separated string """
     result = sep.join([str(d) for d in data])
     return result
```

### Comparing `sdevpy-0.0.9/src/sdevpy/tools/filemanager.py` & `sdevpy-0.1.0/src/sdevpy/tools/filemanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     path_exists = os.path.exists(path)
     if not path_exists:
         os.makedirs(path)
 
 
 def write_csv(file):
     """ Write content to csv file """
-    with open(file, mode='w', newline='') as csv_file:
+    with open(file, mode='w', newline='', encoding='utf8') as csv_file:
         writer = csv.writer(csv_file, delimiter=',')
         row = ['alpha', 'beta']
         writer.writerow(row)
 
 
 # def list_csv(path):
 #     """ List all csv files in a folder """
```

### Comparing `sdevpy-0.0.9/src/sdevpy/tools/jsonmanager.py` & `sdevpy-0.1.0/src/sdevpy/tools/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/tools/timegrids.py` & `sdevpy-0.1.0/src/sdevpy/tools/timegrids.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/tools/timer.py` & `sdevpy-0.1.0/src/sdevpy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy/volsurfacegen/fbsabrgenerator.py` & `sdevpy-0.1.0/src/sdevpy/volsurfacegen/fbsabrgenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Smile generator for Free-Boundary SABR model (FBSABR) using Monte-Carlo to calculate option
     prices """
 import os
-import settings
-from analytics import fbsabr
-from volsurfacegen.mcsabrgenerator import McSabrGenerator
-from tools import filemanager
-from tools import timer
+from sdevpy import settings
+from sdevpy.analytics import fbsabr
+from sdevpy.volsurfacegen.mcsabrgenerator import McSabrGenerator
+from sdevpy.tools import filemanager
+from sdevpy.tools import timer
 
 
 class FbSabrGenerator(McSabrGenerator):
     """ Free-Boundary SABR model using Monte-Carlo to calculate option prices. """
     def __init__(self, num_expiries=15, num_strikes=10, num_mc=10000, points_per_year=10,
                  seed=42):
         McSabrGenerator.__init__(self, 0.03, num_expiries, num_strikes, num_mc,
```

### Comparing `sdevpy-0.0.9/src/sdevpy/volsurfacegen/mchestongenerator.py` & `sdevpy-0.1.0/src/sdevpy/volsurfacegen/mchestongenerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Smile generator for Heston model using Monte-Carlo to calculate option prices """
 import os
 import numpy as np
 import pandas as pd
 import scipy.stats as sp
-import settings
-from analytics import mcheston
-from analytics import bachelier
-from volsurfacegen.sabrgenerator import SabrGenerator
-from volsurfacegen.smilegenerator import SmileGenerator
-from tools import filemanager
-from tools import timer
+from sdevpy import settings
+from sdevpy.analytics import mcheston
+from sdevpy.analytics import bachelier
+from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator
+from sdevpy.volsurfacegen.smilegenerator import SmileGenerator
+from sdevpy.tools import filemanager
+from sdevpy.tools import timer
 
 
 class McHestonGenerator(SabrGenerator):
     """ Heston model with a generic shift value, using Monte-Carlo to calculate option prices. """
     def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, num_mc=10000,
                  points_per_year=10):
         SabrGenerator.__init__(self, shift)
@@ -76,15 +76,16 @@
                 k = k - shift
 
                 ks.append(k)
 
             ks = np.asarray(ks)
 
             # Draw parameters
-            params = {'LnVol': lnvol[j], 'Kappa': kappa[j], 'Theta': theta[j], 'Xi': xi[j], 'Rho': rho[j]}
+            params = {'LnVol': lnvol[j], 'Kappa': kappa[j], 'Theta': theta[j], 'Xi': xi[j],
+                      'Rho': rho[j]}
 
             # Calculate prices
             price = self.price(expiries, ks, self.are_calls, fwd, params)
 
             # Flatten the results
             for exp_idx, expiry in enumerate(expiries):
                 ts.extend([expiry] * self.num_strikes)
@@ -100,18 +101,18 @@
         # Put in dataframe
         df = pd.DataFrame({'Ttm': ts, 'K': strikes, 'F': fwds, 'LnVol': lnvols, 'Kappa': kappas,
                            'Theta': thetas, 'Xi': xis, 'Rho': rhos, 'Price': prices})
         df.columns = ['Ttm', 'K', 'F', 'LnVol', 'Kappa', 'Theta', 'Xi', 'Rho', 'Price']
 
         return df
 
-    def price(self, expiry, strike, is_call, fwd, parameters):
-        shifted_k = strike + self.shift
+    def price(self, expiries, strikes, are_calls, fwd, parameters):
+        shifted_k = strikes + self.shift
         shifted_f = fwd + self.shift
-        prices = mcheston.price(expiry, shifted_k, is_call, shifted_f, parameters,
+        prices = mcheston.price(expiries, shifted_k, are_calls, shifted_f, parameters,
                                 self.num_mc, self.points_per_year)
 
         return prices
 
     def retrieve_datasets(self, data_file, shuffle=False):
         data_df = SmileGenerator.from_file(data_file, shuffle)
 
@@ -136,15 +137,15 @@
 
     # def price_surface_ref(self, expiries, strikes, is_call, fwd, parameters):
     #     are_calls = [is_call] * strikes.shape[1]
     #     are_calls = [are_calls] * expiries.shape[0]
     #     ref_prices = self.price(expiries, strikes, are_calls, fwd, parameters)
     #     return ref_prices
 
-    def price_surface_mod(self, model, expiries, strikes, is_call, fwd, parameters):
+    def price_surface_mod(self, model, expiries, strikes, are_calls, fwd, parameters):
         # Retrieve parameters
         lnvol = parameters['LnVol']
         kappa = parameters['Kappa']
         theta = parameters['Theta']
         xi = parameters['Xi']
         rho = parameters['Rho']
 
@@ -158,18 +159,21 @@
         md_inputs[:, 2] *= fwd
         md_inputs[:, 3] *= lnvol
         md_inputs[:, 4] *= kappa
         md_inputs[:, 5] *= theta
         md_inputs[:, 6] *= xi
         md_inputs[:, 7] *= rho
 
+        # Flatten are_calls
+        flat_types = np.asarray(are_calls).reshape(-1)
+
         # Price with learning model
         md_nvols = model.predict(md_inputs)
         md_prices = []
-        for (point, vol) in zip(md_inputs, md_nvols):
+        for (point, vol, is_call) in zip(md_inputs, md_nvols, flat_types):
             expiry = point[0]
             strike = point[1]
             md_prices.append(bachelier.price(expiry, strike, is_call, fwd, vol))
 
         md_prices = np.asarray(md_prices)
         return md_prices.reshape(num_expiries, num_strikes)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/volsurfacegen/mcsabrgenerator.py` & `sdevpy-0.1.0/src/sdevpy/volsurfacegen/mcsabrgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """ Smile generator for SABR model (shifted or not) using Monte-Carlo to calculate option
     prices """
 import os
 import numpy as np
 import pandas as pd
 import scipy.stats as sp
-import settings
-from analytics import mcsabr
+from sdevpy import settings
+from sdevpy.analytics import mcsabr
 # from analytics import black
-from analytics import bachelier
-from volsurfacegen.sabrgenerator import SabrGenerator
-from volsurfacegen.smilegenerator import SmileGenerator
-from tools import filemanager
+from sdevpy.analytics import bachelier
+from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator
+from sdevpy.volsurfacegen.smilegenerator import SmileGenerator
+from sdevpy.tools import filemanager
 # from tools import constants
-from tools import timer
+from sdevpy.tools import timer
 
 
 class McSabrGenerator(SabrGenerator):
     """ SABR model with a generic shift value, using Monte-Carlo to calculate option prices. """
     def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, num_mc=10000,
                  points_per_year=10, seed=42):
         SabrGenerator.__init__(self, shift, num_expiries, num_strikes, seed=seed)
@@ -131,21 +131,21 @@
         x_set = np.column_stack((t, strike, fwd, lnvol, beta, nu, rho))
         num_samples = len(nvol)
         y_set = np.asarray(nvol)
         y_set = np.reshape(y_set, (num_samples, 1))
 
         return x_set, y_set, data_df
 
-    def price_surface_ref(self, expiries, strikes, is_call, fwd, parameters):
-        are_calls = [is_call] * strikes.shape[1]
-        are_calls = [are_calls] * expiries.shape[0]
+    def price_surface_ref(self, expiries, strikes, are_calls, fwd, parameters):
+        # are_calls = [is_call] * strikes.shape[1]
+        # are_calls = [are_calls] * expiries.shape[0]
         ref_prices = self.price(expiries, strikes, are_calls, fwd, parameters)
         return ref_prices
 
-    def price_surface_mod(self, model, expiries, strikes, is_call, fwd, parameters):
+    def price_surface_mod(self, model, expiries, strikes, are_calls, fwd, parameters):
         # Retrieve parameters
         lnvol = parameters['LnVol']
         beta = parameters['Beta']
         nu = parameters['Nu']
         rho = parameters['Rho']
 
         # Prepare learning model inputs
@@ -157,18 +157,21 @@
         md_inputs[:, 1] = strikes.reshape(-1)
         md_inputs[:, 2] *= fwd
         md_inputs[:, 3] *= lnvol
         md_inputs[:, 4] *= beta
         md_inputs[:, 5] *= nu
         md_inputs[:, 6] *= rho
 
+        # Flatten are_calls
+        flat_types = np.asarray(are_calls).reshape(-1)
+
         # Price with learning model
         md_nvols = model.predict(md_inputs)
         md_prices = []
-        for (point, vol) in zip(md_inputs, md_nvols):
+        for (point, vol, is_call) in zip(md_inputs, md_nvols, flat_types):
             expiry = point[0]
             strike = point[1]
             md_prices.append(bachelier.price(expiry, strike, is_call, fwd, vol))
 
         md_prices = np.asarray(md_prices)
         return md_prices.reshape(num_expiries, num_strikes)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/volsurfacegen/mczabrgenerator.py` & `sdevpy-0.1.0/src/sdevpy/volsurfacegen/mczabrgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 """ Smile generator for ZABR model using Monte-Carlo to calculate option prices """
 import os
 import numpy as np
 import pandas as pd
 import scipy.stats as sp
-import settings
-from analytics import mczabr
+from sdevpy import settings
+from sdevpy.analytics import mczabr
 # from analytics import black
-from analytics import bachelier
-from volsurfacegen.sabrgenerator import SabrGenerator
-from volsurfacegen.smilegenerator import SmileGenerator
-from tools import filemanager
-from tools import timer
+from sdevpy.analytics import bachelier
+from sdevpy.volsurfacegen.sabrgenerator import SabrGenerator
+from sdevpy.volsurfacegen.smilegenerator import SmileGenerator
+from sdevpy.tools import filemanager
+from sdevpy.tools import timer
 
 
 class McZabrGenerator(SabrGenerator):
     """ ZABR model with a generic shift value, using Monte-Carlo to calculate option prices. """
     def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, num_mc=10000,
                  points_per_year=10):
         SabrGenerator.__init__(self, shift)
-        self.num_strikes = num_strikes
-        self.num_expiries = num_expiries
-        self.surface_size = self.num_expiries * self.num_strikes
+        # self.num_strikes = num_strikes
+        # self.num_expiries = num_expiries
+        # self.surface_size = self.num_expiries * self.num_strikes
         self.num_mc = num_mc
         self.points_per_year = points_per_year
-        self.are_calls = [[self.is_call] * self.num_strikes] * self.num_expiries
+        # self.are_calls = [[self.is_call] * self.num_strikes] * self.num_expiries
 
     def generate_samples(self, num_samples):
         shift = self.shift
 
         print(f"Number of strikes: {self.num_strikes:,}")
         print(f"Number of expiries: {self.num_expiries:,}")
         print(f"Surface size: {self.surface_size:,}")
@@ -77,15 +77,16 @@
                 k = k - shift
 
                 ks.append(k)
 
             ks = np.asarray(ks)
 
             # Draw parameters
-            params = {'LnVol': lnvol[j], 'Beta': beta[j], 'Nu': nu[j], 'Rho': rho[j], 'Gamma': gamma[j]}
+            params = {'LnVol': lnvol[j], 'Beta': beta[j], 'Nu': nu[j], 'Rho': rho[j],
+                      'Gamma': gamma[j]}
 
             # Calculate prices
             price = self.price(expiries, ks, self.are_calls, fwd, params)
 
             # Flatten the results
             for exp_idx, expiry in enumerate(expiries):
                 ts.extend([expiry] * self.num_strikes)
@@ -101,18 +102,18 @@
         # Put in dataframe
         df = pd.DataFrame({'Ttm': ts, 'K': strikes, 'F': fwds, 'LnVol': lnvols, 'Beta': betas,
                            'Nu': nus, 'Rho': rhos, 'Gamma': gammas, 'Price': prices})
         df.columns = ['Ttm', 'K', 'F', 'LnVol', 'Beta', 'Nu', 'Rho', 'Gamma', 'Price']
 
         return df
 
-    def price(self, expiry, strike, is_call, fwd, parameters):
-        shifted_k = strike + self.shift
+    def price(self, expiries, strikes, are_calls, fwd, parameters):
+        shifted_k = strikes + self.shift
         shifted_f = fwd + self.shift
-        prices = mczabr.price(expiry, shifted_k, is_call, shifted_f, parameters,
+        prices = mczabr.price(expiries, shifted_k, are_calls, shifted_f, parameters,
                               self.num_mc, self.points_per_year)
 
         return prices
 
     def retrieve_datasets(self, data_file, shuffle=False):
         data_df = SmileGenerator.from_file(data_file, shuffle)
 
@@ -137,15 +138,15 @@
 
     # def price_surface_ref(self, expiries, strikes, is_call, fwd, parameters):
     #     are_calls = [is_call] * strikes.shape[1]
     #     are_calls = [are_calls] * expiries.shape[0]
     #     ref_prices = self.price(expiries, strikes, are_calls, fwd, parameters)
     #     return ref_prices
 
-    def price_surface_mod(self, model, expiries, strikes, is_call, fwd, parameters):
+    def price_surface_mod(self, model, expiries, strikes, are_calls, fwd, parameters):
         # Retrieve parameters
         lnvol = parameters['LnVol']
         beta = parameters['Beta']
         nu = parameters['Nu']
         rho = parameters['Rho']
         gamma = parameters['Gamma']
 
@@ -159,18 +160,21 @@
         md_inputs[:, 2] *= fwd
         md_inputs[:, 3] *= lnvol
         md_inputs[:, 4] *= beta
         md_inputs[:, 5] *= nu
         md_inputs[:, 6] *= rho
         md_inputs[:, 7] *= gamma
 
+        # Flatten are_calls
+        flat_types = np.asarray(are_calls).reshape(-1)
+
         # Price with learning model
         md_nvols = model.predict(md_inputs)
         md_prices = []
-        for (point, vol) in zip(md_inputs, md_nvols):
+        for (point, vol, is_call) in zip(md_inputs, md_nvols, flat_types):
             expiry = point[0]
             strike = point[1]
             md_prices.append(bachelier.price(expiry, strike, is_call, fwd, vol))
 
         md_prices = np.asarray(md_prices)
         return md_prices.reshape(num_expiries, num_strikes)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/volsurfacegen/sabrgenerator.py` & `sdevpy-0.1.0/src/sdevpy/volsurfacegen/sabrgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """ Smile generator for classic and shifted Hagan SABR models """
 import os
 import numpy as np
 import pandas as pd
 import scipy.stats as sp
-import settings
-from analytics import sabr
-from analytics import black
-from analytics import bachelier
-from volsurfacegen.smilegenerator import SmileGenerator
-from tools import filemanager
-from tools import constants
+from sdevpy import settings
+from sdevpy.analytics import sabr
+from sdevpy.analytics import black
+from sdevpy.analytics import bachelier
+from sdevpy.volsurfacegen.smilegenerator import SmileGenerator
+from sdevpy.tools import filemanager
+from sdevpy.tools import constants
 
 
 class SabrGenerator(SmileGenerator):
     """ Base class for the classical SABR model with a generic shift value. The classical Hagan
       model (non-shifted) is the default case with shift = 0. """
     def __init__(self, shift=0.0, num_expiries=15, num_strikes=10, seed=42):
         SmileGenerator.__init__(self)
```

### Comparing `sdevpy-0.0.9/src/sdevpy/volsurfacegen/smilegenerator.py` & `sdevpy-0.1.0/src/sdevpy/volsurfacegen/smilegenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Base framework for smile generation """
 from abc import ABC, abstractmethod
 import numpy as np
 import pandas as pd
-from analytics import bachelier
-from analytics import black
+from sdevpy.analytics import bachelier
+# from sdevpy.analytics import black
 
 
 class SmileGenerator(ABC):
     """ Base class for smile generation """
     def __init__(self):
         self.num_curve_parameters = 0
         self.num_vol_parameters = 0
@@ -26,30 +26,30 @@
         """ Retrieve dataset stored in tsv file """
 
     # @abstractmethod
     # def price_strike_ladder(self, model, expiry, spreads, fwd, parameters):
     #     """ Calculate prices for a ladder of strikes for given parameters """
 
     @abstractmethod
-    def price_surface_ref(self, expiries, strikes, is_call, fwd, parameters):
+    def price_surface_ref(self, expiries, strikes, are_calls, fwd, parameters):
         """ Calculate a surface of prices for given parameters using the generating model """
 
     @abstractmethod
-    def price_surface_mod(self, model, expiries, strikes, is_call, fwd, parameters):
+    def price_surface_mod(self, model, expiries, strikes, are_calls, fwd, parameters):
         """ Calculate a surface of prices for given parameters using the learning model """
 
     def convert_strikes(self, expiries, strike_inputs, fwd, parameters, input_method='Strikes'):
         """ Convert strike inputs into absolute strikes using the strike input_method """
         if input_method == 'Strikes':
             strikes = strike_inputs
         elif input_method == 'Spreads':
             strikes = fwd + strike_inputs / 10000.0
         else:
             raise ValueError("Invalid strike input method: " + input_method)
-        
+
         return strikes
 
     def num_parameters(self):
         """ Total number of parameters (curve + vol) """
         return self.num_curve_parameters + self.num_vol_parameters
 
     def to_nvol(self, data_df, cleanse=True, min_vol=0.0001, max_vol=0.1):
```

### Comparing `sdevpy-0.0.9/src/sdevpy/volsurfacegen/stovolfactory.py` & `sdevpy-0.1.0/src/sdevpy/volsurfacegen/stovolfactory.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.0.9/src/sdevpy.egg-info/PKG-INFO` & `sdevpy-0.1.0/src/sdevpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.0.9
+Version: 0.1.0
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.0.9/src/sdevpy.egg-info/SOURCES.txt` & `sdevpy-0.1.0/src/sdevpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,30 @@
 LICENSE
 README.md
 pyproject.toml
 src/sdevpy/__init__.py
-src/sdevpy/example.py
 src/sdevpy/settings.py
 src/sdevpy/test.py
 src/sdevpy.egg-info/PKG-INFO
 src/sdevpy.egg-info/SOURCES.txt
 src/sdevpy.egg-info/dependency_links.txt
 src/sdevpy.egg-info/requires.txt
 src/sdevpy.egg-info/top_level.txt
-src/sdevpy/analytics/__init__.py
 src/sdevpy/analytics/bachelier.py
 src/sdevpy/analytics/black.py
 src/sdevpy/analytics/fbsabr.py
 src/sdevpy/analytics/mcheston.py
 src/sdevpy/analytics/mcsabr.py
 src/sdevpy/analytics/mczabr.py
 src/sdevpy/analytics/sabr.py
-src/sdevpy/machinelearning/__init__.py
 src/sdevpy/machinelearning/callbacks.py
 src/sdevpy/machinelearning/datasets.py
 src/sdevpy/machinelearning/learningmodel.py
 src/sdevpy/machinelearning/learningschedules.py
 src/sdevpy/machinelearning/topology.py
-src/sdevpy/maths/__init__.py
 src/sdevpy/maths/interpolations.py
 src/sdevpy/maths/metrics.py
 src/sdevpy/maths/optimization.py
 src/sdevpy/maths/rand.py
 src/sdevpy/projects/datafiles.py
 src/sdevpy/projects/pinns/ernst_pinns.py
 src/sdevpy/projects/pinns/pinns.py
```

