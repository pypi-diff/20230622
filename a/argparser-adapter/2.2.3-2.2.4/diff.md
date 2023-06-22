# Comparing `tmp/argparser_adapter-2.2.3.tar.gz` & `tmp/argparser_adapter-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argparser_adapter-2.2.3.tar", last modified: Thu Feb  9 13:38:01 2023, max compression
+gzip compressed data, was "argparser_adapter-2.2.4.tar", last modified: Thu Jun 22 12:17:36 2023, max compression
```

## Comparing `argparser_adapter-2.2.3.tar` & `argparser_adapter-2.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-02-09 13:38:01.005593 argparser_adapter-2.2.3/
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1289 2023-01-17 21:07:11.000000 argparser_adapter-2.2.3/LICENSE
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     5853 2023-02-09 13:38:01.005593 argparser_adapter-2.2.3/PKG-INFO
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     5555 2023-02-09 13:10:05.000000 argparser_adapter-2.2.3/README.rst
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)       82 2023-01-17 21:11:42.000000 argparser_adapter-2.2.3/pyproject.toml
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      591 2023-02-09 13:38:01.005593 argparser_adapter-2.2.3/setup.cfg
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-02-09 13:38:01.005593 argparser_adapter-2.2.3/src/
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-02-09 13:38:01.005593 argparser_adapter-2.2.3/src/argparser_adapter/
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      162 2023-02-09 13:37:51.000000 argparser_adapter-2.2.3/src/argparser_adapter/__init__.py
--rwxr-xr-x   0 gweatherby (16342) uconn_health (30059)     8337 2023-02-09 13:37:22.000000 argparser_adapter-2.2.3/src/argparser_adapter/implementation.py
-drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-02-09 13:38:01.005593 argparser_adapter-2.2.3/src/argparser_adapter.egg-info/
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)     5853 2023-02-09 13:38:01.000000 argparser_adapter-2.2.3/src/argparser_adapter.egg-info/PKG-INFO
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)      297 2023-02-09 13:38:01.000000 argparser_adapter-2.2.3/src/argparser_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)        1 2023-02-09 13:38:01.000000 argparser_adapter-2.2.3/src/argparser_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 gweatherby (16342) uconn_health (30059)       18 2023-02-09 13:38:01.000000 argparser_adapter-2.2.3/src/argparser_adapter.egg-info/top_level.txt
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-06-22 12:17:36.925124 argparser_adapter-2.2.4/
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     1289 2023-01-17 21:07:11.000000 argparser_adapter-2.2.4/LICENSE
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     5857 2023-06-22 12:17:36.925124 argparser_adapter-2.2.4/PKG-INFO
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     5555 2023-02-09 13:10:05.000000 argparser_adapter-2.2.4/README.rst
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)       82 2023-01-17 21:11:42.000000 argparser_adapter-2.2.4/pyproject.toml
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      595 2023-06-22 12:17:36.925124 argparser_adapter-2.2.4/setup.cfg
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-06-22 12:17:36.921123 argparser_adapter-2.2.4/src/
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-06-22 12:17:36.925124 argparser_adapter-2.2.4/src/argparser_adapter/
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      162 2023-06-22 12:14:00.000000 argparser_adapter-2.2.4/src/argparser_adapter/__init__.py
+-rwxr-xr-x   0 gweatherby (16342) uconn_health (30059)     8337 2023-02-09 13:37:22.000000 argparser_adapter-2.2.4/src/argparser_adapter/implementation.py
+drwxr-xr-x   0 gweatherby (16342) uconn_health (30059)        0 2023-06-22 12:17:36.925124 argparser_adapter-2.2.4/src/argparser_adapter.egg-info/
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)     5857 2023-06-22 12:17:36.000000 argparser_adapter-2.2.4/src/argparser_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)      297 2023-06-22 12:17:36.000000 argparser_adapter-2.2.4/src/argparser_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)        1 2023-06-22 12:17:36.000000 argparser_adapter-2.2.4/src/argparser_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 gweatherby (16342) uconn_health (30059)       18 2023-06-22 12:17:36.000000 argparser_adapter-2.2.4/src/argparser_adapter.egg-info/top_level.txt
```

### Comparing `argparser_adapter-2.2.3/LICENSE` & `argparser_adapter-2.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `argparser_adapter-2.2.3/PKG-INFO` & `argparser_adapter-2.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: argparser_adapter
-Version: 2.2.3
-Summary: Manage python packages on Ubuntu20 systems
+Version: 2.2.4
+Summary: Automatically add object methods to argparser.
 Home-page: https://github.com/NMRbox/argparser_adapter
 Author: Gerard
 Author-email: gweatherby@uchc.edu
 License: MIT license
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

### Comparing `argparser_adapter-2.2.3/README.rst` & `argparser_adapter-2.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `argparser_adapter-2.2.3/setup.cfg` & `argparser_adapter-2.2.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = argparser_adapter
 version = attr: argparser_adapter.__version__
 author = Gerard
 author_email = gweatherby@uchc.edu
-description = Manage python packages on Ubuntu20 systems
+description = Automatically add object methods to argparser.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 license = MIT license
 url = https://github.com/NMRbox/argparser_adapter
 Funding = https://nmrhub.org
 python_requires > = 3.7
 classifers =
```

### Comparing `argparser_adapter-2.2.3/src/argparser_adapter/implementation.py` & `argparser_adapter-2.2.4/src/argparser_adapter/implementation.py`

 * *Files identical despite different names*

### Comparing `argparser_adapter-2.2.3/src/argparser_adapter.egg-info/PKG-INFO` & `argparser_adapter-2.2.4/src/argparser_adapter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: argparser-adapter
-Version: 2.2.3
-Summary: Manage python packages on Ubuntu20 systems
+Version: 2.2.4
+Summary: Automatically add object methods to argparser.
 Home-page: https://github.com/NMRbox/argparser_adapter
 Author: Gerard
 Author-email: gweatherby@uchc.edu
 License: MIT license
 Description-Content-Type: text/x-rst
 License-File: LICENSE
```

