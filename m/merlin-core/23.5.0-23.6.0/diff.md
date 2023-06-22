# Comparing `tmp/merlin-core-23.5.0.tar.gz` & `tmp/merlin-core-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-core-23.5.0.tar", last modified: Wed May 31 14:39:07 2023, max compression
+gzip compressed data, was "merlin-core-23.6.0.tar", last modified: Thu Jun 22 16:10:54 2023, max compression
```

## Comparing `merlin-core-23.5.0.tar` & `merlin-core-23.6.0.tar`

### file list

```diff
@@ -1,101 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 14:39:00.000000 merlin-core-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 14:39:00.000000 merlin-core-23.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-31 14:39:07.044466 merlin-core-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-31 14:39:00.000000 merlin-core-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.032466 merlin-core-23.5.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/core/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/core/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/core/compat/
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/compat/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/compat/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    25544 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/has_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    16949 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dag/
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12874 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/base_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21211 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7165 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    22848 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dag/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/concat_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/subset_columns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/ops/subtraction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dag/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dispatch/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.036466 merlin-core-23.5.0/merlin/dtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/aliases.py
--rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.040466 merlin-core-23.5.0/merlin/dtypes/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/cudf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/merlin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/python.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/mappings/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/dtypes/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.040466 merlin-core-23.5.0/merlin/io/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/avro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataframe_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataframe_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)    54001 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/dataset_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/fsspec_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/hugectr.py
--rw-r--r--   0 runner    (1001) docker     (123)    46920 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/io/writer_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.040466 merlin-core-23.5.0/merlin/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/schema/io/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/proto_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    36781 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/schema_bp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/io/tensorflow_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/schema/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/table/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/cupy_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/numpy_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/tensor_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/tensor_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/tensorflow_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/table/torch_column.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-31 14:39:00.000000 merlin-core-23.5.0/merlin/testing/assert_equals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:07.044466 merlin-core-23.5.0/merlin_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 14:39:06.000000 merlin-core-23.5.0/merlin_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-31 14:39:00.000000 merlin-core-23.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-31 14:39:00.000000 merlin-core-23.5.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-31 14:39:00.000000 merlin-core-23.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-31 14:39:07.044466 merlin-core-23.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-31 14:39:00.000000 merlin-core-23.5.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-05-31 14:39:00.000000 merlin-core-23.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.689721 merlin-core-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 16:10:47.000000 merlin-core-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-22 16:10:47.000000 merlin-core-23.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 16:10:54.689721 merlin-core-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-22 16:10:47.000000 merlin-core-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.673721 merlin-core-23.6.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.689721 merlin-core-23.6.0/merlin/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 16:10:54.689721 merlin-core-23.6.0/merlin/core/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.677721 merlin-core-23.6.0/merlin/core/compat/
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/compat/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/compat/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26511 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/has_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17047 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.677721 merlin-core-23.6.0/merlin/dag/
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12937 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/base_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25427 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23428 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.677721 merlin-core-23.6.0/merlin/dag/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/add_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/concat_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/stat_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/subset_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/subtraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/ops/udf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dag/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.677721 merlin-core-23.6.0/merlin/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dispatch/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.681721 merlin-core-23.6.0/merlin/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.681721 merlin-core-23.6.0/merlin/dtypes/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/cudf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/merlin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/mappings/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/dtypes/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.685721 merlin-core-23.6.0/merlin/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/avro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/dataframe_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/dataframe_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56311 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/dataset_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11368 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/fsspec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/hugectr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46920 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5272 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/io/writer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.685721 merlin-core-23.6.0/merlin/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.685721 merlin-core-23.6.0/merlin/schema/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/schema/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/schema/io/proto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36781 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/schema/io/schema_bp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/schema/io/tensorflow_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22543 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/schema/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.689721 merlin-core-23.6.0/merlin/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/cupy_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/numpy_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/tensor_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10490 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/tensor_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5307 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/tensorflow_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/table/torch_column.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.689721 merlin-core-23.6.0/merlin/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-06-22 16:10:47.000000 merlin-core-23.6.0/merlin/testing/assert_equals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:10:54.689721 merlin-core-23.6.0/merlin_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 16:10:54.000000 merlin-core-23.6.0/merlin_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-22 16:10:54.000000 merlin-core-23.6.0/merlin_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:10:54.000000 merlin-core-23.6.0/merlin_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:10:54.000000 merlin-core-23.6.0/merlin_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 16:10:54.000000 merlin-core-23.6.0/merlin_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 16:10:54.000000 merlin-core-23.6.0/merlin_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-22 16:10:47.000000 merlin-core-23.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-22 16:10:47.000000 merlin-core-23.6.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-22 16:10:47.000000 merlin-core-23.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-22 16:10:54.689721 merlin-core-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-22 16:10:47.000000 merlin-core-23.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81339 2023-06-22 16:10:47.000000 merlin-core-23.6.0/versioneer.py
```

### Comparing `merlin-core-23.5.0/LICENSE` & `merlin-core-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/PKG-INFO` & `merlin-core-23.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-core
-Version: 23.5.0
+Version: 23.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/core
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-core-23.5.0/README.md` & `merlin-core-23.6.0/README.md`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/core/__init__.py` & `merlin-core-23.6.0/merlin/core/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/core/compat/__init__.py` & `merlin-core-23.6.0/merlin/core/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/core/compat/tensorflow.py` & `merlin-core-23.6.0/merlin/core/compat/tensorflow.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/core/compat/torch.py` & `merlin-core-23.6.0/merlin/core/compat/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/core/dispatch.py` & `merlin-core-23.6.0/merlin/core/dispatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 import pyarrow as pa
 import pyarrow.parquet as pq
 
 # unused HAS_GPU import is here for backwards compatibility
 from merlin.core.compat import HAS_GPU  # pylint: disable=unused-import # noqa: F401
 from merlin.core.compat import cudf
 from merlin.core.compat import cupy as cp
+from merlin.core.compat import dask_cudf
 from merlin.core.protocols import DataFrameLike, DictLike, SeriesLike
 
 rmm = None
 
 if cudf:
     try:
-        import dask_cudf
         import rmm  # type: ignore[no-redef]
         from cudf.core.column import as_column, build_column
 
         try:
             # cudf >= 21.08
             from cudf.api.types import is_list_dtype as cudf_is_list_dtype
             from cudf.api.types import is_string_dtype as cudf_is_string_dtype
@@ -307,14 +307,35 @@
     """Check if Series contains any null values"""
     if isinstance(s, pd.Series):
         return s.isnull().values.any()
     else:
         return s.has_nulls
 
 
+def columnwise_explode(series):
+    """Explode a list column along the column axis"""
+    if isinstance(series, pd.Series):
+        df = pd.DataFrame(series.tolist())
+    else:
+        df = cudf.DataFrame(series.to_pandas().tolist())
+    df.columns = [f"{series.name}_{c}" for c in df.columns]
+    return df
+
+
+def dataframe_columnwise_explode(dataframe):
+    """Explode all list columns in a dataframe along the column axis"""
+    columns_in_dataframe = dataframe.columns
+    for col in columns_in_dataframe:
+        if is_list_dtype(dataframe[col]):
+            col_df = columnwise_explode(dataframe[col])
+            dataframe = concat_columns([dataframe, col_df])
+            dataframe = dataframe.drop(labels=col, axis=1)
+    return dataframe
+
+
 def list_val_dtype(ser: SeriesLike) -> Optional[np.dtype]:
     """
     Return the dtype of the leaves from a list or nested list
 
     Parameters
     ----------
     ser : SeriesLike
@@ -352,14 +373,18 @@
         return ser.is_list
     if isinstance(ser, pd.Series):
         if not len(ser):  # pylint: disable=len-as-condition
             return False
         return pd.api.types.is_list_like(ser.values[0])
     elif cudf and isinstance(ser, (cudf.Series, cudf.ListDtype)):
         return cudf_is_list_dtype(ser)
+    elif dask_cudf and isinstance(ser, dask_cudf.Series):
+        return cudf_is_list_dtype(ser.head())
+    elif isinstance(ser, dd.core.Series):
+        return pd.api.types.is_list_like(ser.head()[0])
     elif isinstance(ser, np.ndarray) or (cp and isinstance(ser, cp.ndarray)):
         return len(ser.shape) > 1
     return pd.api.types.is_list_like(ser)
 
 
 def is_string_dtype(dtype: np.dtype) -> bool:
     """Check if the dtype of obj is a string type
```

