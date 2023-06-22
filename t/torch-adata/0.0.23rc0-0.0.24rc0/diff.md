# Comparing `tmp/torch-adata-0.0.23rc0.tar.gz` & `tmp/torch-adata-0.0.24rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-adata-0.0.23rc0.tar", last modified: Tue May  9 21:01:54 2023, max compression
+gzip compressed data, was "torch-adata-0.0.24rc0.tar", last modified: Thu Jun 22 19:31:31 2023, max compression
```

## Comparing `torch-adata-0.0.23rc0.tar` & `torch-adata-0.0.24rc0.tar`

### file list

```diff
@@ -1,41 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:01:54.434651 torch-adata-0.0.23rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-09 21:01:54.434651 torch-adata-0.0.23rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 21:01:54.434651 torch-adata-0.0.23rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:01:54.430651 torch-adata-0.0.23rc0/torch_adata/
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:01:54.430651 torch-adata-0.0.23rc0/torch_adata/_core/
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_AnnDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:01:54.430651 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_data_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_identity_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_register_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:01:54.434651 torch-adata-0.0.23rc0/torch_adata/_core/_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_auto_parse_base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_configure_adata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_function_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_lightning_anndata_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_train_val_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:01:54.434651 torch-adata-0.0.23rc0/torch_adata/_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_tools/_anndataset_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_tools/_base_lightning_data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_tools/_dummy_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_tools/_fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_tools/_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-09 21:01:44.000000 torch-adata-0.0.23rc0/torch_adata/_tools/_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 21:01:54.430651 torch-adata-0.0.23rc0/torch_adata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-09 21:01:54.000000 torch-adata-0.0.23rc0/torch_adata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-09 21:01:54.000000 torch-adata-0.0.23rc0/torch_adata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 21:01:54.000000 torch-adata-0.0.23rc0/torch_adata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 21:01:54.000000 torch-adata-0.0.23rc0/torch_adata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 21:01:54.000000 torch-adata-0.0.23rc0/torch_adata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.339708 torch-adata-0.0.24rc0/torch_adata/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.339708 torch-adata-0.0.24rc0/torch_adata/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_AnnDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_data_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_identity_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_register_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/torch_adata/_core/_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_auto_parse_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_configure_adata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_function_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_lightning_anndata_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_train_val_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/torch_adata/_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_demo/_demo_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_demo/_larry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_demo/_pbmc_3k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_demo/_plot_umap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/torch_adata/_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_tools/_anndataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_tools/_base_lightning_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_tools/_dummy_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_tools/_fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_tools/_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_tools/_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.343708 torch-adata-0.0.24rc0/torch_adata/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_utils/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_utils/_function_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-22 19:31:20.000000 torch-adata-0.0.24rc0/torch_adata/_utils/_info_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:31:31.339708 torch-adata-0.0.24rc0/torch_adata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 19:31:31.000000 torch-adata-0.0.24rc0/torch_adata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-22 19:31:31.000000 torch-adata-0.0.24rc0/torch_adata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:31:31.000000 torch-adata-0.0.24rc0/torch_adata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-22 19:31:31.000000 torch-adata-0.0.24rc0/torch_adata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 19:31:31.000000 torch-adata-0.0.24rc0/torch_adata.egg-info/top_level.txt
```

### Comparing `torch-adata-0.0.23rc0/LICENSE` & `torch-adata-0.0.24rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/PKG-INFO` & `torch-adata-0.0.24rc0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: torch-adata
-Version: 0.0.23rc0
+Version: 0.0.24rc0
 Summary: torch-adata
 Author: Michael E. Vinyard
-Author-email: mvinyard@g.harvard.edu
+Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![torch-adata-logo](/docs/imgs/torch-adata.logo.github.png)
```

### Comparing `torch-adata-0.0.23rc0/README.md` & `torch-adata-0.0.24rc0/README.md`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/__init__.py` & `torch-adata-0.0.24rc0/torch_adata/_tools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 
 __module_name__ = "__init__.py"
-__doc__ = """Main __init__ module."""
+__doc__ = """functions __init__ module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
 
 
 # -- specify package version: --------------------------------------------------
-__version__ = "0.0.23rc0"
+__version__ = "0.0.20"
 
 
-# -- import modules: -----------------------------------------------------------
-from ._core._AnnDataset import AnnDataset
-from ._core._lightning._lightning_anndata_module import LightningAnnDataModule
-from . import _tools as tl
-
-
-# -- import API-hidden core modules (for dev): ---------------------------------
-from ._core import _core_ancilliary as _core
+# -- import ancilliary functions: ----------------------------------------------
+from ._split import split
+from ._idx import idx
+from ._dummy_batch import dummy_batch
+from ._base_lightning_data_module import BaseLightningDataModule
+from ._anndataset_split import AnnDatasetSplit
+from ._fetch_data import fetch
```

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_AnnDataset.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_AnnDataset.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/__init__.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_data_typing.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_data_typing.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_fetch_data.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_identity_msg.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_identity_msg.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_one_hot_encode.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_register_init.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_register_init.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_auto_parse_base_class.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_auto_parse_base_class.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_configure_adata.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_configure_adata.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_function_kwargs.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_lightning_anndata_module.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_lightning_anndata_module.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_core/_lightning/_train_val_split.py` & `torch-adata-0.0.24rc0/torch_adata/_core/_lightning/_train_val_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_tools/_anndataset_split.py` & `torch-adata-0.0.24rc0/torch_adata/_tools/_anndataset_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_tools/_base_lightning_data_module.py` & `torch-adata-0.0.24rc0/torch_adata/_tools/_base_lightning_data_module.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_tools/_dummy_batch.py` & `torch-adata-0.0.24rc0/torch_adata/_tools/_dummy_batch.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_tools/_fetch_data.py` & `torch-adata-0.0.24rc0/torch_adata/_tools/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_tools/_idx.py` & `torch-adata-0.0.24rc0/torch_adata/_tools/_idx.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.23rc0/torch_adata/_tools/_split.py` & `torch-adata-0.0.24rc0/torch_adata/_tools/_split.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,42 @@
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
 
 
 # -- import packages: ----------------------------------------------------------
 import numpy as np
 import torch
 
