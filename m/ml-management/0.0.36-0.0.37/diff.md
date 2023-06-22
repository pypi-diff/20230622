# Comparing `tmp/ml-management-0.0.36.tar.gz` & `tmp/ml-management-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-management-0.0.36.tar", last modified: Tue Jun 13 14:34:11 2023, max compression
+gzip compressed data, was "ml-management-0.0.37.tar", last modified: Thu Jun 22 14:46:10 2023, max compression
```

## Comparing `ml-management-0.0.36.tar` & `ml-management-0.0.37.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.051743 ml-management-0.0.36/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       18 2023-05-04 09:01:13.000000 ml-management-0.0.36/MANIFEST.in
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/__init__.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/collectors/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      120 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1092 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/collector_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      456 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/collectors/collector_pattern_to_methods_map.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1318 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/collectors/collectors.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/collectors/dummy/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/dummy/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      463 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/collectors/dummy/dummy_collector.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.039743 ml-management-0.0.36/ML_management/collectors/s3/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/s3/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    10609 2023-06-13 11:06:20.000000 ml-management-0.0.36/ML_management/collectors/s3/s3collector.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/collectors/topic_markers/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/collectors/topic_markers/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)   331440 2023-06-07 09:26:42.000000 ml-management-0.0.36/ML_management/collectors/topic_markers/api_schema.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3167 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/collectors/topic_markers/topic_markers_collector.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/dataset_loader_template/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/dataset_loader_template/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2407 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/dataset_loader_template/dataset_loader_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/executor_template/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/executor_template/__init__.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.043743 ml-management-0.0.36/ML_management/executor_template/default_executors/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      895 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/finetune_executor.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      843 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/test_executor.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      869 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/executor_template/default_executors/train_executor.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4566 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/executor_template/executor_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      402 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/executor_template/executor_pattern_to_methods_map.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      334 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/executor_template/upload_model_mode.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/mlmanagement/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      581 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/mlmanagement/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3392 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/mlmanagement/jsonschema_exceptions.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5054 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/mlmanagement/jsonschema_inference.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    13486 2023-06-08 10:13:29.000000 ml-management-0.0.36/ML_management/mlmanagement/mlmanagement.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)    10262 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/mlmanagement/mlmanager.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      201 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/mlmanagement/model_type.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     5001 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/mlmanagement/server_mlmanager_exceptions.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      316 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/mlmanagement/utils.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/models/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/models/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      949 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/model_type_to_methods_map.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/models/patterns/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     4202 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/models/patterns/model_pattern.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      561 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/retrainable_model.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      445 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/torch_model.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      457 2023-05-16 09:30:47.000000 ml-management-0.0.36/ML_management/models/patterns/trainable_model.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/registry/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/registry/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2566 2023-06-07 09:26:35.000000 ml-management-0.0.36/ML_management/registry/exceptions.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     7556 2023-06-09 12:23:31.000000 ml-management-0.0.36/ML_management/registry/registry_manager.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.047743 ml-management-0.0.36/ML_management/tests/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/tests/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     3361 2023-05-04 09:01:13.000000 ml-management-0.0.36/ML_management/tests/test_jsonschema_inference.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     9275 2023-06-13 11:06:20.000000 ml-management-0.0.36/ML_management/tests/test_s3_dataset.py
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.051743 ml-management-0.0.36/ML_management/uploader_data/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        0 2023-05-22 12:29:29.000000 ml-management-0.0.36/ML_management/uploader_data/__init__.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1694 2023-06-13 11:06:20.000000 ml-management-0.0.36/ML_management/uploader_data/s3_uploader.py
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      367 2023-06-13 14:34:11.051743 ml-management-0.0.36/PKG-INFO
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       56 2023-05-04 09:01:13.000000 ml-management-0.0.36/README.md
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        7 2023-06-13 14:30:58.000000 ml-management-0.0.36/VERSION
-drwxrwxr-x   0 mizykov   (1001) mizykov   (1001)        0 2023-06-13 14:34:11.051743 ml-management-0.0.36/ml_management.egg-info/
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      367 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/PKG-INFO
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     2449 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/SOURCES.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)        1 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/dependency_links.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)      154 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/requires.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       14 2023-06-13 14:34:11.000000 ml-management-0.0.36/ml_management.egg-info/top_level.txt
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)       38 2023-06-13 14:34:11.051743 ml-management-0.0.36/setup.cfg
--rw-rw-r--   0 mizykov   (1001) mizykov   (1001)     1053 2023-06-07 09:12:12.000000 ml-management-0.0.36/setup.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.843464 ml-management-0.0.37/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       18 2023-02-15 13:35:59.000000 ml-management-0.0.37/MANIFEST.in
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/__init__.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      120 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1092 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/collector_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      456 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/collector_pattern_to_methods_map.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1318 2023-06-01 12:44:21.000000 ml-management-0.0.37/ML_management/collectors/collectors.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/dummy/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/dummy/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      463 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/dummy/dummy_collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/s3/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/s3/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10609 2023-06-19 11:21:46.000000 ml-management-0.0.37/ML_management/collectors/s3/s3collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/collectors/topic_markers/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/topic_markers/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)   331440 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/topic_markers/api_schema.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3167 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/collectors/topic_markers/topic_markers_collector.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/dataset_loader_template/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/dataset_loader_template/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2407 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/dataset_loader_template/dataset_loader_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/dataset_loader_template/dataset_loader_pattern_to_methods_map.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/executor_template/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/__init__.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/executor_template/default_executors/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      895 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/finetune_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      843 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/test_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      869 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/default_executors/train_executor.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4566 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/executor_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      402 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/executor_pattern_to_methods_map.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      334 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/executor_template/upload_model_mode.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/mlmanagement/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      581 2023-03-13 10:54:54.000000 ml-management-0.0.37/ML_management/mlmanagement/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3392 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/jsonschema_exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5054 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/jsonschema_inference.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    13550 2023-06-22 14:43:51.000000 ml-management-0.0.37/ML_management/mlmanagement/mlmanagement.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)    10262 2023-06-02 13:31:58.000000 ml-management-0.0.37/ML_management/mlmanagement/mlmanager.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      201 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/model_type.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     5001 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/server_mlmanager_exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      316 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/mlmanagement/utils.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/models/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/models/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      949 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/model_type_to_methods_map.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/models/patterns/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     4202 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/model_pattern.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      561 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/retrainable_model.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      445 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/torch_model.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      457 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/models/patterns/trainable_model.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/registry/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/registry/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2566 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/registry/exceptions.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     7556 2023-06-13 13:01:13.000000 ml-management-0.0.37/ML_management/registry/registry_manager.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/tests/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/tests/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     3361 2023-02-15 13:35:59.000000 ml-management-0.0.37/ML_management/tests/test_jsonschema_inference.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     9275 2023-06-19 11:21:46.000000 ml-management-0.0.37/ML_management/tests/test_s3_dataset.py
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ML_management/uploader_data/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        0 2023-05-26 11:00:04.000000 ml-management-0.0.37/ML_management/uploader_data/__init__.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1694 2023-06-19 11:21:46.000000 ml-management-0.0.37/ML_management/uploader_data/s3_uploader.py
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-06-22 14:46:10.839464 ml-management-0.0.37/PKG-INFO
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       56 2023-02-15 13:35:59.000000 ml-management-0.0.37/README.md
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        7 2023-06-22 14:45:56.000000 ml-management-0.0.37/VERSION
+drwxrwxr-x   0 kochetkov  (1000) kochetkov  (1000)        0 2023-06-22 14:46:10.839464 ml-management-0.0.37/ml_management.egg-info/
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      312 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/PKG-INFO
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     2449 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/SOURCES.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)        1 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/dependency_links.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)      154 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/requires.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       14 2023-06-22 14:46:10.000000 ml-management-0.0.37/ml_management.egg-info/top_level.txt
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)       38 2023-06-22 14:46:10.843464 ml-management-0.0.37/setup.cfg
+-rw-rw-r--   0 kochetkov  (1000) kochetkov  (1000)     1053 2023-06-01 12:44:21.000000 ml-management-0.0.37/setup.py
```

### Comparing `ml-management-0.0.36/ML_management/collectors/collector_pattern.py` & `ml-management-0.0.37/ML_management/collectors/collector_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/collectors/collectors.py` & `ml-management-0.0.37/ML_management/collectors/collectors.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/collectors/s3/s3collector.py` & `ml-management-0.0.37/ML_management/collectors/s3/s3collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/collectors/topic_markers/api_schema.py` & `ml-management-0.0.37/ML_management/collectors/topic_markers/api_schema.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/collectors/topic_markers/topic_markers_collector.py` & `ml-management-0.0.37/ML_management/collectors/topic_markers/topic_markers_collector.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/dataset_loader_template/dataset_loader_pattern.py` & `ml-management-0.0.37/ML_management/dataset_loader_template/dataset_loader_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/executor_template/default_executors/finetune_executor.py` & `ml-management-0.0.37/ML_management/executor_template/default_executors/finetune_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/executor_template/default_executors/test_executor.py` & `ml-management-0.0.37/ML_management/executor_template/default_executors/test_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/executor_template/default_executors/train_executor.py` & `ml-management-0.0.37/ML_management/executor_template/default_executors/train_executor.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/executor_template/executor_pattern.py` & `ml-management-0.0.37/ML_management/executor_template/executor_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/mlmanagement/__init__.py` & `ml-management-0.0.37/ML_management/mlmanagement/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/mlmanagement/jsonschema_exceptions.py` & `ml-management-0.0.37/ML_management/mlmanagement/jsonschema_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/mlmanagement/jsonschema_inference.py` & `ml-management-0.0.37/ML_management/mlmanagement/jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/mlmanagement/mlmanagement.py` & `ml-management-0.0.37/ML_management/mlmanagement/mlmanagement.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,16 @@
     active_run_stack.append(_active_run)
     return _active_run
 
 
 def _add_job_registration_metainfo(
     registration_timestamp,
     init_model_version_run_id,
+    dataset_loader_version_run_id,
+    executor_version_run_id,
     name,
     job_executor_name,
     job_executor_version,
     dataset_loader_name,
     dataset_loader_version,
     model_name,
     model_version,
```

### Comparing `ml-management-0.0.36/ML_management/mlmanagement/mlmanager.py` & `ml-management-0.0.37/ML_management/mlmanagement/mlmanager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/mlmanagement/server_mlmanager_exceptions.py` & `ml-management-0.0.37/ML_management/mlmanagement/server_mlmanager_exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/models/model_type_to_methods_map.py` & `ml-management-0.0.37/ML_management/models/model_type_to_methods_map.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/models/patterns/model_pattern.py` & `ml-management-0.0.37/ML_management/models/patterns/model_pattern.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/models/patterns/retrainable_model.py` & `ml-management-0.0.37/ML_management/models/patterns/retrainable_model.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/registry/exceptions.py` & `ml-management-0.0.37/ML_management/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/registry/registry_manager.py` & `ml-management-0.0.37/ML_management/registry/registry_manager.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/tests/test_jsonschema_inference.py` & `ml-management-0.0.37/ML_management/tests/test_jsonschema_inference.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/tests/test_s3_dataset.py` & `ml-management-0.0.37/ML_management/tests/test_s3_dataset.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ML_management/uploader_data/s3_uploader.py` & `ml-management-0.0.37/ML_management/uploader_data/s3_uploader.py`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/ml_management.egg-info/SOURCES.txt` & `ml-management-0.0.37/ml_management.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-management-0.0.36/setup.py` & `ml-management-0.0.37/setup.py`

 * *Files identical despite different names*

