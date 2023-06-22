# Comparing `tmp/datascrub-1.1.0.tar.gz` & `tmp/datascrub-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascrub-1.1.0.tar", last modified: Thu Jun 22 06:36:07 2023, max compression
+gzip compressed data, was "datascrub-1.1.1.tar", last modified: Thu Jun 22 11:19:27 2023, max compression
```

## Comparing `datascrub-1.1.0.tar` & `datascrub-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:36:07.553171 datascrub-1.1.0/
--rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.0/LICENSE.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 06:36:07.553063 datascrub-1.1.0/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)     4913 2023-06-22 06:10:32.000000 datascrub-1.1.0/README.md
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:36:07.552112 datascrub-1.1.0/datascrub/
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.0/datascrub/__init__.py
--rw-r--r--   0 samuelshine   (501) staff       (20)     8824 2023-06-22 04:48:03.000000 datascrub-1.1.0/datascrub/cleaner.py
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:36:07.552899 datascrub-1.1.0/datascrub.egg-info/
--rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 06:36:07.000000 datascrub-1.1.0/datascrub.egg-info/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-06-22 06:36:07.000000 datascrub-1.1.0/datascrub.egg-info/SOURCES.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 06:36:07.000000 datascrub-1.1.0/datascrub.egg-info/dependency_links.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:36:07.000000 datascrub-1.1.0/datascrub.egg-info/requires.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-06-22 06:36:07.000000 datascrub-1.1.0/datascrub.egg-info/top_level.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 06:36:07.553207 datascrub-1.1.0/setup.cfg
--rw-r--r--   0 samuelshine   (501) staff       (20)     1013 2023-06-22 06:36:00.000000 datascrub-1.1.0/setup.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:19:27.274721 datascrub-1.1.1/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.1.1/LICENSE.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:19:27.274599 datascrub-1.1.1/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)     4913 2023-06-22 06:10:32.000000 datascrub-1.1.1/README.md
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:19:27.273458 datascrub-1.1.1/datascrub/
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.1.1/datascrub/__init__.py
+-rw-r--r--   0 samuelshine   (501) staff       (20)     9069 2023-06-22 11:18:24.000000 datascrub-1.1.1/datascrub/cleaner.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 11:19:27.274403 datascrub-1.1.1/datascrub.egg-info/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5610 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/requires.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-06-22 11:19:27.000000 datascrub-1.1.1/datascrub.egg-info/top_level.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 11:19:27.274758 datascrub-1.1.1/setup.cfg
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1013 2023-06-22 11:18:38.000000 datascrub-1.1.1/setup.py
```

### Comparing `datascrub-1.1.0/LICENSE.txt` & `datascrub-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datascrub-1.1.0/PKG-INFO` & `datascrub-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datascrub-1.1.0/README.md` & `datascrub-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `datascrub-1.1.0/datascrub/cleaner.py` & `datascrub-1.1.1/datascrub/cleaner.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,29 @@
 import datetime
 import charset_normalizer
 import fuzzywuzzy
 from fuzzywuzzy import process
 import re
 from scipy import stats
 from pandas.api.types import is_numeric_dtype
+#import dateutil.parser
 import emoji
 import string
 from googletrans import Translator
 
+
 class DataClean:
-    def __init__(self, filepath):
-        if filepath.endswith('.csv'):
-            self.raw_data = pd.read_csv(filepath)
-        elif filepath.endswith('.xlsx'):
-            self.raw_data = pd.read_excel(filepath)
+    def __init__(self, obj):
+      if isinstance(obj, str):
+        if obj.endswith('.csv'):
+            self.raw_data = pd.read_csv(obj)
+        elif obj.endswith('.xlsx'):
+            self.raw_data = pd.read_excel(obj)
+      elif isinstance(obj, pd.DataFrame):
+        self.raw_data = obj
 
     def clean_data(self, columns):
         """
         Cleans text data in a pandas DataFrame.
 
         Parameters:
         columns (str, list): Either 'all' to clean all columns or a list of column names to clean.
@@ -186,23 +191,30 @@
         missing_values (dict): Actions to be taken on missing values. Refer `handle_missing_values` for more details.
         perform_scaling_normalization (bool): If True, will perform scaling normalization on numerical columns.
         explode (dict): Columns to be exploded. Keys are column names and values are separators for splitting.
         parse_date (list): List of column names to be converted to datetime format.
         translate_column_names (dict): Dictionary mapping column names to overwrite boolean values for translation.
 
         Returns:
-        pd.DataFrame: Updated DataFrame with cleaned, transformed, and translated columns.
+        pd.DataFrame: Updated DataFrame with cleaned and processed data.
         """
-        updated_data = self.clean_data(clean)
-        updated_data = self.handle_missing_values(missing_values)
+        if missing_values:
+            self.raw_data = self.handle_missing_values(missing_values)
 
-        if perform_scaling_normalization_bool:
-            updated_data = self.perform_scaling_normalization()
+        if parse_date:
+            self.raw_data = self.parse_date_column(parse_date)
 
-        updated_data = self.explode_data(explode)
+        if translate_column_names:
+            self.raw_data = self.translate_columns(translate_column_names)
 
-        if parse_date:
-            updated_data = self.parse_date_column(parse_date)
+        if clean:
+            self.raw_data = self.clean_data(clean)
 
-        updated_data = self.translate_columns(translate_column_names)
+        if perform_scaling_normalization_bool:
+            self.raw_data = self.perform_scaling_normalization()
 
-        return updated_data
+        if explode:
+            self.raw_data = self.explode_data(explode)
+
+        self.raw_data = self.dupli()
+
+        return self.raw_data
```

### Comparing `datascrub-1.1.0/datascrub.egg-info/PKG-INFO` & `datascrub-1.1.1/datascrub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datascrub-1.1.0/setup.py` & `datascrub-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='datascrub',
-    version='1.1.0',
+    version='1.1.1',
     author=['Samuel Shine', 'Alex Benjamin'],
     author_email='samuelshine112003@gmail.com',
     description='A Python package for cleaning and preprocessing data in pandas DataFrames',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/samuelshine/cleanmydata',
     packages=find_packages(),
```

