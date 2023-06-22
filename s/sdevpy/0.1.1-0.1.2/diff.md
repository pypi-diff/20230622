# Comparing `tmp/sdevpy-0.1.1.tar.gz` & `tmp/sdevpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdevpy-0.1.1.tar", last modified: Thu Jun 22 01:28:28 2023, max compression
+gzip compressed data, was "sdevpy-0.1.2.tar", last modified: Thu Jun 22 04:54:32 2023, max compression
```

## Comparing `sdevpy-0.1.1.tar` & `sdevpy-0.1.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.053605 sdevpy-0.1.1/
--rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1725 2023-06-22 01:28:28.052606 sdevpy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.1.1/README.md
--rw-rw-rw-   0        0        0      655 2023-06-22 01:04:22.000000 sdevpy-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 01:28:28.053605 sdevpy-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:27.936643 sdevpy-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:27.951638 sdevpy-0.1.1/src/sdevpy/
--rw-rw-rw-   0        0        0       23 2023-06-19 11:53:52.000000 sdevpy-0.1.1/src/sdevpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:27.992625 sdevpy-0.1.1/src/sdevpy/analytics/
--rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.1.1/src/sdevpy/analytics/bachelier.py
--rw-rw-rw-   0        0        0     2810 2023-06-20 03:38:43.000000 sdevpy-0.1.1/src/sdevpy/analytics/black.py
--rw-rw-rw-   0        0        0     6308 2023-06-20 03:41:05.000000 sdevpy-0.1.1/src/sdevpy/analytics/fbsabr.py
--rw-rw-rw-   0        0        0     6911 2023-06-20 03:42:55.000000 sdevpy-0.1.1/src/sdevpy/analytics/mcheston.py
--rw-rw-rw-   0        0        0     7657 2023-06-20 03:43:39.000000 sdevpy-0.1.1/src/sdevpy/analytics/mcsabr.py
--rw-rw-rw-   0        0        0     8745 2023-06-20 03:49:45.000000 sdevpy-0.1.1/src/sdevpy/analytics/mczabr.py
--rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.1.1/src/sdevpy/analytics/sabr.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:27.999623 sdevpy-0.1.1/src/sdevpy/machinelearning/
--rw-rw-rw-   0        0        0     4350 2023-06-19 11:59:56.000000 sdevpy-0.1.1/src/sdevpy/machinelearning/callbacks.py
--rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.1.1/src/sdevpy/machinelearning/datasets.py
--rw-rw-rw-   0        0        0     6101 2023-06-20 09:15:35.000000 sdevpy-0.1.1/src/sdevpy/machinelearning/learningmodel.py
--rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.1.1/src/sdevpy/machinelearning/learningschedules.py
--rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.1.1/src/sdevpy/machinelearning/topology.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.006620 sdevpy-0.1.1/src/sdevpy/maths/
--rw-rw-rw-   0        0        0      840 2023-06-20 06:44:09.000000 sdevpy-0.1.1/src/sdevpy/maths/interpolations.py
--rw-rw-rw-   0        0        0      413 2023-06-20 08:24:06.000000 sdevpy-0.1.1/src/sdevpy/maths/metrics.py
--rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.1.1/src/sdevpy/maths/optimization.py
--rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.1.1/src/sdevpy/maths/rand.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.007620 sdevpy-0.1.1/src/sdevpy/projects/
--rw-rw-rw-   0        0        0      893 2023-06-19 11:54:24.000000 sdevpy-0.1.1/src/sdevpy/projects/datafiles.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.018617 sdevpy-0.1.1/src/sdevpy/projects/pinns/
--rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.1.1/src/sdevpy/projects/pinns/ernst_pinns.py
--rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.1.1/src/sdevpy/projects/pinns/pinns.py
--rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.1.1/src/sdevpy/projects/pinns/pinns_worst_of.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.028613 sdevpy-0.1.1/src/sdevpy/projects/stovol/
--rw-rw-rw-   0        0        0     2513 2023-06-21 13:29:16.000000 sdevpy-0.1.1/src/sdevpy/projects/stovol/stovolgen.py
--rw-rw-rw-   0        0        0     5033 2023-06-21 13:31:09.000000 sdevpy-0.1.1/src/sdevpy/projects/stovol/stovolplot.py
--rw-rw-rw-   0        0        0    10181 2023-06-21 13:31:58.000000 sdevpy-0.1.1/src/sdevpy/projects/stovol/stovoltrain.py
--rw-rw-rw-   0        0        0    10577 2023-06-21 13:33:49.000000 sdevpy-0.1.1/src/sdevpy/projects/stovol/xsabrfit.py
--rw-rw-rw-   0        0        0      400 2023-06-19 11:47:07.000000 sdevpy-0.1.1/src/sdevpy/settings.py
--rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.1.1/src/sdevpy/test.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.039610 sdevpy-0.1.1/src/sdevpy/tools/
--rw-rw-rw-   0        0        0     1048 2023-06-20 09:17:04.000000 sdevpy-0.1.1/src/sdevpy/tools/clipboard.py
--rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.1.1/src/sdevpy/tools/constants.py
--rw-rw-rw-   0        0        0     1546 2023-06-20 09:18:04.000000 sdevpy-0.1.1/src/sdevpy/tools/filemanager.py
--rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.1.1/src/sdevpy/tools/jsonmanager.py
--rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.1.1/src/sdevpy/tools/timegrids.py
--rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.1.1/src/sdevpy/tools/timer.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.049607 sdevpy-0.1.1/src/sdevpy/volsurfacegen/
--rw-rw-rw-   0        0        0     2529 2023-06-21 13:34:01.000000 sdevpy-0.1.1/src/sdevpy/volsurfacegen/fbsabrgenerator.py
--rw-rw-rw-   0        0        0     8773 2023-06-20 09:22:19.000000 sdevpy-0.1.1/src/sdevpy/volsurfacegen/mchestongenerator.py
--rw-rw-rw-   0        0        0     9366 2023-06-21 13:33:57.000000 sdevpy-0.1.1/src/sdevpy/volsurfacegen/mcsabrgenerator.py
--rw-rw-rw-   0        0        0     9324 2023-06-21 13:23:45.000000 sdevpy-0.1.1/src/sdevpy/volsurfacegen/mczabrgenerator.py
--rw-rw-rw-   0        0        0    11547 2023-06-21 13:33:58.000000 sdevpy-0.1.1/src/sdevpy/volsurfacegen/sabrgenerator.py
--rw-rw-rw-   0        0        0     4789 2023-06-21 13:33:59.000000 sdevpy-0.1.1/src/sdevpy/volsurfacegen/smilegenerator.py
--rw-rw-rw-   0        0        0     2118 2023-06-21 13:34:03.000000 sdevpy-0.1.1/src/sdevpy/volsurfacegen/stovolfactory.py
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:27.975630 sdevpy-0.1.1/src/sdevpy.egg-info/
--rw-rw-rw-   0        0        0     1725 2023-06-22 01:28:27.000000 sdevpy-0.1.1/src/sdevpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1630 2023-06-22 01:28:27.000000 sdevpy-0.1.1/src/sdevpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 01:28:27.000000 sdevpy-0.1.1/src/sdevpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-06-22 01:28:27.000000 sdevpy-0.1.1/src/sdevpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 01:28:27.000000 sdevpy-0.1.1/src/sdevpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-22 01:28:28.051606 sdevpy-0.1.1/tests/
--rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.1.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.316430 sdevpy-0.1.2/
+-rw-rw-rw-   0        0        0     1098 2023-06-17 02:41:33.000000 sdevpy-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     1725 2023-06-22 04:54:32.315430 sdevpy-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2023-06-18 08:19:59.000000 sdevpy-0.1.2/README.md
+-rw-rw-rw-   0        0        0      655 2023-06-22 04:54:00.000000 sdevpy-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 04:54:32.317429 sdevpy-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.200467 sdevpy-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.218462 sdevpy-0.1.2/src/sdevpy/
+-rw-rw-rw-   0        0        0       23 2023-06-19 11:53:52.000000 sdevpy-0.1.2/src/sdevpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.256449 sdevpy-0.1.2/src/sdevpy/analytics/
+-rw-rw-rw-   0        0        0     2415 2023-04-15 10:09:55.000000 sdevpy-0.1.2/src/sdevpy/analytics/bachelier.py
+-rw-rw-rw-   0        0        0     2810 2023-06-20 03:38:43.000000 sdevpy-0.1.2/src/sdevpy/analytics/black.py
+-rw-rw-rw-   0        0        0     6308 2023-06-20 03:41:05.000000 sdevpy-0.1.2/src/sdevpy/analytics/fbsabr.py
+-rw-rw-rw-   0        0        0     6911 2023-06-20 03:42:55.000000 sdevpy-0.1.2/src/sdevpy/analytics/mcheston.py
+-rw-rw-rw-   0        0        0     7657 2023-06-20 03:43:39.000000 sdevpy-0.1.2/src/sdevpy/analytics/mcsabr.py
+-rw-rw-rw-   0        0        0     8745 2023-06-20 03:49:45.000000 sdevpy-0.1.2/src/sdevpy/analytics/mczabr.py
+-rw-rw-rw-   0        0        0     2790 2023-05-07 07:20:24.000000 sdevpy-0.1.2/src/sdevpy/analytics/sabr.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.267446 sdevpy-0.1.2/src/sdevpy/machinelearning/
+-rw-rw-rw-   0        0        0     4350 2023-06-19 11:59:56.000000 sdevpy-0.1.2/src/sdevpy/machinelearning/callbacks.py
+-rw-rw-rw-   0        0        0     1119 2023-04-28 08:07:24.000000 sdevpy-0.1.2/src/sdevpy/machinelearning/datasets.py
+-rw-rw-rw-   0        0        0     6101 2023-06-20 09:15:35.000000 sdevpy-0.1.2/src/sdevpy/machinelearning/learningmodel.py
+-rw-rw-rw-   0        0        0      997 2023-05-01 01:07:36.000000 sdevpy-0.1.2/src/sdevpy/machinelearning/learningschedules.py
+-rw-rw-rw-   0        0        0     2390 2023-04-08 04:29:36.000000 sdevpy-0.1.2/src/sdevpy/machinelearning/topology.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.272444 sdevpy-0.1.2/src/sdevpy/maths/
+-rw-rw-rw-   0        0        0      840 2023-06-20 06:44:09.000000 sdevpy-0.1.2/src/sdevpy/maths/interpolations.py
+-rw-rw-rw-   0        0        0      413 2023-06-20 08:24:06.000000 sdevpy-0.1.2/src/sdevpy/maths/metrics.py
+-rw-rw-rw-   0        0        0       85 2022-11-12 05:23:02.000000 sdevpy-0.1.2/src/sdevpy/maths/optimization.py
+-rw-rw-rw-   0        0        0     3773 2023-05-20 06:07:54.000000 sdevpy-0.1.2/src/sdevpy/maths/rand.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.275443 sdevpy-0.1.2/src/sdevpy/projects/
+-rw-rw-rw-   0        0        0      893 2023-06-19 11:54:24.000000 sdevpy-0.1.2/src/sdevpy/projects/datafiles.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.281441 sdevpy-0.1.2/src/sdevpy/projects/pinns/
+-rw-rw-rw-   0        0        0    10211 2022-11-29 00:51:51.000000 sdevpy-0.1.2/src/sdevpy/projects/pinns/ernst_pinns.py
+-rw-rw-rw-   0        0        0    11863 2022-12-19 07:49:15.000000 sdevpy-0.1.2/src/sdevpy/projects/pinns/pinns.py
+-rw-rw-rw-   0        0        0    23680 2023-02-26 08:44:57.000000 sdevpy-0.1.2/src/sdevpy/projects/pinns/pinns_worst_of.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.288439 sdevpy-0.1.2/src/sdevpy/projects/stovol/
+-rw-rw-rw-   0        0        0     2513 2023-06-21 13:29:16.000000 sdevpy-0.1.2/src/sdevpy/projects/stovol/stovolgen.py
+-rw-rw-rw-   0        0        0     5033 2023-06-21 13:31:09.000000 sdevpy-0.1.2/src/sdevpy/projects/stovol/stovolplot.py
+-rw-rw-rw-   0        0        0    10181 2023-06-21 13:31:58.000000 sdevpy-0.1.2/src/sdevpy/projects/stovol/stovoltrain.py
+-rw-rw-rw-   0        0        0    10577 2023-06-21 13:33:49.000000 sdevpy-0.1.2/src/sdevpy/projects/stovol/xsabrfit.py
+-rw-rw-rw-   0        0        0      400 2023-06-19 11:47:07.000000 sdevpy-0.1.2/src/sdevpy/settings.py
+-rw-rw-rw-   0        0        0     4810 2023-06-16 03:12:25.000000 sdevpy-0.1.2/src/sdevpy/test.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.300435 sdevpy-0.1.2/src/sdevpy/tools/
+-rw-rw-rw-   0        0        0     1048 2023-06-20 09:17:04.000000 sdevpy-0.1.2/src/sdevpy/tools/clipboard.py
+-rw-rw-rw-   0        0        0       48 2023-04-16 03:13:45.000000 sdevpy-0.1.2/src/sdevpy/tools/constants.py
+-rw-rw-rw-   0        0        0     1546 2023-06-20 09:18:04.000000 sdevpy-0.1.2/src/sdevpy/tools/filemanager.py
+-rw-rw-rw-   0        0        0     1190 2023-06-10 07:03:10.000000 sdevpy-0.1.2/src/sdevpy/tools/jsonmanager.py
+-rw-rw-rw-   0        0        0     2884 2023-05-06 00:57:32.000000 sdevpy-0.1.2/src/sdevpy/tools/timegrids.py
+-rw-rw-rw-   0        0        0      867 2023-04-09 05:08:45.000000 sdevpy-0.1.2/src/sdevpy/tools/timer.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.312431 sdevpy-0.1.2/src/sdevpy/volsurfacegen/
+-rw-rw-rw-   0        0        0     2529 2023-06-21 13:34:01.000000 sdevpy-0.1.2/src/sdevpy/volsurfacegen/fbsabrgenerator.py
+-rw-rw-rw-   0        0        0     8773 2023-06-20 09:22:19.000000 sdevpy-0.1.2/src/sdevpy/volsurfacegen/mchestongenerator.py
+-rw-rw-rw-   0        0        0     9366 2023-06-21 13:33:57.000000 sdevpy-0.1.2/src/sdevpy/volsurfacegen/mcsabrgenerator.py
+-rw-rw-rw-   0        0        0     9324 2023-06-21 13:23:45.000000 sdevpy-0.1.2/src/sdevpy/volsurfacegen/mczabrgenerator.py
+-rw-rw-rw-   0        0        0    11547 2023-06-21 13:33:58.000000 sdevpy-0.1.2/src/sdevpy/volsurfacegen/sabrgenerator.py
+-rw-rw-rw-   0        0        0     4789 2023-06-21 13:33:59.000000 sdevpy-0.1.2/src/sdevpy/volsurfacegen/smilegenerator.py
+-rw-rw-rw-   0        0        0     2118 2023-06-21 13:34:03.000000 sdevpy-0.1.2/src/sdevpy/volsurfacegen/stovolfactory.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.240454 sdevpy-0.1.2/src/sdevpy.egg-info/
+-rw-rw-rw-   0        0        0     1725 2023-06-22 04:54:32.000000 sdevpy-0.1.2/src/sdevpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1630 2023-06-22 04:54:32.000000 sdevpy-0.1.2/src/sdevpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 04:54:32.000000 sdevpy-0.1.2/src/sdevpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-22 04:54:32.000000 sdevpy-0.1.2/src/sdevpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 04:54:32.000000 sdevpy-0.1.2/src/sdevpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 04:54:32.314430 sdevpy-0.1.2/tests/
+-rw-rw-rw-   0        0        0      212 2023-06-18 06:08:53.000000 sdevpy-0.1.2/tests/test.py
```

### Comparing `sdevpy-0.1.1/LICENSE` & `sdevpy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/PKG-INFO` & `sdevpy-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.1.1/README.md` & `sdevpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/pyproject.toml` & `sdevpy-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sdevpy"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Sebastien Gurrieri", email="sebgur@gmail.com" },
 ]
 description = "Python package for Machine Learning in Finance"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `sdevpy-0.1.1/src/sdevpy/analytics/bachelier.py` & `sdevpy-0.1.2/src/sdevpy/analytics/bachelier.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/analytics/black.py` & `sdevpy-0.1.2/src/sdevpy/analytics/black.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/analytics/fbsabr.py` & `sdevpy-0.1.2/src/sdevpy/analytics/fbsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/analytics/mcheston.py` & `sdevpy-0.1.2/src/sdevpy/analytics/mcheston.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/analytics/mcsabr.py` & `sdevpy-0.1.2/src/sdevpy/analytics/mcsabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/analytics/mczabr.py` & `sdevpy-0.1.2/src/sdevpy/analytics/mczabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/analytics/sabr.py` & `sdevpy-0.1.2/src/sdevpy/analytics/sabr.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/machinelearning/callbacks.py` & `sdevpy-0.1.2/src/sdevpy/machinelearning/callbacks.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/machinelearning/datasets.py` & `sdevpy-0.1.2/src/sdevpy/machinelearning/datasets.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/machinelearning/learningmodel.py` & `sdevpy-0.1.2/src/sdevpy/machinelearning/learningmodel.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/machinelearning/learningschedules.py` & `sdevpy-0.1.2/src/sdevpy/machinelearning/learningschedules.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/machinelearning/topology.py` & `sdevpy-0.1.2/src/sdevpy/machinelearning/topology.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/maths/interpolations.py` & `sdevpy-0.1.2/src/sdevpy/maths/interpolations.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/maths/rand.py` & `sdevpy-0.1.2/src/sdevpy/maths/rand.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/datafiles.py` & `sdevpy-0.1.2/src/sdevpy/projects/datafiles.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/pinns/ernst_pinns.py` & `sdevpy-0.1.2/src/sdevpy/projects/pinns/ernst_pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/pinns/pinns.py` & `sdevpy-0.1.2/src/sdevpy/projects/pinns/pinns.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/pinns/pinns_worst_of.py` & `sdevpy-0.1.2/src/sdevpy/projects/pinns/pinns_worst_of.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/stovol/stovolgen.py` & `sdevpy-0.1.2/src/sdevpy/projects/stovol/stovolgen.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/stovol/stovolplot.py` & `sdevpy-0.1.2/src/sdevpy/projects/stovol/stovolplot.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/stovol/stovoltrain.py` & `sdevpy-0.1.2/src/sdevpy/projects/stovol/stovoltrain.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/projects/stovol/xsabrfit.py` & `sdevpy-0.1.2/src/sdevpy/projects/stovol/xsabrfit.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/test.py` & `sdevpy-0.1.2/src/sdevpy/test.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/tools/clipboard.py` & `sdevpy-0.1.2/src/sdevpy/tools/clipboard.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/tools/filemanager.py` & `sdevpy-0.1.2/src/sdevpy/tools/filemanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/tools/jsonmanager.py` & `sdevpy-0.1.2/src/sdevpy/tools/jsonmanager.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/tools/timegrids.py` & `sdevpy-0.1.2/src/sdevpy/tools/timegrids.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/tools/timer.py` & `sdevpy-0.1.2/src/sdevpy/tools/timer.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/volsurfacegen/fbsabrgenerator.py` & `sdevpy-0.1.2/src/sdevpy/volsurfacegen/fbsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/volsurfacegen/mchestongenerator.py` & `sdevpy-0.1.2/src/sdevpy/volsurfacegen/mchestongenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/volsurfacegen/mcsabrgenerator.py` & `sdevpy-0.1.2/src/sdevpy/volsurfacegen/mcsabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/volsurfacegen/mczabrgenerator.py` & `sdevpy-0.1.2/src/sdevpy/volsurfacegen/mczabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/volsurfacegen/sabrgenerator.py` & `sdevpy-0.1.2/src/sdevpy/volsurfacegen/sabrgenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/volsurfacegen/smilegenerator.py` & `sdevpy-0.1.2/src/sdevpy/volsurfacegen/smilegenerator.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy/volsurfacegen/stovolfactory.py` & `sdevpy-0.1.2/src/sdevpy/volsurfacegen/stovolfactory.py`

 * *Files identical despite different names*

### Comparing `sdevpy-0.1.1/src/sdevpy.egg-info/PKG-INFO` & `sdevpy-0.1.2/src/sdevpy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdevpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python package for Machine Learning in Finance
 Author-email: Sebastien Gurrieri <sebgur@gmail.com>
 Project-URL: Git page, https://github.com/sebgur/SDev.Python
 Project-URL: SDev Finance, http://sdev-finance.com/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sdevpy-0.1.1/src/sdevpy.egg-info/SOURCES.txt` & `sdevpy-0.1.2/src/sdevpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

