# Comparing `tmp/trainml-0.4.9.tar.gz` & `tmp/trainml-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/trainml-0.4.9.tar", last modified: Tue Jan 17 22:35:28 2023, max compression
+gzip compressed data, was "trainml-0.5.0.tar", last modified: Thu Jun 22 02:51:26 2023, max compression
```

## Comparing `trainml-0.4.9.tar` & `trainml-0.5.0.tar`

### file list

```diff
@@ -1,78 +1,114 @@
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.839909 trainml-0.4.9/
--rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.4.9/LICENSE
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-01-17 22:35:28.839337 trainml-0.4.9/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.4.9/README.md
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.791775 trainml-0.4.9/examples/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.4.9/examples/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.4.9/examples/create_dataset_and_training_job.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.4.9/examples/local_storage.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2333 2023-01-10 21:57:07.000000 trainml-0.4.9/examples/training_inference_pipeline.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      710 2023-01-05 20:17:55.000000 trainml-0.4.9/pyproject.toml
--rw-r--r--   0 akowalsk   (501) staff       (20)       38 2023-01-17 22:35:28.840079 trainml-0.4.9/setup.cfg
--rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.4.9/setup.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.785582 trainml-0.4.9/tests/
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.801964 trainml-0.4.9/tests/integration/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.4.9/tests/integration/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.4.9/tests/integration/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3116 2023-01-05 21:36:25.000000 trainml-0.4.9/tests/integration/test_checkpoints_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3412 2023-01-05 20:33:29.000000 trainml-0.4.9/tests/integration/test_datasets_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1391 2021-03-11 02:41:10.000000 trainml-0.4.9/tests/integration/test_environments_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2022-02-07 16:08:41.000000 trainml-0.4.9/tests/integration/test_gpu_types_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    23476 2023-01-10 22:21:04.000000 trainml-0.4.9/tests/integration/test_jobs_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2835 2022-09-22 16:37:05.000000 trainml-0.4.9/tests/integration/test_models_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1480 2021-09-28 14:24:02.000000 trainml-0.4.9/tests/integration/test_projects_integration.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2023-01-10 22:00:20.000000 trainml-0.4.9/tests/integration/test_providers_integration.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.814977 trainml-0.4.9/tests/unit/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.4.9/tests/unit/__init__.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.816956 trainml-0.4.9/tests/unit/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.4.9/tests/unit/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.4.9/tests/unit/cli/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      683 2021-03-12 19:19:14.000000 trainml-0.4.9/tests/unit/cli/test_cli_environment_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20053 2023-01-10 22:45:56.000000 trainml-0.4.9/tests/unit/conftest.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      815 2021-03-11 02:25:33.000000 trainml-0.4.9/tests/unit/test_auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15935 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_checkpoints_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_connections_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15815 2023-01-16 16:42:32.000000 trainml-0.4.9/tests/unit/test_datasets_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2021-03-11 02:32:19.000000 trainml-0.4.9/tests/unit/test_environments_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.4.9/tests/unit/test_exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1703 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_gpu_types_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26446 2023-01-10 22:45:55.000000 trainml-0.4.9/tests/unit/test_jobs_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    15021 2023-01-16 16:42:31.000000 trainml-0.4.9/tests/unit/test_models_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3803 2021-12-07 17:57:14.000000 trainml-0.4.9/tests/unit/test_projects_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3700 2022-11-03 18:50:49.000000 trainml-0.4.9/tests/unit/test_providers_unit.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.4.9/tests/unit/test_trainml.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.827826 trainml-0.4.9/trainml/
--rw-r--r--   0 akowalsk   (501) staff       (20)      422 2023-01-17 22:34:22.000000 trainml-0.4.9/trainml/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.4.9/trainml/__main__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    26446 2022-04-16 18:55:57.000000 trainml-0.4.9/trainml/auth.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     7156 2023-01-10 22:09:49.000000 trainml-0.4.9/trainml/checkpoints.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.836458 trainml-0.4.9/trainml/cli/
--rw-r--r--   0 akowalsk   (501) staff       (20)     4322 2023-01-17 21:52:08.000000 trainml-0.4.9/trainml/cli/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6526 2023-01-10 22:10:42.000000 trainml-0.4.9/trainml/cli/checkpoint.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2022-08-29 15:36:54.000000 trainml-0.4.9/trainml/cli/connection.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6285 2022-09-19 22:07:28.000000 trainml-0.4.9/trainml/cli/dataset.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2021-08-20 02:02:59.000000 trainml-0.4.9/trainml/cli/environment.py
--rw-r--r--   0 akowalsk   (501) staff       (20)      919 2022-02-08 15:46:35.000000 trainml-0.4.9/trainml/cli/gpu.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.837749 trainml-0.4.9/trainml/cli/job/
--rw-r--r--   0 akowalsk   (501) staff       (20)     6544 2022-09-19 22:08:20.000000 trainml-0.4.9/trainml/cli/job/__init__.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    33021 2023-01-16 20:15:17.000000 trainml-0.4.9/trainml/cli/job/create.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     5509 2022-09-19 22:07:15.000000 trainml-0.4.9/trainml/cli/model.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1654 2021-09-15 16:00:52.000000 trainml-0.4.9/trainml/cli/project.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1594 2023-01-17 21:53:43.000000 trainml-0.4.9/trainml/cli/provider.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    20059 2023-01-10 14:50:42.000000 trainml-0.4.9/trainml/connections.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6951 2023-01-16 16:41:50.000000 trainml-0.4.9/trainml/datasets.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1537 2021-02-11 18:25:46.000000 trainml-0.4.9/trainml/environments.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     3724 2023-01-05 20:17:59.000000 trainml-0.4.9/trainml/exceptions.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1831 2022-02-07 15:42:56.000000 trainml-0.4.9/trainml/gpu_types.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    16710 2023-01-10 21:47:55.000000 trainml-0.4.9/trainml/jobs.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     6620 2023-01-16 16:42:01.000000 trainml-0.4.9/trainml/models.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     2009 2021-12-07 17:49:13.000000 trainml-0.4.9/trainml/projects.py
--rw-r--r--   0 akowalsk   (501) staff       (20)     1844 2022-11-03 18:21:21.000000 trainml-0.4.9/trainml/providers.py
--rw-r--r--   0 akowalsk   (501) staff       (20)    10618 2023-01-05 20:17:57.000000 trainml-0.4.9/trainml/trainml.py
-drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-01-17 22:35:28.830721 trainml-0.4.9/trainml.egg-info/
--rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/PKG-INFO
--rw-r--r--   0 akowalsk   (501) staff       (20)     1877 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/SOURCES.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)        1 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/dependency_links.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       63 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/entry_points.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       67 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/requires.txt
--rw-r--r--   0 akowalsk   (501) staff       (20)       23 2023-01-17 22:35:28.000000 trainml-0.4.9/trainml.egg-info/top_level.txt
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.728306 trainml-0.5.0/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1069 2021-01-24 17:36:29.000000 trainml-0.5.0/LICENSE
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-06-22 02:51:26.728036 trainml-0.5.0/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6734 2021-09-29 15:45:34.000000 trainml-0.5.0/README.md
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.706520 trainml-0.5.0/examples/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-19 16:26:24.000000 trainml-0.5.0/examples/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1178 2023-01-10 21:56:22.000000 trainml-0.5.0/examples/create_dataset_and_training_job.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1745 2023-01-10 21:56:46.000000 trainml-0.5.0/examples/local_storage.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2334 2023-01-22 22:47:55.000000 trainml-0.5.0/examples/training_inference_pipeline.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      945 2023-06-16 17:00:39.000000 trainml-0.5.0/pyproject.toml
+-rw-r--r--   0 akowalsk   (501) staff       (20)       38 2023-06-22 02:51:26.728348 trainml-0.5.0/setup.cfg
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1226 2021-03-31 16:56:30.000000 trainml-0.5.0/setup.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.704725 trainml-0.5.0/tests/
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.708912 trainml-0.5.0/tests/integration/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:47.000000 trainml-0.5.0/tests/integration/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.709279 trainml-0.5.0/tests/integration/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-19 19:22:07.000000 trainml-0.5.0/tests/integration/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1473 2023-06-19 19:31:30.000000 trainml-0.5.0/tests/integration/cloudbender/test_providers_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1134 2021-06-23 16:25:57.000000 trainml-0.5.0/tests/integration/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3128 2023-03-20 21:28:50.000000 trainml-0.5.0/tests/integration/test_checkpoints_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3424 2023-03-20 21:28:58.000000 trainml-0.5.0/tests/integration/test_datasets_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1403 2023-03-20 21:29:08.000000 trainml-0.5.0/tests/integration/test_environments_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1256 2023-03-20 21:29:14.000000 trainml-0.5.0/tests/integration/test_gpu_types_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    23496 2023-06-03 13:16:22.000000 trainml-0.5.0/tests/integration/test_jobs_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2848 2023-03-20 21:29:23.000000 trainml-0.5.0/tests/integration/test_models_integration.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1492 2023-03-20 21:29:29.000000 trainml-0.5.0/tests/integration/test_projects_integration.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.712437 trainml-0.5.0/tests/unit/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-02-11 14:59:48.000000 trainml-0.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.714211 trainml-0.5.0/tests/unit/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2021-03-11 02:10:08.000000 trainml-0.5.0/tests/unit/cli/__init__.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.715726 trainml-0.5.0/tests/unit/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-21 01:22:34.000000 trainml-0.5.0/tests/unit/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1381 2023-06-22 02:19:34.000000 trainml-0.5.0/tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1316 2023-06-21 02:49:51.000000 trainml-0.5.0/tests/unit/cli/cloudbender/test_cli_node_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      781 2023-06-21 01:49:51.000000 trainml-0.5.0/tests/unit/cli/cloudbender/test_cli_provider_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1262 2023-06-21 02:10:35.000000 trainml-0.5.0/tests/unit/cli/cloudbender/test_cli_region_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1407 2023-06-22 02:20:03.000000 trainml-0.5.0/tests/unit/cli/cloudbender/test_cli_reservation_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      236 2021-03-11 02:43:04.000000 trainml-0.5.0/tests/unit/cli/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      702 2023-06-22 01:39:48.000000 trainml-0.5.0/tests/unit/cli/test_cli_checkpoint_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      653 2023-06-22 01:40:30.000000 trainml-0.5.0/tests/unit/cli/test_cli_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      683 2023-06-21 00:35:39.000000 trainml-0.5.0/tests/unit/cli/test_cli_environment_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      650 2023-06-21 00:36:29.000000 trainml-0.5.0/tests/unit/cli/test_cli_gpu_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      611 2023-06-22 01:49:26.000000 trainml-0.5.0/tests/unit/cli/test_cli_job_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      629 2023-06-22 01:42:02.000000 trainml-0.5.0/tests/unit/cli/test_cli_model_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1756 2023-06-22 01:48:21.000000 trainml-0.5.0/tests/unit/cli/test_cli_project_unit.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.717806 trainml-0.5.0/tests/unit/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)        0 2023-06-16 16:46:40.000000 trainml-0.5.0/tests/unit/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4644 2023-06-19 18:30:44.000000 trainml-0.5.0/tests/unit/cloudbender/test_datastores_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4858 2023-06-19 18:41:08.000000 trainml-0.5.0/tests/unit/cloudbender/test_device_configs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4686 2023-06-19 18:22:11.000000 trainml-0.5.0/tests/unit/cloudbender/test_nodes_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3730 2023-06-19 16:30:35.000000 trainml-0.5.0/tests/unit/cloudbender/test_providers_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5635 2023-06-19 19:02:40.000000 trainml-0.5.0/tests/unit/cloudbender/test_regions_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4827 2023-06-19 18:34:29.000000 trainml-0.5.0/tests/unit/cloudbender/test_reservations_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    27336 2023-06-22 01:51:34.000000 trainml-0.5.0/tests/unit/conftest.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      815 2023-03-20 20:29:56.000000 trainml-0.5.0/tests/unit/test_auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    16008 2023-03-31 21:38:18.000000 trainml-0.5.0/tests/unit/test_checkpoints_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5507 2023-01-10 22:45:55.000000 trainml-0.5.0/tests/unit/test_connections_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15879 2023-03-31 21:39:46.000000 trainml-0.5.0/tests/unit/test_datasets_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1882 2023-06-04 18:32:37.000000 trainml-0.5.0/tests/unit/test_environments_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      906 2021-03-11 02:25:50.000000 trainml-0.5.0/tests/unit/test_exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2054 2023-06-21 20:53:31.000000 trainml-0.5.0/tests/unit/test_gpu_types_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26835 2023-06-04 18:29:09.000000 trainml-0.5.0/tests/unit/test_jobs_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    15064 2023-03-31 21:39:17.000000 trainml-0.5.0/tests/unit/test_models_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     9530 2023-06-22 01:37:38.000000 trainml-0.5.0/tests/unit/test_projects_unit.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1701 2021-03-11 02:26:10.000000 trainml-0.5.0/tests/unit/test_trainml.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.721077 trainml-0.5.0/trainml/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      432 2023-06-22 02:50:42.000000 trainml-0.5.0/trainml/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)       59 2021-02-24 01:47:01.000000 trainml-0.5.0/trainml/__main__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    26646 2023-04-11 15:08:13.000000 trainml-0.5.0/trainml/auth.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8274 2023-06-19 18:43:35.000000 trainml-0.5.0/trainml/checkpoints.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.723592 trainml-0.5.0/trainml/cli/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     4338 2023-06-19 19:39:43.000000 trainml-0.5.0/trainml/cli/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7170 2023-06-19 19:34:08.000000 trainml-0.5.0/trainml/cli/checkpoint.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.724905 trainml-0.5.0/trainml/cli/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)      484 2023-06-22 02:17:53.000000 trainml-0.5.0/trainml/cli/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3478 2023-06-22 02:11:56.000000 trainml-0.5.0/trainml/cli/cloudbender/datastore.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3843 2023-06-22 02:09:01.000000 trainml-0.5.0/trainml/cli/cloudbender/node.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1726 2023-06-22 02:09:04.000000 trainml-0.5.0/trainml/cli/cloudbender/provider.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     2892 2023-06-22 02:09:07.000000 trainml-0.5.0/trainml/cli/cloudbender/region.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3569 2023-06-22 02:14:39.000000 trainml-0.5.0/trainml/cli/cloudbender/reservation.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1700 2023-06-19 19:34:11.000000 trainml-0.5.0/trainml/cli/connection.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6893 2023-06-19 19:34:12.000000 trainml-0.5.0/trainml/cli/dataset.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1019 2023-06-19 19:34:12.000000 trainml-0.5.0/trainml/cli/environment.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      883 2023-06-19 19:40:03.000000 trainml-0.5.0/trainml/cli/gpu.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.725456 trainml-0.5.0/trainml/cli/job/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6545 2023-06-19 19:34:17.000000 trainml-0.5.0/trainml/cli/job/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    34652 2023-06-19 19:34:17.000000 trainml-0.5.0/trainml/cli/job/create.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     6071 2023-06-19 19:34:14.000000 trainml-0.5.0/trainml/cli/model.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3522 2023-06-21 21:09:43.000000 trainml-0.5.0/trainml/cli/project.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.727454 trainml-0.5.0/trainml/cloudbender/
+-rw-r--r--   0 akowalsk   (501) staff       (20)       64 2023-06-16 13:41:42.000000 trainml-0.5.0/trainml/cloudbender/__init__.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)      565 2023-06-16 16:35:20.000000 trainml-0.5.0/trainml/cloudbender/cloudbender.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3245 2023-06-22 02:10:32.000000 trainml-0.5.0/trainml/cloudbender/datastores.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3134 2023-06-19 18:42:07.000000 trainml-0.5.0/trainml/cloudbender/device_configs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3608 2023-06-19 18:42:39.000000 trainml-0.5.0/trainml/cloudbender/nodes.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1834 2023-06-19 18:44:21.000000 trainml-0.5.0/trainml/cloudbender/providers.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3339 2023-06-19 18:42:18.000000 trainml-0.5.0/trainml/cloudbender/regions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3323 2023-06-19 18:43:29.000000 trainml-0.5.0/trainml/cloudbender/reservations.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    20029 2023-06-21 20:40:05.000000 trainml-0.5.0/trainml/connections.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7394 2023-06-19 18:43:42.000000 trainml-0.5.0/trainml/datasets.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1507 2023-06-21 20:39:07.000000 trainml-0.5.0/trainml/environments.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3724 2023-01-05 20:17:59.000000 trainml-0.5.0/trainml/exceptions.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     1663 2023-06-21 21:03:28.000000 trainml-0.5.0/trainml/gpu_types.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    17807 2023-06-19 18:48:46.000000 trainml-0.5.0/trainml/jobs.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     7043 2023-06-19 18:44:07.000000 trainml-0.5.0/trainml/models.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)     5209 2023-06-21 21:05:20.000000 trainml-0.5.0/trainml/projects.py
+-rw-r--r--   0 akowalsk   (501) staff       (20)    10982 2023-06-16 13:52:35.000000 trainml-0.5.0/trainml/trainml.py
+drwxr-xr-x   0 akowalsk   (501) staff       (20)        0 2023-06-22 02:51:26.721850 trainml-0.5.0/trainml.egg-info/
+-rw-r--r--   0 akowalsk   (501) staff       (20)     8988 2023-06-22 02:51:26.000000 trainml-0.5.0/trainml.egg-info/PKG-INFO
+-rw-r--r--   0 akowalsk   (501) staff       (20)     3184 2023-06-22 02:51:26.000000 trainml-0.5.0/trainml.egg-info/SOURCES.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)        1 2023-06-22 02:51:26.000000 trainml-0.5.0/trainml.egg-info/dependency_links.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       63 2023-06-22 02:51:26.000000 trainml-0.5.0/trainml.egg-info/entry_points.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       67 2023-06-22 02:51:26.000000 trainml-0.5.0/trainml.egg-info/requires.txt
+-rw-r--r--   0 akowalsk   (501) staff       (20)       23 2023-06-22 02:51:26.000000 trainml-0.5.0/trainml.egg-info/top_level.txt
```

### Comparing `trainml-0.4.9/LICENSE` & `trainml-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/PKG-INFO` & `trainml-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.4.9
+Version: 0.5.0
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.4.9 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.0 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           [https://www.trainml.ai/static/img/trainML-logo-purple.png]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.4.9/README.md` & `trainml-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/examples/create_dataset_and_training_job.py` & `trainml-0.5.0/examples/create_dataset_and_training_job.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/examples/local_storage.py` & `trainml-0.5.0/examples/local_storage.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/examples/training_inference_pipeline.py` & `trainml-0.5.0/examples/training_inference_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,16 +26,15 @@
         gpu_types=["rtx2080ti", "rtx3090"],
         gpu_count=1,
         disk_size=10,
         workers=[
             "python training/image-classification/resnet_cifar.py --epochs 10 --optimizer adam --batch-size 128",
         ],
         data=dict(
-            datasets=[dataset.id],
-            output_type="trainml",
+            datasets=[dataset.id], output_type="trainml", output_uri="model"
         ),
         model=dict(
             source_type="git",
             source_uri="https://github.com/trainML/examples.git",
         ),
     )
 )
