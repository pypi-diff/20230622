# Comparing `tmp/NORDic-2.4.2.tar.gz` & `tmp/NORDic-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NORDic-2.4.2.tar", last modified: Fri Apr 14 18:05:27 2023, max compression
+gzip compressed data, was "NORDic-2.4.3.tar", last modified: Thu Jun 22 21:17:27 2023, max compression
```

## Comparing `NORDic-2.4.2.tar` & `NORDic-2.4.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.306291 NORDic-2.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-14 18:05:27.306291 NORDic-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5550 2023-04-14 18:05:19.000000 NORDic-2.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-14 18:05:19.000000 NORDic-2.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:05:27.306291 NORDic-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-04-14 18:05:19.000000 NORDic-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.298291 NORDic-2.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.298291 NORDic-2.4.2/src/NORDic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic/NORDic_DR/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16854 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/bandits.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6023 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14603 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DR/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic/NORDic_DS/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13551 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic/NORDic_NI/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_NI/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8840 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_NI/cytoscape_style.py
--rw-r--r--   0 runner    (1001) docker     (123)    40173 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_NI/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.306291 NORDic-2.4.2/src/NORDic/NORDic_PMR/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_PMR/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/NORDic_PMR/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.306291 NORDic-2.4.2/src/NORDic/UTILS/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7097 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/DISGENET_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28342 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/LINCS_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17756 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/STRING_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9247 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14958 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_exp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33766 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_grn.py
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_sim.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7357 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/UTILS/utils_state.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:19.000000 NORDic-2.4.2/src/NORDic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:05:27.302291 NORDic-2.4.2/src/NORDic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 18:05:27.000000 NORDic-2.4.2/src/NORDic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.151082 NORDic-2.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-22 21:17:27.151082 NORDic-2.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-06-22 21:17:15.000000 NORDic-2.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-22 21:17:15.000000 NORDic-2.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:17:27.151082 NORDic-2.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-22 21:17:16.000000 NORDic-2.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.147082 NORDic-2.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.147082 NORDic-2.4.3/src/NORDic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.147082 NORDic-2.4.3/src/NORDic/NORDic_DR/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DR/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16854 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DR/bandits.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6023 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DR/functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14603 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DR/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.147082 NORDic-2.4.3/src/NORDic/NORDic_DS/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13551 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DS/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DS/get_drug_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_DS/get_drug_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.147082 NORDic-2.4.3/src/NORDic/NORDic_NI/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_NI/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8840 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_NI/cytoscape_style.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40190 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_NI/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.147082 NORDic-2.4.3/src/NORDic/NORDic_PMR/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_PMR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/NORDic_PMR/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.151082 NORDic-2.4.3/src/NORDic/UTILS/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7097 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/DISGENET_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28342 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/LINCS_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17756 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/STRING_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9247 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/utils_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14958 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/utils_exp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33766 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/utils_grn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/utils_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18155 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/utils_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/utils_sim.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7357 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/UTILS/utils_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:15.000000 NORDic-2.4.3/src/NORDic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:17:27.147082 NORDic-2.4.3/src/NORDic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-06-22 21:17:27.000000 NORDic-2.4.3/src/NORDic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-22 21:17:27.000000 NORDic-2.4.3/src/NORDic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:17:27.000000 NORDic-2.4.3/src/NORDic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 21:17:27.000000 NORDic-2.4.3/src/NORDic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 21:17:27.000000 NORDic-2.4.3/src/NORDic.egg-info/top_level.txt
```

### Comparing `NORDic-2.4.2/PKG-INFO` & `NORDic-2.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: NORDic
-Version: 2.4.2
+Version: 2.4.3
 Summary: Network Oriented Repurposing of Drugs (NORDic): network identification / master regulator detection / drug effect simulator / drug repurposing
 Home-page: https://github.com/clreda/NORDic
 Author: Clémence Réda
 Author-email: clemence.reda@inserm.fr
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 
 # Network Oriented Repurposing of Drugs (NORDic)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
