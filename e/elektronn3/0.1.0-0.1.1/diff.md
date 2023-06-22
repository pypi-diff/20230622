# Comparing `tmp/elektronn3-0.1.0.tar.gz` & `tmp/elektronn3-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elektronn3-0.1.0.tar", last modified: Mon May  1 22:44:13 2023, max compression
+gzip compressed data, was "elektronn3-0.1.1.tar", last modified: Thu Jun 22 19:54:39 2023, max compression
```

## Comparing `elektronn3-0.1.0.tar` & `elektronn3-0.1.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.611394 elektronn3-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 22:43:58.000000 elektronn3-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-01 22:43:58.000000 elektronn3-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-01 22:44:13.611394 elektronn3-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-05-01 22:43:58.000000 elektronn3-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.611394 elektronn3-0.1.0/elektronn3/
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-01 22:44:13.611394 elektronn3-0.1.0/elektronn3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.603394 elektronn3-0.1.0/elektronn3/data/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35208 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/cnndata.py
--rw-r--r--   0 runner    (1001) docker     (123)    25591 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/coord_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/knossos.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/knossos_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/sources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.607394 elektronn3-0.1.0/elektronn3/data/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/transforms/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/transforms/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/transforms/random_blurring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/transforms/region_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    46776 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/transforms/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.607394 elektronn3-0.1.0/elektronn3/inference/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34465 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/inference/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.607394 elektronn3-0.1.0/elektronn3/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/_model_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/fcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/fcn_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/msdnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    42420 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/resunet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/tiramisu_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/unet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/unet3d_lite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/models/vnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.607394 elektronn3-0.1.0/elektronn3/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/axial_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/evonorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/l1batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33126 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/lovasz_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/modules/wsconv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.611394 elektronn3-0.1.0/elektronn3/training/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/_trainer_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/noise2void.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/padam.py
--rw-r--r--   0 runner    (1001) docker     (123)    12725 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/recalibration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/swa.py
--rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/train_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/trainer_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/trainer_gnn_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/trainer_gnn_minibatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-05-01 22:43:58.000000 elektronn3-0.1.0/elektronn3/training/triplettrainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:44:13.603394 elektronn3-0.1.0/elektronn3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-05-01 22:44:13.000000 elektronn3-0.1.0/elektronn3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-01 22:44:13.000000 elektronn3-0.1.0/elektronn3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:44:13.000000 elektronn3-0.1.0/elektronn3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-01 22:44:13.000000 elektronn3-0.1.0/elektronn3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-01 22:44:13.000000 elektronn3-0.1.0/elektronn3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-01 22:44:13.611394 elektronn3-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-01 22:43:58.000000 elektronn3-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-01 22:43:58.000000 elektronn3-0.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.916563 elektronn3-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-22 19:54:30.000000 elektronn3-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 19:54:30.000000 elektronn3-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-22 19:54:39.916563 elektronn3-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-22 19:54:30.000000 elektronn3-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.916563 elektronn3-0.1.1/elektronn3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-22 19:54:39.916563 elektronn3-0.1.1/elektronn3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.912563 elektronn3-0.1.1/elektronn3/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35208 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/cnndata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25601 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/coord_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/knossos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/knossos_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4561 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/sources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.912563 elektronn3-0.1.1/elektronn3/data/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/transforms/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/transforms/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13878 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/transforms/random_blurring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/transforms/region_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46776 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/transforms/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11108 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.912563 elektronn3-0.1.1/elektronn3/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34467 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/inference/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.916563 elektronn3-0.1.1/elektronn3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/_model_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13656 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/fcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/fcn_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/msdnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42420 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/resunet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7484 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/tiramisu_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/unet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/unet3d_lite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/models/vnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.916563 elektronn3-0.1.1/elektronn3/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11109 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/axial_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/evonorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/l1batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33126 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/lovasz_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26743 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/modules/wsconv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.916563 elektronn3-0.1.1/elektronn3/training/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/_trainer_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19004 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14101 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/noise2void.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/padam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12727 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/recalibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13921 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/swa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/train_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51256 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/trainer_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15164 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/trainer_gnn_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/trainer_gnn_minibatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-06-22 19:54:30.000000 elektronn3-0.1.1/elektronn3/training/triplettrainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:54:39.908563 elektronn3-0.1.1/elektronn3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-22 19:54:39.000000 elektronn3-0.1.1/elektronn3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-22 19:54:39.000000 elektronn3-0.1.1/elektronn3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:54:39.000000 elektronn3-0.1.1/elektronn3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 19:54:39.000000 elektronn3-0.1.1/elektronn3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 19:54:39.000000 elektronn3-0.1.1/elektronn3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-22 19:54:39.916563 elektronn3-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-22 19:54:30.000000 elektronn3-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-22 19:54:30.000000 elektronn3-0.1.1/versioneer.py
```

### Comparing `elektronn3-0.1.0/LICENSE` & `elektronn3-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/PKG-INFO` & `elektronn3-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: elektronn3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utilities for 3D CNNs in PyTorch
 Home-page: https://github.com/ELEKTRONN/elektronn3
 Author: ELEKTRONN team
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Read the Docs](https://readthedocs.org/projects/elektronn3/badge/?version=latest)](https://elektronn3.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/elektronn3)](https://pypi.org/project/elektronn3/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ELEKTRONN/elektronn3/python-publish.yml)](https://github.com/ELEKTRONN/elektronn3/actions) [![Read the Docs](https://readthedocs.org/projects/elektronn3/badge/?version=latest)](https://elektronn3.readthedocs.io/en/latest/)
 
 # elektronn3
 
 A PyTorch-based library for working with 3D and 2D convolutional neural networks, with focus on semantic segmentation of volumetric biomedical image data.
 
 Quick overview of **elektronn3**'s code structure:
```

### Comparing `elektronn3-0.1.0/README.md` & `elektronn3-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Read the Docs](https://readthedocs.org/projects/elektronn3/badge/?version=latest)](https://elektronn3.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/elektronn3)](https://pypi.org/project/elektronn3/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ELEKTRONN/elektronn3/python-publish.yml)](https://github.com/ELEKTRONN/elektronn3/actions) [![Read the Docs](https://readthedocs.org/projects/elektronn3/badge/?version=latest)](https://elektronn3.readthedocs.io/en/latest/)
 
 # elektronn3
 
 A PyTorch-based library for working with 3D and 2D convolutional neural networks, with focus on semantic segmentation of volumetric biomedical image data.
 
 Quick overview of **elektronn3**'s code structure:
```

### Comparing `elektronn3-0.1.0/elektronn3/__init__.py` & `elektronn3-0.1.1/elektronn3/__init__.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/cnndata.py` & `elektronn3-0.1.1/elektronn3/data/cnndata.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/coord_transforms.py` & `elektronn3-0.1.1/elektronn3/data/coord_transforms.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,15 +257,15 @@
 
 @lru_cache()
 def make_dest_coords(sh):
     """
     Make coordinate list for destination array of shape sh
     """
     zz,xx,yy = np.mgrid[0:sh[0], 0:sh[1], 0:sh[2]]
-    hh = np.ones(sh, dtype=np.int)
+    hh = np.ones(sh, dtype=np.int64)
     coords = np.concatenate([zz[...,None], xx[...,None],
                              yy[...,None], hh[...,None]], axis=-1)
     return coords.astype(floatX)
 
 
 @lru_cache()
 def make_dest_corners(sh):
@@ -378,16 +378,16 @@
     dest_corners = make_dest_corners(patch_shape)
     src_corners = np.dot(M_inv, dest_corners.T).T
     if np.any(M[3,:3] != 0): # homogeneous divide
         src_corners /= src_corners[:,3][:,None]
 
     # check corners
     src_corners = src_corners[:,:3]
-    lo = np.min(np.floor(src_corners), 0).astype(np.int)
-    hi = np.max(np.ceil(src_corners + 1), 0).astype(np.int)
+    lo = np.min(np.floor(src_corners), 0).astype(np.int64)
+    hi = np.max(np.ceil(src_corners + 1), 0).astype(np.int64)
     # compute/transform dense coords
     dest_coords = make_dest_coords(patch_shape)
     src_coords = np.tensordot(dest_coords, M_inv, axes=[[-1], [1]])
     if np.any(M[3, :3] != 0):  # homogeneous divide
         src_coords /= src_coords[..., 3][..., None]
     # cut patch
     src_coords = src_coords[..., :3]
@@ -434,16 +434,16 @@
 
         src_coords_target = src_coords[
             target_offset[0]:(target_offset[0] + target_patch_shape[0]),
             target_offset[1]:(target_offset[1] + target_patch_shape[1]),
             target_offset[2]:(target_offset[2] + target_patch_shape[2])
         ]
         # shift coords to be w.r.t. to origin of target_src array
-        lo_targ = np.floor(src_coords_target.min(2).min(1).min(0) - target_src_offset).astype(np.int)
-        hi_targ = np.ceil(src_coords_target.max(2).max(1).max(0) + 1 - target_src_offset).astype(np.int)
+        lo_targ = np.floor(src_coords_target.min(2).min(1).min(0) - target_src_offset).astype(np.int64)
+        hi_targ = np.ceil(src_coords_target.max(2).max(1).max(0) + 1 - target_src_offset).astype(np.int64)
         if np.any(lo_targ < 0) or np.any(hi_targ >= target_src_shape - 1):
             raise WarpingOOBError("Out of bounds for target_src")
 
     if np.any(lo < 0) or np.any(hi >= inp_src_shape - 1):
         raise WarpingOOBError("Out of bounds for inp_src")
 
     # Slice and interpolate input
```

### Comparing `elektronn3-0.1.0/elektronn3/data/knossos.py` & `elektronn3-0.1.1/elektronn3/data/knossos.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/knossos_labels.py` & `elektronn3-0.1.1/elektronn3/data/knossos_labels.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/sources.py` & `elektronn3-0.1.1/elektronn3/data/sources.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/transforms/random.py` & `elektronn3-0.1.1/elektronn3/data/transforms/random.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/transforms/random_blurring.py` & `elektronn3-0.1.1/elektronn3/data/transforms/random_blurring.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/transforms/region_generator.py` & `elektronn3-0.1.1/elektronn3/data/transforms/region_generator.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/transforms/transforms.py` & `elektronn3-0.1.1/elektronn3/data/transforms/transforms.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/data/utils.py` & `elektronn3-0.1.1/elektronn3/data/utils.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/inference/__init__.py` & `elektronn3-0.1.1/elektronn3/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/inference/inference.py` & `elektronn3-0.1.1/elektronn3/inference/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -649,15 +649,15 @@
                     'Make sure that out_shape is divisible by tile_shape or '
                     'relax this constraint by setting strict_shapes=False.'
                 )
             else:
                 padded_out_shape = np.array(self.out_shape)
                 padded_out_shape[1:] = np.ceil(self.out_shape[1:] / self.tile_shape) * self.tile_shape
                 if self.offset is None:
