# Comparing `tmp/PyEmailExtracter-0.6.tar.gz` & `tmp/PyEmailExtracter-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailExtracter-0.6.tar", last modified: Thu Jun 22 12:29:51 2023, max compression
+gzip compressed data, was "PyEmailExtracter-0.7.tar", last modified: Thu Jun 22 12:33:28 2023, max compression
```

## Comparing `PyEmailExtracter-0.6.tar` & `PyEmailExtracter-0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 12:29:51.249480 PyEmailExtracter-0.6/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 12:29:51.249480 PyEmailExtracter-0.6/PKG-INFO
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 12:29:51.245480 PyEmailExtracter-0.6/PyEmailExtracter/
--rw-rw-r--   0 karki     (1000) karki     (1000)      132 2023-06-22 10:33:58.000000 PyEmailExtracter-0.6/PyEmailExtracter/__init__.py
--rw-rw-r--   0 karki     (1000) karki     (1000)      958 2023-06-22 10:33:25.000000 PyEmailExtracter-0.6/PyEmailExtracter/driver.py
--rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 10:33:31.000000 PyEmailExtracter-0.6/PyEmailExtracter/helper.py
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 12:29:51.245480 PyEmailExtracter-0.6/PyEmailExtracter.egg-info/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 12:29:51.000000 PyEmailExtracter-0.6/PyEmailExtracter.egg-info/PKG-INFO
--rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-22 12:29:51.000000 PyEmailExtracter-0.6/PyEmailExtracter.egg-info/SOURCES.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-22 12:29:51.000000 PyEmailExtracter-0.6/PyEmailExtracter.egg-info/dependency_links.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       81 2023-06-22 12:29:51.000000 PyEmailExtracter-0.6/PyEmailExtracter.egg-info/requires.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-22 12:29:51.000000 PyEmailExtracter-0.6/PyEmailExtracter.egg-info/top_level.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:26:17.000000 PyEmailExtracter-0.6/README.md
--rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-22 12:29:51.249480 PyEmailExtracter-0.6/setup.cfg
--rw-rw-r--   0 karki     (1000) karki     (1000)      471 2023-06-22 12:29:47.000000 PyEmailExtracter-0.6/setup.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 12:33:28.497391 PyEmailExtracter-0.7/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 12:33:28.497391 PyEmailExtracter-0.7/PKG-INFO
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 12:33:28.497391 PyEmailExtracter-0.7/PyEmailExtracter/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      132 2023-06-22 10:33:58.000000 PyEmailExtracter-0.7/PyEmailExtracter/__init__.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)      958 2023-06-22 10:33:25.000000 PyEmailExtracter-0.7/PyEmailExtracter/driver.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 10:33:31.000000 PyEmailExtracter-0.7/PyEmailExtracter/helper.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 12:33:28.497391 PyEmailExtracter-0.7/PyEmailExtracter.egg-info/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 12:33:28.000000 PyEmailExtracter-0.7/PyEmailExtracter.egg-info/PKG-INFO
+-rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-22 12:33:28.000000 PyEmailExtracter-0.7/PyEmailExtracter.egg-info/SOURCES.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-22 12:33:28.000000 PyEmailExtracter-0.7/PyEmailExtracter.egg-info/dependency_links.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       76 2023-06-22 12:33:28.000000 PyEmailExtracter-0.7/PyEmailExtracter.egg-info/requires.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-22 12:33:28.000000 PyEmailExtracter-0.7/PyEmailExtracter.egg-info/top_level.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:26:17.000000 PyEmailExtracter-0.7/README.md
+-rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-22 12:33:28.497391 PyEmailExtracter-0.7/setup.cfg
+-rw-rw-r--   0 karki     (1000) karki     (1000)      473 2023-06-22 12:33:24.000000 PyEmailExtracter-0.7/setup.py
```

### Comparing `PyEmailExtracter-0.6/PyEmailExtracter/driver.py` & `PyEmailExtracter-0.7/PyEmailExtracter/driver.py`

 * *Files identical despite different names*

### Comparing `PyEmailExtracter-0.6/PyEmailExtracter/helper.py` & `PyEmailExtracter-0.7/PyEmailExtracter/helper.py`

 * *Files identical despite different names*

