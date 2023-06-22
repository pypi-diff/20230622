# Comparing `tmp/PyEmailExtracter-0.4.tar.gz` & `tmp/PyEmailExtracter-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailExtracter-0.4.tar", last modified: Thu Jun 22 10:31:04 2023, max compression
+gzip compressed data, was "PyEmailExtracter-0.5.tar", last modified: Thu Jun 22 10:34:10 2023, max compression
```

## Comparing `PyEmailExtracter-0.4.tar` & `PyEmailExtracter-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:31:04.560619 PyEmailExtracter-0.4/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 10:31:04.556619 PyEmailExtracter-0.4/PKG-INFO
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:31:04.556619 PyEmailExtracter-0.4/PyEmailExtracter/
--rw-rw-r--   0 karki     (1000) karki     (1000)       64 2023-06-22 10:31:00.000000 PyEmailExtracter-0.4/PyEmailExtracter/__init__.py
--rw-rw-r--   0 karki     (1000) karki     (1000)      957 2023-06-22 10:21:01.000000 PyEmailExtracter-0.4/PyEmailExtracter/driver.py
--rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 09:32:55.000000 PyEmailExtracter-0.4/PyEmailExtracter/helper.py
-drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:31:04.556619 PyEmailExtracter-0.4/PyEmailExtracter.egg-info/
--rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 10:31:04.000000 PyEmailExtracter-0.4/PyEmailExtracter.egg-info/PKG-INFO
--rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-22 10:31:04.000000 PyEmailExtracter-0.4/PyEmailExtracter.egg-info/SOURCES.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-22 10:31:04.000000 PyEmailExtracter-0.4/PyEmailExtracter.egg-info/dependency_links.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       81 2023-06-22 10:31:04.000000 PyEmailExtracter-0.4/PyEmailExtracter.egg-info/requires.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-22 10:31:04.000000 PyEmailExtracter-0.4/PyEmailExtracter.egg-info/top_level.txt
--rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:26:17.000000 PyEmailExtracter-0.4/README.md
--rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-22 10:31:04.560619 PyEmailExtracter-0.4/setup.cfg
--rw-rw-r--   0 karki     (1000) karki     (1000)      471 2023-06-22 10:30:37.000000 PyEmailExtracter-0.4/setup.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:34:10.454113 PyEmailExtracter-0.5/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 10:34:10.454113 PyEmailExtracter-0.5/PKG-INFO
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:34:10.454113 PyEmailExtracter-0.5/PyEmailExtracter/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      132 2023-06-22 10:33:58.000000 PyEmailExtracter-0.5/PyEmailExtracter/__init__.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)      958 2023-06-22 10:33:25.000000 PyEmailExtracter-0.5/PyEmailExtracter/driver.py
+-rw-rw-r--   0 karki     (1000) karki     (1000)     1898 2023-06-22 10:33:31.000000 PyEmailExtracter-0.5/PyEmailExtracter/helper.py
+drwxrwxr-x   0 karki     (1000) karki     (1000)        0 2023-06-22 10:34:10.454113 PyEmailExtracter-0.5/PyEmailExtracter.egg-info/
+-rw-rw-r--   0 karki     (1000) karki     (1000)      208 2023-06-22 10:34:10.000000 PyEmailExtracter-0.5/PyEmailExtracter.egg-info/PKG-INFO
+-rw-rw-r--   0 karki     (1000) karki     (1000)      300 2023-06-22 10:34:10.000000 PyEmailExtracter-0.5/PyEmailExtracter.egg-info/SOURCES.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        1 2023-06-22 10:34:10.000000 PyEmailExtracter-0.5/PyEmailExtracter.egg-info/dependency_links.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       81 2023-06-22 10:34:10.000000 PyEmailExtracter-0.5/PyEmailExtracter.egg-info/requires.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)       17 2023-06-22 10:34:10.000000 PyEmailExtracter-0.5/PyEmailExtracter.egg-info/top_level.txt
+-rw-rw-r--   0 karki     (1000) karki     (1000)        0 2023-06-22 09:26:17.000000 PyEmailExtracter-0.5/README.md
+-rw-rw-r--   0 karki     (1000) karki     (1000)       38 2023-06-22 10:34:10.454113 PyEmailExtracter-0.5/setup.cfg
+-rw-rw-r--   0 karki     (1000) karki     (1000)      471 2023-06-22 10:34:07.000000 PyEmailExtracter-0.5/setup.py
```

### Comparing `PyEmailExtracter-0.4/PyEmailExtracter/driver.py` & `PyEmailExtracter-0.5/PyEmailExtracter/driver.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from helper import *
+from .helper import *
 
 
 def extract_emails(dir=""):
     # Example: "/home/user_name/some_directory/resumes"
     # directory = str(
     #     input("Paste the absolute path of the directory and press enter.\n")
     # )
```

### Comparing `PyEmailExtracter-0.4/PyEmailExtracter/helper.py` & `PyEmailExtracter-0.5/PyEmailExtracter/helper.py`

 * *Files identical despite different names*

