# Comparing `tmp/emreader-0.1.6.tar.gz` & `tmp/emreader-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emreader-0.1.6.tar", max compression
+gzip compressed data, was "emreader-0.1.7.tar", max compression
```

## Comparing `emreader-0.1.6.tar` & `emreader-0.1.7.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.6/README.md
--rw-r--r--   0        0        0      854 2023-06-22 19:52:10.353075 emreader-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.6/src/__init__.py
--rw-r--r--   0        0        0     3677 2023-06-22 19:50:55.518572 emreader-0.1.6/src/app.py
--rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.6/src/core/__init__.py
--rw-r--r--   0        0        0      143 2023-06-22 19:52:00.056298 emreader-0.1.6/src/core/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      159 2023-06-22 19:35:57.735123 emreader-0.1.6/src/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4303 2023-06-22 19:52:00.059538 emreader-0.1.6/src/core/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     8713 2023-06-22 19:35:57.738541 emreader-0.1.6/src/core/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     2204 2023-06-22 19:52:01.171812 emreader-0.1.6/src/core/__pycache__/eml.cpython-310.pyc
--rw-r--r--   0        0        0     4634 2023-06-22 19:37:13.102413 emreader-0.1.6/src/core/__pycache__/eml.cpython-311.pyc
--rw-r--r--   0        0        0     1818 2023-06-22 19:52:01.169455 emreader-0.1.6/src/core/__pycache__/parse_tab.cpython-310.pyc
--rw-r--r--   0        0        0     3256 2023-06-22 19:37:13.099936 emreader-0.1.6/src/core/__pycache__/parse_tab.cpython-311.pyc
--rw-r--r--   0        0        0     3538 2023-06-22 19:52:01.170857 emreader-0.1.6/src/core/__pycache__/util.cpython-310.pyc
--rw-r--r--   0        0        0     7680 2023-06-22 19:37:13.101358 emreader-0.1.6/src/core/__pycache__/util.cpython-311.pyc
--rw-r--r--   0        0        0     6062 2023-06-22 19:51:14.534375 emreader-0.1.6/src/core/base.py
--rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.6/src/core/eml.py
--rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.6/src/core/parse_tab.py
--rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.6/src/core/util.py
--rw-r--r--   0        0        0      189 2023-06-22 19:51:55.311457 emreader-0.1.6/src/runner.py
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 emreader-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.7/README.md
+-rw-r--r--   0        0        0      854 2023-06-22 19:56:51.953062 emreader-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.7/src/__init__.py
+-rw-r--r--   0        0        0     3677 2023-06-22 19:50:55.518572 emreader-0.1.7/src/app.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.7/src/core/__init__.py
+-rw-r--r--   0        0        0      143 2023-06-22 19:52:00.056298 emreader-0.1.7/src/core/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      159 2023-06-22 19:35:57.735123 emreader-0.1.7/src/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4303 2023-06-22 19:52:00.059538 emreader-0.1.7/src/core/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     8713 2023-06-22 19:35:57.738541 emreader-0.1.7/src/core/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     2204 2023-06-22 19:52:01.171812 emreader-0.1.7/src/core/__pycache__/eml.cpython-310.pyc
+-rw-r--r--   0        0        0     4634 2023-06-22 19:37:13.102413 emreader-0.1.7/src/core/__pycache__/eml.cpython-311.pyc
+-rw-r--r--   0        0        0     1818 2023-06-22 19:52:01.169455 emreader-0.1.7/src/core/__pycache__/parse_tab.cpython-310.pyc
+-rw-r--r--   0        0        0     3256 2023-06-22 19:37:13.099936 emreader-0.1.7/src/core/__pycache__/parse_tab.cpython-311.pyc
+-rw-r--r--   0        0        0     3538 2023-06-22 19:52:01.170857 emreader-0.1.7/src/core/__pycache__/util.cpython-310.pyc
+-rw-r--r--   0        0        0     7680 2023-06-22 19:37:13.101358 emreader-0.1.7/src/core/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0     6062 2023-06-22 19:51:14.534375 emreader-0.1.7/src/core/base.py
+-rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.7/src/core/eml.py
+-rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.7/src/core/parse_tab.py
+-rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.7/src/core/util.py
+-rw-r--r--   0        0        0      189 2023-06-22 19:51:55.311457 emreader-0.1.7/src/runner.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:55:56.070115 emreader-0.1.7/src/storage/output/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-22 19:56:09.592388 emreader-0.1.7/src/storage/source/emails/.gitkeep
+-rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 emreader-0.1.7/PKG-INFO
```

### Comparing `emreader-0.1.6/pyproject.toml` & `emreader-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emreader"
-version = "0.1.6"
+version = "0.1.7"
 description = ""
 authors = ["themba <themba@advantch.com>"]
 readme = "README.md"
 license = "Commercial"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `emreader-0.1.6/src/app.py` & `emreader-0.1.7/src/app.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/base.cpython-310.pyc` & `emreader-0.1.7/src/core/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/base.cpython-311.pyc` & `emreader-0.1.7/src/core/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/eml.cpython-310.pyc` & `emreader-0.1.7/src/core/__pycache__/eml.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/eml.cpython-311.pyc` & `emreader-0.1.7/src/core/__pycache__/eml.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/parse_tab.cpython-310.pyc` & `emreader-0.1.7/src/core/__pycache__/parse_tab.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/parse_tab.cpython-311.pyc` & `emreader-0.1.7/src/core/__pycache__/parse_tab.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/util.cpython-310.pyc` & `emreader-0.1.7/src/core/__pycache__/util.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/__pycache__/util.cpython-311.pyc` & `emreader-0.1.7/src/core/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/base.py` & `emreader-0.1.7/src/core/base.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/eml.py` & `emreader-0.1.7/src/core/eml.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/parse_tab.py` & `emreader-0.1.7/src/core/parse_tab.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/src/core/util.py` & `emreader-0.1.7/src/core/util.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.6/PKG-INFO` & `emreader-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emreader
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 License: Commercial
 Author: themba
 Author-email: themba@advantch.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