+# -- set typing: ---------------------------------------------------------------
+from typing import Union, List
+
 
 # -- supporting functions: -----------------------------------------------------
-"""Split dataset length with even proportions according to number of groups"""
+def _sum_norm(vals: Union[List, np.ndarray]) -> np.ndarray:
+    return np.array(vals) / vals.sum()
+
+
 def uniform_group_sizes(n_cells: int, n_groups: int = 2):
-    """Split groups based on number of cells and groups."""
+    """
+    Split dataset length with even proportions according to number of
+    groups and cells.
+    """
     div, mod = divmod(n_cells, n_groups)
     return [div] * (n_groups - 1) + [div + mod]
 
 
 def proportioned_group_sizes(
     dataset: torch.utils.data.Dataset,
     percentages: list([float, "...", float]),
     remainder_idx: int = -1,
 ) -> list([int, "...", int]):
     """Split dataset length with specified proportions/number of groups"""
     
     n_cells = len(dataset)
     n_groups = len(percentages)
-    percentages = sum_norm(np.array(percentages))
+    percentages = _sum_norm(np.array(percentages))
 
     split_lengths = [int(n_cells * pct_i) for pct_i in percentages]
     remainder = n_cells - sum(split_lengths)
     split_lengths[remainder_idx] += remainder
 
     return split_lengths
 
@@ -40,15 +49,16 @@
     dataset: torch.utils.data.Dataset,
     n_groups: int = 2,
     percentages: list([float, "...", float]) = None,
 ) -> list([int, "...", int]):
     """Split the length of the dataset into proportioned subsets"""
     if percentages:
         return proportioned_group_sizes(dataset, percentages, remainder_idx=-1)
-    return uniform_group_sizes(dataset, n_groups)
+    n_cells = dataset.X.shape[0]
+    return uniform_group_sizes(n_cells, n_groups)
 
 
 # -- main module function: ---------------------------------------------------------------
 def split(
     dataset: torch.utils.data.Dataset,
     n_groups: int = 2,
     percentages: list([float, "...", float]) = None,
```

### Comparing `torch-adata-0.0.23rc0/torch_adata.egg-info/PKG-INFO` & `torch-adata-0.0.24rc0/torch_adata.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: torch-adata
-Version: 0.0.23rc0
+Version: 0.0.24rc0
 Summary: torch-adata
 Author: Michael E. Vinyard
-Author-email: mvinyard@g.harvard.edu
+Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ![torch-adata-logo](/docs/imgs/torch-adata.logo.github.png)
```

### Comparing `torch-adata-0.0.23rc0/torch_adata.egg-info/SOURCES.txt` & `torch-adata-0.0.24rc0/torch_adata.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 torch_adata/_core/_core_ancilliary/_return_data_on_axis.py
 torch_adata/_core/_lightning/__init__.py
 torch_adata/_core/_lightning/_auto_parse_base_class.py
 torch_adata/_core/_lightning/_configure_adata.py
 torch_adata/_core/_lightning/_function_kwargs.py
 torch_adata/_core/_lightning/_lightning_anndata_module.py
 torch_adata/_core/_lightning/_train_val_split.py
+torch_adata/_demo/__init__.py
+torch_adata/_demo/_demo_data.py
+torch_adata/_demo/_larry.py
+torch_adata/_demo/_pbmc_3k.py
+torch_adata/_demo/_plot_umap.py
 torch_adata/_tools/__init__.py
 torch_adata/_tools/_anndataset_split.py
 torch_adata/_tools/_base_lightning_data_module.py
 torch_adata/_tools/_dummy_batch.py
 torch_adata/_tools/_fetch_data.py
 torch_adata/_tools/_idx.py
-torch_adata/_tools/_split.py
+torch_adata/_tools/_split.py
+torch_adata/_utils/__init__.py
+torch_adata/_utils/_abc_parse.py
+torch_adata/_utils/_function_inspector.py
+torch_adata/_utils/_info_message.py
```