### Comparing `merlin-core-23.5.0/merlin/core/has_gpu.py` & `merlin-core-23.6.0/merlin/core/has_gpu.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/core/protocols.py` & `merlin-core-23.6.0/merlin/core/protocols.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/core/utils.py` & `merlin-core-23.6.0/merlin/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     conventional `with` statement::
 
         from merlin.core.utils import Disributed
 
         workflow = nvt.Workflow(["col"] >> ops.Normalize())
         dataset = nvt.Dataset(...)
         with Distributed():
+            workflow.fit(dataset)
             workflow.transform(dataset).to_parquet(...)
 
     In this case, all Dask-based scheduling and execution
     required within the `with Distributed()` block will be
     performed using a distributed cluster. If an existing
     client is not detected, a default `LocalCUDACluster`
     or `LocalCluster` will be automatically deployed (the
@@ -191,14 +192,15 @@
 
     Alternatively, the distributed-execution manager can be
     used without a `with` statement as follows::
 
         workflow = nvt.Workflow(["col"] >> ops.Normalize())
         dataset = nvt.Dataset(...)
         exec = Distributed()
+        workflow.fit(dataset)
         workflow.transform(dataset).to_parquet(...)
         exec.deactivate()
 
     Note that `deactivate()` must be used to resume default
     execution in the case that `Distributed` is not used in
     a `with` context.
 
@@ -212,14 +214,15 @@
             n_workers=4,
             local_directory="/raid/dask-space",
             protocol="ucx",
             device_memory_limit=0.8,
             rmm_pool_size="20GB",
             log_spilling=True,
         ):
