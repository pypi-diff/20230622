# Comparing `tmp/betainc-0.2.6.tar.gz` & `tmp/betainc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betainc-0.2.6.tar", max compression
+gzip compressed data, was "betainc-0.3.0.tar", max compression
```

## Comparing `betainc-0.2.6.tar` & `betainc-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       50 2023-06-22 06:19:20.964542 betainc-0.2.6/betainc/__init__.py
--rw-r--r--   0        0        0   261419 2023-06-22 03:52:37.829434 betainc-0.2.6/betainc/betainc.c
--rw-r--r--   0        0        0     1761 2023-06-22 03:52:37.829434 betainc-0.2.6/betainc/betainc.pyx
--rw-r--r--   0        0        0     1289 2023-06-22 03:52:37.831434 betainc-0.2.6/build.py
--rw-r--r--   0        0        0      395 2023-06-22 06:19:41.434298 betainc-0.2.6/pyproject.toml
--rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 betainc-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-22 06:35:07.295255 betainc-0.3.0/betainc/__init__.py
+-rw-r--r--   0        0        0   261419 2023-06-22 03:52:37.829434 betainc-0.3.0/betainc/betainc.c
+-rw-r--r--   0        0        0     1761 2023-06-22 03:52:37.829434 betainc-0.3.0/betainc/betainc.pyx
+-rw-r--r--   0        0        0     1289 2023-06-22 03:52:37.831434 betainc-0.3.0/build.py
+-rw-r--r--   0        0        0      395 2023-06-22 06:35:19.845105 betainc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      423 1970-01-01 00:00:00.000000 betainc-0.3.0/PKG-INFO
```

### Comparing `betainc-0.2.6/betainc/betainc.c` & `betainc-0.3.0/betainc/betainc.c`

 * *Files identical despite different names*

### Comparing `betainc-0.2.6/betainc/betainc.pyx` & `betainc-0.3.0/betainc/betainc.pyx`

 * *Files identical despite different names*

### Comparing `betainc-0.2.6/build.py` & `betainc-0.3.0/build.py`

 * *Files identical despite different names*

