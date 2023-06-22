# Comparing `tmp/oapi3-1.4.2.tar.gz` & `tmp/oapi3-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oapi3-1.4.2.tar", last modified: Fri Apr 21 10:01:00 2023, max compression
+gzip compressed data, was "oapi3-1.4.3.tar", last modified: Thu Jun 22 12:58:57 2023, max compression
```

## Comparing `oapi3-1.4.2.tar` & `oapi3-1.4.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.704018 oapi3-1.4.2/
--rw-r--r--   0 motor      (501) staff       (20)     1071 2022-09-06 13:51:56.000000 oapi3-1.4.2/LICENSE
--rw-r--r--   0 motor      (501) staff       (20)      507 2023-04-21 10:01:00.703901 oapi3-1.4.2/PKG-INFO
--rw-r--r--   0 motor      (501) staff       (20)       53 2022-09-06 13:51:56.000000 oapi3-1.4.2/README.md
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.702008 oapi3-1.4.2/oapi3/
--rw-r--r--   0 motor      (501) staff       (20)      617 2023-01-19 13:11:11.000000 oapi3-1.4.2/oapi3/__init__.py
--rw-r--r--   0 motor      (501) staff       (20)     4957 2022-09-06 13:51:56.000000 oapi3-1.4.2/oapi3/client.py
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.703240 oapi3-1.4.2/oapi3/entities/
--rw-r--r--   0 motor      (501) staff       (20)      946 2023-01-23 09:13:39.000000 oapi3-1.4.2/oapi3/entities/__init__.py
--rw-r--r--   0 motor      (501) staff       (20)      192 2023-01-17 11:57:21.000000 oapi3-1.4.2/oapi3/entities/base.py
--rw-r--r--   0 motor      (501) staff       (20)     2679 2023-01-31 12:08:56.000000 oapi3-1.4.2/oapi3/entities/media_types.py
--rw-r--r--   0 motor      (501) staff       (20)     3701 2023-01-20 11:08:24.000000 oapi3-1.4.2/oapi3/entities/operations.py
--rw-r--r--   0 motor      (501) staff       (20)    10088 2023-04-20 13:14:43.000000 oapi3-1.4.2/oapi3/entities/parameters.py
--rw-r--r--   0 motor      (501) staff       (20)     2626 2023-01-19 14:12:56.000000 oapi3-1.4.2/oapi3/entities/paths.py
--rw-r--r--   0 motor      (501) staff       (20)      729 2023-01-17 14:18:00.000000 oapi3-1.4.2/oapi3/entities/schema.py
--rw-r--r--   0 motor      (501) staff       (20)     3654 2023-01-20 11:24:48.000000 oapi3-1.4.2/oapi3/exceptions.py
--rw-r--r--   0 motor      (501) staff       (20)     5860 2023-01-23 09:31:05.000000 oapi3-1.4.2/oapi3/iktomi.py
--rw-r--r--   0 motor      (501) staff       (20)     2758 2023-01-19 13:39:26.000000 oapi3-1.4.2/oapi3/jsonschema_validator.py
--rw-r--r--   0 motor      (501) staff       (20)     4349 2023-01-19 13:12:42.000000 oapi3-1.4.2/oapi3/resolve.py
--rw-r--r--   0 motor      (501) staff       (20)     3616 2023-04-20 11:57:16.000000 oapi3-1.4.2/oapi3/schema.py
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.702515 oapi3-1.4.2/oapi3.egg-info/
--rw-r--r--   0 motor      (501) staff       (20)      507 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/PKG-INFO
--rw-r--r--   0 motor      (501) staff       (20)      614 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/SOURCES.txt
--rw-r--r--   0 motor      (501) staff       (20)        1 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/dependency_links.txt
--rw-r--r--   0 motor      (501) staff       (20)       41 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/requires.txt
--rw-r--r--   0 motor      (501) staff       (20)       12 2023-04-21 10:01:00.000000 oapi3-1.4.2/oapi3.egg-info/top_level.txt
--rw-r--r--   0 motor      (501) staff       (20)       38 2023-04-21 10:01:00.704058 oapi3-1.4.2/setup.cfg
--rw-r--r--   0 motor      (501) staff       (20)      838 2023-04-21 09:59:48.000000 oapi3-1.4.2/setup.py
-drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-04-21 10:01:00.703753 oapi3-1.4.2/tests/
--rw-r--r--   0 motor      (501) staff       (20)        0 2023-01-19 13:39:59.000000 oapi3-1.4.2/tests/__init__.py
--rw-r--r--   0 motor      (501) staff       (20)      123 2023-01-20 10:29:56.000000 oapi3-1.4.2/tests/conftest.py
--rw-r--r--   0 motor      (501) staff       (20)       35 2023-01-23 08:01:55.000000 oapi3-1.4.2/tests/test_iktomi.py
--rw-r--r--   0 motor      (501) staff       (20)     8490 2023-01-30 16:58:08.000000 oapi3-1.4.2/tests/test_request_validation.py
--rw-r--r--   0 motor      (501) staff       (20)     2688 2023-01-20 11:22:10.000000 oapi3-1.4.2/tests/test_response_validation.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-06-22 12:58:57.482257 oapi3-1.4.3/
+-rw-r--r--   0 motor      (501) staff       (20)     1071 2022-09-06 13:51:56.000000 oapi3-1.4.3/LICENSE
+-rw-r--r--   0 motor      (501) staff       (20)      470 2023-06-22 12:58:57.482146 oapi3-1.4.3/PKG-INFO
+-rw-r--r--   0 motor      (501) staff       (20)       53 2022-09-06 13:51:56.000000 oapi3-1.4.3/README.md
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-06-22 12:58:57.477032 oapi3-1.4.3/oapi3/
+-rw-r--r--   0 motor      (501) staff       (20)      617 2023-01-19 13:11:11.000000 oapi3-1.4.3/oapi3/__init__.py
+-rw-r--r--   0 motor      (501) staff       (20)     4957 2022-09-06 13:51:56.000000 oapi3-1.4.3/oapi3/client.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-06-22 12:58:57.480674 oapi3-1.4.3/oapi3/entities/
+-rw-r--r--   0 motor      (501) staff       (20)      946 2023-01-23 09:13:39.000000 oapi3-1.4.3/oapi3/entities/__init__.py
+-rw-r--r--   0 motor      (501) staff       (20)      192 2023-01-17 11:57:21.000000 oapi3-1.4.3/oapi3/entities/base.py
+-rw-r--r--   0 motor      (501) staff       (20)     2679 2023-01-31 12:08:56.000000 oapi3-1.4.3/oapi3/entities/media_types.py
+-rw-r--r--   0 motor      (501) staff       (20)     3701 2023-01-20 11:08:24.000000 oapi3-1.4.3/oapi3/entities/operations.py
+-rw-r--r--   0 motor      (501) staff       (20)    10088 2023-04-20 13:14:43.000000 oapi3-1.4.3/oapi3/entities/parameters.py
+-rw-r--r--   0 motor      (501) staff       (20)     2626 2023-01-19 14:12:56.000000 oapi3-1.4.3/oapi3/entities/paths.py
+-rw-r--r--   0 motor      (501) staff       (20)      729 2023-01-17 14:18:00.000000 oapi3-1.4.3/oapi3/entities/schema.py
+-rw-r--r--   0 motor      (501) staff       (20)     3654 2023-01-20 11:24:48.000000 oapi3-1.4.3/oapi3/exceptions.py
+-rw-r--r--   0 motor      (501) staff       (20)     5860 2023-01-23 09:31:05.000000 oapi3-1.4.3/oapi3/iktomi.py
+-rw-r--r--   0 motor      (501) staff       (20)     2758 2023-01-19 13:39:26.000000 oapi3-1.4.3/oapi3/jsonschema_validator.py
+-rw-r--r--   0 motor      (501) staff       (20)     4461 2023-06-22 12:56:54.000000 oapi3-1.4.3/oapi3/resolve.py
+-rw-r--r--   0 motor      (501) staff       (20)     3616 2023-04-20 11:57:16.000000 oapi3-1.4.3/oapi3/schema.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-06-22 12:58:57.477674 oapi3-1.4.3/oapi3.egg-info/
+-rw-r--r--   0 motor      (501) staff       (20)      470 2023-06-22 12:58:57.000000 oapi3-1.4.3/oapi3.egg-info/PKG-INFO
+-rw-r--r--   0 motor      (501) staff       (20)      614 2023-06-22 12:58:57.000000 oapi3-1.4.3/oapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 motor      (501) staff       (20)        1 2023-06-22 12:58:57.000000 oapi3-1.4.3/oapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 motor      (501) staff       (20)       41 2023-06-22 12:58:57.000000 oapi3-1.4.3/oapi3.egg-info/requires.txt
+-rw-r--r--   0 motor      (501) staff       (20)       12 2023-06-22 12:58:57.000000 oapi3-1.4.3/oapi3.egg-info/top_level.txt
+-rw-r--r--   0 motor      (501) staff       (20)       38 2023-06-22 12:58:57.482287 oapi3-1.4.3/setup.cfg
+-rw-r--r--   0 motor      (501) staff       (20)      838 2023-06-22 12:57:31.000000 oapi3-1.4.3/setup.py
+drwxr-xr-x   0 motor      (501) staff       (20)        0 2023-06-22 12:58:57.481867 oapi3-1.4.3/tests/
+-rw-r--r--   0 motor      (501) staff       (20)        0 2023-01-19 13:39:59.000000 oapi3-1.4.3/tests/__init__.py
+-rw-r--r--   0 motor      (501) staff       (20)      123 2023-01-20 10:29:56.000000 oapi3-1.4.3/tests/conftest.py
+-rw-r--r--   0 motor      (501) staff       (20)       35 2023-01-23 08:01:55.000000 oapi3-1.4.3/tests/test_iktomi.py
+-rw-r--r--   0 motor      (501) staff       (20)     8490 2023-01-30 16:58:08.000000 oapi3-1.4.3/tests/test_request_validation.py
+-rw-r--r--   0 motor      (501) staff       (20)     2688 2023-01-20 11:22:10.000000 oapi3-1.4.3/tests/test_response_validation.py
```

### Comparing `oapi3-1.4.2/LICENSE` & `oapi3-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/__init__.py` & `oapi3-1.4.3/oapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/client.py` & `oapi3-1.4.3/oapi3/client.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/entities/__init__.py` & `oapi3-1.4.3/oapi3/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/entities/media_types.py` & `oapi3-1.4.3/oapi3/entities/media_types.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/entities/operations.py` & `oapi3-1.4.3/oapi3/entities/operations.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/entities/parameters.py` & `oapi3-1.4.3/oapi3/entities/parameters.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/entities/paths.py` & `oapi3-1.4.3/oapi3/entities/paths.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/entities/schema.py` & `oapi3-1.4.3/oapi3/entities/schema.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/exceptions.py` & `oapi3-1.4.3/oapi3/exceptions.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/iktomi.py` & `oapi3-1.4.3/oapi3/iktomi.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/jsonschema_validator.py` & `oapi3-1.4.3/oapi3/jsonschema_validator.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3/resolve.py` & `oapi3-1.4.3/oapi3/resolve.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 
 Exemple:
 
     schema = open_schema('api.yaml')
 
 """
 import os
-from urllib.parse import urljoin
 from urllib.parse import urlparse
 
 import yaml
+try:
+    from yaml import CSafeLoader as SafeLoader
+except ImportError:
+    from yaml import SafeLoader
 
 from .schema import Schema
 
 
 def open_schema(root_file_path):
     """ Open schema """
     root_file_path = os.path.abspath(root_file_path)
@@ -26,20 +29,21 @@
 
 def open_schema_file(schema, file_path):
     """ Open and parse schema file. Function open recuesive other files,
     if the file contains refs.
     """
     if file_path in schema:
         return schema
-    with open(file_path, encoding='utf-8') as f:
-        value = yaml.load(f, Loader=yaml.SafeLoader)
+    with open(file_path, encoding='utf-8') as fp:
+        value = yaml.load(fp, Loader=SafeLoader)
     schema[file_path] = value
     ref_files = {ref[0] for ref in get_refs(schema, file_path, value)}
     for ref_file_path in ref_files:
-        open_schema_file(schema, ref_file_path)
+        if ref_file_path not in schema:
+            open_schema_file(schema, ref_file_path)
     return schema
 
 
 def get_refs(schema, base_path, value):
     """ Get all refs from value """
     result = set()
     if isinstance(value, dict):
```

### Comparing `oapi3-1.4.2/oapi3/schema.py` & `oapi3-1.4.3/oapi3/schema.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/oapi3.egg-info/SOURCES.txt` & `oapi3-1.4.3/oapi3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/setup.py` & `oapi3-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 PY3 = sys.version_info >= (3, 0)
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='oapi3',
-    version='1.4.2',
+    version='1.4.3',
     author="Mayorov Evgeny",
     author_email="motormen@gmail.com",
     description="Validator of openapi3 requests and responses",
     packages=find_packages(),
     package_dir={'oapi3': 'oapi3'},
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `oapi3-1.4.2/tests/test_request_validation.py` & `oapi3-1.4.3/tests/test_request_validation.py`

 * *Files identical despite different names*

### Comparing `oapi3-1.4.2/tests/test_response_validation.py` & `oapi3-1.4.3/tests/test_response_validation.py`

 * *Files identical despite different names*

