# Comparing `tmp/jobbergate_api-3.5.0a4.tar.gz` & `tmp/jobbergate_api-3.5.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jobbergate_api-3.5.0a4.tar", max compression
+gzip compressed data, was "jobbergate_api-3.5.0a5.tar", max compression
```

## Comparing `jobbergate_api-3.5.0a4.tar` & `jobbergate_api-3.5.0a5.tar`

### file list

```diff
@@ -1,61 +1,61 @@
--rw-r--r--   0        0        0     1082 2023-06-12 18:40:59.727394 jobbergate_api-3.5.0a4/LICENSE
--rw-r--r--   0        0        0      738 2023-06-12 18:40:59.727394 jobbergate_api-3.5.0a4/README.rst
--rw-r--r--   0        0        0      169 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/__init__.py
--rw-r--r--   0        0        0       30 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/__init__.py
--rw-r--r--   0        0        0       41 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/__init__.py
--rw-r--r--   0        0        0     5655 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/application_files.py
--rw-r--r--   0        0        0      234 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/constants.py
--rw-r--r--   0        0        0     9408 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/file_validation.py
--rw-r--r--   0        0        0     1474 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/models.py
--rw-r--r--   0        0        0    14123 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/routers.py
--rw-r--r--   0        0        0     7421 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/schemas.py
--rw-r--r--   0        0        0       40 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0    12157 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/job_script_files.py
--rw-r--r--   0        0        0     1287 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/models.py
--rw-r--r--   0        0        0    15623 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/routers.py
--rw-r--r--   0        0        0     4088 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/schemas.py
--rw-r--r--   0        0        0       44 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0      529 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/constants.py
--rw-r--r--   0        0        0     1909 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/models.py
--rw-r--r--   0        0        0    12331 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/properties_parser.py
--rw-r--r--   0        0        0    18431 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/routers.py
--rw-r--r--   0        0        0    15946 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/schemas.py
--rw-r--r--   0        0        0      554 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/apps/permissions.py
--rw-r--r--   0        0        0     3621 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/config.py
--rw-r--r--   0        0        0     2466 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/email_notification.py
--rw-r--r--   0        0        0     3268 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/main.py
--rw-r--r--   0        0        0     3433 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/meta_mapper.py
--rw-r--r--   0        0        0       96 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/metadata.py
--rw-r--r--   0        0        0     3470 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/pagination.py
--rw-r--r--   0        0        0     2284 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/s3_manager.py
--rw-r--r--   0        0        0     2166 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/security.py
--rw-r--r--   0        0        0     5580 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/storage.py
--rw-r--r--   0        0        0       40 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-06-12 18:40:59.731395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/__init__.py
--rw-r--r--   0        0        0       44 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/__init__.py
--rw-r--r--   0        0        0    10634 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_application_files.py
--rw-r--r--   0        0        0     1967 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_file_validation.py
--rw-r--r--   0        0        0    44032 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_routers.py
--rw-r--r--   0        0        0     5180 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_schemas.py
--rw-r--r--   0        0        0     2756 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/conftest.py
--rw-r--r--   0        0        0       42 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/__init__.py
--rw-r--r--   0        0        0     1376 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/conftest.py
--rw-r--r--   0        0        0    11518 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
--rw-r--r--   0        0        0    52389 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_routers.py
--rw-r--r--   0        0        0       46 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/__init__.py
--rw-r--r--   0        0        0    24706 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
--rw-r--r--   0        0        0    78149 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_routers.py
--rw-r--r--   0        0        0      511 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/test_main.py
--rw-r--r--   0        0        0     8900 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/conftest.py
--rw-r--r--   0        0        0     4503 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
--rw-r--r--   0        0        0     3215 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_config.py
--rw-r--r--   0        0        0     4974 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_email_notification.py
--rw-r--r--   0        0        0     3177 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_meta_mapper.py
--rw-r--r--   0        0        0     3959 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_pagination.py
--rw-r--r--   0        0        0     1146 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_s3_manager.py
--rw-r--r--   0        0        0     2718 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_security.py
--rw-r--r--   0        0        0     4512 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_storage.py
--rw-r--r--   0        0        0     2777 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/tests/test_version.py
--rw-r--r--   0        0        0     1102 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/jobbergate_api/version.py
--rw-r--r--   0        0        0     2898 2023-06-12 18:40:59.735395 jobbergate_api-3.5.0a4/pyproject.toml
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/LICENSE
+-rw-r--r--   0        0        0      738 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/README.rst
+-rw-r--r--   0        0        0      169 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/__init__.py
+-rw-r--r--   0        0        0       30 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/__init__.py
+-rw-r--r--   0        0        0       41 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/__init__.py
+-rw-r--r--   0        0        0     5655 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/application_files.py
+-rw-r--r--   0        0        0      234 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/constants.py
+-rw-r--r--   0        0        0     9408 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/file_validation.py
+-rw-r--r--   0        0        0     1474 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/models.py
+-rw-r--r--   0        0        0    14123 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/routers.py
+-rw-r--r--   0        0        0     7421 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/schemas.py
+-rw-r--r--   0        0        0       40 2023-06-22 17:40:37.483250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0    12639 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/job_script_files.py
+-rw-r--r--   0        0        0     1287 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/models.py
+-rw-r--r--   0        0        0    17426 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/routers.py
+-rw-r--r--   0        0        0     3800 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/schemas.py
+-rw-r--r--   0        0        0       44 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0      529 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/constants.py
+-rw-r--r--   0        0        0     1909 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/models.py
+-rw-r--r--   0        0        0    12331 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/properties_parser.py
+-rw-r--r--   0        0        0    18431 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/routers.py
+-rw-r--r--   0        0        0    15946 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/schemas.py
+-rw-r--r--   0        0        0      554 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/apps/permissions.py
+-rw-r--r--   0        0        0     3621 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/config.py
+-rw-r--r--   0        0        0     2466 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/email_notification.py
+-rw-r--r--   0        0        0     3268 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/main.py
+-rw-r--r--   0        0        0     3433 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/meta_mapper.py
+-rw-r--r--   0        0        0       96 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/metadata.py
+-rw-r--r--   0        0        0     3470 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/pagination.py
+-rw-r--r--   0        0        0     2284 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/s3_manager.py
+-rw-r--r--   0        0        0     2166 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/security.py
+-rw-r--r--   0        0        0     5580 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/storage.py
+-rw-r--r--   0        0        0       40 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/__init__.py
+-rw-r--r--   0        0        0       44 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/__init__.py
+-rw-r--r--   0        0        0    10634 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_application_files.py
+-rw-r--r--   0        0        0     1967 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_file_validation.py
+-rw-r--r--   0        0        0    44032 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_routers.py
+-rw-r--r--   0        0        0     5180 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_schemas.py
+-rw-r--r--   0        0        0     2756 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/conftest.py
+-rw-r--r--   0        0        0       42 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/__init__.py
+-rw-r--r--   0        0        0     1376 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/conftest.py
+-rw-r--r--   0        0        0    11518 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py
+-rw-r--r--   0        0        0    53958 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_routers.py
+-rw-r--r--   0        0        0       46 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/__init__.py
+-rw-r--r--   0        0        0    24706 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py
+-rw-r--r--   0        0        0    78149 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_routers.py
+-rw-r--r--   0        0        0      511 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/test_main.py
+-rw-r--r--   0        0        0     8900 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/conftest.py
+-rw-r--r--   0        0        0     4503 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py
+-rw-r--r--   0        0        0     3215 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_config.py
+-rw-r--r--   0        0        0     4974 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_email_notification.py
+-rw-r--r--   0        0        0     3177 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_meta_mapper.py
+-rw-r--r--   0        0        0     3959 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_pagination.py
+-rw-r--r--   0        0        0     1146 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_s3_manager.py
+-rw-r--r--   0        0        0     2718 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_security.py
+-rw-r--r--   0        0        0     4512 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_storage.py
+-rw-r--r--   0        0        0     2777 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/tests/test_version.py
+-rw-r--r--   0        0        0     1102 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/jobbergate_api/version.py
+-rw-r--r--   0        0        0     2898 2023-06-22 17:40:37.487250 jobbergate_api-3.5.0a5/pyproject.toml
+-rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 jobbergate_api-3.5.0a5/PKG-INFO
```

### Comparing `jobbergate_api-3.5.0a4/LICENSE` & `jobbergate_api-3.5.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/README.rst` & `jobbergate_api-3.5.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/application_files.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/file_validation.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/models.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/routers.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/applications/schemas.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/applications/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/job_script_files.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/job_script_files.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Provide a convenience class for managing job-script files.
 """
 
 from pathlib import Path
 from typing import Any, Dict, List, Optional, cast
 
 from buzz import Buzz, require_condition
+from fastapi import UploadFile
 from file_storehouse import FileManager
 from jinja2 import Template
 from loguru import logger
 from pydantic import BaseModel, root_validator
 
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.schemas import ApplicationConfig
@@ -143,14 +144,26 @@
     def main_file(self):
         """
         Obtain the main file with this helper property.
         """
         return self.files.get(self.main_file_path)
 
     @classmethod
+    def get_from_single_upload_file(cls, upload_file: UploadFile):
+        """
+        Initialize a JobScriptFiles from a single upload file.
+        """
+        logger.debug("Creating JobScriptFiles from single upload file")
+        main_file_path = Path(".", upload_file.filename)
+        return cls(
+            main_file_path=main_file_path,
+            files={main_file_path: upload_file.file.read().decode("utf-8")},
+        )
+
+    @classmethod
     def get_from_s3(cls, job_script_id: int):
         """
         Alternative method to initialize the model getting the objects from S3.
         """
         logger.debug(f"Getting job-script files from S3: {job_script_id=}")
         file_manager = cls.file_manager_factory(job_script_id)
```

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/models.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/routers.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/routers.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     JOBSCRIPTS_MAIN_FILE_FOLDER,
     JobScriptCreationError,
     JobScriptFiles,
 )
 from jobbergate_api.apps.job_scripts.models import job_scripts_table, searchable_fields, sortable_fields
 from jobbergate_api.apps.job_scripts.schemas import (
     JobScriptCreateRequest,
-    JobScriptPartialResponse,
     JobScriptResponse,
     JobScriptUpdateRequest,
 )
 from jobbergate_api.apps.job_submissions.models import job_submissions_table
 from jobbergate_api.apps.permissions import Permissions
 from jobbergate_api.pagination import Pagination, ok_response, package_response
 from jobbergate_api.security import IdentityClaims, guard
@@ -51,50 +50,57 @@
     """
     Create a new job script.
 
     Make a post request to this endpoint with the required values to create a new job script.
     """
     logger.debug(f"Creating {job_script=}")
 
-    select_query = applications_table.select().where(applications_table.c.id == job_script.application_id)
-    logger.trace(f"select_query = {render_sql(select_query)}")
-
-    raw_application = await database.fetch_one(select_query)
-
-    if not raw_application:
-        message = f"Application with id={job_script.application_id} not found."
-        logger.warning(message)
-        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
-
-    application = ApplicationResponse.parse_obj(raw_application)
-
-    if application.application_uploaded is False:
-        raise HTTPException(
-            status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
-            detail=f"Application with id={job_script.application_id} was not uploaded.",
-        )
+    jobscript_files = None
+    application_name = None
+    if job_script.application_id is not None:
+        select_query = applications_table.select().where(applications_table.c.id == job_script.application_id)
+        logger.trace(f"select_query = {render_sql(select_query)}")
+
+        raw_application = await database.fetch_one(select_query)
+
+        if not raw_application:
+            message = f"Application with id={job_script.application_id} not found."
+            logger.warning(message)
+            raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+        application = ApplicationResponse.parse_obj(raw_application)
+        application_name = application.application_name
+
+        if application.application_uploaded is False:
+            raise HTTPException(
+                status_code=status.HTTP_422_UNPROCESSABLE_ENTITY,
+                detail=f"Application with id={job_script.application_id} was not uploaded.",
+            )
+        try:
+            jobscript_files = JobScriptFiles.render_from_application(
+                application_files=ApplicationFiles.get_from_s3(application.id),
+                user_supplied_parameters=job_script.param_dict or {},
+                sbatch_params=job_script.sbatch_params or [],
+            )
+        except JobScriptCreationError as e:
+            message = str(e)
+            logger.error(message)
+            raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=message)
 
     identity_claims = IdentityClaims.from_token_payload(token_payload)
 
     create_dict = dict(
-        **{k: v for (k, v) in job_script.dict(exclude_unset=True).items() if k != "param_dict"},
+        **{
+            k: v
+            for (k, v) in job_script.dict(exclude_unset=True).items()
+            if k not in ("param_dict", "sbatch_params")
+        },
         job_script_owner_email=identity_claims.email,
     )
 
-    try:
-        jobscript_files = JobScriptFiles.render_from_application(
-            application_files=ApplicationFiles.get_from_s3(application.id),
-            user_supplied_parameters=job_script.param_dict,
-            sbatch_params=create_dict.pop("sbatch_params", []),
-        )
-    except JobScriptCreationError as e:
-        message = str(e)
-        logger.error(message)
-        raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=message)
-
     logger.debug("Inserting job_script")
 
     async with database.transaction():
 
         try:
             insert_query = job_scripts_table.insert().returning(job_scripts_table)
             logger.trace(f"insert_query = {render_sql(insert_query)}")
@@ -104,29 +110,30 @@
                 message = "An error occurred when inserting the JobScript at the database."
                 logger.error(message)
                 raise HTTPException(
                     status_code=status.HTTP_400_BAD_REQUEST,
                     detail=message,
                 )
 
-            jobscript_files.write_to_s3(job_script_data["id"])
+            if jobscript_files:
+                jobscript_files.write_to_s3(job_script_data["id"])
 
         except INTEGRITY_CHECK_EXCEPTIONS as e:
             logger.error(f"Reverting database transaction: {str(e)}")
             raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e))
 
         except KeyError as e:
             logger.error(f"Reverting database transaction: {str(e)}")
             raise HTTPException(status_code=status.HTTP_422_UNPROCESSABLE_ENTITY, detail=str(e))
 
     logger.debug(f"Job-script created: {dict(job_script_data)}")
 
     response = JobScriptResponse(
         **job_script_data,
-        application_name=application.application_name,
+        application_name=application_name,
         job_script_files=jobscript_files,
     )
     return response
 
 
 @router.get(
     "/job-scripts/{job_script_id}",
@@ -143,14 +150,15 @@
     query = (
         select([job_scripts_table, applications_table.c.application_name])
         .select_from(
             join(
                 job_scripts_table,
                 applications_table,
                 applications_table.columns.id == job_scripts_table.columns.application_id,
+                isouter=True,
             )
         )
         .where(job_scripts_table.c.id == job_script_id)
     )
     logger.trace(f"get_query = {render_sql(query)}")
     job_script = await database.fetch_one(query)
 
@@ -176,14 +184,49 @@
         )
 
     logger.debug(f"Job-script data: {response}")
 
     return response
 
 
+@router.post(
+    "/job-scripts/{job_script_id}/upload",
+    status_code=status.HTTP_200_OK,
+    description="Endpoint to upload a new job script file.",
+    dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
+)
+async def job_script_create_file_content(
+    job_script_id: int = Query(...),
+    job_script_file: UploadFile = File(...),
+):
+    """Create a job script file (only if the job script has none)."""
+    logger.debug(f"Creating the main file for {job_script_id=}")
+
+    query = job_scripts_table.select().where(job_scripts_table.c.id == job_script_id)
+    logger.trace(f"get_query = {render_sql(query)}")
+    job_script = await database.fetch_one(query)
+
+    if not job_script:
+        message = f"JobScript with id={job_script_id} was not found."
+        logger.warning(message)
+        raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
+
+    jobscript_files = JobScriptFiles.get_from_single_upload_file(job_script_file)
+    jobscript_files.write_to_s3(job_script_id, remove_previous_files=True)
+
+    update_query = (
+        job_scripts_table.update()
+        .where(job_scripts_table.c.id == job_script["id"])
+        .values(updated_at=func.now())
+    )
+    await database.execute(update_query)
+    logger.debug(f"Success creating job script files from single upload file for {job_script_id=}")
+    return dict(message=f"Successfully uploaded {job_script_file.filename} for {job_script_id=}")
+
+
 @router.patch(
     "/job-scripts/{job_script_id}/upload",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to replace a job script file.",
     dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
 )
 async def job_script_replace_file_content(
@@ -255,15 +298,15 @@
     logger.warning(message)
     raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=message)
 
 
 @router.get(
     "/job-scripts",
     description="Endpoint to list job_scripts",
-    responses=ok_response(JobScriptPartialResponse),
+    responses=ok_response(JobScriptResponse),
 )
 async def job_script_list(
     pagination: Pagination = Depends(),
     all: Optional[bool] = Query(False),
     include_archived: bool = Query(False),
     search: Optional[str] = Query(None),
     sort_field: Optional[str] = Query(None),
@@ -286,14 +329,15 @@
     logger.debug("Preparing to list job-scripts")
 
     query = select([job_scripts_table, applications_table.c.application_name]).select_from(
         join(
             job_scripts_table,
             applications_table,
             applications_table.c.id == job_scripts_table.c.application_id,
+            isouter=True,
         )
     )
     identity_claims = IdentityClaims.from_token_payload(token_payload)
     if not all:
         query = query.where(job_scripts_table.c.job_script_owner_email == identity_claims.email)
     if not include_archived:
         query = query.where(not_(job_scripts_table.c.is_archived))
@@ -303,15 +347,15 @@
         query = query.where(search_clause(search, searchable_fields))
     if sort_field is not None:
         query = query.order_by(sort_clause(sort_field, sortable_fields, sort_ascending))
     else:
         query = query.order_by(job_scripts_table.c.id.asc())
 
     logger.debug(f"Query = {render_sql(query)}")
-    return await package_response(JobScriptPartialResponse, query, pagination)
+    return await package_response(JobScriptResponse, query, pagination)
 
 
 @router.delete(
     "/job-scripts/{job_script_id}",
     status_code=status.HTTP_204_NO_CONTENT,
     description="Endpoint to delete job script",
     dependencies=[Depends(guard.lockdown(Permissions.JOB_SCRIPTS_EDIT))],
```

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_scripts/schemas.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_scripts/schemas.py`

 * *Files 19% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 class JobScriptCreateRequest(BaseModel):
     """
     Request model for creating JobScript instances.
     """
 
     job_script_name: str
     job_script_description: Optional[str]
-    application_id: int
+    application_id: Optional[int]
     sbatch_params: Optional[List[str]]
     param_dict: Optional[Dict[str, Any]]
 
     class Config:
         schema_extra = job_script_meta_mapper
 
 
@@ -91,41 +91,28 @@
     param_dict: Optional[str]
     is_archived: Optional[bool]
 
     class Config:
         schema_extra = job_script_meta_mapper
 
 
-class JobScriptPartialResponse(BaseModel):
+class JobScriptResponse(BaseModel):
     """
     Complete model to match database for the JobScript resource.
 
     Notice this model does not include job_script_files from S3.
     """
 
     id: Optional[int] = None
     created_at: Optional[datetime] = None
     updated_at: Optional[datetime] = None
     job_script_name: str
     job_script_description: Optional[str] = None
+    job_script_files: Optional[JobScriptFiles] = None
     job_script_owner_email: str
     application_name: Optional[str] = None
     application_id: Optional[int] = None
     is_archived: bool
 
     class Config:
         orm_mode = True
         schema_extra = job_script_meta_mapper
-
-
-class JobScriptResponse(JobScriptPartialResponse):
-    """
-    Complete model to match database for the JobScript resource.
-
-    In addition to the field job_script_files from S3, for the JobScript resource.
-    """
-
-    job_script_files: JobScriptFiles
-
-    class Config:
-        orm_mode = True
-        schema_extra = job_script_meta_mapper
```

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/constants.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/constants.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/models.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/models.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/properties_parser.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/routers.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/job_submissions/schemas.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/job_submissions/schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/apps/permissions.py` & `jobbergate_api-3.5.0a5/jobbergate_api/apps/permissions.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/config.py` & `jobbergate_api-3.5.0a5/jobbergate_api/config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/email_notification.py` & `jobbergate_api-3.5.0a5/jobbergate_api/email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/main.py` & `jobbergate_api-3.5.0a5/jobbergate_api/main.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/meta_mapper.py` & `jobbergate_api-3.5.0a5/jobbergate_api/meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/pagination.py` & `jobbergate_api-3.5.0a5/jobbergate_api/pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/s3_manager.py` & `jobbergate_api-3.5.0a5/jobbergate_api/s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/security.py` & `jobbergate_api-3.5.0a5/jobbergate_api/security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/storage.py` & `jobbergate_api-3.5.0a5/jobbergate_api/storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_application_files.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_application_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_file_validation.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_file_validation.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_routers.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/applications/test_schemas.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/applications/test_schemas.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/conftest.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/conftest.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_job_script_files.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_scripts/test_routers.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_scripts/test_routers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pytest
 from fastapi import status
 
 from jobbergate_api.apps.applications.application_files import ApplicationFiles
 from jobbergate_api.apps.applications.models import applications_table
 from jobbergate_api.apps.job_scripts.job_script_files import JobScriptFiles
 from jobbergate_api.apps.job_scripts.models import job_scripts_table
-from jobbergate_api.apps.job_scripts.schemas import JobScriptPartialResponse, JobScriptResponse
+from jobbergate_api.apps.job_scripts.schemas import JobScriptResponse
 from jobbergate_api.apps.job_submissions.models import job_submissions_table
 from jobbergate_api.apps.permissions import Permissions
 from jobbergate_api.storage import database
 
 # Force the async event loop at the app to begin.
 # Since this is a time consuming fixture, it is just used where strict necessary.
 pytestmark = pytest.mark.usefixtures("startup_event_force")
@@ -74,15 +74,15 @@
     """
     return ["--comment=some_comment", "--nice=-1", "-N 10"]
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
 @mock.patch("jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.write_to_s3")
