# Comparing `tmp/lincot-1.0.0.tar.gz` & `tmp/lincot-1.0.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincot-1.0.0.tar", last modified: Wed Jun 21 22:15:03 2023, max compression
+gzip compressed data, was "lincot-1.0.2b2.tar", last modified: Thu Jun 22 05:12:42 2023, max compression
```

## Comparing `lincot-1.0.0.tar` & `lincot-1.0.2b2.tar`

### file list

```diff
@@ -1,22 +1,20 @@
-drwxr-xr-x   0 gba        (501) staff       (20)        0 2023-06-21 22:15:03.793496 lincot-1.0.0/
--rw-r--r--   0 gba        (501) staff       (20)      557 2023-06-15 05:55:45.000000 lincot-1.0.0/LICENSE
--rw-r--r--   0 gba        (501) staff       (20)       76 2023-06-15 05:12:50.000000 lincot-1.0.0/MANIFEST.in
--rw-r--r--   0 gba        (501) staff       (20)     4196 2023-06-21 22:15:03.793883 lincot-1.0.0/PKG-INFO
--rw-r--r--   0 gba        (501) staff       (20)     2764 2023-06-15 06:28:29.000000 lincot-1.0.0/README.rst
-drwxr-xr-x   0 gba        (501) staff       (20)        0 2023-06-21 22:15:03.787705 lincot-1.0.0/lincot/
--rw-r--r--   0 gba        (501) staff       (20)     1113 2023-06-21 22:11:21.000000 lincot-1.0.0/lincot/__init__.py
--rw-r--r--   0 gba        (501) staff       (20)     2500 2023-06-21 22:11:15.000000 lincot-1.0.0/lincot/classes.py
--rw-r--r--   0 gba        (501) staff       (20)      960 2023-06-15 06:14:14.000000 lincot-1.0.0/lincot/commands.py
--rw-r--r--   0 gba        (501) staff       (20)      962 2023-06-21 22:11:43.000000 lincot-1.0.0/lincot/constants.py
--rw-r--r--   0 gba        (501) staff       (20)     4483 2023-06-21 22:12:12.000000 lincot-1.0.0/lincot/functions.py
-drwxr-xr-x   0 gba        (501) staff       (20)        0 2023-06-21 22:15:03.791994 lincot-1.0.0/lincot.egg-info/
--rw-r--r--   0 gba        (501) staff       (20)     4196 2023-06-21 22:15:03.000000 lincot-1.0.0/lincot.egg-info/PKG-INFO
--rw-r--r--   0 gba        (501) staff       (20)      351 2023-06-21 22:15:03.000000 lincot-1.0.0/lincot.egg-info/SOURCES.txt
--rw-r--r--   0 gba        (501) staff       (20)        1 2023-06-21 22:15:03.000000 lincot-1.0.0/lincot.egg-info/dependency_links.txt
--rw-r--r--   0 gba        (501) staff       (20)       48 2023-06-21 22:15:03.000000 lincot-1.0.0/lincot.egg-info/entry_points.txt
--rw-r--r--   0 gba        (501) staff       (20)      113 2023-06-21 22:15:03.000000 lincot-1.0.0/lincot.egg-info/requires.txt
--rw-r--r--   0 gba        (501) staff       (20)        7 2023-06-21 22:15:03.000000 lincot-1.0.0/lincot.egg-info/top_level.txt
--rw-r--r--   0 gba        (501) staff       (20)     1571 2023-06-21 22:15:03.796058 lincot-1.0.0/setup.cfg
--rw-r--r--   0 gba        (501) staff       (20)      769 2023-06-21 22:11:04.000000 lincot-1.0.0/setup.py
-drwxr-xr-x   0 gba        (501) staff       (20)        0 2023-06-21 22:15:03.792769 lincot-1.0.0/tests/
--rw-r--r--   0 gba        (501) staff       (20)     2752 2023-06-21 22:12:44.000000 lincot-1.0.0/tests/test_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:12:42.333452 lincot-1.0.2b2/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 05:12:26.000000 lincot-1.0.2b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 05:12:26.000000 lincot-1.0.2b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:12:42.333452 lincot-1.0.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-06-22 05:12:26.000000 lincot-1.0.2b2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:12:42.333452 lincot-1.0.2b2/lincot/
+-rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:12:42.333452 lincot-1.0.2b2/lincot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-22 05:12:42.333452 lincot-1.0.2b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-22 05:12:26.000000 lincot-1.0.2b2/setup.py
```

### Comparing `lincot-1.0.0/LICENSE` & `lincot-1.0.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `lincot-1.0.0/PKG-INFO` & `lincot-1.0.2b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincot
-Version: 1.0.0
+Version: 1.0.2b2
 Summary: LINCOT: Linux GPS to TAK Gateway.
 Home-page: https://github.com/snstac/lincot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/lincot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/lincot/issues
```

### Comparing `lincot-1.0.0/README.rst` & `lincot-1.0.2b2/README.rst`

 * *Files identical despite different names*

### Comparing `lincot-1.0.0/lincot/__init__.py` & `lincot-1.0.2b2/lincot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     DEFAULT_GPS_INFO_CMD,
 )
 
 from .functions import gpspipe_to_cot, create_tasks  # NOQA
 
 from .classes import LincotWorker  # NOQA
 
-__version__ = "1.0.0"
+__version__ = "1.0.2-beta2"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
```

### Comparing `lincot-1.0.0/lincot/classes.py` & `lincot-1.0.2b2/lincot/classes.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.0/lincot/commands.py` & `lincot-1.0.2b2/lincot/commands.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.0/lincot/constants.py` & `lincot-1.0.2b2/lincot/constants.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.0/lincot/functions.py` & `lincot-1.0.2b2/lincot/functions.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.0/lincot.egg-info/PKG-INFO` & `lincot-1.0.2b2/lincot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincot
-Version: 1.0.0
+Version: 1.0.2b2
 Summary: LINCOT: Linux GPS to TAK Gateway.
 Home-page: https://github.com/snstac/lincot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/lincot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/lincot/issues
```

### Comparing `lincot-1.0.0/setup.cfg` & `lincot-1.0.2b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `lincot-1.0.0/setup.py` & `lincot-1.0.2b2/setup.py`

 * *Files identical despite different names*

