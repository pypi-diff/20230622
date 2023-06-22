# Comparing `tmp/pythemis-0.9.5.1.tar.gz` & `tmp/pythemis-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pythemis-0.9.5.1.tar", last modified: Fri Oct 13 15:50:43 2017, max compression
+gzip compressed data, was "dist/pythemis-0.9.6.tar", last modified: Thu Dec 14 10:12:18 2017, max compression
```

## Comparing `pythemis-0.9.5.1.tar` & `pythemis-0.9.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 hdf        (501) staff       (20)        0 2017-10-13 15:50:43.000000 pythemis-0.9.5.1/
--rw-r--r--   0 hdf        (501) staff       (20)       60 2017-09-07 11:25:47.000000 pythemis-0.9.5.1/AUTHORS
--rw-r--r--   0 hdf        (501) staff       (20)     9694 2017-09-07 11:25:47.000000 pythemis-0.9.5.1/LICENSE
--rw-r--r--   0 hdf        (501) staff       (20)       51 2017-09-07 11:25:47.000000 pythemis-0.9.5.1/MANIFEST.in
--rw-r--r--   0 hdf        (501) staff       (20)     1634 2017-10-13 15:50:43.000000 pythemis-0.9.5.1/PKG-INFO
-drwxr-xr-x   0 hdf        (501) staff       (20)        0 2017-10-13 15:50:43.000000 pythemis-0.9.5.1/pythemis/
--rw-r--r--   0 hdf        (501) staff       (20)      648 2017-09-07 11:58:48.000000 pythemis-0.9.5.1/pythemis/__init__.py
--rw-r--r--   0 hdf        (501) staff       (20)     1295 2017-09-07 11:58:48.000000 pythemis-0.9.5.1/pythemis/exception.py
--rw-r--r--   0 hdf        (501) staff       (20)     8801 2017-10-13 13:33:41.000000 pythemis-0.9.5.1/pythemis/scell.py
--rw-r--r--   0 hdf        (501) staff       (20)     4433 2017-09-07 11:58:48.000000 pythemis-0.9.5.1/pythemis/scomparator.py
--rw-r--r--   0 hdf        (501) staff       (20)     2520 2017-09-07 11:58:48.000000 pythemis-0.9.5.1/pythemis/skeygen.py
--rw-r--r--   0 hdf        (501) staff       (20)     4740 2017-09-07 11:58:48.000000 pythemis-0.9.5.1/pythemis/smessage.py
--rw-r--r--   0 hdf        (501) staff       (20)    10669 2017-09-07 11:58:48.000000 pythemis-0.9.5.1/pythemis/ssession.py
-drwxr-xr-x   0 hdf        (501) staff       (20)        0 2017-10-13 15:50:43.000000 pythemis-0.9.5.1/pythemis.egg-info/
--rw-r--r--   0 hdf        (501) staff       (20)        1 2017-10-13 15:50:42.000000 pythemis-0.9.5.1/pythemis.egg-info/dependency_links.txt
--rw-r--r--   0 hdf        (501) staff       (20)     1634 2017-10-13 15:50:42.000000 pythemis-0.9.5.1/pythemis.egg-info/PKG-INFO
--rw-r--r--   0 hdf        (501) staff       (20)      332 2017-10-13 15:50:43.000000 pythemis-0.9.5.1/pythemis.egg-info/SOURCES.txt
--rw-r--r--   0 hdf        (501) staff       (20)        9 2017-10-13 15:50:42.000000 pythemis-0.9.5.1/pythemis.egg-info/top_level.txt
--rw-r--r--   0 hdf        (501) staff       (20)      373 2017-09-07 11:25:47.000000 pythemis-0.9.5.1/README.rst
--rw-r--r--   0 hdf        (501) staff       (20)      132 2017-10-13 15:50:43.000000 pythemis-0.9.5.1/setup.cfg
--rw-r--r--   0 hdf        (501) staff       (20)     2027 2017-10-13 15:49:30.000000 pythemis-0.9.5.1/setup.py
+drwxr-xr-x   0 lagovas   (1000) lagovas   (1000)        0 2017-12-14 10:12:18.000000 pythemis-0.9.6/
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     1598 2017-12-14 10:12:18.000000 pythemis-0.9.6/PKG-INFO
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     2025 2017-12-14 10:11:17.000000 pythemis-0.9.6/setup.py
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)      132 2017-12-14 10:12:18.000000 pythemis-0.9.6/setup.cfg
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)      373 2017-12-14 10:10:46.000000 pythemis-0.9.6/README.rst
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)       51 2017-12-14 10:10:46.000000 pythemis-0.9.6/MANIFEST.in
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     9694 2017-12-14 10:10:46.000000 pythemis-0.9.6/LICENSE
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)       60 2017-12-14 10:10:46.000000 pythemis-0.9.6/AUTHORS
+drwxr-xr-x   0 lagovas   (1000) lagovas   (1000)        0 2017-12-14 10:12:18.000000 pythemis-0.9.6/pythemis.egg-info/
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)        9 2017-12-14 10:12:18.000000 pythemis-0.9.6/pythemis.egg-info/top_level.txt
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)        1 2017-12-14 10:12:18.000000 pythemis-0.9.6/pythemis.egg-info/dependency_links.txt
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)      332 2017-12-14 10:12:18.000000 pythemis-0.9.6/pythemis.egg-info/SOURCES.txt
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     1598 2017-12-14 10:12:18.000000 pythemis-0.9.6/pythemis.egg-info/PKG-INFO
+drwxr-xr-x   0 lagovas   (1000) lagovas   (1000)        0 2017-12-14 10:12:18.000000 pythemis-0.9.6/pythemis/
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)    10669 2017-12-14 10:10:46.000000 pythemis-0.9.6/pythemis/ssession.py
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     4740 2017-12-14 10:10:46.000000 pythemis-0.9.6/pythemis/smessage.py
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     2520 2017-12-14 10:10:46.000000 pythemis-0.9.6/pythemis/skeygen.py
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     4433 2017-12-14 10:10:46.000000 pythemis-0.9.6/pythemis/scomparator.py
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     8801 2017-12-14 10:10:46.000000 pythemis-0.9.6/pythemis/scell.py
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)     1295 2017-12-14 10:10:46.000000 pythemis-0.9.6/pythemis/exception.py
+-rw-r--r--   0 lagovas   (1000) lagovas   (1000)      648 2017-12-14 10:10:46.000000 pythemis-0.9.6/pythemis/__init__.py
```

### Comparing `pythemis-0.9.5.1/LICENSE` & `pythemis-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/PKG-INFO` & `pythemis-0.9.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: pythemis
-Version: 0.9.5.1
+Version: 0.9.6
 Summary: UNKNOWN
 Home-page: https://cossacklabs.com
 Author: CossackLabs
 Author-email: dev@cossacklabs.com
 License: Apache 2.0
