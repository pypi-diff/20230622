# Comparing `tmp/ssbtoolkit-1.0.5.tar.gz` & `tmp/ssbtoolkit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssbtoolkit-1.0.5.tar", last modified: Mon Apr 10 13:58:23 2023, max compression
+gzip compressed data, was "ssbtoolkit-1.0.6.tar", last modified: Thu Jun 22 11:59:36 2023, max compression
```

## Comparing `ssbtoolkit-1.0.5.tar` & `ssbtoolkit-1.0.6.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:58:23.188085 ssbtoolkit-1.0.5/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       66 2023-04-10 11:48:28.000000 ssbtoolkit-1.0.5/MANIFEST.in
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 13:58:23.188085 ssbtoolkit-1.0.5/PKG-INFO
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       38 2023-04-10 13:58:23.188085 ssbtoolkit-1.0.5/setup.cfg
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1261 2023-04-10 13:58:20.000000 ssbtoolkit-1.0.5/setup.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:58:23.188085 ssbtoolkit-1.0.5/ssbtoolkit/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    17110 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/Utils.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    71651 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/__init__.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:58:23.188085 ssbtoolkit-1.0.5/ssbtoolkit/pathways/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    20658 2023-04-10 13:57:48.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gi.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1736 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gi_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2640 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gi_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    14154 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gq.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1153 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gq_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     1121 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gq_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    21135 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gs.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1763 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gs_parameters.csv
--rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2709 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gs_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    15771 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1725 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway_parameters.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1319 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway_reactions.csv
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    13822 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway_testing.py
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 11:24:36.000000 ssbtoolkit-1.0.5/ssbtoolkit/pathways/__init__.py
-drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-04-10 13:58:23.188085 ssbtoolkit-1.0.5/ssbtoolkit.egg-info/
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-04-10 13:58:23.000000 ssbtoolkit-1.0.5/ssbtoolkit.egg-info/PKG-INFO
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      742 2023-04-10 13:58:23.000000 ssbtoolkit-1.0.5/ssbtoolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        1 2023-04-10 13:58:23.000000 ssbtoolkit-1.0.5/ssbtoolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      143 2023-04-10 13:58:23.000000 ssbtoolkit-1.0.5/ssbtoolkit.egg-info/requires.txt
--rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       11 2023-04-10 13:58:23.000000 ssbtoolkit-1.0.5/ssbtoolkit.egg-info/top_level.txt
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-06-22 11:59:36.762245 ssbtoolkit-1.0.6/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       68 2023-06-22 11:46:24.000000 ssbtoolkit-1.0.6/MANIFEST.in
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-06-22 11:59:36.762245 ssbtoolkit-1.0.6/PKG-INFO
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       38 2023-06-22 11:59:36.762245 ssbtoolkit-1.0.6/setup.cfg
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1261 2023-06-22 11:59:20.000000 ssbtoolkit-1.0.6/setup.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-06-22 11:59:36.762245 ssbtoolkit-1.0.6/ssbtoolkit/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)   106496 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/HuTRdb.sqlite3
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    17110 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/Utils.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    71651 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/__init__.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-06-22 11:59:36.762245 ssbtoolkit-1.0.6/ssbtoolkit/pathways/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    20658 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gi.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1736 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gi_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2640 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gi_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    14154 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gq.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1153 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gq_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     1121 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gq_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    21135 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gs.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1763 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gs_parameters.csv
+-rw-r--r--   0 rribeiro  (1000) rribeiro  (1000)     2709 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gs_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    15771 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1725 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway_parameters.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)     1319 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway_reactions.csv
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)    13822 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway_testing.py
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        0 2023-06-22 11:46:11.000000 ssbtoolkit-1.0.6/ssbtoolkit/pathways/__init__.py
+drwxrwxr-x   0 rribeiro  (1000) rribeiro  (1000)        0 2023-06-22 11:59:36.762245 ssbtoolkit-1.0.6/ssbtoolkit.egg-info/
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      719 2023-06-22 11:59:36.000000 ssbtoolkit-1.0.6/ssbtoolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      768 2023-06-22 11:59:36.000000 ssbtoolkit-1.0.6/ssbtoolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)        1 2023-06-22 11:59:36.000000 ssbtoolkit-1.0.6/ssbtoolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)      143 2023-06-22 11:59:36.000000 ssbtoolkit-1.0.6/ssbtoolkit.egg-info/requires.txt
+-rw-rw-r--   0 rribeiro  (1000) rribeiro  (1000)       11 2023-06-22 11:59:36.000000 ssbtoolkit-1.0.6/ssbtoolkit.egg-info/top_level.txt
```

### Comparing `ssbtoolkit-1.0.5/PKG-INFO` & `ssbtoolkit-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssbtoolkit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simulation of methematical models of signaling pathways of GPCRs
 Author: Rui Ribeiro
 Author-email: <rui.ribeiro@univr.it>
 Keywords: python,bioinformatics,Systems Biology,GPCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssbtoolkit-1.0.5/setup.py` & `ssbtoolkit-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '1.0.5'
+VERSION = '1.0.6'
 DESCRIPTION = 'Simulation of methematical models of signaling pathways of GPCRs'
 LONG_DESCRIPTION = 'The SSB computational toolkit was developed to easily predict classical pharmacodynamic models of drug-GPCR (class A) interactions given just as input structural information of the receptor and the ligand.'
 
 # Setting up
 setup(
     name="ssbtoolkit",
     version=VERSION,
```

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/Utils.py` & `ssbtoolkit-1.0.6/ssbtoolkit/Utils.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/__init__.py` & `ssbtoolkit-1.0.6/ssbtoolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gi.py` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gi.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gi_parameters.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gi_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gi_reactions.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gi_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gq.py` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gq.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gq_parameters.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gq_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gq_reactions.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gq_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gs.py` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gs.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gs_parameters.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gs_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/Gs_reactions.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/Gs_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway.py` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway_parameters.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway_parameters.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway_reactions.csv` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway_reactions.csv`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit/pathways/OXTR_pathway_testing.py` & `ssbtoolkit-1.0.6/ssbtoolkit/pathways/OXTR_pathway_testing.py`

 * *Files identical despite different names*

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit.egg-info/PKG-INFO` & `ssbtoolkit-1.0.6/ssbtoolkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssbtoolkit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simulation of methematical models of signaling pathways of GPCRs
 Author: Rui Ribeiro
 Author-email: <rui.ribeiro@univr.it>
 Keywords: python,bioinformatics,Systems Biology,GPCR
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ssbtoolkit-1.0.5/ssbtoolkit.egg-info/SOURCES.txt` & `ssbtoolkit-1.0.6/ssbtoolkit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 setup.py
+ssbtoolkit/HuTRdb.sqlite3
 ssbtoolkit/Utils.py
 ssbtoolkit/__init__.py
 ssbtoolkit.egg-info/PKG-INFO
 ssbtoolkit.egg-info/SOURCES.txt
 ssbtoolkit.egg-info/dependency_links.txt
 ssbtoolkit.egg-info/requires.txt
 ssbtoolkit.egg-info/top_level.txt
```

