# Comparing `tmp/spoutlang-0.2.2.tar.gz` & `tmp/spoutlang-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spoutlang-0.2.2.tar", last modified: Thu Jun 22 13:47:09 2023, max compression
+gzip compressed data, was "spoutlang-0.2.3.tar", last modified: Thu Jun 22 13:59:38 2023, max compression
```

## Comparing `spoutlang-0.2.2.tar` & `spoutlang-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:47:09.262492 spoutlang-0.2.2/
--rw-r--r--   0 tapu      (1000) tapu      (1000)      421 2023-06-22 13:47:09.261484 spoutlang-0.2.2/PKG-INFO
--rw-r--r--   0 tapu      (1000) tapu      (1000)      258 2023-05-24 10:18:07.000000 spoutlang-0.2.2/README.md
--rw-r--r--   0 tapu      (1000) tapu      (1000)     1280 2023-06-22 12:12:43.000000 spoutlang-0.2.2/main.py
--rw-r--r--   0 tapu      (1000) tapu      (1000)       38 2023-06-22 13:47:09.263062 spoutlang-0.2.2/setup.cfg
--rw-r--r--   0 tapu      (1000) tapu      (1000)      759 2023-06-22 13:47:06.000000 spoutlang-0.2.2/setup.py
-drwxr-xr-x   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:47:09.169217 spoutlang-0.2.2/spout/
--rw-r--r--   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:34:38.000000 spoutlang-0.2.2/spout/__init__.py
--rw-r--r--   0 tapu      (1000) tapu      (1000)     1725 2023-06-22 12:18:56.000000 spoutlang-0.2.2/spout/environment.py
--rw-r--r--   0 tapu      (1000) tapu      (1000)     5660 2023-06-02 12:10:12.000000 spoutlang-0.2.2/spout/interpreter.py
--rw-r--r--   0 tapu      (1000) tapu      (1000)     5412 2023-06-04 13:01:22.000000 spoutlang-0.2.2/spout/lexer.py
--rw-r--r--   0 tapu      (1000) tapu      (1000)     8707 2023-06-02 11:38:47.000000 spoutlang-0.2.2/spout/parser.py
--rw-r--r--   0 tapu      (1000) tapu      (1000)      401 2023-06-04 12:55:47.000000 spoutlang-0.2.2/spout/spout.py
--rw-r--r--   0 tapu      (1000) tapu      (1000)     1288 2023-05-25 10:25:50.000000 spoutlang-0.2.2/spout/whale.py
-drwxr-xr-x   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:47:09.258518 spoutlang-0.2.2/spoutlang.egg-info/
--rw-r--r--   0 tapu      (1000) tapu      (1000)      421 2023-06-22 13:47:08.000000 spoutlang-0.2.2/spoutlang.egg-info/PKG-INFO
--rw-r--r--   0 tapu      (1000) tapu      (1000)      315 2023-06-22 13:47:09.000000 spoutlang-0.2.2/spoutlang.egg-info/SOURCES.txt
--rw-r--r--   0 tapu      (1000) tapu      (1000)        1 2023-06-22 13:47:08.000000 spoutlang-0.2.2/spoutlang.egg-info/dependency_links.txt
--rw-r--r--   0 tapu      (1000) tapu      (1000)       55 2023-06-22 13:47:08.000000 spoutlang-0.2.2/spoutlang.egg-info/entry_points.txt
--rw-r--r--   0 tapu      (1000) tapu      (1000)        5 2023-06-22 13:47:08.000000 spoutlang-0.2.2/spoutlang.egg-info/top_level.txt
+drwxr-xr-x   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:59:38.350659 spoutlang-0.2.3/
+-rw-r--r--   0 tapu      (1000) tapu      (1000)      421 2023-06-22 13:59:38.349124 spoutlang-0.2.3/PKG-INFO
+-rw-r--r--   0 tapu      (1000) tapu      (1000)      258 2023-05-24 10:18:07.000000 spoutlang-0.2.3/README.md
+-rw-r--r--   0 tapu      (1000) tapu      (1000)     1280 2023-06-22 12:12:43.000000 spoutlang-0.2.3/main.py
+-rw-r--r--   0 tapu      (1000) tapu      (1000)       38 2023-06-22 13:59:38.351345 spoutlang-0.2.3/setup.cfg
+-rw-r--r--   0 tapu      (1000) tapu      (1000)      733 2023-06-22 13:59:35.000000 spoutlang-0.2.3/setup.py
+drwxr-xr-x   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:59:38.321705 spoutlang-0.2.3/spout/
+-rw-r--r--   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:34:38.000000 spoutlang-0.2.3/spout/__init__.py
+-rw-r--r--   0 tapu      (1000) tapu      (1000)     1725 2023-06-22 12:18:56.000000 spoutlang-0.2.3/spout/environment.py
+-rw-r--r--   0 tapu      (1000) tapu      (1000)     5660 2023-06-02 12:10:12.000000 spoutlang-0.2.3/spout/interpreter.py
+-rw-r--r--   0 tapu      (1000) tapu      (1000)     5412 2023-06-04 13:01:22.000000 spoutlang-0.2.3/spout/lexer.py
+-rw-r--r--   0 tapu      (1000) tapu      (1000)     8707 2023-06-02 11:38:47.000000 spoutlang-0.2.3/spout/parser.py
+-rw-r--r--   0 tapu      (1000) tapu      (1000)      401 2023-06-04 12:55:47.000000 spoutlang-0.2.3/spout/spout.py
+-rw-r--r--   0 tapu      (1000) tapu      (1000)     1288 2023-05-25 10:25:50.000000 spoutlang-0.2.3/spout/whale.py
+drwxr-xr-x   0 tapu      (1000) tapu      (1000)        0 2023-06-22 13:59:38.345335 spoutlang-0.2.3/spoutlang.egg-info/
+-rw-r--r--   0 tapu      (1000) tapu      (1000)      421 2023-06-22 13:59:38.000000 spoutlang-0.2.3/spoutlang.egg-info/PKG-INFO
+-rw-r--r--   0 tapu      (1000) tapu      (1000)      315 2023-06-22 13:59:38.000000 spoutlang-0.2.3/spoutlang.egg-info/SOURCES.txt
+-rw-r--r--   0 tapu      (1000) tapu      (1000)        1 2023-06-22 13:59:38.000000 spoutlang-0.2.3/spoutlang.egg-info/dependency_links.txt
+-rw-r--r--   0 tapu      (1000) tapu      (1000)       55 2023-06-22 13:59:38.000000 spoutlang-0.2.3/spoutlang.egg-info/entry_points.txt
+-rw-r--r--   0 tapu      (1000) tapu      (1000)       11 2023-06-22 13:59:38.000000 spoutlang-0.2.3/spoutlang.egg-info/top_level.txt
```

### Comparing `spoutlang-0.2.2/main.py` & `spoutlang-0.2.3/main.py`

 * *Files identical despite different names*

### Comparing `spoutlang-0.2.2/setup.py` & `spoutlang-0.2.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import setup, find_packages
 
 # Build command: python setup.py sdist
 # Upload command: twine upload dist/*
 
 setup(
     name = 'spoutlang',
-    version = '0.2.2',
+    version = '0.2.3',
     author = 'Tasfiqul Tapu',
     author_email = 'iamtasfiqultapu@gmail.com',
     license = 'MIT',
     description = 'An interpreted programming language aimed at demistifying bit manipulation.',
     url = 'https://github.com/TasfiqulTapu/spout',
     py_modules = ['main'],
-    package_dir={
-        "spout": "spout"
-    },
+    packages=["spout"],
     install_requires = [],
     python_requires='>=3.7',
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     entry_points = '''
```

### Comparing `spoutlang-0.2.2/spout/environment.py` & `spoutlang-0.2.3/spout/environment.py`

 * *Files identical despite different names*

### Comparing `spoutlang-0.2.2/spout/interpreter.py` & `spoutlang-0.2.3/spout/interpreter.py`

 * *Files identical despite different names*

### Comparing `spoutlang-0.2.2/spout/lexer.py` & `spoutlang-0.2.3/spout/lexer.py`

 * *Files identical despite different names*

### Comparing `spoutlang-0.2.2/spout/parser.py` & `spoutlang-0.2.3/spout/parser.py`

 * *Files identical despite different names*

### Comparing `spoutlang-0.2.2/spout/whale.py` & `spoutlang-0.2.3/spout/whale.py`

 * *Files identical despite different names*

