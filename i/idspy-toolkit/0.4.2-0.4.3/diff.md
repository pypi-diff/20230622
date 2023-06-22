# Comparing `tmp/idspy_toolkit-0.4.2.tar.gz` & `tmp/idspy_toolkit-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idspy_toolkit-0.4.2.tar", last modified: Tue Jun 20 17:10:01 2023, max compression
+gzip compressed data, was "idspy_toolkit-0.4.3.tar", last modified: Thu Jun 22 09:42:29 2023, max compression
```

## Comparing `idspy_toolkit-0.4.2.tar` & `idspy_toolkit-0.4.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:10:00.977416 idspy_toolkit-0.4.2/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-08 14:59:54.000000 idspy_toolkit-0.4.2/LICENSE
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4711 2023-06-20 17:10:00.963415 idspy_toolkit-0.4.2/PKG-INFO
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2033 2023-06-20 17:09:32.000000 idspy_toolkit-0.4.2/README.rst
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:09:59.788453 idspy_toolkit-0.4.2/idspy_toolkit/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      611 2023-06-20 16:49:28.000000 idspy_toolkit-0.4.2/idspy_toolkit/__init__.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    15133 2023-06-20 16:42:29.000000 idspy_toolkit-0.4.2/idspy_toolkit/accessor.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2645 2023-06-20 16:42:43.000000 idspy_toolkit-0.4.2/idspy_toolkit/constants.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10923 2023-06-20 16:47:28.000000 idspy_toolkit-0.4.2/idspy_toolkit/converter.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1997 2023-06-20 16:47:41.000000 idspy_toolkit-0.4.2/idspy_toolkit/snippets.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8357 2023-06-20 16:49:53.000000 idspy_toolkit-0.4.2/idspy_toolkit/toolkit.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8518 2023-06-20 16:50:19.000000 idspy_toolkit-0.4.2/idspy_toolkit/utils.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:10:00.246192 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4711 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/PKG-INFO
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      548 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/SOURCES.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/dependency_links.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       69 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/requires.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       14 2023-06-20 17:09:58.000000 idspy_toolkit-0.4.2/idspy_toolkit.egg-info/top_level.txt
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7906 2023-06-20 16:46:04.000000 idspy_toolkit-0.4.2/pyproject.toml
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-20 17:10:00.982430 idspy_toolkit-0.4.2/setup.cfg
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-12 10:54:27.000000 idspy_toolkit-0.4.2/setup.py
-drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-20 17:10:00.844191 idspy_toolkit-0.4.2/tests/
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7600 2023-06-20 16:48:35.000000 idspy_toolkit-0.4.2/tests/test_accessor.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6561 2023-06-20 16:48:49.000000 idspy_toolkit-0.4.2/tests/test_converter_hdf5.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1493 2023-06-08 14:51:39.000000 idspy_toolkit-0.4.2/tests/test_hdf5_io.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2542 2023-06-12 10:05:30.000000 idspy_toolkit-0.4.2/tests/test_ids_browse.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1397 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.2/tests/test_snippets.py
--rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4192 2023-06-20 16:45:10.000000 idspy_toolkit-0.4.2/tests/test_utils.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-22 09:42:29.793705 idspy_toolkit-0.4.3/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1599 2023-06-08 14:59:54.000000 idspy_toolkit-0.4.3/LICENSE
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4711 2023-06-22 09:42:29.786707 idspy_toolkit-0.4.3/PKG-INFO
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2033 2023-06-22 09:42:07.000000 idspy_toolkit-0.4.3/README.rst
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-22 09:42:28.786164 idspy_toolkit-0.4.3/idspy_toolkit/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      611 2023-06-22 09:34:43.000000 idspy_toolkit-0.4.3/idspy_toolkit/__init__.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    15133 2023-06-20 16:42:29.000000 idspy_toolkit-0.4.3/idspy_toolkit/accessor.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2645 2023-06-20 16:42:43.000000 idspy_toolkit-0.4.3/idspy_toolkit/constants.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)    10970 2023-06-22 09:34:29.000000 idspy_toolkit-0.4.3/idspy_toolkit/converter.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1997 2023-06-20 16:47:41.000000 idspy_toolkit-0.4.3/idspy_toolkit/snippets.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8357 2023-06-20 16:49:53.000000 idspy_toolkit-0.4.3/idspy_toolkit/toolkit.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     8473 2023-06-22 09:34:54.000000 idspy_toolkit-0.4.3/idspy_toolkit/utils.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-22 09:42:29.207502 idspy_toolkit-0.4.3/idspy_toolkit.egg-info/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4711 2023-06-22 09:42:27.000000 idspy_toolkit-0.4.3/idspy_toolkit.egg-info/PKG-INFO
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)      548 2023-06-22 09:42:27.000000 idspy_toolkit-0.4.3/idspy_toolkit.egg-info/SOURCES.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        1 2023-06-22 09:42:27.000000 idspy_toolkit-0.4.3/idspy_toolkit.egg-info/dependency_links.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       69 2023-06-22 09:42:27.000000 idspy_toolkit-0.4.3/idspy_toolkit.egg-info/requires.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       14 2023-06-22 09:42:27.000000 idspy_toolkit-0.4.3/idspy_toolkit.egg-info/top_level.txt
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7906 2023-06-22 09:35:06.000000 idspy_toolkit-0.4.3/pyproject.toml
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       38 2023-06-22 09:42:29.796738 idspy_toolkit-0.4.3/setup.cfg
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)       39 2023-06-12 10:54:27.000000 idspy_toolkit-0.4.3/setup.py
+drwxrwxrwx   0 guillaume  (1000) guillaume  (1000)        0 2023-06-22 09:42:29.706093 idspy_toolkit-0.4.3/tests/
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     7600 2023-06-20 16:48:35.000000 idspy_toolkit-0.4.3/tests/test_accessor.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     6561 2023-06-20 16:48:49.000000 idspy_toolkit-0.4.3/tests/test_converter_hdf5.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2401 2023-06-22 09:35:18.000000 idspy_toolkit-0.4.3/tests/test_hdf5_io.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     2542 2023-06-12 10:05:30.000000 idspy_toolkit-0.4.3/tests/test_ids_browse.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     1397 2023-06-08 14:51:40.000000 idspy_toolkit-0.4.3/tests/test_snippets.py
+-rwxrwxrwx   0 guillaume  (1000) guillaume  (1000)     4192 2023-06-20 16:45:10.000000 idspy_toolkit-0.4.3/tests/test_utils.py
```

### Comparing `idspy_toolkit-0.4.2/LICENSE` & `idspy_toolkit-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/PKG-INFO` & `idspy_toolkit-0.4.3/idspy_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idspy_toolkit
-Version: 0.4.2
+Name: idspy-toolkit
+Version: 0.4.3
 Summary: Tools to manipulate the IDSPy Dictionaries
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
```

### Comparing `idspy_toolkit-0.4.2/README.rst` & `idspy_toolkit-0.4.3/README.rst`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit/__init__.py` & `idspy_toolkit-0.4.3/idspy_toolkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from idspy_toolkit.toolkit import fill_default_values_ids, list_ids_members,\
     get_ids_classes_as_dict
 from idspy_toolkit.converter import ids_to_hdf5, hdf5_to_ids
 from idspy_toolkit.accessor import get_ids_value_from_string, \
     set_ids_value_from_string, copy_ids
 from idspy_toolkit.utils import get_field_with_type
-__version__ = "0.4.2"
+__version__ = "0.4.3"
 
 __all__ = [
     "__version__",
     "fill_default_values_ids",
     "ids_to_hdf5",
     "hdf5_to_ids",
     "get_ids_value_from_string",
```

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit/accessor.py` & `idspy_toolkit-0.4.3/idspy_toolkit/accessor.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit/constants.py` & `idspy_toolkit-0.4.3/idspy_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit/converter.py` & `idspy_toolkit-0.4.3/idspy_toolkit/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,20 +244,21 @@
         return ids_group, ids_dataset
 
     if overwrite is False :
         tmp_file = filename
         if os.path.exists(filename):
             raise IOError(f"HDF5 file {filename} already exist")
     if overwrite is True :