+            workflow.fit(dataset)
             workflow.transform(dataset).to_parquet(...)
 
     In this case, the `cluster_type="cuda"` calls for the
     creation of a `LocalCUDACluster`, and all other key-word
     arguments are passed to the `LocalCUDACluster` constructor.
     """
```

### Comparing `merlin-core-23.5.0/merlin/dag/__init__.py` & `merlin-core-23.6.0/merlin/dag/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dag/base_operator.py` & `merlin-core-23.6.0/merlin/dag/base_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,14 +278,18 @@
 
         return col_schema.with_shape(shape)
 
     @property
     def dynamic_dtypes(self):
         return False
 
+    @property
+    def is_subgraph(self):
+        return False
+
     def _compute_tags(self, col_schema, input_schema):
         tags = []
         if input_schema.column_schemas:
             source_col_name = input_schema.column_names[0]
             tags = input_schema[source_col_name].tags
 
         # Override empty tags with tags from the input schema
```

### Comparing `merlin-core-23.5.0/merlin/dag/executors.py` & `merlin-core-23.6.0/merlin/dag/executors.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,15 +26,17 @@
 from merlin.core.dispatch import concat_columns, is_list_dtype, list_val_dtype
 from merlin.core.utils import (
     ensure_optimize_dataframe_graph,
     global_dask_client,
     set_client_deprecated,
 )
 from merlin.dag import ColumnSelector, DataFormats, Graph, Node
+from merlin.dag.ops.stat_operator import StatOperator
 from merlin.dtypes.shape import DefaultShapes
+from merlin.io import Dataset
 from merlin.io.worker import clean_worker_cache
 from merlin.table import CupyColumn, NumpyColumn, TensorTable
 
 LOG = logging.getLogger("merlin")
 
 
 class Device(Enum):
@@ -267,21 +269,25 @@
                     f"`{output_data_dtype}`."
                 )
 
     # TODO: Turn this into a function
     def _combine_node_outputs(self, node, transformed, output):
         node_output_cols = _get_unique(node.output_schema.column_names)
 
-        # dask needs output to be in the same order defined as meta, reorder partitions here
-        # this also selects columns (handling the case of removing columns from the output using
-        # "-" overload)
+        if isinstance(transformed, dict):
+            selected_cols = {col: transformed[col] for col in node_output_cols}
+        else:
+            # dask needs output columns to be defined in the same order as meta,
+            # so reorder columns here
+            selected_cols = transformed[node_output_cols]
+
         if output is None:
-            output = transformed[node_output_cols]
+            output = selected_cols
         else:
-            output = concat_columns([output, transformed[node_output_cols]])
+            output = concat_columns([output, selected_cols])
 
         return output
 
 
 class DaskExecutor:
     """
     An executor for running Merlin operator DAGs as distributed Dask jobs
@@ -324,25 +330,33 @@
                 " `graph` argument must be either a `Graph` object (preferred)"
                 " or a list of `Node` objects (deprecated, but supported for backward"
                 " compatibility.)"
             )
 
         self._clear_worker_cache()
 
+        for node in nodes:
+            if isinstance(node.op, StatOperator) and not node.op.fitted:
+                raise RuntimeError(
+                    f"Graphs containing {node.op} must be fit before "
+                    "attempting to use them to transform data."
+                )
+
         # Check if we are only selecting columns (no transforms).
         # If so, we should perform column selection at the ddf level.
         # Otherwise, Dask will not push the column selection into the
         # IO function.
+
         if not nodes:
             return ddf[_get_unique(additional_columns)] if additional_columns else ddf
 
         if isinstance(nodes, Node):
             nodes = [nodes]
 
-        columns = list(flatten(wfn.output_columns.names for wfn in nodes))
+        columns = list(flatten(node.output_columns.names for node in nodes))
         columns += additional_columns if additional_columns else []
 
         if isinstance(output_dtypes, dict):
             for col_name, col_dtype in output_dtypes.items():
                 if col_dtype:
                     output_dtypes[col_name] = md.dtype(col_dtype).to_numpy
 
@@ -368,68 +382,167 @@
                 capture_dtypes=capture_dtypes,
                 strict=strict,
                 meta=output_dtypes,
                 enforce_metadata=False,
             )
         )
 
