# Comparing `tmp/netzip-0.3.0.tar.gz` & `tmp/netzip-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netzip-0.3.0.tar", last modified: Tue Jun 20 15:40:57 2023, max compression
+gzip compressed data, was "netzip-0.3.1.tar", last modified: Thu Jun 22 09:38:14 2023, max compression
```

## Comparing `netzip-0.3.0.tar` & `netzip-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.508407 netzip-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 15:40:21.000000 netzip-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 15:40:57.508407 netzip-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-20 15:40:21.000000 netzip-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 15:40:21.000000 netzip-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:40:57.508407 netzip-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.504407 netzip-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.504407 netzip-0.3.0/src/netzip/
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-20 15:40:21.000000 netzip-0.3.0/src/netzip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.508407 netzip-0.3.0/src/netzip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 15:40:57.000000 netzip-0.3.0/src/netzip.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:40:57.508407 netzip-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-20 15:40:21.000000 netzip-0.3.0/tests/test_netzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:14.525377 netzip-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 09:37:45.000000 netzip-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-22 09:38:14.521377 netzip-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 09:37:45.000000 netzip-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-22 09:37:45.000000 netzip-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:38:14.525377 netzip-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:14.521377 netzip-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:14.521377 netzip-0.3.1/src/netzip/
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-22 09:37:45.000000 netzip-0.3.1/src/netzip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:14.521377 netzip-0.3.1/src/netzip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-22 09:38:14.000000 netzip-0.3.1/src/netzip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-22 09:38:14.000000 netzip-0.3.1/src/netzip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:38:14.000000 netzip-0.3.1/src/netzip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 09:38:14.000000 netzip-0.3.1/src/netzip.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:38:14.521377 netzip-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-22 09:37:45.000000 netzip-0.3.1/tests/test_netzip.py
```

### Comparing `netzip-0.3.0/LICENSE.txt` & `netzip-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netzip-0.3.0/pyproject.toml` & `netzip-0.3.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netzip"
-version = "0.3.0"
+version = "0.3.1"
 authors = [{ name = "Emil Melnikov", email = "emilmelnikov@gmail.com" }]
 description = "ZIP file reader optimized for network access"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
 
 [project.urls]
-"Homepage" = "https://github.com/emilmelnikov/netzip"
-"Bug Tracker" = "https://github.com/emilmelnikov/netzip/issues"
-"Source" = "https://github.com/emilmelnikov/netzip"
+"Homepage" = "https://github.com/ilastik/netzip"
+"Bug Tracker" = "https://github.com/ilastik/netzip/issues"
+"Source" = "https://github.com/ilastik/netzip"
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.pytest.ini_options]
 addopts = "-rfEP --quiet"
 testpaths = ["tests"]
```

### Comparing `netzip-0.3.0/src/netzip/__init__.py` & `netzip-0.3.1/src/netzip/__init__.py`

 * *Files identical despite different names*

### Comparing `netzip-0.3.0/tests/test_netzip.py` & `netzip-0.3.1/tests/test_netzip.py`

 * *Files identical despite different names*

