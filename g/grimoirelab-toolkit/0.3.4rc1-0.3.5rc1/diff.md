# Comparing `tmp/grimoirelab_toolkit-0.3.4rc1.tar.gz` & `tmp/grimoirelab_toolkit-0.3.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab_toolkit-0.3.4rc1.tar", max compression
+gzip compressed data, was "grimoirelab_toolkit-0.3.5rc1.tar", max compression
```

## Comparing `grimoirelab_toolkit-0.3.4rc1.tar` & `grimoirelab_toolkit-0.3.5rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      229 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/LICENSE
--rw-r--r--   0        0        0     1002 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/NEWS
--rw-r--r--   0        0        0     2091 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/README.md
--rw-r--r--   0        0        0     1011 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/__init__.py
--rw-r--r--   0        0        0       91 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/_version.py
--rw-r--r--   0        0        0     5606 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/datetime.py
--rw-r--r--   0        0        0     3846 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/introspect.py
--rw-r--r--   0        0        0     1383 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/uris.py
--rw-r--r--   0        0        0     1119 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/pyproject.toml
--rwxr-xr-x   0        0        0     1063 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/run_tests.py
--rw-r--r--   0        0        0    10186 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/test_datetime.py
--rw-r--r--   0        0        0     7078 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/test_introspect.py
--rw-r--r--   0        0        0     2678 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/test_uris.py
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 grimoirelab_toolkit-0.3.4rc1/PKG-INFO
+-rw-r--r--   0        0        0      229 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/LICENSE
+-rw-r--r--   0        0        0     1093 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/NEWS
+-rw-r--r--   0        0        0     2091 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/README.md
+-rw-r--r--   0        0        0     1011 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/_version.py
+-rw-r--r--   0        0        0     5606 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/datetime.py
+-rw-r--r--   0        0        0     3846 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/introspect.py
+-rw-r--r--   0        0        0     1383 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/uris.py
+-rw-r--r--   0        0        0     1119 2023-06-22 07:42:16.025964 grimoirelab_toolkit-0.3.5rc1/pyproject.toml
+-rwxr-xr-x   0        0        0     1063 2023-06-22 07:42:16.029964 grimoirelab_toolkit-0.3.5rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    10186 2023-06-22 07:42:16.029964 grimoirelab_toolkit-0.3.5rc1/tests/test_datetime.py
+-rw-r--r--   0        0        0     7078 2023-06-22 07:42:16.029964 grimoirelab_toolkit-0.3.5rc1/tests/test_introspect.py
+-rw-r--r--   0        0        0     2678 2023-06-22 07:42:16.029964 grimoirelab_toolkit-0.3.5rc1/tests/test_uris.py
+-rw-r--r--   0        0        0     3055 1970-01-01 00:00:00.000000 grimoirelab_toolkit-0.3.5rc1/PKG-INFO
```

### Comparing `grimoirelab_toolkit-0.3.4rc1/LICENSE` & `grimoirelab_toolkit-0.3.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/NEWS` & `grimoirelab_toolkit-0.3.5rc1/NEWS`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## grimoirelab-toolkit 0.3.4 - (2023-04-21)
+  
+  * Update Poetry's package dependencies
+
   ## grimoirelab-toolkit 0.3.3 - (2023-02-01)
   
   * Update Poetry's package dependencies
 
   ## grimoirelab-toolkit 0.3.2 - (2022-10-31)
   
   * Update Poetry's package dependencies
```

### Comparing `grimoirelab_toolkit-0.3.4rc1/README.md` & `grimoirelab_toolkit-0.3.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/__init__.py` & `grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/datetime.py` & `grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/datetime.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/introspect.py` & `grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/introspect.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/uris.py` & `grimoirelab_toolkit-0.3.5rc1/grimoirelab_toolkit/uris.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/pyproject.toml` & `grimoirelab_toolkit-0.3.5rc1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab-toolkit"
-version = "0.3.4-rc.1"
+version = "0.3.5-rc.1"
 description = "Toolkit of common functions used across GrimoireLab"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `grimoirelab_toolkit-0.3.4rc1/tests/run_tests.py` & `grimoirelab_toolkit-0.3.5rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/tests/test_datetime.py` & `grimoirelab_toolkit-0.3.5rc1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/tests/test_introspect.py` & `grimoirelab_toolkit-0.3.5rc1/tests/test_introspect.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/tests/test_uris.py` & `grimoirelab_toolkit-0.3.5rc1/tests/test_uris.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.4rc1/PKG-INFO` & `grimoirelab_toolkit-0.3.5rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab-toolkit
-Version: 0.3.4rc1
+Version: 0.3.5rc1
 Summary: Toolkit of common functions used across GrimoireLab
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,15 +12,14 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Project-URL: Repository, https://github.com/chaoss/grimoirelab-toolkit
 Description-Content-Type: text/markdown
 
 # GrimoireLab Toolkit [![Build Status](https://github.com/chaoss/grimoirelab-toolkit/workflows/tests/badge.svg)](https://github.com/chaoss/grimoirelab-toolkit/actions?query=workflow:tests+branch:master+event:push) [![Coverage Status](https://img.shields.io/coveralls/chaoss/grimoirelab-toolkit.svg)](https://coveralls.io/r/chaoss/grimoirelab-toolkit?branch=master)
```

