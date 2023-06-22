# Comparing `tmp/emreader-0.1.2.tar.gz` & `tmp/emreader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emreader-0.1.2.tar", max compression
+gzip compressed data, was "emreader-0.1.3.tar", max compression
```

## Comparing `emreader-0.1.2.tar` & `emreader-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.2/README.md
--rw-r--r--   0        0        0      849 2023-06-22 19:29:57.733960 emreader-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.2/src/__init__.py
--rw-r--r--   0        0        0     3689 2023-06-22 19:20:24.490676 emreader-0.1.2/src/app.py
--rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.2/src/core/__init__.py
--rw-r--r--   0        0        0     6062 2023-06-22 19:20:24.471228 emreader-0.1.2/src/core/base.py
--rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.2/src/core/eml.py
--rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.2/src/core/parse_tab.py
--rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.2/src/core/util.py
--rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 emreader-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      246 2023-06-22 19:29:06.216827 emreader-0.1.3/README.md
+-rw-r--r--   0        0        0      855 2023-06-22 19:38:20.566536 emreader-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-20 17:45:55.551587 emreader-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0     3689 2023-06-22 19:20:24.490676 emreader-0.1.3/src/app.py
+-rw-r--r--   0        0        0        0 2023-06-22 19:19:46.699802 emreader-0.1.3/src/core/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-22 19:35:57.735123 emreader-0.1.3/src/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8713 2023-06-22 19:35:57.738541 emreader-0.1.3/src/core/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     4634 2023-06-22 19:37:13.102413 emreader-0.1.3/src/core/__pycache__/eml.cpython-311.pyc
+-rw-r--r--   0        0        0     3256 2023-06-22 19:37:13.099936 emreader-0.1.3/src/core/__pycache__/parse_tab.cpython-311.pyc
+-rw-r--r--   0        0        0     7680 2023-06-22 19:37:13.101358 emreader-0.1.3/src/core/__pycache__/util.cpython-311.pyc
+-rw-r--r--   0        0        0     6062 2023-06-22 19:20:24.471228 emreader-0.1.3/src/core/base.py
+-rw-r--r--   0        0        0     2257 2023-06-22 19:20:24.473512 emreader-0.1.3/src/core/eml.py
+-rw-r--r--   0        0        0     2326 2023-06-20 18:53:15.483548 emreader-0.1.3/src/core/parse_tab.py
+-rw-r--r--   0        0        0     5540 2023-06-20 18:45:11.583746 emreader-0.1.3/src/core/util.py
+-rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 emreader-0.1.3/PKG-INFO
```

### Comparing `emreader-0.1.2/pyproject.toml` & `emreader-0.1.3/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "emreader"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["themba <themba@advantch.com>"]
 readme = "README.md"
-license = ""
+license = "Commercial"
 packages = [{include = "src"}]
 
 [tool.poetry.dependencies]
-python =   ">=3.9,<3.9.7 || >3.9.7,<4.0"
-camelot-py = "^0.9.0"
+python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 cffi = "^1.15.1"
 chardet = "^5.1.0"
 charset-normalizer = "^3.1.0"
 click = "^8.1.3"
 cryptography = "^41.0.1"
 distro = "^1.8.0"
 et-xmlfile = "^1.1.0"
@@ -28,14 +27,15 @@
 pytz = "^2023.3"
 setuptools = "^67.7.2"
 tabula-py = "2.7.0"
 tzdata = "^2023.3"
 wheel = "^0.40.0"
 rich = "^13.4.2"
 streamlit = "^1.23.1"
+pymupdf = "^1.22.5"
 
 [tool.poetry.scripts]
 run = "streamlit run app.py"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `emreader-0.1.2/src/app.py` & `emreader-0.1.3/src/app.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.2/src/core/base.py` & `emreader-0.1.3/src/core/base.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.2/src/core/eml.py` & `emreader-0.1.3/src/core/eml.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.2/src/core/parse_tab.py` & `emreader-0.1.3/src/core/parse_tab.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.2/src/core/util.py` & `emreader-0.1.3/src/core/util.py`

 * *Files identical despite different names*

### Comparing `emreader-0.1.2/PKG-INFO` & `emreader-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: emreader
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
+License: Commercial
 Author: themba
 Author-email: themba@advantch.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
+Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyPDF2 (==2.0)
-Requires-Dist: camelot-py (>=0.9.0,<0.10.0)
 Requires-Dist: cffi (>=1.15.1,<2.0.0)
 Requires-Dist: chardet (>=5.1.0,<6.0.0)
 Requires-Dist: charset-normalizer (>=3.1.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: cryptography (>=41.0.1,<42.0.0)
 Requires-Dist: distro (>=1.8.0,<2.0.0)
 Requires-Dist: et-xmlfile (>=1.1.0,<2.0.0)
 Requires-Dist: numpy (>=1.25.0,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<5.0.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pip (>=23.1.2,<24.0.0)
 Requires-Dist: pycparser (>=2.21,<3.0)
+Requires-Dist: pymupdf (>=1.22.5,<2.0.0)
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: setuptools (>=67.7.2,<68.0.0)
 Requires-Dist: streamlit (>=1.23.1,<2.0.0)
 Requires-Dist: tabula-py (==2.7.0)
 Requires-Dist: tzdata (>=2023.3,<2024.0)
```

