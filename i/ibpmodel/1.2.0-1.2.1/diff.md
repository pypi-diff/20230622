# Comparing `tmp/ibpmodel-1.2.0.tar.gz` & `tmp/ibpmodel-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibpmodel-1.2.0.tar", last modified: Mon May  8 10:09:12 2023, max compression
+gzip compressed data, was "ibpmodel-1.2.1.tar", last modified: Thu Jun 22 08:09:31 2023, max compression
```

## Comparing `ibpmodel-1.2.0.tar` & `ibpmodel-1.2.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       93 2023-03-29 07:21:17.000000 ibpmodel-1.2.0/.gitignore
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      672 2023-03-29 11:58:52.000000 ibpmodel-1.2.0/.readthedocs.yml
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      617 2023-03-30 10:54:42.000000 ibpmodel-1.2.0/CHANGELOG.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1067 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/LICENSE
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     5398 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/PKG-INFO
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     4186 2023-04-13 08:01:15.000000 ibpmodel-1.2.0/README.rst
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.722227 ibpmodel-1.2.0/docs/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      638 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/Makefile
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      804 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/make.bat
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.722227 ibpmodel-1.2.0/docs/source/
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.726227 ibpmodel-1.2.0/docs/source/_static/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)  3933900 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf
--rw-rw-r--   0 iw01      (1000) iw01      (1000)    81773 2023-03-29 12:42:24.000000 ibpmodel-1.2.0/docs/source/_static/example_plotButterfly.png
--rw-rw-r--   0 iw01      (1000) iw01      (1000)    67180 2023-03-29 13:41:06.000000 ibpmodel-1.2.0/docs/source/_static/example_plotIBP.png
--rw-rw-r--   0 iw01      (1000) iw01      (1000)   158206 2023-05-08 06:38:12.000000 ibpmodel-1.2.0/docs/source/_static/example_subplot.png
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       32 2023-03-30 10:10:13.000000 ibpmodel-1.2.0/docs/source/changelog.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1658 2023-04-18 05:52:28.000000 ibpmodel-1.2.0/docs/source/conf.py
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      317 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/ibpmodel.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      503 2023-03-30 10:20:17.000000 ibpmodel-1.2.0/docs/source/index.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      588 2023-04-13 06:57:00.000000 ibpmodel-1.2.0/docs/source/installation.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      111 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/modules.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      112 2023-03-02 13:04:40.000000 ibpmodel-1.2.0/docs/source/reference.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       89 2023-04-12 12:08:33.000000 ibpmodel-1.2.0/docs/source/requirements.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     2195 2023-05-08 06:38:12.000000 ibpmodel-1.2.0/docs/source/usage.rst
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1577 2023-03-30 13:35:51.000000 ibpmodel-1.2.0/pyproject.toml
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     1173 2023-04-13 08:08:08.000000 ibpmodel-1.2.0/requirements.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       38 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/setup.cfg
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.722227 ibpmodel-1.2.0/src/
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.726227 ibpmodel-1.2.0/src/ibpmodel/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)  1212651 2023-03-22 11:18:00.000000 ibpmodel-1.2.0/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      325 2023-04-13 09:35:36.000000 ibpmodel-1.2.0/src/ibpmodel/__init__.py
--rw-rw-r--   0 iw01      (1000) iw01      (1000)    22302 2023-05-08 07:46:52.000000 ibpmodel-1.2.0/src/ibpmodel/ibpcalc.py
--rw-rw-r--   0 iw01      (1000) iw01      (1000)    10169 2023-05-08 06:38:12.000000 ibpmodel-1.2.0/src/ibpmodel/ibpforward.py
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/src/ibpmodel.egg-info/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)     5398 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/PKG-INFO
--rw-rw-r--   0 iw01      (1000) iw01      (1000)      900 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/SOURCES.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)        1 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/dependency_links.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)       65 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/requires.txt
--rw-rw-r--   0 iw01      (1000) iw01      (1000)        9 2023-05-08 10:09:12.000000 ibpmodel-1.2.0/src/ibpmodel.egg-info/top_level.txt
-drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-05-08 10:09:12.730227 ibpmodel-1.2.0/template/
--rw-rw-r--   0 iw01      (1000) iw01      (1000)  1189939 2023-05-08 09:55:14.000000 ibpmodel-1.2.0/template/IBP_CLI_2_bubble-probability.ipynb
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.605705 ibpmodel-1.2.1/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      101 2023-06-22 07:43:19.000000 ibpmodel-1.2.1/.gitignore
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      672 2023-03-29 11:58:52.000000 ibpmodel-1.2.1/.readthedocs.yml
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      784 2023-06-22 07:39:51.000000 ibpmodel-1.2.1/CHANGELOG.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     1066 2023-06-21 14:26:36.000000 ibpmodel-1.2.1/LICENSE
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     5406 2023-06-22 08:09:31.605705 ibpmodel-1.2.1/PKG-INFO
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     4196 2023-06-21 13:28:02.000000 ibpmodel-1.2.1/README.rst
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.589705 ibpmodel-1.2.1/docs/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      638 2023-03-02 13:04:40.000000 ibpmodel-1.2.1/docs/Makefile
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      804 2023-03-02 13:04:40.000000 ibpmodel-1.2.1/docs/make.bat
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.593705 ibpmodel-1.2.1/docs/source/
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.601705 ibpmodel-1.2.1/docs/source/_static/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)  3933900 2023-03-02 13:04:40.000000 ibpmodel-1.2.1/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    82341 2023-06-21 13:27:45.000000 ibpmodel-1.2.1/docs/source/_static/example_plotButterfly.png
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    89100 2023-06-21 13:27:21.000000 ibpmodel-1.2.1/docs/source/_static/example_plotIBP.png
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)   158206 2023-05-08 10:43:17.000000 ibpmodel-1.2.1/docs/source/_static/example_subplot.png
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       32 2023-03-30 10:10:13.000000 ibpmodel-1.2.1/docs/source/changelog.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     1656 2023-06-21 14:20:42.000000 ibpmodel-1.2.1/docs/source/conf.py
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      317 2023-03-02 13:04:40.000000 ibpmodel-1.2.1/docs/source/ibpmodel.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      503 2023-03-30 10:20:17.000000 ibpmodel-1.2.1/docs/source/index.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      588 2023-04-13 06:57:00.000000 ibpmodel-1.2.1/docs/source/installation.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      111 2023-03-02 13:04:40.000000 ibpmodel-1.2.1/docs/source/modules.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      112 2023-03-02 13:04:40.000000 ibpmodel-1.2.1/docs/source/reference.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       89 2023-04-12 12:08:33.000000 ibpmodel-1.2.1/docs/source/requirements.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     2195 2023-05-08 10:43:17.000000 ibpmodel-1.2.1/docs/source/usage.rst
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     1580 2023-06-21 14:20:00.000000 ibpmodel-1.2.1/pyproject.toml
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      166 2023-06-21 14:06:09.000000 ibpmodel-1.2.1/requirements-dev.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       73 2023-06-21 14:16:36.000000 ibpmodel-1.2.1/requirements.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       38 2023-06-22 08:09:31.605705 ibpmodel-1.2.1/setup.cfg
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.585705 ibpmodel-1.2.1/src/
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.601705 ibpmodel-1.2.1/src/ibpmodel/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)  1212651 2023-03-22 11:18:00.000000 ibpmodel-1.2.1/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      325 2023-06-21 10:07:56.000000 ibpmodel-1.2.1/src/ibpmodel/__init__.py
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    22300 2023-06-21 10:46:25.000000 ibpmodel-1.2.1/src/ibpmodel/ibpcalc.py
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)    10372 2023-06-21 11:39:13.000000 ibpmodel-1.2.1/src/ibpmodel/ibpforward.py
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.601705 ibpmodel-1.2.1/src/ibpmodel.egg-info/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)     5406 2023-06-22 08:09:31.000000 ibpmodel-1.2.1/src/ibpmodel.egg-info/PKG-INFO
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)      946 2023-06-22 08:09:31.000000 ibpmodel-1.2.1/src/ibpmodel.egg-info/SOURCES.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)        1 2023-06-22 08:09:31.000000 ibpmodel-1.2.1/src/ibpmodel.egg-info/dependency_links.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)       68 2023-06-22 08:09:31.000000 ibpmodel-1.2.1/src/ibpmodel.egg-info/requires.txt
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)        9 2023-06-22 08:09:31.000000 ibpmodel-1.2.1/src/ibpmodel.egg-info/top_level.txt
+drwxrwxr-x   0 iw01      (1000) iw01      (1000)        0 2023-06-22 08:09:31.601705 ibpmodel-1.2.1/template/
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)   107065 2023-05-25 12:17:59.000000 ibpmodel-1.2.1/template/IBP-VirES.ipynb
+-rw-rw-r--   0 iw01      (1000) iw01      (1000)  1189939 2023-05-25 11:46:50.000000 ibpmodel-1.2.1/template/IBP_CLI_2_bubble-probability.ipynb
```

### Comparing `ibpmodel-1.2.0/.readthedocs.yml` & `ibpmodel-1.2.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/LICENSE` & `ibpmodel-1.2.1/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Ina Wehner
+Copyright (c) 2023 Ina Rusch
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ibpmodel-1.2.0/PKG-INFO` & `ibpmodel-1.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ibpmodel
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ionospheric Bubble Probability
 Author: Martin Rother
