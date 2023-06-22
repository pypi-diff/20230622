# Comparing `tmp/stdlib_list-0.9.0.tar.gz` & `tmp/stdlib_list-0.9.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stdlib_list-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "stdlib_list-0.9.0rc0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `stdlib_list-0.9.0.tar` & `stdlib_list-0.9.0rc0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1077 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/LICENSE
--rw-r--r--   0        0        0     1928 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/README.md
--rw-r--r--   0        0        0     1567 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      350 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/__init__.py
--rw-r--r--   0        0        0     2922 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/base.py
--rw-r--r--   0        0        0     4720 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/lists/2.6.txt
--rw-r--r--   0        0        0    27222 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/lists/2.7.txt
--rw-r--r--   0        0        0    18293 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/lists/3.10.txt
--rw-r--r--   0        0        0    18405 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/lists/3.11.txt
--rw-r--r--   0        0        0     3514 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/lists/3.2.txt
--rw-r--r--   0        0        0     3618 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/lists/3.3.txt
--rw-r--r--   0        0        0    31024 2023-06-22 04:02:41.652160 stdlib_list-0.9.0/stdlib_list/lists/3.4.txt
--rw-r--r--   0        0        0    32711 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/stdlib_list/lists/3.5.txt
--rw-r--r--   0        0        0    34003 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/stdlib_list/lists/3.6.txt
--rw-r--r--   0        0        0    35554 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/stdlib_list/lists/3.7.txt
--rw-r--r--   0        0        0    36675 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/stdlib_list/lists/3.8.txt
--rw-r--r--   0        0        0    34880 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/stdlib_list/lists/3.9.txt
--rw-r--r--   0        0        0        0 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/stdlib_list/py.typed
--rw-r--r--   0        0        0        0 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0      952 2023-06-22 04:02:41.656160 stdlib_list-0.9.0/tests/test_base.py
--rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 stdlib_list-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/LICENSE
+-rw-r--r--   0        0        0     1928 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/README.md
+-rw-r--r--   0        0        0     1567 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/pyproject.toml
+-rw-r--r--   0        0        0      353 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/__init__.py
+-rw-r--r--   0        0        0     2922 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/base.py
+-rw-r--r--   0        0        0     4720 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/2.6.txt
+-rw-r--r--   0        0        0    27222 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/2.7.txt
+-rw-r--r--   0        0        0    18293 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.10.txt
+-rw-r--r--   0        0        0    18405 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.11.txt
+-rw-r--r--   0        0        0     3514 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.2.txt
+-rw-r--r--   0        0        0     3618 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.3.txt
+-rw-r--r--   0        0        0    31024 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.4.txt
+-rw-r--r--   0        0        0    32711 2023-06-22 03:57:34.675631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.5.txt
+-rw-r--r--   0        0        0    34003 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.6.txt
+-rw-r--r--   0        0        0    35554 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.7.txt
+-rw-r--r--   0        0        0    36675 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.8.txt
+-rw-r--r--   0        0        0    34880 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/lists/3.9.txt
+-rw-r--r--   0        0        0        0 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/stdlib_list/py.typed
+-rw-r--r--   0        0        0        0 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/tests/__init__.py
+-rw-r--r--   0        0        0      952 2023-06-22 03:57:34.679631 stdlib_list-0.9.0rc0/tests/test_base.py
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 stdlib_list-0.9.0rc0/PKG-INFO
```

### Comparing `stdlib_list-0.9.0/LICENSE` & `stdlib_list-0.9.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/README.md` & `stdlib_list-0.9.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/pyproject.toml` & `stdlib_list-0.9.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/base.py` & `stdlib_list-0.9.0rc0/stdlib_list/base.py`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/2.6.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/2.6.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/2.7.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/2.7.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.10.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.10.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.11.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.11.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.2.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.2.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.3.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.3.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.4.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.4.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.5.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.5.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.6.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.6.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.7.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.7.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.8.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.8.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/stdlib_list/lists/3.9.txt` & `stdlib_list-0.9.0rc0/stdlib_list/lists/3.9.txt`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/tests/test_base.py` & `stdlib_list-0.9.0rc0/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `stdlib_list-0.9.0/PKG-INFO` & `stdlib_list-0.9.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stdlib-list
-Version: 0.9.0
+Version: 0.9.0rc0
 Summary: A list of Python Standard Libraries (2.7 through 3.9).
 Author-email: Jack Maney <jackmaney@gmail.com>
 Maintainer-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: build ; extra == "dev"
 Requires-Dist: stdlib-list[test,lint,doc] ; extra == "dev"
```