@@ -44,15 +43,15 @@
 # Watch the log output, attach will return when the training job stops
 asyncio.run(training_job.attach())
 
 # Get the trained model id from the workers
 training_job = asyncio.run(training_job.refresh())
 
 model = asyncio.run(
-    trainml_client.models.get(training_job.workers[0].get("output_model_uuid"))
+    trainml_client.models.get(training_job.workers[0].get("output_uuid"))
 )
 
 # Ensure the model is ready to use
 asyncio.run(model.wait_for("ready"))
 
 # Use the model in an inference job on new data
 inference_job = asyncio.run(
```

### Comparing `trainml-0.4.9/setup.py` & `trainml-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/integration/conftest.py` & `trainml-0.5.0/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/integration/test_checkpoints_integration.py` & `trainml-0.5.0/tests/integration/test_checkpoints_integration.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
     async def test_checkpoint_properties(self, checkpoint):
         assert isinstance(checkpoint.id, str)
         assert isinstance(checkpoint.status, str)
         assert isinstance(checkpoint.name, str)
         assert isinstance(checkpoint.size, int)
 
-    def test_checkpoint_str(self, checkpoint):
+    async def test_checkpoint_str(self, checkpoint):
         string = str(checkpoint)
         regex = r"^{.*\"checkpoint_uuid\": \"" + checkpoint.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_checkpoint_repr(self, checkpoint):
+    async def test_checkpoint_repr(self, checkpoint):
         string = repr(checkpoint)
         regex = (
             r"^Checkpoint\( trainml , \*\*{.*'checkpoint_uuid': '"
             + checkpoint.id
             + r"'.*}\)$"
         )
         assert isinstance(string, str)
```

### Comparing `trainml-0.4.9/tests/integration/test_datasets_integration.py` & `trainml-0.5.0/tests/integration/test_datasets_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 
     async def test_dataset_properties(self, dataset):
         assert isinstance(dataset.id, str)
         assert isinstance(dataset.status, str)
         assert isinstance(dataset.name, str)
         assert isinstance(dataset.size, int)
 
-    def test_dataset_str(self, dataset):
+    async def test_dataset_str(self, dataset):
         string = str(dataset)
         regex = r"^{.*\"dataset_uuid\": \"" + dataset.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_dataset_repr(self, dataset):
+    async def test_dataset_repr(self, dataset):
         string = repr(dataset)
         regex = (
             r"^Dataset\( trainml , \*\*{.*'dataset_uuid': '"
             + dataset.id
             + r"'.*}\)$"
         )
         assert isinstance(string, str)
```

### Comparing `trainml-0.4.9/tests/integration/test_environments_integration.py` & `trainml-0.5.0/tests/integration/test_environments_integration.py`

 * *Files 13% similar despite different names*

```diff
@@ -31,23 +31,23 @@
     assert isinstance(environment.py_version, str)
     assert isinstance(environment.framework, str)
     assert isinstance(environment.version, str)
     assert isinstance(environment.cuda_version, str)
 
 
 @mark.asyncio
-def test_environment_str(environment):
+async def test_environment_str(environment):
     string = str(environment)
     regex = r"^{.*\"id\": \"" + environment.id + r"\".*}$"
     assert isinstance(string, str)
     assert re.match(regex, string)
 
 
 @mark.asyncio
-def test_environment_repr(environment):
+async def test_environment_repr(environment):
     string = repr(environment)
     regex = (
         r"^Environment\( trainml , \*\*{.*'id': '"
         + environment.id
         + r"'.*}\)$"
     )
     assert isinstance(string, str)
```

### Comparing `trainml-0.4.9/tests/integration/test_gpu_types_integration.py` & `trainml-0.5.0/tests/integration/test_gpu_types_integration.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/integration/test_jobs_integration.py` & `trainml-0.5.0/tests/integration/test_jobs_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 
     async def test_job_properties(self, job):
         assert isinstance(job.id, str)
         assert isinstance(job.name, str)
         assert isinstance(job.status, str)
         assert isinstance(job.type, str)
 
-    def test_job_str(self, job):
+    async def test_job_str(self, job):
         string = str(job)
         regex = r"^{.*\"job_uuid\": \"" + job.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_job_repr(self, job):
+    async def test_job_repr(self, job):
         string = repr(job)
         regex = r"^Job\( trainml , {.*'job_uuid': '" + job.id + r"'.*}\)$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
     async def test_start_job(self, job):
         assert job.status == "stopped"
@@ -371,15 +371,15 @@
         job = await trainml.jobs.create(
             name="CLI Automated Tests - Local Output",
             type="training",
             gpu_types=["gtx1060"],
             disk_size=10,
             workers=["python $TRAINML_MODEL_PATH/tensorflow/main.py"],
             environment=dict(
-                type="DEEPLEARNING_PY39",
+                type="DEEPLEARNING_PY310",
                 env=[
                     dict(
                         key="CHECKPOINT_FILE",
                         value="model.ckpt-0050",
                     )
                 ],
             ),
@@ -421,15 +421,14 @@
         sys.stderr.write(captured.err)
         assert "Epoch 1/2" in captured.out
         assert "Epoch 2/2" in captured.out
         assert "adding: model.ckpt-0001.data-00000-of-00001" in captured.out
         assert "Send complete" in captured.out
 
     async def test_job_model_input_and_output(self, trainml, capsys):
-
         model = await trainml.models.create(
             name="CLI Automated Tests - Job Git Model",
             source_type="git",
             source_uri="git@github.com:trainML/environment-tests.git",
         )
         await model.wait_for("ready", 300)
         assert model.size >= 500000
@@ -446,14 +445,15 @@
                 datasets=[
                     dict(
                         id="CIFAR-10",
                         public=True,
                     )
                 ],
                 output_type="trainml",
+                output_uri="model",
             ),
             model=dict(source_type="trainml", source_uri=model.id),
         )
         await job.attach()
         await job.refresh()
         assert job.status == "finished"
         workers = job.workers
@@ -461,17 +461,15 @@
         await model.remove()
         captured = capsys.readouterr()
         sys.stdout.write(captured.out)
         sys.stderr.write(captured.err)
         assert "Epoch 1/2" in captured.out
         assert "Epoch 2/2" in captured.out
 
-        new_model = await trainml.models.get(
-            workers[0].get("output_model_uuid")
-        )
+        new_model = await trainml.models.get(workers[0].get("output_uuid"))
         assert new_model.id
         await new_model.wait_for("ready")
         await new_model.refresh()
         assert new_model.size > model.size + 1000000
         assert (
             new_model.name
             == "Job - CLI Automated Tests - Training With trainML Model Output"
@@ -549,20 +547,22 @@
                 source_uri="git@github.com:trainML/environment-tests.git",
             ),
             environment=dict(
                 type="CUSTOM",
                 custom_image="tensorflow/tensorflow:2.10.0-gpu",
                 packages=dict(
                     pip=[
-                        "tensorflow_addons",
+                        "tensorflow_addons==0.18.0",
                         "matplotlib",
                         "scipy",
-                        "tensorflow_hub",
+                        "tensorflow_hub==0.12.0",
                         "keras_applications",
                         "keras_preprocessing",
+                        "protobuf==3.20.1",
+                        "typing-extensions==4.4.0",
                     ]
                 ),
             ),
             worker_commands=[
                 "python $TRAINML_MODEL_PATH/tensorflow/main.py",
             ],
             data=dict(
@@ -614,20 +614,15 @@
                 source_type="git",
                 source_uri="git@github.com:trainML/environment-tests.git",
             ),
             worker_commands=[
                 "python $TRAINML_MODEL_PATH/pytorch/main.py",
             ],
             data=dict(
-                datasets=[
-                    dict(
-                        id="CIFAR-10",
-                        public=True,
-                    )
-                ],
+                datasets=[dict(id="MNIST", public=True)],
             ),
         )
         assert job.id
         await job.attach()
         await job.refresh()
         assert job.status == "finished"
         await job.remove()
```

### Comparing `trainml-0.4.9/tests/integration/test_models_integration.py` & `trainml-0.5.0/tests/integration/test_models_integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
     async def test_model_properties(self, model):
         assert isinstance(model.id, str)
         assert isinstance(model.status, str)
         assert isinstance(model.name, str)
         assert isinstance(model.size, int)
 
-    def test_model_str(self, model):
+    async def test_model_str(self, model):
         string = str(model)
         regex = r"^{.*\"model_uuid\": \"" + model.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_model_repr(self, model):
