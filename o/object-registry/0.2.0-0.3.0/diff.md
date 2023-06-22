# Comparing `tmp/object_registry-0.2.0.tar.gz` & `tmp/object_registry-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "object_registry-0.2.0.tar", max compression
+gzip compressed data, was "object_registry-0.3.0.tar", max compression
```

## Comparing `object_registry-0.2.0.tar` & `object_registry-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    35093 2023-06-18 14:46:21.918955 object_registry-0.2.0/LICENSE
--rw-r--r--   0        0        0      618 2023-06-18 14:00:45.865151 object_registry-0.2.0/README.md
--rw-r--r--   0        0        0     1512 2023-06-20 00:07:13.544118 object_registry-0.2.0/object_registry/__init__.py
--rw-r--r--   0        0        0      459 2023-06-19 23:49:21.403205 object_registry-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 object_registry-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35093 2023-06-18 14:46:21.918955 object_registry-0.3.0/LICENSE
+-rw-r--r--   0        0        0      618 2023-06-18 14:00:45.865151 object_registry-0.3.0/README.md
+-rw-r--r--   0        0        0     2236 2023-06-22 00:00:25.496605 object_registry-0.3.0/object_registry/__init__.py
+-rw-r--r--   0        0        0      459 2023-06-22 00:02:22.538363 object_registry-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1203 1970-01-01 00:00:00.000000 object_registry-0.3.0/PKG-INFO
```

### Comparing `object_registry-0.2.0/LICENSE` & `object_registry-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `object_registry-0.2.0/README.md` & `object_registry-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `object_registry-0.2.0/PKG-INFO` & `object_registry-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: object-registry
-Version: 0.2.0
+Version: 0.3.0
 Summary: Keep track of all instantiated objects of a class.
 Home-page: https://gitlab.com/deepadmax/object-registry
 License: GPL-3.0-or-later
 Author: Maximillian Strand
 Author-email: maxi@millian.se
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

