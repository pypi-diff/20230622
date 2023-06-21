# Comparing `tmp/featurelayers-1.1.6.tar.gz` & `tmp/featurelayers-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.1.6.tar", last modified: Wed Jun 21 19:13:54 2023, max compression
+gzip compressed data, was "featurelayers-1.1.7.tar", last modified: Wed Jun 21 22:06:22 2023, max compression
```

## Comparing `featurelayers-1.1.6.tar` & `featurelayers-1.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:13:54.721624 featurelayers-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 19:13:54.721624 featurelayers-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:13:37.000000 featurelayers-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:13:54.721624 featurelayers-1.1.6/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 19:13:37.000000 featurelayers-1.1.6/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:13:37.000000 featurelayers-1.1.6/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 19:13:37.000000 featurelayers-1.1.6/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:13:54.721624 featurelayers-1.1.6/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 19:13:37.000000 featurelayers-1.1.6/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 19:13:37.000000 featurelayers-1.1.6/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:13:54.721624 featurelayers-1.1.6/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-21 19:13:54.000000 featurelayers-1.1.6/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 19:13:54.000000 featurelayers-1.1.6/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:13:54.000000 featurelayers-1.1.6/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 19:13:54.000000 featurelayers-1.1.6/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 19:13:54.000000 featurelayers-1.1.6/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:13:54.721624 featurelayers-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-21 19:13:37.000000 featurelayers-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:06:22.562602 featurelayers-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 22:06:22.562602 featurelayers-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:06:04.000000 featurelayers-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:06:22.562602 featurelayers-1.1.7/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 22:06:04.000000 featurelayers-1.1.7/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 22:06:04.000000 featurelayers-1.1.7/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 22:06:04.000000 featurelayers-1.1.7/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:06:22.562602 featurelayers-1.1.7/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-21 22:06:04.000000 featurelayers-1.1.7/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 22:06:04.000000 featurelayers-1.1.7/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:06:22.562602 featurelayers-1.1.7/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 22:06:22.000000 featurelayers-1.1.7/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-21 22:06:22.000000 featurelayers-1.1.7/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:06:22.000000 featurelayers-1.1.7/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-21 22:06:22.000000 featurelayers-1.1.7/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 22:06:22.000000 featurelayers-1.1.7/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:06:22.562602 featurelayers-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-21 22:06:04.000000 featurelayers-1.1.7/setup.py
```

### Comparing `featurelayers-1.1.6/featurelayers/layers/LBC.py` & `featurelayers-1.1.7/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