+    async def test_model_repr(self, model):
         string = repr(model)
         regex = (
             r"^Model\( trainml , \*\*{.*'model_uuid': '"
             + model.id
             + r"'.*}\)$"
         )
         assert isinstance(string, str)
@@ -87,8 +87,8 @@
     assert status == "ready"
     assert size >= 1000000
     captured = capsys.readouterr()
     sys.stdout.write(captured.out)
     sys.stderr.write(captured.err)
     assert "Starting data upload from local" in captured.out
     assert "official/LICENSE  11456 bytes" in captured.out
-    assert "Upload complete" in captured.out
+    assert "Upload complete" in captured.out
```

### Comparing `trainml-0.4.9/tests/integration/test_projects_integration.py` & `trainml-0.5.0/tests/integration/test_projects_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,20 +29,20 @@
         assert isinstance(project.id, str)
         assert isinstance(project.name, str)
         assert isinstance(project.owner_name, str)
         assert isinstance(project.is_owner, bool)
         assert project.name == "New Project"
         assert project.is_owner
 
-    def test_project_str(self, project):
+    async def test_project_str(self, project):
         string = str(project)
         regex = r"^{.*\"id\": \"" + project.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_project_repr(self, project):
+    async def test_project_repr(self, project):
         string = repr(project)
         regex = (
             r"^Project\( trainml , \*\*{.*'id': '" + project.id + r"'.*}\)$"
         )
         assert isinstance(string, str)
         assert re.match(regex, string)
```

### Comparing `trainml-0.4.9/tests/integration/test_providers_integration.py` & `trainml-0.5.0/tests/integration/cloudbender/test_providers_integration.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import re
 import sys
 import asyncio
 from pytest import mark, fixture
 
-pytestmark = [mark.sdk, mark.integration, mark.providers]
+pytestmark = [mark.sdk, mark.integration, mark.cloudbender, mark.providers]
 
 
 @mark.create
 @mark.asyncio
 class GetProvidersTests:
     @fixture(scope="class")
     async def provider(self, trainml):
-        provider = await trainml.providers.enable(type="test")
+        provider = await trainml.cloudbender.providers.enable(type="test")
         yield provider
         await provider.remove()
 
     async def test_get_providers(self, trainml):
-        providers = await trainml.providers.list()
+        providers = await trainml.cloudbender.providers.list()
         assert len(providers) > 0
 
     async def test_get_provider(self, trainml, provider):
-        response = await trainml.providers.get(provider.id)
+        response = await trainml.cloudbender.providers.get(provider.id)
         assert response.id == provider.id
 
     async def test_provider_properties(self, provider):
         assert isinstance(provider.id, str)
         assert isinstance(provider.type, str)
         assert provider.type == "test"
         assert provider.credits == 0
 
-    def test_provider_str(self, provider):
+    async def test_provider_str(self, provider):
         string = str(provider)
         regex = r"^{.*\"provider_uuid\": \"" + provider.id + r"\".*}$"
         assert isinstance(string, str)
         assert re.match(regex, string)
 
-    def test_provider_repr(self, provider):
+    async def test_provider_repr(self, provider):
         string = repr(provider)
         regex = (
             r"^Provider\( trainml , \*\*{.*'provider_uuid': '"
             + provider.id
             + r"'.*}\)$"
         )
         assert isinstance(string, str)
```

### Comparing `trainml-0.4.9/tests/unit/cli/test_cli_environment_unit.py` & `trainml-0.5.0/tests/unit/cli/test_cli_environment_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/unit/test_auth.py` & `trainml-0.5.0/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/unit/test_checkpoints_unit.py` & `trainml-0.5.0/tests/unit/test_checkpoints_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @fixture
 def checkpoint(mock_trainml):
     yield specimen.Checkpoint(
         mock_trainml,
         checkpoint_uuid="1",
         project_uuid="proj-id-1",
         name="first one",
-        status="new",
+        status="downloading",
         size=100000,
         createdAt="2020-12-31T23:59:59.000Z",
     )
 
 
 class CheckpointsTests:
     @mark.asyncio
@@ -40,26 +40,30 @@
         self,
         checkpoints,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await checkpoints.get("1234")
