# Comparing `tmp/sarus-0.7.2.tar.gz` & `tmp/sarus-0.7.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.7.2.tar", last modified: Tue Jun 13 07:37:39 2023, max compression
+gzip compressed data, was "sarus-0.7.3rc0.tar", last modified: Thu Jun 22 08:25:15 2023, max compression
```

## Comparing `sarus-0.7.2.tar` & `sarus-0.7.3rc0.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.544621 sarus-0.7.2/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.2/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-06-13 07:37:39.544621 sarus-0.7.2/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.2/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.2/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-06-13 07:36:24.000000 sarus-0.7.2/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/base_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     7988 2023-06-08 20:23:56.000000 sarus-0.7.2/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    20840 2023-06-08 20:23:56.000000 sarus-0.7.2/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    43589 2023-06-08 20:23:56.000000 sarus-0.7.2/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.544621 sarus-0.7.2/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.544621 sarus-0.7.2/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.544621 sarus-0.7.2/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.544621 sarus-0.7.2/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-06-07 13:55:59.000000 sarus-0.7.2/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.544621 sarus-0.7.2/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.2/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.540621 sarus-0.7.2/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-06-13 07:37:39.000000 sarus-0.7.2/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-06-13 07:37:39.000000 sarus-0.7.2/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-13 07:37:39.000000 sarus-0.7.2/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.2/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      342 2023-06-13 07:37:39.000000 sarus-0.7.2/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-06-13 07:37:39.000000 sarus-0.7.2/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-06-13 07:37:39.544621 sarus-0.7.2/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-06-13 07:36:16.000000 sarus-0.7.2/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-13 07:37:39.544621 sarus-0.7.2/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.2/tests/test_sanity.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/MANIFEST.in
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.7.3rc0/README.rst
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.7.3rc0/pyproject.toml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.750965 sarus-0.7.3rc0/sarus/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-06-13 07:36:24.000000 sarus-0.7.3rc0/sarus/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13201 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/config.yaml
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.750965 sarus-0.7.3rc0/sarus/context/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/context/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3137 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/context/local_sdk.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      345 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/context/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13990 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/dataspec_wrapper.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/debug.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.750965 sarus-0.7.3rc0/sarus/imblearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/imblearn/under_sampling.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.754965 sarus-0.7.3rc0/sarus/legacy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/legacy/__init__.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.754965 sarus-0.7.3rc0/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/legacy/tensorflow/model.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.758965 sarus-0.7.3rc0/sarus/manager/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     5490 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1927 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1296 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/base_remote.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3869 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     8719 2023-06-22 08:24:35.000000 sarus-0.7.3rc0/sarus/manager/dataspec_api.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.758965 sarus-0.7.3rc0/sarus/manager/ops/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      688 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/manager/ops/api.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     3487 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/parquet_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    20372 2023-06-22 08:24:35.000000 sarus-0.7.3rc0/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     2650 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/manager/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4729 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/value_local.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1573 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/manager/value_remote.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.758965 sarus-0.7.3rc0/sarus/numpy/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/numpy/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/numpy/random.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/numpy/scalars.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.758965 sarus-0.7.3rc0/sarus/pandas/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/pandas/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      838 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/pandas/core.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4843 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/pandas/io.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.758965 sarus-0.7.3rc0/sarus/pandas_profiling/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      377 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/pandas_profiling/profile_report.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.758965 sarus-0.7.3rc0/sarus/plotly/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/plotly/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/plotly/express.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    43028 2023-06-22 08:24:35.000000 sarus-0.7.3rc0/sarus/sarus.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.758965 sarus-0.7.3rc0/sarus/scripts/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/scripts/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     4672 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/scripts/generate_op_list.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/sarus/sklearn/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/compose.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/ensemble.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/impute.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1073 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1571 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/sklearn/svm.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/sarus/skopt/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/skopt/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/skopt/searchcv.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/sarus/std/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/std/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1600 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/std/types.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/sarus/tensorflow/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/tensorflow/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1831 2023-06-07 13:55:59.000000 sarus-0.7.3rc0/sarus/typing.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)    10848 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/utils.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/wrapper_factory.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/sarus/xgboost/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      754 2023-05-23 10:20:26.000000 sarus-0.7.3rc0/sarus/xgboost/xgboost.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.750965 sarus-0.7.3rc0/sarus.egg-info/
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1556 2023-06-22 08:25:15.000000 sarus-0.7.3rc0/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)     1965 2023-06-22 08:25:15.000000 sarus-0.7.3rc0/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-06-22 08:25:15.000000 sarus-0.7.3rc0/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.7.3rc0/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)      359 2023-06-22 08:25:15.000000 sarus-0.7.3rc0/sarus.egg-info/requires.txt
+-rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-06-22 08:25:15.000000 sarus-0.7.3rc0/sarus.egg-info/top_level.txt
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1321 2023-06-22 08:25:15.766965 sarus-0.7.3rc0/setup.cfg
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      109 2023-06-22 08:24:57.000000 sarus-0.7.3rc0/setup.py
+drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-06-22 08:25:15.762965 sarus-0.7.3rc0/tests/
+-rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.7.3rc0/tests/test_sanity.py
```

### Comparing `sarus-0.7.2/PKG-INFO` & `sarus-0.7.3rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.2
+Version: 0.7.3rc0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.2/README.rst` & `sarus-0.7.3rc0/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/__init__.py` & `sarus-0.7.3rc0/sarus/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/config.yaml` & `sarus-0.7.3rc0/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/context/local_sdk.py` & `sarus-0.7.3rc0/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/dataspec_wrapper.py` & `sarus-0.7.3rc0/sarus/dataspec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/debug.py` & `sarus-0.7.3rc0/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/imblearn/over_sampling.py` & `sarus-0.7.3rc0/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/imblearn/pipeline.py` & `sarus-0.7.3rc0/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/imblearn/under_sampling.py` & `sarus-0.7.3rc0/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/legacy/tensorflow/dataset.py` & `sarus-0.7.3rc0/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/legacy/tensorflow/model.py` & `sarus-0.7.3rc0/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/arrow_local.py` & `sarus-0.7.3rc0/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/arrow_remote.py` & `sarus-0.7.3rc0/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/base_remote.py` & `sarus-0.7.3rc0/sarus/manager/base_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/cache_scalar_local.py` & `sarus-0.7.3rc0/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/dataspec_api.py` & `sarus-0.7.3rc0/sarus/manager/dataspec_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import sarus_data_spec.protobuf as sp
 import sarus_data_spec.typing as st
 from requests import Response
 from sarus_data_spec.constants import (
     BEST_ALTERNATIVE,
     CONSTRAINT_KIND,
     PRIVACY_LIMIT,
+    SCHEMA_TASK,
 )
 from sarus_data_spec.dataspec_validator.typing import DataspecPrivacyPolicy
 from sarus_data_spec.manager.async_utils import async_iter
 from sarus_data_spec.protobuf.utilities import dict_deserialize, dict_serialize
 
 from sarus.typing import Client
 
