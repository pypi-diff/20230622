# Comparing `tmp/syscoloringspkgs-1.0.0.tar.gz` & `tmp/syscoloringspkgs-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscoloringspkgs-1.0.0.tar", last modified: Thu Jun 22 20:25:15 2023, max compression
+gzip compressed data, was "syscoloringspkgs-1.1.0.tar", last modified: Thu Jun 22 20:27:21 2023, max compression
```

## Comparing `syscoloringspkgs-1.0.0.tar` & `syscoloringspkgs-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:25:15.499486 syscoloringspkgs-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-22 20:25:15.495486 syscoloringspkgs-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:25:15.499486 syscoloringspkgs-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      562 2023-06-22 20:25:14.000000 syscoloringspkgs-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:25:15.495486 syscoloringspkgs-1.0.0/syscoloringspkgs/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-22 20:25:14.000000 syscoloringspkgs-1.0.0/syscoloringspkgs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:25:15.495486 syscoloringspkgs-1.0.0/syscoloringspkgs.egg-info/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-22 20:25:15.000000 syscoloringspkgs-1.0.0/syscoloringspkgs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      197 2023-06-22 20:25:15.000000 syscoloringspkgs-1.0.0/syscoloringspkgs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:25:15.000000 syscoloringspkgs-1.0.0/syscoloringspkgs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-22 20:25:15.000000 syscoloringspkgs-1.0.0/syscoloringspkgs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:21.087165 syscoloringspkgs-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-22 20:27:21.087165 syscoloringspkgs-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 20:27:21.087165 syscoloringspkgs-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      562 2023-06-22 20:27:20.000000 syscoloringspkgs-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:21.087165 syscoloringspkgs-1.1.0/syscoloringspkgs/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-06-22 20:27:20.000000 syscoloringspkgs-1.1.0/syscoloringspkgs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 20:27:21.087165 syscoloringspkgs-1.1.0/syscoloringspkgs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-22 20:27:20.000000 syscoloringspkgs-1.1.0/syscoloringspkgs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-22 20:27:21.000000 syscoloringspkgs-1.1.0/syscoloringspkgs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 20:27:20.000000 syscoloringspkgs-1.1.0/syscoloringspkgs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-22 20:27:20.000000 syscoloringspkgs-1.1.0/syscoloringspkgs.egg-info/top_level.txt
```

### Comparing `syscoloringspkgs-1.0.0/setup.py` & `syscoloringspkgs-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syscoloringspkgs",
     version=VERSION,
```

