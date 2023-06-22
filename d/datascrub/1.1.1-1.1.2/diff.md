# Comparing `tmp/datascrub-1.1.1.tar.gz` & `tmp/datascrub-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascrub-1.1.1.tar", last modified: Thu Jun 22 11:19:27 2023, max compression
+gzip compressed data, was "datascrub-1.1.2.tar", last modified: Thu Jun 22 11:28:23 2023, max compression
```

## Comparing `datascrub-1.1.1.tar` & `datascrub-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:19:27.274721 datascrub-1.1.1/
--rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.1/LICENSE.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:19:27.274599 datascrub-1.1.1/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)     4913 2023-06-22 06:10:32.000000 datascrub-1.1.1/README.md
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:19:27.273458 datascrub-1.1.1/datascrub/
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.1/datascrub/__init__.py
--rw-r--r--   0 samuelshine   (501) staff       (20)     9069 2023-06-22 11:18:24.000000 datascrub-1.1.1/datascrub/cleaner.py
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:19:27.274403 datascrub-1.1.1/datascrub.egg-info/
--rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/SOURCES.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/dependency_links.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/requires.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/top_level.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 11:19:27.274758 datascrub-1.1.1/setup.cfg
--rw-r--r--   0 samuelshine   (501) staff       (20)     1013 2023-06-22 11:18:38.000000 datascrub-1.1.1/setup.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:28:23.651081 datascrub-1.1.2/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.2/LICENSE.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:28:23.650956 datascrub-1.1.2/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)     4913 2023-06-22 06:10:32.000000 datascrub-1.1.2/README.md
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:28:23.650053 datascrub-1.1.2/datascrub/
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.2/datascrub/__init__.py
+-rw-r--r--   0 samuelshine   (501) staff       (20)     9448 2023-06-22 11:27:58.000000 datascrub-1.1.2/datascrub/cleaner.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:28:23.650763 datascrub-1.1.2/datascrub.egg-info/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/requires.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-06-22 11:28:23.000000 datascrub-1.1.2/datascrub.egg-info/top_level.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 11:28:23.651121 datascrub-1.1.2/setup.cfg
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1013 2023-06-22 11:28:18.000000 datascrub-1.1.2/setup.py
```

### Comparing `datascrub-1.1.1/LICENSE.txt` & `datascrub-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datascrub-1.1.1/PKG-INFO` & `datascrub-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datascrub-1.1.1/README.md` & `datascrub-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `datascrub-1.1.1/datascrub/cleaner.py` & `datascrub-1.1.2/datascrub/cleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 import datetime
 import charset_normalizer
 import fuzzywuzzy
 from fuzzywuzzy import process
 import re
 from scipy import stats
 from pandas.api.types import is_numeric_dtype
-#import dateutil.parser
 import emoji
 import string
 from googletrans import Translator
 
 
 class DataClean:
     def __init__(self, obj):
-      if isinstance(obj, str):
-        if obj.endswith('.csv'):
+      if isinstance(obj, pd.DataFrame):
+        # If data is a DataFrame, return it as it is
+        self.raw_data = obj
+      elif isinstance(obj, str):
+        # If data is a string, assume it's a file path and read the file into a DataFrame
+        if obj.endswith('.csv'):      #if data is a csv file
             self.raw_data = pd.read_csv(obj)
-        elif obj.endswith('.xlsx'):
+        elif obj.endswith('.xlsx'):   #if data is an excel file
             self.raw_data = pd.read_excel(obj)
-      elif isinstance(obj, pd.DataFrame):
-        self.raw_data = obj
+      else:
+        # If the object type is not recognized, raise an error or return None as per your requirement
+        raise ValueError("Invalid data type. Please provide a DataFrame or a file path.")
 
     def clean_data(self, columns):
         """
         Cleans text data in a pandas DataFrame.
 
         Parameters:
         columns (str, list): Either 'all' to clean all columns or a list of column names to clean.
```

### Comparing `datascrub-1.1.1/datascrub.egg-info/PKG-INFO` & `datascrub-1.1.2/datascrub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.1.1
+Version: 1.1.2
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datascrub-1.1.1/setup.py` & `datascrub-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='datascrub',
-    version='1.1.1',
+    version='1.1.2',
     author=['Samuel Shine', 'Alex Benjamin'],
     author_email='samuelshine112003@gmail.com',
     description='A Python package for cleaning and preprocessing data in pandas DataFrames',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/samuelshine/cleanmydata',
     packages=find_packages(),
```