-    def fit(self, ddf, nodes, strict=False):
+    def _transform_impl(self, dataset: Dataset, graph: Graph, capture_dtypes=False):
+        if graph.output_schema:
+            graph.construct_schema(dataset.schema)
+
+        ddf = dataset.to_ddf(columns=graph._input_columns())
+
+        return Dataset(
+            self._executor.transform(
+                ddf,
+                graph.output_node,
+                graph.output_dtypes,
+                capture_dtypes=capture_dtypes,
+            ),
+            cpu=dataset.cpu,
+            base_dataset=dataset.base_dataset,
+            schema=graph.output_schema,
+        )
+
+    def _transform_df(self, df):
+        if not self.graph.output_schema:
+            raise ValueError("no output schema")
+
+        return LocalExecutor().transform(df, self.output_node, self.output_dtypes)
+
+    def fit(self, dataset: Dataset, graph: Graph, refit=True):
+        if refit:
+            clear_stats(graph)
+
+        if not graph.output_schema:
+            graph.construct_schema(dataset.schema)
+
+        # Get a dictionary mapping all StatOperators we need to fit to a set of any dependent
+        # StatOperators (having StatOperators that depend on the output of other StatOperators
+        # means that will have multiple phases in the fit cycle here)
+        stat_op_nodes = {
+            node: Graph.get_nodes_by_op_type(
+                node.parents_with_dependencies,
+                StatOperator,
+            )
+            for node in Graph.get_nodes_by_op_type([graph.output_node], StatOperator)
+            if refit or not node.op.fitted
+        }
+
+        while stat_op_nodes:
+            # get all the StatOperators that we can currently call fit on (no outstanding
+            # dependencies)
+            current_phase = [
+                node for node, dependencies in stat_op_nodes.items() if not dependencies
+            ]
+            if not current_phase:
+                # this shouldn't happen, but lets not infinite loop just in case
+                raise RuntimeError("failed to find dependency-free StatOperator to fit")
+
+            self.fit_phase(dataset, current_phase)
+
+            # Remove all the operators we processed in this phase, and remove
+            # from the dependencies of other ops too
+            for node in current_phase:
+                stat_op_nodes.pop(node)
+            for dependencies in stat_op_nodes.values():
+                dependencies.difference_update(current_phase)
+
+        # This captures the output dtypes of operators like LambdaOp where
+        # the dtype can't be determined without running the transform
+        # self._transform_impl(dataset, capture_dtypes=True).sample_dtypes()
+        #
+        Dataset(
+            self.transform(
+                dataset.to_ddf(),
+                graph.output_node,
+                graph.output_dtypes,
+                capture_dtypes=True,
+            ),
+            cpu=dataset.cpu,
+            base_dataset=dataset.base_dataset,
+            schema=graph.output_schema,
+        ).sample_dtypes()
+        graph.construct_schema(dataset.schema, preserve_dtypes=True)
+
+        return graph
+
+    def fit_phase(self, dataset, nodes, strict=False):
         """Calculates statistics for a set of nodes on the input dataframe
 
         Parameters
         -----------
         ddf: dask.Dataframe
             The input dataframe to calculate statistics for. If there is a
             train/test split this should be the training dataset only.
         """
         stats = []
+        ddf = dataset.to_ddf()
         for node in nodes:
-            # Check for additional input columns that aren't generated by parents
-            addl_input_cols = set()
-            if node.parents:
-                upstream_output_cols = sum(
-                    [upstream.output_columns for upstream in node.parents_with_dependencies],
-                    ColumnSelector(),
-                )
-                addl_input_cols = set(node.input_columns.names) - set(upstream_output_cols.names)
+            if hasattr(node.op, "fit"):
+                # Check for additional input columns that aren't generated by parents
+                addl_input_cols = set()
+                if node.parents:
+                    upstream_output_cols = sum(
+                        [upstream.output_columns for upstream in node.parents_with_dependencies],
+                        ColumnSelector(),
+                    )
+                    addl_input_cols = set(node.input_columns.names) - set(
+                        upstream_output_cols.names
+                    )
 
-            # apply transforms necessary for the inputs to the current column group, ignoring
-            # the transforms from the statop itself
-            transformed_ddf = self.transform(
-                ddf,
-                node.parents_with_dependencies,
-                additional_columns=addl_input_cols,
-                capture_dtypes=True,
-                strict=strict,
-            )
+                # apply transforms necessary for the inputs to the current column group, ignoring
+                # the transforms from the statop itself
+                transformed_ddf = self.transform(
+                    ddf,
+                    node.parents_with_dependencies,
+                    additional_columns=addl_input_cols,
+                    capture_dtypes=True,
+                    strict=strict,
+                )
 
-            try:
-                stats.append(node.op.fit(node.input_columns, transformed_ddf))
-            except Exception:
-                LOG.exception("Failed to fit operator %s", node.op)
-                raise
+                try:
+                    if node.op.is_subgraph:
+                        stats.append(node.op.fit(node.input_columns, Dataset(ddf)))
+                    else:
+                        stats.append(node.op.fit(node.input_columns, transformed_ddf))
+                except Exception:
+                    LOG.exception("Failed to fit operator %s", node.op)
+                    raise
 
         dask_client = global_dask_client()
         if dask_client:
-            results = [r.result() for r in dask_client.compute(stats)]
+            results = [r.result() for r in dask_client.compute(stats) if r is not None]
         else:
             results = dask.compute(stats, scheduler="synchronous")[0]
-
         for computed_stats, node in zip(results, nodes):
             node.op.fit_finalize(computed_stats)
+            node.op.fitted = True
 
     def _clear_worker_cache(self):
         # Clear worker caches to be "safe"
         dask_client = global_dask_client()
         if dask_client:
             dask_client.run(clean_worker_cache)
         else:
             clean_worker_cache()
 
 
+def clear_stats(graph):
+    """Removes calculated statistics from each node in the workflow graph
+
+    See Also
+    --------
+    nvtabular.ops.stat_operator.StatOperator.clear
+    """
+    for stat in Graph.get_nodes_by_op_type([graph.output_node], StatOperator):
+        stat.op.clear()
+
+
 def _get_unique(cols):
     # Need to preserve order in unique-column list
     return list({x: x for x in cols}.keys())
 
 
 def _mask_cpu_only(supported):
     return functools.reduce(
@@ -439,35 +552,33 @@
             for v in list(DataFormats)
             if v & supported and ("NUMPY" in str(v) or "PANDAS" in str(v))
         ),
     )
 
 
 def _data_format(transformable):