@@ -77,15 +78,15 @@
     return epsilon
 
 
 def pull_dataspec_graph(client: Client, uuid: str) -> None:
     """Fetch a dataspec's computation graph and store it."""
     start = time.perf_counter()
     resp: Response = client.session().get(
-        f"{client.url()}/dataspecs/{uuid}/graph",
+        f"{client.url()}/dataspecs/{uuid}/graph"
     )
     end = time.perf_counter()
     logger.debug(
         f"GET /dataspecs/{uuid}/graph {resp.status_code} ({end-start:.2f}s)"
     )
     raise_response(resp)
 
@@ -93,14 +94,35 @@
     referrables = [
         client.context().factory().create(proto, store=False)
         for proto in protos
     ]
     client.context().storage().batch_store(referrables)
 
 
+def pull_dataspec_schema(client: Client, uuid: str) -> None:
+    """Fetch a dataspec's computation graph and store it."""
+    start = time.perf_counter()
+    resp: Response = client.session().get(
+        f"{client.url()}/dataspecs/{uuid}/schema"
+    )
+    end = time.perf_counter()
+    logger.debug(
+        f"GET /dataspecs/{uuid}/schema {resp.status_code} ({end-start:.2f}s)"
+    )
+    raise_response(resp)
+
+    dataspec = client.context().storage().referrable(uuid)
+    proto_schema = dict_deserialize(resp.json()["schema"])
+    schema = client.context().factory().create(proto_schema)
+    client.context().manager().copy_status_from_server(
+        dataspec, task_names=[SCHEMA_TASK]
+    )
+    return schema
+
+
 def push_dataspec_graph(client: Client, graph: t.List[st.Referrable]) -> None:
     """Push a list of referrables to the server."""
     start = time.perf_counter()
     resp: Response = client.session().post(
         f"{client.url()}/dataspecs/graph",
         json=[dict_serialize(ref.protobuf()) for ref in graph],
     )
```

### Comparing `sarus-0.7.2/sarus/manager/ops/api.py` & `sarus-0.7.3rc0/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/parquet_local.py` & `sarus-0.7.3rc0/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/sdk_manager.py` & `sarus-0.7.3rc0/sarus/manager/sdk_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -455,30 +455,17 @@
             computation_graph = self.computation_graph(dataset)
             referrables = (
                 list(computation_graph["dataspecs"])
                 + list(computation_graph["transforms"])
                 + list(computation_graph["attributes"])
             )
             api.push_dataspec_graph(self._client, referrables)
