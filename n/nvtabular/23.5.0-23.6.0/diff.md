# Comparing `tmp/nvtabular-23.5.0.tar.gz` & `tmp/nvtabular-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvtabular-23.5.0.tar", last modified: Wed May 31 14:39:50 2023, max compression
+gzip compressed data, was "nvtabular-23.6.0.tar", last modified: Thu Jun 22 20:57:30 2023, max compression
```

## Comparing `nvtabular-23.5.0.tar` & `nvtabular-23.6.0.tar`

### file list

```diff
@@ -1,121 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.997602 nvtabular-23.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:39:10.000000 nvtabular-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-31 14:39:10.000000 nvtabular-23.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-31 14:39:49.997602 nvtabular-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-05-31 14:39:10.000000 nvtabular-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/cpp/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/cpp/nvtabular/
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/__init__.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/cpp/nvtabular/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/inference/__init__.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/inference/categorify.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-31 14:39:10.000000 nvtabular-23.5.0/cpp/nvtabular/inference/fill.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/merlin/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-31 14:39:10.000000 nvtabular-23.5.0/merlin/transforms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.985602 nvtabular-23.5.0/merlin/transforms/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-31 14:39:10.000000 nvtabular-23.5.0/merlin/transforms/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.997602 nvtabular-23.5.0/nvtabular/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:49.997602 nvtabular-23.5.0/nvtabular/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/dispatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/framework_utils/torch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/triton/
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/benchmarking_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/data_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25369 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/triton/model/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/model/model_pt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/triton/workflow_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular/inference/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3665 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/hugectr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/inference/workflow/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/loader/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/ops/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/add_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/bucketize.py
--rw-r--r--   0 runner    (1001) docker     (123)    61346 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/categorify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/column_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/data_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/difference_lag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/drop_low_cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/dropna.py
--rw-r--r--   0 runner    (1001) docker     (123)     5512 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/hashed_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/join_external.py
--rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/join_groupby.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/lambdaop.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/list_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/logop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/reduce_dtype_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/stat_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16901 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/target_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/ops/value_counts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/data_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/dataset_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/tools/inspector_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.993602 nvtabular-23.5.0/nvtabular/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/workflow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/workflow/node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17893 2023-05-31 14:39:10.000000 nvtabular-23.5.0/nvtabular/workflow/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.989602 nvtabular-23.5.0/nvtabular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 14:39:49.000000 nvtabular-23.5.0/nvtabular.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-31 14:39:10.000000 nvtabular-23.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:49.997602 nvtabular-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/gpu.txt
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-31 14:39:10.000000 nvtabular-23.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-31 14:39:49.997602 nvtabular-23.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-31 14:39:10.000000 nvtabular-23.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-05-31 14:39:10.000000 nvtabular-23.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.886384 nvtabular-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 20:56:45.000000 nvtabular-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-22 20:56:45.000000 nvtabular-23.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-22 20:57:30.886384 nvtabular-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-06-22 20:56:45.000000 nvtabular-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.874384 nvtabular-23.6.0/cpp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.878384 nvtabular-23.6.0/cpp/nvtabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-22 20:56:45.000000 nvtabular-23.6.0/cpp/nvtabular/__init__.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.878384 nvtabular-23.6.0/cpp/nvtabular/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-22 20:56:45.000000 nvtabular-23.6.0/cpp/nvtabular/inference/__init__.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11920 2023-06-22 20:56:45.000000 nvtabular-23.6.0/cpp/nvtabular/inference/categorify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-06-22 20:56:45.000000 nvtabular-23.6.0/cpp/nvtabular/inference/fill.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.874384 nvtabular-23.6.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.878384 nvtabular-23.6.0/merlin/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-22 20:56:45.000000 nvtabular-23.6.0/merlin/transforms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.878384 nvtabular-23.6.0/merlin/transforms/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-22 20:56:45.000000 nvtabular-23.6.0/merlin/transforms/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.890384 nvtabular-23.6.0/nvtabular/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 20:57:30.890384 nvtabular-23.6.0/nvtabular/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/dispatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.878384 nvtabular-23.6.0/nvtabular/framework_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.882384 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11968 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.882384 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.882384 nvtabular-23.6.0/nvtabular/framework_utils/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.882384 nvtabular-23.6.0/nvtabular/framework_utils/torch/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/torch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/torch/layers/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/torch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/framework_utils/torch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.882384 nvtabular-23.6.0/nvtabular/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.882384 nvtabular-23.6.0/nvtabular/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/loader/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/loader/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/loader/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/loader/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.886384 nvtabular-23.6.0/nvtabular/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/bucketize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76133 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/categorify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10299 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/column_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/data_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/difference_lag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/drop_low_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/dropna.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11143 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/hashed_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/join_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/join_groupby.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/lambdaop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/list_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/logop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6682 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/reduce_dtype_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/stat_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17258 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/target_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/ops/value_counts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.886384 nvtabular-23.6.0/nvtabular/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/tools/data_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/tools/dataset_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/tools/inspector_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.886384 nvtabular-23.6.0/nvtabular/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/workflow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      641 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/workflow/node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16553 2023-06-22 20:56:45.000000 nvtabular-23.6.0/nvtabular/workflow/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.878384 nvtabular-23.6.0/nvtabular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-22 20:57:30.000000 nvtabular-23.6.0/nvtabular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-22 20:57:30.000000 nvtabular-23.6.0/nvtabular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:57:30.000000 nvtabular-23.6.0/nvtabular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:57:30.000000 nvtabular-23.6.0/nvtabular.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 20:57:30.000000 nvtabular-23.6.0/nvtabular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 20:57:30.000000 nvtabular-23.6.0/nvtabular.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-06-22 20:56:45.000000 nvtabular-23.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:57:30.886384 nvtabular-23.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-22 20:56:45.000000 nvtabular-23.6.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-22 20:56:45.000000 nvtabular-23.6.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-22 20:56:45.000000 nvtabular-23.6.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:56:45.000000 nvtabular-23.6.0/requirements/gpu.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-22 20:56:45.000000 nvtabular-23.6.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-22 20:57:30.890384 nvtabular-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-22 20:56:45.000000 nvtabular-23.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-06-22 20:56:45.000000 nvtabular-23.6.0/versioneer.py
```

### Comparing `nvtabular-23.5.0/LICENSE` & `nvtabular-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/PKG-INFO` & `nvtabular-23.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvtabular
-Version: 23.5.0
+Version: 23.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/NVTabular
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 ## [NVTabular](https://github.com/NVIDIA/NVTabular)
 
 [![PyPI](https://img.shields.io/pypi/v/NVTabular?color=orange&label=version)](https://pypi.python.org/pypi/NVTabular/)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/NVTabular)](https://github.com/NVIDIA-Merlin/NVTabular/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/NVTabular)](https://github.com/NVIDIA-Merlin/NVTabular/blob/stable/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html)
 
 NVTabular is a feature engineering and preprocessing library for tabular data that is designed to easily manipulate terabyte scale datasets and train deep learning (DL) based recommender systems. It provides high-level abstraction to simplify code and accelerates computation on the GPU using the [RAPIDS Dask-cuDF](https://github.com/rapidsai/cudf/tree/main/python/dask_cudf) library.
 
 NVTabular is a component of [NVIDIA Merlin](https://developer.nvidia.com/nvidia-merlin), an open source framework for building and deploying recommender systems and works with the other Merlin components including [Merlin Models](https://github.com/NVIDIA-Merlin/models), [HugeCTR](https://github.com/NVIDIA/HugeCTR) and [Merlin Systems](https://github.com/NVIDIA-Merlin/systems) to provide end-to-end acceleration of recommender systems on the GPU. Extending beyond model training, with NVIDIA’s [Triton Inference Server](https://github.com/NVIDIA/tensorrt-inference-server), the feature engineering and preprocessing steps performed on the data during training can be automatically applied to incoming data during inference.
 
 <!-- <img src='https://developer.nvidia.com/blog/wp-content/uploads/2020/07/recommender-system-training-pipeline-1.png'/> -->
 
@@ -45,15 +45,15 @@
 NVTabular alleviates these challenges and helps data scientists and ML engineers:
 
 - process datasets that exceed GPU and CPU memory without having to worry about scale.
 - focus on what to do with the data and not how to do it by using abstraction at the operation level.
 - prepare datasets quickly and easily for experimentation so that more models can be trained.
 - deploy models into production by providing faster dataset transformation
 
-Learn more in the NVTabular [core features documentation](https://nvidia-merlin.github.io/NVTabular/main/core_features.html).
+Learn more in the NVTabular [core features documentation](https://nvidia-merlin.github.io/NVTabular/stable/core_features.html).
 
 ### Performance
 
 When running NVTabular on the Criteo 1TB Click Logs Dataset using a single V100 32GB GPU, feature engineering and preprocessing was able to be completed in 13 minutes. Furthermore, when running NVTabular on a DGX-1 cluster with eight V100 GPUs, feature engineering and preprocessing was able to be completed within three minutes. Combined with [HugeCTR](http://www.github.com/NVIDIA/HugeCTR/), the dataset can be processed and a full model can be trained in only six minutes.
 
 The performance of the Criteo DRLM workflow also demonstrates the effectiveness of the NVTabular library. The original ETL script provided in Numpy took over five days to complete. Combined with CPU training, the total iteration time is over one week. By optimizing the ETL code in Spark and running on a DGX-1 equivalent cluster, the time to complete feature engineering and preprocessing was reduced to three hours. Meanwhile, training was completed in one hour.
 
@@ -93,32 +93,32 @@
 
 | Container Name    | Container Location                                                                   | Functionality                              |
 | ----------------- | ------------------------------------------------------------------------------------ | ------------------------------------------ |
 | merlin-hugectr    | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-hugectr    | NVTabular, HugeCTR, and Triton Inference   |
 | merlin-tensorflow | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-tensorflow | NVTabular, Tensorflow and Triton Inference |
 | merlin-pytorch    | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-pytorch    | NVTabular, PyTorch, and Triton Inference   |
 
-To use these Docker containers, you'll first need to install the [NVIDIA Container Toolkit](https://github.com/NVIDIA/nvidia-docker) to provide GPU support for Docker. You can use the NGC links referenced in the table above to obtain more information about how to launch and run these containers. To obtain more information about the software and model versions that NVTabular supports per container, see [Support Matrix](https://github.com/NVIDIA/NVTabular/blob/main/docs/source/resources/support_matrix.rst).
+To use these Docker containers, you'll first need to install the [NVIDIA Container Toolkit](https://github.com/NVIDIA/nvidia-docker) to provide GPU support for Docker. You can use the NGC links referenced in the table above to obtain more information about how to launch and run these containers. To obtain more information about the software and model versions that NVTabular supports per container, see [Support Matrix](https://github.com/NVIDIA/NVTabular/blob/stable/docs/source/resources/support_matrix.rst).
 
 ### Notebook Examples and Tutorials
 
-We provide a [collection of examples](https://github.com/NVIDIA-Merlin/NVTabular/tree/main/examples) to demonstrate feature engineering with NVTabular as Jupyter notebooks:
+We provide a [collection of examples](https://github.com/NVIDIA-Merlin/NVTabular/tree/stable/examples) to demonstrate feature engineering with NVTabular as Jupyter notebooks:
 
 - Introduction to NVTabular's High-Level API
 - Advanced workflows with NVTabular
 - NVTabular on CPU
 - Scaling NVTabular to multi-GPU systems
 
 In addition, NVTabular is used in many of our examples in other Merlin libraries:
 
-- [End-To-End Examples with Merlin](https://github.com/NVIDIA-Merlin/Merlin/tree/main/examples)
-- [Training Examples with Merlin Models](https://github.com/NVIDIA-Merlin/models/tree/main/examples)
-- [Training Examples with Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/tree/main/examples)
+- [End-To-End Examples with Merlin](https://github.com/NVIDIA-Merlin/Merlin/tree/stable/examples)
+- [Training Examples with Merlin Models](https://github.com/NVIDIA-Merlin/models/tree/stable/examples)
+- [Training Examples with Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/tree/stable/examples)
 
 ### Feedback and Support
 
-If you'd like to contribute to the library directly, see the [Contributing.md](https://github.com/NVIDIA/NVTabular/blob/main/CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
+If you'd like to contribute to the library directly, see the [Contributing.md](https://github.com/NVIDIA/NVTabular/blob/stable/CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
 
 If you're interested in learning more about how NVTabular works, see
-[our NVTabular documentation](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html). We also have [API documentation](https://nvidia-merlin.github.io/NVTabular/main/api/index.html) that outlines the specifics of the available calls within the library.
+[our NVTabular documentation](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html). We also have [API documentation](https://nvidia-merlin.github.io/NVTabular/stable/api/index.html) that outlines the specifics of the available calls within the library.
```

### Comparing `nvtabular-23.5.0/README.md` & `nvtabular-23.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## [NVTabular](https://github.com/NVIDIA/NVTabular)
 
 [![PyPI](https://img.shields.io/pypi/v/NVTabular?color=orange&label=version)](https://pypi.python.org/pypi/NVTabular/)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/NVTabular)](https://github.com/NVIDIA-Merlin/NVTabular/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/NVTabular)](https://github.com/NVIDIA-Merlin/NVTabular/blob/stable/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html)
 
 NVTabular is a feature engineering and preprocessing library for tabular data that is designed to easily manipulate terabyte scale datasets and train deep learning (DL) based recommender systems. It provides high-level abstraction to simplify code and accelerates computation on the GPU using the [RAPIDS Dask-cuDF](https://github.com/rapidsai/cudf/tree/main/python/dask_cudf) library.
 
 NVTabular is a component of [NVIDIA Merlin](https://developer.nvidia.com/nvidia-merlin), an open source framework for building and deploying recommender systems and works with the other Merlin components including [Merlin Models](https://github.com/NVIDIA-Merlin/models), [HugeCTR](https://github.com/NVIDIA/HugeCTR) and [Merlin Systems](https://github.com/NVIDIA-Merlin/systems) to provide end-to-end acceleration of recommender systems on the GPU. Extending beyond model training, with NVIDIA’s [Triton Inference Server](https://github.com/NVIDIA/tensorrt-inference-server), the feature engineering and preprocessing steps performed on the data during training can be automatically applied to incoming data during inference.
 
 <!-- <img src='https://developer.nvidia.com/blog/wp-content/uploads/2020/07/recommender-system-training-pipeline-1.png'/> -->
 
@@ -22,15 +22,15 @@
 NVTabular alleviates these challenges and helps data scientists and ML engineers:
 
 - process datasets that exceed GPU and CPU memory without having to worry about scale.
 - focus on what to do with the data and not how to do it by using abstraction at the operation level.
 - prepare datasets quickly and easily for experimentation so that more models can be trained.
 - deploy models into production by providing faster dataset transformation
 
-Learn more in the NVTabular [core features documentation](https://nvidia-merlin.github.io/NVTabular/main/core_features.html).
+Learn more in the NVTabular [core features documentation](https://nvidia-merlin.github.io/NVTabular/stable/core_features.html).
 
 ### Performance
 
 When running NVTabular on the Criteo 1TB Click Logs Dataset using a single V100 32GB GPU, feature engineering and preprocessing was able to be completed in 13 minutes. Furthermore, when running NVTabular on a DGX-1 cluster with eight V100 GPUs, feature engineering and preprocessing was able to be completed within three minutes. Combined with [HugeCTR](http://www.github.com/NVIDIA/HugeCTR/), the dataset can be processed and a full model can be trained in only six minutes.
 
 The performance of the Criteo DRLM workflow also demonstrates the effectiveness of the NVTabular library. The original ETL script provided in Numpy took over five days to complete. Combined with CPU training, the total iteration time is over one week. By optimizing the ETL code in Spark and running on a DGX-1 equivalent cluster, the time to complete feature engineering and preprocessing was reduced to three hours. Meanwhile, training was completed in one hour.
 
@@ -70,30 +70,30 @@
 
 | Container Name    | Container Location                                                                   | Functionality                              |
 | ----------------- | ------------------------------------------------------------------------------------ | ------------------------------------------ |
 | merlin-hugectr    | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-hugectr    | NVTabular, HugeCTR, and Triton Inference   |
 | merlin-tensorflow | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-tensorflow | NVTabular, Tensorflow and Triton Inference |
 | merlin-pytorch    | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-pytorch    | NVTabular, PyTorch, and Triton Inference   |
 
-To use these Docker containers, you'll first need to install the [NVIDIA Container Toolkit](https://github.com/NVIDIA/nvidia-docker) to provide GPU support for Docker. You can use the NGC links referenced in the table above to obtain more information about how to launch and run these containers. To obtain more information about the software and model versions that NVTabular supports per container, see [Support Matrix](https://github.com/NVIDIA/NVTabular/blob/main/docs/source/resources/support_matrix.rst).
+To use these Docker containers, you'll first need to install the [NVIDIA Container Toolkit](https://github.com/NVIDIA/nvidia-docker) to provide GPU support for Docker. You can use the NGC links referenced in the table above to obtain more information about how to launch and run these containers. To obtain more information about the software and model versions that NVTabular supports per container, see [Support Matrix](https://github.com/NVIDIA/NVTabular/blob/stable/docs/source/resources/support_matrix.rst).
 
 ### Notebook Examples and Tutorials
 
-We provide a [collection of examples](https://github.com/NVIDIA-Merlin/NVTabular/tree/main/examples) to demonstrate feature engineering with NVTabular as Jupyter notebooks:
+We provide a [collection of examples](https://github.com/NVIDIA-Merlin/NVTabular/tree/stable/examples) to demonstrate feature engineering with NVTabular as Jupyter notebooks:
 
 - Introduction to NVTabular's High-Level API
 - Advanced workflows with NVTabular
 - NVTabular on CPU
 - Scaling NVTabular to multi-GPU systems
 
 In addition, NVTabular is used in many of our examples in other Merlin libraries:
 
-- [End-To-End Examples with Merlin](https://github.com/NVIDIA-Merlin/Merlin/tree/main/examples)
-- [Training Examples with Merlin Models](https://github.com/NVIDIA-Merlin/models/tree/main/examples)
-- [Training Examples with Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/tree/main/examples)
+- [End-To-End Examples with Merlin](https://github.com/NVIDIA-Merlin/Merlin/tree/stable/examples)
+- [Training Examples with Merlin Models](https://github.com/NVIDIA-Merlin/models/tree/stable/examples)
+- [Training Examples with Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/tree/stable/examples)
 
 ### Feedback and Support
 
-If you'd like to contribute to the library directly, see the [Contributing.md](https://github.com/NVIDIA/NVTabular/blob/main/CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
+If you'd like to contribute to the library directly, see the [Contributing.md](https://github.com/NVIDIA/NVTabular/blob/stable/CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
 
 If you're interested in learning more about how NVTabular works, see
-[our NVTabular documentation](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html). We also have [API documentation](https://nvidia-merlin.github.io/NVTabular/main/api/index.html) that outlines the specifics of the available calls within the library.
+[our NVTabular documentation](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html). We also have [API documentation](https://nvidia-merlin.github.io/NVTabular/stable/api/index.html) that outlines the specifics of the available calls within the library.
```

### Comparing `nvtabular-23.5.0/cpp/nvtabular/__init__.cc` & `nvtabular-23.6.0/cpp/nvtabular/__init__.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/cpp/nvtabular/inference/__init__.cc` & `nvtabular-23.6.0/cpp/nvtabular/inference/__init__.cc`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/cpp/nvtabular/inference/categorify.cc` & `nvtabular-23.6.0/cpp/nvtabular/inference/categorify.cc`

 * *Files 7% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         py::object df = pandas.attr("read_parquet")(filename);
         py::object isnull = pandas.attr("isnull");
         py::array values = df[column_name.c_str()].attr("values");
         auto dtype = values.dtype();
 
         if ((dtype.kind() == 'O') || (dtype.kind() == 'U'))
         {
-          int64_t i = 0;
+          int64_t i = UNIQUE_OFFSET;
           for (auto &value : values)
           {
             if (!py::cast<bool>(isnull(value)))
             {
               if (PyUnicode_Check(value.ptr()) || PyBytes_Check(value.ptr()))
               {
                 std::string key = py::cast<std::string>(value);
@@ -134,28 +134,37 @@
       template <typename T>
       void insert_int_mapping(py::array_t<T> values)
       {
         const T *data = values.data();
         size_t size = values.size();
         for (size_t i = 0; i < size; ++i)
         {
-          mapping_int[static_cast<int64_t>(data[i])] = i;
+          mapping_int[static_cast<int64_t>(data[i])] = i + UNIQUE_OFFSET;
         }
       }
 
       template <typename T>
       py::array transform_int(py::array_t<T> input) const
       {
+        py::object pandas = py::module_::import("pandas");
+        py::object isnull = pandas.attr("isnull");
         py::array_t<int64_t> output(input.size());
         const T *input_data = input.data();
         int64_t *output_data = output.mutable_data();
         for (int64_t i = 0; i < input.size(); ++i)
         {
           auto it = mapping_int.find(static_cast<int64_t>(input_data[i]));
-          output_data[i] = it == mapping_int.end() ? 0 : it->second;
+          if (it == mapping_int.end())
+          {
+            output_data[i] = py::cast<bool>(isnull(input_data[i])) ? NULL_INDEX : OOV_INDEX;
+          }
+          else
+          {
+            output_data[i] = it->second;
+          }
         }
         return output;
       }
 
       py::array transform(py::array input) const
       {
         auto dtype = input.dtype();
@@ -165,26 +174,26 @@
           size_t i = 0;
           py::array_t<int64_t> output(input.size());
           int64_t *data = output.mutable_data();
           for (auto &value : input)
           {
             if (value.is_none())
             {
-              data[i] = 0;
+              data[i] = NULL_INDEX;
             }
             else if (PyUnicode_Check(value.ptr()) || PyBytes_Check(value.ptr()))
             {
               std::string key = py::cast<std::string>(value);
               auto it = mapping_str.find(key);
-              data[i] = it == mapping_str.end() ? 0 : it->second;
+              data[i] = it == mapping_str.end() ? OOV_INDEX : it->second;
             }
             else if (PyBool_Check(value.ptr()))
             {
               auto it = mapping_int.find(value.ptr() == Py_True);
-              data[i] = it == mapping_int.end() ? 0 : it->second;
+              data[i] = it == mapping_int.end() ? OOV_INDEX : it->second;
             }
             else
             {
               throw std::invalid_argument("unknown dtype");
             }
             i++;
           }
@@ -243,14 +252,19 @@
       }
 
       std::string filename;
       std::string column_name;
 
       std::unordered_map<std::string, int64_t> mapping_str;
       std::unordered_map<int64_t, int64_t> mapping_int;
+
+      // TODO: Handle multiple OOV buckets?
+      const int64_t NULL_INDEX = 1;
+      const int64_t OOV_INDEX = 2;
+      const int64_t UNIQUE_OFFSET = 3;
     };
 
     // Reads in a parquet category mapping file in cpu memory using pandas
     std::shared_ptr<ColumnMapping> get_column_mapping(const std::string &column_name,
                                                       const std::string &filename)
     {
       // because of how we're doing multi-gpu inside of tritonserver, we could have
@@ -321,11 +335,16 @@
           .def("transform", &CategorifyTransform::transform)
 
           // this operator currently only supports CPU arrays
           .def_property_readonly("supports", [](py::object self)
                                  {
                                    py::object supports = py::module_::import("nvtabular").attr("graph").attr("base_operator").attr("Supports");
                                    return supports.attr("CPU_DICT_ARRAY");
+                                 })
+          .def_property_readonly("supported_formats", [](py::object self)
+                                 {
+                                   py::object supported = py::module_::import("nvtabular").attr("graph").attr("base_operator").attr("DataFormats");
+                                   return supported.attr("NUMPY_DICT_ARRAY");
                                  });
     }
   } // namespace inference
 } // namespace nvtabular
```

### Comparing `nvtabular-23.5.0/cpp/nvtabular/inference/fill.cc` & `nvtabular-23.6.0/cpp/nvtabular/inference/fill.cc`

 * *Files 5% similar despite different names*

```diff
@@ -111,11 +111,16 @@
           .def(py::init<py::object>())
           // this operator currently only supports CPU arrays
           .def_property_readonly("supports", [](py::object self)
                                  {
                                    py::object supports = py::module_::import("nvtabular").attr("graph").attr("base_operator").attr("Supports");
                                    return supports.attr("CPU_DICT_ARRAY");
                                  })
+          .def_property_readonly("supported_formats", [](py::object self)
+                                 {
+                                   py::object supported = py::module_::import("nvtabular").attr("graph").attr("base_operator").attr("DataFormats");
+                                   return supported.attr("NUMPY_DICT_ARRAY");
+                                 })
           .def("transform", &FillTransform::transform);
     }
   } // namespace inference
 } // namespace nvtabular
```

### Comparing `nvtabular-23.5.0/merlin/transforms/__init__.py` & `nvtabular-23.6.0/merlin/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/merlin/transforms/ops/__init__.py` & `nvtabular-23.6.0/merlin/transforms/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/__init__.py` & `nvtabular-23.6.0/nvtabular/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
 # this is to mimic the previous API, but all of these should probably be removed
 import merlin.dag as graph  # noqa
 from merlin import io
 from merlin.core import dispatch, utils  # noqa
 from merlin.dag import ColumnSelector
 from merlin.schema import ColumnSchema, Schema
-from nvtabular import workflow  # noqa
-from nvtabular import _version
+from nvtabular import _version, ops, workflow  # noqa
 
 # suppress some warnings with cudf warning about column ordering with dlpack
 # and numba warning about deprecated environment variables
 warnings.filterwarnings("ignore", module="cudf.io.dlpack")
 warnings.filterwarnings("ignore", module="numba.cuda.envvars")
```

### Comparing `nvtabular-23.5.0/nvtabular/dispatch.py` & `nvtabular-23.6.0/nvtabular/dispatch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/__init__.py` & `nvtabular-23.6.0/nvtabular/framework_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/__init__.py` & `nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py` & `nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/feature_column_utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/__init__.py` & `nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/embedding.py` & `nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/interaction.py` & `nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/interaction.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py` & `nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/layers/outer_product.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py` & `nvtabular-23.6.0/nvtabular/framework_utils/tensorflow/tfrecords_to_parquet.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/torch/__init__.py` & `nvtabular-23.6.0/nvtabular/framework_utils/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/__init__.py` & `nvtabular-23.6.0/nvtabular/framework_utils/torch/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/torch/layers/embeddings.py` & `nvtabular-23.6.0/nvtabular/framework_utils/torch/layers/embeddings.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/torch/models.py` & `nvtabular-23.6.0/nvtabular/framework_utils/torch/models.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/framework_utils/torch/utils.py` & `nvtabular-23.6.0/nvtabular/framework_utils/torch/utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/graph.py` & `nvtabular-23.6.0/nvtabular/graph.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/inference/__init__.py` & `nvtabular-23.6.0/nvtabular/io.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,29 @@
+#
 # Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
+# pylint: disable=wildcard-import,unused-import,unused-wildcard-import
 import warnings
 
+# Re-export classes/modules from the core library for backwards compatibility
+from merlin.io import *  # noqa
+
 warnings.warn(
-    "The `nvtabular.inference` module is being replaced by the Merlin Systems library. "
-    "Support for importing from `nvtabular.inference` is deprecated, "
-    "and will be removed in a future version. Please consider using "
-    "operators and ensembles from Merlin Systems instead.",
+    "The `nvtabular.io` module has moved to `merlin.io`. "
+    "Support for importing from `nvtabular.io` is deprecated, "
+    "and will be removed in a future version. Please update "
+    "your imports to refer to `merlin.io`.",
     DeprecationWarning,
 )
```

### Comparing `nvtabular-23.5.0/nvtabular/inference/triton/__init__.py` & `nvtabular-23.6.0/nvtabular/ops/reduce_dtype_size.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,86 @@
-# Copyright (c) 2021, NVIDIA CORPORATION.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-#
-import json
-import os
-
-import pandas as pd
-import tritonclient.grpc as grpcclient
-from tritonclient.utils import np_to_triton_dtype
-
-from merlin.core.dispatch import is_list_dtype, is_string_dtype, make_df
-from nvtabular.inference.triton.ensemble import (  # noqa
-    _convert_string2pytorch_dtype,
-    export_hugectr_ensemble,
-    export_pytorch_ensemble,
-    export_tensorflow_ensemble,
-    generate_hugectr_model,
-    generate_nvtabular_model,
-)
-
-
-def convert_df_to_triton_input(column_names, batch, input_class=grpcclient.InferInput):
-    columns = [(col, batch[col]) for col in column_names]
-    inputs = []
-    for i, (name, col) in enumerate(columns):
-        if is_list_dtype(col):
-            if isinstance(col, pd.Series):
-                raise ValueError("this function doesn't support CPU list values yet")
-            inputs.append(
-                _convert_column_to_triton_input(
-                    col._column.offsets.values_host.astype("int64"), name + "__nnzs", input_class
-                )
-            )
-            inputs.append(
-                _convert_column_to_triton_input(
-                    col.list.leaves.values_host.astype("int64"), name + "__values", input_class
-                )
-            )
-        else:
-            values = col.values if isinstance(col, pd.Series) else col.values_host
-            inputs.append(_convert_column_to_triton_input(values, name, input_class))
-    return inputs
-
-
-def _convert_column_to_triton_input(col, name, input_class=grpcclient.InferInput):
-    col = col.reshape(len(col), 1)
-    input_tensor = input_class(name, col.shape, np_to_triton_dtype(col.dtype))
-    input_tensor.set_data_from_numpy(col)
-    return input_tensor
-
-
-def convert_triton_output_to_df(columns, response):
-    return make_df({col: response.as_numpy(col) for col in columns})
-
-
-def get_column_types(path):
-    return json.load(open(os.path.join(path, "column_types.json"), encoding="utf8"))
-
-
-def _convert_tensor(t):
-    out = t.as_numpy()
-    # cudf doesn't seem to handle dtypes like |S15 or object that well
-    if is_string_dtype(out.dtype):
-        out = out.astype("str")
-    return out
+#
+# Copyright (c) 2021, NVIDIA CORPORATION.
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+#
+import dask.dataframe as dd
+import numpy as np
+
+from merlin.core.dispatch import DataFrameType, annotate
+from merlin.dag.ops.stat_operator import StatOperator
+from merlin.schema import Schema
+from nvtabular.ops.operator import ColumnSelector, Operator
+
+_INT_DTYPES = [np.int8, np.int16, np.int32, np.int64]
+
+
+class ReduceDtypeSize(StatOperator):
+    """
+    ReduceDtypeSize changes the dtypes of numeric columns. For integer columns
+    this will choose a dtype such that the minimum and maximum values in the
+    column will fit. For float columns this will cast to a float32.
+    """
+
+    def __init__(self, float_dtype=np.float32):
+        super().__init__()
+        self.float_dtype = float_dtype
+        self.ranges = {}
+        self.dtypes = {}
+
+    @annotate("reduce_dtype_size_fit", color="green", domain="nvt_python")
+    def fit(self, col_selector: ColumnSelector, ddf: dd.DataFrame):
+        return {col: (ddf[col].min(), ddf[col].max()) for col in col_selector.names}
+
+    def fit_finalize(self, dask_stats):
+        self.ranges = dask_stats
+
+    def clear(self):
+        self.dtypes = {}
+        self.ranges = {}
+
+    @annotate("reduce_dtype_size_transform", color="darkgreen", domain="nvt_python")
+    def transform(self, col_selector: ColumnSelector, df: DataFrameType) -> DataFrameType:
+        for col_name, col_dtype in self.dtypes.items():
+            np_dtype = col_dtype.to_numpy
+            df[col_name] = df[col_name].astype(np_dtype)
+        return df
+
+    def compute_output_schema(self, input_schema, selector, prev_output_schema=None):
+        if not self.ranges:
+            return input_schema
+
+        output_columns = []
+        for column, (min_value, max_value) in self.ranges.items():
+            column = input_schema[column]
+
+            dtype = column.dtype
+            if column.dtype.element_type.value == "int":
+                for possible_dtype in _INT_DTYPES:
+                    dtype_range = np.iinfo(possible_dtype)
+                    if min_value >= dtype_range.min and max_value <= dtype_range.max:
+                        dtype = possible_dtype
+                        break
+
+            elif column.dtype.element_type.value == "float":
+                dtype = self.float_dtype
+
+            output_columns.append(column.with_dtype(dtype))
+
+        self.dtypes = {column.name: column.dtype for column in output_columns}
+        return Schema(output_columns)
+
+    transform.__doc__ = Operator.transform.__doc__
+    compute_output_schema.__doc__ = Operator.compute_output_schema.__doc__
+    fit.__doc__ = StatOperator.fit.__doc__
+    fit_finalize.__doc__ = StatOperator.fit_finalize.__doc__
+    clear.__doc__ = StatOperator.clear.__doc__
```

### Comparing `nvtabular-23.5.0/nvtabular/inference/triton/model/__init__.py` & `nvtabular-23.6.0/nvtabular/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#
 # Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `nvtabular-23.5.0/nvtabular/inference/workflow/__init__.py` & `nvtabular-23.6.0/nvtabular/workflow/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
+#
 # Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from merlin.dag import Node
+
+WorkflowNode = Node
```

### Comparing `nvtabular-23.5.0/nvtabular/io.py` & `nvtabular-23.6.0/nvtabular/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # limitations under the License.
 #
 
 # pylint: disable=wildcard-import,unused-import,unused-wildcard-import
 import warnings
 
 # Re-export classes/modules from the core library for backwards compatibility
-from merlin.io import *  # noqa
+from merlin.core.compat import *  # noqa
 
 warnings.warn(
-    "The `nvtabular.io` module has moved to `merlin.io`. "
-    "Support for importing from `nvtabular.io` is deprecated, "
+    "The `nvtabular.utils` module has moved to `merlin.core.utils`. "
+    "Support for importing from `nvtabular.utils` is deprecated, "
     "and will be removed in a future version. Please update "
-    "your imports to refer to `merlin.io`.",
+    "your imports to refer to `merlin.core.utils`.",
     DeprecationWarning,
 )
```

### Comparing `nvtabular-23.5.0/nvtabular/loader/__init__.py` & `nvtabular-23.6.0/nvtabular/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/loader/backend.py` & `nvtabular-23.6.0/nvtabular/loader/backend.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/loader/tensorflow.py` & `nvtabular-23.6.0/nvtabular/loader/tensorflow.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/loader/tf_utils.py` & `nvtabular-23.6.0/nvtabular/loader/tf_utils.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/loader/torch.py` & `nvtabular-23.6.0/nvtabular/loader/torch.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/__init__.py` & `nvtabular-23.6.0/nvtabular/ops/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+from merlin.dag import ColumnSelector
+
 # alias submodules here to avoid breaking everything with moving to submodules
 # flake8: noqa
 from nvtabular.ops.add_metadata import (
     AddMetadata,
     AddProperties,
     AddTags,
     TagAsItemFeatures,
@@ -40,13 +42,13 @@
 from nvtabular.ops.hashed_cross import HashedCross
 from nvtabular.ops.join_external import JoinExternal
 from nvtabular.ops.join_groupby import JoinGroupby
 from nvtabular.ops.lambdaop import LambdaOp
 from nvtabular.ops.list_slice import ListSlice
 from nvtabular.ops.logop import LogOp
 from nvtabular.ops.normalize import Normalize, NormalizeMinMax
-from nvtabular.ops.operator import ColumnSelector, Operator
+from nvtabular.ops.operator import Operator
 from nvtabular.ops.reduce_dtype_size import ReduceDtypeSize
 from nvtabular.ops.rename import Rename
 from nvtabular.ops.stat_operator import StatOperator
 from nvtabular.ops.target_encoding import TargetEncoding
 from nvtabular.ops.value_counts import ValueCount
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/add_metadata.py` & `nvtabular-23.6.0/nvtabular/ops/add_metadata.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/bucketize.py` & `nvtabular-23.6.0/nvtabular/ops/bucketize.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/categorify.py` & `nvtabular-23.6.0/nvtabular/ops/categorify.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,53 +9,70 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
+import math
 import os
 import warnings
+from collections import defaultdict
 from copy import deepcopy
 from dataclasses import dataclass
 from operator import getitem
 from pathlib import Path
 from typing import Optional, Union
 
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 import pyarrow as pa
+import pyarrow.dataset as pa_ds
 from dask.base import tokenize
+from dask.blockwise import BlockIndex
 from dask.core import flatten
-from dask.dataframe.core import _concat
+from dask.dataframe.core import DataFrame as DaskDataFrame
+from dask.dataframe.core import _concat, new_dd_object
 from dask.dataframe.shuffle import shuffle_group
 from dask.delayed import Delayed
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import parse_bytes
 from fsspec.core import get_fs_token_paths
-from pyarrow import parquet as pq
 
 from merlin.core import dispatch
 from merlin.core.dispatch import DataFrameType, annotate, is_cpu_object, nullable_series
 from merlin.core.utils import device_mem_size, run_on_worker
+from merlin.dag.ops.stat_operator import StatOperator
 from merlin.io.worker import fetch_table_data, get_worker_cache
 from merlin.schema import Schema, Tags
 from nvtabular.ops.operator import ColumnSelector, Operator
-from nvtabular.ops.stat_operator import StatOperator
+
+# Constants
+# (NVTabular will reserve `0` for padding and `1` for nulls)
+PAD_OFFSET = 0
+NULL_OFFSET = 1
+OOV_OFFSET = 2
 
 
 class Categorify(StatOperator):
     """
     Most of the data set will contain categorical features,
     and these variables are typically stored as text values.
     Machine Learning algorithms don't support these text values.
     Categorify operation can be added to the workflow to
     transform categorical features into unique integer values.
 
+    Encoding Convention::
+
+        - `0`: Not used by `Categorify` (reserved for padding).
+        - `1`: Null and NaN values.
+        - `[2, 2 + num_buckets)`: OOV values (including hash buckets).
+        - `[2 + num_buckets, max_size)`: Unique vocabulary.
+
     Example usage::
 
         # Define pipeline
         cat_features = CATEGORICAL_COLUMNS >> nvt.ops.Categorify(freq_threshold=10)
 
         # Initialize the workflow and execute it
         proc = nvt.Workflow(cat_features)
@@ -117,104 +134,125 @@
         print(ddf.compute())
 
     Parameters
     -----------
     freq_threshold : int or dictionary:{column: freq_limit_value}, default 0
         Categories with a count/frequency below this threshold will be
         omitted from the encoding and corresponding data will be mapped
-        to the "null" category. Can be represented as both an integer or
+        to the OOV indices. Can be represented as both an integer or
         a dictionary with column names as keys and frequency limit as
         value. If dictionary is used, all columns targeted must be included
         in the dictionary.
     encode_type : {"joint", "combo"}, default "joint"
         If "joint", the columns within any multi-column group will be
         jointly encoded. If "combo", the combination of values will be
         encoded as a new column. Note that replacement is not allowed for
         "combo", because the same column name can be included in
         multiple groups.
-    tree_width : dict or int, optional
-        Tree width of the hash-based groupby reduction for each categorical
-        column. High-cardinality columns may require a large `tree_width`,
-        while low-cardinality columns can likely use `tree_width=1`.
+    split_out : dict or int, optional
+        Number of files needed to store the unique values of each categorical
+        column. High-cardinality columns may require `split_out>1`, while
+        low-cardinality columns should be fine with the `split_out=1` default.
         If passing a dict, each key and value should correspond to the column
-        name and width, respectively. The default value is 8 for all columns.
+        name and value, respectively. The default value is 1 for all columns.
+    split_every : dict or int, optional
+        Number of adjacent partitions to aggregate in each tree-reduction
+        node. The default value is 8 for all columns.
     out_path : str, optional
         Root directory where groupby statistics will be written out in
         parquet format.
     on_host : bool, default True
         Whether to convert cudf data to pandas between tasks in the hash-based
         groupby reduction. The extra host <-> device data movement can reduce
         performance.  However, using `on_host=True` typically improves stability
         (by avoiding device-level memory pressure).
-    na_sentinel : default 0
-        Label to use for null-category mapping
     cat_cache : {"device", "host", "disk"} or dict
         Location to cache the list of unique categories for
         each categorical column. If passing a dict, each key and value
         should correspond to the column name and location, respectively.
         Default is "host" for all columns.
     dtype :
         If specified, categorical labels will be cast to this dtype
         after encoding is performed.
     name_sep : str, default "_"
         String separator to use between concatenated column names
         for multi-column groups.
     search_sorted : bool, default False.
         Set it True to apply searchsorted algorithm in encoding.
-    num_buckets : int, or dictionary:{column: num_hash_buckets}
-        Column-wise modulo to apply after hash function. Note that this
-        means that the corresponding value will be the categorical cardinality
-        of the transformed categorical feature. If given as an int, that value
-        will be used as the number of "hash buckets" for every feature. If a dictionary is passed,
-        it will be used to specify explicit mappings from a column name to a number of buckets.
-        In this case, only the columns specified in the keys of `num_buckets`
-        will be transformed.
-    max_size : int or dictionary:{column: max_size_value}, default 0
-        This parameter allows you to set the maximum size for an embedding table for each column.
-        For example, if max_size is set to 1000 only the first 999 most frequent values for each
-        column will be be encoded, and the rest will be mapped to a single value (0). To map the
-        rest to a number of buckets,  you can set the num_buckets parameter > 1. In that case, topK
-        value will be `max_size - num_buckets -1`.  Setting the max_size param means that
-        freq_threshold should not be given.  If the num_buckets parameter is set,  it must be
-        smaller than the max_size value.
-    start_index: int, default 0
-        The start index where Categorify will begin to translate dataframe entries
-        into integer values, including an initial out-of-vocabulary encoding value.
-        For instance, if our original translated dataframe entries appear
-        as [[1], [1, 4], [3, 2], [2]], with an out-of-vocabulary value of 0, then with a
-        start_index of 16, Categorify will reserve 16 as the out-of-vocabulary encoding value,
-        and our new translated dataframe entry will now be [[17], [17, 20], [19, 18], [18]].
-        This parameter is useful to reserve an initial segment of non-negative translated integers
-        for special user-defined values.
-    cardinality_memory_limit: int or str, default None
+    num_buckets : int, or dictionary:{column: num_oov_indices}, optional
+        Number of indices to reserve for out-of-vocabulary (OOV) encoding at
+        transformation time. By default, all OOV values will be mapped to
+        the same index (`2`). If `num_buckets` is set to an integer greater
+        than one, a column-wise hash and modulo will be used to map each OOV
+        value to an index in the range `[2, 2 + num_buckets)`. A dictionary
+        may be used if the desired `num_buckets` behavior varies by column.
+    max_size : int or dictionary:{column: max_size_value}, optional
+        Set the maximum size of the expected embedding table for each column.
+        For example, if `max_size` is set to 1000, only the first 997 most-
+        frequent values will be included in the unique-value vocabulary, and
+        all remaining non-null values will be mapped to the OOV indices
+        (indices `0` and `1` will still be reserved for padding and nulls).
+        To use multiple OOV indices for infrequent values, set the `num_buckets`
+        parameter accordingly. Note that `max_size` cannot be combined with
+        `freq_threshold`, and it cannot be less than `num_buckets + 2`. By
+        default, the total number of encoding indices will be unconstrained.
+    cardinality_memory_limit: int or str, optional
         Upper limit on the "allowed" memory usage of the internal DataFrame and Table objects
         used to store unique categories. By default, this limit is 12.5% of the total memory.
         Note that this argument is meant as a guide for internal optimizations and UserWarnings
         within NVTabular, and does not guarantee that the memory limit will be satisfied.
     """
 
     def __init__(
         self,
         freq_threshold=0,
         out_path=None,
-        tree_width=None,
-        na_sentinel=None,
         cat_cache="host",
         dtype=None,
         on_host=True,
         encode_type="joint",
         name_sep="_",
         search_sorted=False,
         num_buckets=None,
         vocabs=None,
         max_size=0,
-        start_index=0,
         single_table=False,
         cardinality_memory_limit=None,
+        tree_width=None,
+        split_out=1,
+        split_every=8,
+        **kwargs,  # Deprecated/unsupported arguments
     ):
+        # Handle deprecations and unsupported kwargs
+        if "start_index" in kwargs:
+            raise ValueError(
+                "start_index is now deprecated. `Categorify` will always "
+                "reserve index `0` for user-specific purposes, and will "
+                "use index `1` for null values."
+            )
+        if "na_sentinel" in kwargs:
+            raise ValueError(
+                "na_sentinel is now deprecated. `Categorify` will always "
+                "reserve index `1` for null values, and the following "
+                "`num_buckets` indices for out-of-vocabulary values "
+                "(or just index `2` if `num_buckets is None`)."
+            )
+        if kwargs:
+            raise ValueError(f"Unrecognized key-word arguments: {kwargs}")
+
+        # Warn user if they set num_buckets without setting max_size or
+        # freq_threshold - This setting used to hash everything, but will
+        # now just use multiple indices for OOV encodings at transform time
+        if num_buckets and not (max_size or freq_threshold):
+            warnings.warn(
+                "You are setting num_buckets without using max_size or "
+                "freq_threshold to restrict the number of distinct "
+                "categories. Are you sure this is what you want?"
+            )
+
         # We need to handle three types of encoding here:
         #
         #   (1) Conventional encoding. There are no multi-column groups. So,
         #       each categorical column is separately transformed into a new
         #       "encoded" column (1-to-1).  The unique values are calculated
         #       separately for each column.
         #
@@ -251,23 +289,23 @@
             raise ValueError("Passing in vocabs is not supported with a combo encoding.")
 
         # Other self-explanatory initialization
         super().__init__()
         self.single_table = single_table
         self.freq_threshold = freq_threshold or 0
         self.out_path = out_path or "./"
-        self.tree_width = tree_width
-        self.na_sentinel = na_sentinel or 0
         self.dtype = dtype
         self.on_host = on_host
         self.cat_cache = cat_cache
         self.encode_type = encode_type
         self.search_sorted = search_sorted
-        self.start_index = start_index
         self.cardinality_memory_limit = cardinality_memory_limit
+        self.split_every = split_every
+        self.split_out = split_out
+        _deprecate_tree_width(tree_width)
 
         if self.search_sorted and self.freq_threshold:
             raise ValueError(
                 "cannot use search_sorted=True with anything else than the default freq_threshold"
             )
         if num_buckets == 0:
             raise ValueError(
@@ -340,16 +378,19 @@
                 warnings.warn("Cannot use `search_sorted=True` for pandas-backed data.")
 
         # convert tuples to lists
         cols_with_vocabs = list(self.categories.keys())
         columns = [
             list(c) if isinstance(c, tuple) else c
             for c in col_selector.grouped_names
-            if c not in cols_with_vocabs
+            if (_make_name(*c, sep=self.name_sep) if isinstance(c, tuple) else c)
+            not in cols_with_vocabs
         ]
+        if not columns:
+            return Delayed("no-op", {"no-op": {}})
 
         # Define a rough row-count at which we are likely to
         # start hitting memory-pressure issues that cannot
         # be accommodated with smaller partition sizes.
         # By default, we estimate a "problematic" cardinality
         # to be one that consumes >12.5% of the total memory.
         self.cardinality_memory_limit = parse_bytes(
@@ -357,15 +398,14 @@
         )
 
         dsk, key = _category_stats(ddf, self._create_fit_options_from_columns(columns))
         return Delayed(key, dsk)
 
     def fit_finalize(self, categories):
         idx_count = 0
-
         for cat in categories:
             # this is a path
             self.categories[cat] = categories[cat]
             # check the argument
             if self.single_table:
                 cat_file_path = self.categories[cat]
                 idx_count, new_cat_file_path = run_on_worker(
@@ -379,27 +419,34 @@
 
     def process_vocabs(self, vocabs):
         """Process vocabs passed in by the user."""
         categories = {}
         if isinstance(vocabs, dict) and all(dispatch.is_series_object(v) for v in vocabs.values()):
             fit_options = self._create_fit_options_from_columns(list(vocabs.keys()))
             base_path = os.path.join(self.out_path, fit_options.stat_name)
+            num_buckets = fit_options.num_buckets
             os.makedirs(base_path, exist_ok=True)
             for col, vocab in vocabs.items():
-                vals = {col: vocab}
-                if vocab.iloc[0] is not None:
-                    with_empty = dispatch.add_to_series(vocab, [None]).reset_index()[0]
-                    vals = {col: with_empty}
-
-                save_path = os.path.join(base_path, f"unique.{col}.parquet")
-                col_df = dispatch.make_df(vals)
-                col_df.to_parquet(save_path)
-                categories[col] = save_path
+                col_name = _make_name(*col, sep=self.name_sep) if isinstance(col, tuple) else col
+                vals = {col_name: vocab}
+                oov_count = 1
+                if num_buckets:
+                    oov_count = (
+                        num_buckets if isinstance(num_buckets, int) else num_buckets[col_name]
+                    ) or 1
+                col_df = dispatch.make_df(vals).dropna()
+                col_df.index += NULL_OFFSET + oov_count
+                save_path = _save_encodings(col_df, base_path, col_name)
+                categories[col_name] = save_path
         elif isinstance(vocabs, dict) and all(isinstance(v, str) for v in vocabs.values()):
-            categories = vocabs
+            # TODO: How to deal with the fact that this file may be missing null and oov rows??
+            categories = {
+                (_make_name(*col, sep=self.name_sep) if isinstance(col, tuple) else col): path
+                for col, path in vocabs.items()
+            }
         else:
             error = """Unrecognized vocab type,
             please provide either a dictionary with paths to parquet files
             or a dictionary with pandas Series objects.
             """
             raise ValueError(error)
 
@@ -408,21 +455,22 @@
     def _create_fit_options_from_columns(self, columns) -> "FitOptions":
         return FitOptions(
             columns,
             [],
             [],
             self.out_path,
             self.freq_threshold,
-            self.tree_width,
+            self.split_out,
             self.on_host,
             concat_groups=self.encode_type == "joint",
             name_sep=self.name_sep,
             max_size=self.max_size,
             num_buckets=self.num_buckets,
             cardinality_memory_limit=self.cardinality_memory_limit,
+            split_every=self.split_every,
         )
 
     def set_storage_path(self, new_path, copy=False):
         self.categories = _copy_storage(self.categories, self.out_path, new_path, copy=copy)
         self.out_path = new_path
 
     @annotate("Categorify_transform", color="darkgreen", domain="nvt_python")
@@ -461,25 +509,29 @@
 
                 encoded = _encode(
                     use_name,
                     storage_name,
                     path,
                     df,
                     self.cat_cache,
-                    na_sentinel=self.na_sentinel,
                     freq_threshold=self.freq_threshold[name]
                     if isinstance(self.freq_threshold, dict)
                     else self.freq_threshold,
                     search_sorted=self.search_sorted,
                     buckets=self.num_buckets,
                     encode_type=self.encode_type,
                     cat_names=column_names,
                     max_size=self.max_size,
                     dtype=self.output_dtype,
-                    start_index=self.start_index,
+                    split_out=(
+                        self.split_out.get(storage_name, 1)
+                        if isinstance(self.split_out, dict)
+                        else self.split_out
+                    ),
+                    single_table=self.single_table,
                 )
                 new_df[name] = encoded
             except Exception as e:
                 raise RuntimeError(f"Failed to categorical encode column {name}") from e
 
         return new_df
 
@@ -514,15 +566,14 @@
             else self.num_buckets,
             "freq_threshold": self.freq_threshold[col_name]
             if isinstance(self.freq_threshold, dict)
             else self.freq_threshold,
             "max_size": self.max_size[col_name]
             if isinstance(self.max_size, dict)
             else self.max_size,
-            "start_index": self.start_index,
             "cat_path": target_category_path,
             "domain": {"min": 0, "max": cardinality - 1, "name": category_name},
             "embedding_sizes": {"cardinality": cardinality, "dimension": dimensions},
         }
 
         return col_schema.with_properties({**new_schema.properties, **to_add})
 
@@ -541,22 +592,15 @@
         parents_selector: ColumnSelector,
         dependencies_selector: ColumnSelector,
     ) -> ColumnSelector:
         self._validate_matching_cols(input_schema, parents_selector, "computing input selector")
         return parents_selector
 
     def get_embedding_sizes(self, columns):
-        return _get_embeddings_dask(
-            self.categories,
-            columns,
-            self.num_buckets,
-            self.freq_threshold,
-            self.max_size,
-            self.start_index,
-        )
+        return _get_embeddings_dask(self.categories, columns, self.num_buckets)
 
     def inference_initialize(self, columns, inference_config):
         # we don't currently support 'combo'
         if self.encode_type == "combo":
             warnings.warn("Falling back to unoptimized inference path for encode_type 'combo' ")
             return None
         import nvtabular_cpp
@@ -614,54 +658,173 @@
         return output
 
     single_hots = {k: v for k, v in output.items() if k not in multihot_columns}
     multi_hots = {k: v for k, v in output.items() if k in multihot_columns}
     return single_hots, multi_hots
 
 
-def _get_embeddings_dask(paths, cat_names, buckets=0, freq_limit=0, max_size=0, start_index=0):
+def _get_embeddings_dask(paths, cat_names, buckets=0):
     embeddings = {}
-    if isinstance(freq_limit, int):
-        freq_limit = {name: freq_limit for name in cat_names}
     if isinstance(buckets, int):
         buckets = {name: buckets for name in cat_names}
-    if isinstance(max_size, int):
-        max_size = {name: max_size for name in cat_names}
     for col in cat_names:
         path = paths.get(col)
-        num_rows = pq.ParquetFile(path).metadata.num_rows if path else 0
+        num_rows = OOV_OFFSET
+        if path:
+            for file_frag in pa_ds.dataset(path, format="parquet").get_fragments():
+                num_rows += file_frag.metadata.num_rows
         if isinstance(buckets, dict):
             bucket_size = buckets.get(col, 0)
         elif isinstance(buckets, int):
             bucket_size = buckets
         else:
-            bucket_size = 0
-
-        _has_frequency_limit = col in freq_limit and freq_limit[col] > 0
-        _has_max_size = col in max_size and max_size[col] > 0
-
-        if bucket_size and not _has_frequency_limit and not _has_max_size:
-            # pure hashing (no categorical lookup)
-            num_rows = bucket_size
-        else:
-            num_rows += bucket_size
-
-        num_rows += start_index
+            bucket_size = 1
+        num_rows += bucket_size
         embeddings[col] = _emb_sz_rule(num_rows)
     return embeddings
 
 
 def _emb_sz_rule(n_cat: int, minimum_size=16, maximum_size=512) -> int:
     return n_cat, min(max(minimum_size, round(1.6 * n_cat**0.56)), maximum_size)
 
 
 def _make_name(*args, sep="_"):
     return sep.join(args)
 
 
+def _to_parquet_dask_lazy(df, path, write_index=False):
+    # Write DataFrame data to parquet (lazily) with dask
+
+    # Check if we already have a dask collection
+    is_collection = isinstance(df, DaskDataFrame)
+
+    # Use `ddf.to_parquet` method
+    kwargs = {
+        "overwrite": True,
+        "compute": False,
+        "write_index": write_index,
+        "schema": None,
+    }
+    return (
+        df
+        if is_collection
+        else dispatch.convert_data(
+            df,
+            cpu=isinstance(df, pd.DataFrame),
+            to_collection=True,
+        )
+    ).to_parquet(path, **kwargs)
+
+
+def _save_encodings(
+    df,
+    base_path,
+    field_name,
+    preserve_index=False,
+    first_n=None,
+    freq_threshold=None,
+    oov_count=1,
+    null_size=None,
+):
+    # Write DataFrame data to parquet (eagerly) with dask
+
+    # Define paths
+    unique_path = "/".join([str(base_path), f"unique.{field_name}.parquet"])
+    meta_path = "/".join([str(base_path), f"meta.{field_name}.parquet"])
+
+    # Check if we already have a dask collection
+    is_collection = isinstance(df, DaskDataFrame)
+
+    # Create empty directory if it doesn't already exist
+    use_directory = is_collection and df.npartitions > 1
+    fs = get_fs_token_paths(unique_path, mode="wb")[0]
+    _path = fs._strip_protocol(unique_path)
+    if fs.isdir(_path) or fs.exists(_path):
+        fs.rm(_path, recursive=True)
+    if use_directory:
+        fs.mkdir(_path, exists_ok=True)
+
+    # Start tracking embedding metadata
+    record_size_meta = True
+    oov_size = 0
+    unique_count = 0
+    unique_size = 0
+
+    # Iterate over partitions and write to disk
+    size = oov_count + OOV_OFFSET  # Reserve null and oov buckets
+    for p, part in enumerate(df.partitions if is_collection else [df]):
+        local_path = "/".join([unique_path, f"part.{p}.parquet"]) if use_directory else unique_path
+        _df = _compute_sync(part) if is_collection else part
+        _len = len(_df)
+        if _len == 0:
+            continue
+
+        size_col = f"{field_name}_size"
+        if size_col not in _df.columns:
+            record_size_meta = False
+
+        if record_size_meta:
+            # Set number of rows allowed from this part
+            if first_n is not None:
+                first_n_local = first_n - size
+            else:
+                first_n_local = _len
+
+            # Update oov size
+            if first_n or freq_threshold:
+                removed = None
+                if freq_threshold:
+                    sizes = _df[size_col]
+                    removed = df[(sizes < freq_threshold) & (sizes > 0)]
+                    _df = _df[(sizes >= freq_threshold) | (sizes == 0)]
+                if first_n and _len > first_n_local:
+                    removed = _df.iloc[first_n_local:]
+                    _df = _df.iloc[:first_n_local]
+                if removed is not None:
+                    oov_size += removed[size_col].sum()
+                    _len = len(_df)
+
+            # Record unique-value metadata
+            unique_size += _df[size_col].sum()
+
+        if not preserve_index:
+            # If we are NOT writing the index of df,
+            # then make sure we are writing a "correct"
+            # index. Note that we avoid using ddf.to_parquet
+            # so that we can make sure the index is correct
+            _df.set_index(
+                pd.RangeIndex(
+                    start=size,
+                    stop=size + _len,
+                    step=1,
+                ),
+                drop=True,
+                inplace=True,
+            )
+
+        size += _len
+        unique_count += _len
+        _df.to_parquet(local_path, compression=None)
+        if first_n and size >= first_n:
+            break  # Ignore any remaining files
+
+    # Write encoding metadata
+    meta = {
+        "kind": ["pad", "null", "oov", "unique"],
+        "offset": [PAD_OFFSET, NULL_OFFSET, OOV_OFFSET, OOV_OFFSET + oov_count],
+        "num_indices": [1, 1, oov_count, unique_count],
+    }
+    if record_size_meta:
+        meta["num_observed"] = [0, null_size, oov_size, unique_size]
+    type(_df)(meta).to_parquet(meta_path)
+
+    # Return path to uniques
+    return unique_path
+
+
 @dataclass
 class FitOptions:
     """Contains options on how to fit statistics.
 
     Parameters
     ----------
         col_groups: list
@@ -673,49 +836,49 @@
             List of operations (sum/max/...) to perform on the grouped continuous columns
         out_path: str
             Where to write statistics in parquet format
         freq_limit: int or dict
             Categories with a count/frequency below this threshold will be
             omitted from the encoding and corresponding data will be mapped
             to the "null" category.
-        tree_width:
-           Tree width of the hash-based groupby reduction for each categorical column.
+        split_out:
+           Number of output partitions to use for each category in ``fit``.
         on_host:
             Whether to convert cudf data to pandas between tasks in the groupby reduction.
         stat_name:
             Name of statistic to use when writing out statistics
         concat_groups:
             Whether to use a 'joint' vocabulary between columns
         name_sep:
             Delimiter to use for concatenating columns into a string
         max_size:
             The maximum size of an embedding table
         num_buckets:
             If specified will also do hashing operation for values that would otherwise be mapped
             to as unknown (by freq_limit or max_size parameters)
-        start_index: int
-            The index to start mapping our output categorical values to.
         cardinality_memory_limit: int
             Suggested upper limit on categorical data containers.
+        split_every:
+            Number of adjacent partitions to reduce in each tree node.
     """
 
     col_groups: list
     agg_cols: list
     agg_list: list
     out_path: str
     freq_limit: Union[int, dict]
-    tree_width: Union[int, dict]
+    split_out: Union[int, dict]
     on_host: bool
     stat_name: str = "categories"
     concat_groups: bool = False
     name_sep: str = "-"
     max_size: Optional[Union[int, dict]] = None
     num_buckets: Optional[Union[int, dict]] = None
-    start_index: int = 0
     cardinality_memory_limit: Optional[int] = None
+    split_every: Optional[Union[int, dict]] = 8
 
     def __post_init__(self):
         if not isinstance(self.col_groups, ColumnSelector):
             self.col_groups = ColumnSelector(self.col_groups)
 
         col_selectors = []
         for cat_col_names in self.col_groups.grouped_names:
@@ -731,16 +894,70 @@
                 cat_col_selector = cat_col_names
 
             col_selectors.append(cat_col_selector)
 
         self.col_groups = col_selectors
 
 
+def _general_concat(
+    frames,
+    cardinality_memory_limit=False,
+    col_selector=None,
+    **kwargs,
+):
+    # Concatenate DataFrame or pa.Table objects
+    if isinstance(frames[0], pa.Table):
+        df = pa.concat_tables(frames, promote=True)
+        if (
+            cardinality_memory_limit
+            and col_selector is not None
+            and df.nbytes > cardinality_memory_limit
+        ):
+            # Before fully converting this pyarrow Table
+            # to a cudf DatFrame, we can reduce the memory
+            # footprint of `df`. Since the size of `df`
+            # depends on the cardinality of the features,
+            # and NOT on the partition size, the remaining
+            # logic in this function has an OOM-error risk
+            # (even with tiny partitions).
+            size_columns = []
+            for col in col_selector.names:
+                name = col + "_size"
+                if name in df.schema.names:
+                    # Convert this column alone to cudf,
+                    # and drop the field from df. Note that
+                    # we are only converting this column to
+                    # cudf to take advantage of fast `max`
+                    # performance.
+                    size_columns.append(dispatch.from_host(df.select([name])))
+                    df = df.drop([name])
+                    # Use numpy to calculate the "minimum"
+                    # dtype needed to capture the "size" column,
+                    # and cast the type
+                    typ = np.min_scalar_type(size_columns[-1][name].max() * 2)
+                    size_columns[-1][name] = size_columns[-1][name].astype(typ)
+            # Convert the remaining columns in df to cudf,
+            # and append the type-casted "size" columns
+            df = dispatch.concat_columns([dispatch.from_host(df)] + size_columns)
+        else:
+            # Empty DataFrame - No need for type-casting
+            df = dispatch.from_host(df)
+        return df
+    else:
+        # For now, if we are not concatenating in host memory,
+        # we will assume that reducing the memory footprint of
+        # "size" columns is not a priority. However, the same
+        # type-casting optimization can also be done for both
+        # pandas and cudf-backed data here.
+        return _concat(frames, **kwargs)
+
+
 @annotate("top_level_groupby", color="green", domain="nvt_python")
-def _top_level_groupby(df, options: FitOptions):
+def _top_level_groupby(df, options: FitOptions = None, spill=True):
+    assert options is not None
     sum_sq = "std" in options.agg_list or "var" in options.agg_list
     calculate_min = "min" in options.agg_list
     calculate_max = "max" in options.agg_list
     # Top-level operation for category-based groupby aggregations
     output = {}
     k = 0
     for i, cat_col_names in enumerate(options.col_groups):
@@ -802,51 +1019,68 @@
             _make_name(*(tuple(cat_col_selector.names) + name[1:]), sep=options.name_sep)
             if name[0] == cat_col_selector.names[0]
             else _make_name(*(tuple(cat_col_selector.names) + name), sep=options.name_sep)
             for name in gb.columns.to_flat_index()
         ]
         gb.reset_index(inplace=True, drop=False)
         del df_gb
+
+        # Extract null groups into gb_null
+        isnull = gb.isnull().any(axis=1)
+        gb_null = gb[~isnull]
+        gb = gb[isnull]
+        if not len(gb_null):
+            gb_null = None
+        del isnull
+
         # Split the result by the hash value of the categorical column
-        nsplits = options.tree_width[cat_col_selector_str]
+        nsplits = options.split_out[cat_col_selector_str]
         for j, split in shuffle_group(
             gb, cat_col_selector.names, 0, nsplits, nsplits, True, nsplits
         ).items():
-            if options.on_host and not is_cpu_object(split):
+            if gb_null is not None:
+                # Guarantee that the first split will contain null groups
+                split = _concat([gb_null, split], ignore_index=True)
+                gb_null = None
+            if spill and options.on_host and not is_cpu_object(split):
                 output[k] = split.to_arrow(preserve_index=False)
             else:
                 output[k] = split
             k += 1
         del gb
     return output
 
 
 @annotate("mid_level_groupby", color="green", domain="nvt_python")
-def _mid_level_groupby(dfs, col_selector: ColumnSelector, freq_limit_val, options: FitOptions):
+def _mid_level_groupby(dfs, col_selector: ColumnSelector, options: FitOptions, spill=True):
     if options.concat_groups and len(col_selector.names) > 1:
         col_selector = ColumnSelector([_make_name(*col_selector.names, sep=options.name_sep)])
 
-    if options.on_host and not is_cpu_object(dfs[0]):
-        # Construct gpu DataFrame from pyarrow data.
-        # `on_host=True` implies gpu-backed data.
-        df = pa.concat_tables(dfs, promote=True)
-        df = dispatch.from_host(df)
-    else:
-        df = _concat(dfs, ignore_index=True)
-
+    df = _general_concat(dfs, ignore_index=True)
     groups = df.groupby(col_selector.names, dropna=False)
     gb = groups.agg(
         {col: _get_aggregation_type(col) for col in df.columns if col not in col_selector.names}
     )
     gb.reset_index(drop=False, inplace=True)
 
+    if spill and options.on_host and not is_cpu_object(gb):
+        gb_pd = gb.to_arrow(preserve_index=False)
+        del gb
+        return gb_pd
+    return gb
+
+
+@annotate("bottom_level_groupby", color="green", domain="nvt_python")
+def _bottom_level_groupby(dfs, col_selector: ColumnSelector, options: FitOptions, spill=True):
+    gb = _mid_level_groupby(dfs, col_selector, options, spill=False)
+    if options.concat_groups and len(col_selector.names) > 1:
+        col_selector = ColumnSelector([_make_name(*col_selector.names, sep=options.name_sep)])
+
     name_count = _make_name(*(col_selector.names + ["count"]), sep=options.name_sep)
     name_size = _make_name(*(col_selector.names + ["size"]), sep=options.name_sep)
-    if options.freq_limit and not options.max_size:
-        gb = gb[gb[name_size] >= freq_limit_val]
 
     required = col_selector.names.copy()
     if "count" in options.agg_list:
         required.append(name_count)
     if "size" in options.agg_list:
         required.append(name_size)
     ddof = 1
@@ -891,15 +1125,15 @@
             if "std" in options.agg_list:
                 name_std = _make_name(
                     *(col_selector.names + [cont_col, "std"]), sep=options.name_sep
                 )
                 required.append(name_std)
                 gb[name_std] = np.sqrt(result)
 
-    if options.on_host and not is_cpu_object(gb[required]):
+    if spill and options.on_host and not is_cpu_object(gb[required]):
         gb_pd = gb[required].to_arrow(preserve_index=False)
         del gb
         return gb_pd
     return gb[required]
 
 
 def _get_aggregation_type(col):
@@ -907,58 +1141,23 @@
         return "min"
     elif col.endswith("_max"):
         return "max"
     else:
         return "sum"
 
 
-@annotate("write_gb_stats", color="green", domain="nvt_python")
-def _write_gb_stats(dfs, base_path, col_selector: ColumnSelector, options: FitOptions):
-    if options.concat_groups and len(col_selector) > 1:
-        col_selector = ColumnSelector([_make_name(*col_selector.names, sep=options.name_sep)])
-
-    rel_path = "cat_stats.%s.parquet" % (_make_name(*col_selector.names, sep=options.name_sep))
-    path = os.path.join(base_path, rel_path)
-    pwriter = None
-    if (not options.on_host or is_cpu_object(dfs[0])) and len(dfs):
-        # Want first non-empty df for schema (if there are any)
-        _d = next((df for df in dfs if len(df)), dfs[0])
-        pwriter = dispatch.parquet_writer_dispatch(_d, path=path, compression=None)
-
-    # Loop over dfs and append to file
-    # TODO: For high-cardinality columns, should support
-    #       Dask-based to_parquet call here (but would need to
-    #       support directory reading within dependent ops)
-    n_writes = 0
-    for df in dfs:
-        if len(df):
-            if options.on_host and not is_cpu_object(df):
-                # Use pyarrow - df is already a pyarrow table
-                if pwriter is None:
-                    pwriter = pq.ParquetWriter(path, df.schema, compression=None)
-                pwriter.write_table(df)
-            else:
-                # df is a cudf or pandas DataFrame
-                df.reset_index(drop=True, inplace=True)
-                pwriter.write_table(df)
-            n_writes += 1
-
-    # No data to write
-    if n_writes == 0:
-        raise RuntimeError("GroupbyStatistics result is empty.")
-
-    # Close writer and return path
-    if pwriter is not None:
-        pwriter.close()
-
-    return path
-
-
 @annotate("write_uniques", color="green", domain="nvt_python")
-def _write_uniques(dfs, base_path, col_selector: ColumnSelector, options: FitOptions):
+def _write_uniques(
+    dfs,
+    base_path,
+    col_selector: ColumnSelector,
+    options: FitOptions,
+    cpu: bool,
+    path: str = None,
+):
     """Writes out a dataframe to a parquet file.
 
     Parameters
     ----------
     dfs : DataFrame
     base_path : str
     col_selector :
@@ -974,311 +1173,378 @@
     path : str
         the path to the output parquet file.
 
     """
     if options.concat_groups and len(col_selector.names) > 1:
         col_selector = ColumnSelector([_make_name(*col_selector.names, sep=options.name_sep)])
 
-    if options.on_host:
-        # Construct gpu DataFrame from pyarrow data.
-        # `on_host=True` implies gpu-backed data,
-        # because CPU-backed data would have never
-        # been converted from pandas to pyarrow.
-        df = pa.concat_tables(dfs, promote=True)
-        if (
-            df.nbytes > options.cardinality_memory_limit
-            if options.cardinality_memory_limit
-            else False
-        ):
-            # Before fully converting this pyarrow Table
-            # to a cudf DatFrame, we can reduce the memory
-            # footprint of `df`. Since the size of `df`
-            # depends on the cardinality of the features,
-            # and NOT on the partition size, the remaining
-            # logic in this function has an OOM-error risk
-            # (even with tiny partitions).
-            size_columns = []
-            for col in col_selector.names:
-                name = col + "_size"
-                if name in df.schema.names:
-                    # Convert this column alone to cudf,
-                    # and drop the field from df. Note that
-                    # we are only converting this column to
-                    # cudf to take advantage of fast `max`
-                    # performance.
-                    size_columns.append(dispatch.from_host(df.select([name])))
-                    df = df.drop([name])
-                    # Use numpy to calculate the "minimum"
-                    # dtype needed to capture the "size" column,
-                    # and cast the type
-                    typ = np.min_scalar_type(size_columns[-1][name].max() * 2)
-                    size_columns[-1][name] = size_columns[-1][name].astype(typ)
-            # Convert the remaining columns in df to cudf,
-            # and append the type-casted "size" columns
-            df = dispatch.concat_columns([dispatch.from_host(df)] + size_columns)
-        else:
-            # Empty DataFrame - No need for type-casting
-            df = dispatch.from_host(df)
+    # Set max_emb_size
+    # This is the maximum number of rows we will write to
+    # the unique-value parquet files
+    col_name = col_selector.names[0]
+    max_emb_size = options.max_size
+    if max_emb_size:
+        max_emb_size = max_emb_size[col_name] if isinstance(max_emb_size, dict) else max_emb_size
+
+    # Set num_buckets
+    # This is the maximum number of indices
+    num_buckets = options.num_buckets
+    if num_buckets:
+        num_buckets = num_buckets if isinstance(num_buckets, int) else num_buckets[col_name]
+    oov_count = num_buckets or 1
+
+    # Set freq_threshold
+    # This is the minimum unique count for a distinct
+    # category to be included in the unique-value files
+    freq_threshold = options.freq_limit
+    if freq_threshold:
+        freq_threshold = (
+            freq_threshold if isinstance(freq_threshold, int) else freq_threshold[col_name]
+        )
+
+    # Sanity check
+    if max_emb_size and max_emb_size < oov_count + 2:
+        raise ValueError(
+            "`max_size` can never be less than the maximum of "
+            "`num_buckets + 2` and `3`, because we must always "
+            "reserve pad, null and at least 1 oov-bucket index."
+        )
+
+    null_size = None
+    if path:
+        # We have a parquet path to construct uniques from
+        # (rather than a list of DataFrame objects)
+        df = dispatch.read_dispatch(cpu=cpu, collection=True)(
+            path,
+            split_row_groups=False,
+        ).reset_index(drop=True)
+
+        # Check if we need to compute the DataFrame collection
+        # of unique values. For now, we can avoid doing this when
+        # we are not jointly encoding multiple columns
+        if simple := (len(col_selector.names) == 1 and df.npartitions > 1):
+            col_name = col_selector.names[0]
+            name_size = col_name + "_size"
+            has_size = name_size in df
+            try:
+                # Sort by col_name
+                df = df.sort_values(col_name, na_position="first")
+            except (NotImplementedError, TypeError):
+                # Dask-based sort failed - Need to compute first
+                simple = False
+
+        # At this point, `simple` may have changed from True to False
+        # if the backend library failed to sort by the target column.
+        if simple:
+            # Define the null row
+            def _drop_first_row(part, index):
+                return part.iloc[1:] if index == (0,) else part
+
+            null_row = df.head(1)
+            if null_row[col_name].iloc[:1].isnull().any():
+                df = df.map_partitions(_drop_first_row, BlockIndex((df.npartitions,)))
+                if has_size:
+                    null_size = null_row[name_size].iloc[0]
+            else:
+                null_size = 0
+
+            # Sort by size (without null and oov rows)
+            if has_size:
+                # Avoid using dask_cudf to calculate divisions
+                # (since it may produce too-few partitions)
+                df = df.sort_values(
+                    name_size,
+                    ascending=False,
+                    divisions=dd.shuffle._calculate_divisions(
+                        df, df[name_size], False, df.npartitions
+                    )[0][::-1],
+                )
+
+            unique_path = _save_encodings(
+                df,
+                base_path,
+                _make_name(*col_selector.names, sep=options.name_sep),
+                first_n=max_emb_size,
+                freq_threshold=freq_threshold,
+                oov_count=oov_count,
+                null_size=null_size,
+            )
+
+            # TODO: Delete temporary parquet file(s) now thet the final
+            # uniques are written to disk? (May not want to wait on deletion)
+            return unique_path
+
+        # If we have reached this point, we have a dask collection
+        # that must be computed before continuing
+        df = _compute_sync(df)
     else:
-        # For now, if we are not concatenating in host memory,
-        # we will assume that reducing the memory footprint of
-        # "size" columns is not a priority. However, the same
-        # type-casting optimization can also be done for both
-        # pandas and cudf-backed data here.
-        df = _concat(dfs, ignore_index=True)
+        # We have a list of DataFrame objects.
+        # Collect aggregation results into single frame
+        df = _general_concat(
+            dfs,
+            cardinality_memory_limit=options.cardinality_memory_limit,
+            col_selector=col_selector,
+            ignore_index=True,
+        )
 
     # Check if we should warn user that this Column is likely
     # to cause memory-pressure issues
     _df_size = df.memory_usage(deep=True, index=True).sum()
     if (_df_size > options.cardinality_memory_limit) if options.cardinality_memory_limit else False:
         warnings.warn(
             f"Category DataFrame (with columns: {df.columns}) is {_df_size} "
             f"bytes in size. This is large compared to the suggested "
             f"upper limit of {options.cardinality_memory_limit} bytes!"
             f"(12.5% of the total memory by default)"
         )
 
-    rel_path = "unique.%s.parquet" % (_make_name(*col_selector.names, sep=options.name_sep))
-    path = "/".join([base_path, rel_path])
     if len(df):
         # Make sure first category is Null.
         # Use ignore_index=True to avoid allocating memory for
         # an index we don't even need
         df = df.sort_values(col_selector.names, na_position="first", ignore_index=True)
-
         name_size_multi = "_".join(col_selector.names + ["size"])
-        if len(col_selector.names) > 1 and name_size_multi in df:
-            # Using "combo" encoding
-            df = _combo_encode(df, name_size_multi, col_selector, options)
-        else:
-            # Using (default) "joint" encoding
-            df = _joint_encode(df, col_selector, options)
+        has_size = name_size_multi in df
 
-        df.to_parquet(path, index=False, compression=None)
+        # Check if we already have a null row
+        has_nans = df[col_selector.names].iloc[0].transpose().isnull().all()
+        if hasattr(has_nans, "iloc"):
+            has_nans = has_nans[0]
+
+        if has_nans:
+            if has_size:
+                null_size = df[name_size_multi].iloc[0]
+            df = df.iloc[1:]
+        else:
+            null_size = 0
+        if has_size:
+            df = df.sort_values(name_size_multi, ascending=False, ignore_index=True)
+        df_write = df
     else:
         if hasattr(df, "convert_dtypes"):
             df = df.convert_dtypes()
         df_null = type(df)({c: [None] for c in col_selector.names})
         for c in col_selector.names:
             df_null[c] = df_null[c].astype(df[c].dtype)
-        df_null.to_parquet(path, index=False, compression=None)
+        df_write = df_null
 
+    unique_path = _save_encodings(
+        df_write,
+        base_path,
+        _make_name(*col_selector.names, sep=options.name_sep),
+        first_n=max_emb_size,
+        freq_threshold=freq_threshold,
+        oov_count=oov_count,
+        null_size=null_size,
+    )
     del df
-    return path
-
-
-@annotate("_combo_encode", color="green", domain="nvt_python")
-def _combo_encode(df, name_size_multi: str, col_selector: ColumnSelector, options: FitOptions):
-    # Combo-encoding utility (used by _write_uniques)
-
-    # Account for max_size and num_buckets
-    if options.max_size:
-        max_emb_size = options.max_size
-        if isinstance(options.max_size, dict):
-            raise NotImplementedError(
-                "Cannot specify max_size as a dictionary for 'combo' encoding."
-            )
-        if options.num_buckets:
-            if isinstance(options.num_buckets, dict):
-                raise NotImplementedError(
-                    "Cannot specify num_buckets as a dictionary for 'combo' encoding."
-                )
-            nlargest = max_emb_size - options.num_buckets - 1
-        else:
-            nlargest = max_emb_size - 1
-
-        if nlargest <= 0:
-            raise ValueError("`nlargest` cannot be 0 or negative")
-
-        if nlargest < len(df):
-            # sort based on count (name_size_multi column)
-            df = df.nlargest(n=nlargest, columns=name_size_multi)
-
-    # Deal with nulls
-    has_nans = df[col_selector.names].iloc[0].transpose().isnull().all()
-    if hasattr(has_nans, "iloc"):
-        has_nans = has_nans[0]
-    if not has_nans:
-        null_data = {col: nullable_series([None], df, df[col].dtype) for col in col_selector.names}
-        null_data[name_size_multi] = [0]
-        null_df = type(df)(null_data)
-        df = _concat([null_df, df], ignore_index=True)
-
-    return df
-
-
-@annotate("_joint_encode", color="green", domain="nvt_python")
-def _joint_encode(df, col_selector: ColumnSelector, options: FitOptions):
-    # Joint-encoding utility (used by _write_uniques)
-
-    new_cols = {}
-    nulls_missing = False
-    for col in col_selector.names:
-        name_size = col + "_size"
-        null_size = 0
-        # Set null size if first element in `col` is
-        # null, and the `size` aggregation is known
-        if name_size in df and df[col].iloc[:1].isnull().any():
-            null_size = df[name_size].iloc[0]
-        if options.max_size:
-            max_emb_size = options.max_size
-            if isinstance(options.max_size, dict):
-                max_emb_size = max_emb_size[col]
-            if options.num_buckets:
-                if isinstance(options.num_buckets, int):
-                    nlargest = max_emb_size - options.num_buckets - 1
-                else:
-                    nlargest = max_emb_size - options.num_buckets[col] - 1
-            else:
-                nlargest = max_emb_size - 1
-
-            if nlargest <= 0:
-                raise ValueError("`nlargest` cannot be 0 or negative")
-
-            if nlargest < len(df) and name_size in df:
-                # remove NAs from column, we have na count from above.
-                df = df.dropna()  # TODO: This seems dangerous - Check this
-                # sort based on count (name_size column)
-                df = df.nlargest(n=nlargest, columns=name_size)
-                new_cols[col] = _concat(
-                    [nullable_series([None], df, df[col].dtype), df[col]],
-                    ignore_index=True,
-                )
-                new_cols[name_size] = _concat(
-                    [nullable_series([null_size], df, df[name_size].dtype), df[name_size]],
-                    ignore_index=True,
-                )
-                # recreate newly "count" ordered df
-                df = type(df)(new_cols)
-        if not dispatch.series_has_nulls(df[col]):
-            if name_size in df:
-                df = df.sort_values(name_size, ascending=False, ignore_index=True)
-
-            nulls_missing = True
-            new_cols[col] = _concat(
-                [nullable_series([None], df, df[col].dtype), df[col]],
-                ignore_index=True,
-            )
-            if name_size in df:
-                new_cols[name_size] = _concat(
-                    [nullable_series([null_size], df, df[name_size].dtype), df[name_size]],
-                    ignore_index=True,
-                )
-
-        else:
-            # ensure None aka "unknown" stays at index 0
-            if name_size in df:
-                df_0 = df.iloc[0:1]
-                df_1 = df.iloc[1:].sort_values(name_size, ascending=False, ignore_index=True)
-                df = _concat([df_0, df_1])
-            new_cols[col] = df[col].copy(deep=False)
-
-            if name_size in df:
-                new_cols[name_size] = df[name_size].copy(deep=False)
-    if nulls_missing:
-        return type(df)(new_cols)
-    return df
+    del df_write
+    return unique_path
 
 
 def _finish_labels(paths, cols):
     return {col: paths[i] for i, col in enumerate(cols)}
 
 
 def _groupby_to_disk(ddf, write_func, options: FitOptions):
     if not options.col_groups:
-        return {}
+        raise ValueError("no column groups to aggregate")
 
     if options.concat_groups:
         if options.agg_list and not set(options.agg_list).issubset({"count", "size"}):
             raise ValueError(
                 "Cannot use concat_groups=True with aggregations other than count and size"
             )
         if options.agg_cols:
             raise ValueError("Cannot aggregate continuous-column stats with concat_groups=True")
 
-    # Update tree_width
-    tw = {}
+    # Update split_out and split_every
+    so, se = {}, {}
     for col in options.col_groups:
         col = [col] if isinstance(col, str) else col
         if isinstance(col, tuple):
             col = list(col)
-
         col_str = _make_name(*col.names, sep=options.name_sep)
-        if options.tree_width is None:
-            tw[col_str] = 8
-        elif isinstance(options.tree_width, int):
-            tw[col_str] = options.tree_width
-        else:
-            tw[col_str] = options.tree_width.get(col_str, None) or 8
-    options.tree_width = tw
+
+        for _d, _opt, _default in [
+            (so, options.split_out, 1),
+            (se, options.split_every, 8),
+        ]:
+            if _opt is None:
+                _d[col_str] = _default
+            elif isinstance(_opt, int):
+                _d[col_str] = _opt
+            else:
+                _d[col_str] = _opt.get(col_str, _default)
+
+    options.split_out = so
+    options.split_every = se
 
     # Make dedicated output directory for the categories
     fs = get_fs_token_paths(options.out_path)[0]
     out_path = fs.sep.join([options.out_path, options.stat_name])
     fs.mkdirs(out_path, exist_ok=True)
 
     dsk = {}
     token = tokenize(
         ddf,
         options.col_groups,
         options.out_path,
         options.freq_limit,
-        options.tree_width,
+        options.split_out,
+        options.split_every,
         options.on_host,
     )
-    level_1_name = "level_1-" + token
     split_name = "split-" + token
-    level_2_name = "level_2-" + token
-    level_3_name = "level_3-" + token
+    reduce_1_name = "reduce_1-" + token
+    reduce_3_name = "reduce_3-" + token
     finalize_labels_name = options.stat_name + "-" + token
+
+    # Use map_partitions to improve task fusion
+    grouped = ddf.to_bag(format="frame").map_partitions(
+        _top_level_groupby, options=options, token="level_1"
+    )
+    _grouped_meta = _top_level_groupby(ddf._meta, options=options)
+    _grouped_meta_col = {}
+
+    dsk_split = defaultdict(dict)
     for p in range(ddf.npartitions):
-        dsk[(level_1_name, p)] = (_top_level_groupby, (ddf._name, p), options)
         k = 0
         for c, col in enumerate(options.col_groups):
             col = [col] if isinstance(col, str) else col
             col_str = _make_name(*col.names, sep=options.name_sep)
-            for s in range(options.tree_width[col_str]):
-                dsk[(split_name, p, c, s)] = (getitem, (level_1_name, p), k)
+            _grouped_meta_col[c] = _grouped_meta[k]
+            for s in range(options.split_out[col_str]):
+                dsk_split[c][(split_name, p, c, s)] = (getitem, (grouped.name, p), k)
                 k += 1
 
     col_groups_str = []
+    col_group_frames = []
     for c, col in enumerate(options.col_groups):
         col = [col] if isinstance(col, str) else col
         col_str = _make_name(*col.names, sep=options.name_sep)
         col_groups_str.append(col_str)
-        freq_limit_val = None
-        if options.freq_limit:
-            freq_limit_val = (
-                options.freq_limit[col_str]
-                if isinstance(options.freq_limit, dict)
-                else options.freq_limit
-            )
-        for s in range(options.tree_width[col_str]):
-            dsk[(level_2_name, c, s)] = (
-                _mid_level_groupby,
-                [(split_name, p, c, s) for p in range(ddf.npartitions)],
-                col,
-                freq_limit_val,
-                options,
-            )
+        reduce_2_name = f"reduce_2-{c}-" + token
+        for s in range(options.split_out[col_str]):
+            split_every = options.split_every[col_str]
+            parts = ddf.npartitions
+            widths = [parts]
+            while parts > 1:
+                parts = math.ceil(parts / split_every)
+                widths.append(int(parts))
+            height = len(widths)
+            if height >= 2:
+                # Loop over reduction levels
+                for depth in range(1, height):
+                    # Loop over reduction groups
+                    for group in range(widths[depth]):
+                        # Calculate inputs for the current group
+                        p_max = widths[depth - 1]
+                        lstart = split_every * group
+                        lstop = min(lstart + split_every, p_max)
+                        if depth == 1:
+                            # Input nodes are from input layer
+                            input_keys = [(split_name, p, c, s) for p in range(lstart, lstop)]
+                        else:
+                            # Input nodes are tree-reduction nodes
+                            input_keys = [
+                                (reduce_1_name, p, c, s, depth - 1) for p in range(lstart, lstop)
+                            ]
+
+                        # Define task
+                        if depth == height - 1:
+                            # Final Node
+                            assert (
+                                group == 0
+                            ), f"group = {group}, not 0 for final tree reduction task"
+                            dsk_split[c][(reduce_2_name, s)] = (
+                                _bottom_level_groupby,
+                                input_keys,
+                                col,
+                                options,
+                                False,
+                            )
+                        else:
+                            # Intermediate Node
+                            dsk_split[c][(reduce_1_name, group, c, s, depth)] = (
+                                _mid_level_groupby,
+                                input_keys,
+                                col,
+                                options,
+                            )
+            else:
+                # Deal with single-partition case
+                dsk_split[c][(reduce_2_name, s)] = (
+                    _bottom_level_groupby,
+                    [(split_name, 0, c, s)],
+                    col,
+                    options,
+                    False,
+                )
 
-        dsk[(level_3_name, c)] = (
-            write_func,
-            [(level_2_name, c, s) for s in range(options.tree_width[col_str])],
-            out_path,
+        # Make DataFrame collection for column-group result
+        _meta = _bottom_level_groupby(
+            [_grouped_meta_col[c]],
             col,
             options,
+            spill=False,
         )
+        _divisions = (None,) * (options.split_out[col_str] + 1)
+        graph = HighLevelGraph.from_collections(reduce_2_name, dsk_split[c], dependencies=[grouped])
+        col_group_frames.append(new_dd_object(graph, reduce_2_name, _meta, _divisions))
+
+        # Write data to (possibly temporary) parquet files
+        cpu = isinstance(col_group_frames[-1]._meta, pd.DataFrame)
+        if write_func is None:
+            # Write results directly to disk, and use
+            # a final "barrier" task
+            if options.concat_groups and len(col) > 1:
+                col_selector = ColumnSelector([_make_name(*col.names, sep=options.name_sep)])
+            else:
+                col_selector = col
+            rel_path = "cat_stats.%s.parquet" % (
+                _make_name(*col_selector.names, sep=options.name_sep)
+            )
+            path = os.path.join(out_path, rel_path)
+            col_group_frames[-1] = _to_parquet_dask_lazy(col_group_frames[-1], path)
+            # Barrier-only task
+            dsk[(reduce_3_name, c)] = (
+                lambda keys, path: path,
+                col_group_frames[-1].__dask_keys__(),
+                path,
+            )
+        else:
+            # Possibly write data to temporary parquet files,
+            # and perform write operation(s) in final `write_func` task
+            assert callable(write_func)
+            if col_group_frames[-1].npartitions > 1 and write_func.__name__ == "_write_uniques":
+                path = os.path.join(out_path, f"tmp.uniques.{col_str}")
+                col_group_frames[-1] = _to_parquet_dask_lazy(col_group_frames[-1], path)
+            else:
+                path = None
+            # Write + barrier task
+            dsk[(reduce_3_name, c)] = (
+                write_func,
+                col_group_frames[-1].__dask_keys__(),
+                out_path,
+                col,
+                options,
+                cpu,
+                path,
+            )
 
+    # Tie everything together into a graph with a single output key
     dsk[finalize_labels_name] = (
         _finish_labels,
-        [(level_3_name, c) for c, col in enumerate(options.col_groups)],
+        [(reduce_3_name, c) for c, col in enumerate(options.col_groups)],
         col_groups_str,
     )
-    graph = HighLevelGraph.from_collections(finalize_labels_name, dsk, dependencies=[ddf])
+    graph = HighLevelGraph.from_collections(
+        finalize_labels_name, dsk, dependencies=col_group_frames
+    )
     return graph, finalize_labels_name
 
 
 def _category_stats(ddf, options: FitOptions):
     # Check if we only need categories
     if options.agg_cols == [] and options.agg_list == []:
         options.agg_list = ["size"]
@@ -1286,46 +1552,44 @@
 
     # Otherwise, getting category-statistics
     if isinstance(options.agg_cols, str):
         options.agg_cols = [options.agg_cols]
     if options.agg_list == []:
         options.agg_list = ["count"]
 
-    return _groupby_to_disk(ddf, _write_gb_stats, options)
+    return _groupby_to_disk(ddf, None, options)
 
 
 def _encode(
     name,
     storage_name,
     path,
     df,
     cat_cache,
-    na_sentinel=-1,
     freq_threshold=0,
     search_sorted=False,
     buckets=None,
     encode_type="joint",
     cat_names=None,
     max_size=0,
     dtype=None,
-    start_index=0,
+    split_out=1,
+    single_table=False,
 ):
     """The _encode method is responsible for transforming a dataframe by taking the written
     out vocabulary file and looking up values to translate inputs to numeric
     outputs.
 
     Parameters
     ----------
     name :
     storage_name : dict
     path : str
     df : DataFrame
     cat_cache :
-    na_sentinel : int
-        Sentinel for NA value. Defaults to -1.
     freq_threshold :  int
         Categories with a count or frequency below this threshold will
         be omitted from the encoding and corresponding data will be
         mapped to the "Null" category. Defaults to 0.
     search_sorted :
         Defaults to False.
     buckets :
@@ -1334,118 +1598,214 @@
         Defaults to "joint".
     cat_names :
         Defaults to None.
     max_size :
         Defaults to 0.
     dtype :
         Defaults to None.
-    start_index :  int
-        The index to start outputting categorical values to. This is useful
-        to, for instance, reserve an initial segment of non-negative
-        integers for out-of-vocabulary or other special values. Defaults
-        to 1.
 
     Returns
     -------
     labels : numpy ndarray or Pandas Series
 
     """
     if isinstance(buckets, int):
         buckets = {name: buckets for name in cat_names}
-    # this is to apply freq_hashing logic
-    if max_size:
-        freq_threshold = 1
     value = None
     selection_l = ColumnSelector(name if isinstance(name, list) else [name])
     selection_r = ColumnSelector(name if isinstance(name, list) else [storage_name])
     list_col = is_list_col(selection_l, df)
+
+    # Find number of oov buckets
+    if buckets and storage_name in buckets:
+        num_oov_buckets = buckets[storage_name]
+        search_sorted = False
+    else:
+        num_oov_buckets = 1
+
     if path:
-        read_pq_func = dispatch.read_parquet_dispatch(df)
-        if cat_cache is not None:
+        read_pq_func = dispatch.read_dispatch(
+            df,
+            fmt="parquet",
+            collection=split_out > 1,
+        )
+        if cat_cache is not None and split_out == 1:
             cat_cache = (
                 cat_cache if isinstance(cat_cache, str) else cat_cache.get(storage_name, "disk")
             )
             if len(df):
                 with get_worker_cache("cats") as cache:
                     value = fetch_table_data(
                         cache,
                         path,
                         columns=selection_r.names,
                         cache=cat_cache,
                         cats_only=True,
                         reader=read_pq_func,
                     )
+                    if len(value) and value["labels"].iloc[0] < OOV_OFFSET + num_oov_buckets:
+                        # See: https://github.com/rapidsai/cudf/issues/12837
+                        value["labels"] += OOV_OFFSET + num_oov_buckets
         else:
             value = read_pq_func(  # pylint: disable=unexpected-keyword-arg
-                path, columns=selection_r.names
+                path,
+                columns=selection_r.names,
+                **({"split_row_groups": False} if split_out > 1 else {}),
             )
-            value.index.name = "labels"
-            value.reset_index(drop=False, inplace=True)
+
+            value.index = value.index.rename("labels")
+            if split_out > 1:
+                value = value.reset_index(drop=False)
+                if type(df).__module__.split(".")[0] == "cudf":
+                    # `cudf.read_parquet` may drop the RangeIndex, so we need
+                    # to use the parquet metadata to set a proper RangeIndex.
+                    # We can avoid this workaround for cudf>=23.04
+                    # (See: https://github.com/rapidsai/cudf/issues/12837)
+                    ranges, size = [], OOV_OFFSET + num_oov_buckets
+                    for file_frag in pa_ds.dataset(path, format="parquet").get_fragments():
+                        part_size = file_frag.metadata.num_rows
+                        ranges.append((size, size + part_size))
+                        size += part_size
+                    value["labels"] = dd.from_map(lambda r: pd.RangeIndex(*r), ranges)
+            else:
+                value.reset_index(drop=False, inplace=True)
 
     if value is None:
         value = type(df)()
         for c in selection_r.names:
             typ = df[selection_l.names[0]].dtype if len(selection_l.names) == 1 else df[c].dtype
             value[c] = nullable_series([None], df, typ)
-        value.index.name = "labels"
+        value.index = value.index.rename("labels")
         value.reset_index(drop=False, inplace=True)
 
-    if not search_sorted:
+    use_collection = isinstance(value, DaskDataFrame)
+    if use_collection and value.npartitions == 1:
+        # Use simple merge for single-partition case
+        value = _compute_sync(value)
+        use_collection = False
+
+    # Determine encoding offsets
+    null_encoding_offset = value["labels"].head(1).iloc[0] if single_table else NULL_OFFSET
+    bucket_encoding_offset = null_encoding_offset + 1  # 2 (if not single_table)
+    distinct_encoding_offset = bucket_encoding_offset + num_oov_buckets
+
+    # Determine indices of "real" null values
+    # (these will always be encoded to `1`)
+    expr = df[selection_l.names[0]].isna()
+    for _name in selection_l.names[1:]:
+        expr = expr & df[_name].isna()
+    nulls = df[expr].index.values
+
+    if use_collection or not search_sorted:
         if list_col:
             codes = dispatch.flatten_list_column(df[selection_l.names[0]])
             codes["order"] = dispatch.arange(len(codes), like_df=df)
         else:
             # We go into this case
             codes = type(df)({"order": dispatch.arange(len(df), like_df=df)}, index=df.index)
 
         for cl, cr in zip(selection_l.names, selection_r.names):
             if isinstance(df[cl].dropna().iloc[0], (np.ndarray, list)):
                 ser = df[cl].copy()
                 codes[cl] = dispatch.flatten_list_column_values(ser).astype(value[cr].dtype)
             else:
                 codes[cl] = df[cl].copy().astype(value[cr].dtype)
 
+        indistinct = bucket_encoding_offset
         if buckets and storage_name in buckets:
-            na_sentinel = _hash_bucket(df, buckets, selection_l.names, encode_type=encode_type)
+            # apply hashing for "infrequent" categories
+            indistinct = (
+                _hash_bucket(df, buckets, selection_l.names, encode_type=encode_type)
+                + bucket_encoding_offset
+            )
+
+            if use_collection:
+                # Manual broadcast merge
+                merged_df = _concat(
+                    [
+                        codes.merge(
+                            _compute_sync(part),
+                            left_on=selection_l.names,
+                            right_on=selection_r.names,
+                            how="left",
+                        ).dropna(subset=["labels"])
+                        for part in value.partitions
+                    ],
+                    ignore_index=False,
+                ).sort_values("order")
+            else:
+                merged_df = codes.merge(
+                    value, left_on=selection_l.names, right_on=selection_r.names, how="left"
+                ).sort_values("order")
 
-        # apply frequency hashing
-        if freq_threshold and buckets and storage_name in buckets:
-            merged_df = codes.merge(
-                value, left_on=selection_l.names, right_on=selection_r.names, how="left"
-            ).sort_values("order")
             merged_df.reset_index(drop=True, inplace=True)
-            max_id = merged_df["labels"].max()
-            merged_df["labels"].fillna(
-                df._constructor_sliced(na_sentinel + max_id + 1), inplace=True
-            )
-            labels = merged_df["labels"].values
-        # only do hashing
-        elif buckets and storage_name in buckets:
-            labels = na_sentinel
-        # no hashing
+            if len(merged_df) < len(codes):
+                # Missing nulls
+                labels = df._constructor_sliced(indistinct)
+                labels.iloc[merged_df["order"]] = merged_df["labels"]
+                labels = labels.values
+            else:
+                merged_df["labels"].fillna(df._constructor_sliced(indistinct), inplace=True)
+                labels = merged_df["labels"].values
         else:
-            na_sentinel = 0
-            labels = codes.merge(
-                value, left_on=selection_l.names, right_on=selection_r.names, how="left"
-            ).sort_values("order")["labels"]
-            labels.fillna(na_sentinel, inplace=True)
+            # no hashing
+            if use_collection:
+                # Manual broadcast merge
+                merged_df = _concat(
+                    [
+                        codes.merge(
+                            _compute_sync(part),
+                            left_on=selection_l.names,
+                            right_on=selection_r.names,
+                            how="left",
+                        ).dropna(subset=["labels"])
+                        for part in value.partitions
+                    ],
+                    ignore_index=True,
+                )
+                if len(merged_df) < len(codes):
+                    # Missing nulls
+                    labels = codes._constructor_sliced(
+                        np.full(
+                            len(codes),
+                            indistinct,
+                            like=merged_df["labels"].values,
+                        ),
+                    )
+                    labels.iloc[merged_df["order"]] = merged_df["labels"]
+                else:
+                    labels = merged_df.sort_values("order")["labels"].reset_index(drop=True)
+            else:
+                labels = codes.merge(
+                    value, left_on=selection_l.names, right_on=selection_r.names, how="left"
+                ).sort_values("order")["labels"]
+            labels.fillna(indistinct, inplace=True)
             labels = labels.values
     else:
         # Use `searchsorted` if we are using a "full" encoding
         if list_col:
-            labels = value[selection_r.names].searchsorted(
-                df[selection_l.names[0]].list.leaves, side="left", na_position="first"
+            labels = (
+                value[selection_r.names].searchsorted(
+                    df[selection_l.names[0]].list.leaves, side="left", na_position="first"
+                )
+                + distinct_encoding_offset
             )
         else:
-            labels = value[selection_r.names].searchsorted(
-                df[selection_l.names], side="left", na_position="first"
+            labels = (
+                value[selection_r.names].searchsorted(
+                    df[selection_l.names], side="left", na_position="first"
+                )
+                + distinct_encoding_offset
             )
-        labels[labels >= len(value[selection_r.names])] = na_sentinel
+        labels[labels >= len(value[selection_r.names])] = bucket_encoding_offset
 
-    labels = labels + start_index
+    # Make sure nulls are encoded to `null_encoding_offset`
+    # (This should be `1` in most casese)
+    if len(nulls):
+        labels[nulls] = null_encoding_offset
 
     if list_col:
         labels = dispatch.encode_list_column(df[selection_l.names[0]], labels, dtype=dtype)
     elif dtype:
         labels = labels.astype(dtype, copy=False)
 
     return labels
@@ -1497,29 +1857,64 @@
 
 
 def _copy_storage(existing_stats, existing_path, new_path, copy):
     """helper function to copy files to a new storage location"""
     existing_fs = get_fs_token_paths(existing_path)[0]
     new_fs = get_fs_token_paths(new_path)[0]
     new_locations = {}
+
     for column, existing_file in existing_stats.items():
         new_file = existing_file.replace(str(existing_path), str(new_path))
         if copy and new_file != existing_file:
             new_fs.makedirs(os.path.dirname(new_file), exist_ok=True)
-            with new_fs.open(new_file, "wb") as output:
-                output.write(existing_fs.open(existing_file, "rb").read())
+
+            # For some ops, the existing "file" is a directory containing `part.N.parquet` files.
+            # In that case, new_file is actually a directory and we will iterate through the "part"
+            # files and copy them individually
+            if os.path.isdir(existing_file):
+                new_fs.makedirs(new_file, exist_ok=True)
+                for existing_file_part in existing_fs.ls(existing_file):
+                    new_file_part = os.path.join(new_file, os.path.basename(existing_file_part))
+                    with new_fs.open(new_file_part, "wb") as output:
+                        output.write(existing_fs.open(existing_file_part, "rb").read())
+            else:
+                with new_fs.open(new_file, "wb") as output:
+                    output.write(existing_fs.open(existing_file, "rb").read())
 
         new_locations[column] = new_file
 
     return new_locations
 
 
 def _reset_df_index(col_name, cat_file_path, idx_count):
-    cat_df = dispatch.read_parquet_dispatch(None)(cat_file_path)
+    cat_df = _compute_sync(dispatch.read_dispatch(collection=True)(cat_file_path))
     # change indexes for category
-    cat_df.index += idx_count
+    cat_df.index = cat_df.index + idx_count
     # update count
     idx_count += cat_df.shape[0]
     # save the new indexes in file
-    new_cat_file_path = Path(cat_file_path).parent / f"unique.{col_name}.all.parquet"
-    cat_df.to_parquet(new_cat_file_path)
+    new_cat_file_path = _save_encodings(
+        cat_df,
+        Path(cat_file_path).parent,
+        col_name,
+        preserve_index=True,
+    )
     return idx_count, new_cat_file_path
+
+
+def _deprecate_tree_width(tree_width):
+    # Warn user if tree_width is specified
+    if tree_width is not None:
+        warnings.warn(
+            "The tree_width argument is now deprecated, and will be ignored. "
+            "Please use split_out and split_every.",
+            FutureWarning,
+        )
+
+
+def _compute_sync(collection):
+    # Simple utility to compute a dask collection with
+    # a synchronous scheduler (and to catch warnings
+    # that are intended for users doing this by accident)
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", message="Running on a single-machine scheduler.*")
+        return collection.compute(scheduler="synchronous")
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/clip.py` & `nvtabular-23.6.0/nvtabular/ops/clip.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/column_similarity.py` & `nvtabular-23.6.0/nvtabular/ops/column_similarity.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/data_stats.py` & `nvtabular-23.6.0/nvtabular/ops/data_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import dask.dataframe as dd
 import numpy as np
 
 from merlin.core.dispatch import DataFrameType, annotate
+from merlin.dag.ops.stat_operator import StatOperator
 from nvtabular.ops.moments import _custom_moments
 from nvtabular.ops.operator import ColumnSelector, Operator
-from nvtabular.ops.stat_operator import StatOperator
 
 
 class DataStats(StatOperator):
     """DataStats calculates statistics for each column in a Dataset
 
     Calculates statistics for each column, including things like:
      * the min and max value
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/difference_lag.py` & `nvtabular-23.6.0/nvtabular/ops/difference_lag.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/drop_low_cardinality.py` & `nvtabular-23.6.0/nvtabular/ops/drop_low_cardinality.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 class DropLowCardinality(Operator):
     """
     DropLowCardinality drops low cardinality categorical columns. This requires the
     cardinality of these columns to be known in the schema - for instance by
     first encoding these columns using Categorify.
     """
 
-    def __init__(self, min_cardinality=2):
+    def __init__(self, min_cardinality=4):
         super().__init__()
         self.min_cardinality = min_cardinality
 
     def transform(self, col_selector: ColumnSelector, df: DataFrameType) -> DataFrameType:
         """
         Selects all non-categorical columns and any categorical columns
         of at least the minimum cardinality from the dataframe.
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/dropna.py` & `nvtabular-23.6.0/nvtabular/ops/dropna.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/fill.py` & `nvtabular-23.6.0/nvtabular/ops/fill.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import dask.dataframe as dd
 import numpy as np
 
 from merlin.core.dispatch import DataFrameType, annotate
+from merlin.dag.ops.stat_operator import StatOperator
 from nvtabular.ops.operator import ColumnSelector, Operator
-from nvtabular.ops.stat_operator import StatOperator
 
 
 class FillMissing(Operator):
     """
     This operation replaces missing values with a constant pre-defined value
 
     Example usage::
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/filter.py` & `nvtabular-23.6.0/nvtabular/ops/filter.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/groupby.py` & `nvtabular-23.6.0/nvtabular/ops/groupby.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/hash_bucket.py` & `nvtabular-23.6.0/nvtabular/ops/hash_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
            feature_a  feature_b
         0         90         11
         1         70         40
         2         52          9
 
     If you would like to do frequency capping or frequency hashing,
     you should use Categorify op instead. See
-    `Categorify op <https://github.com/NVIDIA/NVTabular/blob/main/nvtabular/ops/categorify.py#L43>`_
+    `Categorify op <https://github.com/NVIDIA/NVTabular/blob/stable/nvtabular/ops/categorify.py>`_
     for example usage.
 
 
     Parameters
     ----------
     num_buckets : int or dictionary:{column: num_hash_buckets}
         Column-wise modulo to apply after hash function. Note that this
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/hashed_cross.py` & `nvtabular-23.6.0/nvtabular/ops/hashed_cross.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/join_external.py` & `nvtabular-23.6.0/nvtabular/ops/join_external.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/join_groupby.py` & `nvtabular-23.6.0/nvtabular/ops/join_groupby.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,27 +9,26 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import dask.dataframe as dd
 import numpy as np
 import pandas as pd
 from dask.delayed import Delayed
 
-import nvtabular as nvt
 from merlin.core.dispatch import DataFrameType, arange, concat_columns, read_parquet_dispatch
+from merlin.dag import Node
+from merlin.dag.ops.stat_operator import StatOperator
 from merlin.dtypes.shape import DefaultShapes
 from merlin.schema import Schema
 from nvtabular.ops import categorify as nvt_cat
 from nvtabular.ops.operator import ColumnSelector, Operator
-from nvtabular.ops.stat_operator import StatOperator
 
 AGG_DTYPES = {
     "count": np.int32,
     "std": np.float32,
     "var": np.float32,
     "mean": np.float32,
 }
@@ -59,20 +58,23 @@
         The continuous columns to calculate statistics for
         (for each unique group in each column in `columns`).
     stats : list of str, default []
         List of statistics to calculate for each unique group. Note
         that "count" corresponds to the group itself, while all
         other statistics correspond to a specific continuous column.
         Supported statistics include ["count", "sum", "mean", "std", "var"].
-    tree_width : dict or int, optional
-        Tree width of the hash-based groupby reduction for each categorical
-        column. High-cardinality columns may require a large `tree_width`,
-        while low-cardinality columns can likely use `tree_width=1`.
+    split_out : dict or int, optional
+        Number of files needed to store the final result of each groupby
+        reduction. High-cardinality groups may require a large `split_out`,
+        while low-cardinality columns can likely use `split_out=1` (default).
         If passing a dict, each key and value should correspond to the column
-        name and width, respectively. The default value is 8 for all columns.
+        name and value, respectively. The default value is 1 for all columns.
+    split_every : dict or int, optional
+        Number of adjacent partitions to aggregate in each tree-reduction
+        node. The default value is 8 for all columns.
     cat_cache: ToDo Describe
         TEXT
     out_path : str, optional
         Root directory where groupby statistics will be written out in
         parquet format.
     on_host : bool, default True
         Whether to convert cudf data to pandas between tasks in the hash-based
@@ -84,34 +86,38 @@
         for multi-column groups.
     """
 
     def __init__(
         self,
         cont_cols=None,
         stats=("count",),
-        tree_width=None,
+        split_out=None,
+        split_every=None,
         cat_cache="host",
         out_path=None,
         on_host=True,
         name_sep="_",
+        tree_width=None,
     ):
         super().__init__()
 
         self.storage_name = {}
         self.name_sep = name_sep
         self.stats = stats
-        self.tree_width = tree_width
+        self.split_out = split_out
+        self.split_every = split_every
         self.out_path = out_path or "./"
         self.on_host = on_host
         self.cat_cache = cat_cache
         self.categories = {}
+        nvt_cat._deprecate_tree_width(tree_width)
 
         self._cont_names = None
 
-        if isinstance(cont_cols, nvt.WorkflowNode):
+        if isinstance(cont_cols, Node):
             self.cont_cols = cont_cols
         elif isinstance(cont_cols, ColumnSelector):
             self.cont_cols = self._cont_names = cont_cols
         else:
             self.cont_cols = self._cont_names = ColumnSelector(cont_cols)
 
         supported_ops = ["count", "sum", "mean", "std", "var", "min", "max"]
@@ -149,18 +155,19 @@
             ddf,
             nvt_cat.FitOptions(
                 col_selector,
                 self.cont_names,
                 self.stats,
                 self.out_path,
                 0,
-                self.tree_width,
+                self.split_out,
                 self.on_host,
                 concat_groups=False,
                 name_sep=self.name_sep,
+                split_every=self.split_every,
             ),
         )
         return Delayed(key, dsk)
 
     def fit_finalize(self, dask_stats):
         for col in dask_stats:
             self.categories[col] = dask_stats[col]
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/list_slice.py` & `nvtabular-23.6.0/nvtabular/ops/list_slice.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/logop.py` & `nvtabular-23.6.0/nvtabular/ops/logop.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/moments.py` & `nvtabular-23.6.0/nvtabular/ops/moments.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/normalize.py` & `nvtabular-23.6.0/nvtabular/ops/normalize.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 from merlin.core.dispatch import (
     DataFrameType,
     annotate,
     encode_list_column,
     flatten_list_column_values,
     is_list_dtype,
 )
-from merlin.dag import Supports
+from merlin.dag import DataFormats, Supports
+from merlin.dag.ops.stat_operator import StatOperator
 from merlin.schema import Tags
 from nvtabular.ops.moments import _custom_moments
 from nvtabular.ops.operator import ColumnSelector, Operator
-from nvtabular.ops.stat_operator import StatOperator
 
 
 class Normalize(StatOperator):
     """
     Standardizing the features around 0 with a standard deviation
     of 1 is a common technique to compare measurements that have
     different units. This operation can be added to the workflow
@@ -94,14 +94,23 @@
         return (
             Supports.CPU_DICT_ARRAY
             | Supports.GPU_DICT_ARRAY
             | Supports.CPU_DATAFRAME
             | Supports.GPU_DATAFRAME
         )
 
+    @property
+    def supported_formats(self):
+        return (
+            DataFormats.PANDAS_DATAFRAME
+            | DataFormats.CUDF_DATAFRAME
+            | DataFormats.NUMPY_DICT_ARRAY
+            | DataFormats.CUPY_DICT_ARRAY
+        )
+
     def clear(self):
         self.means = {}
         self.stds = {}
 
     @property
     def output_tags(self):
         return [Tags.CONTINUOUS]
@@ -178,14 +187,23 @@
             Supports.CPU_DICT_ARRAY
             | Supports.GPU_DICT_ARRAY
             | Supports.CPU_DATAFRAME
             | Supports.GPU_DATAFRAME
         )
 
     @property
+    def supported_formats(self):
+        return (
+            DataFormats.PANDAS_DATAFRAME
+            | DataFormats.CUDF_DATAFRAME
+            | DataFormats.NUMPY_DICT_ARRAY
+            | DataFormats.CUPY_DICT_ARRAY
+        )
+
+    @property
     def output_tags(self):
         return [Tags.CONTINUOUS]
 
     @property
     def output_dtype(self):
         return self.out_dtype or numpy.float64
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/rename.py` & `nvtabular-23.6.0/nvtabular/ops/rename.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/ops/target_encoding.py` & `nvtabular-23.6.0/nvtabular/ops/target_encoding.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,19 @@
     DataFrameType,
     arange,
     concat_columns,
     random_state,
     read_parquet_dispatch,
 )
 from merlin.dag import Node
+from merlin.dag.ops.stat_operator import StatOperator
 from merlin.schema import Schema, Tags
 from nvtabular.ops import categorify as nvt_cat
 from nvtabular.ops.moments import _custom_moments
 from nvtabular.ops.operator import ColumnSelector, Operator
-from nvtabular.ops.stat_operator import StatOperator
 
 
 class TargetEncoding(StatOperator):
     """
     Target encoding is a common feature-engineering technique for
     categorical columns in tabular datasets. For each categorical group,
     the mean of a continuous target column is calculated, and the
@@ -93,20 +93,23 @@
         Smoothing factor.
     out_col : str or list of str, default is problem-specific
         Name of output target-encoding column. If `cat_groups` includes
         multiple elements, this should be a list of the same length (and
         elements must be unique).
     out_dtype : str, default is problem-specific
         dtype of output target-encoding columns.
-    tree_width : dict or int, optional
-        Tree width of the hash-based groupby reduction for each categorical
-        column. High-cardinality columns may require a large `tree_width`,
-        while low-cardinality columns can likely use `tree_width=1`.
+    split_out : dict or int, optional
+        Number of files needed to store the final result of each groupby
+        reduction. High-cardinality groups may require a large `split_out`,
+        while low-cardinality columns can likely use `split_out=1` (default).
         If passing a dict, each key and value should correspond to the column
-        name and width, respectively. The default value is 8 for all columns.
+        name and value, respectively. The default value is 1 for all columns.
+    split_every : dict or int, optional
+        Number of adjacent partitions to aggregate in each tree-reduction
+        node. The default value is 8 for all columns.
     cat_cache : {"device", "host", "disk"} or dict
         Location to cache the list of unique categories for
         each categorical column. If passing a dict, each key and value
         should correspond to the column name and location, respectively.
         Default is "host" for all columns.
     out_path : str, optional
         Root directory where category statistics will be written out in
@@ -128,42 +131,46 @@
         target,
         target_mean=None,
         kfold=None,
         fold_seed=42,
         p_smooth=20,
         out_col=None,
         out_dtype=None,
-        tree_width=None,
+        split_out=None,
+        split_every=None,
         cat_cache="host",
         out_path=None,
         on_host=True,
         name_sep="_",
         drop_folds=True,
+        tree_width=None,
     ):
         super().__init__()
 
         target = Node.construct_from(target)
         self.dependency = target
         self.target = target
 
         self.target_mean = target_mean
         self.kfold = kfold or 3
         self.fold_seed = fold_seed
         self.p_smooth = p_smooth
         self.out_col = [out_col] if isinstance(out_col, str) else out_col
         self.out_dtype = out_dtype
-        self.tree_width = tree_width
+        self.split_out = split_out
+        self.split_every = split_every
         self.out_path = out_path or "./"
         self.on_host = on_host
         self.cat_cache = cat_cache
         self.name_sep = name_sep
         self.drop_folds = drop_folds
         self.fold_name = "__fold__"
         self.stats = {}
         self.means = {}  # TODO: just update target_mean?
+        nvt_cat._deprecate_tree_width(tree_width)
 
     def fit(self, col_selector: ColumnSelector, ddf: dd.DataFrame):
         moments = None
 
         if self.target_mean is None:
             # calculate the mean if we don't have it already
             moments = _custom_moments(ddf[self.target_columns])
@@ -193,18 +200,19 @@
             ddf,
             nvt_cat.FitOptions(
                 col_groups,
                 self.target_columns,
                 ["count", "sum"],
                 self.out_path,
                 0,
-                self.tree_width,
+                self.split_out,
                 self.on_host,
                 concat_groups=False,
                 name_sep=self.name_sep,
+                split_every=self.split_every,
             ),
         )
         return Delayed(key, dsk), moments
 
     def fit_finalize(self, dask_stats):
         for col, value in dask_stats[0].items():
             self.stats[col] = value
```

### Comparing `nvtabular-23.5.0/nvtabular/ops/value_counts.py` & `nvtabular-23.6.0/nvtabular/ops/value_counts.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 #
 
 from typing import Any
 
 import dask.dataframe as dd
 
 from merlin.core.dispatch import DataFrameType, is_list_dtype, pull_apart_list
+from merlin.dag.ops.stat_operator import StatOperator
 from nvtabular.ops.operator import ColumnSelector
-from nvtabular.ops.stat_operator import StatOperator
 
 
 class ValueCount(StatOperator):
     """
     The operator calculates the min and max lengths of multihot columns.
     """
```

### Comparing `nvtabular-23.5.0/nvtabular/tools/__init__.py` & `nvtabular-23.6.0/nvtabular/ops/lambdaop.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,7 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+from merlin.dag.ops.udf import UDF
+
+LambdaOp = UDF
```

### Comparing `nvtabular-23.5.0/nvtabular/tools/data_gen.py` & `nvtabular-23.6.0/nvtabular/tools/data_gen.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/tools/dataset_inspector.py` & `nvtabular-23.6.0/nvtabular/tools/dataset_inspector.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/tools/inspector_script.py` & `nvtabular-23.6.0/nvtabular/tools/inspector_script.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/utils.py` & `nvtabular-23.6.0/nvtabular/worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # limitations under the License.
 #
 
 # pylint: disable=wildcard-import,unused-import,unused-wildcard-import
 import warnings
 
 # Re-export classes/modules from the core library for backwards compatibility
-from merlin.core.compat import *  # noqa
+from merlin.io.worker import *  # noqa
 
 warnings.warn(
-    "The `nvtabular.utils` module has moved to `merlin.core.utils`. "
-    "Support for importing from `nvtabular.utils` is deprecated, "
+    "The `nvtabular.worker` module has moved to `merlin.io.worker`. "
+    "Support for importing from `nvtabular.worker` is deprecated, "
     "and will be removed in a future version. Please update "
-    "your imports to refer to `merlin.core.utils`.",
+    "your imports to refer to `merlin.io.worker`.",
     DeprecationWarning,
 )
```

### Comparing `nvtabular-23.5.0/nvtabular/workflow/__init__.py` & `nvtabular-23.6.0/nvtabular/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/nvtabular/workflow/workflow.py` & `nvtabular-23.6.0/nvtabular/workflow/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,32 +13,34 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import inspect
 import json
 import logging
+import os
 import sys
 import time
 import types
 import warnings
 from functools import singledispatchmethod
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Optional, Union
 
 import cloudpickle
 import fsspec
 import pandas as pd
 
 from merlin.core.compat import cudf
 from merlin.dag import Graph
 from merlin.dag.executors import DaskExecutor, LocalExecutor
 from merlin.dag.node import iter_nodes
+from merlin.dag.ops.stat_operator import StatOperator
 from merlin.io import Dataset
 from merlin.schema import Schema
-from nvtabular.ops import LambdaOp, StatOperator
+from nvtabular.ops import LambdaOp
 from nvtabular.workflow.node import WorkflowNode
 
 LOG = logging.getLogger("nvtabular")
 
 
 if TYPE_CHECKING:
     import distributed
@@ -137,14 +139,18 @@
         Workflow
             This workflow where each node in the graph has a fitted schema
         """
         self.graph.construct_schema(input_schema)
         return self
 
     @property
+    def subworkflows(self):
+        return list(self.graph.subgraphs.keys())
+
+    @property
     def input_dtypes(self):
         return self.graph.input_dtypes
 
     @property
     def input_schema(self):
         return self.graph.input_schema
 
@@ -159,14 +165,18 @@
     @property
     def output_node(self):
         return self.graph.output_node
 
     def _input_columns(self):
         return self.graph._input_columns()
 
+    def get_subworkflow(self, subgraph_name):
+        subgraph = self.graph.subgraph(subgraph_name)
+        return Workflow(subgraph.output_node)
+
     def remove_inputs(self, input_cols) -> "Workflow":
         """Removes input columns from the workflow.
 
         This is useful for the case of inference where you might need to remove label columns
         from the processed set.
 
         Parameters
@@ -196,53 +206,15 @@
             data should be the training dataset only.
 
         Returns
         -------
         Workflow
             This Workflow with statistics calculated on it
         """
-        self.clear_stats()
-
-        if not self.graph.output_schema:
-            self.graph.construct_schema(dataset.schema)
-
-        ddf = dataset.to_ddf(columns=self._input_columns())
-
-        # Get a dictionary mapping all StatOperators we need to fit to a set of any dependent
-        # StatOperators (having StatOperators that depend on the output of other StatOperators
-        # means that will have multiple phases in the fit cycle here)
-        stat_op_nodes = {
-            node: Graph.get_nodes_by_op_type(node.parents_with_dependencies, StatOperator)
-            for node in Graph.get_nodes_by_op_type([self.graph.output_node], StatOperator)
-        }
-
-        while stat_op_nodes:
-            # get all the StatOperators that we can currently call fit on (no outstanding
-            # dependencies)
-            current_phase = [
-                node for node, dependencies in stat_op_nodes.items() if not dependencies
-            ]
-            if not current_phase:
-                # this shouldn't happen, but lets not infinite loop just in case
-                raise RuntimeError("failed to find dependency-free StatOperator to fit")
-
-            self.executor.fit(ddf, current_phase)
-
-            # Remove all the operators we processed in this phase, and remove
-            # from the dependencies of other ops too
-            for node in current_phase:
-                stat_op_nodes.pop(node)
-            for dependencies in stat_op_nodes.values():
-                dependencies.difference_update(current_phase)
-
-        # This captures the output dtypes of operators like LambdaOp where
-        # the dtype can't be determined without running the transform
-        self._transform_impl(dataset, capture_dtypes=True).sample_dtypes()
-        self.graph.construct_schema(dataset.schema, preserve_dtypes=True)
-
+        self.executor.fit(dataset, self.graph)
         return self
 
     def fit_transform(self, dataset: Dataset) -> Dataset:
         """Convenience method to both fit the workflow and transform the dataset in a single
         call. Equivalent to calling ``workflow.fit(dataset)`` followed by
         ``workflow.transform(dataset)``
 
@@ -328,33 +300,35 @@
             else:
                 mod = inspect.getmodule(f)
                 if mod is not None:
                     result.add(mod)
 
         return [mod for mod in result if mod.__name__ not in exclusions]
 
-    def save(self, path, modules_byvalue=None):
+    def save(self, path: Union[str, os.PathLike], modules_byvalue=None):
         """Save this workflow to disk
 
         Parameters
         ----------
-        path: str
+        path: Union[str, os.PathLike]
             The path to save the workflow to
         modules_byvalue:
             A list of modules that should be serialized by value. This
             should include any modules that will not be available on
             the host where this workflow is ultimately deserialized.
 
             In lieu of an explicit list, pass None to serialize all modules
             by reference or pass "auto" to use a heuristic to infer which
             modules to serialize by value.
         """
         # avoid a circular import getting the version
         from nvtabular import __version__ as nvt_version
 
+        path = str(path)
+
         fs = fsspec.get_fs_token_paths(path)[0]
 
         fs.makedirs(path, exist_ok=True)
 
         # point all stat ops to store intermediate output (parquet etc) at the path
         # this lets us easily bundle
         for stat in Graph.get_nodes_by_op_type([self.output_node], StatOperator):
@@ -418,32 +392,34 @@
                     if m.__name__ not in preexisting_modules_byvalue:
                         cloudpickle.unregister_pickle_by_value(m)
                 elif isinstance(m, str) and m in sys.modules:
                     if m not in preexisting_modules_byvalue:
                         cloudpickle.unregister_pickle_by_value(sys.modules[m])
 
     @classmethod
-    def load(cls, path, client=None) -> "Workflow":
+    def load(cls, path: Union[str, os.PathLike], client=None) -> "Workflow":
         """Load up a saved workflow object from disk
 
         Parameters
         ----------
-        path: str
+        path: Union[str, os.PathLike]
             The path to load the workflow from
         client: distributed.Client, optional
             The Dask distributed client to use for multi-gpu processing and multi-node processing
 
         Returns
         -------
         Workflow
             The Workflow loaded from disk
         """
         # avoid a circular import getting the version
         from nvtabular import __version__ as nvt_version
 
+        path = str(path)
+
         fs = fsspec.get_fs_token_paths(path)[0]
 
         # check version information from the metadata blob, and warn if we have a mismatch
         meta = json.load(fs.open(fs.sep.join([path, "metadata.json"])))
 
         def parse_version(version):
             return version.split(".")[:2]
```

### Comparing `nvtabular-23.5.0/nvtabular.egg-info/PKG-INFO` & `nvtabular-23.6.0/nvtabular.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvtabular
-Version: 23.5.0
+Version: 23.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/NVTabular
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
 License-File: LICENSE
 
 ## [NVTabular](https://github.com/NVIDIA/NVTabular)
 
 [![PyPI](https://img.shields.io/pypi/v/NVTabular?color=orange&label=version)](https://pypi.python.org/pypi/NVTabular/)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/NVTabular)](https://github.com/NVIDIA-Merlin/NVTabular/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/NVTabular)](https://github.com/NVIDIA-Merlin/NVTabular/blob/stable/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html)
 
 NVTabular is a feature engineering and preprocessing library for tabular data that is designed to easily manipulate terabyte scale datasets and train deep learning (DL) based recommender systems. It provides high-level abstraction to simplify code and accelerates computation on the GPU using the [RAPIDS Dask-cuDF](https://github.com/rapidsai/cudf/tree/main/python/dask_cudf) library.
 
 NVTabular is a component of [NVIDIA Merlin](https://developer.nvidia.com/nvidia-merlin), an open source framework for building and deploying recommender systems and works with the other Merlin components including [Merlin Models](https://github.com/NVIDIA-Merlin/models), [HugeCTR](https://github.com/NVIDIA/HugeCTR) and [Merlin Systems](https://github.com/NVIDIA-Merlin/systems) to provide end-to-end acceleration of recommender systems on the GPU. Extending beyond model training, with NVIDIA’s [Triton Inference Server](https://github.com/NVIDIA/tensorrt-inference-server), the feature engineering and preprocessing steps performed on the data during training can be automatically applied to incoming data during inference.
 
 <!-- <img src='https://developer.nvidia.com/blog/wp-content/uploads/2020/07/recommender-system-training-pipeline-1.png'/> -->
 
@@ -45,15 +45,15 @@
 NVTabular alleviates these challenges and helps data scientists and ML engineers:
 
 - process datasets that exceed GPU and CPU memory without having to worry about scale.
 - focus on what to do with the data and not how to do it by using abstraction at the operation level.
 - prepare datasets quickly and easily for experimentation so that more models can be trained.
 - deploy models into production by providing faster dataset transformation
 
-Learn more in the NVTabular [core features documentation](https://nvidia-merlin.github.io/NVTabular/main/core_features.html).
+Learn more in the NVTabular [core features documentation](https://nvidia-merlin.github.io/NVTabular/stable/core_features.html).
 
 ### Performance
 
 When running NVTabular on the Criteo 1TB Click Logs Dataset using a single V100 32GB GPU, feature engineering and preprocessing was able to be completed in 13 minutes. Furthermore, when running NVTabular on a DGX-1 cluster with eight V100 GPUs, feature engineering and preprocessing was able to be completed within three minutes. Combined with [HugeCTR](http://www.github.com/NVIDIA/HugeCTR/), the dataset can be processed and a full model can be trained in only six minutes.
 
 The performance of the Criteo DRLM workflow also demonstrates the effectiveness of the NVTabular library. The original ETL script provided in Numpy took over five days to complete. Combined with CPU training, the total iteration time is over one week. By optimizing the ETL code in Spark and running on a DGX-1 equivalent cluster, the time to complete feature engineering and preprocessing was reduced to three hours. Meanwhile, training was completed in one hour.
 
@@ -93,32 +93,32 @@
 
 | Container Name    | Container Location                                                                   | Functionality                              |
 | ----------------- | ------------------------------------------------------------------------------------ | ------------------------------------------ |
 | merlin-hugectr    | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-hugectr    | NVTabular, HugeCTR, and Triton Inference   |
 | merlin-tensorflow | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-tensorflow | NVTabular, Tensorflow and Triton Inference |
 | merlin-pytorch    | https://catalog.ngc.nvidia.com/orgs/nvidia/teams/merlin/containers/merlin-pytorch    | NVTabular, PyTorch, and Triton Inference   |
 
-To use these Docker containers, you'll first need to install the [NVIDIA Container Toolkit](https://github.com/NVIDIA/nvidia-docker) to provide GPU support for Docker. You can use the NGC links referenced in the table above to obtain more information about how to launch and run these containers. To obtain more information about the software and model versions that NVTabular supports per container, see [Support Matrix](https://github.com/NVIDIA/NVTabular/blob/main/docs/source/resources/support_matrix.rst).
+To use these Docker containers, you'll first need to install the [NVIDIA Container Toolkit](https://github.com/NVIDIA/nvidia-docker) to provide GPU support for Docker. You can use the NGC links referenced in the table above to obtain more information about how to launch and run these containers. To obtain more information about the software and model versions that NVTabular supports per container, see [Support Matrix](https://github.com/NVIDIA/NVTabular/blob/stable/docs/source/resources/support_matrix.rst).
 
 ### Notebook Examples and Tutorials
 
-We provide a [collection of examples](https://github.com/NVIDIA-Merlin/NVTabular/tree/main/examples) to demonstrate feature engineering with NVTabular as Jupyter notebooks:
+We provide a [collection of examples](https://github.com/NVIDIA-Merlin/NVTabular/tree/stable/examples) to demonstrate feature engineering with NVTabular as Jupyter notebooks:
 
 - Introduction to NVTabular's High-Level API
 - Advanced workflows with NVTabular
 - NVTabular on CPU
 - Scaling NVTabular to multi-GPU systems
 
 In addition, NVTabular is used in many of our examples in other Merlin libraries:
 
-- [End-To-End Examples with Merlin](https://github.com/NVIDIA-Merlin/Merlin/tree/main/examples)
-- [Training Examples with Merlin Models](https://github.com/NVIDIA-Merlin/models/tree/main/examples)
-- [Training Examples with Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/tree/main/examples)
+- [End-To-End Examples with Merlin](https://github.com/NVIDIA-Merlin/Merlin/tree/stable/examples)
+- [Training Examples with Merlin Models](https://github.com/NVIDIA-Merlin/models/tree/stable/examples)
+- [Training Examples with Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/tree/stable/examples)
 
 ### Feedback and Support
 
-If you'd like to contribute to the library directly, see the [Contributing.md](https://github.com/NVIDIA/NVTabular/blob/main/CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
+If you'd like to contribute to the library directly, see the [Contributing.md](https://github.com/NVIDIA/NVTabular/blob/stable/CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin Roadmap, we encourage you to share all the details regarding your recommender system pipeline in this [survey](https://developer.nvidia.com/merlin-devzone-survey).
 
 If you're interested in learning more about how NVTabular works, see
-[our NVTabular documentation](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html). We also have [API documentation](https://nvidia-merlin.github.io/NVTabular/main/api/index.html) that outlines the specifics of the available calls within the library.
+[our NVTabular documentation](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html). We also have [API documentation](https://nvidia-merlin.github.io/NVTabular/stable/api/index.html) that outlines the specifics of the available calls within the library.
```

### Comparing `nvtabular-23.5.0/nvtabular.egg-info/SOURCES.txt` & `nvtabular-23.6.0/nvtabular.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -34,26 +34,14 @@
 nvtabular/framework_utils/tensorflow/layers/outer_product.py
 nvtabular/framework_utils/torch/__init__.py
 nvtabular/framework_utils/torch/models.py
 nvtabular/framework_utils/torch/utils.py
 nvtabular/framework_utils/torch/layers/__init__.py
 nvtabular/framework_utils/torch/layers/embeddings.py
 nvtabular/inference/__init__.py
-nvtabular/inference/triton/__init__.py
-nvtabular/inference/triton/benchmarking_tools.py
-nvtabular/inference/triton/data_conversions.py
-nvtabular/inference/triton/ensemble.py
-nvtabular/inference/triton/workflow_model.py
-nvtabular/inference/triton/model/__init__.py
-nvtabular/inference/triton/model/model_pt.py
-nvtabular/inference/workflow/__init__.py
-nvtabular/inference/workflow/base.py
-nvtabular/inference/workflow/hugectr.py
-nvtabular/inference/workflow/pytorch.py
-nvtabular/inference/workflow/tensorflow.py
 nvtabular/loader/__init__.py
 nvtabular/loader/backend.py
 nvtabular/loader/tensorflow.py
 nvtabular/loader/tf_utils.py
 nvtabular/loader/torch.py
 nvtabular/ops/__init__.py
 nvtabular/ops/add_metadata.py
```

### Comparing `nvtabular-23.5.0/pyproject.toml` & `nvtabular-23.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/setup.cfg` & `nvtabular-23.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/setup.py` & `nvtabular-23.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `nvtabular-23.5.0/versioneer.py` & `nvtabular-23.6.0/versioneer.py`

 * *Files identical despite different names*

