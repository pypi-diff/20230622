# Comparing `tmp/torch-adata-0.0.24rc1.tar.gz` & `tmp/torch-adata-0.0.24rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-adata-0.0.24rc1.tar", last modified: Thu Jun 22 19:38:04 2023, max compression
+gzip compressed data, was "torch-adata-0.0.24rc2.tar", last modified: Thu Jun 22 19:44:27 2023, max compression
```

## Comparing `torch-adata-0.0.24rc1.tar` & `torch-adata-0.0.24rc2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.883467 torch-adata-0.0.24rc1/torch_adata/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.883467 torch-adata-0.0.24rc1/torch_adata/_core/
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_AnnDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_data_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_identity_msg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_one_hot_encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_register_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/torch_adata/_core/_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_auto_parse_base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_configure_adata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_function_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_lightning_anndata_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_train_val_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/torch_adata/_demo/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_demo/_demo_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_demo/_larry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_demo/_pbmc_3k.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_demo/_plot_umap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/torch_adata/_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_tools/_anndataset_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_tools/_base_lightning_data_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_tools/_dummy_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_tools/_fetch_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_tools/_idx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_tools/_split.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.887467 torch-adata-0.0.24rc1/torch_adata/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_utils/_abc_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_utils/_function_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-22 19:37:53.000000 torch-adata-0.0.24rc1/torch_adata/_utils/_info_message.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:38:04.883467 torch-adata-0.0.24rc1/torch_adata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 19:38:04.000000 torch-adata-0.0.24rc1/torch_adata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-22 19:38:04.000000 torch-adata-0.0.24rc1/torch_adata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:38:04.000000 torch-adata-0.0.24rc1/torch_adata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-22 19:38:04.000000 torch-adata-0.0.24rc1/torch_adata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 19:38:04.000000 torch-adata-0.0.24rc1/torch_adata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.343970 torch-adata-0.0.24rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 19:44:27.343970 torch-adata-0.0.24rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:44:27.343970 torch-adata-0.0.24rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.331970 torch-adata-0.0.24rc2/torch_adata/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.331970 torch-adata-0.0.24rc2/torch_adata/_core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_AnnDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.335970 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_data_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_identity_msg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_one_hot_encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_register_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.339970 torch-adata-0.0.24rc2/torch_adata/_core/_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_auto_parse_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_configure_adata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_function_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_lightning_anndata_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_train_val_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.339970 torch-adata-0.0.24rc2/torch_adata/_demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_demo/_demo_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_demo/_larry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_demo/_pbmc_3k.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_demo/_plot_umap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.339970 torch-adata-0.0.24rc2/torch_adata/_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_tools/_anndataset_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_tools/_base_lightning_data_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_tools/_dummy_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_tools/_fetch_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_tools/_idx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_tools/_split.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.339970 torch-adata-0.0.24rc2/torch_adata/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_utils/_abc_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_utils/_function_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-22 19:44:14.000000 torch-adata-0.0.24rc2/torch_adata/_utils/_info_message.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:44:27.331970 torch-adata-0.0.24rc2/torch_adata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-22 19:44:27.000000 torch-adata-0.0.24rc2/torch_adata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-22 19:44:27.000000 torch-adata-0.0.24rc2/torch_adata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:44:27.000000 torch-adata-0.0.24rc2/torch_adata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 19:44:27.000000 torch-adata-0.0.24rc2/torch_adata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 19:44:27.000000 torch-adata-0.0.24rc2/torch_adata.egg-info/top_level.txt
```

### Comparing `torch-adata-0.0.24rc1/LICENSE` & `torch-adata-0.0.24rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/PKG-INFO` & `torch-adata-0.0.24rc2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-adata
-Version: 0.0.24rc1
+Version: 0.0.24rc2
 Summary: torch-adata
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
@@ -20,15 +20,15 @@
 [![Documentation Status](https://readthedocs.org/projects/torch-adata/badge/?version=latest)](https://torch-adata.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Create [`PyTorch Datasets`](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) from [`AnnData`](https://anndata.readthedocs.io/en/latest/)
 
 ## Installation
 
-Install from PYPI (current version: **[`0.0.23`](https://pypi.org/project/torch-adata/)**):
+Install from PYPI (current version: **[`0.0.24`](https://pypi.org/project/torch-adata/)**):
 ```BASH
 pip install torch-adata
 ```
 
 Install the developer version:
 ```BASH
 git clone https://github.com/mvinyard/torch-adata.git; cd torch-adata;
```

### Comparing `torch-adata-0.0.24rc1/README.md` & `torch-adata-0.0.24rc2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Documentation Status](https://readthedocs.org/projects/torch-adata/badge/?version=latest)](https://torch-adata.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Create [`PyTorch Datasets`](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) from [`AnnData`](https://anndata.readthedocs.io/en/latest/)
 
 ## Installation
 
-Install from PYPI (current version: **[`0.0.23`](https://pypi.org/project/torch-adata/)**):
+Install from PYPI (current version: **[`0.0.24`](https://pypi.org/project/torch-adata/)**):
 ```BASH
 pip install torch-adata
 ```
 
 Install the developer version:
 ```BASH
 git clone https://github.com/mvinyard/torch-adata.git; cd torch-adata;
```

### Comparing `torch-adata-0.0.24rc1/setup.py` & `torch-adata-0.0.24rc2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,32 +11,33 @@
 import os
 import sys
 
 
 # -- run setup: ----------------------------------------------------------------
 setuptools.setup(
     name="torch-adata",
-    version="0.0.24rc1",
+    version="0.0.24rc2",
     python_requires=">3.9.0",
     author="Michael E. Vinyard",
     author_email="mvinyard.ai@gmail.com",
     url=None,
     long_description=open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     description="torch-adata",
     packages=setuptools.find_packages(),
     install_requires=[
         "anndata>=0.9.1",
         "licorice_font>=0.0.3",
         "lightning>=2.0.1",
         "torch>=2.0",
-        "numpy==1.23",
+#         "numpy==1.23",
         "scanpy==1.9.3",
         "scikit-learn==1.2.2",
         "webfiles",
+	"vinplots",
     ],
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Programming Language :: Python :: 3.9",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
```

### Comparing `torch-adata-0.0.24rc1/torch_adata/__init__.py` & `torch-adata-0.0.24rc2/torch_adata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 __module_name__ = "__init__.py"
 __doc__ = """Main __init__ module."""
 __author__ = ", ".join(["Michael E. Vinyard"])
 __email__ = ", ".join(["vinyard@g.harvard.edu"])
 
 
 # -- specify package version: --------------------------------------------------
-__version__ = "0.0.24rc1"
+__version__ = "0.0.24rc2"
 
 
 # -- import modules: -----------------------------------------------------------
 from ._core._AnnDataset import AnnDataset
 from ._core._lightning._lightning_anndata_module import LightningAnnDataModule
 from . import _tools as tl
```

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_AnnDataset.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_AnnDataset.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/__init__.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_data_typing.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_data_typing.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_fetch_data.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_group_and_pad_adata.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_identity_msg.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_identity_msg.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_one_hot_encode.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_one_hot_encode.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_register_init.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_register_init.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_core_ancilliary/_return_data_on_axis.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_auto_parse_base_class.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_auto_parse_base_class.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_configure_adata.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_configure_adata.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_function_kwargs.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_function_kwargs.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_lightning_anndata_module.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_lightning_anndata_module.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_core/_lightning/_train_val_split.py` & `torch-adata-0.0.24rc2/torch_adata/_core/_lightning/_train_val_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_demo/_demo_data.py` & `torch-adata-0.0.24rc2/torch_adata/_demo/_demo_data.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_demo/_larry.py` & `torch-adata-0.0.24rc2/torch_adata/_demo/_larry.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_demo/_pbmc_3k.py` & `torch-adata-0.0.24rc2/torch_adata/_demo/_pbmc_3k.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_demo/_plot_umap.py` & `torch-adata-0.0.24rc2/torch_adata/_demo/_plot_umap.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_tools/__init__.py` & `torch-adata-0.0.24rc2/torch_adata/_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_tools/_anndataset_split.py` & `torch-adata-0.0.24rc2/torch_adata/_tools/_anndataset_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_tools/_base_lightning_data_module.py` & `torch-adata-0.0.24rc2/torch_adata/_tools/_base_lightning_data_module.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_tools/_dummy_batch.py` & `torch-adata-0.0.24rc2/torch_adata/_tools/_dummy_batch.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_tools/_fetch_data.py` & `torch-adata-0.0.24rc2/torch_adata/_tools/_fetch_data.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_tools/_idx.py` & `torch-adata-0.0.24rc2/torch_adata/_tools/_idx.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_tools/_split.py` & `torch-adata-0.0.24rc2/torch_adata/_tools/_split.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_utils/_abc_parse.py` & `torch-adata-0.0.24rc2/torch_adata/_utils/_abc_parse.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata/_utils/_function_inspector.py` & `torch-adata-0.0.24rc2/torch_adata/_utils/_function_inspector.py`

 * *Files identical despite different names*

### Comparing `torch-adata-0.0.24rc1/torch_adata.egg-info/PKG-INFO` & `torch-adata-0.0.24rc2/torch_adata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-adata
-Version: 0.0.24rc1
+Version: 0.0.24rc2
 Summary: torch-adata
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Intended Audience :: Science/Research
@@ -20,15 +20,15 @@
 [![Documentation Status](https://readthedocs.org/projects/torch-adata/badge/?version=latest)](https://torch-adata.readthedocs.io/en/latest/?badge=latest)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Create [`PyTorch Datasets`](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) from [`AnnData`](https://anndata.readthedocs.io/en/latest/)
 
 ## Installation
 
-Install from PYPI (current version: **[`0.0.23`](https://pypi.org/project/torch-adata/)**):
+Install from PYPI (current version: **[`0.0.24`](https://pypi.org/project/torch-adata/)**):
 ```BASH
 pip install torch-adata
 ```
 
 Install the developer version:
 ```BASH
 git clone https://github.com/mvinyard/torch-adata.git; cd torch-adata;
```

### Comparing `torch-adata-0.0.24rc1/torch_adata.egg-info/SOURCES.txt` & `torch-adata-0.0.24rc2/torch_adata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