-    data = TensorTable(transformable) if isinstance(transformable, dict) else transformable
-
-    if cudf and isinstance(data, cudf.DataFrame):
+    if cudf and isinstance(transformable, cudf.DataFrame):
         return DataFormats.CUDF_DATAFRAME
-    elif pandas and isinstance(data, pandas.DataFrame):
+    elif pandas and isinstance(transformable, pandas.DataFrame):
         return DataFormats.PANDAS_DATAFRAME
-    elif isinstance(data, dict) and data.values():
-        first = list(data.values())[0]
-        if cupy and first and isinstance(first, cupy.ndarray):
+    elif isinstance(transformable, dict) and transformable.values():
+        first = list(transformable.values())[0]
+        if cupy and isinstance(first, cupy.ndarray):
             return DataFormats.CUPY_DICT_ARRAY
-        if numpy and first and isinstance(first, numpy.ndarray):
+        if numpy and isinstance(first, numpy.ndarray):
             return DataFormats.NUMPY_DICT_ARRAY
-    elif data.column_type is CupyColumn:
+    elif transformable.column_type is CupyColumn:
         return DataFormats.CUPY_TENSOR_TABLE
-    elif data.column_type is NumpyColumn:
+    elif transformable.column_type is NumpyColumn:
         return DataFormats.NUMPY_TENSOR_TABLE
     else:
-        if isinstance(data, TensorTable):
-            raise TypeError(f"Unknown type: {data.column_type}")
+        if isinstance(transformable, TensorTable):
+            raise TypeError(f"Unknown type: {transformable.column_type}")
         else:
-            raise TypeError(f"Unknown type: {type(data)}")
+            raise TypeError(f"Unknown type: {type(transformable)}")
 
 
 def _convert_format(tensors, target_format):
     """
     Converts data to one of the formats specified in 'target_format'
 
     This allows us to convert data to/from dataframe representations for operators that
```

### Comparing `merlin-core-23.5.0/merlin/dag/graph.py` & `merlin-core-23.6.0/merlin/dag/graph.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,51 +12,52 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import logging
 from collections import deque
-from typing import Dict, Optional
+from typing import Dict
 
+from merlin.dag.base_operator import BaseOperator
 from merlin.dag.node import (
     Node,
     _combine_schemas,
     iter_nodes,
     postorder_iter_nodes,
     preorder_iter_nodes,
 )
+from merlin.dag.ops.stat_operator import StatOperator
 from merlin.schema import Schema
 
 LOG = logging.getLogger("merlin")
 
 
 class Graph:
     """
     Represents an DAG composed of Nodes, each of which contains an operator that
     transforms dataframes or dataframe-like data
     """
 
-    def __init__(self, output_node: Node, subgraphs: Optional[Dict[str, Node]] = None):
+    def __init__(self, output_node: Node):
+        if isinstance(output_node, BaseOperator):
+            output_node = Node.construct_from(output_node)
+
         self.output_node = output_node
-        self.subgraphs = subgraphs or {}
 
         parents_with_deps = self.output_node.parents_with_dependencies
         parents_with_deps.append(output_node)
 
-        for name, sg in self.subgraphs.items():
-            if sg not in parents_with_deps:
-                raise ValueError(
-                    f"The output node of subgraph {name} does not exist in the provided graph."
-                )
+        self.subgraphs: Dict[str, "Graph"] = {}
+        _find_subgraphs(output_node, self.subgraphs)
 
     def subgraph(self, name: str) -> "Graph":
-        if name not in self.subgraphs.keys():
+        if name not in self.subgraphs:
             raise ValueError(f"No subgraph named {name}. Options are: {self.subgraphs.keys()}")
-        return Graph(self.subgraphs[name])
+        return self.subgraphs[name]
 
     @property
     def input_dtypes(self):
         if self.input_schema:
             return {
                 name: col_schema.dtype
                 for name, col_schema in self.input_schema.column_schemas.items()
@@ -194,20 +195,43 @@
 
         return self
 
     @classmethod
     def get_nodes_by_op_type(cls, nodes, op_type):
         return set(node for node in iter_nodes(nodes) if isinstance(node.op, op_type))
 
+    def clear_stats(self):
+        """Removes calculated statistics from each node in the graph
+
+        See Also
+        --------
+        StatOperator.clear
+        """
+        for stat in Graph.get_nodes_by_op_type([self.output_node], StatOperator):
+            stat.op.clear()
+
 
 def _get_schemaless_nodes(nodes):
     schemaless_nodes = []
     for node in iter_nodes(nodes):
         if node.input_schema is None:
             schemaless_nodes.append(node)
 
     return set(schemaless_nodes)
 
 
 def _get_unique(cols):
     # Need to preserve order in unique-column list
     return list({x: x for x in cols}.keys())
+
+
+def _find_subgraphs(output_node, subgraphs):
+    for node in postorder_iter_nodes(output_node):
+        op = node.op
+        if op.is_subgraph and op.name:
+            if op.name in subgraphs:
+                raise ValueError(
+                    f"Found two subgraphs called {op.name}. "
+                    "Each subgraph must have a unique name."
+                )
+            subgraphs[op.name] = op.graph
+            _find_subgraphs(op.graph.output_node, subgraphs)
```

### Comparing `merlin-core-23.5.0/merlin/dag/node.py` & `merlin-core-23.6.0/merlin/dag/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 #
 import collections.abc
 from typing import List, Union
 
 from merlin.dag.base_operator import BaseOperator
 from merlin.dag.ops import ConcatColumns, SelectionOp, SubsetColumns, SubtractionOp
+from merlin.dag.ops.udf import UDF
 from merlin.dag.selector import ColumnSelector
 from merlin.schema import Schema
 
 
 class Node:
     """A Node is a group of columns that you want to apply the same transformations to.
     Node's can be transformed by shifting operators on to them, which returns a new
