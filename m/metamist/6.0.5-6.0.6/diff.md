# Comparing `tmp/metamist-6.0.5.tar.gz` & `tmp/metamist-6.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metamist-6.0.5.tar", last modified: Sun Jun 18 23:47:45 2023, max compression
+gzip compressed data, was "metamist-6.0.6.tar", last modified: Thu Jun 22 11:50:42 2023, max compression
```

## Comparing `metamist-6.0.5.tar` & `metamist-6.0.6.tar`

### file list

```diff
@@ -1,108 +1,116 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.185627 metamist-6.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-18 23:41:45.000000 metamist-6.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-18 23:41:45.000000 metamist-6.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-18 23:47:45.181627 metamist-6.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-06-18 23:41:45.000000 metamist-6.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.157627 metamist-6.0.5/metamist/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.161627 metamist-6.0.5/metamist/api/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55799 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/analysis_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/assay_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/enums_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/family_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41903 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/participant_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/sample_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    46958 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/seqr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/sequencing_group_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18066 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api/web_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.161627 metamist-6.0.5/metamist/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.161627 metamist-6.0.5/metamist/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-18 23:41:45.000000 metamist-6.0.5/metamist/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-18 23:44:48.000000 metamist-6.0.5/metamist/graphql/schema.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.169627 metamist-6.0.5/metamist/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/analysis_query_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/analysis_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/analysis_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/assay.py
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/assay_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/body_get_assays_by_criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/body_get_latest_complete_analysis_for_type_post.py
--rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/body_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/body_get_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/export_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/extra_participant_importer_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/family_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/family_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/family_update_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/meta_search_entity_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/nested_participant.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/nested_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/nested_sequencing_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/paging_links.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/participant_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/participant_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/project_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/sample_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/sample_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/search_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/search_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/search_response_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/search_response_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/sequencing_group_search_response_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/sequencing_group_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-18 23:44:42.000000 metamist-6.0.5/metamist/model/web_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.169627 metamist-6.0.5/metamist/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.173627 metamist-6.0.5/metamist/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 23:41:45.000000 metamist-6.0.5/metamist/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-18 23:41:45.000000 metamist-6.0.5/metamist/parser/cloudhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    31027 2023-06-18 23:41:45.000000 metamist-6.0.5/metamist/parser/generic_metadata_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-06-18 23:41:45.000000 metamist-6.0.5/metamist/parser/generic_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-06-18 23:41:45.000000 metamist-6.0.5/metamist/parser/sample_file_map_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-18 23:44:43.000000 metamist-6.0.5/metamist/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.157627 metamist-6.0.5/metamist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-18 23:47:45.000000 metamist-6.0.5/metamist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-18 23:47:45.000000 metamist-6.0.5/metamist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 23:47:45.000000 metamist-6.0.5/metamist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 23:47:45.000000 metamist-6.0.5/metamist.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-18 23:47:45.000000 metamist-6.0.5/metamist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-18 23:47:45.000000 metamist-6.0.5/metamist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-18 23:41:45.000000 metamist-6.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 23:47:45.185627 metamist-6.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-18 23:41:45.000000 metamist-6.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 23:47:45.181627 metamist-6.0.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11118 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    14896 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_assay.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_generate_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_generic_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_get_participants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_import_individual_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_metamist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_parse_existing_cohort.py
--rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_parse_file_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_parse_generic_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_parse_ont_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_parse_ont_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_pedigree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_sequencing_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_upsert.py
--rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-18 23:41:45.000000 metamist-6.0.5/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-18 23:41:45.000000 metamist-6.0.5/test/testbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.040164 metamist-6.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 11:44:49.000000 metamist-6.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 11:44:49.000000 metamist-6.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-22 11:50:42.040164 metamist-6.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10777 2023-06-22 11:44:49.000000 metamist-6.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.000163 metamist-6.0.6/metamist/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.004163 metamist-6.0.6/metamist/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/analysis_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23776 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/assay_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25181 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/enums_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28817 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/family_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47368 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/participant_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28288 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53117 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/sample_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46972 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/seqr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/sequencing_group_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18090 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api/web_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37543 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.008164 metamist-6.0.6/metamist/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.012163 metamist-6.0.6/metamist/audit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9376 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/audit_upload_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/audithelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/delete_sequence_files_from_audit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27845 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/audit/generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17007 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.012163 metamist-6.0.6/metamist/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-22 11:47:48.000000 metamist-6.0.6/metamist/graphql/schema.graphql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.020164 metamist-6.0.6/metamist/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13546 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis_query_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/analysis_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/assay_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12827 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_assays_by_criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_latest_complete_analysis_for_type_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12236 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/body_get_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/export_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/extra_participant_importer_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11866 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/family_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/family_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/family_update_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/meta_search_entity_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13138 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/nested_participant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/nested_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/nested_sequencing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/paging_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/participant_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13524 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/participant_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12248 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/project_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sample_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sample_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_response_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/search_response_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sequencing_group_search_response_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/sequencing_group_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11641 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-22 11:47:42.000000 metamist-6.0.6/metamist/model/web_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82230 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.020164 metamist-6.0.6/metamist/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.024164 metamist-6.0.6/metamist/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/cloudhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31027 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/generic_metadata_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50852 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/generic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-22 11:44:49.000000 metamist-6.0.6/metamist/parser/sample_file_map_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12698 2023-06-22 11:47:43.000000 metamist-6.0.6/metamist/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.000163 metamist-6.0.6/metamist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11508 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 11:50:41.000000 metamist-6.0.6/metamist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 11:44:49.000000 metamist-6.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 11:50:42.040164 metamist-6.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-22 11:44:49.000000 metamist-6.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:50:42.040164 metamist-6.0.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_assay.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21470 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_generic_auditor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_generic_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_get_participants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_import_individual_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_metamist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_existing_cohort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7806 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_file_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_generic_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_ont_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5000 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_parse_ont_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_pedigree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_sequencing_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_update_participant_family.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_upsert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19228 2023-06-22 11:44:49.000000 metamist-6.0.6/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-22 11:44:49.000000 metamist-6.0.6/test/testbase.py
```

### Comparing `metamist-6.0.5/LICENSE` & `metamist-6.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/PKG-INFO` & `metamist-6.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.5
+Version: 6.0.6
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.5/README.md` & `metamist-6.0.6/README.md`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/metamist/__init__.py` & `metamist-6.0.6/metamist/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # flake8: noqa
 
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 __version__ = "1.0.0"
 
 # import ApiClient
```

