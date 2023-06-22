# Comparing `tmp/kidash-0.5.6rc1.tar.gz` & `tmp/kidash-0.5.7rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kidash-0.5.6rc1.tar", max compression
+gzip compressed data, was "kidash-0.5.7rc1.tar", max compression
```

## Comparing `kidash-0.5.6rc1.tar` & `kidash-0.5.7rc1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      300 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/AUTHORS
--rw-r--r--   0        0        0    35147 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/LICENSE
--rw-r--r--   0        0        0     1288 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/NEWS
--rw-r--r--   0        0        0     2525 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/README.md
--rw-r--r--   0        0        0      894 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/kidash/__init__.py
--rw-r--r--   0        0        0       91 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/kidash/_version.py
--rwxr-xr-x   0        0        0     4355 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/kidash/bin/kidash.py
--rwxr-xr-x   0        0        0    59367 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/kidash/kidash.py
--rw-r--r--   0        0        0     1307 2023-05-17 12:45:05.193713 kidash-0.5.6rc1/pyproject.toml
--rw-r--r--   0        0        0    54328 2023-05-17 12:45:05.197713 kidash-0.5.6rc1/tests/data/overview-with-index-patterns.json
--rwxr-xr-x   0        0        0     1166 2023-05-17 12:45:05.197713 kidash-0.5.6rc1/tests/run_tests.py
--rw-r--r--   0        0        0     2131 2023-05-17 12:45:05.197713 kidash-0.5.6rc1/tests/test_export.py
--rw-r--r--   0        0        0     3709 1970-01-01 00:00:00.000000 kidash-0.5.6rc1/PKG-INFO
+-rw-r--r--   0        0        0      300 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/LICENSE
+-rw-r--r--   0        0        0     1366 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/NEWS
+-rw-r--r--   0        0        0     2525 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/README.md
+-rw-r--r--   0        0        0      894 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/kidash/__init__.py
+-rw-r--r--   0        0        0       91 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/kidash/_version.py
+-rwxr-xr-x   0        0        0     4355 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/kidash/bin/kidash.py
+-rwxr-xr-x   0        0        0    59367 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/kidash/kidash.py
+-rw-r--r--   0        0        0     1307 2023-06-22 07:42:09.206982 kidash-0.5.7rc1/pyproject.toml
+-rw-r--r--   0        0        0    54328 2023-06-22 07:42:09.210982 kidash-0.5.7rc1/tests/data/overview-with-index-patterns.json
+-rwxr-xr-x   0        0        0     1166 2023-06-22 07:42:09.210982 kidash-0.5.7rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     2131 2023-06-22 07:42:09.210982 kidash-0.5.7rc1/tests/test_export.py
+-rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 kidash-0.5.7rc1/PKG-INFO
```

### Comparing `kidash-0.5.6rc1/LICENSE` & `kidash-0.5.7rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/NEWS` & `kidash-0.5.7rc1/NEWS`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## kidash 0.5.6 - (2023-05-17)
+  
+  * Update Poetry's package dependencies
+
   ## kidash 0.5.5 - (2023-04-27)
   
   * Update Poetry's package dependencies
 
   ## kidash 0.5.4 - (2023-04-21)
   
   * Update Poetry's package dependencies
```

### Comparing `kidash-0.5.6rc1/README.md` & `kidash-0.5.7rc1/README.md`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/kidash/__init__.py` & `kidash-0.5.7rc1/kidash/__init__.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/kidash/bin/kidash.py` & `kidash-0.5.7rc1/kidash/bin/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/kidash/kidash.py` & `kidash-0.5.7rc1/kidash/kidash.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/pyproject.toml` & `kidash-0.5.7rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kidash"
-version = "0.5.6-rc.1"
+version = "0.5.7-rc.1"
 description = "GrimoireLab script to manage Kibana dashboards from the command line"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `kidash-0.5.6rc1/tests/data/overview-with-index-patterns.json` & `kidash-0.5.7rc1/tests/data/overview-with-index-patterns.json`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/tests/run_tests.py` & `kidash-0.5.7rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/tests/test_export.py` & `kidash-0.5.7rc1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `kidash-0.5.6rc1/PKG-INFO` & `kidash-0.5.7rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kidash
-Version: 0.5.6rc1
+Version: 0.5.7rc1
 Summary: GrimoireLab script to manage Kibana dashboards from the command line
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
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
 Requires-Dist: requests (>=2.7.0,<3.0.0)
 Requires-Dist: urllib3 (>=1.26,<2.0)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab-kidash/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab-kidash
 Description-Content-Type: text/markdown
```