@@ -190,14 +191,15 @@
         root_schema : Schema
             Schema of the input dataset
         preserve_dtypes : bool, optional
             `True` if we don't want to override dtypes in the current schema, by default False
         """
         parents_schema = _combine_schemas(self.parents)
         deps_schema = _combine_schemas(self.dependencies)
+
         parents_selector = _combine_selectors(self.parents)
         dependencies_selector = _combine_selectors(self.dependencies)
 
         # If parent is an addition or selection node, we may need to
         # propagate grouping unless this node already has a selector
         if len(self.parents) == 1 and isinstance(self.parents[0].op, (ConcatColumns, SelectionOp)):
             parents_selector = self.parents[0].selector
@@ -255,28 +257,39 @@
                         f"Mismatched dtypes for column '{col_name}' provided to "
                         f"'{self.op.__class__.__name__}': "
                         f"ancestor nodes provided dtype '{source_col_schema.dtype}', "
                         f"expected dtype '{col_schema.dtype}'."
                     )
 
             self.op.validate_schemas(
-                parents_schema, deps_schema, self.input_schema, self.output_schema, strict_dtypes
+                parents_schema,
+                deps_schema,
+                self.input_schema,
+                self.output_schema,
+                strict_dtypes,
             )
 
     def __rshift__(self, operator):
         """Transforms this Node by applying an BaseOperator
 
         Parameters
         -----------
         operators: BaseOperator or callable
 
         Returns
         -------
         Node
         """
+
+        if callable(operator) and not (
+            isinstance(operator, type) and issubclass(operator, BaseOperator)
+        ):
+            # implicit lambdaop conversion.
+            operator = UDF(operator)
+
         if isinstance(operator, type) and issubclass(operator, BaseOperator):
             # handle case where an operator class is passed
             operator = operator()
 
         if not isinstance(operator, BaseOperator):
             raise ValueError(f"Expected operator or callable, got {operator.__class__}")
 
@@ -518,15 +531,19 @@
         return cols_repr
 
     @property
     def graph(self):
         return _to_graphviz(self)
 
     Nodable = Union[
-        "Node", str, List[str], ColumnSelector, List[Union["Node", str, List[str], ColumnSelector]]
+        "Node",
+        str,
+        List[str],
+        ColumnSelector,
+        List[Union["Node", str, List[str], ColumnSelector]],
     ]
 
     @classmethod
     def construct_from(
         cls,
         nodable: Nodable,
     ):
@@ -548,14 +565,18 @@
         TypeError
             If supplied input cannot be converted to a Node or list of Nodes
         """
         if isinstance(nodable, str):
             return Node(ColumnSelector([nodable]))
         if isinstance(nodable, ColumnSelector):
             return Node(nodable)
+        elif isinstance(nodable, BaseOperator):
+            node = Node()
+            node.op = nodable
+            return node
         elif isinstance(nodable, Node):
             return nodable
         elif isinstance(nodable, list):
             if all(isinstance(elem, str) for elem in nodable):
                 return Node(nodable)
             else:
                 nodes = [Node.construct_from(node) for node in nodable]
@@ -578,14 +599,16 @@
 
 def iter_nodes(nodes):
     queue = nodes[:]
     while queue:
         current = queue.pop()
         if isinstance(current, list):
             queue.extend(current)
+        elif current.op.is_subgraph:
+            queue.extend(iter_nodes([current.op.graph.output_node]))
         else:
             yield current
             for node in current.parents_with_dependencies:
                 if node not in queue:
                     queue.append(node)
```

### Comparing `merlin-core-23.5.0/merlin/dag/ops/__init__.py` & `merlin-core-23.6.0/merlin/testing/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2023, NVIDIA CORPORATION.
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
-# alias submodules here to avoid breaking everything with moving to submodules
+
 # flake8: noqa
