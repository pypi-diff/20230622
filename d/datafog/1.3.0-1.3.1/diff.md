# Comparing `tmp/datafog-1.3.0.tar.gz` & `tmp/datafog-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datafog-1.3.0.tar", last modified: Thu Jun 22 17:55:46 2023, max compression
+gzip compressed data, was "dist/datafog-1.3.1.tar", last modified: Thu Jun 22 18:01:41 2023, max compression
```

## Comparing `datafog-1.3.0.tar` & `datafog-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2334 2023-06-22 17:55:46.000000 datafog-1.3.0/PKG-INFO
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.3.0/datafog/datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.0/datafog/models.py
--rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.0/datafog/__init__.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.0/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.0/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.0/tests/test_models.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      893 2023-06-22 17:55:33.000000 datafog-1.3.0/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2334 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      280 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       63 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 17:55:46.000000 datafog-1.3.0/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 17:55:46.000000 datafog-1.3.0/setup.cfg
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:01:41.000000 datafog-1.3.1/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2334 2023-06-22 18:01:41.000000 datafog-1.3.1/PKG-INFO
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:01:41.000000 datafog-1.3.1/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.3.1/datafog/datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.1/datafog/models.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.1/datafog/__init__.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:01:41.000000 datafog-1.3.1/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.1/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.1/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.1/tests/test_models.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      893 2023-06-22 18:01:09.000000 datafog-1.3.1/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:01:41.000000 datafog-1.3.1/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2334 2023-06-22 18:01:41.000000 datafog-1.3.1/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      280 2023-06-22 18:01:41.000000 datafog-1.3.1/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       63 2023-06-22 18:01:41.000000 datafog-1.3.1/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 18:01:41.000000 datafog-1.3.1/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 18:01:41.000000 datafog-1.3.1/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 18:01:41.000000 datafog-1.3.1/setup.cfg
```

### Comparing `datafog-1.3.0/PKG-INFO` & `datafog-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.0
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 License: UNKNOWN
 Description: # DataFog
```

### Comparing `datafog-1.3.0/datafog/datafog.py` & `datafog-1.3.1/datafog/datafog.py`

 * *Files identical despite different names*

### Comparing `datafog-1.3.0/tests/test_datafog.py` & `datafog-1.3.1/tests/test_datafog.py`

 * *Files identical despite different names*

### Comparing `datafog-1.3.0/setup.py` & `datafog-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Read README for the long description
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
     name='datafog',
-    version='1.3.0',  # versioning of your package
+    version='1.3.1',  # versioning of your package
     packages=find_packages(),  # automatically find all packages
     author='Sid Mohan',
     author_email='sid@datafog.dev',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     install_requires=['faker', 'pandas','sqlalchemy','sqlalchemy.orm','werkzeug','typing','hashlib'],  # a list of other Python packages required by this package
     classifiers=[
```

### Comparing `datafog-1.3.0/datafog.egg-info/PKG-INFO` & `datafog-1.3.1/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.0
+Version: 1.3.1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 License: UNKNOWN
 Description: # DataFog
```

