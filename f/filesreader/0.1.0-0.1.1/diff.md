# Comparing `tmp/filesreader-0.1.0.tar.gz` & `tmp/filesreader-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesreader-0.1.0.tar", max compression
+gzip compressed data, was "filesreader-0.1.1.tar", max compression
```

## Comparing `filesreader-0.1.0.tar` & `filesreader-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11341 2023-06-22 10:48:37.820010 filesreader-0.1.0/LICENSE
--rw-r--r--   0        0        0      449 2023-06-22 10:49:22.084768 filesreader-0.1.0/README.md
--rw-r--r--   0        0        0      510 2023-06-22 10:03:49.003886 filesreader-0.1.0/filesreader.py
--rw-r--r--   0        0        0      359 2023-06-22 10:53:26.617111 filesreader-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 filesreader-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11341 2023-06-22 10:48:37.820010 filesreader-0.1.1/LICENSE
+-rw-r--r--   0        0        0      450 2023-06-22 11:19:05.186309 filesreader-0.1.1/README.md
+-rw-r--r--   0        0        0      510 2023-06-22 10:03:49.003886 filesreader-0.1.1/filesreader.py
+-rw-r--r--   0        0        0      359 2023-06-22 11:19:12.687130 filesreader-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 filesreader-0.1.1/PKG-INFO
```

### Comparing `filesreader-0.1.0/LICENSE` & `filesreader-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `filesreader-0.1.0/PKG-INFO` & `filesreader-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesreader
-Version: 0.1.0
+Version: 0.1.1
 Summary: A small project to read files
 Author: Sergio lema
 Author-email: lema.sergio.85@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -18,10 +18,10 @@
 ## Usage
 
 ```
 reader = FileReader("path/of/the_file.txt")
 lines = reader.read_all_lines()
 ```
 
-The resources context is already managed inside the controller. An FileNotFoundError will be thrown if the file doesn't exist. The returned lines won't have the special characters `\n` or `\r`.
+The resources context is already managed inside the constructor. An FileNotFoundError will be thrown if the file doesn't exist. The returned lines won't have the special characters `\n` or `\r`.
```

