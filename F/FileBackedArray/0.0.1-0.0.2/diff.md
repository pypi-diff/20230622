# Comparing `tmp/FileBackedArray-0.0.1.tar.gz` & `tmp/FileBackedArray-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FileBackedArray-0.0.1.tar", last modified: Wed Jun 21 15:51:48 2023, max compression
+gzip compressed data, was "FileBackedArray-0.0.2.tar", last modified: Wed Jun 21 16:07:13 2023, max compression
```

## Comparing `FileBackedArray-0.0.1.tar` & `FileBackedArray-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.167661 FileBackedArray-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.155661 FileBackedArray-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.159661 FileBackedArray-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-21 15:51:48.167661 FileBackedArray-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.163661 FileBackedArray-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.163661 FileBackedArray-0.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-21 15:51:48.167661 FileBackedArray-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.155661 FileBackedArray-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.163661 FileBackedArray-0.0.1/src/FileBackedArray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-21 15:51:48.000000 FileBackedArray-0.0.1/src/FileBackedArray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-21 15:51:48.000000 FileBackedArray-0.0.1/src/FileBackedArray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:51:48.000000 FileBackedArray-0.0.1/src/FileBackedArray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:51:47.000000 FileBackedArray-0.0.1/src/FileBackedArray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 15:51:48.000000 FileBackedArray-0.0.1/src/FileBackedArray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 15:51:48.000000 FileBackedArray-0.0.1/src/FileBackedArray.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.163661 FileBackedArray-0.0.1/src/filebackedarray/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/src/filebackedarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/src/filebackedarray/backedH5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/src/filebackedarray/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.163661 FileBackedArray-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:51:48.163661 FileBackedArray-0.0.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/tests/data/tenx.sub.h5
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/tests/test_h5_backed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 15:50:40.000000 FileBackedArray-0.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.821186 FileBackedArray-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.805186 FileBackedArray-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.809186 FileBackedArray-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-21 16:07:13.821186 FileBackedArray-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.813186 FileBackedArray-0.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.817186 FileBackedArray-0.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-21 16:07:13.825186 FileBackedArray-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.809186 FileBackedArray-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.817186 FileBackedArray-0.0.2/src/FileBackedArray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-21 16:07:13.000000 FileBackedArray-0.0.2/src/FileBackedArray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-21 16:07:13.000000 FileBackedArray-0.0.2/src/FileBackedArray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:07:13.000000 FileBackedArray-0.0.2/src/FileBackedArray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:07:13.000000 FileBackedArray-0.0.2/src/FileBackedArray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 16:07:13.000000 FileBackedArray-0.0.2/src/FileBackedArray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 16:07:13.000000 FileBackedArray-0.0.2/src/FileBackedArray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.821186 FileBackedArray-0.0.2/src/filebackedarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/src/filebackedarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/src/filebackedarray/backedH5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/src/filebackedarray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.821186 FileBackedArray-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:07:13.821186 FileBackedArray-0.0.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/tests/test_h5_backed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-21 16:05:59.000000 FileBackedArray-0.0.2/tox.ini
```

### Comparing `FileBackedArray-0.0.1/.coveragerc` & `FileBackedArray-0.0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/.github/workflows/pypi-publish.yml` & `FileBackedArray-0.0.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/.github/workflows/pypi-test.yml` & `FileBackedArray-0.0.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/.gitignore` & `FileBackedArray-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/.readthedocs.yml` & `FileBackedArray-0.0.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/CONTRIBUTING.md` & `FileBackedArray-0.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/LICENSE.txt` & `FileBackedArray-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/PKG-INFO` & `FileBackedArray-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: FileBackedArray
-Version: 0.0.1
+Version: 0.0.2
 Summary: File backed objects for array and matrix like data
-Home-page: https://github.com/pyscaffold/pyscaffold/
+Home-page: https://github.com/biocpy/FileBackedArray
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: Documentation, https://biocpy.github.io/FileBackedArray/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
```

### Comparing `FileBackedArray-0.0.1/README.md` & `FileBackedArray-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/docs/Makefile` & `FileBackedArray-0.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/docs/conf.py` & `FileBackedArray-0.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/docs/index.md` & `FileBackedArray-0.0.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/setup.cfg` & `FileBackedArray-0.0.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 description = File backed objects for array and matrix like data
 author = Jayaram Kancherla
 author_email = jayaram.kancherla@gmail.com
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
-url = https://github.com/pyscaffold/pyscaffold/
+url = https://github.com/biocpy/FileBackedArray
 project_urls = 
-	Documentation = https://pyscaffold.org/
+	Documentation = https://biocpy.github.io/FileBackedArray/
 platforms = any
 classifiers = 
 	Development Status :: 4 - Beta
 	Programming Language :: Python
 
 [options]
 zip_safe = False
```

### Comparing `FileBackedArray-0.0.1/setup.py` & `FileBackedArray-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/src/FileBackedArray.egg-info/PKG-INFO` & `FileBackedArray-0.0.2/src/FileBackedArray.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: FileBackedArray
-Version: 0.0.1
+Version: 0.0.2
 Summary: File backed objects for array and matrix like data
-Home-page: https://github.com/pyscaffold/pyscaffold/
+Home-page: https://github.com/biocpy/FileBackedArray
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
-Project-URL: Documentation, https://pyscaffold.org/
+Project-URL: Documentation, https://biocpy.github.io/FileBackedArray/
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Provides-Extra: testing
 License-File: LICENSE.txt
```

### Comparing `FileBackedArray-0.0.1/src/FileBackedArray.egg-info/SOURCES.txt` & `FileBackedArray-0.0.2/src/FileBackedArray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/src/filebackedarray/__init__.py` & `FileBackedArray-0.0.2/src/filebackedarray/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
     dist_name = "FileBackedArray"
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
-from .backedH5 import H5Backed
+from .backedH5 import H5BackedData
```

### Comparing `FileBackedArray-0.0.1/src/filebackedarray/backedH5.py` & `FileBackedArray-0.0.2/src/filebackedarray/backedH5.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional, Sequence, Tuple, Union
 
 import h5py
 
 from .utils import _check_indices, _slice_h5_sparse, infer_h5_dataset
 
 
-class H5Backed:
+class H5BackedData:
     """H5 backed matrix or array store.
 
     Args:
         path (str): Path to the H5 file.
         group (str): Group inside the file that contains the matrix or array.
     """
```

### Comparing `FileBackedArray-0.0.1/src/filebackedarray/utils.py` & `FileBackedArray-0.0.2/src/filebackedarray/utils.py`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/tests/data/tenx.sub.h5` & `FileBackedArray-0.0.2/tests/data/tenx.sub.h5`

 * *Files identical despite different names*

### Comparing `FileBackedArray-0.0.1/tox.ini` & `FileBackedArray-0.0.2/tox.ini`

 * *Files identical despite different names*

