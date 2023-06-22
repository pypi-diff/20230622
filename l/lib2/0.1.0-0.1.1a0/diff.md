# Comparing `tmp/lib2-0.1.0.tar.gz` & `tmp/lib2-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib2-0.1.0.tar", max compression
+gzip compressed data, was "lib2-0.1.1a0.tar", max compression
```

## Comparing `lib2-0.1.0.tar` & `lib2-0.1.1a0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-06-22 16:21:55.253423 lib2-0.1.0/README.md
--rw-r--r--   0        0        0      344 2023-06-22 16:46:19.364191 lib2-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-06-22 16:26:55.633376 lib2-0.1.0/src/lib2/__init__.py
--rw-r--r--   0        0        0      697 2023-06-22 16:31:52.369999 lib2-0.1.0/src/lib2/preprocessing.py
--rw-r--r--   0        0        0      228 2023-06-22 16:32:52.527746 lib2-0.1.0/src/lib2/version_util.py
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 lib2-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-22 17:14:08.961948 lib2-0.1.1a0/README.md
+-rw-r--r--   0        0        0       69 2023-06-22 17:06:53.229148 lib2-0.1.1a0/lib2/__init__.py
+-rw-r--r--   0        0        0      697 2023-06-22 16:31:52.369999 lib2-0.1.1a0/lib2/preprocessing.py
+-rw-r--r--   0        0        0      228 2023-06-22 16:32:52.527746 lib2-0.1.1a0/lib2/version_util.py
+-rw-r--r--   0        0        0      300 2023-06-22 17:16:14.624984 lib2-0.1.1a0/pyproject.toml
+-rw-r--r--   0        0        0      465 1970-01-01 00:00:00.000000 lib2-0.1.1a0/PKG-INFO
```

### Comparing `lib2-0.1.0/src/lib2/preprocessing.py` & `lib2-0.1.1a0/lib2/preprocessing.py`

 * *Files identical despite different names*