-Maintainer-email: Ina Wehner <wehner@iap-kborn.de>
+Maintainer-email: Ina Rusch <rusch@iap-kborn.de>
 License: MIT License
 Project-URL: homepage, https://igit.iap-kborn.de/ibp/ibp-model.git
 Project-URL: documentation, https://ibp-model.readthedocs.io
 Project-URL: repository, https://igit.iap-kborn.de/ibp/ibp-model.git
 Project-URL: changelog, https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/CHANGELOG.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -25,19 +25,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Ionospheric Bubble Probability (IBP)
 ====================================
 
-The ionospheric bubble probability statistical model is a Swarm L2 product, named IBP_CLI. The output of the Ionospheric Bubble Probability (IBP) product is an index, that depends  on the day of year or the month of the year, geographic longitude, local time and solar flux index. 
+The ionospheric bubble probability statistical model is a Swarm L2 product, named IBP_CLI. The output of the Ionospheric Bubble Probability (IBP) product is an index, that depends on the day of year or the month of the year, geographic longitude, local time and solar flux index. 
 
 The output floating point index ranges 0-1 and characterizes the percentage probability of low latitude bubble occurence at the specified time, location and solar flux.
 
-This empirical IBP model  has been derived from magnetic observations obtained by the CHAMP and Swarm missions. The model is representative for the altitude range 350 - 500 km and low geographic latitudes of +/- 45 degree.
+This empirical IBP model has been derived from magnetic observations obtained by the CHAMP and Swarm missions. The model is representative for the altitude range 350 - 500 km and low geographic latitudes of +/- 45 degree.
 
 .. inclusion-marker-install
 
 Documentation
 -------------
 
 Detailed documentation can be found at: `<https://ibp-model.readthedocs.io>`_
