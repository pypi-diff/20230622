# Comparing `tmp/pipcolourextension-1.0.0.tar.gz` & `tmp/pipcolourextension-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipcolourextension-1.0.0.tar", last modified: Thu Jun 22 17:47:58 2023, max compression
+gzip compressed data, was "pipcolourextension-1.1.0.tar", last modified: Thu Jun 22 17:50:04 2023, max compression
```

## Comparing `pipcolourextension-1.0.0.tar` & `pipcolourextension-1.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:47:58.591635 pipcolourextension-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-22 17:47:58.591635 pipcolourextension-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:47:58.587635 pipcolourextension-1.0.0/pipcolourextension/
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-22 17:47:58.000000 pipcolourextension-1.0.0/pipcolourextension/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:47:58.591635 pipcolourextension-1.0.0/pipcolourextension.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-06-22 17:47:58.000000 pipcolourextension-1.0.0/pipcolourextension.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-06-22 17:47:58.000000 pipcolourextension-1.0.0/pipcolourextension.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:47:58.000000 pipcolourextension-1.0.0/pipcolourextension.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-22 17:47:58.000000 pipcolourextension-1.0.0/pipcolourextension.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 17:47:58.591635 pipcolourextension-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-06-22 17:47:58.000000 pipcolourextension-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:50:04.179270 pipcolourextension-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-22 17:50:04.179270 pipcolourextension-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:50:04.175270 pipcolourextension-1.1.0/pipcolourextension/
+-rw-r--r--   0 root         (0) root         (0)    96763 2023-06-22 17:50:03.000000 pipcolourextension-1.1.0/pipcolourextension/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 17:50:04.179270 pipcolourextension-1.1.0/pipcolourextension.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-06-22 17:50:04.000000 pipcolourextension-1.1.0/pipcolourextension.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-06-22 17:50:04.000000 pipcolourextension-1.1.0/pipcolourextension.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 17:50:04.000000 pipcolourextension-1.1.0/pipcolourextension.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-22 17:50:04.000000 pipcolourextension-1.1.0/pipcolourextension.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 17:50:04.179270 pipcolourextension-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-06-22 17:50:03.000000 pipcolourextension-1.1.0/setup.py
```

### Comparing `pipcolourextension-1.0.0/setup.py` & `pipcolourextension-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="pipcolourextension",
     version=VERSION,
```