-Description-Content-Type: UNKNOWN
 Description: themis
         =====
         Themis is a data security library, providing users with high-quality 
         security services for secure messaging of any kinds and flexible data 
         storage. Themis is aimed at modern developers, with high level OOP 
         wrappers for Ruby, Python, PHP, Java / Android and iOS / OSX. It is d
         esigned with ease of use in mind, high security and cross-platform
```

### Comparing `pythemis-0.9.5.1/pythemis/__init__.py` & `pythemis-0.9.6/pythemis/__init__.py`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/pythemis/exception.py` & `pythemis-0.9.6/pythemis/exception.py`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/pythemis/scell.py` & `pythemis-0.9.6/pythemis/scell.py`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/pythemis/scomparator.py` & `pythemis-0.9.6/pythemis/scomparator.py`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/pythemis/skeygen.py` & `pythemis-0.9.6/pythemis/skeygen.py`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/pythemis/smessage.py` & `pythemis-0.9.6/pythemis/smessage.py`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/pythemis/ssession.py` & `pythemis-0.9.6/pythemis/ssession.py`

 * *Files identical despite different names*

### Comparing `pythemis-0.9.5.1/pythemis.egg-info/PKG-INFO` & `pythemis-0.9.6/pythemis.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 1.1
 Name: pythemis
-Version: 0.9.5.1
+Version: 0.9.6
 Summary: UNKNOWN
 Home-page: https://cossacklabs.com
 Author: CossackLabs
 Author-email: dev@cossacklabs.com
 License: Apache 2.0
-Description-Content-Type: UNKNOWN
 Description: themis
         =====
         Themis is a data security library, providing users with high-quality 
         security services for secure messaging of any kinds and flexible data 
         storage. Themis is aimed at modern developers, with high level OOP 
         wrappers for Ruby, Python, PHP, Java / Android and iOS / OSX. It is d
         esigned with ease of use in mind, high security and cross-platform
```

### Comparing `pythemis-0.9.5.1/setup.py` & `pythemis-0.9.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 install_requires = []
 if sys.version_info < (3, 4):
     install_requires.append('enum34')
 
 setup(
     name='pythemis',
-    version='0.9.5.1',
+    version='0.9.6',
 
     description='',
     long_description=open("README.rst").read(),
     license='Apache 2.0',
     url='https://cossacklabs.com',
 
     author='CossackLabs',
```

