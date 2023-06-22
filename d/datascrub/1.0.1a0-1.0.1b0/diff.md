# Comparing `tmp/datascrub-1.0.1a0.tar.gz` & `tmp/datascrub-1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datascrub-1.0.1a0.tar", last modified: Thu Jun 22 06:28:23 2023, max compression
+gzip compressed data, was "datascrub-1.0.1b0.tar", last modified: Thu Jun 22 06:32:45 2023, max compression
```

## Comparing `datascrub-1.0.1a0.tar` & `datascrub-1.0.1b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:28:23.496089 datascrub-1.0.1a0/
--rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.0.1a0/LICENSE.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)     5612 2023-06-22 06:28:23.495938 datascrub-1.0.1a0/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)     4913 2023-06-22 06:10:32.000000 datascrub-1.0.1a0/README.md
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:28:23.494465 datascrub-1.0.1a0/datascrub/
--rw-r--r--   0 samuelshine   (501) staff       (20)       44 2023-06-22 06:27:51.000000 datascrub-1.0.1a0/datascrub/__init__.py
--rw-r--r--   0 samuelshine   (501) staff       (20)     8824 2023-06-22 04:48:03.000000 datascrub-1.0.1a0/datascrub/datascrub.py
-drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:28:23.495678 datascrub-1.0.1a0/datascrub.egg-info/
--rw-r--r--   0 samuelshine   (501) staff       (20)     5612 2023-06-22 06:28:23.000000 datascrub-1.0.1a0/datascrub.egg-info/PKG-INFO
--rw-r--r--   0 samuelshine   (501) staff       (20)      239 2023-06-22 06:28:23.000000 datascrub-1.0.1a0/datascrub.egg-info/SOURCES.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 06:28:23.000000 datascrub-1.0.1a0/datascrub.egg-info/dependency_links.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:28:23.000000 datascrub-1.0.1a0/datascrub.egg-info/requires.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-06-22 06:28:23.000000 datascrub-1.0.1a0/datascrub.egg-info/top_level.txt
--rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 06:28:23.496147 datascrub-1.0.1a0/setup.cfg
--rw-r--r--   0 samuelshine   (501) staff       (20)     1014 2023-06-22 06:28:15.000000 datascrub-1.0.1a0/setup.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:32:45.411840 datascrub-1.0.1b0/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1069 2023-06-21 11:22:05.000000 datascrub-1.0.1b0/LICENSE.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5612 2023-06-22 06:32:45.411732 datascrub-1.0.1b0/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)     4913 2023-06-22 06:10:32.000000 datascrub-1.0.1b0/README.md
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:32:45.410769 datascrub-1.0.1b0/datascrub/
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:25.000000 datascrub-1.0.1b0/datascrub/__init__.py
+-rw-r--r--   0 samuelshine   (501) staff       (20)     8824 2023-06-22 04:48:03.000000 datascrub-1.0.1b0/datascrub/cleaner.py
+drwxr-xr-x   0 samuelshine   (501) staff       (20)        0 2023-06-22 06:32:45.411559 datascrub-1.0.1b0/datascrub.egg-info/
+-rw-r--r--   0 samuelshine   (501) staff       (20)     5612 2023-06-22 06:32:45.000000 datascrub-1.0.1b0/datascrub.egg-info/PKG-INFO
+-rw-r--r--   0 samuelshine   (501) staff       (20)      237 2023-06-22 06:32:45.000000 datascrub-1.0.1b0/datascrub.egg-info/SOURCES.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)        1 2023-06-22 06:32:45.000000 datascrub-1.0.1b0/datascrub.egg-info/dependency_links.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       67 2023-06-22 06:32:45.000000 datascrub-1.0.1b0/datascrub.egg-info/requires.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       10 2023-06-22 06:32:45.000000 datascrub-1.0.1b0/datascrub.egg-info/top_level.txt
+-rw-r--r--   0 samuelshine   (501) staff       (20)       38 2023-06-22 06:32:45.411876 datascrub-1.0.1b0/setup.cfg
+-rw-r--r--   0 samuelshine   (501) staff       (20)     1014 2023-06-22 06:32:39.000000 datascrub-1.0.1b0/setup.py
```

### Comparing `datascrub-1.0.1a0/LICENSE.txt` & `datascrub-1.0.1b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datascrub-1.0.1a0/PKG-INFO` & `datascrub-1.0.1b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.0.1a0
+Version: 1.0.1b0
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datascrub-1.0.1a0/README.md` & `datascrub-1.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `datascrub-1.0.1a0/datascrub/datascrub.py` & `datascrub-1.0.1b0/datascrub/cleaner.py`

 * *Files identical despite different names*

### Comparing `datascrub-1.0.1a0/datascrub.egg-info/PKG-INFO` & `datascrub-1.0.1b0/datascrub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datascrub
-Version: 1.0.1a0
+Version: 1.0.1b0
 Summary: A Python package for cleaning and preprocessing data in pandas DataFrames
 Home-page: https://github.com/samuelshine/cleanmydata
 Author: ['Samuel Shine', 'Alex Benjamin']
 Author-email: samuelshine112003@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `datascrub-1.0.1a0/setup.py` & `datascrub-1.0.1b0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='datascrub',
-    version='1.0.1a',
+    version='1.0.1b',
     author=['Samuel Shine', 'Alex Benjamin'],
     author_email='samuelshine112003@gmail.com',
     description='A Python package for cleaning and preprocessing data in pandas DataFrames',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/samuelshine/cleanmydata',
     packages=find_packages(),
```

