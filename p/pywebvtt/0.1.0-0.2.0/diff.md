# Comparing `tmp/pywebvtt-0.1.0.tar.gz` & `tmp/pywebvtt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebvtt-0.1.0.tar", max compression
+gzip compressed data, was "pywebvtt-0.2.0.tar", max compression
```

## Comparing `pywebvtt-0.1.0.tar` & `pywebvtt-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      430 2023-06-20 22:49:02.995524 pywebvtt-0.1.0/README.md
--rw-r--r--   0        0        0      374 2023-06-20 23:02:12.230459 pywebvtt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-20 22:53:20.246850 pywebvtt-0.1.0/pywebvtt/__init__.py
--rw-r--r--   0        0        0      349 2023-06-20 20:00:45.664914 pywebvtt-0.1.0/pywebvtt/errors.py
--rw-r--r--   0        0        0     1694 2023-06-20 22:40:16.565908 pywebvtt-0.1.0/pywebvtt/scene.py
--rw-r--r--   0        0        0     1940 2023-06-20 20:01:39.783783 pywebvtt-0.1.0/pywebvtt/timestamp.py
--rw-r--r--   0        0        0     1734 2023-06-20 22:40:27.226880 pywebvtt-0.1.0/pywebvtt/webvtt.py
--rw-r--r--   0        0        0      767 1970-01-01 00:00:00.000000 pywebvtt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-20 23:06:16.384820 pywebvtt-0.2.0/README.md
+-rw-r--r--   0        0        0      374 2023-06-22 18:38:35.061359 pywebvtt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      843 2023-06-22 15:22:24.556397 pywebvtt-0.2.0/pywebvtt/__init__.py
+-rw-r--r--   0        0        0      349 2023-06-20 20:00:45.664914 pywebvtt-0.2.0/pywebvtt/errors.py
+-rw-r--r--   0        0        0     7087 2023-06-22 18:25:51.261496 pywebvtt-0.2.0/pywebvtt/scene.py
+-rw-r--r--   0        0        0     3867 2023-06-22 18:37:44.360500 pywebvtt-0.2.0/pywebvtt/timestamp.py
+-rw-r--r--   0        0        0     4029 2023-06-22 17:51:16.033286 pywebvtt-0.2.0/pywebvtt/webvtt.py
+-rw-r--r--   0        0        0      850 1970-01-01 00:00:00.000000 pywebvtt-0.2.0/PKG-INFO
```

### Comparing `pywebvtt-0.1.0/PKG-INFO` & `pywebvtt-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: pywebvtt
-Version: 0.1.0
+Version: 0.2.0
 Summary: webvtt subtitle parser to traversable data struct
 Author: AbhishekKr
 Author-email: abhikumar163@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 
 ## pywebvtt
 
 > to parse WebVTT subtitle file into a traversable data structure
+>
+> [pypi/pywebvtt](https://pypi.org/project/pywebvtt/)
 
 * to run tests `poetry install && poetry run pytest`
 
 * to run example `poetry install && poetry run python examples/parse-sample.py`
 
-* sample usage
+* sample usage `pip install pywebvtt` and
 
 ```
 import pywebvtt
 
 
 scenes = pywebvtt.ParseFile('sample.vtt')
 for s in scenes:
```

