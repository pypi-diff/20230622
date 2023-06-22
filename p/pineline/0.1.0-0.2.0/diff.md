# Comparing `tmp/pineline-0.1.0.tar.gz` & `tmp/pineline-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pineline-0.1.0.tar", max compression
+gzip compressed data, was "pineline-0.2.0.tar", max compression
```

## Comparing `pineline-0.1.0.tar` & `pineline-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0       11 2023-02-15 17:59:14.486836 pineline-0.1.0/README.md
--rw-r--r--   0        0        0      615 2023-02-15 18:00:08.046865 pineline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-02-15 18:00:08.046865 pineline-0.1.0/src/pineline/__init__.py
--rw-r--r--   0        0        0      754 1970-01-01 00:00:00.000000 pineline-0.1.0/setup.py
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 pineline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       11 2023-06-22 16:52:29.119192 pineline-0.2.0/README.md
+-rw-r--r--   0        0        0      857 2023-06-22 16:53:10.582503 pineline-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-22 16:53:10.586503 pineline-0.2.0/src/pineline/__init__.py
+-rw-r--r--   0        0        0      686 1970-01-01 00:00:00.000000 pineline-0.2.0/PKG-INFO
```

### Comparing `pineline-0.1.0/PKG-INFO` & `pineline-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pineline
-Version: 0.1.0
+Version: 0.2.0
 Summary: Theory predictions for PDF fitting
-Author: Alessandro Candido
-Author-email: candido.ale@gmail.com
-Requires-Python: >=3.8,<3.11
+Author: Andrea Barontini
+Author-email: andrea.barontini@mi.infn.it
+Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: eko (>=0.12.0,<0.13.0)
-Requires-Dist: pineappl (>=0.5.9,<0.6.0)
-Requires-Dist: pinefarm[full] (>=0.2.2,<0.3.0)
-Requires-Dist: pineko (>=0.3.3,<0.4.0)
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: full
+Requires-Dist: eko (>=0.13.5,<0.14.0)
+Requires-Dist: pineappl (>=0.6.0,<0.7.0)
+Requires-Dist: pinefarm (==0.3.0) ; extra == "full"
+Requires-Dist: pineko (>=0.4.1,<0.5.0)
 Description-Content-Type: text/markdown
 
 # Pineline
```

