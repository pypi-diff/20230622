# Comparing `tmp/cleanmydataset-1.0.0.tar.gz` & `tmp/cleanmydataset-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanmydataset-1.0.0.tar", last modified: Thu Jun 22 03:46:40 2023, max compression
+gzip compressed data, was "cleanmydataset-1.1.0.tar", last modified: Thu Jun 22 04:50:21 2023, max compression
```

## Comparing `cleanmydataset-1.0.0.tar` & `cleanmydataset-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 03:46:40.259940 cleanmydataset-1.0.0/
--rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 cleanmydataset-1.0.0/LICENSE.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 03:46:40.259829 cleanmydataset-1.0.0/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)     4918 2023-06-22 03:45:25.000000 cleanmydataset-1.0.0/README.md
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 03:46:40.258859 cleanmydataset-1.0.0/cleanmydataset/
--rw-r--r--   0 samuelshine   (501) staff       (20)       64 2023-06-22 03:43:17.000000 cleanmydataset-1.0.0/cleanmydataset/__init__.py
--rw-r--r--   0 samuelshine   (501) staff       (20)     8847 2023-06-21 10:26:13.000000 cleanmydataset-1.0.0/cleanmydataset/cleanmydataset.py
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 03:46:40.259664 cleanmydataset-1.0.0/cleanmydataset.egg-info/
--rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 03:46:40.000000 cleanmydataset-1.0.0/cleanmydataset.egg-info/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)      279 2023-06-22 03:46:40.000000 cleanmydataset-1.0.0/cleanmydataset.egg-info/SOURCES.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 03:46:40.000000 cleanmydataset-1.0.0/cleanmydataset.egg-info/dependency_links.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       85 2023-06-22 03:46:40.000000 cleanmydataset-1.0.0/cleanmydataset.egg-info/requires.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       15 2023-06-22 03:46:40.000000 cleanmydataset-1.0.0/cleanmydataset.egg-info/top_level.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 03:46:40.259993 cleanmydataset-1.0.0/setup.cfg
--rw-r--r--   0 samuelshine   (501) staff       (20)     1058 2023-06-22 03:42:32.000000 cleanmydataset-1.0.0/setup.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 04:50:21.163154 cleanmydataset-1.1.0/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 cleanmydataset-1.1.0/LICENSE.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 04:50:21.162979 cleanmydataset-1.1.0/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)     4918 2023-06-22 03:45:25.000000 cleanmydataset-1.1.0/README.md
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 04:50:21.161653 cleanmydataset-1.1.0/cleanmydataset/
+-rw-r--r--   0 samuelshine   (501) staff       (20)       64 2023-06-22 03:43:17.000000 cleanmydataset-1.1.0/cleanmydataset/__init__.py
+-rw-r--r--   0 samuelshine   (501) staff       (20)     8824 2023-06-22 04:48:03.000000 cleanmydataset-1.1.0/cleanmydataset/cleanmydataset.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 04:50:21.162701 cleanmydataset-1.1.0/cleanmydataset.egg-info/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 04:50:21.000000 cleanmydataset-1.1.0/cleanmydataset.egg-info/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)      279 2023-06-22 04:50:21.000000 cleanmydataset-1.1.0/cleanmydataset.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 04:50:21.000000 cleanmydataset-1.1.0/cleanmydataset.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       76 2023-06-22 04:50:21.000000 cleanmydataset-1.1.0/cleanmydataset.egg-info/requires.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       15 2023-06-22 04:50:21.000000 cleanmydataset-1.1.0/cleanmydataset.egg-info/top_level.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 04:50:21.163208 cleanmydataset-1.1.0/setup.cfg
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1038 2023-06-22 04:48:40.000000 cleanmydataset-1.1.0/setup.py
```

### Comparing `cleanmydataset-1.0.0/LICENSE.txt` & `cleanmydataset-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleanmydataset-1.0.0/PKG-INFO` & `cleanmydataset-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanmydataset
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cleanmydataset-1.0.0/README.md` & `cleanmydataset-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cleanmydataset-1.0.0/cleanmydataset/cleanmydataset.py` & `cleanmydataset-1.1.0/cleanmydataset/cleanmydataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import datetime
 import charset_normalizer
 import fuzzywuzzy
 from fuzzywuzzy import process
 import re
 from scipy import stats
 from pandas.api.types import is_numeric_dtype
-import dateutil.parser
 import emoji
 import string
 from googletrans import Translator
 
 class DataClean:
     def __init__(self, filepath):
         if filepath.endswith('.csv'):
```

### Comparing `cleanmydataset-1.0.0/cleanmydataset.egg-info/PKG-INFO` & `cleanmydataset-1.1.0/cleanmydataset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanmydataset
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cleanmydataset-1.0.0/setup.py` & `cleanmydataset-1.1.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cleanmydataset',
-    version='1.0.0',
+    version='1.1.0',
     author=['Samuel Shine', 'Alex Benjamin'],
     author_email='samuelshine112003@gmail.com',
     description='A Python package for cleaning and preprocessing data in pandas DataFrames',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/samuelshine/cleanmydata',
     packages=find_packages(),
@@ -18,15 +18,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     install_requires=[
         'pandas',
         'numpy',
-        'datetime',
         'charset_normalizer',
         'fuzzywuzzy',
         'scipy',
         'dateutil',
         'emoji',
         'googletrans',
     ],
```

