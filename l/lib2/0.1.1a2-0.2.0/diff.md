# Comparing `tmp/lib2-0.1.1a2.tar.gz` & `tmp/lib2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib2-0.1.1a2.tar", max compression
+gzip compressed data, was "lib2-0.2.0.tar", max compression
```

## Comparing `lib2-0.1.1a2.tar` & `lib2-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-22 17:42:57.977891 lib2-0.1.1a2/README.md
--rw-r--r--   0        0        0       69 2023-06-22 17:42:57.977891 lib2-0.1.1a2/lib2/__init__.py
--rw-r--r--   0        0        0      697 2023-06-22 17:42:57.977891 lib2-0.1.1a2/lib2/preprocessing.py
--rw-r--r--   0        0        0      202 2023-06-22 17:42:57.977891 lib2-0.1.1a2/lib2/version_util.py
--rw-r--r--   0        0        0      300 2023-06-22 17:42:57.977891 lib2-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 lib2-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-22 17:54:12.697481 lib2-0.2.0/README.md
+-rw-r--r--   0        0        0       69 2023-06-22 17:54:12.697481 lib2-0.2.0/lib2/__init__.py
+-rw-r--r--   0        0        0      697 2023-06-22 17:54:12.697481 lib2-0.2.0/lib2/preprocessing.py
+-rw-r--r--   0        0        0      202 2023-06-22 17:54:12.697481 lib2-0.2.0/lib2/version_util.py
+-rw-r--r--   0        0        0      298 2023-06-22 17:54:24.361553 lib2-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 lib2-0.2.0/PKG-INFO
```

### Comparing `lib2-0.1.1a2/lib2/preprocessing.py` & `lib2-0.2.0/lib2/preprocessing.py`

 * *Files identical despite different names*

