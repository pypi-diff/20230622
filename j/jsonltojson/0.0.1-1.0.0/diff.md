# Comparing `tmp/jsonltojson-0.0.1.tar.gz` & `tmp/jsonltojson-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonltojson-0.0.1.tar", last modified: Thu Jun 22 10:55:50 2023, max compression
+gzip compressed data, was "jsonltojson-1.0.0.tar", last modified: Thu Jun 22 10:56:13 2023, max compression
```

## Comparing `jsonltojson-0.0.1.tar` & `jsonltojson-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 10:55:50.401151 jsonltojson-0.0.1/
--rw-rw-rw-   0        0        0     1098 2023-06-22 10:14:48.000000 jsonltojson-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1287 2023-06-22 10:55:50.400150 jsonltojson-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      703 2023-06-22 10:44:43.000000 jsonltojson-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 10:55:50.393148 jsonltojson-0.0.1/jsonltojson/
--rw-rw-rw-   0        0        0       44 2023-06-22 08:42:47.000000 jsonltojson-0.0.1/jsonltojson/__init__.py
--rw-rw-rw-   0        0        0     1480 2023-06-22 07:57:03.000000 jsonltojson-0.0.1/jsonltojson/formatters.py
-drwxrwxrwx   0        0        0        0 2023-06-22 10:55:50.399150 jsonltojson-0.0.1/jsonltojson.egg-info/
--rw-rw-rw-   0        0        0     1287 2023-06-22 10:55:50.000000 jsonltojson-0.0.1/jsonltojson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2023-06-22 10:55:50.000000 jsonltojson-0.0.1/jsonltojson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 10:55:50.000000 jsonltojson-0.0.1/jsonltojson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-22 10:55:50.000000 jsonltojson-0.0.1/jsonltojson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      664 2023-06-22 10:47:20.000000 jsonltojson-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-22 10:55:50.402149 jsonltojson-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 10:56:13.755981 jsonltojson-1.0.0/
+-rw-rw-rw-   0        0        0     1098 2023-06-22 10:14:48.000000 jsonltojson-1.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1287 2023-06-22 10:56:13.754990 jsonltojson-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2023-06-22 10:44:43.000000 jsonltojson-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 10:56:13.743981 jsonltojson-1.0.0/jsonltojson/
+-rw-rw-rw-   0        0        0       44 2023-06-22 08:42:47.000000 jsonltojson-1.0.0/jsonltojson/__init__.py
+-rw-rw-rw-   0        0        0     1480 2023-06-22 07:57:03.000000 jsonltojson-1.0.0/jsonltojson/formatters.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:56:13.751989 jsonltojson-1.0.0/jsonltojson.egg-info/
+-rw-rw-rw-   0        0        0     1287 2023-06-22 10:56:13.000000 jsonltojson-1.0.0/jsonltojson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2023-06-22 10:56:13.000000 jsonltojson-1.0.0/jsonltojson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:56:13.000000 jsonltojson-1.0.0/jsonltojson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-22 10:56:13.000000 jsonltojson-1.0.0/jsonltojson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      664 2023-06-22 10:56:03.000000 jsonltojson-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 10:56:13.755981 jsonltojson-1.0.0/setup.cfg
```

### Comparing `jsonltojson-0.0.1/LICENSE.txt` & `jsonltojson-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jsonltojson-0.0.1/PKG-INFO` & `jsonltojson-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonltojson
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python package for formatting JSONL files to a single JSON array
 Author-email: Ismail Ibrahim <ismailsoftdev@gmail.com>
 Project-URL: Homepage, https://github.com/ismailsoftdev/jsonltojson
 Project-URL: Bug Tracker, https://github.com/ismailsoftdev/jsonltojson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonltojson-0.0.1/README.md` & `jsonltojson-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonltojson-0.0.1/jsonltojson/formatters.py` & `jsonltojson-1.0.0/jsonltojson/formatters.py`

 * *Files identical despite different names*

### Comparing `jsonltojson-0.0.1/jsonltojson.egg-info/PKG-INFO` & `jsonltojson-1.0.0/jsonltojson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonltojson
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python package for formatting JSONL files to a single JSON array
 Author-email: Ismail Ibrahim <ismailsoftdev@gmail.com>
 Project-URL: Homepage, https://github.com/ismailsoftdev/jsonltojson
 Project-URL: Bug Tracker, https://github.com/ismailsoftdev/jsonltojson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jsonltojson-0.0.1/pyproject.toml` & `jsonltojson-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=57.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jsonltojson"
-version = "0.0.1"
+version = "1.0.0"
 authors = [
   { name="Ismail Ibrahim", email="ismailsoftdev@gmail.com" },
 ]
 description = "A Python package for formatting JSONL files to a single JSON array"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