-            parent_schema = await self.async_schema(dataset.parents()[0][0])
-            iterator = await self.async_to_arrow(dataset, batch_size=1000)
-            table = pa.Table.from_batches([batch async for batch in iterator])
-            fields = {
-                col: type_from_arrow(
-                    arrow_type=table.field(col).type,
-                    nullable=table.field(col).nullable,
-                )
-                for col in table.schema.names
-            }
-            schema_type = sdt.Struct(fields=fields)
-            return schema_builder(
-                dataset,
-                schema_type=schema_type,
-                name=parent_schema.name(),
-            )
+            # TODO: remove when we can compute the pep token of select SQL in SDK
+            api.pull_dataspec_graph(self._client, dataset.uuid())
+            return api.pull_dataspec_schema(self._client, dataset.uuid())
 
         if dataset.is_transformed():
             return await TransformedDataset(dataset).schema()
         else:
             raise ValueError('Dataset should be transformed.')
 
     async def async_to_arrow_op(
```

### Comparing `sarus-0.7.2/sarus/manager/typing.py` & `sarus-0.7.3rc0/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/value_local.py` & `sarus-0.7.3rc0/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/manager/value_remote.py` & `sarus-0.7.3rc0/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/numpy/scalars.py` & `sarus-0.7.3rc0/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/pandas/core.py` & `sarus-0.7.3rc0/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/pandas/dataframe.py` & `sarus-0.7.3rc0/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sarus.py` & `sarus-0.7.3rc0/sarus/sarus.py`

 * *Files 3% similar despite different names*

```diff
@@ -239,43 +239,25 @@
             client.context()
             .factory()
             .create(
                 dict_deserialize(serialized_dataspec["dataset"]), store=False
             )
         )
         pull_dataspec_graph(client=client, uuid=dataspec.uuid())
-        manager.set_remote(dataspec)
 
-        syn_dataset_uuid, _ = compile_dataspec(
-            client=client,
-            uuid=dataspec.uuid(),
-            constraint_kind=st.ConstraintKind.SYNTHETIC,
-        )
-
-        pull_dataspec_graph(client=client, uuid=syn_dataset_uuid)
-
-        syn_dataset: st.Dataset = (
-            client.context().storage().referrable(syn_dataset_uuid)
-        )
+        syn_dataset: st.Dataset = dataspec.variant(st.ConstraintKind.SYNTHETIC)
 
         # Update statuses
         dataspec.manager().copy_status_from_server(
             dataspec, task_names=[SCHEMA_TASK]
         )
         dataspec.manager().copy_status_from_server(
             syn_dataset, task_names=[SCHEMA_TASK]
         )
 
-        # Create mock
-        mock_dataset: st.Dataset = extract(size=dataspec.manager()._mock_size)(
-            syn_dataset
-        )
-        mock_constraint(mock_dataset)
-        attach_variant(dataspec, mock_dataset, st.ConstraintKind.MOCK)
-
         # TODO fetch the PEP token from the API
         # (it is lazily computed on the server)
         h = hashlib.md5()
         h.update(dataspec.protobuf().SerializeToString())
         pep_token = h.hexdigest()
         pep_constraint(
             dataspec=dataspec,
```

### Comparing `sarus-0.7.2/sarus/scripts/generate_op_list.py` & `sarus-0.7.3rc0/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/__init__.py` & `sarus-0.7.3rc0/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/cluster.py` & `sarus-0.7.3rc0/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/compose.py` & `sarus-0.7.3rc0/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/decomposition.py` & `sarus-0.7.3rc0/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/ensemble.py` & `sarus-0.7.3rc0/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/impute.py` & `sarus-0.7.3rc0/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/linear_model.py` & `sarus-0.7.3rc0/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/model_selection.py` & `sarus-0.7.3rc0/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/pipeline.py` & `sarus-0.7.3rc0/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/preprocessing.py` & `sarus-0.7.3rc0/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/sklearn/svm.py` & `sarus-0.7.3rc0/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/skopt/searchcv.py` & `sarus-0.7.3rc0/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/std/types.py` & `sarus-0.7.3rc0/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/typing.py` & `sarus-0.7.3rc0/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/utils.py` & `sarus-0.7.3rc0/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/wrapper_factory.py` & `sarus-0.7.3rc0/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus/xgboost/xgboost.py` & `sarus-0.7.3rc0/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/sarus.egg-info/PKG-INFO` & `sarus-0.7.3rc0/sarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.7.2
+Version: 0.7.3rc0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
 Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
 Keywords: differential privacy,AI,Data privacy
```

### Comparing `sarus-0.7.2/sarus.egg-info/SOURCES.txt` & `sarus-0.7.3rc0/sarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sarus-0.7.2/setup.cfg` & `sarus-0.7.3rc0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -20,17 +20,18 @@
 
 [options]
 zip_safe = False
 python_requires = >=3.7, <3.11
 packages = find:
 include_package_data = True
 install_requires = 
-	sarus-data-spec-public==3.5.0
+	sarus-data-spec-public==3.5.5
 	cloudpickle>=1.2, <2.1
 	pyarrow >= 11.0
+	protobuf >= 3.20.3
 
 [options.extras_require]
 sklearn = 
 	scikit-learn==1.2.2
 	scipy==1.9.0
 imblearn = 
 	imbalanced-learn
```

