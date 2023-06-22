# Comparing `tmp/makolator-0.1.0.tar.gz` & `tmp/makolator-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makolator-0.1.0.tar", max compression
+gzip compressed data, was "makolator-1.0.0.tar", max compression
```

## Comparing `makolator-0.1.0.tar` & `makolator-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-0.1.0/LICENSE
--rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-0.1.0/README.md
--rw-r--r--   0        0        0     1403 2023-06-20 10:13:16.213966 makolator-0.1.0/makolator/__init__.py
--rw-r--r--   0        0        0     2066 2023-06-20 10:18:54.509053 makolator-0.1.0/makolator/config.py
--rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-0.1.0/makolator/datamodel.py
--rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-0.1.0/makolator/escape.py
--rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-0.1.0/makolator/exceptions.py
--rw-r--r--   0        0        0    12353 2023-06-20 21:47:13.927681 makolator-0.1.0/makolator/makolator.py
--rw-r--r--   0        0        0     1392 2023-06-20 16:51:29.954462 makolator-0.1.0/makolator/util.py
--rw-r--r--   0        0        0     2186 2023-06-20 20:58:28.650107 makolator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-19 22:25:27.699704 makolator-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1140 2023-06-19 22:25:27.703704 makolator-1.0.0/README.md
+-rw-r--r--   0        0        0     4414 2023-06-21 13:56:34.948091 makolator-1.0.0/makolator/__init__.py
+-rw-r--r--   0        0        0     6106 2023-06-22 04:53:34.122764 makolator-1.0.0/makolator/_inplace.py
+-rw-r--r--   0        0        0     2066 2023-06-21 13:54:07.929256 makolator-1.0.0/makolator/config.py
+-rw-r--r--   0        0        0     2004 2023-06-19 22:00:06.937371 makolator-1.0.0/makolator/datamodel.py
+-rw-r--r--   0        0        0      897 2023-06-20 10:17:27.576552 makolator-1.0.0/makolator/escape.py
+-rw-r--r--   0        0        0      106 2023-06-19 07:58:57.579352 makolator-1.0.0/makolator/exceptions.py
+-rw-r--r--   0        0        0     7205 2023-06-22 04:52:48.846012 makolator-1.0.0/makolator/makolator.py
+-rw-r--r--   0        0        0     2186 2023-06-22 04:54:28.979683 makolator-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 makolator-1.0.0/PKG-INFO
```

### Comparing `makolator-0.1.0/LICENSE` & `makolator-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `makolator-0.1.0/README.md` & `makolator-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `makolator-0.1.0/makolator/config.py` & `makolator-1.0.0/makolator/config.py`

 * *Files identical despite different names*

### Comparing `makolator-0.1.0/makolator/datamodel.py` & `makolator-1.0.0/makolator/datamodel.py`

 * *Files identical despite different names*

### Comparing `makolator-0.1.0/makolator/escape.py` & `makolator-1.0.0/makolator/escape.py`

 * *Files identical despite different names*

### Comparing `makolator-0.1.0/pyproject.toml` & `makolator-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makolator"
-version = "0.1.0"
+version = "1.0.0"
 description = "Extended Mako Templates for Python"
 readme = "README.md"
 license = "MIT"
 authors = [
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `makolator-0.1.0/PKG-INFO` & `makolator-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makolator
-Version: 0.1.0
+Version: 1.0.0
 Summary: Extended Mako Templates for Python
 License: MIT
 Requires-Python: >=3.7.2,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

