# Comparing `tmp/LNPLab-0.0.1.tar.gz` & `tmp/LNPLab-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LNPLab-0.0.1.tar", last modified: Thu Jun 22 06:51:18 2023, max compression
+gzip compressed data, was "LNPLab-0.0.2.tar", last modified: Thu Jun 22 07:28:57 2023, max compression
```

## Comparing `LNPLab-0.0.1.tar` & `LNPLab-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 06:51:18.980670 LNPLab-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-06-22 06:51:18.976624 LNPLab-0.0.1/LNPLab.egg-info/
--rw-rw-rw-   0        0        0      541 2023-06-22 06:51:18.000000 LNPLab-0.0.1/LNPLab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-06-22 06:51:18.000000 LNPLab-0.0.1/LNPLab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 06:51:18.000000 LNPLab-0.0.1/LNPLab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-22 06:51:18.000000 LNPLab-0.0.1/LNPLab.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       31 2023-06-22 06:51:18.000000 LNPLab-0.0.1/LNPLab.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 06:51:18.000000 LNPLab-0.0.1/LNPLab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      541 2023-06-22 06:51:18.979651 LNPLab-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-22 06:51:18.980670 LNPLab-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      742 2023-06-22 06:44:00.000000 LNPLab-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:28:57.458508 LNPLab-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-06-22 07:28:57.428870 LNPLab-0.0.2/LNPLab/
+-rw-rw-rw-   0        0        0       21 2023-06-22 07:28:54.000000 LNPLab-0.0.2/LNPLab/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:28:57.445113 LNPLab-0.0.2/LNPLab/cheminfo/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:19:48.000000 LNPLab-0.0.2/LNPLab/cheminfo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:28:57.450130 LNPLab-0.0.2/LNPLab/cheminfo/fin/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:19:58.000000 LNPLab-0.0.2/LNPLab/cheminfo/fin/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:22:00.000000 LNPLab-0.0.2/LNPLab/cheminfo/fin/tda.py
+-rw-rw-rw-   0        0        0      100 2023-06-22 07:27:47.000000 LNPLab-0.0.2/LNPLab/cheminfo/fin/vec.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:28:57.455497 LNPLab-0.0.2/LNPLab/cheminfo/prop/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:19:48.000000 LNPLab-0.0.2/LNPLab/cheminfo/prop/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:18:20.000000 LNPLab-0.0.2/LNPLab/cheminfo/prop/cal.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:28:57.443092 LNPLab-0.0.2/LNPLab.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-06-22 07:28:57.000000 LNPLab-0.0.2/LNPLab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-06-22 07:28:57.000000 LNPLab-0.0.2/LNPLab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:28:57.000000 LNPLab-0.0.2/LNPLab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-22 06:51:18.000000 LNPLab-0.0.2/LNPLab.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-06-22 07:28:57.000000 LNPLab-0.0.2/LNPLab.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 07:28:57.000000 LNPLab-0.0.2/LNPLab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      541 2023-06-22 07:28:57.457504 LNPLab-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:28:57.458508 LNPLab-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      742 2023-06-22 07:28:54.000000 LNPLab-0.0.2/setup.py
```

### Comparing `LNPLab-0.0.1/LNPLab.egg-info/PKG-INFO` & `LNPLab-0.0.2/LNPLab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: LNPLab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utils for LNP Solution and Clients
 Home-page: https://github.com/wosaKim/LNPLab
 Author: william
 Author-email: william@lnpsolution.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: Deep Learning Model Evaluation,Smart Banch
```

### Comparing `LNPLab-0.0.1/PKG-INFO` & `LNPLab-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: LNPLab
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utils for LNP Solution and Clients
 Home-page: https://github.com/wosaKim/LNPLab
 Author: william
 Author-email: william@lnpsolution.com
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: Deep Learning Model Evaluation,Smart Banch
```

### Comparing `LNPLab-0.0.1/setup.py` & `LNPLab-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='LNPLab',
-    version='0.0.1',
+    version='0.0.2',
     description='Utils for LNP Solution and Clients',
     author='william',
     author_email='william@lnpsolution.com',
     url='https://github.com/wosaKim/LNPLab',
     install_requires=['tqdm', 'pandas', 'scikit-learn', 'rdkit'],
     packages=find_packages(exclude=[]),
     keywords=['Deep Learning Model Evaluation', 'Smart Banch'],
```

