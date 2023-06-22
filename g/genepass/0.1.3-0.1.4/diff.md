# Comparing `tmp/genepass-0.1.3.tar.gz` & `tmp/genepass-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genepass-0.1.3.tar", last modified: Thu Jun 22 14:04:28 2023, max compression
+gzip compressed data, was "genepass-0.1.4.tar", last modified: Thu Jun 22 14:10:57 2023, max compression
```

## Comparing `genepass-0.1.3.tar` & `genepass-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:04:28.660929 genepass-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 14:04:16.000000 genepass-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-22 14:04:28.660929 genepass-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-22 14:04:16.000000 genepass-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:04:28.660929 genepass-0.1.3/genepass/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 14:04:16.000000 genepass-0.1.3/genepass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-22 14:04:16.000000 genepass-0.1.3/genepass/genepass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:04:28.660929 genepass-0.1.3/genepass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-22 14:04:28.000000 genepass-0.1.3/genepass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 14:04:28.000000 genepass-0.1.3/genepass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:04:28.000000 genepass-0.1.3/genepass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 14:04:28.000000 genepass-0.1.3/genepass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:04:28.660929 genepass-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-22 14:04:16.000000 genepass-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:10:57.586479 genepass-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 14:10:46.000000 genepass-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 14:10:57.586479 genepass-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-22 14:10:46.000000 genepass-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:10:57.582479 genepass-0.1.4/genepass/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 14:10:46.000000 genepass-0.1.4/genepass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-22 14:10:46.000000 genepass-0.1.4/genepass/genepass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:10:57.586479 genepass-0.1.4/genepass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 14:10:57.000000 genepass-0.1.4/genepass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:10:57.586479 genepass-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-22 14:10:46.000000 genepass-0.1.4/setup.py
```

### Comparing `genepass-0.1.3/LICENSE` & `genepass-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `genepass-0.1.3/PKG-INFO` & `genepass-0.1.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: genepass
-Version: 0.1.3
+Version: 0.1.4
 Summary: genepass can automatically generates passwords
 Home-page: https://github.com/senya-koku/genepass
 Author:  ny7777
 Author-email: meathouse47@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # genepass
 
 generating passward randomly!
 
+----
 # Install
-`pip install odach`
+`pip install genepass`
 
+----
 # Usage
 
 ```python
 import genepass
 
 genepass.create_random_password()
 ```
 
+----
 # Option
 - security_level
     - strong : DIGITS & CAPITAL_LETTER & SMALL_LETTER
-    - god : DIGITS & CAPITAL_LETTER & SMALL_LETTER & SYMBOLS
+    - god    : DIGITS & CAPITAL_LETTER & SMALL_LETTER & SYMBOLS
     - custom : Under construction
+ 
+    ----
```

### Comparing `genepass-0.1.3/genepass/genepass.py` & `genepass-0.1.4/genepass/genepass.py`

 * *Files identical despite different names*

### Comparing `genepass-0.1.3/genepass.egg-info/PKG-INFO` & `genepass-0.1.4/genepass.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 Metadata-Version: 2.1
 Name: genepass
-Version: 0.1.3
+Version: 0.1.4
 Summary: genepass can automatically generates passwords
 Home-page: https://github.com/senya-koku/genepass
 Author:  ny7777
 Author-email: meathouse47@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # genepass
 
 generating passward randomly!
 
+----
 # Install
-`pip install odach`
+`pip install genepass`
 
+----
 # Usage
 
 ```python
 import genepass
 
 genepass.create_random_password()
 ```
 
+----
 # Option
 - security_level
     - strong : DIGITS & CAPITAL_LETTER & SMALL_LETTER
-    - god : DIGITS & CAPITAL_LETTER & SMALL_LETTER & SYMBOLS
+    - god    : DIGITS & CAPITAL_LETTER & SMALL_LETTER & SYMBOLS
     - custom : Under construction
+ 
+    ----
```

