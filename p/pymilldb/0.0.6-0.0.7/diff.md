# Comparing `tmp/pymilldb-0.0.6.tar.gz` & `tmp/pymilldb-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilldb-0.0.6.tar", last modified: Tue Jun  6 21:15:59 2023, max compression
+gzip compressed data, was "pymilldb-0.0.7.tar", last modified: Thu Jun 22 20:11:07 2023, max compression
```

## Comparing `pymilldb-0.0.6.tar` & `pymilldb-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1095 2023-05-30 21:05:16.000000 pymilldb-0.0.6/LICENSE
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-06 21:15:59.185585 pymilldb-0.0.6/PKG-INFO
--rw-r--r--   0 zeus      (1000) zeus      (1000)      523 2023-05-30 21:18:35.000000 pymilldb-0.0.6/README.md
--rw-r--r--   0 zeus      (1000) zeus      (1000)       89 2023-05-30 21:05:16.000000 pymilldb-0.0.6/pyproject.toml
--rw-r--r--   0 zeus      (1000) zeus      (1000)      633 2023-06-06 21:15:59.185585 pymilldb-0.0.6/setup.cfg
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/pymilldb/
--rw-r--r--   0 zeus      (1000) zeus      (1000)      167 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/__init__.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     2802 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/mdb_client.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1518 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/protocol.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1430 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/sampler.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)    10804 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/tensor_store.py
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/pymilldb/utils/
--rw-r--r--   0 zeus      (1000) zeus      (1000)        0 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/utils/__init__.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)      353 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/utils/decorators.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)      630 2023-05-30 21:05:16.000000 pymilldb-0.0.6/src/pymilldb/utils/graph.py
--rw-r--r--   0 zeus      (1000) zeus      (1000)     2173 2023-06-06 21:04:43.000000 pymilldb-0.0.6/src/pymilldb/utils/packer.py
-drwxr-xr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-06 21:15:59.185585 pymilldb-0.0.6/src/pymilldb.egg-info/
--rw-r--r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/PKG-INFO
--rw-r--r--   0 zeus      (1000) zeus      (1000)      437 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/SOURCES.txt
--rw-r--r--   0 zeus      (1000) zeus      (1000)        1 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/dependency_links.txt
--rw-r--r--   0 zeus      (1000) zeus      (1000)        9 2023-06-06 21:15:59.000000 pymilldb-0.0.6/src/pymilldb.egg-info/top_level.txt
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.402823 pymilldb-0.0.7/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1095 2023-06-01 18:38:01.000000 pymilldb-0.0.7/LICENSE
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-22 20:11:07.402823 pymilldb-0.0.7/PKG-INFO
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      523 2023-06-01 18:38:01.000000 pymilldb-0.0.7/README.md
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)       89 2023-06-01 18:38:01.000000 pymilldb-0.0.7/pyproject.toml
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      633 2023-06-22 20:11:07.402823 pymilldb-0.0.7/setup.cfg
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.250806 pymilldb-0.0.7/src/
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.338816 pymilldb-0.0.7/src/pymilldb/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      167 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/__init__.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     2802 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/mdb_client.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1518 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/protocol.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1430 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/sampler.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)    10748 2023-06-22 20:09:52.000000 pymilldb-0.0.7/src/pymilldb/tensor_store.py
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.402823 pymilldb-0.0.7/src/pymilldb/utils/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        0 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/utils/__init__.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      353 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/utils/decorators.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      630 2023-06-01 18:38:01.000000 pymilldb-0.0.7/src/pymilldb/utils/graph.py
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     2173 2023-06-07 16:03:26.000000 pymilldb-0.0.7/src/pymilldb/utils/packer.py
+drwxrwxr-x   0 zeus      (1000) zeus      (1000)        0 2023-06-22 20:11:07.342816 pymilldb-0.0.7/src/pymilldb.egg-info/
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)     1031 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/PKG-INFO
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)      437 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/SOURCES.txt
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        1 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/dependency_links.txt
+-rw-rw-r--   0 zeus      (1000) zeus      (1000)        9 2023-06-22 20:11:07.000000 pymilldb-0.0.7/src/pymilldb.egg-info/top_level.txt
```

### Comparing `pymilldb-0.0.6/LICENSE` & `pymilldb-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.6/PKG-INFO` & `pymilldb-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pymilldb-0.0.6/README.md` & `pymilldb-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.6/setup.cfg` & `pymilldb-0.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pymilldb
-version = 0.0.6
+version = 0.0.7
 author = Vicente Calisto
 author_email = vecalisto@uc.cl
 description = A python library for MillenniumDB
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MillenniumDB/PyMillDB
 project_urls =
```

### Comparing `pymilldb-0.0.6/src/pymilldb/mdb_client.py` & `pymilldb-0.0.7/src/pymilldb/mdb_client.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.6/src/pymilldb/protocol.py` & `pymilldb-0.0.7/src/pymilldb/protocol.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.6/src/pymilldb/sampler.py` & `pymilldb-0.0.7/src/pymilldb/sampler.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.6/src/pymilldb/tensor_store.py` & `pymilldb-0.0.7/src/pymilldb/tensor_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,14 @@
     @decorators.check_closed
     def multi_insert(
         self, keys: Union[List[int], List[str]], tensors: torch.Tensor
     ) -> None:
         packed_key = b""
         if all(isinstance(key, int) for key in keys):
             packed_key += packer.pack_bool(True)
-            packed_key += packer.pack_uint64(len(keys))
             packed_key += packer.pack_uint64_vector(keys)
         elif all(isinstance(key, str) for key in keys):
             packed_key += packer.pack_bool(False)
             packed_key += packer.pack_string_vector(keys)
         else:
             raise TypeError(f"Key must be List[int] or List[str], got {type(keys)}")
```

### Comparing `pymilldb-0.0.6/src/pymilldb/utils/graph.py` & `pymilldb-0.0.7/src/pymilldb/utils/graph.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.6/src/pymilldb/utils/packer.py` & `pymilldb-0.0.7/src/pymilldb/utils/packer.py`

 * *Files identical despite different names*

### Comparing `pymilldb-0.0.6/src/pymilldb.egg-info/PKG-INFO` & `pymilldb-0.0.7/src/pymilldb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymilldb
-Version: 0.0.6
+Version: 0.0.7
 Summary: A python library for MillenniumDB
 Home-page: https://github.com/MillenniumDB/PyMillDB
 Author: Vicente Calisto
 Author-email: vecalisto@uc.cl
 Project-URL: Bug Tracker, https://github.com/MillenniumDB/PyMillDB/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