-        mock_trainml._query.assert_called_once_with("/checkpoint/1234", "GET")
+        mock_trainml._query.assert_called_once_with(
+            "/checkpoint/1234", "GET", dict()
+        )
 
     @mark.asyncio
     async def test_list_checkpoints(
         self,
         checkpoints,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await checkpoints.list()
-        mock_trainml._query.assert_called_once_with("/checkpoint", "GET")
+        mock_trainml._query.assert_called_once_with(
+            "/checkpoint", "GET", dict()
+        )
 
     @mark.asyncio
     async def test_remove_checkpoint(
         self,
         checkpoints,
         mock_trainml,
     ):
@@ -127,26 +131,24 @@
     def test_checkpoint_bool(self, checkpoint, mock_trainml):
         empty_checkpoint = specimen.Checkpoint(mock_trainml)
         assert bool(checkpoint)
         assert not bool(empty_checkpoint)
 
     @mark.asyncio
     async def test_checkpoint_get_log_url(self, checkpoint, mock_trainml):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/logs/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await checkpoint.get_log_url()
         mock_trainml._query.assert_called_once_with(
             "/checkpoint/1/logs", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_checkpoint_get_details(self, checkpoint, mock_trainml):
-
         api_response = {
             "type": "directory",
             "name": "/",
             "count": "8",
             "size": "177M",
             "contents": [],
         }
@@ -157,15 +159,14 @@
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_checkpoint_get_connection_utility_url(
         self, checkpoint, mock_trainml
     ):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/vpn/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await checkpoint.get_connection_utility_url()
         mock_trainml._query.assert_called_once_with(
             "/checkpoint/1/download", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
@@ -408,15 +409,15 @@
         assert response.status == "ready"
 
     @mark.asyncio
     async def test_checkpoint_wait_for_timeout(self, checkpoint, mock_trainml):
         api_response = dict(
             checkpoint_uuid="1",
             name="first one",
-            status="new",
+            status="downloading",
             createdAt="2020-12-31T23:59:59.000Z",
         )
         mock_trainml._query = AsyncMock(return_value=api_response)
         with raises(TrainMLException):
             await checkpoint.wait_for("ready", 10)
         mock_trainml._query.assert_called()
```

### Comparing `trainml-0.4.9/tests/unit/test_connections_unit.py` & `trainml-0.5.0/tests/unit/test_connections_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/unit/test_datasets_unit.py` & `trainml-0.5.0/tests/unit/test_datasets_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @fixture
 def dataset(mock_trainml):
     yield specimen.Dataset(
         mock_trainml,
         dataset_uuid="1",
         project_uuid="proj-id-1",
         name="first one",
-        status="new",
+        status="downloading",
         size=100000,
         createdAt="2020-12-31T23:59:59.000Z",
     )
 
 
 class DatasetsTests:
     @mark.asyncio
@@ -43,38 +43,41 @@
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await datasets.get("1234")
         mock_trainml._query.assert_called_once_with(
             "/dataset/1234",
             "GET",
+            dict(),
         )
 
     @mark.asyncio
     async def test_list_datasets(
         self,
         datasets,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await datasets.list()
         mock_trainml._query.assert_called_once_with(
             "/dataset",
             "GET",
+            dict(),
         )
 
     @mark.asyncio
     async def test_list_public_datasets(self, datasets, mock_trainml):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await datasets.list_public()
         mock_trainml._query.assert_called_once_with(
             "/dataset/public",
             "GET",
+            dict(),
         )
 
     @mark.asyncio
     async def test_remove_dataset(
         self,
         datasets,
         mock_trainml,
@@ -146,26 +149,24 @@
     def test_dataset_bool(self, dataset, mock_trainml):
         empty_dataset = specimen.Dataset(mock_trainml)
         assert bool(dataset)
         assert not bool(empty_dataset)
 
     @mark.asyncio
     async def test_dataset_get_log_url(self, dataset, mock_trainml):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/logs/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await dataset.get_log_url()
         mock_trainml._query.assert_called_once_with(
             "/dataset/1/logs", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_dataset_get_details(self, dataset, mock_trainml):
-
         api_response = {
             "type": "directory",
             "name": "/",
             "count": "8",
             "size": "177M",
             "contents": [],
         }
@@ -176,15 +177,14 @@
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_dataset_get_connection_utility_url(
         self, dataset, mock_trainml
     ):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/vpn/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await dataset.get_connection_utility_url()
         mock_trainml._query.assert_called_once_with(
             "/dataset/1/download", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
@@ -259,15 +259,14 @@
         mock_trainml._query.assert_called_once_with(
             "/dataset/1",
             "DELETE",
             dict(project_uuid="proj-id-1", force=False),
         )
 
     def test_dataset_default_ws_msg_handler(self, dataset, capsys):
-
         data = {
             "msg": "download: s3://trainml-examples/data/cifar10/data_batch_2.bin to ./data_batch_2.bin\n",
             "time": 1613079345318,
             "type": "subscription",
             "stream": "worker-id-1",
             "job_worker_uuid": "worker-id-1",
         }
```

### Comparing `trainml-0.4.9/tests/unit/test_environments_unit.py` & `trainml-0.5.0/tests/unit/test_environments_unit.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/unit/test_exceptions.py` & `trainml-0.5.0/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/tests/unit/test_gpu_types_unit.py` & `trainml-0.5.0/tests/unit/test_gpu_types_unit.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,14 +35,23 @@
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await gpu_types.list()
         mock_trainml._query.assert_called_once_with(
             f"/project/proj-id-1/gputypes", "GET"
         )
 
+    @mark.asyncio
+    async def test_project_refresh_gpu_types(self, gpu_types, mock_trainml):
+        api_response = dict()
+        mock_trainml._query = AsyncMock(return_value=api_response)
+        await gpu_types.refresh_gpu_types()
+        mock_trainml._query.assert_called_once_with(
+            "/project/proj-id-1/gputypes", "PATCH"
+        )
+
 
 class GpuTypeTests:
     def test_gpu_type_properties(self, gpu_type):
         assert isinstance(gpu_type.id, str)
         assert isinstance(gpu_type.name, str)
         assert isinstance(gpu_type.abbrv, str)
         assert isinstance(gpu_type.credits_per_hour_min, float)
```

### Comparing `trainml-0.4.9/tests/unit/test_jobs_unit.py` & `trainml-0.5.0/tests/unit/test_jobs_unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                         "type": "public",
                         "size": 5068061409,
                     },
                 ],
                 "status": "ready",
             },
             "environment": {
-                "type": "DEEPLEARNING_PY38",
+                "type": "DEEPLEARNING_PY310",
                 "image_size": 44966989795,
                 "env": [
                     {"value": "env1val", "key": "env1"},
                     {"value": "env2val", "key": "env2"},
                 ],
                 "worker_key_types": ["aws", "gcp"],
                 "status": "new",
@@ -146,15 +146,15 @@
                         "type": "public",
                         "size": 5068061409,
                     },
                 ],
                 "status": "ready",
             },
             "environment": {
-                "type": "DEEPLEARNING_PY38",
+                "type": "DEEPLEARNING_PY310",
                 "image_size": 44966989795,
                 "env": [
                     {"value": "env1val", "key": "env1"},
                     {"value": "env2val", "key": "env2"},
                 ],
                 "worker_key_types": ["aws", "gcp"],
                 "status": "ready",
@@ -178,25 +178,25 @@
         self,
         jobs,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await jobs.get("1234")
-        mock_trainml._query.assert_called_once_with("/job/1234", "GET")
+        mock_trainml._query.assert_called_once_with("/job/1234", "GET", dict())
 
     async def test_jobs_list(
         self,
         jobs,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await jobs.list()
-        mock_trainml._query.assert_called_once_with("/job", "GET")
+        mock_trainml._query.assert_called_once_with("/job", "GET", dict())
 
     async def test_jobs_remove(
         self,
         jobs,
         mock_trainml,
     ):
         api_response = dict()
@@ -310,52 +310,62 @@
     def test_job_bool(self, job, mock_trainml):
         empty_job = specimen.Job(mock_trainml)
         assert bool(job)
         assert not bool(empty_job)
 
     @mark.asyncio
     async def test_job_start(self, job, mock_trainml):
-        api_response = None
+        api_response = {
+            "customer_uuid": "cus-id-1",
+            "job_uuid": "job-id-1",
+            "name": "test notebook",
+            "type": "notebook",
+            "status": "starting",
+        }
         mock_trainml._query = AsyncMock(return_value=api_response)
         await job.start()
         mock_trainml._query.assert_called_once_with(
             "/job/job-id-1",
             "PATCH",
             dict(project_uuid="proj-id-1"),
             dict(command="start"),
         )
 
     @mark.asyncio
     async def test_job_stop(self, job, mock_trainml):
-        api_response = None
+        api_response = {
+            "customer_uuid": "cus-id-1",
+            "job_uuid": "job-id-1",
+            "name": "test notebook",
+            "type": "notebook",
+            "status": "stopping",
+        }
         mock_trainml._query = AsyncMock(return_value=api_response)
         await job.stop()
         mock_trainml._query.assert_called_once_with(
             "/job/job-id-1",
             "PATCH",
             dict(project_uuid="proj-id-1"),
             dict(command="stop"),
         )
 
     @mark.asyncio
     async def test_job_get_worker_log_url(self, job, mock_trainml):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/job-id-1/logs/worker-id-1/test_notebook.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await job.get_worker_log_url("worker-id-1")
         mock_trainml._query.assert_called_once_with(
             "/job/job-id-1/worker/worker-id-1/logs",
             "GET",
             dict(project_uuid="proj-id-1"),
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_job_get_connection_utility_url(self, job, mock_trainml):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/job-id-1/vpn/trainml-test_notebook.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await job.get_connection_utility_url()
         mock_trainml._query.assert_called_once_with(
             "/job/job-id-1/download", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
@@ -506,15 +516,14 @@
         mock_trainml._query.assert_called_once_with(
             "/job/job-id-1", "GET", dict(project_uuid="proj-id-1")
         )
         assert job.status == "running"
         assert response.status == "running"
 
     def test_job_default_ws_msg_handler(self, job, capsys):
-
         data = {
             "msg": "Epoch (1/1000)\n",
             "time": 1613079345318,
             "type": "subscription",
             "stream": "worker-id-1",
             "job_worker_uuid": "worker-id-1",
         }
```

### Comparing `trainml-0.4.9/tests/unit/test_models_unit.py` & `trainml-0.5.0/tests/unit/test_models_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 @fixture
 def model(mock_trainml):
     yield specimen.Model(
         mock_trainml,
         model_uuid="1",
         project_uuid="proj-id-1",
         name="first one",
-        status="new",
+        status="downloading",
         size=100000,
         createdAt="2020-12-31T23:59:59.000Z",
     )
 
 
 class ModelsTests:
     @mark.asyncio
@@ -40,26 +40,28 @@
         self,
         models,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await models.get("1234")
-        mock_trainml._query.assert_called_once_with("/model/1234", "GET")
+        mock_trainml._query.assert_called_once_with(
+            "/model/1234", "GET", dict()
+        )
 
     @mark.asyncio
     async def test_list_models(
         self,
         models,
         mock_trainml,
     ):
         api_response = dict()
         mock_trainml._query = AsyncMock(return_value=api_response)
         await models.list()
-        mock_trainml._query.assert_called_once_with("/model", "GET")
+        mock_trainml._query.assert_called_once_with("/model", "GET", dict())
 
     @mark.asyncio
     async def test_remove_model(
         self,
         models,
         mock_trainml,
     ):
@@ -127,26 +129,24 @@
     def test_model_bool(self, model, mock_trainml):
         empty_model = specimen.Model(mock_trainml)
         assert bool(model)
         assert not bool(empty_model)
 
     @mark.asyncio
     async def test_model_get_log_url(self, model, mock_trainml):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/logs/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await model.get_log_url()
         mock_trainml._query.assert_called_once_with(
             "/model/1/logs", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_model_get_details(self, model, mock_trainml):
-
         api_response = {
             "type": "directory",
             "name": "/",
             "count": "8",
             "size": "177M",
             "contents": [],
         }
@@ -155,15 +155,14 @@
         mock_trainml._query.assert_called_once_with(
             "/model/1/details", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
 
     @mark.asyncio
     async def test_model_get_connection_utility_url(self, model, mock_trainml):
-
         api_response = "https://trainml-jobs-dev.s3.us-east-2.amazonaws.com/1/vpn/first_one.zip"
         mock_trainml._query = AsyncMock(return_value=api_response)
         response = await model.get_connection_utility_url()
         mock_trainml._query.assert_called_once_with(
             "/model/1/download", "GET", dict(project_uuid="proj-id-1")
         )
         assert response == api_response
```

### Comparing `trainml-0.4.9/tests/unit/test_providers_unit.py` & `trainml-0.5.0/tests/unit/cloudbender/test_providers_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import re
 import json
 import logging
 from unittest.mock import AsyncMock, patch
 from pytest import mark, fixture, raises
 from aiohttp import WSMessage, WSMsgType
 
-import trainml.providers as specimen
+import trainml.cloudbender.providers as specimen
 from trainml.exceptions import (
     ApiError,
     SpecificationError,
     TrainMLException,
 )
 
-pytestmark = [mark.sdk, mark.unit, mark.providers]
+pytestmark = [mark.sdk, mark.unit, mark.cloudbender, mark.providers]
 
 
 @fixture
 def providers(mock_trainml):
     yield specimen.Providers(mock_trainml)
```

### Comparing `trainml-0.4.9/tests/unit/test_trainml.py` & `trainml-0.5.0/tests/unit/test_trainml.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/trainml/auth.py` & `trainml-0.5.0/trainml/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -289,15 +289,14 @@
     :return {Long integer} Computed U value.
     """
     u_hex_hash = hex_hash(pad_hex(big_a) + pad_hex(big_b))
     return hex_to_long(u_hex_hash)
 
 
 class AWSSRP(object):
-
     NEW_PASSWORD_REQUIRED_CHALLENGE = "NEW_PASSWORD_REQUIRED"
     PASSWORD_VERIFIER_CHALLENGE = "PASSWORD_VERIFIER"
 
     def __init__(
         self,
         username,
         password,
@@ -509,40 +508,43 @@
         else:
             raise NotImplementedError(
                 "The %s challenge is not supported" % response["ChallengeName"]
             )
 
 
 class Auth(object):
-    def __init__(self, **kwargs):
-
+    def __init__(self, domain_suffix="trainml.ai", **kwargs):
         try:
             with open(f"{CONFIG_DIR}/environment.json", "r") as file:
                 env_str = file.read().replace("\n", "")
             env = json.loads(env_str)
         except:
             env = dict()
 
+        auth_defaults = requests.get(
+            "https://app.{}/.well-known/auth-config.json".format(domain_suffix)
+        ).json()
+
         self.region = (
             kwargs.get("region")
             or os.environ.get("TRAINML_REGION")
             or env.get("region")
-            or "us-east-2"
+            or auth_defaults.get("region")
         )
         self.client_id = (
             kwargs.get("client_id")
             or os.environ.get("TRAINML_CLIENT_ID")
             or env.get("client_id")
-            or "32mc1obk9nq97iv015fnmc5eq5"
+            or auth_defaults.get("userPoolSDKClientId")
         )
         self.pool_id = (
             kwargs.get("pool_id")
             or os.environ.get("TRAINML_POOL_ID")
             or env.get("pool_id")
-            or "us-east-2_68kbvTL5p"
+            or auth_defaults.get("userPoolId")
         )
 
         try:
             with open(f"{CONFIG_DIR}/credentials.json", "r") as file:
                 key_str = file.read().replace("\n", "")
             keys = json.loads(key_str)
         except:
```

### Comparing `trainml-0.4.9/trainml/checkpoints.py` & `trainml-0.5.0/trainml/checkpoints.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,50 +13,50 @@
 from .connections import Connection
 
 
 class Checkpoints(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
-    async def get(self, id):
-        resp = await self.trainml._query(f"/checkpoint/{id}", "GET")
+    async def get(self, id, **kwargs):
+        resp = await self.trainml._query(f"/checkpoint/{id}", "GET", kwargs)
         return Checkpoint(self.trainml, **resp)
 
-    async def list(self):
-        resp = await self.trainml._query(f"/checkpoint", "GET")
+    async def list(self, **kwargs):
+        resp = await self.trainml._query(f"/checkpoint", "GET", kwargs)
         checkpoints = [
             Checkpoint(self.trainml, **checkpoint) for checkpoint in resp
         ]
         return checkpoints
 
-    async def list_public(self):
-        resp = await self.trainml._query(f"/checkpoint/public", "GET")
+    async def list_public(self, **kwargs):
+        resp = await self.trainml._query(f"/checkpoint/public", "GET", kwargs)
         datasets = [Checkpoint(self.trainml, **dataset) for dataset in resp]
         return datasets
 
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
             project_uuid=kwargs.get("project_uuid")
             or self.trainml.active_project,
         )
-        payload = {k: v for k, v in data.items() if v}
+        payload = {k: v for k, v in data.items() if v is not None}
         logging.info(f"Creating Checkpoint {name}")
         resp = await self.trainml._query("/checkpoint", "POST", None, payload)
         checkpoint = Checkpoint(self.trainml, **resp)
         logging.info(f"Created Checkpoint {name} with id {checkpoint.id}")
 
         return checkpoint
 
-    async def remove(self, id):
+    async def remove(self, id, **kwargs):
         await self.trainml._query(
-            f"/checkpoint/{id}", "DELETE", dict(force=True)
+            f"/checkpoint/{id}", "DELETE", dict(**kwargs, force=True)
         )
 
 
 class Checkpoint:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._checkpoint = kwargs
@@ -122,27 +122,33 @@
             details = dict(
                 entity_type="checkpoint",
                 project_uuid=self._checkpoint.get("project_uuid"),
                 cidr=self._checkpoint.get("vpn").get("cidr"),
                 ssh_port=self._checkpoint.get("vpn")
                 .get("client")
                 .get("ssh_port"),
-                input_path=self._checkpoint.get("source_uri"),
-                output_path=None,
+                input_path=self._checkpoint.get("source_uri")
+                if self.status in ["new", "downloading"]
+                else None,
+                output_path=self._checkpoint.get("output_uri")
+                if self.status == "exporting"
+                else None,
             )
         else:
             details = dict()
         return details
 
     async def connect(self):
         if self.status in ["ready", "failed"]:
             raise SpecificationError(
                 "status",
-                f"You can only connect to new or downloading checkpoints.",
+                f"You can only connect to downloading or exporting checkpoints.",
             )
+        if self.status == "new":
+            await self.wait_for("downloading")
         connection = Connection(
             self.trainml, entity_type="checkpoint", id=self.id, entity=self
         )
         await connection.start()
         return connection.status
 
     async def disconnect(self):
@@ -155,14 +161,38 @@
     async def remove(self, force=False):
         await self.trainml._query(
             f"/checkpoint/{self._id}",
             "DELETE",
             dict(project_uuid=self._project_uuid, force=force),
         )
 
+    async def rename(self, name):
+        resp = await self.trainml._query(
+            f"/checkpoint/{self._id}",
+            "PATCH",
+            dict(project_uuid=self._project_uuid),
+            dict(name=name),
+        )
+        self.__init__(self.trainml, **resp)
+        return self
+
+    async def export(self, output_type, output_uri, output_options=dict()):
+        resp = await self.trainml._query(
+            f"/checkpoint/{self._id}/export",
+            "POST",
+            dict(project_uuid=self._project_uuid),
+            dict(
+                output_type=output_type,
+                output_uri=output_uri,
+                output_options=output_options,
+            ),
+        )
+        self.__init__(self.trainml, **resp)
+        return self
+
     def _get_msg_handler(self, msg_handler):
         def handler(data):
             if data.get("type") == "subscription":
                 if msg_handler:
                     msg_handler(data)
                 else:
                     timestamp = datetime.fromtimestamp(
```

### Comparing `trainml-0.4.9/trainml/cli/__init__.py` & `trainml-0.5.0/trainml/cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     count=True,
     type=click.INT,
     default=0,
     help="Specify verbosity (repeat to increase).",
 )
 @pass_config
 def cli(config, debug, output_file, silent, verbosity):
-    """TrainML command-line interface."""
+    """trainML command-line interface."""
     config.stdout = output_file
 
     if debug or verbosity > 0:
         if silent:
             click.echo(
                 "Ignoring silent flag when debug or verbosity is set.",
                 file=config.stderr,
@@ -119,16 +119,16 @@
     if verbosity != logging.WARNING:  # default
         click.echo(
             f"Verbosity set to {logging.getLevelName(verbosity)}",
             file=config.stderr,
         )
 
     logging.basicConfig(
-        format="%(asctime)s  %(levelname)s  %(message)s",
-        datefmt="%m/%d/%Y %I:%M:%S %p",
+        format="%(asctime)s.%(msecs)03dZ  %(levelname)s  %(message)s",
+        datefmt="%Y-%m-%dT%H:%M:%S",
         level=verbosity,
         stream=config.stderr,
         force=True,
     )
 
 
 @cli.command()
@@ -164,8 +164,8 @@
 from trainml.cli.dataset import dataset
 from trainml.cli.model import model
 from trainml.cli.checkpoint import checkpoint
 from trainml.cli.environment import environment
 from trainml.cli.gpu import gpu
 from trainml.cli.job import job
 from trainml.cli.project import project
-from trainml.cli.provider import provider
+from trainml.cli.cloudbender import cloudbender
```

### Comparing `trainml-0.4.9/trainml/cli/checkpoint.py` & `trainml-0.5.0/trainml/cli/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         n += 1
     return f"{num:.2f} {s[n]}"
 
 
 @cli.group()
 @pass_config
 def checkpoint(config):
-    """TrainML checkpoint commands."""
+    """trainML checkpoint commands."""
     pass
 
 
 @checkpoint.command()
 @click.argument("checkpoint", type=click.STRING)
 @pass_config
 def attach(config, checkpoint):
@@ -237,7 +237,29 @@
     if None is found:
         if force:
             config.trainml.run(found.client.checkpoints.remove(checkpoint))
         else:
             raise click.UsageError("Cannot find specified checkpoint.")
 
     return config.trainml.run(found.remove(force=force))
+
+
+@checkpoint.command()
+@click.argument("checkpoint", type=click.STRING)
+@click.argument("name", type=click.STRING)
+@pass_config
+def rename(config, checkpoint, name):
+    """
+    Renames a checkpoint.
+
+    CHECKPOINT may be specified by name or ID, but ID is preferred.
+    """
+    try:
+        checkpoint = config.trainml.run(
+            config.trainml.client.checkpoints.get(checkpoint)
+        )
+        if checkpoint is None:
+            raise click.UsageError("Cannot find specified checkpoint.")
+    except:
+        raise click.UsageError("Cannot find specified checkpoint.")
+
+    return config.trainml.run(checkpoint.rename(name=name))
```

### Comparing `trainml-0.4.9/trainml/cli/connection.py` & `trainml-0.5.0/trainml/cli/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 from trainml.cli import cli, pass_config, search_by_id_name
 
 
 @cli.group()
 @pass_config
 def connection(config):
-    """TrainML connection commands."""
+    """trainML connection commands."""
     pass
 
 
 @connection.command()
 @pass_config
 def list(config):
     """List connections."""
@@ -51,11 +51,11 @@
     "--all-projects/--no-all-projects",
     default=False,
     show_default=True,
     help="Auto attach to dataset and show creation logs.",
 )
 @pass_config
 def remove_all(config, all_projects):
-    """Clear and clean-up all TrainML connections."""
+    """Clear and clean-up all trainML connections."""
     return config.trainml.run(
         config.trainml.client.connections.remove_all(all_projects=all_projects)
     )
```

### Comparing `trainml-0.4.9/trainml/cli/dataset.py` & `trainml-0.5.0/trainml/cli/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         n += 1
     return f"{num:.2f} {s[n]}"
 
 
 @cli.group()
 @pass_config
 def dataset(config):
-    """TrainML dataset commands."""
+    """trainML dataset commands."""
     pass
 
 
 @dataset.command()
 @click.argument("dataset", type=click.STRING)
 @pass_config
 def attach(config, dataset):
@@ -235,7 +235,29 @@
     if None is found:
         if force:
             config.trainml.run(config.trainml.client.datasets.remove(dataset))
         else:
             raise click.UsageError("Cannot find specified dataset.")
 
     return config.trainml.run(found.remove(force=force))
+
+
+@dataset.command()
+@click.argument("dataset", type=click.STRING)
+@click.argument("name", type=click.STRING)
+@pass_config
+def rename(config, dataset, name):
+    """
+    Renames a dataset.
+
+    DATASET may be specified by name or ID, but ID is preferred.
+    """
+    try:
+        dataset = config.trainml.run(
+            config.trainml.client.datasets.get(dataset)
+        )
+        if dataset is None:
+            raise click.UsageError("Cannot find specified dataset.")
+    except:
+        raise click.UsageError("Cannot find specified dataset.")
+
+    return config.trainml.run(dataset.rename(name=name))
```

### Comparing `trainml-0.4.9/trainml/cli/environment.py` & `trainml-0.5.0/trainml/cli/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 from trainml.cli import cli, pass_config
 
 
 @cli.group()
 @pass_config
 def environment(config):
-    """TrainML environment commands."""
+    """trainML environment commands."""
     pass
 
 
 @environment.command()
 @pass_config
 def list(config):
     """List environments."""
```

### Comparing `trainml-0.4.9/trainml/cli/gpu.py` & `trainml-0.5.0/trainml/cli/gpu.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import asyncio
 import click
 from trainml.cli import cli, pass_config
-from trainml.trainml import TrainML
 
 
 @cli.group()
 @pass_config
 def gpu(config):
-    """TrainML GPU commands."""
+    """trainML GPU commands."""
     pass
 
 
 @gpu.command()
 @pass_config
 def list(config):
     """List GPUs."""
```

### Comparing `trainml-0.4.9/trainml/cli/job/__init__.py` & `trainml-0.5.0/trainml/cli/job/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from webbrowser import open as browse
 from trainml.cli import cli, pass_config, search_by_id_name
 
 
 @cli.group()
 @pass_config
 def job(config):
-    """TrainML job commands."""
+    """trainML job commands."""
     pass
 
 
 @job.command()
 @click.argument("job", type=click.STRING)
 @pass_config
 def attach(config, job):
@@ -215,15 +215,15 @@
     type=click.Choice(["text", "json"], case_sensitive=False),
     default="text",
     show_default=True,
     help="Choose output format.",
 )
 @pass_config
 def list(config, format):
-    """List TrainML jobs."""
+    """List trainML jobs."""
     jobs = config.trainml.run(config.trainml.client.jobs.list())
 
     if format == "text":
         data = [
             ["ID", "NAME", "STATUS", "TYPE"],
             ["-" * 80, "-" * 80, "-" * 80, "-" * 80],
         ]
@@ -238,8 +238,8 @@
     elif format == "json":
         output = []
         for job in jobs:
             output.append(job.dict)
         click.echo(output, file=config.stdout)
 
 
-from trainml.cli.job.create import create
+from trainml.cli.job.create import create
```

### Comparing `trainml-0.4.9/trainml/cli/job/create.py` & `trainml-0.5.0/trainml/cli/job/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import click
 import json
 from webbrowser import open as browse
 from trainml.cli import pass_config
 from trainml.cli.job import job
 
 
+def validate_cpu_count(ctx, param, value):
+    if value is None:
+        return
+    try:
+        count = int(value)
+    except:
+        raise click.BadParameter("must be integer")
+    if count % 4 != 0:
+        raise click.BadParameter("must be multiple of 4")
+
+    return count
+
+
 @job.group()
 @pass_config
 def create(config):
-    """TrainML job create."""
+    """trainML job create."""
     pass
 
 
 @create.command()
 @click.option(
     "--attach/--no-attach",
     default=True,
@@ -43,34 +56,43 @@
 )
 @click.option(
     "--gpu-type",
     "-gt",
     type=click.Choice(
         [
             "gtx1060",
+            "gtx1080ti",
             "rtx2060s",
             "rtx2070s",
             "rtx2080ti",
             "rtx3090",
             "p100",
             "t4",
             "v100",
             "a100",
+            "a100xl",
             "a6000",
             "a4000",
             "cpu",
         ],
         case_sensitive=False,
     ),
     default=["rtx3090"],
     show_default=True,
     multiple=True,
     help="GPU type.",
 )
 @click.option(
+    "--cpu-count",
+    "-cc",
+    type=click.UNPROCESSED,
+    callback=validate_cpu_count,
+    help="CPU Count (per Worker).",
+)
+@click.option(
     "--max-price",
     "-mp",
     type=click.FLOAT,
     default=10.0,
     show_default=True,
     help="Max Price (per GPU).",
 )
@@ -103,30 +125,27 @@
     help="ID or Name of a public checkpoint to add to the job",
     multiple=True,
 )
 @click.option(
     "--environment",
     type=click.Choice(
         [
-            "DEEPLEARNING_PY38",
             "DEEPLEARNING_PY39",
+            "DEEPLEARNING_PY310",
+            "PYTORCH_PY39_20",
             "PYTORCH_PY39_113",
             "PYTORCH_PY39_112",
-            "PYTORCH_PY38_110",
-            "PYTORCH_PY38_19",
-            "PYTORCH_PY38_18",
+            "TENSORFLOW_PY39_212",
             "TENSORFLOW_PY39_211",
             "TENSORFLOW_PY39_210",
-            "TENSORFLOW_PY38_26",
             "MXNET_PY39_19",
-            "MXNET_PY38_18",
         ],
         case_sensitive=False,
     ),
-    default="DEEPLEARNING_PY39",
+    default="DEEPLEARNING_PY310",
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
@@ -179,23 +198,24 @@
 @click.option(
     "--timeout",
     type=click.INT,
     default=300,
     show_default=True,
     help="Seconds to wait for job to start",
 )
-@click.argument("name", type=click.STRING)
+@click.argument("name", type=click.STRING, required=True)
 @pass_config
 def notebook(
     config,
     attach,
     connect,
     disk_size,
     gpu_count,
     gpu_type,
+    cpu_count,
     max_price,
     data_dir,
     dataset,
     public_dataset,
     checkpoint,
     public_checkpoint,
     environment,
@@ -233,14 +253,18 @@
         max_price=max_price,
         data=dict(datasets=datasets),
         model=dict(checkpoints=checkpoints),
         environment=dict(
             worker_key_types=[k for k in key],
         ),
     )
+
+    if not (len(gpu_type) == 1 and gpu_type[0] == "cpu"):
+        options["gpu_count"] = gpu_count
+
     if custom_image:
         options["environment"]["type"] = "CUSTOM"
         options["environment"]["custom_image"] = custom_image
     else:
         options["environment"]["type"] = environment
 
     try:
@@ -293,15 +317,15 @@
         options["model"]["source_uri"] = model_dir
 
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="notebook",
             gpu_types=gpu_type,
-            gpu_count=gpu_count,
+            cpu_count=cpu_count,
             disk_size=disk_size,
             **options,
         )
     )
     click.echo("Created Job.", file=config.stdout)
     if model_dir:
         config.trainml.run(job.wait_for("waiting for data/model download"))
@@ -353,33 +377,42 @@
 )
 @click.option(
     "--gpu-type",
     "-gt",
     type=click.Choice(
         [
             "gtx1060",
+            "gtx1080ti",
             "rtx2060s",
             "rtx2070s",
             "rtx2080ti",
             "rtx3090",
             "p100",
             "t4",
             "v100",
             "a100",
+            "a100xl",
             "a6000",
             "a4000",
             "cpu",
         ],
         case_sensitive=False,
     ),
     default="rtx3090",
     show_default=True,
     help="GPU type.",
 )
 @click.option(
+    "--cpu-count",
+    "-cc",
+    type=click.UNPROCESSED,
+    callback=validate_cpu_count,
+    help="CPU Count (per Worker).",
+)
+@click.option(
     "--max-price",
     "-mp",
     type=click.FLOAT,
     default=10.0,
     show_default=True,
     help="Max Price (per GPU).",
 )
@@ -433,33 +466,36 @@
 @click.option(
     "--archive/--no-archive",
     default=False,
     show_default=True,
     help="Zip the output contents before uploading.",
 )
 @click.option(
+    "--save-model/--no-save-model",
+    default=False,
+    show_default=True,
+    help="Include the model directory in the job output",
+)
+@click.option(
     "--environment",
     type=click.Choice(
         [
-            "DEEPLEARNING_PY38",
             "DEEPLEARNING_PY39",
+            "DEEPLEARNING_PY310",
+            "PYTORCH_PY39_20",
             "PYTORCH_PY39_113",
             "PYTORCH_PY39_112",
-            "PYTORCH_PY38_110",
-            "PYTORCH_PY38_19",
-            "PYTORCH_PY38_18",
+            "TENSORFLOW_PY39_212",
             "TENSORFLOW_PY39_211",
             "TENSORFLOW_PY39_210",
-            "TENSORFLOW_PY38_26",
             "MXNET_PY39_19",
-            "MXNET_PY38_18",
         ],
         case_sensitive=False,
     ),
-    default="DEEPLEARNING_PY39",
+    default="DEEPLEARNING_PY310",
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
@@ -505,38 +541,36 @@
     help="trainML Model ID to use as the model data",
 )
 @click.option(
     "--model-dir",
     type=click.Path(exists=True, file_okay=False, resolve_path=True),
     help="Local file path to copy as the model data",
 )
-@click.argument("name", type=click.STRING)
-@click.argument(
-    "commands",
-    type=click.STRING,
-    nargs=-1,
-)
+@click.argument("name", type=click.STRING, required=True)
+@click.argument("commands", type=click.STRING, nargs=-1, required=True)
 @pass_config
 def training(
     config,
     attach,
     connect,
     disk_size,
     gpu_count,
     gpu_type,
+    cpu_count,
     max_price,
     data_dir,
     dataset,
     public_dataset,
     checkpoint,
     public_checkpoint,
     output_dir,
     output_type,
     output_uri,
     archive,
+    save_model,
     environment,
     custom_image,
     env,
     key,
     apt_packages,
     pip_packages,
     conda_packages,
@@ -568,31 +602,37 @@
         max_price=max_price,
         data=dict(datasets=datasets),
         model=dict(checkpoints=checkpoints),
         environment=dict(
             worker_key_types=[k for k in key],
         ),
     )
+
+    if not (len(gpu_type) == 1 and gpu_type[0] == "cpu"):
+        options["gpu_count"] = gpu_count
+
     if custom_image:
         options["environment"]["type"] = "CUSTOM"
         options["environment"]["custom_image"] = custom_image
     else:
         options["environment"]["type"] = environment
 
     if output_type:
         options["data"]["output_type"] = output_type
         options["data"]["output_uri"] = output_uri
-        if not archive:
-            options["data"]["output_options"] = dict(archive=False)
+        options["data"]["output_options"] = dict(
+            archive=archive, save_model=save_model
+        )
 
     if output_dir:
         options["data"]["output_type"] = "local"
         options["data"]["output_uri"] = output_dir
-        if not archive:
-            options["data"]["output_options"] = dict(archive=False)
+        options["data"]["output_options"] = dict(
+            archive=archive, save_model=save_model
+        )
 
     try:
         envs = [
             {"key": e.split("=")[0], "value": e.split("=")[1]} for e in env
         ]
         options["environment"]["env"] = envs
     except IndexError:
@@ -640,15 +680,15 @@
         options["model"]["source_uri"] = model_dir
 
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="training",
             gpu_type=gpu_type,
-            gpu_count=gpu_count,
+            cpu_count=cpu_count,
             disk_size=disk_size,
             workers=[command for command in commands],
             **options,
         )
     )
     click.echo("Created Job.", file=config.stdout)
 
@@ -691,33 +731,42 @@
 )
 @click.option(
     "--gpu-type",
     "-gt",
     type=click.Choice(
         [
             "gtx1060",
+            "gtx1080ti",
             "rtx2060s",
             "rtx2070s",
             "rtx2080ti",
             "rtx3090",
             "p100",
             "t4",
             "v100",
             "a100",
+            "a100xl",
             "a6000",
             "a4000",
             "cpu",
         ],
         case_sensitive=False,
     ),
     default="rtx3090",
     show_default=True,
     help="GPU type.",
 )
 @click.option(
+    "--cpu-count",
+    "-cc",
+    type=click.UNPROCESSED,
+    callback=validate_cpu_count,
+    help="CPU Count (per Worker).",
+)
+@click.option(
     "--max-price",
     "-mp",
     type=click.FLOAT,
     default=10.0,
     show_default=True,
     help="Max Price (per GPU).",
 )
@@ -772,33 +821,36 @@
 @click.option(
     "--archive/--no-archive",
     default=False,
     show_default=True,
     help="Zip the output contents before uploading.",
 )
 @click.option(
+    "--save-model/--no-save-model",
+    default=False,
+    show_default=True,
+    help="Include the model directory in the job output",
+)
+@click.option(
     "--environment",
     type=click.Choice(
         [
-            "DEEPLEARNING_PY38",
             "DEEPLEARNING_PY39",
+            "DEEPLEARNING_PY310",
+            "PYTORCH_PY39_20",
             "PYTORCH_PY39_113",
             "PYTORCH_PY39_112",
-            "PYTORCH_PY38_110",
-            "PYTORCH_PY38_19",
-            "PYTORCH_PY38_18",
+            "TENSORFLOW_PY39_212",
             "TENSORFLOW_PY39_211",
             "TENSORFLOW_PY39_210",
-            "TENSORFLOW_PY38_26",
             "MXNET_PY39_19",
-            "MXNET_PY38_18",
         ],
         case_sensitive=False,
     ),
-    default="DEEPLEARNING_PY39",
+    default="DEEPLEARNING_PY310",
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
@@ -844,37 +896,36 @@
     help="trainML Model ID to use as the model data",
 )
 @click.option(
     "--model-dir",
     type=click.Path(exists=True, file_okay=False, resolve_path=True),
     help="Local file path to copy as the model data",
 )
-@click.argument("name", type=click.STRING)
-@click.argument(
-    "command",
-    type=click.STRING,
-)
+@click.argument("name", type=click.STRING, required=True)
+@click.argument("command", type=click.STRING, required=True)
 @pass_config
 def inference(
     config,
     attach,
     connect,
     disk_size,
     gpu_count,
     gpu_type,
+    cpu_count,
     max_price,
     checkpoint,
     public_checkpoint,
     input_dir,
     input_type,
     input_uri,
     output_dir,
     output_type,
     output_uri,
     archive,
+    save_model,
     environment,
     custom_image,
     env,
     key,
     apt_packages,
     pip_packages,
     conda_packages,
@@ -899,14 +950,18 @@
         max_price=max_price,
         data=dict(datasets=[]),
         model=dict(checkpoints=checkpoints),
         environment=dict(
             worker_key_types=[k for k in key],
         ),
     )
+
+    if not (len(gpu_type) == 1 and gpu_type[0] == "cpu"):
+        options["gpu_count"] = gpu_count
+
     if custom_image:
         options["environment"]["type"] = "CUSTOM"
         options["environment"]["custom_image"] = custom_image
     else:
         options["environment"]["type"] = environment
 
     if input_type:
@@ -916,22 +971,24 @@
     if input_dir:
         options["data"]["input_type"] = "local"
         options["data"]["input_uri"] = input_dir
 
     if output_type:
         options["data"]["output_type"] = output_type
         options["data"]["output_uri"] = output_uri
-        if not archive:
-            options["data"]["output_options"] = dict(archive=False)
+        options["data"]["output_options"] = dict(
+            archive=archive, save_model=save_model
+        )
 
     if output_dir:
         options["data"]["output_type"] = "local"
         options["data"]["output_uri"] = output_dir
-        if not archive:
-            options["data"]["output_options"] = dict(archive=False)
+        options["data"]["output_options"] = dict(
+            archive=archive, save_model=save_model
+        )
 
     try:
         envs = [
             {"key": e.split("=")[0], "value": e.split("=")[1]} for e in env
         ]
         options["environment"]["env"] = envs
     except IndexError:
@@ -961,15 +1018,15 @@
         options["model"]["source_uri"] = model_dir
 
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="inference",
             gpu_type=gpu_type,
-            gpu_count=gpu_count,
+            cpu_count=cpu_count,
             disk_size=disk_size,
             workers=[command],
             **options,
         )
     )
     click.echo("Created Job.", file=config.stdout)
 
@@ -1048,33 +1105,42 @@
 )
 @click.option(
     "--gpu-type",
     "-gt",
     type=click.Choice(
         [
             "gtx1060",
+            "gtx1080ti",
             "rtx2060s",
             "rtx2070s",
             "rtx2080ti",
             "rtx3090",
             "p100",
             "t4",
             "v100",
             "a100",
+            "a100xl",
             "a6000",
             "a4000",
             "cpu",
         ],
         case_sensitive=False,
     ),
     default="rtx3090",
     show_default=True,
     help="GPU type.",
 )
 @click.option(
+    "--cpu-count",
+    "-cc",
+    type=click.UNPROCESSED,
+    callback=validate_cpu_count,
+    help="CPU Count (per Worker).",
+)
+@click.option(
     "--max-price",
     "-mp",
     type=click.FLOAT,
     default=10.0,
     show_default=True,
     help="Max Price (per GPU).",
 )
@@ -1090,30 +1156,27 @@
     help="ID or Name of a public checkpoint to add to the job",
     multiple=True,
 )
 @click.option(
     "--environment",
     type=click.Choice(
         [
-            "DEEPLEARNING_PY38",
             "DEEPLEARNING_PY39",
+            "DEEPLEARNING_PY310",
+            "PYTORCH_PY39_20",
             "PYTORCH_PY39_113",
             "PYTORCH_PY39_112",
-            "PYTORCH_PY38_110",
-            "PYTORCH_PY38_19",
-            "PYTORCH_PY38_18",
+            "TENSORFLOW_PY39_212",
             "TENSORFLOW_PY39_211",
             "TENSORFLOW_PY39_210",
-            "TENSORFLOW_PY38_26",
             "MXNET_PY39_19",
-            "MXNET_PY38_18",
         ],
         case_sensitive=False,
     ),
-    default="DEEPLEARNING_PY39",
+    default="DEEPLEARNING_PY310",
     show_default=True,
     help="Job environment to use",
 )
 @click.option(
     "--custom-image",
     type=click.STRING,
     help="Docker Image to use for the job.  Implies 'CUSTOM' environment type.",
@@ -1172,23 +1235,24 @@
 @click.option(
     "--timeout",
     type=click.INT,
     default=300,
     show_default=True,
     help="Seconds to wait for job to start",
 )
-@click.argument("name", type=click.STRING)
+@click.argument("name", type=click.STRING, required=True)
 @pass_config
 def endpoint(
     config,
     attach,
     connect,
     disk_size,
     gpu_count,
     gpu_type,
+    cpu_count,
     max_price,
     checkpoint,
     public_checkpoint,
     environment,
     custom_image,
     env,
     key,
@@ -1217,14 +1281,18 @@
     options = dict(
         max_price=max_price,
         model=dict(checkpoints=checkpoints),
         environment=dict(
             worker_key_types=[k for k in key],
         ),
     )
+
+    if not (len(gpu_type) == 1 and gpu_type[0] == "cpu"):
+        options["gpu_count"] = gpu_count
+
     if custom_image:
         options["environment"]["type"] = "CUSTOM"
         options["environment"]["custom_image"] = custom_image
     else:
         options["environment"]["type"] = environment
 
     try:
@@ -1259,15 +1327,15 @@
         options["model"]["source_uri"] = model_dir
 
     job = config.trainml.run(
         config.trainml.client.jobs.create(
             name=name,
             type="endpoint",
             gpu_type=gpu_type,
-            gpu_count=gpu_count,
+            cpu_count=cpu_count,
             disk_size=disk_size,
             endpoint=dict(routes=routes),
             **options,
         )
     )
     click.echo("Created Job.", file=config.stdout)
```

### Comparing `trainml-0.4.9/trainml/cli/model.py` & `trainml-0.5.0/trainml/cli/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         n += 1
     return f"{num:.2f} {s[n]}"
 
 
 @cli.group()
 @pass_config
 def model(config):
-    """TrainML model commands."""
+    """trainML model commands."""
     pass
 
 
 @model.command()
 @click.argument("model", type=click.STRING)
 @pass_config
 def attach(config, model):
@@ -208,7 +208,27 @@
     if None is found:
         if force:
             config.trainml.run(found.client.models.remove(model))
         else:
             raise click.UsageError("Cannot find specified model.")
 
     return config.trainml.run(found.remove(force=force))
+
+
+@model.command()
+@click.argument("model", type=click.STRING)
+@click.argument("name", type=click.STRING)
+@pass_config
+def rename(config, model, name):
+    """
+    Renames a model.
+
+    MODEL may be specified by name or ID, but ID is preferred.
+    """
+    try:
+        model = config.trainml.run(config.trainml.client.models.get(model))
+        if model is None:
+            raise click.UsageError("Cannot find specified model.")
+    except:
+        raise click.UsageError("Cannot find specified model.")
+
+    return config.trainml.run(model.rename(name=name))
```

### Comparing `trainml-0.4.9/trainml/cli/project.py` & `trainml-0.5.0/trainml/cli/project.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import click
 from trainml.cli import cli, pass_config, search_by_id_name
 
 
 @cli.group()
 @pass_config
 def project(config):
-    """TrainML project commands."""
+    """trainML project commands."""
     pass
 
 
 @project.command()
 @pass_config
 def list(config):
     """List projects."""
@@ -71,7 +71,84 @@
     projects = config.trainml.run(config.trainml.client.projects.list())
 
     found = search_by_id_name(project, projects)
     if None is found:
         raise click.UsageError("Cannot find specified project.")
 
     return config.trainml.run(found.remove())
+
+
+@project.command()
+@pass_config
+def list_datastores(config):
+    """List project datastores."""
+    data = [
+        ["ID", "NAME", "TYPE", "REGION_UUID"],
+        [
+            "-" * 80,
+            "-" * 80,
+            "-" * 80,
+            "-" * 80,
+        ],
+    ]
+    project = config.trainml.run(
+        config.trainml.client.projects.get(config.trainml.client.project)
+    )
+
+    datastores = config.trainml.run(project.list_datastores())
+
+    for datastore in datastores:
+        data.append(
+            [
+                datastore.id,
+                datastore.name,
+                datastore.type,
+                datastore.region_uuid,
+            ]
+        )
+
+    for row in data:
+        click.echo(
+            "{: >38.36} {: >30.28} {: >15.13} {: >38.36}" "".format(*row),
+            file=config.stdout,
+        )
+
+
+@project.command()
+@pass_config
+def list_reservations(config):
+    """List project reservations."""
+    data = [
+        ["ID", "NAME", "TYPE", "RESOURCE", "HOSTNAME", "REGION_UUID"],
+        [
+            "-" * 80,
+            "-" * 80,
+            "-" * 80,
+            "-" * 80,
+            "-" * 80,
+            "-" * 80,
+        ],
+    ]
+    project = config.trainml.run(
+        config.trainml.client.projects.get(config.trainml.client.project)
+    )
+
+    reservations = config.trainml.run(project.list_reservations())
+
+    for reservation in reservations:
+        data.append(
+            [
+                reservation.id,
+                reservation.name,
+                reservation.type,
+                reservation.resource,
+                reservation.hostname,
+                reservation.region_uuid,
+            ]
+        )
+
+    for row in data:
+        click.echo(
+            "{: >38.36} {: >30.28} {: >8.6} {: >15.13} {: >30.28} {: >38.36}"
+            "".format(*row),
+            file=config.stdout,
+        )
```

### Comparing `trainml-0.4.9/trainml/connections.py` & `trainml-0.5.0/trainml/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import shutil
 import asyncio
 import aiohttp
 import aiodocker
 import zipfile
 import re
 import logging
-from datetime import datetime
 
 from .exceptions import (
     ConnectionError,
     ApiError,
     SpecificationError,
     TrainMLException,
 )
```

### Comparing `trainml-0.4.9/trainml/datasets.py` & `trainml-0.5.0/trainml/datasets.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,47 +13,49 @@
 from .connections import Connection
 
 
 class Datasets(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
-    async def get(self, id):
-        resp = await self.trainml._query(f"/dataset/{id}", "GET")
+    async def get(self, id, **kwargs):
+        resp = await self.trainml._query(f"/dataset/{id}", "GET", kwargs)
         return Dataset(self.trainml, **resp)
 
-    async def list(self):
-        resp = await self.trainml._query(f"/dataset", "GET")
+    async def list(self, **kwargs):
+        resp = await self.trainml._query(f"/dataset", "GET", kwargs)
         datasets = [Dataset(self.trainml, **dataset) for dataset in resp]
         return datasets
 
-    async def list_public(self):
-        resp = await self.trainml._query(f"/dataset/public", "GET")
+    async def list_public(self, **kwargs):
+        resp = await self.trainml._query(f"/dataset/public", "GET", kwargs)
         datasets = [Dataset(self.trainml, **dataset) for dataset in resp]
         return datasets
 
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
             project_uuid=kwargs.get("project_uuid")
             or self.trainml.active_project,
         )
-        payload = {k: v for k, v in data.items() if v}
+        payload = {k: v for k, v in data.items() if v is not None}
         logging.info(f"Creating Dataset {name}")
         resp = await self.trainml._query("/dataset", "POST", None, payload)
         dataset = Dataset(self.trainml, **resp)
         logging.info(f"Created Dataset {name} with id {dataset.id}")
 
         return dataset
 
-    async def remove(self, id):
-        await self.trainml._query(f"/dataset/{id}", "DELETE", dict(force=True))
+    async def remove(self, id, **kwargs):
+        await self.trainml._query(
+            f"/dataset/{id}", "DELETE", dict(**kwargs, force=True)
+        )
 
 
 class Dataset:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._dataset = kwargs
         self._id = self._dataset.get("id", self._dataset.get("dataset_uuid"))
@@ -129,14 +131,16 @@
 
     async def connect(self):
         if self.status in ["ready", "failed"]:
             raise SpecificationError(
                 "status",
                 f"You can only connect to new or downloading datasets.",
             )
+        if self.status == "new":
+            await self.wait_for("downloading")
         connection = Connection(
             self.trainml, entity_type="dataset", id=self.id, entity=self
         )
         await connection.start()
         return connection.status
 
     async def disconnect(self):
@@ -149,14 +153,24 @@
     async def remove(self, force=False):
         await self.trainml._query(
             f"/dataset/{self._id}",
             "DELETE",
             dict(project_uuid=self._project_uuid, force=force),
         )
 
+    async def rename(self, name):
+        resp = await self.trainml._query(
+            f"/dataset/{self._id}",
+            "PATCH",
+            None,
+            dict(name=name),
+        )
+        self.__init__(self.trainml, **resp)
+        return self
+
     def _get_msg_handler(self, msg_handler):
         def handler(data):
             if data.get("type") == "subscription":
                 if msg_handler:
                     msg_handler(data)
                 else:
                     timestamp = datetime.fromtimestamp(
```

### Comparing `trainml-0.4.9/trainml/environments.py` & `trainml-0.5.0/trainml/environments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-from datetime import datetime
 
 
 class Environments(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
     async def list(self):
```

### Comparing `trainml-0.4.9/trainml/exceptions.py` & `trainml-0.5.0/trainml/exceptions.py`

 * *Files identical despite different names*

### Comparing `trainml-0.4.9/trainml/gpu_types.py` & `trainml-0.5.0/trainml/gpu_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 import json
-from datetime import datetime
 
 
 class GpuTypes(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
     async def list(self):
-        if self.trainml.active_project:
-            project_id = self.trainml.active_project
-        else:
-            projects = await self.trainml.projects.list()
-            project_id = next(
-                (p.id for p in projects if p.name == "Personal"),
-                None,
-            )
         resp = await self.trainml._query(
-            f"/project/{project_id}/gputypes", "GET"
+            f"/project/{self.trainml.project}/gputypes", "GET"
         )
         gpu_types = [GpuType(self.trainml, **gpu_type) for gpu_type in resp]
         return gpu_types
 
+    async def refresh_gpu_types(self):
+        await self.trainml._query(
+            f"/project/{self.trainml.project}/gputypes", "PATCH"
+        )
+
 
 class GpuType:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._gpu_type = kwargs
         self._id = self._gpu_type.get("id", self._gpu_type.get("gpu_type_id"))
         self._name = self._gpu_type.get("name")
```

### Comparing `trainml-0.4.9/trainml/jobs.py` & `trainml-0.5.0/trainml/jobs.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 from trainml.connections import Connection
 
 
 class Jobs(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
-    async def get(self, id):
-        resp = await self.trainml._query(f"/job/{id}", "GET")
+    async def get(self, id, **kwargs):
+        resp = await self.trainml._query(f"/job/{id}", "GET", kwargs)
         return Job(self.trainml, **resp)
 
-    async def list(self):
-        resp = await self.trainml._query(f"/job", "GET")
+    async def list(self, **kwargs):
+        resp = await self.trainml._query(f"/job", "GET", kwargs)
         jobs = [Job(self.trainml, **job) for job in resp]
         return jobs
 
     async def create(
         self,
         name,
         type,
@@ -41,15 +41,14 @@
         worker_commands=[],
         environment=dict(),
         data=dict(),
         model=dict(),
         endpoint=dict(),
         **kwargs,
     ):
-
         resources = {
             k: v
             for k, v in dict(
                 gpu_count=gpu_count,
                 disk_size=disk_size,
                 max_price=max_price,
                 cpu_count=cpu_count,
@@ -99,16 +98,18 @@
 
     async def create_json(self, payload):
         logging.debug(f"Job payload: {payload}")
         resp = await self.trainml._query("/job", "POST", None, payload)
         job = Job(self.trainml, **resp)
         return job
 
-    async def remove(self, id):
-        await self.trainml._query(f"/job/{id}", "DELETE", dict(force=True))
+    async def remove(self, id, **kwargs):
+        await self.trainml._query(
+            f"/job/{id}", "DELETE", dict(**kwargs, force=True)
+        )
 
 
 class Job:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._job = kwargs
         self._id = self._job.get("id", self._job.get("job_uuid"))
@@ -172,14 +173,15 @@
             "type",
             "resources",
             "model",
             "data",
             "environment",
             "endpoint",
             "workers",
+            "project_uuid",
         ]
         resources_keys = [
             "gpu_count",
             "gpu_types",
             "disk_size",
             "max_price",
             "preemptible",
@@ -247,41 +249,47 @@
                         workers.append(worker.get("command"))
                     create_json["workers"] = workers
                 else:
                     create_json[k] = v
         return create_json
 
     async def start(self):
-        await self.trainml._query(
+        resp = await self.trainml._query(
             f"/job/{self._id}",
             "PATCH",
             dict(project_uuid=self._project_uuid),
             dict(command="start"),
         )
+        self.__init__(self.trainml, **resp)
+        return self
 
     async def stop(self):
-        await self.trainml._query(
+        resp = await self.trainml._query(
             f"/job/{self._id}",
             "PATCH",
             dict(project_uuid=self._project_uuid),
             dict(command="stop"),
         )
+        self.__init__(self.trainml, **resp)
+        return self
 
     async def update(self, data):
         if self.type != "notebook":
             raise SpecificationError(
                 "type",
                 "Only notebook jobs can be modified.",
             )
-        await self.trainml._query(
+        resp = await self.trainml._query(
             f"/job/{self._id}",
             "PATCH",
             dict(project_uuid=self._project_uuid),
             data,
         )
+        self.__init__(self.trainml, **resp)
+        return self
 
     async def get_worker_log_url(self, job_worker_uuid):
         resp = await self.trainml._query(
             f"/job/{self._id}/worker/{job_worker_uuid}/logs",
             "GET",
             dict(project_uuid=self._project_uuid),
         )
@@ -324,14 +332,15 @@
         webbrowser.open(self.notebook_url)
 
     async def connect(self):
         if self.type == "notebook" and self.status not in [
             "new",
             "waiting for data/model download",
             "waiting for GPUs",
+            "waiting for resources",
         ]:
             raise SpecificationError(
                 "type",
                 "Notebooks cannot be connected to after model download is complete.  Use open() instead.",
             )
         if self.type == "endpoint" and self.status not in [
             "new",
@@ -346,21 +355,29 @@
             "removed",
             "removing",
         ]:
             raise SpecificationError(
                 "status",
                 f"You can only connect to active jobs.",
             )
+        if self._job.get("vpn").get("status") == "n/a":
+            logging.info("Local connection not enabled for this job.")
+            return
+        if self.status == "new":
+            await self.wait_for("waiting for data/model download")
         connection = Connection(
             self.trainml, entity_type="job", id=self.id, entity=self
         )
         await connection.start()
         return connection.status
 
     async def disconnect(self):
+        if self._job.get("vpn").get("status") == "n/a":
+            logging.info("Local connection not enabled for this job.")
+            return
         connection = Connection(
             self.trainml, entity_type="job", id=self.id, entity=self
         )
         await connection.stop()
         return connection.status
 
     async def remove(self, force=False):
@@ -453,24 +470,30 @@
         logging.debug(f"copy result: {job}")
         return job
 
     async def wait_for(self, status, timeout=300):
         valid_statuses = [
             "waiting for data/model download",
             "waiting for GPUs",
+            "waiting for resources",
             "running",
             "stopped",
             "finished",
             "archived",
         ]
         if not status in valid_statuses:
             raise SpecificationError(
                 "status",
                 f"Invalid wait_for status {status}.  Valid statuses are: {valid_statuses}",
             )
+        if status == "waiting for GPUs":
+            warnings.warn(
+                "'waiting for GPUs' status is deprecated, use 'waiting for resources' instead.",
+                DeprecationWarning,
+            )
         if (self.type == "training") and status == "stopped":
             warnings.warn(
                 "'stopped' status is deprecated for training jobs, use 'finished' instead.",
                 DeprecationWarning,
             )
         if self.status == status or (
             self.type == "training"
@@ -499,15 +522,18 @@
                 or (
                     self.type == "training"
                     and status == "finished"
                     and self.status == "stopped"
                 )
                 or (
                     status
-                    == "waiting for GPUs"  ## this status could be very short and the polling could miss it
+                    in [
+                        "waiting for GPUs",
+                        "waiting for resources",
+                    ]  ## this status could be very short and the polling could miss it
                     and self.status in ["starting", "provisioning", "running"]
                 )
                 or (
                     status
                     == "waiting for data/model download"  ## this status could be very short and the polling could miss it
                     and self.status in ["starting", "provisioning", "running"]
                 )
```

### Comparing `trainml-0.4.9/trainml/models.py` & `trainml-0.5.0/trainml/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,42 +13,44 @@
 from .connections import Connection
 
 
 class Models(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
-    async def get(self, id):
-        resp = await self.trainml._query(f"/model/{id}", "GET")
+    async def get(self, id, **kwargs):
+        resp = await self.trainml._query(f"/model/{id}", "GET", kwargs)
         return Model(self.trainml, **resp)
 
-    async def list(self):
-        resp = await self.trainml._query(f"/model", "GET")
+    async def list(self, **kwargs):
+        resp = await self.trainml._query(f"/model", "GET", kwargs)
         models = [Model(self.trainml, **model) for model in resp]
         return models
 
     async def create(self, name, source_type, source_uri, **kwargs):
         data = dict(
             name=name,
             source_type=source_type,
             source_uri=source_uri,
             source_options=kwargs.get("source_options"),
             project_uuid=kwargs.get("project_uuid")
             or self.trainml.active_project,
         )
-        payload = {k: v for k, v in data.items() if v}
+        payload = {k: v for k, v in data.items() if v is not None}
         logging.info(f"Creating Model {name}")
         resp = await self.trainml._query("/model", "POST", None, payload)
         model = Model(self.trainml, **resp)
         logging.info(f"Created Model {name} with id {model.id}")
 
         return model
 
-    async def remove(self, id):
-        await self.trainml._query(f"/model/{id}", "DELETE", dict(force=True))
+    async def remove(self, id, **kwargs):
+        await self.trainml._query(
+            f"/model/{id}", "DELETE", dict(**kwargs, force=True)
+        )
 
 
 class Model:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
         self._model = kwargs
         self._id = self._model.get("id", self._model.get("model_uuid"))
@@ -122,14 +124,16 @@
 
     async def connect(self):
         if self.status in ["ready", "failed"]:
             raise SpecificationError(
                 "status",
                 f"You can only connect to new or downloading models.",
             )
+        if self.status == "new":
+            await self.wait_for("downloading")
         connection = Connection(
             self.trainml, entity_type="model", id=self.id, entity=self
         )
         await connection.start()
         return connection.status
 
     async def disconnect(self):
@@ -142,14 +146,24 @@
     async def remove(self, force=False):
         await self.trainml._query(
             f"/model/{self._id}",
             "DELETE",
             dict(project_uuid=self._project_uuid, force=force),
         )
 
+    async def rename(self, name):
+        resp = await self.trainml._query(
+            f"/model/{self._id}",
+            "PATCH",
+            None,
+            dict(name=name),
+        )
+        self.__init__(self.trainml, **resp)
+        return self
+
     def _get_msg_handler(self, msg_handler):
         def handler(data):
             if data.get("type") == "subscription":
                 if msg_handler:
                     msg_handler(data)
                 else:
                     timestamp = datetime.fromtimestamp(
```

### Comparing `trainml-0.4.9/trainml/projects.py` & `trainml-0.5.0/trainml/cloudbender/providers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,63 @@
 import json
 import logging
 from datetime import datetime
 
 
-class Projects(object):
+class Providers(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
     async def get(self, id):
-        resp = await self.trainml._query(f"/project/{id}", "GET")
-        return Project(self.trainml, **resp)
+        resp = await self.trainml._query(f"/provider/{id}", "GET")
+        return Provider(self.trainml, **resp)
 
     async def list(self):
-        resp = await self.trainml._query(f"/project", "GET")
-        projects = [Project(self.trainml, **project) for project in resp]
-        return projects
-
-    async def create(self, name, copy_keys=False, **kwargs):
-        data = dict(
-            name=name,
-            copy_keys=copy_keys,
-        )
-        payload = {k: v for k, v in data.items() if v or k in ["copy_keys"]}
-        logging.info(f"Creating Project {name}")
-        resp = await self.trainml._query("/project", "POST", None, payload)
-        project = Project(self.trainml, **resp)
-        logging.info(f"Created Project {name} with id {project.id}")
+        resp = await self.trainml._query(f"/provider", "GET")
+        providers = [Provider(self.trainml, **provider) for provider in resp]
+        return providers
+
+    async def enable(self, type, **kwargs):
+        data = dict(type=type, **kwargs)
+        payload = {k: v for k, v in data.items() if v is not None}
+        logging.info(f"Enabling Provider {type}")
+        resp = await self.trainml._query("/provider", "POST", None, payload)
+        provider = Provider(self.trainml, **resp)
+        logging.info(f"Enabled Provider {type} with id {provider.id}")
 
-        return project
+        return provider
 
     async def remove(self, id):
-        await self.trainml._query(f"/project/{id}", "DELETE")
+        await self.trainml._query(f"/provider/{id}", "DELETE")
 
 
-class Project:
+class Provider:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
-        self._project = kwargs
-        self._id = self._project.get("id")
-        self._name = self._project.get("name")
-        self._is_owner = self._project.get("owner")
-        self._owner_name = self._project.get("owner_name")
+        self._provider = kwargs
+        self._id = self._provider.get("provider_uuid")
+        self._type = self._provider.get("type")
+        self._credits = self._provider.get("credits")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
-    def name(self) -> str:
-        return self._name
+    def type(self) -> str:
+        return self._type
 
     @property
-    def is_owner(self) -> bool:
-        return self._is_owner
-
-    @property
-    def owner_name(self) -> str:
-        return self._owner_name
+    def credits(self) -> float:
+        return self._credits
 
     def __str__(self):
-        return json.dumps({k: v for k, v in self._project.items()})
+        return json.dumps({k: v for k, v in self._provider.items()})
 
     def __repr__(self):
-        return f"Project( trainml , **{self._project.__repr__()})"
+        return f"Provider( trainml , **{self._provider.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
     async def remove(self):
-        await self.trainml._query(f"/project/{self._id}", "DELETE")
+        await self.trainml._query(f"/provider/{self._id}", "DELETE")
```

### Comparing `trainml-0.4.9/trainml/providers.py` & `trainml-0.5.0/trainml/cloudbender/regions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,105 @@
 import json
 import logging
-from datetime import datetime
 
 
-class Providers(object):
+class Regions(object):
     def __init__(self, trainml):
         self.trainml = trainml
 
-    async def get(self, id):
-        resp = await self.trainml._query(f"/provider/{id}", "GET")
-        return Provider(self.trainml, **resp)
-
-    async def list(self):
-        resp = await self.trainml._query(f"/provider", "GET")
-        providers = [Provider(self.trainml, **provider) for provider in resp]
-        return providers
-
-    async def enable(self, type, **kwargs):
-        data = dict(type=type, **kwargs)
-        payload = {k: v for k, v in data.items() if v or k in ["copy_keys"]}
-        logging.info(f"Enabling Provider {type}")
-        resp = await self.trainml._query("/provider", "POST", None, payload)
-        provider = Provider(self.trainml, **resp)
-        logging.info(f"Enabled Provider {type} with id {provider.id}")
+    async def get(self, provider_uuid, id, **kwargs):
+        resp = await self.trainml._query(
+            f"/provider/{provider_uuid}/region/{id}", "GET", kwargs
+        )
+        return Region(self.trainml, **resp)
+
+    async def list(self, provider_uuid, **kwargs):
+        resp = await self.trainml._query(
+            f"/provider/{provider_uuid}/region", "GET", kwargs
+        )
+        regions = [Region(self.trainml, **region) for region in resp]
+        return regions
+
+    async def create(self, provider_uuid, name, public, storage, **kwargs):
+        logging.info(f"Creating Region {name}")
+        data = dict(name=name, public=public, storage=storage, **kwargs)
+        payload = payload = {k: v for k, v in data.items() if v is not None}
+        resp = await self.trainml._query(
+            f"/provider/{provider_uuid}/region", "POST", None, payload
+        )
+        region = Region(self.trainml, **resp)
+        logging.info(f"Created Region {name} with id {region.id}")
+        return region
+
+    async def remove(self, provider_uuid, id, **kwargs):
+        await self.trainml._query(
+            f"/provider/{provider_uuid}/region/{id}", "DELETE", kwargs
+        )
 
-        return provider
 
-    async def remove(self, id):
-        await self.trainml._query(f"/provider/{id}", "DELETE")
-
-
-class Provider:
+class Region:
     def __init__(self, trainml, **kwargs):
         self.trainml = trainml
-        self._provider = kwargs
-        self._id = self._provider.get("provider_uuid")
-        self._type = self._provider.get("type")
-        self._credits = self._provider.get("credits")
+        self._region = kwargs
+        self._id = self._region.get("region_uuid")
+        self._provider_uuid = self._region.get("provider_uuid")
+        self._type = self._region.get("provider_type")
+        self._name = self._region.get("name")
+        self._status = self._region.get("status")
 
     @property
     def id(self) -> str:
         return self._id
 
     @property
+    def provider_uuid(self) -> str:
+        return self._provider_uuid
+
+    @property
     def type(self) -> str:
         return self._type
 
     @property
-    def credits(self) -> float:
-        return self._credits
+    def name(self) -> str:
+        return self._name
+
+    @property
+    def status(self) -> str:
+        return self._status
 
     def __str__(self):
-        return json.dumps({k: v for k, v in self._provider.items()})
+        return json.dumps({k: v for k, v in self._region.items()})
 
     def __repr__(self):
-        return f"Provider( trainml , **{self._provider.__repr__()})"
+        return f"Region( trainml , **{self._region.__repr__()})"
 
     def __bool__(self):
         return bool(self._id)
 
     async def remove(self):
-        await self.trainml._query(f"/provider/{self._id}", "DELETE")
+        await self.trainml._query(
+            f"/provider/{self._provider_uuid}/region/{self._id}", "DELETE"
+        )
+
+    async def add_dataset(self, project_uuid, dataset_uuid, **kwargs):
+        await self.trainml._query(
+            f"/provider/{self._provider_uuid}/region/{self._id}/dataset",
+            "POST",
+            None,
+            dict(project_uuid=project_uuid, dataset_uuid=dataset_uuid),
+        )
+
+    async def add_model(self, project_uuid, model_uuid, **kwargs):
+        await self.trainml._query(
+            f"/provider/{self._provider_uuid}/region/{self._id}/model",
+            "POST",
+            None,
+            dict(project_uuid=project_uuid, model_uuid=model_uuid),
+        )
+
+    async def add_checkpoint(self, project_uuid, checkpoint_uuid, **kwargs):
+        await self.trainml._query(
+            f"/provider/{self._provider_uuid}/region/{self._id}/checkpoint",
+            "POST",
+            None,
+            dict(project_uuid=project_uuid, checkpoint_uuid=checkpoint_uuid),
+        )
```

### Comparing `trainml-0.4.9/trainml/trainml.py` & `trainml-0.5.0/trainml/trainml.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from trainml.checkpoints import Checkpoints
 from trainml.jobs import Jobs
 from trainml.gpu_types import GpuTypes
 from trainml.environments import Environments
 from trainml.exceptions import ApiError, TrainMLException
 from trainml.connections import Connections
 from trainml.projects import Projects
-from trainml.providers import Providers
+from trainml.cloudbender import Cloudbender
 
 
 async def delayed_close(ws):
     await asyncio.sleep(15)
     if not ws.closed:
         await ws.close()
 
@@ -46,14 +46,15 @@
         self.domain_suffix = (
             kwargs.get("domain_suffix")
             or os.environ.get("TRAINML_DOMAIN_SUFFIX")
             or env.get("domain_suffix")
             or "trainml.ai"
         )
         self.auth = Auth(
+            domain_suffix=self.domain_suffix,
             user=kwargs.get("user"),
             key=kwargs.get("key"),
             region=kwargs.get("region"),
             client_id=kwargs.get("client_id"),
             pool_id=kwargs.get("pool_id"),
         )
         self.active_project = (
@@ -65,26 +66,26 @@
         self.models = Models(self)
         self.checkpoints = Checkpoints(self)
         self.jobs = Jobs(self)
         self.gpu_types = GpuTypes(self)
         self.environments = Environments(self)
         self.connections = Connections(self)
         self.projects = Projects(self)
-        self.providers = Providers(self)
+        self.cloudbender = Cloudbender(self)
         self.api_url = (
             kwargs.get("api_url")
             or os.environ.get("TRAINML_API_URL")
             or env.get("api_url")
-            or "api.trainml.ai"
+            or f"api.{self.domain_suffix}"
         )
         self.ws_url = (
             kwargs.get("ws_url")
             or os.environ.get("TRAINML_WS_URL")
             or env.get("ws_url")
-            or "api-ws.trainml.ai"
+            or f"api-ws.{self.domain_suffix}"
         )
 
     @property
     def project(self) -> str:
         return self.active_project
 
     async def _query(self, path, method, params=None, data=None, headers=None):
@@ -92,14 +93,17 @@
             tokens = self.auth.get_tokens()
         except TrainMLException as e:
             raise e
         except Exception:
             raise TrainMLException(
                 f"Error getting authorization tokens.  Verify configured credentials. Error: {traceback.format_exc()}"
             )
+        logging.debug(
+            f"Call parameters - Path: {path}, Method: {method}, Params: {params}, Body: {data}, Headers: {headers}"
+        )
         headers = (
             {
                 **headers,
                 **{
                     "Authorization": tokens.get("id_token"),
                     "User-Agent": f"trainML-sdk/{self._version}",
                 },
@@ -129,14 +133,18 @@
                 if params
                 else {"project_uuid": self.active_project}
             )
 
         if "Content-Type" not in headers:
             headers["Content-Type"] = "application/json"
         url = f"https://{self.api_url}{path}"
+
+        logging.debug(
+            f"Request - Url: {url}, Method: {method}, Params: {params}, Body: {data}, Headers: {headers}"
+        )
         async with aiohttp.ClientSession() as session:
             async with session.request(
                 method,
                 url,
                 data=json.dumps(data),
                 headers=headers,
                 params=params,
@@ -245,15 +253,14 @@
                         )
                         async for msg in ws:
                             if msg.type in (
                                 aiohttp.WSMsgType.CLOSED,
                                 aiohttp.WSMsgType.ERROR,
                                 aiohttp.WSMsgType.CLOSE,
                             ):
-
                                 logging.debug(
                                     f"Websocket Received Closed Message.  Done? {done}"
                                 )
                                 await ws.close()
                                 break
                             data = json.loads(msg.data)
                             if data.get("type") == "end":
```

### Comparing `trainml-0.4.9/trainml.egg-info/PKG-INFO` & `trainml-0.5.0/trainml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trainml
-Version: 0.4.9
+Version: 0.5.0
 Summary: trainML client SDK and command line utilities
 Home-page: https://github.com/trainML/trainml-cli
 Author: trainML
 Author-email: support@trainml.ai
 License: MIT
 Description: <div align="center">
           <a href="https://www.trainml.ai/"><img src="https://www.trainml.ai/static/img/trainML-logo-purple.png"></a><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: trainml Version: 0.4.9 Summary: trainML client SDK
+Metadata-Version: 2.1 Name: trainml Version: 0.5.0 Summary: trainML client SDK
 and command line utilities Home-page: https://github.com/trainML/trainml-cli
 Author: trainML Author-email: support@trainml.ai License: MIT Description:
           [https://www.trainml.ai/static/img/trainML-logo-purple.png]
 # trainML Python SDK and Command Line Tools Provides programmatic access to
 [trainML platform](https://app.trainml.ai). ## Installation Python 3.8 or above
 is required. ``` pip install trainml ``` ## Authentication ### Prerequisites
 You must have a valid [trainML account](https://app.trainml.ai). On the
```

### Comparing `trainml-0.4.9/trainml.egg-info/SOURCES.txt` & `trainml-0.5.0/trainml.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -11,45 +11,63 @@
 tests/integration/test_checkpoints_integration.py
 tests/integration/test_datasets_integration.py
 tests/integration/test_environments_integration.py
 tests/integration/test_gpu_types_integration.py
 tests/integration/test_jobs_integration.py
 tests/integration/test_models_integration.py
 tests/integration/test_projects_integration.py
-tests/integration/test_providers_integration.py
+tests/integration/cloudbender/__init__.py
+tests/integration/cloudbender/test_providers_integration.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/test_auth.py
 tests/unit/test_checkpoints_unit.py
 tests/unit/test_connections_unit.py
 tests/unit/test_datasets_unit.py
 tests/unit/test_environments_unit.py
 tests/unit/test_exceptions.py
 tests/unit/test_gpu_types_unit.py
 tests/unit/test_jobs_unit.py
 tests/unit/test_models_unit.py
 tests/unit/test_projects_unit.py
-tests/unit/test_providers_unit.py
 tests/unit/test_trainml.py
 tests/unit/cli/__init__.py
 tests/unit/cli/conftest.py
+tests/unit/cli/test_cli_checkpoint_unit.py
+tests/unit/cli/test_cli_datasets_unit.py
 tests/unit/cli/test_cli_environment_unit.py
+tests/unit/cli/test_cli_gpu_unit.py
+tests/unit/cli/test_cli_job_unit.py
+tests/unit/cli/test_cli_model_unit.py
+tests/unit/cli/test_cli_project_unit.py
+tests/unit/cli/cloudbender/__init__.py
+tests/unit/cli/cloudbender/test_cli_datastore_unit.py
+tests/unit/cli/cloudbender/test_cli_node_unit.py
+tests/unit/cli/cloudbender/test_cli_provider_unit.py
+tests/unit/cli/cloudbender/test_cli_region_unit.py
+tests/unit/cli/cloudbender/test_cli_reservation_unit.py
+tests/unit/cloudbender/__init__.py
+tests/unit/cloudbender/test_datastores_unit.py
+tests/unit/cloudbender/test_device_configs_unit.py
+tests/unit/cloudbender/test_nodes_unit.py
+tests/unit/cloudbender/test_providers_unit.py
+tests/unit/cloudbender/test_regions_unit.py
+tests/unit/cloudbender/test_reservations_unit.py
 trainml/__init__.py
 trainml/__main__.py
 trainml/auth.py
 trainml/checkpoints.py
 trainml/connections.py
 trainml/datasets.py
 trainml/environments.py
 trainml/exceptions.py
 trainml/gpu_types.py
 trainml/jobs.py
 trainml/models.py
 trainml/projects.py
-trainml/providers.py
 trainml/trainml.py
 trainml.egg-info/PKG-INFO
 trainml.egg-info/SOURCES.txt
 trainml.egg-info/dependency_links.txt
 trainml.egg-info/entry_points.txt
 trainml.egg-info/requires.txt
 trainml.egg-info/top_level.txt
@@ -57,10 +75,23 @@
 trainml/cli/checkpoint.py
 trainml/cli/connection.py
 trainml/cli/dataset.py
 trainml/cli/environment.py
 trainml/cli/gpu.py
 trainml/cli/model.py
 trainml/cli/project.py
-trainml/cli/provider.py
+trainml/cli/cloudbender/__init__.py
+trainml/cli/cloudbender/datastore.py
+trainml/cli/cloudbender/node.py
+trainml/cli/cloudbender/provider.py
+trainml/cli/cloudbender/region.py
+trainml/cli/cloudbender/reservation.py
 trainml/cli/job/__init__.py
-trainml/cli/job/create.py
+trainml/cli/job/create.py
+trainml/cloudbender/__init__.py
+trainml/cloudbender/cloudbender.py
+trainml/cloudbender/datastores.py
+trainml/cloudbender/device_configs.py
+trainml/cloudbender/nodes.py
+trainml/cloudbender/providers.py
+trainml/cloudbender/regions.py
+trainml/cloudbender/reservations.py
```

