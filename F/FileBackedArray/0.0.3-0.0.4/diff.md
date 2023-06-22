# Comparing `tmp/FileBackedArray-0.0.3.tar.gz` & `tmp/FileBackedArray-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileBackedArray-0.0.3.tar", last modified: Thu Jun 22 00:55:32 2023, max compression
+gzip compressed data, was "FileBackedArray-0.0.4.tar", last modified: Thu Jun 22 19:43:43 2023, max compression
```

## Comparing `FileBackedArray-0.0.3.tar` & `FileBackedArray-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.297648 FileBackedArray-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.285648 FileBackedArray-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.289648 FileBackedArray-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 00:55:32.297648 FileBackedArray-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.289648 FileBackedArray-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.293648 FileBackedArray-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 00:55:32.297648 FileBackedArray-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.285648 FileBackedArray-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.293648 FileBackedArray-0.0.3/src/FileBackedArray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 00:55:32.000000 FileBackedArray-0.0.3/src/FileBackedArray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-22 00:55:32.000000 FileBackedArray-0.0.3/src/FileBackedArray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:55:32.000000 FileBackedArray-0.0.3/src/FileBackedArray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:55:32.000000 FileBackedArray-0.0.3/src/FileBackedArray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 00:55:32.000000 FileBackedArray-0.0.3/src/FileBackedArray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 00:55:32.000000 FileBackedArray-0.0.3/src/FileBackedArray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.293648 FileBackedArray-0.0.3/src/filebackedarray/
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/src/filebackedarray/H5Dense.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/src/filebackedarray/H5Sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/src/filebackedarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/src/filebackedarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.293648 FileBackedArray-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:55:32.293648 FileBackedArray-0.0.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    82048 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/tests/data/dense.h5
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/tests/data/dense_F.h5
--rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/tests/data/tenx.sub.h5
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/tests/test_h5_dense.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/tests/test_h5_sparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-22 00:54:26.000000 FileBackedArray-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.183019 FileBackedArray-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.151019 FileBackedArray-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.163019 FileBackedArray-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 19:43:43.183019 FileBackedArray-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.167019 FileBackedArray-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.167019 FileBackedArray-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-22 19:43:43.183019 FileBackedArray-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.155019 FileBackedArray-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.171019 FileBackedArray-0.0.4/src/FileBackedArray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 19:43:43.000000 FileBackedArray-0.0.4/src/FileBackedArray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-22 19:43:43.000000 FileBackedArray-0.0.4/src/FileBackedArray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:43:43.000000 FileBackedArray-0.0.4/src/FileBackedArray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:43:42.000000 FileBackedArray-0.0.4/src/FileBackedArray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 19:43:43.000000 FileBackedArray-0.0.4/src/FileBackedArray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 19:43:43.000000 FileBackedArray-0.0.4/src/FileBackedArray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.175019 FileBackedArray-0.0.4/src/filebackedarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/src/filebackedarray/H5Dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/src/filebackedarray/H5Sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/src/filebackedarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/src/filebackedarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.179019 FileBackedArray-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:43:43.179019 FileBackedArray-0.0.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    82048 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/tests/data/dense.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/tests/data/dense_F.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/tests/test_h5_dense.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/tests/test_h5_sparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-22 19:42:16.000000 FileBackedArray-0.0.4/tox.ini
```

### Comparing `FileBackedArray-0.0.3/.coveragerc` & `FileBackedArray-0.0.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/.github/workflows/pypi-publish.yml` & `FileBackedArray-0.0.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/.github/workflows/pypi-test.yml` & `FileBackedArray-0.0.4/.github/workflows/pypi-test.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This workflow will install Python dependencies, run tests and lint with a single version of Python
 # For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 name: Test the library
 
 on:
   push:
-    branches: [ master ]
+    branches: [ main ]
   pull_request:
-    branches: [ master ]
+    branches: [ main ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `FileBackedArray-0.0.3/.gitignore` & `FileBackedArray-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/.readthedocs.yml` & `FileBackedArray-0.0.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/CONTRIBUTING.md` & `FileBackedArray-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/LICENSE.txt` & `FileBackedArray-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/PKG-INFO` & `FileBackedArray-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileBackedArray
-Version: 0.0.3
+Version: 0.0.4
 Summary: File backed objects for array and matrix like data
 Home-page: https://github.com/biocpy/FileBackedArray
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/FileBackedArray/
 Platform: any
```

### Comparing `FileBackedArray-0.0.3/README.md` & `FileBackedArray-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/docs/Makefile` & `FileBackedArray-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/docs/conf.py` & `FileBackedArray-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/docs/index.md` & `FileBackedArray-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/docs/tutorial.md` & `FileBackedArray-0.0.4/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/setup.cfg` & `FileBackedArray-0.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/setup.py` & `FileBackedArray-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/src/FileBackedArray.egg-info/PKG-INFO` & `FileBackedArray-0.0.4/src/FileBackedArray.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FileBackedArray
-Version: 0.0.3
+Version: 0.0.4
 Summary: File backed objects for array and matrix like data
 Home-page: https://github.com/biocpy/FileBackedArray
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://biocpy.github.io/FileBackedArray/
 Platform: any
```

### Comparing `FileBackedArray-0.0.3/src/FileBackedArray.egg-info/SOURCES.txt` & `FileBackedArray-0.0.4/src/FileBackedArray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/src/filebackedarray/H5Dense.py` & `FileBackedArray-0.0.4/src/filebackedarray/H5Dense.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, Sequence, Tuple, Union
 
 import h5py
+import numpy as np
 
 from .utils import _check_indices, infer_h5_dataset
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
@@ -27,14 +28,20 @@
             group (str): Group inside the file that contains the matrix or array.
             order (str): dense matrix representation, ‘C’, ‘F’,
                 row-major (C-style) or column-major (Fortran-style) order.
         """
         self._h5file = h5py.File(path, mode="r")
         self._dataset = self._h5file[group]
         self._dataset_info = infer_h5_dataset(self._dataset)
+
+        if order not in ("C", "F"):
+            raise ValueError(
+                "order must be C (c-style, row-major) or F (fortran-style, column-major)"
+            )
+
         self._order = order
 
         if self._dataset_info.format != "dense":
             raise ValueError("File does not contain a dense matrix")
 
     @property
     def shape(self) -> Tuple[int, int]:
@@ -67,15 +74,15 @@
              str: matrix format.
         """
         return self._order
 
     def __getitem__(
         self,
         args: Tuple[Union[slice, Sequence[int]], Optional[Union[slice, Sequence[int]]]],
-    ):
+    ) -> np.ndarray:
         if len(args) == 0:
             raise ValueError("Arguments must contain one slice")
 
         rowIndices = _check_indices(args[0])
         colIndices = None
 
         if len(args) > 1:
```

### Comparing `FileBackedArray-0.0.3/src/filebackedarray/H5Sparse.py` & `FileBackedArray-0.0.4/src/filebackedarray/H5Sparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional, Sequence, Tuple, Union
 
 import h5py
+import scipy.sparse as sp
 
 from .utils import _check_indices, _slice_h5_sparse, infer_h5_dataset
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
@@ -63,15 +64,15 @@
              str: matrix format.
         """
         return self._dataset_info.format
 
     def __getitem__(
         self,
         args: Tuple[Union[slice, Sequence[int]], Optional[Union[slice, Sequence[int]]]],
-    ):
+    ) -> sp.spmatrix:
         if len(args) == 0:
             raise ValueError("Arguments must contain one slice")
 
         rowIndices = _check_indices(args[0])
         colIndices = None
 
         if len(args) > 1:
```

### Comparing `FileBackedArray-0.0.3/src/filebackedarray/__init__.py` & `FileBackedArray-0.0.4/src/filebackedarray/__init__.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/src/filebackedarray/utils.py` & `FileBackedArray-0.0.4/src/filebackedarray/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from collections import namedtuple
 from typing import Optional, Sequence, Union
 
 import h5py
 from scipy import sparse as sp
 
-
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
 H5DatasetInfo = namedtuple("H5DatasetInfo", ["shape", "dtype", "format"])
 
@@ -45,15 +44,18 @@
 
         if verbose:
             print("shape is ", shape)
 
         shape = tuple(shape)
 
         format = "csc_matrix"
-        print("length of indptr", dataset["indptr"], len(dataset["indptr"]))
+
+        if verbose:
+            print("length of indptr", dataset["indptr"], len(dataset["indptr"]))
+
         if shape[0] == len(dataset["indptr"]) - 1:
             format = "csr_matrix"
 
         dtype = dataset["data"].dtype.type
     else:
         # dense
         shape = dataset.shape
@@ -108,15 +110,15 @@
     elif h5info.format == "csc_matrix":
         shape = (h5info.shape[0], indptr.size - 1)
 
     mformat = _get_mat_class(h5info.format)
     return mformat((data, indices, indptr), shape=shape)
 
 
-def _get_mat_class(sparse_format):
+def _get_mat_class(sparse_format: str):
     if sparse_format == "csr_matrix":
         return sp.csc_matrix
     elif sparse_format == "csc_matrix":
         return sp.csc_matrix
     else:
         raise ValueError(f"sparse format {sparse_format} not supported")
```

### Comparing `FileBackedArray-0.0.3/tests/data/dense.h5` & `FileBackedArray-0.0.4/tests/data/dense.h5`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/tests/data/dense_F.h5` & `FileBackedArray-0.0.4/tests/data/dense_F.h5`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/tests/data/tenx.sub.h5` & `FileBackedArray-0.0.4/tests/data/tenx.sub.h5`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/tests/test_h5_dense.py` & `FileBackedArray-0.0.4/tests/test_h5_dense.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/tests/test_h5_sparse.py` & `FileBackedArray-0.0.4/tests/test_h5_sparse.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.3/tox.ini` & `FileBackedArray-0.0.4/tox.ini`

 * *Files identical despite different names*

