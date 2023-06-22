# Comparing `tmp/emreader-0.1.0.tar.gz` & `tmp/emreader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emreader-0.1.0.tar", max compression
+gzip compressed data, was "emreader-0.1.1.tar", max compression
```

## Comparing `emreader-0.1.0.tar` & `emreader-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      480 2023-06-22 19:23:01.425232 emreader-0.1.0/README.md
--rw-r--r--   0        0        0      899 2023-06-22 19:23:01.419431 emreader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     3689 2023-06-22 19:20:24.490676 emreader-0.1.0/src/app.py
--rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.0/src/core/__init__.py
--rw-r--r--   0        0        0     6062 2023-06-22 19:20:24.471228 emreader-0.1.0/src/core/base.py
--rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.0/src/core/eml.py
--rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.0/src/core/parse_tab.py
--rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.0/src/core/util.py
--rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 emreader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      480 2023-06-22 19:23:01.425232 emreader-0.1.1/README.md
+-rw-r--r--   0        0        0      870 2023-06-22 19:28:13.033507 emreader-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     3689 2023-06-22 19:20:24.490676 emreader-0.1.1/src/app.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.1/src/core/__init__.py
+-rw-r--r--   0        0        0     6062 2023-06-22 19:20:24.471228 emreader-0.1.1/src/core/base.py
+-rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.1/src/core/eml.py
+-rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.1/src/core/parse_tab.py
+-rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.1/src/core/util.py
+-rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 emreader-0.1.1/PKG-INFO
```

### Comparing `emreader-0.1.0/pyproject.toml` & `emreader-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emreader"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["themba <themba@advantch.com>"]
 readme = "README.md"
 license = ""
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
@@ -26,15 +26,15 @@
 PyPDF2 = "2.0"
 python-dateutil = "^2.8.2"
 pytz = "^2023.3"
 setuptools = "^67.7.2"
 tabula-py = "2.7.0"
 tzdata = "^2023.3"
 wheel = "^0.40.0"
-camelot = {extras = ["cv"], version = "^12.6.29"}
+camelot = "^12.6.29"
 rich = "^13.4.2"
 streamlit = "^1.23.1"
 
 [tool.poetry.scripts]
 run = "streamlit run app.py"
 
 [build-system]
```

### Comparing `emreader-0.1.0/src/app.py` & `emreader-0.1.1/src/app.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.0/src/core/base.py` & `emreader-0.1.1/src/core/base.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.0/src/core/eml.py` & `emreader-0.1.1/src/core/eml.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.0/src/core/parse_tab.py` & `emreader-0.1.1/src/core/parse_tab.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.0/src/core/util.py` & `emreader-0.1.1/src/core/util.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.0/PKG-INFO` & `emreader-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: emreader
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: themba
 Author-email: themba@advantch.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyPDF2 (==2.0)
+Requires-Dist: camelot (>=12.6.29,<13.0.0)
 Requires-Dist: camelot-py (>=0.9.0,<0.10.0)
-Requires-Dist: camelot[cv] (>=12.6.29,<13.0.0)
 Requires-Dist: cffi (>=1.15.1,<2.0.0)
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: distro (>=1.8.0,<2.0.0)
 Requires-Dist: et-xmlfile (>=1.1.0,<2.0.0)
```

