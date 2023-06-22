# Comparing `tmp/wordview-0.3.0.tar.gz` & `tmp/wordview-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-0.3.0.tar", max compression
+gzip compressed data, was "wordview-0.3.1.tar", max compression
```

## Comparing `wordview-0.3.0.tar` & `wordview-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      867 2023-06-22 10:25:56.687295 wordview-0.3.0/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-06-22 10:25:56.687295 wordview-0.3.0/LICENSE
--rw-r--r--   0        0        0     4638 2023-06-22 10:25:56.687295 wordview-0.3.0/README.rst
--rw-r--r--   0        0        0      873 2023-06-22 10:26:22.163890 wordview-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4788 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/clustering/cluster.py
--rw-r--r--   0        0        0       85 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/am.py
--rw-r--r--   0        0        0     8698 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0       55 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0       75 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    11805 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8399 2023-06-22 10:25:56.783296 wordview-0.3.0/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-06-22 17:48:02.895774 wordview-0.3.1/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-06-22 17:48:02.895774 wordview-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4638 2023-06-22 17:48:02.895774 wordview-0.3.1/README.rst
+-rw-r--r--   0        0        0      873 2023-06-22 17:48:02.975774 wordview-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4788 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       48 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0       85 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     2900 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/am.py
+-rw-r--r--   0        0        0     8698 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     3962 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/mwes/mwe_utils.py
+-rw-r--r--   0        0        0       55 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0       75 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    11805 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8399 2023-06-22 17:48:02.975774 wordview-0.3.1/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 wordview-0.3.1/PKG-INFO
```

### Comparing `wordview-0.3.0/LICENSE` & `wordview-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/README.rst` & `wordview-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/pyproject.toml` & `wordview-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "0.3.0"
+version = "0.3.1"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
```

### Comparing `wordview-0.3.0/wordview/anomaly/gaussianize.py` & `wordview-0.3.1/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/anomaly/normaldist.py` & `wordview-0.3.1/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/clustering/cluster.py` & `wordview-0.3.1/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/mwes/am.py` & `wordview-0.3.1/wordview/mwes/am.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/mwes/mwe.py` & `wordview-0.3.1/wordview/mwes/mwe.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/mwes/mwe_utils.py` & `wordview-0.3.1/wordview/mwes/mwe_utils.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/preprocessing/cleaning.py` & `wordview-0.3.1/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/text_analysis/core.py` & `wordview-0.3.1/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/wordview/text_analysis/wrapper.py` & `wordview-0.3.1/wordview/text_analysis/wrapper.py`

 * *Files identical despite different names*

### Comparing `wordview-0.3.0/PKG-INFO` & `wordview-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 0.3.0
+Version: 0.3.1
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