### Comparing `metamist-6.0.5/metamist/api/analysis_api.py` & `metamist-6.0.6/metamist/api/analysis_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -465,15 +465,15 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'project',
                     'export_type',
-                    'sequence_types',
+                    'sequencing_types',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -487,29 +487,29 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'export_type':
                         (bool, date, datetime, dict, float, int, list, str, none_type,),
-                    'sequence_types':
+                    'sequencing_types':
                         ([str],),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'export_type': 'export_type',
-                    'sequence_types': 'sequence_types',
+                    'sequencing_types': 'sequencing_types',
                 },
                 'location_map': {
                     'project': 'path',
                     'export_type': 'query',
-                    'sequence_types': 'query',
+                    'sequencing_types': 'query',
                 },
                 'collection_format_map': {
-                    'sequence_types': 'multi',
+                    'sequencing_types': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -1223,15 +1223,15 @@
         >>> result = thread.get()
 
         Args:
             project (str):
 
         Keyword Args:
             export_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
-            sequence_types ([str]): [optional]
+            sequencing_types ([str]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `metamist-6.0.5/metamist/api/assay_api.py` & `metamist-6.0.6/metamist/api/assay_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -201,121 +201,14 @@
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
 
-        self.get_assay_ids_for_sample_id_by_type_async = async_wrap(self.get_assay_ids_for_sample_id_by_type)
-        self.get_assay_ids_for_sample_id_by_type_endpoint = _Endpoint(
-            settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [
-                    'HTTPBearer'
-                ],
-                'endpoint_path': '/api/v1/assay/ids-for-sample-by-type',
-                'operation_id': 'get_assay_ids_for_sample_id_by_type',
-                'http_method': 'GET',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'sample_id',
-                ],
-                'required': [
-                    'sample_id',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'sample_id':
-                        (str,),
-                },
-                'attribute_map': {
-                    'sample_id': 'sample_id',
-                },
-                'location_map': {
-                    'sample_id': 'query',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [],
-            },
-            api_client=api_client
-        )
-
-        self.get_assay_ids_for_sample_ids_by_type_async = async_wrap(self.get_assay_ids_for_sample_ids_by_type)
-        self.get_assay_ids_for_sample_ids_by_type_endpoint = _Endpoint(
-            settings={
-                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
-                'auth': [
-                    'HTTPBearer'
-                ],
-                'endpoint_path': '/api/v1/assay/ids-for-samples-by-type',
-                'operation_id': 'get_assay_ids_for_sample_ids_by_type',
-                'http_method': 'POST',
-                'servers': None,
-            },
-            params_map={
-                'all': [
-                    'request_body',
-                ],
-                'required': [
-                    'request_body',
-                ],
-                'nullable': [
-                ],
-                'enum': [
-                ],
-                'validation': [
-                ]
-            },
-            root_map={
-                'validations': {
-                },
-                'allowed_values': {
-                },
-                'openapi_types': {
-                    'request_body':
-                        ([str],),
-                },
-                'attribute_map': {
-                },
-                'location_map': {
-                    'request_body': 'body',
-                },
-                'collection_format_map': {
-                }
-            },
-            headers_map={
-                'accept': [
-                    'application/json'
-                ],
-                'content_type': [
-                    'application/json'
-                ]
-            },
-            api_client=api_client
-        )
-
         self.get_assays_by_criteria_async = async_wrap(self.get_assays_by_criteria)
         self.get_assays_by_criteria_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
@@ -631,156 +524,14 @@
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['assay_id'] = \
             assay_id
         return self.get_assay_by_id_endpoint.call_with_http_info(**kwargs)
 
-    def get_assay_ids_for_sample_id_by_type(
-        self,
-        sample_id,
-        **kwargs
-    ):
-        """Get Assay Ids For Sample Id  # noqa: E501
-
-        Get all assay IDs for internal Sample ID  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_assay_ids_for_sample_id_by_type(sample_id, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            sample_id (str):
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['sample_id'] = \
-            sample_id
-        return self.get_assay_ids_for_sample_id_by_type_endpoint.call_with_http_info(**kwargs)
-
-    def get_assay_ids_for_sample_ids_by_type(
-        self,
-        request_body,
-        **kwargs
-    ):
-        """Get Assay Ids For Sample Ids By Type  # noqa: E501
-
-        Get all assay IDs keyed by internal Sample ID  # noqa: E501
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_assay_ids_for_sample_ids_by_type(request_body, async_req=True)
-        >>> result = thread.get()
-
-        Args:
-            request_body ([str]):
-
-        Keyword Args:
-            _return_http_data_only (bool): response data without head status
-                code and headers. Default is True.
-            _preload_content (bool): if False, the urllib3.HTTPResponse object
-                will be returned without reading/decoding response data.
-                Default is True.
-            _request_timeout (int/float/tuple): timeout setting for this request. If
-                one number provided, it will be total request timeout. It can also
-                be a pair (tuple) of (connection, read) timeouts.
-                Default is None.
-            _check_input_type (bool): specifies if type checking
-                should be done one the data sent to the server.
-                Default is True.
-            _check_return_type (bool): specifies if type checking
-                should be done one the data received from the server.
-                Default is True.
-            _content_type (str/None): force body content-type.
-                Default is None and content-type will be predicted by allowed
-                content-types and body.
-            _host_index (int/None): specifies the index of the server
-                that we want to use.
-                Default is read from the configuration.
-            async_req (bool): execute request asynchronously
-
-        Returns:
-            bool, date, datetime, dict, float, int, list, str, none_type
-                If the method is called asynchronously, returns the request
-                thread.
-        """
-        kwargs['async_req'] = kwargs.get(
-            'async_req', False
-        )
-        kwargs['_return_http_data_only'] = kwargs.get(
-            '_return_http_data_only', True
-        )
-        kwargs['_preload_content'] = kwargs.get(
-            '_preload_content', True
-        )
-        kwargs['_request_timeout'] = kwargs.get(
-            '_request_timeout', None
-        )
-        kwargs['_check_input_type'] = kwargs.get(
-            '_check_input_type', True
-        )
-        kwargs['_check_return_type'] = kwargs.get(
-            '_check_return_type', True
-        )
-        kwargs['_content_type'] = kwargs.get(
-            '_content_type')
-        kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['request_body'] = \
-            request_body
-        return self.get_assay_ids_for_sample_ids_by_type_endpoint.call_with_http_info(**kwargs)
-
     def get_assays_by_criteria(
         self,
         **kwargs
     ):
         """Get Assays By Criteria  # noqa: E501
 
         Get assays by criteria  # noqa: E501
```

### Comparing `metamist-6.0.5/metamist/api/enums_api.py` & `metamist-6.0.6/metamist/api/enums_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/api/family_api.py` & `metamist-6.0.6/metamist/api/family_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/api/import_api.py` & `metamist-6.0.6/metamist/api/import_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/api/participant_api.py` & `metamist-6.0.6/metamist/api/participant_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -458,14 +458,79 @@
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
 
+        self.update_participant_family_async = async_wrap(self.update_participant_family)
+        self.update_participant_family_endpoint = _Endpoint(
+            settings={
+                'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
+                'auth': [
+                    'HTTPBearer'
+                ],
+                'endpoint_path': '/api/v1/participant/{participant_id}/update-participant-family',
+                'operation_id': 'update_participant_family',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'participant_id',
+                    'old_family_id',
+                    'new_family_id',
+                ],
+                'required': [
+                    'participant_id',
+                    'old_family_id',
+                    'new_family_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'participant_id':
+                        (int,),
+                    'old_family_id':
+                        (int,),
+                    'new_family_id':
+                        (int,),
+                },
+                'attribute_map': {
+                    'participant_id': 'participant_id',
+                    'old_family_id': 'old_family_id',
+                    'new_family_id': 'new_family_id',
+                },
+                'location_map': {
+                    'participant_id': 'path',
+                    'old_family_id': 'query',
+                    'new_family_id': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+
         self.upsert_participants_async = async_wrap(self.upsert_participants)
         self.upsert_participants_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
@@ -1030,14 +1095,93 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['participant_id'] = \
             participant_id
         kwargs['participant_upsert'] = \
             participant_upsert
         return self.update_participant_endpoint.call_with_http_info(**kwargs)
 
+    def update_participant_family(
+        self,
+        participant_id,
+        old_family_id,
+        new_family_id,
+        **kwargs
+    ):
+        """Update Participant Family  # noqa: E501
+
+        Change a participants family from old_family_id to new_family_id, maintaining all other fields. The new_family_id must already exist.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.update_participant_family(participant_id, old_family_id, new_family_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            participant_id (int):
+            old_family_id (int):
+            new_family_id (int):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            bool, date, datetime, dict, float, int, list, str, none_type
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['participant_id'] = \
+            participant_id
+        kwargs['old_family_id'] = \
+            old_family_id
+        kwargs['new_family_id'] = \
+            new_family_id
+        return self.update_participant_family_endpoint.call_with_http_info(**kwargs)
+
     def upsert_participants(
         self,
         project,
         participant_upsert,
         **kwargs
     ):
         """Upsert Participants  # noqa: E501
```

### Comparing `metamist-6.0.5/metamist/api/project_api.py` & `metamist-6.0.6/metamist/api/project_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/api/sample_api.py` & `metamist-6.0.6/metamist/api/sample_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/api/seqr_api.py` & `metamist-6.0.6/metamist/api/seqr_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -335,15 +335,15 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'project',
                     'export_type',
-                    'sequence_types',
+                    'sequencing_types',
                 ],
                 'required': [
                     'project',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -357,29 +357,29 @@
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'project':
                         (str,),
                     'export_type':
                         (bool, date, datetime, dict, float, int, list, str, none_type,),
-                    'sequence_types':
+                    'sequencing_types':
                         ([str],),
                 },
                 'attribute_map': {
                     'project': 'project',
                     'export_type': 'export_type',
-                    'sequence_types': 'sequence_types',
+                    'sequencing_types': 'sequencing_types',
                 },
                 'location_map': {
                     'project': 'path',
                     'export_type': 'query',
-                    'sequence_types': 'query',
+                    'sequencing_types': 'query',
                 },
                 'collection_format_map': {
-                    'sequence_types': 'multi',
+                    'sequencing_types': 'multi',
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
@@ -918,15 +918,15 @@
         >>> result = thread.get()
 
         Args:
             project (str):
 
         Keyword Args:
             export_type (bool, date, datetime, dict, float, int, list, str, none_type): [optional]
-            sequence_types ([str]): [optional]
+            sequencing_types ([str]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `metamist-6.0.5/metamist/api/sequencing_group_api.py` & `metamist-6.0.6/metamist/api/sequencing_group_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/api/web_api.py` & `metamist-6.0.6/metamist/api/web_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -166,33 +166,33 @@
         self.sync_seqr_project_async = async_wrap(self.sync_seqr_project)
         self.sync_seqr_project_endpoint = _Endpoint(
             settings={
                 'response_type': (bool, date, datetime, dict, float, int, list, str, none_type,),
                 'auth': [
                     'HTTPBearer'
                 ],
-                'endpoint_path': '/api/v1/web/{project}/{sequence_type}/sync-dataset',
+                'endpoint_path': '/api/v1/web/{project}/{sequencing_type}/sync-dataset',
                 'operation_id': 'sync_seqr_project',
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
-                    'sequence_type',
+                    'sequencing_type',
                     'project',
                     'sync_families',
                     'sync_individual_metadata',
                     'sync_individuals',
                     'sync_es_index',
                     'sync_saved_variants',
                     'sync_cram_map',
                     'post_slack_notification',
                 ],
                 'required': [
-                    'sequence_type',
+                    'sequencing_type',
                     'project',
                 ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
@@ -200,15 +200,15 @@
             },
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
-                    'sequence_type':
+                    'sequencing_type':
                         (str,),
                     'project':
                         (str,),
                     'sync_families':
                         (bool,),
                     'sync_individual_metadata':
                         (bool,),
@@ -220,26 +220,26 @@
                         (bool,),
                     'sync_cram_map':
                         (bool,),
                     'post_slack_notification':
                         (bool,),
                 },
                 'attribute_map': {
-                    'sequence_type': 'sequence_type',
+                    'sequencing_type': 'sequencing_type',
                     'project': 'project',
                     'sync_families': 'sync_families',
                     'sync_individual_metadata': 'sync_individual_metadata',
                     'sync_individuals': 'sync_individuals',
                     'sync_es_index': 'sync_es_index',
                     'sync_saved_variants': 'sync_saved_variants',
                     'sync_cram_map': 'sync_cram_map',
                     'post_slack_notification': 'post_slack_notification',
                 },
                 'location_map': {
-                    'sequence_type': 'path',
+                    'sequencing_type': 'path',
                     'project': 'path',
                     'sync_families': 'query',
                     'sync_individual_metadata': 'query',
                     'sync_individuals': 'query',
                     'sync_es_index': 'query',
                     'sync_saved_variants': 'query',
                     'sync_cram_map': 'query',
@@ -403,29 +403,29 @@
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['keyword'] = \
             keyword
         return self.search_by_keyword_endpoint.call_with_http_info(**kwargs)
 
     def sync_seqr_project(
         self,
-        sequence_type,
+        sequencing_type,
         project,
         **kwargs
     ):
         """Sync Seqr Project  # noqa: E501
 
         Sync a metamist project with its seqr project (for a specific sequence type)  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.sync_seqr_project(sequence_type, project, async_req=True)
+        >>> thread = api.sync_seqr_project(sequencing_type, project, async_req=True)
         >>> result = thread.get()
 
         Args:
-            sequence_type (str):
+            sequencing_type (str):
             project (str):
 
         Keyword Args:
             sync_families (bool): [optional] if omitted the server will use the default value of True
             sync_individual_metadata (bool): [optional] if omitted the server will use the default value of True
             sync_individuals (bool): [optional] if omitted the server will use the default value of True
             sync_es_index (bool): [optional] if omitted the server will use the default value of True
@@ -477,13 +477,13 @@
         )
         kwargs['_check_return_type'] = kwargs.get(
             '_check_return_type', True
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
-        kwargs['sequence_type'] = \
-            sequence_type
+        kwargs['sequencing_type'] = \
+            sequencing_type
         kwargs['project'] = \
             project
         return self.sync_seqr_project_endpoint.call_with_http_info(**kwargs)
```

### Comparing `metamist-6.0.5/metamist/api_client.py` & `metamist-6.0.6/metamist/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
```

### Comparing `metamist-6.0.5/metamist/apis/__init__.py` & `metamist-6.0.6/metamist/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/metamist/configuration.py` & `metamist-6.0.6/metamist/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from os import getenv
 import json
 import copy
@@ -402,15 +402,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 6.0.5\n"\
+               "Version of the API: 6.0.6\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `metamist-6.0.5/metamist/exceptions.py` & `metamist-6.0.6/metamist/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `metamist-6.0.5/metamist/graphql/__init__.py` & `metamist-6.0.6/metamist/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/metamist/graphql/schema.graphql` & `metamist-6.0.6/metamist/graphql/schema.graphql`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/metamist/model/analysis.py` & `metamist-6.0.6/metamist/model/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/analysis_query_model.py` & `metamist-6.0.6/metamist/model/analysis_query_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/analysis_status.py` & `metamist-6.0.6/metamist/model/analysis_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/analysis_update_model.py` & `metamist-6.0.6/metamist/model/analysis_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/assay.py` & `metamist-6.0.6/metamist/model/assay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/assay_upsert.py` & `metamist-6.0.6/metamist/model/assay_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/body_get_assays_by_criteria.py` & `metamist-6.0.6/metamist/model/body_get_assays_by_criteria.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/body_get_latest_complete_analysis_for_type_post.py` & `metamist-6.0.6/metamist/model/body_get_latest_complete_analysis_for_type_post.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/body_get_participants.py` & `metamist-6.0.6/metamist/model/body_get_participants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/body_get_samples.py` & `metamist-6.0.6/metamist/model/body_get_samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/error_response.py` & `metamist-6.0.6/metamist/model/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/export_type.py` & `metamist-6.0.6/metamist/model/export_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/extra_participant_importer_handler.py` & `metamist-6.0.6/metamist/model/extra_participant_importer_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/family_search_response_data.py` & `metamist-6.0.6/metamist/model/family_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/family_simple.py` & `metamist-6.0.6/metamist/model/family_simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/family_update_model.py` & `metamist-6.0.6/metamist/model/family_update_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/http_validation_error.py` & `metamist-6.0.6/metamist/model/http_validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/meta_search_entity_prefix.py` & `metamist-6.0.6/metamist/model/meta_search_entity_prefix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/nested_participant.py` & `metamist-6.0.6/metamist/model/nested_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/nested_sample.py` & `metamist-6.0.6/metamist/model/nested_sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/nested_sequencing_group.py` & `metamist-6.0.6/metamist/model/nested_sequencing_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/paging_links.py` & `metamist-6.0.6/metamist/model/paging_links.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/participant_search_response_data.py` & `metamist-6.0.6/metamist/model/participant_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/participant_upsert.py` & `metamist-6.0.6/metamist/model/participant_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/project.py` & `metamist-6.0.6/metamist/model/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/project_summary.py` & `metamist-6.0.6/metamist/model/project_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/sample_search_response_data.py` & `metamist-6.0.6/metamist/model/sample_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/sample_upsert.py` & `metamist-6.0.6/metamist/model/sample_upsert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/search_item.py` & `metamist-6.0.6/metamist/model/search_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/search_response.py` & `metamist-6.0.6/metamist/model/search_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/search_response_model.py` & `metamist-6.0.6/metamist/model/search_response_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/search_response_type.py` & `metamist-6.0.6/metamist/model/search_response_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/sequencing_group_search_response_data.py` & `metamist-6.0.6/metamist/model/sequencing_group_search_response_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/sequencing_group_upsert.py` & `metamist-6.0.6/metamist/model/sequencing_group_upsert.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/validation_error.py` & `metamist-6.0.6/metamist/model/validation_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model/web_project.py` & `metamist-6.0.6/metamist/model/web_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `metamist-6.0.5/metamist/model_utils.py` & `metamist-6.0.6/metamist/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `metamist-6.0.5/metamist/models/__init__.py` & `metamist-6.0.6/metamist/models/__init__.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/metamist/parser/cloudhelper.py` & `metamist-6.0.6/metamist/parser/cloudhelper.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/metamist/parser/generic_metadata_parser.py` & `metamist-6.0.6/metamist/parser/generic_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/metamist/parser/generic_parser.py` & `metamist-6.0.6/metamist/parser/generic_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 logger.setLevel(logging.INFO)
 
 FASTQ_EXTENSIONS = ('.fq.gz', '.fastq.gz', '.fq', '.fastq')
 BAM_EXTENSIONS = ('.bam',)
 CRAM_EXTENSIONS = ('.cram',)
 GVCF_EXTENSIONS = ('.g.vcf.gz',)
 VCF_EXTENSIONS = ('.vcf', '.vcf.gz')
+READS_EXTENSIONS = FASTQ_EXTENSIONS + CRAM_EXTENSIONS + BAM_EXTENSIONS
 
 ALL_EXTENSIONS = (
     FASTQ_EXTENSIONS
     + CRAM_EXTENSIONS
     + BAM_EXTENSIONS
     + GVCF_EXTENSIONS
     + VCF_EXTENSIONS
@@ -263,40 +264,40 @@
 
     def __init__(
         self,
         sample: ParsedSample,
         rows: GroupedRow,
         internal_seqgroup_id: int | None,
         external_seqgroup_id: str | None,
-        sequence_type: str,
+        sequencing_type: str,
         sequence_technology: str,
         sequence_platform: str | None,
         meta: dict[str, Any] | None,
     ):
         self.sample = sample
         self.rows = rows
 
         self.internal_seqgroup_id = internal_seqgroup_id
         self.external_seqgroup_id = external_seqgroup_id
-        self.sequencing_type = sequence_type
+        self.sequencing_type = sequencing_type
         self.sequencing_technology = sequence_technology
         self.sequencing_platform = sequence_platform
         self.meta = meta
 
         self.assays: list[ParsedAssay] = []
         self.analyses: list[ParsedAnalysis] = []
 
     def to_sm(self) -> SequencingGroupUpsert:
         """Convert to SM upsert model"""
         return SequencingGroupUpsert(
             type=self.sequencing_type,
             technology=self.sequencing_technology,
             platform=self.sequencing_platform,
             meta=self.meta,
-            assays=[sq.to_sm() for sq in self.assays],
+            assays=[sq.to_sm() for sq in self.assays or []],
             id=self.internal_seqgroup_id,
         )
 
 
 class ParsedAssay:
     """Parsed assay object, internal to parsers"""
 
@@ -946,15 +947,15 @@
             seq_type = self.get_sequencing_type(seq_rows[0])
             seq_tech = self.get_sequencing_technology(seq_rows[0])
             seq_platform = self.get_sequencing_platform(seq_rows[0])
 
             seq_group = ParsedSequencingGroup(
                 internal_seqgroup_id=None,
                 external_seqgroup_id=self.get_sequencing_group_id(seq_rows[0]),
-                sequence_type=seq_type,
+                sequencing_type=seq_type,
                 sequence_technology=seq_tech,
                 sequence_platform=seq_platform,
                 meta={},
                 sample=sample,
                 rows=seq_rows,
             )
```

### Comparing `metamist-6.0.5/metamist/parser/sample_file_map_parser.py` & `metamist-6.0.6/metamist/parser/sample_file_map_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     <sample-id>     <sample-id>.filename-R1.fastq.gz,<sample-id>.filename-R2.fastq.gz
     # OR
     <sample-id2>    <sample-id2>.filename-R1.fastq.gz
     <sample-id2>    <sample-id2>.filename-R2.fastq.gz
 
 Example with optional columns
 Note: Individual ID column must contain values in every row
-Note: Any missing values in Type will default to the default_sequence_type ('genome')
+Note: Any missing values in Type will default to the default_sequencing_type ('genome')
 e.g.
     Individual ID	Sample ID	    Filenames	                                                                    Type
     Demeter	        sample_id001	sample_id001.filename-R1.fastq.gz,sample_id001.filename-R2.fastq.gz	            WGS
     Demeter	        sample_id001	sample_id001.exome.filename-R1.fastq.gz,sample_id001.exome.filename-R2.fastq.gz	WES
     Apollo	        sample_id002	sample_id002.filename-R1.fastq.gz	                                            WGS
     Apollo	        sample_id002	sample_id002.filename-R2.fastq.gz	                                            WGS
     Athena	        sample_id003	sample_id003.filename-R1.fastq.gz
@@ -154,15 +154,15 @@
 @click.argument('manifests', nargs=-1)
 @run_as_sync
 async def main(
     manifests,
     search_path: List[str],
     project,
     default_sample_type='blood',
-    default_sequence_type='genome',
+    default_sequencing_type='genome',
     default_sequence_technology='short-read',
     default_reference_assembly: str = None,
     confirm=False,
     dry_run=False,
     allow_extra_files_in_search_path=False,
 ):
     """Run script from CLI arguments"""
@@ -172,15 +172,15 @@
     extra_seach_paths = [m for m in manifests if m.startswith('gs://')]
     if extra_seach_paths:
         search_path = list(set(search_path).union(set(extra_seach_paths)))
 
     parser = SampleFileMapParser(
         project=project,
         default_sample_type=default_sample_type,
-        default_sequencing_type=default_sequence_type,
+        default_sequencing_type=default_sequencing_type,
         default_sequencing_technology=default_sequence_technology,
         search_locations=search_path,
         allow_extra_files_in_search_path=allow_extra_files_in_search_path,
         default_reference_assembly_location=default_reference_assembly,
     )
     for manifest in manifests:
         logger.info(f'Importing {manifest}')
```

### Comparing `metamist-6.0.5/metamist/rest.py` & `metamist-6.0.6/metamist/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Sample metadata API
 
     No description provided (generated by Openapi Generator https://github.com/openapitools/openapi-generator)  # noqa: E501
 
-    The version of the OpenAPI document: 6.0.5
+    The version of the OpenAPI document: 6.0.6
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `metamist-6.0.5/metamist.egg-info/PKG-INFO` & `metamist-6.0.6/metamist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metamist
-Version: 6.0.5
+Version: 6.0.6
 Summary: Python API for interacting with the Sample API system
 Home-page: https://github.com/populationgenomics/sample-metadata
 License: MIT
 Keywords: bioinformatics
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `metamist-6.0.5/metamist.egg-info/SOURCES.txt` & `metamist-6.0.6/metamist.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 metamist/api/participant_api.py
 metamist/api/project_api.py
 metamist/api/sample_api.py
 metamist/api/seqr_api.py
 metamist/api/sequencing_group_api.py
 metamist/api/web_api.py
 metamist/apis/__init__.py
+metamist/audit/__init__.py
+metamist/audit/audit_upload_bucket.py
+metamist/audit/audithelper.py
+metamist/audit/delete_sequence_files_from_audit.py
+metamist/audit/generic_auditor.py
 metamist/graphql/__init__.py
 metamist/graphql/schema.graphql
 metamist/model/__init__.py
 metamist/model/analysis.py
 metamist/model/analysis_query_model.py
 metamist/model/analysis_status.py
 metamist/model/analysis_update_model.py
@@ -72,14 +77,15 @@
 metamist/parser/cloudhelper.py
 metamist/parser/generic_metadata_parser.py
 metamist/parser/generic_parser.py
 metamist/parser/sample_file_map_parser.py
 test/test_analysis.py
 test/test_assay.py
 test/test_generate_data.py
+test/test_generic_auditor.py
 test/test_generic_filters.py
 test/test_get_participants.py
 test/test_graphql.py
 test/test_import_individual_metadata.py
 test/test_metamist.py
 test/test_models.py
 test/test_parse_existing_cohort.py
@@ -87,10 +93,11 @@
 test/test_parse_generic_metadata.py
 test/test_parse_ont_processor.py
 test/test_parse_ont_sheet.py
 test/test_pedigree.py
 test/test_sample.py
 test/test_search.py
 test/test_sequencing_groups.py
+test/test_update_participant_family.py
 test/test_upsert.py
 test/test_web.py
 test/testbase.py
```

### Comparing `metamist-6.0.5/setup.py` & `metamist-6.0.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 with open('README.md', encoding='utf-8') as f:
     readme = f.read()
 
 
 setup(
     name=PKG,
     # This tag is automatically updated by bump2version
-    version='6.0.5',
+    version='6.0.6',
     description='Python API for interacting with the Sample API system',
     long_description=readme,
     long_description_content_type='text/markdown',
     url=f'https://github.com/populationgenomics/sample-metadata',
     license='MIT',
     packages=all_packages,
     install_requires=[
```

### Comparing `metamist-6.0.5/test/test_analysis.py` & `metamist-6.0.6/test/test_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
         self.exome_sequencing_group_id = sample.sequencing_groups[self.project_id].id
 
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[self.genome_sequencing_group_id],
-                meta={'sequence_type': 'genome', 'size': 1024},
+                meta={'sequencing_type': 'genome', 'size': 1024},
             )
         )
 
     @run_as_sync
     async def test_add_cram(self):
         """
         Test adding an analysis of type CRAM
@@ -177,15 +177,15 @@
 
         # Add exome cram
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[self.exome_sequencing_group_id],
-                meta={'sequence_type': 'exome', 'size': 3141},
+                meta={'sequencing_type': 'exome', 'size': 3141},
             )
         )
         expected = {
             'project': self.project_id,
             'sequencing_groups': {
                 self.genome_sequencing_group_id: [
                     {
@@ -233,15 +233,15 @@
 
         # Add another genome cram that's newer
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[self.genome_sequencing_group_id],
-                meta={'sequence_type': 'genome', 'size': 11111},
+                meta={'sequencing_type': 'genome', 'size': 11111},
             )
         )
         expected = {
             'project': self.project_id,
             'sequencing_groups': {
                 self.genome_sequencing_group_id: [
                     {
@@ -291,15 +291,15 @@
         )
         sequencing_group_2_id = sample_2.sequencing_groups[0].id
         await self.al.create_analysis(
             AnalysisInternal(
                 type='cram',
                 status=AnalysisStatus.COMPLETED,
                 sequencing_group_ids=[sequencing_group_2_id],
-                meta={'sequence_type': 'genome', 'size': 987654321},
+                meta={'sequencing_type': 'genome', 'size': 987654321},
             )
         )
 
         expected = {
             'project': self.project_id,
             'sequencing_groups': {
                 self.genome_sequencing_group_id: [
```

### Comparing `metamist-6.0.5/test/test_assay.py` & `metamist-6.0.6/test/test_assay.py`

 * *Files 4% similar despite different names*

```diff
@@ -204,45 +204,14 @@
         self.assertEqual(seq1.id, (await self.assaylayer.query(fquery_1))[0].id)
         fquery_2 = AssayFilter(external_id='EXT_SEQ1', project=self.project_id)
         self.assertEqual(seq1.id, (await self.assaylayer.query(fquery_2))[0].id)
         fquery_3 = AssayFilter(external_id='SEQ02', project=self.project_id)
         self.assertEqual(seq2.id, (await self.assaylayer.query(fquery_3))[0].id)
 
     @run_as_sync
-    async def test_get_assays_by_sample_id(self):
-        """Get many assays by sample ID"""
-        seq1 = await self.assaylayer.upsert_assay(
-            AssayUpsertInternal(
-                sample_id=self.sample_id_raw,
-                type='sequencing',
-                meta={**default_sequencing_meta},
-                external_ids={},
-            )
-        )
-        seq2 = await self.assaylayer.upsert_assay(
-            AssayUpsertInternal(
-                sample_id=self.sample_id_raw,
-                type='sequencing',
-                meta={**default_sequencing_meta},
-                external_ids={},
-            )
-        )
-
-        by_type = await self.assaylayer.get_assay_ids_for_sample_ids_by_type(
-            [self.sample_id_raw], check_project_ids=False
-        )
-
-        self.assertIn(self.sample_id_raw, by_type)
-        self.assertEqual(1, len(by_type))
-
-        self.assertSetEqual(
-            {seq1.id, seq2.id}, set(by_type[self.sample_id_raw]['sequencing'])
-        )
-
-    @run_as_sync
     async def test_query(self):
         """Test query_assays in different combinations"""
         sample = await self.slayer.upsert_sample(
             SampleUpsertInternal(
                 external_id='SAM_TEST_QUERY',
                 type='blood',
                 active=True,
@@ -365,15 +334,15 @@
         #     await search_result_to_ids(
         #         external_assay_ids=['SEQ01'], types=[SequenceType.EXOME]
         #     ),
         # )
 
     @run_as_sync
     async def test_update(self):
-        """Test updating a assay, and all fields are updated correctly"""
+        """Test updating an assay, and all fields are updated correctly"""
         # insert
         assay = await self.assaylayer.upsert_assay(
             AssayUpsertInternal(
                 sample_id=self.sample_id_raw,
                 type='sequencing',
                 meta={'a': 1, 'b': 2, **default_sequencing_meta},
                 external_ids={
```

### Comparing `metamist-6.0.5/test/test_generate_data.py` & `metamist-6.0.6/test/test_generate_data.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_generic_filters.py` & `metamist-6.0.6/test/test_generic_filters.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_get_participants.py` & `metamist-6.0.6/test/test_get_participants.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_graphql.py` & `metamist-6.0.6/test/test_graphql.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_import_individual_metadata.py` & `metamist-6.0.6/test/test_import_individual_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_metamist.py` & `metamist-6.0.6/test/test_metamist.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_models.py` & `metamist-6.0.6/test/test_models.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_parse_existing_cohort.py` & `metamist-6.0.6/test/test_parse_existing_cohort.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_parse_file_map.py` & `metamist-6.0.6/test/test_parse_file_map.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_parse_generic_metadata.py` & `metamist-6.0.6/test/test_parse_generic_metadata.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_parse_ont_processor.py` & `metamist-6.0.6/test/test_parse_ont_processor.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_parse_ont_sheet.py` & `metamist-6.0.6/test/test_parse_ont_sheet.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_pedigree.py` & `metamist-6.0.6/test/test_pedigree.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_sample.py` & `metamist-6.0.6/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_search.py` & `metamist-6.0.6/test/test_search.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_sequencing_groups.py` & `metamist-6.0.6/test/test_sequencing_groups.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_upsert.py` & `metamist-6.0.6/test/test_upsert.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/test_web.py` & `metamist-6.0.6/test/test_web.py`

 * *Files identical despite different names*

### Comparing `metamist-6.0.5/test/testbase.py` & `metamist-6.0.6/test/testbase.py`

 * *Files identical despite different names*

