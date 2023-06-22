# Comparing `tmp/featurelayers-1.1.8.tar.gz` & `tmp/featurelayers-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.1.8.tar", last modified: Wed Jun 21 23:53:51 2023, max compression
+gzip compressed data, was "featurelayers-1.1.9.tar", last modified: Thu Jun 22 01:00:26 2023, max compression
```

## Comparing `featurelayers-1.1.8.tar` & `featurelayers-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:53:51.183989 featurelayers-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 23:53:51.183989 featurelayers-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:53:34.000000 featurelayers-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:53:51.183989 featurelayers-1.1.8/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 23:53:34.000000 featurelayers-1.1.8/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 23:53:34.000000 featurelayers-1.1.8/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 23:53:34.000000 featurelayers-1.1.8/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:53:51.183989 featurelayers-1.1.8/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 23:53:34.000000 featurelayers-1.1.8/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 23:53:34.000000 featurelayers-1.1.8/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:53:51.183989 featurelayers-1.1.8/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 23:53:51.000000 featurelayers-1.1.8/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 23:53:51.000000 featurelayers-1.1.8/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:53:51.000000 featurelayers-1.1.8/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 23:53:51.000000 featurelayers-1.1.8/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 23:53:51.000000 featurelayers-1.1.8/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:53:51.183989 featurelayers-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 23:53:34.000000 featurelayers-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:00:26.536322 featurelayers-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 01:00:26.536322 featurelayers-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 01:00:06.000000 featurelayers-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:00:26.536322 featurelayers-1.1.9/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:00:06.000000 featurelayers-1.1.9/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 01:00:06.000000 featurelayers-1.1.9/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 01:00:06.000000 featurelayers-1.1.9/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:00:26.536322 featurelayers-1.1.9/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-22 01:00:06.000000 featurelayers-1.1.9/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 01:00:06.000000 featurelayers-1.1.9/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:00:26.536322 featurelayers-1.1.9/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 01:00:26.000000 featurelayers-1.1.9/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 01:00:26.000000 featurelayers-1.1.9/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:00:26.000000 featurelayers-1.1.9/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 01:00:26.000000 featurelayers-1.1.9/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 01:00:26.000000 featurelayers-1.1.9/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:00:26.536322 featurelayers-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 01:00:06.000000 featurelayers-1.1.9/setup.py
```

### Comparing `featurelayers-1.1.8/featurelayers/layers/LBC.py` & `featurelayers-1.1.9/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.1.8/setup.py` & `featurelayers-1.1.9/setup.py`

 * *Files identical despite different names*