-from merlin.dag.ops.concat_columns import ConcatColumns
-from merlin.dag.ops.selection import SelectionOp
-from merlin.dag.ops.subset_columns import SubsetColumns
-from merlin.dag.ops.subtraction import SubtractionOp
+from merlin.testing.assert_equals import assert_transformable_equal
```

### Comparing `merlin-core-23.5.0/merlin/dag/ops/concat_columns.py` & `merlin-core-23.6.0/merlin/dag/ops/concat_columns.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,19 @@
             Combined column selectors of dependency nodes
 
         Returns
         -------
         ColumnSelector
             Combined column selectors of parent and dependency nodes
         """
-        return super().compute_selector(
+        selector = super().compute_selector(
             input_schema,
             parents_selector + dependencies_selector,
         )
+        return selector
 
     def compute_input_schema(
         self,
         root_schema: Schema,
         parents_schema: Schema,
         deps_schema: Schema,
         selector: ColumnSelector,
```

### Comparing `merlin-core-23.5.0/merlin/dag/ops/rename.py` & `merlin-core-23.6.0/merlin/dag/ops/rename.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 from merlin.core.protocols import Transformable
-from merlin.dag import ColumnSelector
 from merlin.dag.base_operator import BaseOperator
+from merlin.dag.selector import ColumnSelector
 
 
 class Rename(BaseOperator):
     """This operation renames columns by one of several methods:
 
         - using a user defined lambda function to transform column names
         - appending a postfix string to every column name
```

### Comparing `merlin-core-23.5.0/merlin/dag/ops/selection.py` & `merlin-core-23.6.0/merlin/dag/ops/selection.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dag/ops/subset_columns.py` & `merlin-core-23.6.0/merlin/dag/ops/subset_columns.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dag/ops/subtraction.py` & `merlin-core-23.6.0/merlin/dag/ops/subtraction.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dag/selector.py` & `merlin-core-23.6.0/merlin/dag/selector.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dag/utils.py` & `merlin-core-23.6.0/merlin/dag/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dispatch/lazy.py` & `merlin-core-23.6.0/merlin/dispatch/lazy.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/__init__.py` & `merlin-core-23.6.0/merlin/dtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/aliases.py` & `merlin-core-23.6.0/merlin/dtypes/aliases.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/base.py` & `merlin-core-23.6.0/merlin/dtypes/base.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mapping.py` & `merlin-core-23.6.0/merlin/dtypes/mapping.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/__init__.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/cudf.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/cudf.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/merlin.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/merlin.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/numpy.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/numpy.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/pandas.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/pandas.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/python.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/python.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/tf.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/tf.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/torch.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/torch.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/mappings/triton.py` & `merlin-core-23.6.0/merlin/dtypes/mappings/triton.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/registry.py` & `merlin-core-23.6.0/merlin/dtypes/registry.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/dtypes/shape.py` & `merlin-core-23.6.0/merlin/dtypes/shape.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/__init__.py` & `merlin-core-23.6.0/merlin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/avro.py` & `merlin-core-23.6.0/merlin/io/avro.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/csv.py` & `merlin-core-23.6.0/merlin/io/csv.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/dask.py` & `merlin-core-23.6.0/merlin/io/dask.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/dataframe_engine.py` & `merlin-core-23.6.0/merlin/io/dataframe_engine.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/dataframe_iter.py` & `merlin-core-23.6.0/merlin/io/dataframe_iter.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/dataset.py` & `merlin-core-23.6.0/merlin/io/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,28 @@
 import logging
 import math
 import random
 import warnings
 from pathlib import Path
 
 import dask
+import distributed
 import numpy as np
 from dask.base import tokenize
 from dask.dataframe.core import new_dd_object
 from dask.highlevelgraph import HighLevelGraph
 from dask.utils import natural_sort_key, parse_bytes
 from fsspec.core import get_fs_token_paths
 from fsspec.utils import stringify_path
+from npy_append_array import NpyAppendArray
 
-from merlin.core.compat import HAS_GPU, cudf, device_mem_size
+from merlin.core.compat import HAS_GPU, cudf, dask_cudf, device_mem_size
 from merlin.core.dispatch import (
     convert_data,
+    dataframe_columnwise_explode,
     hex_to_int,
     is_dataframe_object,
     is_list_dtype,
     list_val_dtype,
 )
 from merlin.core.utils import global_dask_client, set_client_deprecated
 from merlin.dtypes.shape import DefaultShapes
@@ -419,15 +422,31 @@
             # Convert the HLG to a Dask collection
             divisions = [None] * (ddf.npartitions + 1)
             ddf = new_dd_object(new_graph, new_name, ddf._meta, divisions)
 
         # Special dtype conversion (optional)
         if self.dtypes:
             _meta = _set_dtypes(ddf._meta, self.dtypes)
-            return ddf.map_partitions(_set_dtypes, self.dtypes, meta=_meta)
+            ddf = ddf.map_partitions(_set_dtypes, self.dtypes, meta=_meta)
+
+        dask_client = global_dask_client()
+        if dask_client is not None:
+            # pylint: disable=unidiomatic-typecheck
+            if (
+                dask_cudf
+                and isinstance(ddf, dask_cudf.DataFrame)
+                and type(dask_client.cluster) is distributed.LocalCluster
+            ):
+                raise RuntimeError(
+                    "`dask_cudf.DataFrame` is incompatible with `distributed.LocalCluster`. "
+                    "Please setup a `dask_cuda.LocalCUDACluster` instead. "
+                    "Or to run on CPU instead, "
+                    "provide the parameter `cpu=True` when creating the `Dataset`. "
+                )
+
         return ddf
 
     @property
     def file_partition_map(self):
         return self.engine._file_partition_map
 
     @property
@@ -1063,14 +1082,49 @@
             labels,
             "hugectr",
             num_threads,
             self.cpu,
             schema=self.schema,
         )
 
