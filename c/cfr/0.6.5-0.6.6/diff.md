# Comparing `tmp/cfr-0.6.5.tar.gz` & `tmp/cfr-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfr-0.6.5.tar", last modified: Thu Jun 22 18:48:40 2023, max compression
+gzip compressed data, was "cfr-0.6.6.tar", last modified: Thu Jun 22 18:50:58 2023, max compression
```

## Comparing `cfr-0.6.5.tar` & `cfr-0.6.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.101587 cfr-0.6.5/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.5/LICENSE
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:48:40.101391 cfr-0.6.5/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.5/README.md
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.090044 cfr-0.6.5/bin/
--rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.5/bin/cfr
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.097023 cfr-0.6.5/cfr/
--rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-0.6.5/cfr/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.5/cfr/climate.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.100884 cfr-0.6.5/cfr/da/
--rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.5/cfr/da/__init__.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.5/cfr/da/enkf.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.5/cfr/gcm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.5/cfr/ml.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    67033 2023-06-22 17:29:40.000000 cfr-0.6.5/cfr/proxy.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.5/cfr/psm.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-21 23:52:13.000000 cfr-0.6.5/cfr/reconjob.py
--rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.5/cfr/reconres.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.5/cfr/ts.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    26722 2023-06-20 23:08:04.000000 cfr-0.6.5/cfr/utils.py
--rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.5/cfr/visual.py
-drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:48:40.100005 cfr-0.6.5/cfr.egg-info/
--rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.5/cfr.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu    (502) staff       (20)      203 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/requires.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-22 18:48:40.000000 cfr-0.6.5/cfr.egg-info/top_level.txt
--rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-22 18:48:40.101715 cfr-0.6.5/setup.cfg
--rw-r--r--   0 fengzhu    (502) staff       (20)     1413 2023-06-22 18:47:12.000000 cfr-0.6.5/setup.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:50:58.787927 cfr-0.6.6/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1516 2022-04-27 05:34:15.000000 cfr-0.6.6/LICENSE
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:50:58.787716 cfr-0.6.6/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1207 2023-05-29 21:16:00.000000 cfr-0.6.6/README.md
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:50:58.775645 cfr-0.6.6/bin/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     5163 2023-06-19 02:34:42.000000 cfr-0.6.6/bin/cfr
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:50:58.782914 cfr-0.6.6/cfr/
+-rw-r--r--   0 fengzhu    (502) staff       (20)      732 2023-06-21 18:25:21.000000 cfr-0.6.6/cfr/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22467 2023-05-29 23:34:35.000000 cfr-0.6.6/cfr/climate.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:50:58.787129 cfr-0.6.6/cfr/da/
+-rw-r--r--   0 fengzhu    (502) staff       (20)       22 2022-07-02 05:30:36.000000 cfr-0.6.6/cfr/da/__init__.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    16319 2023-03-27 02:39:30.000000 cfr-0.6.6/cfr/da/enkf.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    22484 2023-04-17 19:25:37.000000 cfr-0.6.6/cfr/gcm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     7623 2022-05-05 04:13:16.000000 cfr-0.6.6/cfr/ml.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    67033 2023-06-22 17:29:40.000000 cfr-0.6.6/cfr/proxy.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    45058 2023-06-20 03:51:38.000000 cfr-0.6.6/cfr/psm.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54926 2023-06-21 23:52:13.000000 cfr-0.6.6/cfr/reconjob.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)     2311 2023-03-27 02:39:30.000000 cfr-0.6.6/cfr/reconres.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    19837 2023-05-29 21:16:00.000000 cfr-0.6.6/cfr/ts.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    26722 2023-06-20 23:08:04.000000 cfr-0.6.6/cfr/utils.py
+-rw-r--r--   0 fengzhu    (502) staff       (20)    54810 2023-04-17 19:25:37.000000 cfr-0.6.6/cfr/visual.py
+drwxr-xr-x   0 fengzhu    (502) staff       (20)        0 2023-06-22 18:50:58.786158 cfr-0.6.6/cfr.egg-info/
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1770 2023-06-22 18:50:58.000000 cfr-0.6.6/cfr.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu    (502) staff       (20)      373 2023-06-22 18:50:58.000000 cfr-0.6.6/cfr.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2023-06-22 18:50:58.000000 cfr-0.6.6/cfr.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        1 2022-04-28 04:59:29.000000 cfr-0.6.6/cfr.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu    (502) staff       (20)      208 2023-06-22 18:50:58.000000 cfr-0.6.6/cfr.egg-info/requires.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)        4 2023-06-22 18:50:58.000000 cfr-0.6.6/cfr.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu    (502) staff       (20)       38 2023-06-22 18:50:58.787997 cfr-0.6.6/setup.cfg
+-rw-r--r--   0 fengzhu    (502) staff       (20)     1418 2023-06-22 18:50:38.000000 cfr-0.6.6/setup.py
```

### Comparing `cfr-0.6.5/LICENSE` & `cfr-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/PKG-INFO` & `cfr-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.5
+Version: 0.6.6
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.5/README.md` & `cfr-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/bin/cfr` & `cfr-0.6.6/bin/cfr`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/__init__.py` & `cfr-0.6.6/cfr/__init__.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/climate.py` & `cfr-0.6.6/cfr/climate.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/da/enkf.py` & `cfr-0.6.6/cfr/da/enkf.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/gcm.py` & `cfr-0.6.6/cfr/gcm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/ml.py` & `cfr-0.6.6/cfr/ml.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/proxy.py` & `cfr-0.6.6/cfr/proxy.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/psm.py` & `cfr-0.6.6/cfr/psm.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/reconjob.py` & `cfr-0.6.6/cfr/reconjob.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/reconres.py` & `cfr-0.6.6/cfr/reconres.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/ts.py` & `cfr-0.6.6/cfr/ts.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/utils.py` & `cfr-0.6.6/cfr/utils.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr/visual.py` & `cfr-0.6.6/cfr/visual.py`

 * *Files identical despite different names*

### Comparing `cfr-0.6.5/cfr.egg-info/PKG-INFO` & `cfr-0.6.6/cfr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfr
-Version: 0.6.5
+Version: 0.6.6
 Summary: cfr: a Python package for Climate Field Reconstruction
 Home-page: https://github.com/fzhu2e/cfr
 Author: Feng Zhu, Julien Emile-Geay
 Author-email: fengzhu@ucar.edu, julieneg@usc.edu
 License: BSD 3-Clause
 Keywords: climate field reconstruction
 Classifier: Natural Language :: English
```

### Comparing `cfr-0.6.5/setup.py` & `cfr-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='cfr',  # required
-    version='0.6.5',
+    version='0.6.6',
     description='cfr: a Python package for Climate Field Reconstruction',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Julien Emile-Geay',
     author_email='fengzhu@ucar.edu, julieneg@usc.edu',
     url='https://github.com/fzhu2e/cfr',
     packages=find_packages(),
@@ -41,15 +41,15 @@
     extras_require={
         'psm': [
             'pathos',
             'fbm',
             'pyvsl',
         ],
         'ml': [
-            'sklearn',
+            'scikit-learn',
             'torch',
             'torchvision',
         ],
         'graphem': [
             'cython',
             'scikit-learn',
             'cfr-graphem',
```