-        tmp_file = filename+".tmp"
+        tmp_file = str(filename)+".tmp"
     # open the hdf5 file
     with h5py.File(tmp_file, "w") as h5f:
         total_group, total_dataset = _browse_ids(ids, h5f, total_group, total_dataset)
     if overwrite is True:
-        os.remove(filename)
+        if os.path.exists(filename):
+            os.remove(filename)
         os_rename(tmp_file, filename)
     print(f"IDS written to file : {filename}")
     return total_group, total_dataset
 
 
 def _iterate_hdf5_dataset(name: str, hdf5obj: Any, h5struct: list) -> None:
     if isinstance(hdf5obj, h5py.Dataset):
```

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit/snippets.py` & `idspy_toolkit-0.4.3/idspy_toolkit/snippets.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit/toolkit.py` & `idspy_toolkit-0.4.3/idspy_toolkit/toolkit.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit/utils.py` & `idspy_toolkit-0.4.3/idspy_toolkit/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,14 @@
         :param module_name: name of the ids module
         :param current_dict: generated dict
         :return : None
     """
 
     correspondance_table = {x[0]: x[1] for x in getmembers(module_name, predicate=isclass) if
                             (x[0].startswith("__") is False) and ("ndarray" not in x[0])}
-    print(list(correspondance_table.keys()))
     for k, v in correspondance_table.items():
         member = v()
 
         _get_all_subdataclasses(member, current_dict)
 
 
 def extract_ndarray_info(expr: str):
```

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit.egg-info/PKG-INFO` & `idspy_toolkit-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idspy-toolkit
-Version: 0.4.2
+Name: idspy_toolkit
+Version: 0.4.3
 Summary: Tools to manipulate the IDSPy Dictionaries
 Author-email: Guillaume Fuhr <guillaume.fuhr@univ-amu.fr>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, CNRS, contributor: Y. Camenen
         Copyright (c) 2023, Aix-Marseille Univ., contributor: G. Fuhr
         All rights reserved.