+    def to_npy(
+        self,
+        output_file: str,
+        append: bool = False,
+    ):
+        """Converts a dataset into an npy file, can append if data is larger than memory
+
+        Parameters
+        ----------
+        output_file : str
+            The output file path for the resulting npy file
+        append : bool, optional
+            Enables append mode for larger that memory data, by default False
+        """
+        data = self.to_ddf()
+        if append:
+            data = Dataset(data)
+            itr = iter(data.to_iter())
+            with NpyAppendArray(output_file) as nf:
+                for df in itr:
+                    to_write = dataframe_columnwise_explode(df)
+                    # after the explode there may not be object series anymore
+                    if "object" in to_write.dtypes.values and append:
+                        raise TypeError("Cannot append object columns")
+                    if (to_write.isnull()).any().any():
+                        raise ValueError("Cannot convert data because null values were detected")
+                    nf.append(to_write.to_numpy())
+        else:
+            to_write = dataframe_columnwise_explode(data.compute())
+            if "object" in to_write.dtypes.values and append:
+                raise TypeError("Cannot append object columns")
+            if (to_write.isnull()).any().any():
+                raise ValueError("Cannot convert data because null values were detected")
+            np.save(output_file, to_write.to_numpy())
+
     @property
     def num_rows(self):
         return self.engine.num_rows
 
     @property
     def npartitions(self):
         return self.to_ddf().npartitions
```

### Comparing `merlin-core-23.5.0/merlin/io/dataset_engine.py` & `merlin-core-23.6.0/merlin/io/dataset_engine.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/fsspec_utils.py` & `merlin-core-23.6.0/merlin/io/fsspec_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/hugectr.py` & `merlin-core-23.6.0/merlin/io/hugectr.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/parquet.py` & `merlin-core-23.6.0/merlin/io/parquet.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/shuffle.py` & `merlin-core-23.6.0/merlin/io/shuffle.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/worker.py` & `merlin-core-23.6.0/merlin/io/worker.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/writer.py` & `merlin-core-23.6.0/merlin/io/writer.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/io/writer_factory.py` & `merlin-core-23.6.0/merlin/io/writer_factory.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/schema/__init__.py` & `merlin-core-23.6.0/merlin/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/schema/io/__init__.py` & `merlin-core-23.6.0/merlin/schema/io/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/schema/io/proto_utils.py` & `merlin-core-23.6.0/merlin/schema/io/proto_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/schema/io/schema_bp.py` & `merlin-core-23.6.0/merlin/schema/io/schema_bp.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/schema/io/tensorflow_metadata.py` & `merlin-core-23.6.0/merlin/schema/io/tensorflow_metadata.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/schema/schema.py` & `merlin-core-23.6.0/merlin/schema/schema.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/schema/tags.py` & `merlin-core-23.6.0/merlin/schema/tags.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/__init__.py` & `merlin-core-23.6.0/merlin/table/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/conversions.py` & `merlin-core-23.6.0/merlin/table/conversions.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/cupy_column.py` & `merlin-core-23.6.0/merlin/table/cupy_column.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/numpy_column.py` & `merlin-core-23.6.0/merlin/table/numpy_column.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/tensor_column.py` & `merlin-core-23.6.0/merlin/table/tensor_column.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/tensor_table.py` & `merlin-core-23.6.0/merlin/table/tensor_table.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/tensorflow_column.py` & `merlin-core-23.6.0/merlin/table/tensorflow_column.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/table/torch_column.py` & `merlin-core-23.6.0/merlin/table/torch_column.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin/testing/assert_equals.py` & `merlin-core-23.6.0/merlin/testing/assert_equals.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/merlin_core.egg-info/PKG-INFO` & `merlin-core-23.6.0/merlin_core.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-core
-Version: 23.5.0
+Version: 23.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/core
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `merlin-core-23.5.0/merlin_core.egg-info/SOURCES.txt` & `merlin-core-23.6.0/merlin_core.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -20,19 +20,23 @@
 merlin/dag/base_operator.py
 merlin/dag/executors.py
 merlin/dag/graph.py
 merlin/dag/node.py
 merlin/dag/selector.py
 merlin/dag/utils.py
 merlin/dag/ops/__init__.py
+merlin/dag/ops/add_metadata.py
 merlin/dag/ops/concat_columns.py
 merlin/dag/ops/rename.py
 merlin/dag/ops/selection.py
+merlin/dag/ops/stat_operator.py
+merlin/dag/ops/subgraph.py
 merlin/dag/ops/subset_columns.py
 merlin/dag/ops/subtraction.py
+merlin/dag/ops/udf.py
 merlin/dispatch/lazy.py
 merlin/dtypes/__init__.py
 merlin/dtypes/aliases.py
 merlin/dtypes/base.py
 merlin/dtypes/mapping.py
 merlin/dtypes/registry.py
 merlin/dtypes/shape.py
```

### Comparing `merlin-core-23.5.0/pyproject.toml` & `merlin-core-23.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/setup.cfg` & `merlin-core-23.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/setup.py` & `merlin-core-23.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-core-23.5.0/versioneer.py` & `merlin-core-23.6.0/versioneer.py`

 * *Files identical despite different names*

