# Comparing `tmp/phub-2.5.tar.gz` & `tmp/phub-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phub-2.5.tar", last modified: Mon Jun 19 10:45:59 2023, max compression
+gzip compressed data, was "phub-2.6.tar", last modified: Thu Jun 22 17:50:44 2023, max compression
```

## Comparing `phub-2.5.tar` & `phub-2.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.780948 phub-2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 10:45:46.000000 phub-2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-19 10:45:59.780948 phub-2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-19 10:45:46.000000 phub-2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-19 10:45:46.000000 phub-2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-19 10:45:59.780948 phub-2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 10:45:46.000000 phub-2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.776949 phub-2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.780948 phub-2.5/src/phub/
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-19 10:45:46.000000 phub-2.5/src/phub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-06-19 10:45:46.000000 phub-2.5/src/phub/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-19 10:45:46.000000 phub-2.5/src/phub/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-19 10:45:46.000000 phub-2.5/src/phub/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-19 10:45:46.000000 phub-2.5/src/phub/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-19 10:45:46.000000 phub-2.5/src/phub/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 10:45:59.780948 phub-2.5/src/phub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 10:45:59.000000 phub-2.5/src/phub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-22 17:50:32.000000 phub-2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-22 17:50:44.156976 phub-2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-22 17:50:32.000000 phub-2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 17:50:32.000000 phub-2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-22 17:50:44.160976 phub-2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 17:50:32.000000 phub-2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/src/phub/
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-22 17:50:32.000000 phub-2.6/src/phub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-22 17:50:32.000000 phub-2.6/src/phub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17281 2023-06-22 17:50:32.000000 phub-2.6/src/phub/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-22 17:50:32.000000 phub-2.6/src/phub/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-22 17:50:32.000000 phub-2.6/src/phub/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-06-22 17:50:32.000000 phub-2.6/src/phub/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7762 2023-06-22 17:50:32.000000 phub-2.6/src/phub/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:50:44.156976 phub-2.6/src/phub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 17:50:44.000000 phub-2.6/src/phub.egg-info/top_level.txt
```

### Comparing `phub-2.5/LICENSE` & `phub-2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `phub-2.5/PKG-INFO` & `phub-2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.5
+Version: 2.6
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

### Comparing `phub-2.5/README.md` & `phub-2.6/README.md`

 * *Files identical despite different names*

### Comparing `phub-2.5/setup.cfg` & `phub-2.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = phub
-version = 2.5
+version = 2.6
 description = An API for PornHub
 author = Egsagon
 author_email = egsagon12@gmail.com
 url = https://github.com/Egsagon/PHUB/
 license = GPLv3
 license_file = LICENSE
 long_description = file: README.md
```

### Comparing `phub-2.5/src/phub/__init__.py` & `phub-2.6/src/phub/__init__.py`

 * *Files identical despite different names*

### Comparing `phub-2.5/src/phub/classes.py` & `phub-2.6/src/phub/classes.py`

 * *Files identical despite different names*

### Comparing `phub-2.5/src/phub/consts.py` & `phub-2.6/src/phub/consts.py`

 * *Files identical despite different names*

### Comparing `phub-2.5/src/phub/core.py` & `phub-2.6/src/phub/core.py`

 * *Files identical despite different names*

### Comparing `phub-2.5/src/phub/parser.py` & `phub-2.6/src/phub/parser.py`

 * *Files identical despite different names*

### Comparing `phub-2.5/src/phub/utils.py` & `phub-2.6/src/phub/utils.py`

 * *Files identical despite different names*

### Comparing `phub-2.5/src/phub.egg-info/PKG-INFO` & `phub-2.6/src/phub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phub
-Version: 2.5
+Version: 2.6
 Summary: An API for PornHub
 Home-page: https://github.com/Egsagon/PHUB/
 Author: Egsagon
 Author-email: egsagon12@gmail.com
 License: GPLv3
 Platform: unix
 Platform: linux
```