-async def test_create_job_script(
+async def test_create_job_script__with_application(
     mocked_write_job_script_files_to_s3,
     fill_application_data,
     job_script_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
@@ -90,15 +90,15 @@
     dummy_application_config,
     dummy_application_source_file,
     dummy_template,
     job_script_data_as_string,
     mocked_file_manager_factory,
 ):
     """
-    Test POST /job_scripts/ correctly creates a job_script.
+    Test POST /job_scripts/ correctly creates a job_script with a source application.
 
     This test proves that a job_script is successfully created via a POST request to the /job-scripts/
     endpoint. We show this by asserting that the job_script is created in the database after the post
     request is made, the correct status code (201) is returned.
     """
     inserted_application_id = await database.execute(
         query=applications_table.insert(),
@@ -142,14 +142,57 @@
     assert job_script.created_at in window
     assert job_script.updated_at in window
     assert job_script.job_script_files.main_file == job_script_data_as_string
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
+async def test_create_job_script__without_application(
+    job_script_data,
+    fill_job_script_data,
+    param_dict,
+    client,
+    inject_security_header,
+    time_frame,
+):
+    """
+    Test POST /job_scripts/ correctly creates a job_script without a source application.
+
+    This test proves that a job_script is successfully created via a POST request to the /job-scripts/
+    endpoint without specifying a source application_id. We show this by asserting that the job_script is
+    created in the database after the post request is made, the correct status code (201) is returned.
+    """
+    inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
+    with time_frame() as window:
+        response = await client.post(
+            "/jobbergate/job-scripts/",
+            json=fill_job_script_data(
+                param_dict=param_dict,
+            ),
+        )
+
+    assert response.status_code == status.HTTP_201_CREATED
+
+    id_rows = await database.fetch_all("SELECT id FROM job_scripts")
+    assert len(id_rows) == 1
+
+    job_script = JobScriptResponse(**response.json())
+
+    assert job_script.id == id_rows[0][0]
+    assert job_script.job_script_name == job_script_data["job_script_name"]
+    assert job_script.job_script_owner_email == "owner1@org.com"
+    assert job_script.job_script_description is None
+    assert job_script.job_script_files is None
+    assert job_script.application_id is None
+    assert job_script.created_at in window
+    assert job_script.updated_at in window
+
+
+@pytest.mark.asyncio
+@database.transaction(force_rollback=True)
 async def test_create_job_script_application_not_uploaded(
     fill_application_data,
     fill_job_script_data,
     param_dict,
     client,
     inject_security_header,
 ):
@@ -511,15 +554,15 @@
         main_file_path=main_file_path, files={main_file_path: new_file_content}
     )
     actual_job_script_files = JobScriptFiles.get_from_s3(inserted_job_script_id)
 
     assert actual_job_script_files == expected_job_script_files
 
     query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
-    job_script = JobScriptPartialResponse.parse_obj(await database.fetch_one(query))
+    job_script = JobScriptResponse.parse_obj(await database.fetch_one(query))
 
     assert job_script.updated_at in window
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
 async def test_upload_job_script_file_by_id__job_script_not_found(
@@ -1193,15 +1236,15 @@
     assert data["job_script_description"] == "new description"
     assert JobScriptFiles(**data["job_script_files"]) == dummy_job_script_files
     assert JobScriptFiles.get_from_s3(inserted_job_script_id) == dummy_job_script_files
     assert data["id"] == inserted_job_script_id
     assert data["is_archived"] is True
 
     query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
-    job_script = JobScriptPartialResponse.parse_obj(await database.fetch_one(query))
+    job_script = JobScriptResponse.parse_obj(await database.fetch_one(query))
 
     assert job_script is not None
     assert job_script.job_script_name == "new name"
     assert job_script.job_script_description == "new description"
     assert job_script.updated_at in window
     assert job_script.is_archived
 
@@ -1244,15 +1287,15 @@
     inserted_job_script_id = await database.execute(
         query=job_scripts_table.insert(),
         values=fill_job_script_data(application_id=inserted_application_id),
     )
 
     query = job_scripts_table.select(job_scripts_table.c.id == inserted_job_script_id)
 
-    desired_jobscript_data = JobScriptPartialResponse.parse_obj(await database.fetch_one(query))
+    desired_jobscript_data = JobScriptResponse.parse_obj(await database.fetch_one(query))
 
     inject_security_header("owner1@org.com", Permissions.JOB_SCRIPTS_EDIT)
 
     with mock.patch(
         "jobbergate_api.apps.job_scripts.job_script_files.JobScriptFiles.write_to_s3",
         side_effect=KeyError,
     ):
@@ -1264,15 +1307,15 @@
                 "job_script_data_as_string": "new value",
             },
         )
 
     assert response.status_code == status.HTTP_404_NOT_FOUND
     assert "not found in S3" in response.text
 
