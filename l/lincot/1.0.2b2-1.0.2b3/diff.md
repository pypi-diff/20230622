# Comparing `tmp/lincot-1.0.2b2.tar.gz` & `tmp/lincot-1.0.2b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincot-1.0.2b2.tar", last modified: Thu Jun 22 05:12:42 2023, max compression
+gzip compressed data, was "lincot-1.0.2b3.tar", last modified: Thu Jun 22 05:23:06 2023, max compression
```

## Comparing `lincot-1.0.2b2.tar` & `lincot-1.0.2b3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:12:42.333452 lincot-1.0.2b2/
--rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 05:12:26.000000 lincot-1.0.2b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 05:12:26.000000 lincot-1.0.2b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:12:42.333452 lincot-1.0.2b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-06-22 05:12:26.000000 lincot-1.0.2b2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:12:42.333452 lincot-1.0.2b2/lincot/
--rw-r--r--   0 runner    (1001) docker     (122)     1119 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      960 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/commands.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-06-22 05:12:26.000000 lincot-1.0.2b2/lincot/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:12:42.333452 lincot-1.0.2b2/lincot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-22 05:12:42.000000 lincot-1.0.2b2/lincot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-22 05:12:42.333452 lincot-1.0.2b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-22 05:12:26.000000 lincot-1.0.2b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:23:06.432346 lincot-1.0.2b3/
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-22 05:22:55.000000 lincot-1.0.2b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 05:22:55.000000 lincot-1.0.2b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:23:06.432346 lincot-1.0.2b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-06-22 05:22:55.000000 lincot-1.0.2b3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:23:06.432346 lincot-1.0.2b3/lincot/
+-rw-r--r--   0 runner    (1001) docker     (122)     1331 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2500 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      960 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/commands.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4483 2023-06-22 05:22:55.000000 lincot-1.0.2b3/lincot/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 05:23:06.432346 lincot-1.0.2b3/lincot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4198 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      327 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-22 05:23:06.000000 lincot-1.0.2b3/lincot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1571 2023-06-22 05:23:06.432346 lincot-1.0.2b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      769 2023-06-22 05:22:55.000000 lincot-1.0.2b3/setup.py
```

### Comparing `lincot-1.0.2b2/LICENSE` & `lincot-1.0.2b3/LICENSE`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b2/PKG-INFO` & `lincot-1.0.2b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincot
-Version: 1.0.2b2
+Version: 1.0.2b3
 Summary: LINCOT: Linux GPS to TAK Gateway.
 Home-page: https://github.com/snstac/lincot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/lincot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/lincot/issues
```

### Comparing `lincot-1.0.2b2/README.rst` & `lincot-1.0.2b3/README.rst`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b2/lincot/__init__.py` & `lincot-1.0.2b3/lincot/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,22 +15,28 @@
 #
 
 """LINCOT: Linux GPS to TAK Gateway.
 
 :source: <https://github.com/snstac/lincot>
 """
 
-from .constants import (
-    DEFAULT_COT_TYPE,
-    DEFAULT_COT_STALE,
-    DEFAULT_POLL_INTERVAL,
-    DEFAULT_GPS_INFO_CMD,
-)
-
-from .functions import gpspipe_to_cot, create_tasks  # NOQA
-
-from .classes import LincotWorker  # NOQA
-
-__version__ = "1.0.2-beta2"
+__version__ = "1.0.2-beta3"
 __author__ = "Greg Albrecht <gba@snstac.com>"
 __copyright__ = "Copyright 2023 Sensors & Signals LLC"
 __license__ = "Apache License, Version 2.0"
+
+
+# Python 3.6 test/build work-around:
+try:
+    from .constants import (
+        DEFAULT_COT_TYPE,
+        DEFAULT_COT_STALE,
+        DEFAULT_POLL_INTERVAL,
+        DEFAULT_GPS_INFO_CMD,
+    )
+
+    from .functions import gpspipe_to_cot, create_tasks  # NOQA
+
+    from .classes import LincotWorker  # NOQA
+except ImportError:
+    import warnings
+    warnings.warn("Unable to import required modules, ignoring (Python 3.6 build work-around).")
```

### Comparing `lincot-1.0.2b2/lincot/classes.py` & `lincot-1.0.2b3/lincot/classes.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b2/lincot/commands.py` & `lincot-1.0.2b3/lincot/commands.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b2/lincot/constants.py` & `lincot-1.0.2b3/lincot/constants.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b2/lincot/functions.py` & `lincot-1.0.2b3/lincot/functions.py`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b2/lincot.egg-info/PKG-INFO` & `lincot-1.0.2b3/lincot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincot
-Version: 1.0.2b2
+Version: 1.0.2b3
 Summary: LINCOT: Linux GPS to TAK Gateway.
 Home-page: https://github.com/snstac/lincot
 Maintainer: Greg Albrecht <oss@undef.net>
 Maintainer-email: oss@undef.net
 License: Apache 2.0
 Project-URL: CI: GitHub Actions, https://github.com/snstac/lincot/actions
 Project-URL: GitHub: issues, https://github.com/snstac/lincot/issues
```

### Comparing `lincot-1.0.2b2/setup.cfg` & `lincot-1.0.2b3/setup.cfg`

 * *Files identical despite different names*

### Comparing `lincot-1.0.2b2/setup.py` & `lincot-1.0.2b3/setup.py`

 * *Files identical despite different names*

