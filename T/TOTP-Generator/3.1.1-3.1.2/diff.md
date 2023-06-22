# Comparing `tmp/TOTP Generator-3.1.1.tar.gz` & `tmp/TOTP Generator-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TOTP Generator-3.1.1.tar", last modified: Fri Jul 29 09:33:31 2022, max compression
+gzip compressed data, was "TOTP Generator-3.1.2.tar", last modified: Thu Jun 22 13:59:58 2023, max compression
```

## Comparing `TOTP Generator-3.1.1.tar` & `TOTP Generator-3.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeremy    (1000) users      (100)        0 2022-07-29 09:33:31.600146 TOTP Generator-3.1.1/
--rw-r--r--   0 jeremy    (1000) users      (100)    35147 2019-03-28 16:52:29.000000 TOTP Generator-3.1.1/LICENSE
--rw-r--r--   0 jeremy    (1000) users      (100)     2513 2022-07-29 09:33:31.600146 TOTP Generator-3.1.1/PKG-INFO
--rw-r--r--   0 jeremy    (1000) users      (100)     1817 2022-07-29 09:32:23.000000 TOTP Generator-3.1.1/README.md
-drwxr-xr-x   0 jeremy    (1000) users      (100)        0 2022-07-29 09:33:31.600146 TOTP Generator-3.1.1/TOTP_Generator.egg-info/
--rw-r--r--   0 jeremy    (1000) users      (100)     2513 2022-07-29 09:33:31.000000 TOTP Generator-3.1.1/TOTP_Generator.egg-info/PKG-INFO
--rw-r--r--   0 jeremy    (1000) users      (100)      334 2022-07-29 09:33:31.000000 TOTP Generator-3.1.1/TOTP_Generator.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy    (1000) users      (100)        1 2022-07-29 09:33:31.000000 TOTP Generator-3.1.1/TOTP_Generator.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy    (1000) users      (100)       60 2022-07-29 09:33:31.000000 TOTP Generator-3.1.1/TOTP_Generator.egg-info/entry_points.txt
--rw-r--r--   0 jeremy    (1000) users      (100)      214 2022-07-29 09:33:31.000000 TOTP Generator-3.1.1/TOTP_Generator.egg-info/requires.txt
--rw-r--r--   0 jeremy    (1000) users      (100)       15 2022-07-29 09:33:31.000000 TOTP Generator-3.1.1/TOTP_Generator.egg-info/top_level.txt
--rw-r--r--   0 jeremy    (1000) users      (100)       38 2022-07-29 09:33:31.600146 TOTP Generator-3.1.1/setup.cfg
--rw-r--r--   0 jeremy    (1000) users      (100)     3349 2022-07-29 09:28:59.000000 TOTP Generator-3.1.1/setup.py
-drwxr-xr-x   0 jeremy    (1000) users      (100)        0 2022-07-29 09:33:31.600146 TOTP Generator-3.1.1/totp_generator/
--rw-r--r--   0 jeremy    (1000) users      (100)       75 2022-07-29 09:32:23.000000 TOTP Generator-3.1.1/totp_generator/__init__.py
--rwxr-xr-x   0 jeremy    (1000) users      (100)    12574 2022-07-29 09:32:23.000000 TOTP Generator-3.1.1/totp_generator/cli.py
--rw-r--r--   0 jeremy    (1000) users      (100)     7586 2022-07-29 08:55:50.000000 TOTP Generator-3.1.1/totp_generator/core_utils.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-06-22 13:59:58.685575 TOTP Generator-3.1.2/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)    35147 2019-03-28 16:52:29.000000 TOTP Generator-3.1.2/LICENSE
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     2513 2023-06-22 13:59:58.681575 TOTP Generator-3.1.2/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1817 2022-07-29 09:32:23.000000 TOTP Generator-3.1.2/README.md
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-06-22 13:59:58.681575 TOTP Generator-3.1.2/TOTP_Generator.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     2513 2023-06-22 13:59:58.000000 TOTP Generator-3.1.2/TOTP_Generator.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      334 2023-06-22 13:59:58.000000 TOTP Generator-3.1.2/TOTP_Generator.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2023-06-22 13:59:58.000000 TOTP Generator-3.1.2/TOTP_Generator.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       60 2023-06-22 13:59:58.000000 TOTP Generator-3.1.2/TOTP_Generator.egg-info/entry_points.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      214 2023-06-22 13:59:58.000000 TOTP Generator-3.1.2/TOTP_Generator.egg-info/requires.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       15 2023-06-22 13:59:58.000000 TOTP Generator-3.1.2/TOTP_Generator.egg-info/top_level.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2023-06-22 13:59:58.685575 TOTP Generator-3.1.2/setup.cfg
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     3349 2022-07-29 09:28:59.000000 TOTP Generator-3.1.2/setup.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2023-06-22 13:59:58.681575 TOTP Generator-3.1.2/totp_generator/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       75 2023-06-22 13:59:41.000000 TOTP Generator-3.1.2/totp_generator/__init__.py
+-rwxr-xr-x   0 jeremy    (1000) jeremy    (1000)    12574 2022-07-29 09:32:23.000000 TOTP Generator-3.1.2/totp_generator/cli.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     7586 2022-07-29 08:55:50.000000 TOTP Generator-3.1.2/totp_generator/core_utils.py
```

### Comparing `TOTP Generator-3.1.1/LICENSE` & `TOTP Generator-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TOTP Generator-3.1.1/PKG-INFO` & `TOTP Generator-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TOTP Generator
-Version: 3.1.1
+Version: 3.1.2
 Summary: Utility that generates TOTP codes and stores the TOTP secrets in your system keyring.
 Home-page: https://github.com/jjfalling/totp-generator
 Author: Jeremy Falling
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `TOTP Generator-3.1.1/README.md` & `TOTP Generator-3.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TOTP Generator-3.1.1/TOTP_Generator.egg-info/PKG-INFO` & `TOTP Generator-3.1.2/TOTP_Generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TOTP-Generator
-Version: 3.1.1
+Version: 3.1.2
 Summary: Utility that generates TOTP codes and stores the TOTP secrets in your system keyring.
 Home-page: https://github.com/jjfalling/totp-generator
 Author: Jeremy Falling
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `TOTP Generator-3.1.1/setup.py` & `TOTP Generator-3.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `TOTP Generator-3.1.1/totp_generator/cli.py` & `TOTP Generator-3.1.2/totp_generator/cli.py`

 * *Files identical despite different names*

### Comparing `TOTP Generator-3.1.1/totp_generator/core_utils.py` & `TOTP Generator-3.1.2/totp_generator/core_utils.py`

 * *Files identical despite different names*

