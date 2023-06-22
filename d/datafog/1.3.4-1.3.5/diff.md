# Comparing `tmp/datafog-1.3.4.tar.gz` & `tmp/datafog-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datafog-1.3.4.tar", last modified: Thu Jun 22 18:24:45 2023, max compression
+gzip compressed data, was "datafog-1.3.5.tar", last modified: Thu Jun 22 18:29:49 2023, max compression
```

## Comparing `datafog-1.3.4.tar` & `datafog-1.3.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:24:45.002368 datafog-1.3.4/
--rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.3.4/LICENSE.MD
--rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:24:45.002218 datafog-1.3.4/PKG-INFO
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:24:45.000440 datafog-1.3.4/datafog/
--rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.4/datafog/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.3.4/datafog/datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.4/datafog/models.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:24:45.001380 datafog-1.3.4/datafog.egg-info/
--rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:24:44.000000 datafog-1.3.4/datafog.egg-info/PKG-INFO
--rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 18:24:44.000000 datafog-1.3.4/datafog.egg-info/SOURCES.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 18:24:44.000000 datafog-1.3.4/datafog.egg-info/dependency_links.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       36 2023-06-22 18:24:44.000000 datafog-1.3.4/datafog.egg-info/requires.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 18:24:44.000000 datafog-1.3.4/datafog.egg-info/top_level.txt
--rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 18:24:45.002418 datafog-1.3.4/setup.cfg
--rw-r--r--   0 sidmohan   (501) staff       (20)      860 2023-06-22 18:24:41.000000 datafog-1.3.4/setup.py
-drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:24:45.002040 datafog-1.3.4/tests/
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.4/tests/__init__.py
--rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.4/tests/test_datafog.py
--rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.4/tests/test_models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.547083 datafog-1.3.5/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     1497 2023-06-21 21:52:32.000000 datafog-1.3.5/LICENSE.MD
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:29:49.546903 datafog-1.3.5/PKG-INFO
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.544780 datafog-1.3.5/datafog/
+-rw-r--r--   0 sidmohan   (501) staff       (20)       68 2023-06-21 23:20:54.000000 datafog-1.3.5/datafog/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     8126 2023-06-22 16:52:12.000000 datafog-1.3.5/datafog/datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)      477 2023-06-22 00:03:35.000000 datafog-1.3.5/datafog/models.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.545850 datafog-1.3.5/datafog.egg-info/
+-rw-r--r--   0 sidmohan   (501) staff       (20)     2041 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/PKG-INFO
+-rw-r--r--   0 sidmohan   (501) staff       (20)      291 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/SOURCES.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)        1 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/dependency_links.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       24 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/requires.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       14 2023-06-22 18:29:49.000000 datafog-1.3.5/datafog.egg-info/top_level.txt
+-rw-r--r--   0 sidmohan   (501) staff       (20)       38 2023-06-22 18:29:49.547149 datafog-1.3.5/setup.cfg
+-rw-r--r--   0 sidmohan   (501) staff       (20)      846 2023-06-22 18:29:38.000000 datafog-1.3.5/setup.py
+drwxr-xr-x   0 sidmohan   (501) staff       (20)        0 2023-06-22 18:29:49.546709 datafog-1.3.5/tests/
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:10.000000 datafog-1.3.5/tests/__init__.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)     6000 2023-06-22 16:54:40.000000 datafog-1.3.5/tests/test_datafog.py
+-rw-r--r--   0 sidmohan   (501) staff       (20)        0 2023-06-21 21:47:30.000000 datafog-1.3.5/tests/test_models.py
```

### Comparing `datafog-1.3.4/LICENSE.MD` & `datafog-1.3.5/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `datafog-1.3.4/PKG-INFO` & `datafog-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.4
+Version: 1.3.5
 Summary: A Python package for data anonymization
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
```

### Comparing `datafog-1.3.4/datafog/datafog.py` & `datafog-1.3.5/datafog/datafog.py`

 * *Files identical despite different names*

### Comparing `datafog-1.3.4/datafog.egg-info/PKG-INFO` & `datafog-1.3.5/datafog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafog
-Version: 1.3.4
+Version: 1.3.5
 Summary: A Python package for data anonymization
 Author: Sid Mohan
 Author-email: sid@datafog.dev
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.MD
```

### Comparing `datafog-1.3.4/setup.py` & `datafog-1.3.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 # Read README for the long description
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 
 setup(
     name='datafog',
-    version='1.3.4',  # versioning of your package
+    version='1.3.5',  # versioning of your package
     packages=find_packages(),  # automatically find all packages
     author='Sid Mohan',
     author_email='sid@datafog.dev',
     description='A Python package for data anonymization',
     long_description=long_description,
     long_description_content_type='text/markdown', 
-    install_requires=['faker', 'pandas', 'sqlalchemy','gym==0.21.0'],
+    install_requires=['faker', 'pandas', 'sqlalchemy'],
     classifiers=[
         'License :: OSI Approved :: BSD License',  # Choose a license
         'Programming Language :: Python :: 3.10',  # Python version
         # etc.
     ],
 )
```

### Comparing `datafog-1.3.4/tests/test_datafog.py` & `datafog-1.3.5/tests/test_datafog.py`

 * *Files identical despite different names*