+[![Anaconda version](https://anaconda.org/creda/nordic/badges/version.svg)](https://anaconda.org/creda/nordic) [![PyPI version](https://badge.fury.io/py/nordic.svg)](https://badge.fury.io/py/nordic) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
 
 ## Statement of need
 
 Being able to build in an automated and reproducible way a model of gene interactions and their influences on gene activity will allow to consider more complex diseases and biological phenomena, on a larger set of genes. These models might speed up the understanding of the gene regulation hierarchy by bioinformaticians and biologists, allow to predict novel drugs or gene targets which might be investigated later for healthcare purposes. In particular, the network-oriented approach allow to predict off-targets, which are non-specific drug targets which might lead to otherwise unexpected toxic side effects.
 
 [NORDic](https://github.com/clreda/NORDic) is an open-source package which allows to focus on a network-oriented approach to identify regulatory mechanisms linked to a disease, to detect master regulators in a diseased transcriptomic context, to simulate drug effects on a patient through a network, and adaptively test drugs to perform sample-efficient, error-bound drug repurposing. As such, it is comprised of four distinct submodules:
 - **NORDic NI** identifies a disease-associated gene regulatory network (as a *Boolean network*) with its dynamics combining several biological sources and methods. The main contribution is that this inference can be performed even in the absence of previously curated experiments and prior knowledge networks.
```

### Comparing `NORDic-2.4.2/README.md` & `NORDic-2.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Network Oriented Repurposing of Drugs (NORDic)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
+[![Anaconda version](https://anaconda.org/creda/nordic/badges/version.svg)](https://anaconda.org/creda/nordic) [![PyPI version](https://badge.fury.io/py/nordic.svg)](https://badge.fury.io/py/nordic) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
 
 ## Statement of need
 
 Being able to build in an automated and reproducible way a model of gene interactions and their influences on gene activity will allow to consider more complex diseases and biological phenomena, on a larger set of genes. These models might speed up the understanding of the gene regulation hierarchy by bioinformaticians and biologists, allow to predict novel drugs or gene targets which might be investigated later for healthcare purposes. In particular, the network-oriented approach allow to predict off-targets, which are non-specific drug targets which might lead to otherwise unexpected toxic side effects.
 
 [NORDic](https://github.com/clreda/NORDic) is an open-source package which allows to focus on a network-oriented approach to identify regulatory mechanisms linked to a disease, to detect master regulators in a diseased transcriptomic context, to simulate drug effects on a patient through a network, and adaptively test drugs to perform sample-efficient, error-bound drug repurposing. As such, it is comprised of four distinct submodules:
 - **NORDic NI** identifies a disease-associated gene regulatory network (as a *Boolean network*) with its dynamics combining several biological sources and methods. The main contribution is that this inference can be performed even in the absence of previously curated experiments and prior knowledge networks.
```

### Comparing `NORDic-2.4.2/setup.py` & `NORDic-2.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = "NORDic"
-VERSION = "2.4.2"
+VERSION = "2.4.3"
 
 setup(name=NAME,
     version=VERSION,
     author="Clémence Réda",
     author_email="clemence.reda@inserm.fr",
     url="https://github.com/clreda/NORDic",
     license_files = ('LICENSE'),
```

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_DR/bandits.py` & `NORDic-2.4.3/src/NORDic/NORDic_DR/bandits.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_DR/functions.py` & `NORDic-2.4.3/src/NORDic/NORDic_DR/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_DR/utils.py` & `NORDic-2.4.3/src/NORDic/NORDic_DR/utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_DS/functions.py` & `NORDic-2.4.3/src/NORDic/NORDic_DS/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_signatures.py` & `NORDic-2.4.3/src/NORDic/NORDic_DS/get_drug_signatures.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,26 +139,26 @@
     if (sigs is None):
         return None
     assert sigs.shape[1] == nsamples
     sig = binarize_via_CD(sigs, samples=[2]*len(data_treated)+[1]*len(data_control), binarize=int(binarize), nperm=10000)
     sig.columns = [pubchem_cid]
     return sig
 
-def compute_drug_signatures_L1000(pubchem_cids, lincs_args, binarize=True, chunksize=10):
+def compute_drug_signatures_L1000(pubchem_cids, lincs_args, binarize=True, gene_list=None, chunksize=10):
     '''
         Get drug signatures from LINCS L1000
         @param\tpubchem_cids\tPython integer list: list of drug PubChem CIDs
         @param\tlincs_args\tPython dictionary: additional arguments for LINCS L1000 requests
         @param\tbinarize\tPython bool[default=True]: should the resulting signatures be binarized?
         @return\tsigs\tPandas DataFrame: rows/[genes] x columns/[drug names]
     '''
     assert lincs_args and "credentials" in lincs_args and "path_to_lincs" in lincs_args
     user_key = get_user_key(lincs_args["credentials"])
     path_to_lincs = lincs_args["path_to_lincs"]
     pert_inames = pubchem2drugname(pubchem_cids, lincs_args)
     gene_files, _, _, _ = download_lincs_files(path_to_lincs, which_lvl=[3])
     gene_df = pd.read_csv(path_to_lincs+gene_files[0], sep="\t", engine='python', index_col=0)
-    gene_list, gene_name_list = list(gene_df.index), list(gene_df["pr_gene_symbol"])
+    gene_list, gene_name_list = list(gene_df.index) if (gene_list is None) else gene_list, list(gene_df["pr_gene_symbol"])
     sigs_list = [retrieve_drug_signature(pubchem_cid, get_all_celllines([pert_inames[pubchem_cid]], user_key) if (len(lincs_args.get("cell_lines", []))==0) else lincs_args["cell_lines"], gene_list, lincs_args, binarize) for pubchem_cid in pubchem_cids]
     sigs = sigs_list[0].join(sigs_list[1:], how="outer")
     sigs.index = [gene_df.loc[i]["pr_gene_symbol"] for i in sigs.index]
     return sigs
```

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_DS/get_drug_targets.py` & `NORDic-2.4.3/src/NORDic/NORDic_DS/get_drug_targets.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_NI/cytoscape_style.py` & `NORDic-2.4.3/src/NORDic/NORDic_NI/cytoscape_style.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_NI/functions.py` & `NORDic-2.4.3/src/NORDic/NORDic_NI/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,15 +306,15 @@
             if (profiles is None):
                 profiles = pd.DataFrame([], index=pert_inames, columns=["0","1"]).astype(str)
                 for a in add_rows_profiles:
                     profiles.loc[a] = ["nan"]*profiles.shape[1]
 
         else:
 
-            profiles = pd.read_csv(experiments_fname, sep=",", index_col=0)
+            profiles = pd.read_csv(experiments_fname, sep=",", index_col=0, na_filter=False)
             ## Pandas DataFrame with index=HUGO gene symbols, columns=sample names, and 5 additional rows
             ## 'annotation' 2 if the sample is treated, 1 otherwise
             ## 'perturbed' gene which is perturbed
             ## 'perturbation' experiment UNIQUE identifier, common to samples from the same experiment
             ## 'cell_line' experiment UNIQUE identifier, common to samples from the same experiment
             ## 'sigid' sample unique identifier from LINCS L1000 (can be filled with NaNs)
             ## /!\ SHOULD ALREADY BE BINARIZED
```

### Comparing `NORDic-2.4.2/src/NORDic/NORDic_PMR/functions.py` & `NORDic-2.4.3/src/NORDic/NORDic_PMR/functions.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/DISGENET_utils.py` & `NORDic-2.4.3/src/NORDic/UTILS/DISGENET_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/LINCS_utils.py` & `NORDic-2.4.3/src/NORDic/UTILS/LINCS_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/STRING_utils.py` & `NORDic-2.4.3/src/NORDic/UTILS/STRING_utils.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/utils_data.py` & `NORDic-2.4.3/src/NORDic/UTILS/utils_data.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/utils_exp.py` & `NORDic-2.4.3/src/NORDic/UTILS/utils_exp.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/utils_grn.py` & `NORDic-2.4.3/src/NORDic/UTILS/utils_grn.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/utils_network.py` & `NORDic-2.4.3/src/NORDic/UTILS/utils_network.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/utils_plot.py` & `NORDic-2.4.3/src/NORDic/UTILS/utils_plot.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/utils_sim.py` & `NORDic-2.4.3/src/NORDic/UTILS/utils_sim.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic/UTILS/utils_state.py` & `NORDic-2.4.3/src/NORDic/UTILS/utils_state.py`

 * *Files identical despite different names*

### Comparing `NORDic-2.4.2/src/NORDic.egg-info/PKG-INFO` & `NORDic-2.4.3/src/NORDic.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: NORDic
-Version: 2.4.2
+Version: 2.4.3
 Summary: Network Oriented Repurposing of Drugs (NORDic): network identification / master regulator detection / drug effect simulator / drug repurposing
 Home-page: https://github.com/clreda/NORDic
 Author: Clémence Réda
 Author-email: clemence.reda@inserm.fr
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 
 # Network Oriented Repurposing of Drugs (NORDic)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
+[![Anaconda version](https://anaconda.org/creda/nordic/badges/version.svg)](https://anaconda.org/creda/nordic) [![PyPI version](https://badge.fury.io/py/nordic.svg)](https://badge.fury.io/py/nordic) [![Zenodo version](https://zenodo.org/badge/DOI/10.5281/zenodo.7239047.svg)](https://doi.org/10.5281/zenodo.7239047)
 
 ## Statement of need
 
 Being able to build in an automated and reproducible way a model of gene interactions and their influences on gene activity will allow to consider more complex diseases and biological phenomena, on a larger set of genes. These models might speed up the understanding of the gene regulation hierarchy by bioinformaticians and biologists, allow to predict novel drugs or gene targets which might be investigated later for healthcare purposes. In particular, the network-oriented approach allow to predict off-targets, which are non-specific drug targets which might lead to otherwise unexpected toxic side effects.
 
 [NORDic](https://github.com/clreda/NORDic) is an open-source package which allows to focus on a network-oriented approach to identify regulatory mechanisms linked to a disease, to detect master regulators in a diseased transcriptomic context, to simulate drug effects on a patient through a network, and adaptively test drugs to perform sample-efficient, error-bound drug repurposing. As such, it is comprised of four distinct submodules:
 - **NORDic NI** identifies a disease-associated gene regulatory network (as a *Boolean network*) with its dynamics combining several biological sources and methods. The main contribution is that this inference can be performed even in the absence of previously curated experiments and prior knowledge networks.
```

### Comparing `NORDic-2.4.2/src/NORDic.egg-info/SOURCES.txt` & `NORDic-2.4.3/src/NORDic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

