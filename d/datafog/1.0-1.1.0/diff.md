# Comparing `tmp/datafog-1.0.tar.gz` & `tmp/datafog-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-1.0.tar", last modified: Wed Jun 21 23:25:45 2023, max compression
+gzip compressed data, was "datafog-1.1.0.tar", last modified: Thu Jun 22 00:12:41 2023, max compression
```

## Comparing `datafog-1.0.tar` & `datafog-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-21 23:25:45.471934 datafog-1.0/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.0/LICENSE.MD
--rw-r--r--   0 sidmohan   (501) staff       (20)      298 2023-06-21 23:25:45.471777 datafog-1.0/PKG-INFO
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-21 23:25:45.470272 datafog-1.0/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.0/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     7814 2023-06-21 23:21:55.000000 datafog-1.0/datafog/datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      476 2023-06-21 23:20:54.000000 datafog-1.0/datafog/models.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-21 23:25:45.471226 datafog-1.0/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)      298 2023-06-21 23:25:45.000000 datafog-1.0/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-21 23:25:45.000000 datafog-1.0/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-21 23:25:45.000000 datafog-1.0/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       55 2023-06-21 23:25:45.000000 datafog-1.0/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-21 23:25:45.000000 datafog-1.0/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-21 23:25:45.471979 datafog-1.0/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)      905 2023-06-21 23:25:11.000000 datafog-1.0/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-21 23:25:45.471597 datafog-1.0/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.0/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:20.000000 datafog-1.0/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.0/tests/test_models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.348443 datafog-1.1.0/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.1.0/LICENSE.MD
+-rw-r--r--   0 sidmohan   (501) staff       (20)      300 2023-06-22 00:12:41.348246 datafog-1.1.0/PKG-INFO
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.346483 datafog-1.1.0/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.1.0/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     7829 2023-06-21 23:55:11.000000 datafog-1.1.0/datafog/datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.1.0/datafog/models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.347325 datafog-1.1.0/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)      300 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       63 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 00:12:41.000000 datafog-1.1.0/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 00:12:41.348506 datafog-1.1.0/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)      917 2023-06-22 00:07:48.000000 datafog-1.1.0/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 00:12:41.347993 datafog-1.1.0/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.1.0/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     3123 2023-06-22 00:02:37.000000 datafog-1.1.0/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.1.0/tests/test_models.py
```

### Comparing `datafog-1.0/LICENSE.MD` & `datafog-1.1.0/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `datafog-1.0/datafog/datafog.py` & `datafog-1.1.0/datafog/datafog.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import logging
 import binascii
 import faker
 from faker import Faker
 from .models import ValueMapping, Base
 import typing
 from typing import Optional, Dict, Tuple, List, Any
+import hashlib
 
 # Logging
 logging.basicConfig(filename='app.log', filemode='w', format='%(name)s - %(levelname)s - %(message)s', level=logging.DEBUG)
 
 
 class DataFog:
```

### Comparing `datafog-1.0/setup.py` & `datafog-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from setuptools import setup, find_packages
 
 
 
 
 setup(
     name='datafog',
-    version='1.0',  # versioning of your package
+    version='1.1.0',  # versioning of your package
     packages=find_packages(),  # automatically find all packages
     author='Sid Mohan',
     author_email='sid@datafog.dev',
     description='A Python package that provides several methods for data handling',  # a brief description of your package
     long_description=open('README.md').read(),  # a long description read from the README.md file
-    install_requires=['faker', 'pandas','sqlalchemy','sqlalchemy.orm','werkzeug','typing'],  # a list of other Python packages required by this package
+    install_requires=['faker', 'pandas','sqlalchemy','sqlalchemy.orm','werkzeug','typing','hashlib'],  # a list of other Python packages required by this package
     classifiers=[
         'License :: OSI Approved :: BSD License',  # Choose a license
         'Programming Language :: Python :: 3.10',  # Python version
         # etc.
     ],
 )
```