-                    offset = np.zeros(shape=len(padded_out_shape) - 1, dtype=np.int)
+                    offset = np.zeros(shape=len(padded_out_shape) - 1, dtype=np.int64)
                 else:
                     offset = np.array(self.offset)
                 padded_inp_shape = (*inp.shape[:2], *padded_out_shape[1:] + 2 * offset)
                 padded_inp = np.zeros(padded_inp_shape)
                 # Define the relevant region (that is: without the padding that was just added)
                 relevant_slice_inp = _extend_nc([slice(0, d) for d in inp.shape[2:]])
                 relevant_slice_out = _extend_nc([slice(0, d) for d in self.out_shape[1:]])
```

### Comparing `elektronn3-0.1.0/elektronn3/logger.py` & `elektronn3-0.1.1/elektronn3/logger.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/_model_utils.py` & `elektronn3-0.1.1/elektronn3/models/_model_utils.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/base.py` & `elektronn3-0.1.1/elektronn3/models/base.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/fcn.py` & `elektronn3-0.1.1/elektronn3/models/fcn.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/fcn_2d.py` & `elektronn3-0.1.1/elektronn3/models/fcn_2d.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/msdnet.py` & `elektronn3-0.1.1/elektronn3/models/msdnet.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/resunet.py` & `elektronn3-0.1.1/elektronn3/models/resunet.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/simple.py` & `elektronn3-0.1.1/elektronn3/models/simple.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/tiramisu_2d.py` & `elektronn3-0.1.1/elektronn3/models/tiramisu_2d.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/unet.py` & `elektronn3-0.1.1/elektronn3/models/unet.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/unet3d_lite.py` & `elektronn3-0.1.1/elektronn3/models/unet3d_lite.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/models/vnet.py` & `elektronn3-0.1.1/elektronn3/models/vnet.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/modules/axial_attention.py` & `elektronn3-0.1.1/elektronn3/modules/axial_attention.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/modules/evonorm.py` & `elektronn3-0.1.1/elektronn3/modules/evonorm.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/modules/l1batchnorm.py` & `elektronn3-0.1.1/elektronn3/modules/l1batchnorm.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/modules/layers.py` & `elektronn3-0.1.1/elektronn3/modules/layers.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/modules/loss.py` & `elektronn3-0.1.1/elektronn3/modules/loss.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/modules/lovasz_losses.py` & `elektronn3-0.1.1/elektronn3/modules/lovasz_losses.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/modules/wsconv.py` & `elektronn3-0.1.1/elektronn3/modules/wsconv.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/_trainer_multi.py` & `elektronn3-0.1.1/elektronn3/training/_trainer_multi.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/handlers.py` & `elektronn3-0.1.1/elektronn3/training/handlers.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/metrics.py` & `elektronn3-0.1.1/elektronn3/training/metrics.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/noise2void.py` & `elektronn3-0.1.1/elektronn3/training/noise2void.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/padam.py` & `elektronn3-0.1.1/elektronn3/training/padam.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/plotting.py` & `elektronn3-0.1.1/elektronn3/training/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
 
 def add_timeticks(ax, times, steps, time_str='mins', num=5):
     N = int(times[-1])
     k = max(N / num, 1)
     k = int(np.log10(k))  # 10-base of locators
     m = int(np.round(float(N) / (num * 10 ** k)))  # multiple of base
     s = max(m * 10 ** k, 1)