```

### Comparing `idspy_toolkit-0.4.2/idspy_toolkit.egg-info/SOURCES.txt` & `idspy_toolkit-0.4.3/idspy_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/pyproject.toml` & `idspy_toolkit-0.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "setuptools>=61.0.0",
     "wheel",
 ]
 # build-backend = "setuptools.build_meta"
 
 [project]
 name = 'idspy_toolkit'
-version = '0.4.2'
+version = '0.4.3'
 description = 'Tools to manipulate the IDSPy Dictionaries'
 readme = 'README.rst'
 authors = [
   { name = 'Guillaume Fuhr', email='guillaume.fuhr@univ-amu.fr' },
 ]
 license = {file = 'LICENSE'}
 requires-python = '>=3.9'
```

### Comparing `idspy_toolkit-0.4.2/tests/test_accessor.py` & `idspy_toolkit-0.4.3/tests/test_accessor.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/tests/test_converter_hdf5.py` & `idspy_toolkit-0.4.3/tests/test_converter_hdf5.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/tests/test_ids_browse.py` & `idspy_toolkit-0.4.3/tests/test_ids_browse.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/tests/test_snippets.py` & `idspy_toolkit-0.4.3/tests/test_snippets.py`

 * *Files identical despite different names*

### Comparing `idspy_toolkit-0.4.2/tests/test_utils.py` & `idspy_toolkit-0.4.3/tests/test_utils.py`

 * *Files identical despite different names*

