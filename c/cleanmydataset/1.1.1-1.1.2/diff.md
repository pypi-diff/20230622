# Comparing `tmp/cleanmydataset-1.1.1.tar.gz` & `tmp/cleanmydataset-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanmydataset-1.1.1.tar", last modified: Thu Jun 22 05:42:49 2023, max compression
+gzip compressed data, was "cleanmydataset-1.1.2.tar", last modified: Thu Jun 22 06:02:49 2023, max compression
```

## Comparing `cleanmydataset-1.1.1.tar` & `cleanmydataset-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 05:42:49.112187 cleanmydataset-1.1.1/
--rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 cleanmydataset-1.1.1/LICENSE.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 05:42:49.112073 cleanmydataset-1.1.1/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)     4918 2023-06-22 03:45:25.000000 cleanmydataset-1.1.1/README.md
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 05:42:49.111148 cleanmydataset-1.1.1/cleanmydataset/
--rw-r--r--   0 samuelshine   (501) staff       (20)       64 2023-06-22 03:43:17.000000 cleanmydataset-1.1.1/cleanmydataset/__init__.py
--rw-r--r--   0 samuelshine   (501) staff       (20)     8824 2023-06-22 04:48:03.000000 cleanmydataset-1.1.1/cleanmydataset/cleanmydataset.py
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 05:42:49.111908 cleanmydataset-1.1.1/cleanmydataset.egg-info/
--rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 05:42:49.000000 cleanmydataset-1.1.1/cleanmydataset.egg-info/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)      279 2023-06-22 05:42:49.000000 cleanmydataset-1.1.1/cleanmydataset.egg-info/SOURCES.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 05:42:49.000000 cleanmydataset-1.1.1/cleanmydataset.egg-info/dependency_links.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       76 2023-06-22 05:42:49.000000 cleanmydataset-1.1.1/cleanmydataset.egg-info/requires.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       15 2023-06-22 05:42:49.000000 cleanmydataset-1.1.1/cleanmydataset.egg-info/top_level.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 05:42:49.112221 cleanmydataset-1.1.1/setup.cfg
--rw-r--r--   0 samuelshine   (501) staff       (20)     1038 2023-06-22 05:42:45.000000 cleanmydataset-1.1.1/setup.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:02:49.417399 cleanmydataset-1.1.2/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 cleanmydataset-1.1.2/LICENSE.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 06:02:49.417254 cleanmydataset-1.1.2/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)     4918 2023-06-22 03:45:25.000000 cleanmydataset-1.1.2/README.md
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:02:49.416255 cleanmydataset-1.1.2/cleanmydataset/
+-rw-r--r--   0 samuelshine   (501) staff       (20)       64 2023-06-22 03:43:17.000000 cleanmydataset-1.1.2/cleanmydataset/__init__.py
+-rw-r--r--   0 samuelshine   (501) staff       (20)     8824 2023-06-22 04:48:03.000000 cleanmydataset-1.1.2/cleanmydataset/cleanmydataset.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:02:49.417065 cleanmydataset-1.1.2/cleanmydataset.egg-info/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5620 2023-06-22 06:02:49.000000 cleanmydataset-1.1.2/cleanmydataset.egg-info/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)      279 2023-06-22 06:02:49.000000 cleanmydataset-1.1.2/cleanmydataset.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 06:02:49.000000 cleanmydataset-1.1.2/cleanmydataset.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       76 2023-06-22 06:02:49.000000 cleanmydataset-1.1.2/cleanmydataset.egg-info/requires.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       15 2023-06-22 06:02:49.000000 cleanmydataset-1.1.2/cleanmydataset.egg-info/top_level.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 06:02:49.417438 cleanmydataset-1.1.2/setup.cfg
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1038 2023-06-22 06:02:12.000000 cleanmydataset-1.1.2/setup.py
```

### Comparing `cleanmydataset-1.1.1/LICENSE.txt` & `cleanmydataset-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cleanmydataset-1.1.1/PKG-INFO` & `cleanmydataset-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanmydataset
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

### Comparing `cleanmydataset-1.1.1/README.md` & `cleanmydataset-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cleanmydataset-1.1.1/cleanmydataset/cleanmydataset.py` & `cleanmydataset-1.1.2/cleanmydataset/cleanmydataset.py`

 * *Files identical despite different names*

### Comparing `cleanmydataset-1.1.1/cleanmydataset.egg-info/PKG-INFO` & `cleanmydataset-1.1.2/cleanmydataset.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanmydataset
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

### Comparing `cleanmydataset-1.1.1/setup.py` & `cleanmydataset-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cleanmydataset',
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