-    x_labs = np.arange(0, N, s, dtype=np.int)
+    x_labs = np.arange(0, N, s, dtype=np.int64)
     x_ticks = np.interp(x_labs, times, steps)
     ax.set_xticks(x_ticks)
     ax.set_xticklabels(x_labs)
     ax.set_xlim(0, steps[-1])
     ax.set_xlabel('Runtime [%s]' % time_str)  # (%s)'%("{0:,d}".format(N)))
```

### Comparing `elektronn3-0.1.0/elektronn3/training/recalibration.py` & `elektronn3-0.1.1/elektronn3/training/recalibration.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/swa.py` & `elektronn3-0.1.1/elektronn3/training/swa.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/train_utils.py` & `elektronn3-0.1.1/elektronn3/training/train_utils.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/trainer.py` & `elektronn3-0.1.1/elektronn3/training/trainer.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/trainer_gnn.py` & `elektronn3-0.1.1/elektronn3/training/trainer_gnn.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/trainer_gnn_batch.py` & `elektronn3-0.1.1/elektronn3/training/trainer_gnn_batch.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/trainer_gnn_minibatch.py` & `elektronn3-0.1.1/elektronn3/training/trainer_gnn_minibatch.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3/training/triplettrainer.py` & `elektronn3-0.1.1/elektronn3/training/triplettrainer.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/elektronn3.egg-info/PKG-INFO` & `elektronn3-0.1.1/elektronn3.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: elektronn3
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utilities for 3D CNNs in PyTorch
 Home-page: https://github.com/ELEKTRONN/elektronn3
 Author: ELEKTRONN team
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Read the Docs](https://readthedocs.org/projects/elektronn3/badge/?version=latest)](https://elektronn3.readthedocs.io/en/latest/)
+[![PyPI](https://img.shields.io/pypi/v/elektronn3)](https://pypi.org/project/elektronn3/) [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/ELEKTRONN/elektronn3/python-publish.yml)](https://github.com/ELEKTRONN/elektronn3/actions) [![Read the Docs](https://readthedocs.org/projects/elektronn3/badge/?version=latest)](https://elektronn3.readthedocs.io/en/latest/)
 
 # elektronn3
 
 A PyTorch-based library for working with 3D and 2D convolutional neural networks, with focus on semantic segmentation of volumetric biomedical image data.
 
 Quick overview of **elektronn3**'s code structure:
```

### Comparing `elektronn3-0.1.0/elektronn3.egg-info/SOURCES.txt` & `elektronn3-0.1.1/elektronn3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/setup.py` & `elektronn3-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `elektronn3-0.1.0/versioneer.py` & `elektronn3-0.1.1/versioneer.py`

 * *Files identical despite different names*

