# Comparing `tmp/merlin-dataloader-23.5.0.tar.gz` & `tmp/merlin-dataloader-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-dataloader-23.5.0.tar", last modified: Wed May 31 14:39:22 2023, max compression
+gzip compressed data, was "merlin-dataloader-23.6.0.tar", last modified: Thu Jun 22 20:12:09 2023, max compression
```

## Comparing `merlin-dataloader-23.5.0.tar` & `merlin-dataloader-23.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.920793 merlin-dataloader-23.5.0/merlin/dataloader/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:22.920793 merlin-dataloader-23.5.0/merlin/dataloader/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    29285 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/loader_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/ops/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/ops/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/utils/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/utils/tf/tf_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/dataloader/utils/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/dataloader/utils/torch/torch_trainer_dist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/merlin/loader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 14:39:22.000000 merlin-dataloader-23.5.0/merlin_dataloader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:22.916793 merlin-dataloader-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/jax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/tensorflow.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/requirements/torch.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-31 14:39:22.920793 merlin-dataloader-23.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81931 2023-05-31 14:39:09.000000 merlin-dataloader-23.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.741646 merlin-dataloader-23.6.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/merlin/dataloader/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/merlin/dataloader/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29285 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/loader_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/merlin/dataloader/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/ops/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/ops/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.741646 merlin-dataloader-23.6.0/merlin/dataloader/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/merlin/dataloader/utils/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/utils/tf/tf_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/merlin/dataloader/utils/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/dataloader/utils/torch/torch_trainer_dist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/merlin/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/loader/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/loader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/merlin/loader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/merlin_dataloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-06-22 20:12:09.000000 merlin-dataloader-23.6.0/merlin_dataloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-22 20:12:09.000000 merlin-dataloader-23.6.0/merlin_dataloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:12:09.000000 merlin-dataloader-23.6.0/merlin_dataloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-22 20:12:09.000000 merlin-dataloader-23.6.0/merlin_dataloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 20:12:09.000000 merlin-dataloader-23.6.0/merlin_dataloader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/requirements/jax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/requirements/tensorflow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/requirements/torch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-22 20:12:09.745646 merlin-dataloader-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81931 2023-06-22 20:11:45.000000 merlin-dataloader-23.6.0/versioneer.py
```

### Comparing `merlin-dataloader-23.5.0/LICENSE` & `merlin-dataloader-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/PKG-INFO` & `merlin-dataloader-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-dataloader
-Version: 23.5.0
+Version: 23.6.0
 Summary: Merlin Dataloader
 Home-page: https://github.com/NVIDIA-Merlin/dataloader
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 License-File: LICENSE
 
 # [Merlin Dataloader](https://github.com/NVIDIA-Merlin/dataloader)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/merlin-dataloader)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-dataloader.svg)](https://pypi.python.org/pypi/merlin-dataloader/)
 ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/dataloader)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/dataloader/main/README.html)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/dataloader/stable/README.html)
 
 The merlin-dataloader lets you quickly train recommender models for TensorFlow, PyTorch and JAX. It eliminates the biggest bottleneck in training recommender models, by providing GPU optimized dataloaders that read data directly into the GPU, and then do a 0-copy transfer to TensorFlow and PyTorch using [dlpack](https://github.com/dmlc/dlpack).
 
 The benefits of the Merlin Dataloader include:
 
 - Over 10x speedup over native framework dataloaders
 - Handles larger than memory datasets
@@ -55,15 +55,15 @@
 
 To install from PyPi:
 
 ```
 pip install merlin-dataloader
 ```
 
-There are also [docker containers on NGC](https://nvidia-merlin.github.io/Merlin/main/containers.html) with the merlin-dataloader and dependencies included on them
+There are also [docker containers on NGC](https://nvidia-merlin.github.io/Merlin/stable/containers.html) with the merlin-dataloader and dependencies included on them
 
 ## Basic Usage
 
 ```python
 # Get a merlin dataset from a set of parquet files
 import merlin.io
 dataset = merlin.io.Dataset(PARQUET_FILE_PATHS, engine="parquet")
```

### Comparing `merlin-dataloader-23.5.0/README.md` & `merlin-dataloader-23.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # [Merlin Dataloader](https://github.com/NVIDIA-Merlin/dataloader)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/merlin-dataloader)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-dataloader.svg)](https://pypi.python.org/pypi/merlin-dataloader/)
 ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/dataloader)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/dataloader/main/README.html)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/dataloader/stable/README.html)
 
 The merlin-dataloader lets you quickly train recommender models for TensorFlow, PyTorch and JAX. It eliminates the biggest bottleneck in training recommender models, by providing GPU optimized dataloaders that read data directly into the GPU, and then do a 0-copy transfer to TensorFlow and PyTorch using [dlpack](https://github.com/dmlc/dlpack).
 
 The benefits of the Merlin Dataloader include:
 
 - Over 10x speedup over native framework dataloaders
 - Handles larger than memory datasets
@@ -26,15 +26,15 @@
 
 To install from PyPi:
 
 ```
 pip install merlin-dataloader
 ```
 
-There are also [docker containers on NGC](https://nvidia-merlin.github.io/Merlin/main/containers.html) with the merlin-dataloader and dependencies included on them
+There are also [docker containers on NGC](https://nvidia-merlin.github.io/Merlin/stable/containers.html) with the merlin-dataloader and dependencies included on them
 
 ## Basic Usage
 
 ```python
 # Get a merlin dataset from a set of parquet files
 import merlin.io
 dataset = merlin.io.Dataset(PARQUET_FILE_PATHS, engine="parquet")
```

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/__init__.py` & `merlin-dataloader-23.6.0/merlin/dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/jax.py` & `merlin-dataloader-23.6.0/merlin/dataloader/jax.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/loader_base.py` & `merlin-dataloader-23.6.0/merlin/dataloader/loader_base.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/ops/__init__.py` & `merlin-dataloader-23.6.0/merlin/dataloader/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/ops/embeddings.py` & `merlin-dataloader-23.6.0/merlin/dataloader/ops/embeddings.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/ops/padding.py` & `merlin-dataloader-23.6.0/merlin/dataloader/ops/padding.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/tensorflow.py` & `merlin-dataloader-23.6.0/merlin/dataloader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/tf_utils.py` & `merlin-dataloader-23.6.0/merlin/dataloader/tf_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/torch.py` & `merlin-dataloader-23.6.0/merlin/dataloader/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/utils/tf/tf_trainer.py` & `merlin-dataloader-23.6.0/merlin/dataloader/utils/tf/tf_trainer.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/dataloader/utils/torch/torch_trainer_dist.py` & `merlin-dataloader-23.6.0/merlin/dataloader/utils/torch/torch_trainer_dist.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/loader/__init__.py` & `merlin-dataloader-23.6.0/merlin/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/loader/jax.py` & `merlin-dataloader-23.6.0/merlin/loader/jax.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/loader/tensorflow.py` & `merlin-dataloader-23.6.0/merlin/loader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin/loader/torch.py` & `merlin-dataloader-23.6.0/merlin/loader/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin_dataloader.egg-info/PKG-INFO` & `merlin-dataloader-23.6.0/merlin_dataloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-dataloader
-Version: 23.5.0
+Version: 23.6.0
 Summary: Merlin Dataloader
 Home-page: https://github.com/NVIDIA-Merlin/dataloader
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 License-File: LICENSE
 
 # [Merlin Dataloader](https://github.com/NVIDIA-Merlin/dataloader)
 
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/merlin-dataloader)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-dataloader.svg)](https://pypi.python.org/pypi/merlin-dataloader/)
 ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/dataloader)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/dataloader/main/README.html)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/dataloader/stable/README.html)
 
 The merlin-dataloader lets you quickly train recommender models for TensorFlow, PyTorch and JAX. It eliminates the biggest bottleneck in training recommender models, by providing GPU optimized dataloaders that read data directly into the GPU, and then do a 0-copy transfer to TensorFlow and PyTorch using [dlpack](https://github.com/dmlc/dlpack).
 
 The benefits of the Merlin Dataloader include:
 
 - Over 10x speedup over native framework dataloaders
 - Handles larger than memory datasets
@@ -55,15 +55,15 @@
 
 To install from PyPi:
 
 ```
 pip install merlin-dataloader
 ```
 
-There are also [docker containers on NGC](https://nvidia-merlin.github.io/Merlin/main/containers.html) with the merlin-dataloader and dependencies included on them
+There are also [docker containers on NGC](https://nvidia-merlin.github.io/Merlin/stable/containers.html) with the merlin-dataloader and dependencies included on them
 
 ## Basic Usage
 
 ```python
 # Get a merlin dataset from a set of parquet files
 import merlin.io
 dataset = merlin.io.Dataset(PARQUET_FILE_PATHS, engine="parquet")
```

### Comparing `merlin-dataloader-23.5.0/merlin_dataloader.egg-info/SOURCES.txt` & `merlin-dataloader-23.6.0/merlin_dataloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/merlin_dataloader.egg-info/requires.txt` & `merlin-dataloader-23.6.0/merlin_dataloader.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-merlin-core>=23.04.00
+merlin-core<23.07,>=23.06
 
 [all]
-merlin-core>=23.04.00
+merlin-core<23.07,>=23.06
 tensorflow>=2.3.0
 torch>=1.0
 torch>=1.0
 jax[cpu]
 scipy
 scikit-learn>=0.20
 npy_append_array
@@ -26,15 +26,15 @@
 sphinx_rtd_theme
 natsort<8.2
 myst-nb<0.14
 linkify-it-py<1.1
 markdown==3.3.7
 
 [base]
-merlin-core>=23.04.00
+merlin-core<23.07,>=23.06
 
 [dev]
 scipy
 scikit-learn>=0.20
 npy_append_array
 ipython_genutils
 nbsphinx>=0.6
```

### Comparing `merlin-dataloader-23.5.0/pyproject.toml` & `merlin-dataloader-23.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/requirements/dev.txt` & `merlin-dataloader-23.6.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/setup.cfg` & `merlin-dataloader-23.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/setup.py` & `merlin-dataloader-23.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-dataloader-23.5.0/versioneer.py` & `merlin-dataloader-23.6.0/versioneer.py`

 * *Files identical despite different names*