-    actual_jobscript_data = JobScriptPartialResponse.parse_obj(await database.fetch_one(query))
+    actual_jobscript_data = JobScriptResponse.parse_obj(await database.fetch_one(query))
 
     assert desired_jobscript_data.json() == actual_jobscript_data.json()
 
 
 @pytest.mark.asyncio
 @database.transaction(force_rollback=True)
 async def test_update_job_script_bad_permission(
```

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_properties_parser.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/apps/job_submissions/test_routers.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/apps/job_submissions/test_routers.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/conftest.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/integration/draft_test_jobbergate_slurm_job_properties.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_config.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_email_notification.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_email_notification.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_meta_mapper.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_meta_mapper.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_pagination.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_s3_manager.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_s3_manager.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_security.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_security.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_storage.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/tests/test_version.py` & `jobbergate_api-3.5.0a5/jobbergate_api/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/jobbergate_api/version.py` & `jobbergate_api-3.5.0a5/jobbergate_api/version.py`

 * *Files identical despite different names*

### Comparing `jobbergate_api-3.5.0a4/pyproject.toml` & `jobbergate_api-3.5.0a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jobbergate-api"
-version = "3.5.0a4"
+version = "3.5.0a5"
 description = "Jobbergate API"
 authors = ["Omnivector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/jobbergate"
 classifiers = [
     "License :: OSI Approved :: MIT License",
```

### Comparing `jobbergate_api-3.5.0a4/PKG-INFO` & `jobbergate_api-3.5.0a5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jobbergate-api
-Version: 3.5.0a4
+Version: 3.5.0a5
 Summary: Jobbergate API
 Home-page: https://github.com/omnivector-solutions/jobbergate
 License: MIT
 Author: Omnivector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

