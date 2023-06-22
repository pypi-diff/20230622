# Comparing `tmp/emreader-0.1.4.tar.gz` & `tmp/emreader-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emreader-0.1.4.tar", max compression
+gzip compressed data, was "emreader-0.1.5.tar", max compression
```

## Comparing `emreader-0.1.4.tar` & `emreader-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.4/README.md
--rw-r--r--   0        0        0      851 2023-06-22 19:44:08.735239 emreader-0.1.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.4/src/__init__.py
--rw-r--r--   0        0        0     3689 2023-06-22 19:20:24.490676 emreader-0.1.4/src/app.py
--rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.4/src/core/__init__.py
--rw-r--r--   0        0        0      159 2023-06-22 19:35:57.735123 emreader-0.1.4/src/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     8713 2023-06-22 19:35:57.738541 emreader-0.1.4/src/core/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     4634 2023-06-22 19:37:13.102413 emreader-0.1.4/src/core/__pycache__/eml.cpython-311.pyc
--rw-r--r--   0        0        0     3256 2023-06-22 19:37:13.099936 emreader-0.1.4/src/core/__pycache__/parse_tab.cpython-311.pyc
--rw-r--r--   0        0        0     7680 2023-06-22 19:37:13.101358 emreader-0.1.4/src/core/__pycache__/util.cpython-311.pyc
--rw-r--r--   0        0        0     6062 2023-06-22 19:20:24.471228 emreader-0.1.4/src/core/base.py
--rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.4/src/core/eml.py
--rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.4/src/core/parse_tab.py
--rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.4/src/core/util.py
--rw-r--r--   0        0        0      150 2023-06-22 19:41:33.502317 emreader-0.1.4/src/runner.py
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 emreader-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.5/README.md
+-rw-r--r--   0        0        0      854 2023-06-22 19:48:06.513075 emreader-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.5/src/__init__.py
+-rw-r--r--   0        0        0     3680 2023-06-22 19:47:51.862349 emreader-0.1.5/src/app.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.5/src/core/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-22 19:35:57.735123 emreader-0.1.5/src/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8713 2023-06-22 19:35:57.738541 emreader-0.1.5/src/core/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     4634 2023-06-22 19:37:13.102413 emreader-0.1.5/src/core/__pycache__/eml.cpython-311.pyc
+-rw-r--r--   0        0        0     3256 2023-06-22 19:37:13.099936 emreader-0.1.5/src/core/__pycache__/parse_tab.cpython-311.pyc
+-rw-r--r--   0        0        0     7680 2023-06-22 19:37:13.101358 emreader-0.1.5/src/core/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0     6062 2023-06-22 19:20:24.471228 emreader-0.1.5/src/core/base.py
+-rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.5/src/core/eml.py
+-rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.5/src/core/parse_tab.py
+-rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.5/src/core/util.py
+-rw-r--r--   0        0        0      150 2023-06-22 19:41:33.502317 emreader-0.1.5/src/runner.py
+-rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 emreader-0.1.5/PKG-INFO
```

### Comparing `emreader-0.1.4/pyproject.toml` & `emreader-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "emreader"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["themba <themba@advantch.com>"]
 readme = "README.md"
 license = "Commercial"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
@@ -30,12 +30,12 @@
 tzdata = "^2023.3"
 wheel = "^0.40.0"
 rich = "^13.4.2"
 streamlit = "^1.23.1"
 pymupdf = "^1.22.5"
 
 [tool.poetry.scripts]
-start = "src.runner:run"
+emreader = "src.runner:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `emreader-0.1.4/src/app.py` & `emreader-0.1.5/src/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 
 import pandas as pd
 import rich
 import streamlit as st
 import zipfile
-from src.core.base import extract_from_files
-from src.core.util import transform_dataframe
-from src.core.eml import extract_emails
+from .core.base import extract_from_files
+from .core.util import transform_dataframe
+from .core.eml import extract_emails
 
 
 @st.cache_data
 def convert_df(df):
     # IMPORTANT: Cache the conversion to prevent computation on every rerun
     return df.to_csv().encode("utf-8")
```

### Comparing `emreader-0.1.4/src/core/__pycache__/base.cpython-311.pyc` & `emreader-0.1.5/src/core/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/src/core/__pycache__/eml.cpython-311.pyc` & `emreader-0.1.5/src/core/__pycache__/eml.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/src/core/__pycache__/parse_tab.cpython-311.pyc` & `emreader-0.1.5/src/core/__pycache__/parse_tab.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/src/core/__pycache__/util.cpython-311.pyc` & `emreader-0.1.5/src/core/__pycache__/util.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/src/core/base.py` & `emreader-0.1.5/src/core/base.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/src/core/eml.py` & `emreader-0.1.5/src/core/eml.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/src/core/parse_tab.py` & `emreader-0.1.5/src/core/parse_tab.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/src/core/util.py` & `emreader-0.1.5/src/core/util.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.4/PKG-INFO` & `emreader-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emreader
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 License: Commercial
 Author: themba
 Author-email: themba@advantch.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

