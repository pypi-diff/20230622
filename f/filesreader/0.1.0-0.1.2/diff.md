# Comparing `tmp/filesreader-0.1.0.tar.gz` & `tmp/filesreader-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesreader-0.1.0.tar", max compression
+gzip compressed data, was "filesreader-0.1.2.tar", max compression
```

## Comparing `filesreader-0.1.0.tar` & `filesreader-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11341 2023-06-22 10:48:37.820010 filesreader-0.1.0/LICENSE
--rw-r--r--   0        0        0      449 2023-06-22 10:49:22.084768 filesreader-0.1.0/README.md
--rw-r--r--   0        0        0      510 2023-06-22 10:03:49.003886 filesreader-0.1.0/filesreader.py
--rw-r--r--   0        0        0      359 2023-06-22 10:53:26.617111 filesreader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 filesreader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-06-22 10:48:37.820010 filesreader-0.1.2/LICENSE
+-rw-r--r--   0        0        0      450 2023-06-22 11:26:20.779344 filesreader-0.1.2/README.md
+-rw-r--r--   0        0        0      510 2023-06-22 10:03:49.003886 filesreader-0.1.2/filesreader.py
+-rw-r--r--   0        0        0      437 2023-06-22 11:34:04.324005 filesreader-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1072 1970-01-01 00:00:00.000000 filesreader-0.1.2/PKG-INFO
```

### Comparing `filesreader-0.1.0/LICENSE` & `filesreader-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `filesreader-0.1.0/PKG-INFO` & `filesreader-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: filesreader
-Version: 0.1.0
+Version: 0.1.2
 Summary: A small project to read files
+Home-page: https://github.com/serlesen/filesreader
+License: Apache-2.0
 Author: Sergio lema
 Author-email: lema.sergio.85@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/serlesen/filesreader
 Description-Content-Type: text/markdown
 
 # Files Reader Project
 
-Small project to automatically read all the lines from a line without taking into account resources context and the new lines symbol.
+Small project to automatically read all the lines from a file without taking into account resources context and the new lines symbol.
 
 ## Usage
 
 ```
 reader = FileReader("path/of/the_file.txt")
 lines = reader.read_all_lines()
 ```
 
-The resources context is already managed inside the controller. An FileNotFoundError will be thrown if the file doesn't exist. The returned lines won't have the special characters `\n` or `\r`.
+The resources context is already managed inside the constructor. An FileNotFoundError will be thrown if the file doesn't exist. The returned lines won't have the special characters `\n` or `\r`.
```