@@ -68,25 +68,25 @@
 Usage
 ^^^^^
 The return value of the function *ibpmodel.calculateIBPindex()* is of type pandas.DataFrame.
 
 
 .. code-block:: python
 
-    >>> from ibpmodel import *
-    >>> calculateIBPindex(day_month=15,               # Day of Year or Month 
+    >>> import ibpmodel as ibp
+    >>> ibp.calculateIBPindex(day_month=15,           # Day of Year or Month 
                   longitude=0,                        # Longitude in degree
                   local_time=20.9,                    # Local time in hours 
                   f107=150)                           # F10.7 cm Solar Flux index
        Doy  Month  Lon    LT  F10.7     IBP
     0   15      1    0  20.9    150  0.3547
 
 .. code-block:: python
 
-    >>> calculateIBPindex(day_month=['Jan','Feb','Mar'], local_time=22)
+    >>> ibp.calculateIBPindex(day_month=['Jan','Feb','Mar'], local_time=22)
          Doy  Month  Lon  LT  F10.7     IBP
     0     15      1 -180  22    150  0.0739
     1     15      1 -175  22    150  0.0722
     2     15      1 -170  22    150  0.0717
     3     15      1 -165  22    150  0.0728
     4     15      1 -160  22    150  0.0771
     ..   ...    ...  ...  ..    ...     ...
@@ -96,24 +96,24 @@
     214   74      3  170  22    150  0.1967
     215   74      3  175  22    150  0.1943
 
    [216 rows x 6 columns]
 
 .. code-block:: python
 
-    >>> plotIBPindex(doy=349)
+    >>> ibp.plotIBPindex(doy=349)
     >>>
 
 .. image:: https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/example_plotIBP.png
     :alt: Contour plot of the IBP index for the given day
     :align: center
 
 .. code-block:: python
 
-    >>> plotButterflyData(f107=150)
+    >>> ibp.plotButterflyData(f107=150)
     >>>
 
 .. image:: https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/example_plotButterfly.png
     :alt: Contour plot of result from function ButterflyData()  
     :align: center
```

### Comparing `ibpmodel-1.2.0/README.rst` & `ibpmodel-1.2.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Ionospheric Bubble Probability (IBP)
 ====================================
 
-The ionospheric bubble probability statistical model is a Swarm L2 product, named IBP_CLI. The output of the Ionospheric Bubble Probability (IBP) product is an index, that depends  on the day of year or the month of the year, geographic longitude, local time and solar flux index. 
+The ionospheric bubble probability statistical model is a Swarm L2 product, named IBP_CLI. The output of the Ionospheric Bubble Probability (IBP) product is an index, that depends on the day of year or the month of the year, geographic longitude, local time and solar flux index. 
 
 The output floating point index ranges 0-1 and characterizes the percentage probability of low latitude bubble occurence at the specified time, location and solar flux.
 
-This empirical IBP model  has been derived from magnetic observations obtained by the CHAMP and Swarm missions. The model is representative for the altitude range 350 - 500 km and low geographic latitudes of +/- 45 degree.
+This empirical IBP model has been derived from magnetic observations obtained by the CHAMP and Swarm missions. The model is representative for the altitude range 350 - 500 km and low geographic latitudes of +/- 45 degree.
 
 .. inclusion-marker-install
 
 Documentation
 -------------
 
 Detailed documentation can be found at: `<https://ibp-model.readthedocs.io>`_
@@ -40,25 +40,25 @@
 Usage
 ^^^^^
 The return value of the function *ibpmodel.calculateIBPindex()* is of type pandas.DataFrame.
 
 
 .. code-block:: python
 
-    >>> from ibpmodel import *
-    >>> calculateIBPindex(day_month=15,               # Day of Year or Month 
+    >>> import ibpmodel as ibp
+    >>> ibp.calculateIBPindex(day_month=15,           # Day of Year or Month 
                   longitude=0,                        # Longitude in degree
                   local_time=20.9,                    # Local time in hours 
                   f107=150)                           # F10.7 cm Solar Flux index
        Doy  Month  Lon    LT  F10.7     IBP
     0   15      1    0  20.9    150  0.3547
 
 .. code-block:: python
 
-    >>> calculateIBPindex(day_month=['Jan','Feb','Mar'], local_time=22)
+    >>> ibp.calculateIBPindex(day_month=['Jan','Feb','Mar'], local_time=22)
          Doy  Month  Lon  LT  F10.7     IBP
     0     15      1 -180  22    150  0.0739
     1     15      1 -175  22    150  0.0722
     2     15      1 -170  22    150  0.0717
     3     15      1 -165  22    150  0.0728
     4     15      1 -160  22    150  0.0771
     ..   ...    ...  ...  ..    ...     ...
@@ -68,24 +68,24 @@
     214   74      3  170  22    150  0.1967
     215   74      3  175  22    150  0.1943
 
    [216 rows x 6 columns]
 
 .. code-block:: python
 
-    >>> plotIBPindex(doy=349)
+    >>> ibp.plotIBPindex(doy=349)
     >>>
 
 .. image:: https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/example_plotIBP.png
     :alt: Contour plot of the IBP index for the given day
     :align: center
 
 .. code-block:: python
 
-    >>> plotButterflyData(f107=150)
+    >>> ibp.plotButterflyData(f107=150)
     >>>
 
 .. image:: https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/example_plotButterfly.png
     :alt: Contour plot of result from function ButterflyData()  
     :align: center
```

### Comparing `ibpmodel-1.2.0/docs/Makefile` & `ibpmodel-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/docs/make.bat` & `ibpmodel-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf` & `ibpmodel-1.2.1/docs/source/_static/8thSwarmDataQualityWorkshop_slides.pdf`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/docs/source/_static/example_subplot.png` & `ibpmodel-1.2.1/docs/source/_static/example_subplot.png`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/docs/source/conf.py` & `ibpmodel-1.2.1/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 from ibpmodel import __version__ as ibp_version
 
 project = 'ibpmodel'
-copyright = '2022, Ina Wehner'
-author = 'Ina Wehner'
+copyright = '2023, Ina Rusch'
+author = 'Ina Rusch'
 version = ibp_version
 release = ibp_version
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
```

### Comparing `ibpmodel-1.2.0/docs/source/installation.rst` & `ibpmodel-1.2.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/docs/source/usage.rst` & `ibpmodel-1.2.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/pyproject.toml` & `ibpmodel-1.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 license = {text = "MIT License"}
 readme = "README.rst"
 authors = [
     {name = "Martin Rother"}
 ]
 maintainers = [
-    {name = "Ina Wehner", email = "wehner@iap-kborn.de"}
+    {name = "Ina Rusch", email = "rusch@iap-kborn.de"}
 ]
 description = "Ionospheric Bubble Probability" 
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
@@ -31,15 +31,15 @@
     "Topic :: Scientific/Engineering :: Atmospheric Science" 
 ]
 
 requires-python = ">=3.8"
 
 dependencies = [
     "numpy>=1.18",
-    "cdflib>=0.3.5",
+    "cdflib>=0.3.5, < 1",
     "scipy>=1.4",
     "pandas>=1.4",
     "matplotlib>=2.2"
 ]
 
 [project.urls]
 homepage = "https://igit.iap-kborn.de/ibp/ibp-model.git"
```

### Comparing `ibpmodel-1.2.0/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf` & `ibpmodel-1.2.1/src/ibpmodel/SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf`

 * *Files identical despite different names*

### Comparing `ibpmodel-1.2.0/src/ibpmodel/ibpcalc.py` & `ibpmodel-1.2.1/src/ibpmodel/ibpcalc.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         
     Returns
     -------
     dict
         Contains the content of the CDF file.
 
     """
-    
+
     if file == None:
         basepath = os.path.dirname(__file__)
         file = os.path.abspath(os.path.join(basepath,'SW_OPER_IBP_CLI_2__00000000T000000_99999999T999999_0002.cdf'))
     
     data = {}
     cdf = cdflib.CDF(file)
 
@@ -629,16 +629,16 @@
     """
 
     # CHECKS:
 
     if np.any( (local_time < -6.0) | (local_time >  24.0) ):
         raise ValueError("Local time(s) or hour to midnight out of range!")
         
-    if np.any( (f107       <  0.0) | (f107       > 200.0) ):
-        raise ValueError("F10.7 parameter(s) out of valid range!")
+    #if np.any( (f107       <  0.0) | (f107       > 200.0) ):
+    #    raise ValueError("F10.7 parameter(s) out of valid range!")
 
     # Normalize time selected
     
     (day_of_year, month) = align_time_of_year(day_of_year, month)
     
     # Extraction
```

### Comparing `ibpmodel-1.2.0/src/ibpmodel/ibpforward.py` & `ibpmodel-1.2.1/src/ibpmodel/ibpforward.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,32 +3,33 @@
 """
 from .ibpcalc import *
 import numpy as np
 import pandas as pd
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import matplotlib.ticker as mticker
+import warnings
 
 def calculateIBPindex(day_month=0, longitude=list(range(-180,180,5)), local_time=np.arange(-6,6.1,0.1), f107=150, coeff=None):
     '''Calculates the Ionospheric Bubble propability index based on the input parameters. 
     Returns a *pandas.DataFrame* with input parameters and IBP index. 
 
     Parameters
     ----------
     day_month : int or str or list, optional
         Day of year (*int*) or the month of the year (*str*). 
         *int*: Day of the year, ``0 <= doy <= 365``. The value 0 means it should be calculated based on every month.
         *str*: Abbreviated month name. ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
         The default is 0.
     longitude : int or list of ints, optional
-        The geographical longitude(s), ``-180 <= longitude <= 180``. The default is `list(range(-180,181,5))`.
+        The geographical longitude(s), ``-180 <= longitude <= 180``. The default is `list(range(-180,180,5))`.
     local_time : int or float or list, optional
         The local time, ``-6.0 <= local_time <= 24``. The default is `np.arange(-6,6.1,0.1)`.
     f107 : int or float or list, optional
-        The Solar Radio Flux (F10.7 index), ``0.0 <= f107 <= 200.0``. The default is 150.
+        The Solar Radio Flux (F10.7 index), ``80.0 <= f107``. The default is 150.
     coeff : None or str, optional
         Name of the coefficient file.
         The default is None.
 
     Returns
     -------
     df : pandas.DataFrame
@@ -47,16 +48,18 @@
     longitude_range = range(-180,181)
     longitude = checkParameter(longitude, longitude_range).astype(int)
     longitude[longitude == 180] = -180
 
     local_time_range = range(-6,25)
     local_time = checkParameter(local_time, local_time_range) 
 
-    f107_range = range(0,201)
+    f107_range = range(80,1000)
     f107 = checkParameter(f107, f107_range)
+    if max(f107) > 200:
+        warnings.warn('You are using values for Solar Radio Flux greater than 200sfu. \nPlease note: The model is not designed for these values.')
 
     data = read_model_file(coeff)
 
     parts = tiler(day_of_year, longitude, local_time, f107)
 
     for i, c in enumerate(['Doy', 'Lon', 'LT', 'F10.7']):
         df[c] = parts[i]
@@ -103,27 +106,28 @@
     result = compute_probability_exp(
         day_of_year,month,longitude,local_time,f107,data)
 
     out_data = np.array(tile_aggregate(result,month_range,longitude_range,local_time_range)).transpose()
     
     return out_data
     
-def getcolorbar(cmap, level=np.arange(0.0, 1.0, 0.05)):
+def getcolorbar(cmap, level=np.arange(0.0, 1.05, 0.05)):
     '''Applies level to colormap.
     
     Parameters
     ----------
     cmap : matplotlib.colors.Colormap
 
     level : array-like
     
     Returns
     -------
     matplotlib.cm.ScalarMappable
     '''
+
     norm = mpl.colors.BoundaryNorm(level, cmap.N)
     return mpl.cm.ScalarMappable(norm=norm, cmap=cmap)
  
 def setcolorbar(scalarmap, fig, ax, **kwargs):
     '''Sets colorbar to figure on the specified axis.
 
     Parameters
@@ -171,15 +175,15 @@
 
     Parameters
     ----------
     doy : int or str
         Day of year (*int*) or the month of the year (*str*). 
         *int*: Day of the year, ``0 <= doy <= 365``. The value 0 means it should be calculated based on every month.
         *str*: Abbreviated month name. ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul', 'Aug', 'Sep', 'Oct', 'Nov', 'Dec']
-    f107 : int, optional
+    f107 : int or float, optional
         The Solar Radio Flux (F10.7 index). The default is 150.
     ax : matplotlib.axes, optional
         The Axes object in which the plot will be drawn. The default is None.
     coeff : str, optional
         Path of coefficient file. The default is None.
     cmap : str or Colormap, optional
         The colormap instance or registered colormap name to use. The default is 'coolwarm'.
@@ -212,15 +216,15 @@
         fig, ax = plt.subplots(figsize = (9, 4))
         pltshow = True
     else:
         pltshow = False
     
     cmap = checkcmap(cmap)
 
-    levels = np.arange(0.0, 1.0, 0.05)
+    levels = np.arange(0.0, 1.05, 0.05)
     scalarmap = getcolorbar(cmap, levels)
     
     ax.contourf(x, y, z, levels=levels, cmap=cmap, **kwargs)
     ax.contour(x, y, z, levels=levels, colors=colors, linewidths=linewidths, **kwargs)
 
     ticks_loc = ax.get_yticks().tolist()
     ax.yaxis.set_major_locator(mticker.FixedLocator(ticks_loc))
@@ -239,15 +243,15 @@
         return (ax, scalarmap)
 
 def plotButterflyData(f107=150, ax=None, coeff=None, cmap='plasma_r', colors='#999900', linewidths=0.2, **kwargs):
     '''Create a contour plot of the result from function butterflyData(). Default colormap is 'plasma_r'. 
 
     Parameters
     ----------
-    f107 : int, optional
+    f107 : int or float, optional
         The Solar Radio Flux (F10.7 index). The default is 150.
     ax : matplotlib.axes, optional
         The Axes object in which the plot will be drawn. The default is None.
     coeff : str, optional
         Path of coefficient file. The default is None.
     cmap : str or Colormap, optional
         The colormap instance or registered colormap name to use. The default is 'plasma_r'.
@@ -263,15 +267,15 @@
     '''
     d = butterflyData(f107, coeff)
     
     y = np.transpose(np.reshape(d[:, 0], (12, 72)))
     x = np.transpose(np.reshape(d[:, 1], (12, 72)))
     z = np.transpose(np.reshape(d[:, 2], (12, 72)))
 
-    l = np.arange(0.0, 0.8, 0.05)
+    l = np.arange(0.0, 0.85, 0.05)
 
     if ax == None:
         fig, ax = plt.subplots(figsize = (6.2, 5.0))
         pltshow = True
     else:
         pltshow = False
```

### Comparing `ibpmodel-1.2.0/src/ibpmodel.egg-info/PKG-INFO` & `ibpmodel-1.2.1/src/ibpmodel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ibpmodel
-Version: 1.2.0
+Version: 1.2.1
 Summary: Ionospheric Bubble Probability
 Author: Martin Rother
-Maintainer-email: Ina Wehner <wehner@iap-kborn.de>
+Maintainer-email: Ina Rusch <rusch@iap-kborn.de>
 License: MIT License
 Project-URL: homepage, https://igit.iap-kborn.de/ibp/ibp-model.git
 Project-URL: documentation, https://ibp-model.readthedocs.io
 Project-URL: repository, https://igit.iap-kborn.de/ibp/ibp-model.git
 Project-URL: changelog, https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/CHANGELOG.rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -25,19 +25,19 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Ionospheric Bubble Probability (IBP)
 ====================================
 
-The ionospheric bubble probability statistical model is a Swarm L2 product, named IBP_CLI. The output of the Ionospheric Bubble Probability (IBP) product is an index, that depends  on the day of year or the month of the year, geographic longitude, local time and solar flux index. 
+The ionospheric bubble probability statistical model is a Swarm L2 product, named IBP_CLI. The output of the Ionospheric Bubble Probability (IBP) product is an index, that depends on the day of year or the month of the year, geographic longitude, local time and solar flux index. 
 
 The output floating point index ranges 0-1 and characterizes the percentage probability of low latitude bubble occurence at the specified time, location and solar flux.
 
-This empirical IBP model  has been derived from magnetic observations obtained by the CHAMP and Swarm missions. The model is representative for the altitude range 350 - 500 km and low geographic latitudes of +/- 45 degree.
+This empirical IBP model has been derived from magnetic observations obtained by the CHAMP and Swarm missions. The model is representative for the altitude range 350 - 500 km and low geographic latitudes of +/- 45 degree.
 
 .. inclusion-marker-install
 
 Documentation
 -------------
 
 Detailed documentation can be found at: `<https://ibp-model.readthedocs.io>`_
@@ -68,25 +68,25 @@
 Usage
 ^^^^^
 The return value of the function *ibpmodel.calculateIBPindex()* is of type pandas.DataFrame.
 
 
 .. code-block:: python
 
-    >>> from ibpmodel import *
-    >>> calculateIBPindex(day_month=15,               # Day of Year or Month 
+    >>> import ibpmodel as ibp
+    >>> ibp.calculateIBPindex(day_month=15,           # Day of Year or Month 
                   longitude=0,                        # Longitude in degree
                   local_time=20.9,                    # Local time in hours 
                   f107=150)                           # F10.7 cm Solar Flux index
        Doy  Month  Lon    LT  F10.7     IBP
     0   15      1    0  20.9    150  0.3547
 
 .. code-block:: python
 
-    >>> calculateIBPindex(day_month=['Jan','Feb','Mar'], local_time=22)
+    >>> ibp.calculateIBPindex(day_month=['Jan','Feb','Mar'], local_time=22)
          Doy  Month  Lon  LT  F10.7     IBP
     0     15      1 -180  22    150  0.0739
     1     15      1 -175  22    150  0.0722
     2     15      1 -170  22    150  0.0717
     3     15      1 -165  22    150  0.0728
     4     15      1 -160  22    150  0.0771
     ..   ...    ...  ...  ..    ...     ...
@@ -96,24 +96,24 @@
     214   74      3  170  22    150  0.1967
     215   74      3  175  22    150  0.1943
 
    [216 rows x 6 columns]
 
 .. code-block:: python
 
-    >>> plotIBPindex(doy=349)
+    >>> ibp.plotIBPindex(doy=349)
     >>>
 
 .. image:: https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/example_plotIBP.png
     :alt: Contour plot of the IBP index for the given day
     :align: center
 
 .. code-block:: python
 
-    >>> plotButterflyData(f107=150)
+    >>> ibp.plotButterflyData(f107=150)
     >>>
 
 .. image:: https://igit.iap-kborn.de/ibp/ibp-model/-/raw/main/docs/source/_static/example_plotButterfly.png
     :alt: Contour plot of result from function ButterflyData()  
     :align: center
```

### Comparing `ibpmodel-1.2.0/src/ibpmodel.egg-info/SOURCES.txt` & `ibpmodel-1.2.1/src/ibpmodel.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .readthedocs.yml
 CHANGELOG.rst
 LICENSE
 README.rst
 pyproject.toml
+requirements-dev.txt
 requirements.txt
 docs/Makefile
 docs/make.bat
 docs/source/changelog.rst
 docs/source/conf.py
 docs/source/ibpmodel.rst
 docs/source/index.rst
@@ -25,8 +26,9 @@
 src/ibpmodel/ibpcalc.py
 src/ibpmodel/ibpforward.py
 src/ibpmodel.egg-info/PKG-INFO
 src/ibpmodel.egg-info/SOURCES.txt
 src/ibpmodel.egg-info/dependency_links.txt
 src/ibpmodel.egg-info/requires.txt
 src/ibpmodel.egg-info/top_level.txt
+template/IBP-VirES.ipynb
 template/IBP_CLI_2_bubble-probability.ipynb
```

### Comparing `ibpmodel-1.2.0/template/IBP_CLI_2_bubble-probability.ipynb` & `ibpmodel-1.2.1/template/IBP_CLI_2_bubble-probability.ipynb`

 * *Files identical despite different names*

