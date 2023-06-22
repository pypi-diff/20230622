# Comparing `tmp/rime_sdk-2.1.0rc5.tar.gz` & `tmp/rime_sdk-2.1.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.1.0rc5.tar", last modified: Fri May 26 20:51:04 2023, max compression
+gzip compressed data, was "rime_sdk-2.1.0rc6.tar", last modified: Thu Jun 22 20:45:59 2023, max compression
```

## Comparing `rime_sdk-2.1.0rc5.tar` & `rime_sdk-2.1.0rc6.tar`

### file list

```diff
@@ -1,493 +1,505 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.588338 rime_sdk-2.1.0rc5/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 20:51:04.588338 rime_sdk-2.1.0rc5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.532338 rime_sdk-2.1.0rc5/rime_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63653 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/data_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.532338 rime_sdk-2.1.0rc5/rime_sdk/data_format_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/data_format_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/data_format_check/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/data_format_check/data_format_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/data_format_check/nlp_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/data_format_check/tabular_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.536338 rime_sdk-2.1.0rc5/rime_sdk/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/rest_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/security_config_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/swagger_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/swagger_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/throttle_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18267 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    61304 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    25145 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.536338 rime_sdk-2.1.0rc5/rime_sdk/swagger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.536338 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/
--rw-r--r--   0 runner    (1001) docker     (123)    47104 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.540338 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30625 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21540 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    64388 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60434 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.588338 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/
--rw-r--r--   0 runner    (1001) docker     (123)    44986 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/tags_name_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    12936 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-26 20:51:00.000000 rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/rime_sdk/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:51:04.532338 rime_sdk-2.1.0rc5/rime_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 20:51:04.000000 rime_sdk-2.1.0rc5/rime_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    32553 2023-05-26 20:51:04.000000 rime_sdk-2.1.0rc5/rime_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:51:04.000000 rime_sdk-2.1.0rc5/rime_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-26 20:51:04.000000 rime_sdk-2.1.0rc5/rime_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-26 20:51:04.000000 rime_sdk-2.1.0rc5/rime_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 20:51:04.000000 rime_sdk-2.1.0rc5/rime_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:51:04.588338 rime_sdk-2.1.0rc5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-26 20:50:23.000000 rime_sdk-2.1.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.247388 rime_sdk-2.1.0rc6/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 20:45:59.243387 rime_sdk-2.1.0rc6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.167385 rime_sdk-2.1.0rc6/rime_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63671 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/data_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.167385 rime_sdk-2.1.0rc6/rime_sdk/data_format_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/data_format_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/data_format_check/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/data_format_check/data_format_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/data_format_check/nlp_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/data_format_check/tabular_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.167385 rime_sdk-2.1.0rc6/rime_sdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15159 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/rest_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/security_config_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9119 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/swagger_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/swagger_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/throttle_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17950 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60764 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25848 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.167385 rime_sdk-2.1.0rc6/rime_sdk/swagger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.167385 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/
+-rw-r--r--   0 runner    (1001) docker     (123)    48757 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.171385 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34984 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25195 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18110 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21540 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26888 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26961 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21630 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29459 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19744 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55813 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57319 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64388 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40185 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25498 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64667 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8286 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.243387 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    46616 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8080 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4205 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5158 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4478 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4422 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17754 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3375 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5408 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11606 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8524 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6750 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9233 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3394 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8541 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3110 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5555 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5859 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4811 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7431 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5746 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/tags_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10280 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12809 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5680 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5790 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13296 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13655 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15198 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13992 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11044 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-06-22 20:45:53.000000 rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/rime_sdk/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:45:59.167385 rime_sdk-2.1.0rc6/rime_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 20:45:59.000000 rime_sdk-2.1.0rc6/rime_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33606 2023-06-22 20:45:59.000000 rime_sdk-2.1.0rc6/rime_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:45:59.000000 rime_sdk-2.1.0rc6/rime_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 20:45:59.000000 rime_sdk-2.1.0rc6/rime_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-22 20:45:59.000000 rime_sdk-2.1.0rc6/rime_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-22 20:45:59.000000 rime_sdk-2.1.0rc6/rime_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:45:59.247388 rime_sdk-2.1.0rc6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-22 20:45:11.000000 rime_sdk-2.1.0rc6/setup.py
```

### Comparing `rime_sdk-2.1.0rc5/LICENSE` & `rime_sdk-2.1.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/PKG-INFO` & `rime_sdk-2.1.0rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.1.0rc5
+Version: 2.1.0rc6
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.1.0rc5/README.md` & `rime_sdk-2.1.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/__init__.py` & `rime_sdk-2.1.0rc6/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/client.py` & `rime_sdk-2.1.0rc6/rime_sdk/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from rime_sdk.internal.throttle_queue import ThrottleQueue
 from rime_sdk.job import BaseJob, ContinuousTestJob, FileScanJob, ImageBuilderJob, Job
 from rime_sdk.project import Project
 from rime_sdk.swagger import swagger_client
 from rime_sdk.swagger.swagger_client import ApiClient
 from rime_sdk.swagger.swagger_client.models import (
     ConfigvalidatorConfigTypeBody,
+    GenerativestresstestsProjectIdUuidBody,
     ListImagesRequestPipLibraryFilter,
     ManagedImagePackageRequirement,
     ManagedImagePackageType,
     ManagedImagePipRequirement,
     ProjectCreateProjectRequest,
     RimeActorRole,
     RimeCreateImageRequest,
@@ -192,21 +193,21 @@
             )
         elif limit_status == RimeLimitStatusStatus.ERROR:
             message = (
                 "Your license has expired. Contact the Robust "
                 "Intelligence team to upgrade your license."
             )
             grace_period_end = datetime.fromtimestamp(
-                rime_info_response.grace_period_end_time.seconds
+                rime_info_response.grace_period_end_time.timestamp()
             ).date()
             if date.today() > grace_period_end:
                 # if grace period has ended throw an error
                 raise ValueError(message)
             else:
-                print(message)
+                print(f"{message} You have until {grace_period_end} to upgrade.")
         elif limit_status == RimeLimitStatusStatus.OK:
             pass
         else:
             raise ValueError(f"Unexpected status value: '{limit_status}'")
 
     def _check_stress_test_limit(self) -> None:
         """Check if creating another Stress Test would be within license limits.
@@ -982,15 +983,15 @@
             job: RimeJobMetadata = api.model_testing_start_stress_test(
                 body=req,
                 project_id_uuid=project_id,
             ).job
         return Job(self._api_client, job.job_id)
 
     def start_generative_stress_test(
-        self, test_run_config: dict, project_id: str, **exp_fields: Dict[str, object]
+        self, test_run_config: dict, project_id: str
     ) -> Job:
         """Start a Generative Stress Testing run.
 
         Args:
             test_run_config: dict
                 Configuration for the test to be run, which specifies unique ids to
                 locate the model and datasets to be used for the test.
@@ -1031,26 +1032,25 @@
 
            job = rime_client.start_generative_stress_test_job(
               test_run_config=config, project_id="123-456-789"
            )
         """
         self._validate_config(test_run_config, project_id)
 
-        cv_api = swagger_client.ConfigValidatorApi(self._api_client)
+        # cv_api = swagger_client.ConfigValidatorApi(self._api_client)
         with RESTErrorHandler():
             # TODO (GAI-128): Use GAI config validator instead
-            validate_body = ConfigvalidatorConfigTypeBody(
-                config_json=json.dumps(test_run_config),
-            )
-            cv_api.config_validator_validate_test_config(
-                config_type="CONFIG_TYPE_TEST_RUN", body=validate_body
-            )
-            req = StresstestsProjectIdUuidBody(
+            # validate_body = ConfigvalidatorConfigTypeBody(
+            #     config_json=json.dumps(test_run_config),
+            # )
+            # cv_api.config_validator_validate_test_config(
+            #     config_type="CONFIG_TYPE_TEST_RUN", body=validate_body
+            # )
+            req = GenerativestresstestsProjectIdUuidBody(
                 test_run_config=test_run_config,
-                experimental_fields=exp_fields if exp_fields else None,
             )
             Client._throttler.throttle(
                 throttling_msg="Your request is throttled to limit # of model tests."
             )
             api = swagger_client.ModelTestingApi(self._api_client)
             job: RimeJobMetadata = api.model_testing_start_generative_stress_test(
                 body=req,
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/data_collector.py` & `rime_sdk-2.1.0rc6/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/data_format_check/cli.py` & `rime_sdk-2.1.0rc6/rime_sdk/data_format_check/cli.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/data_format_check/data_format_checker.py` & `rime_sdk-2.1.0rc6/rime_sdk/data_format_check/data_format_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/data_format_check/nlp_checker.py` & `rime_sdk-2.1.0rc6/rime_sdk/data_format_check/nlp_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/data_format_check/tabular_checker.py` & `rime_sdk-2.1.0rc6/rime_sdk/data_format_check/tabular_checker.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/detection_event.py` & `rime_sdk-2.1.0rc6/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/firewall.py` & `rime_sdk-2.1.0rc6/rime_sdk/firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/image_builder.py` & `rime_sdk-2.1.0rc6/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/config_parser.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,42 +5,42 @@
 from copy import deepcopy
 from typing import Any, Callable, Optional, Set, Tuple, Union, cast
 
 from rime_sdk.swagger.swagger_client.models import (
     DataParamsFeatureIntersection,
     DataParamsRankingInfo,
     RegistryConnectionInfo,
+    RegistryDatabricksInfo,
     RegistryDataCollectorInfo,
     RegistryDataFileInfo,
     RegistryDataInfo,
     RegistryDataLoadingInfo,
     RegistryDataParams,
-    RegistryDeltaLakeInfo,
     RegistryHuggingFaceDataInfo,
     RegistryHuggingFaceModelInfo,
     RegistryModelInfo,
     RegistryModelPathInfo,
     RegistryPredictionParams,
     RegistryPredInfo,
     RimeUUID,
 )
 
 DEFAULT_DO_SAMPLING = True
 CONNECTION_INFO_TYPE_SWAGGER = Union[
     RegistryDataFileInfo,
     RegistryDataLoadingInfo,
     RegistryDataCollectorInfo,
-    RegistryDeltaLakeInfo,
+    RegistryDatabricksInfo,
     RegistryHuggingFaceDataInfo,
 ]
 VALID_CONNECTION_TYPES = [
+    "databricks",
     "data_file",
     "data_loading",
     "data_collector",
-    "delta_lake",
     "hugging_face",
 ]
 
 
 def validate_types(func: Callable) -> Callable:
     """Wrap given function with a decorator that validates types of arguments."""
 
@@ -132,15 +132,18 @@
 @validate_types
 def _mutate_data_file_conn_info_to_swag(
     connection_info: dict, path: str
 ) -> RegistryDataFileInfo:
     """Process data file connection info into a connection swagger."""
     required_keys = {"path"}
     _check_required_keys_exist(connection_info, required_keys, path)
-    return RegistryDataFileInfo(path=connection_info.pop("path"))
+    return RegistryDataFileInfo(
+        path=connection_info.pop("path"),
+        data_type=connection_info.pop("data_type", None),
+    )
 
 
 @validate_types
 def _mutate_data_loader_conn_info_to_swag(
     connection_info: dict, path: str
 ) -> RegistryDataLoadingInfo:
     """Process data loader connection info into a connection swagger."""
@@ -181,19 +184,19 @@
     data_stream_id = RimeUUID(connection_info.pop("data_stream_id"))
     return RegistryDataCollectorInfo(data_stream_id=data_stream_id)
 
 
 @validate_types
 def _mutate_delta_lake_conn_info_to_swag(
     connection_info: dict, path: str
-) -> RegistryDeltaLakeInfo:
+) -> RegistryDatabricksInfo:
     """Process delta lake connection info into a connection info swagger."""
     required_keys = {"table_name"}
     _check_required_keys_exist(connection_info, required_keys, path)
-    return RegistryDeltaLakeInfo(table_name=connection_info.pop("table_name"))
+    return RegistryDatabricksInfo(table_name=connection_info.pop("table_name"))
 
 
 @validate_types
 def _mutate_huggingface_conn_info_to_swag(
     connection_info: dict, path: str
 ) -> RegistryHuggingFaceDataInfo:
     """Process huggingface connection info into a connection info swagger."""
@@ -225,15 +228,15 @@
     """Process config connection info into a connection swagger and its swagger key."""
     _config = deepcopy(connection_info)
     _config = _config.pop(config_type)
     connection_loader_map = {
         "data_file": _mutate_data_file_conn_info_to_swag,
         "data_loading": _mutate_data_loader_conn_info_to_swag,
         "data_collector": _mutate_data_collector_conn_info_to_swag,
-        "delta_lake": _mutate_delta_lake_conn_info_to_swag,
+        "databricks": _mutate_delta_lake_conn_info_to_swag,
         "hugging_face": _mutate_huggingface_conn_info_to_swag,
     }
     _path = f"{path}.{config_type}"
     swagger = connection_loader_map[config_type](_config, _path)
     if _config:
         expected_field_names = getattr(swagger, "swagger_types", [])
         raise ValueError(
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/constants.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/decorators.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/file_upload.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/security_config_parser.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/security_config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/internal/utils.py` & `rime_sdk-2.1.0rc6/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/job.py` & `rime_sdk-2.1.0rc6/rime_sdk/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,17 +461,7 @@
 
     _job_type = RimeJobType.FILE_SCAN
 
     def _get_progress(self, job: RimeJobMetadata) -> Optional[str]:
         """Pretty print the progress of the test run."""
         # TODO: find a good way to pretty print the progress of a FileScanJob
         return None
-
-
-class CrossPlaneTask(BaseJob):
-    """This object provides an interface for monitoring a CrossPlaneTasks in the RI platform."""
-
-    _job_type = RimeJobType.CROSS_PLANE_TASK
-
-    def _get_progress(self, job: RimeJobMetadata) -> Optional[str]:
-        """Pretty print the progress of the job."""
-        return None
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/monitor.py` & `rime_sdk-2.1.0rc6/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/project.py` & `rime_sdk-2.1.0rc6/rime_sdk/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Library defining the interface to a Project."""
 import json
-from datetime import datetime, timedelta
+from datetime import timedelta
 from http import HTTPStatus
 from typing import Any, Dict, Iterator, List, NamedTuple, Optional
 
-from deprecated import deprecated
 from google.protobuf.field_mask_pb2 import FieldMask
 from google.protobuf.json_format import MessageToDict
 
 from rime_sdk.data_collector import DataCollector
 from rime_sdk.firewall import Firewall
 from rime_sdk.internal.config_parser import (
     _get_individual_tests_config_swagger,
@@ -19,15 +18,15 @@
 from rime_sdk.internal.rest_error_handler import RESTErrorHandler
 from rime_sdk.internal.swagger_utils import parse_str_to_uuid, timedelta_to_rest
 from rime_sdk.internal.utils import (
     convert_dict_to_html,
     get_swagger_field_mask,
     make_link,
 )
-from rime_sdk.job import CrossPlaneTask, Job
+from rime_sdk.job import Job
 from rime_sdk.registry import Registry
 from rime_sdk.swagger import swagger_client
 from rime_sdk.swagger.swagger_client import (
     ApiClient,
     CreateFirewallRequestScheduledCTParameters,
     RimeCreateFirewallRequest,
     RimeUUID,
@@ -48,23 +47,14 @@
     RimeJobType,
     RimeLicenseLimit,
     RimeLimitStatusStatus,
     RimeListNotificationsResponse,
     SchemanotificationConfig,
     StatedbJobStatus,
 )
-from rime_sdk.swagger.swagger_client.models.rime_get_foo_task_status_response import (
-    RimeGetFooTaskStatusResponse,
-)
-from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_request import (
-    RimeStartFooTaskRequest,
-)
-from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_response import (
-    RimeStartFooTaskResponse,
-)
 from rime_sdk.swagger.swagger_client.models.testrun_profiling_config import (
     TestrunProfilingConfig,
 )
 from rime_sdk.swagger.swagger_client.rest import ApiException
 from rime_sdk.test_run import TestRun
 
 NOTIFICATION_TYPE_JOB_ACTION_STR: str = "Job_Action"
@@ -200,47 +190,14 @@
                 A ``Project`` object.
         """
         api = swagger_client.ProjectServiceApi(self._api_client)
         with RESTErrorHandler():
             response = api.project_service_get_project(self._project_id)
             return response.project.project
 
-    @deprecated
-    def foo_example_cross_plane_task(
-        self, should_fail: bool = False
-    ) -> Optional[datetime]:
-        """Do the Foo toy example for the given project.
-
-        This makes a CrossPlane call to the DataPlane and returns the current
-        time on the agent side.
-        This may fail at certain times :)
-        """
-        # TODO(RAT-1738): remove this method, only for internal testing.
-        api = swagger_client.FooXPInterfaceApi(self._api_client)
-        with RESTErrorHandler():
-            req = RimeStartFooTaskRequest(
-                project_id=RimeUUID(self._project_id), req={"should_fail": should_fail}
-            )
-            res: RimeStartFooTaskResponse = api.foo_xp_interface_start_foo_task(req)
-            job_id: str = res.job_id.uuid
-            job = CrossPlaneTask(self._api_client, job_id)
-            job_res = job.get_status(
-                verbose=False, wait_until_finish=True, poll_rate_sec=1
-            )
-            final_status = job_res.get("status")
-            if final_status == StatedbJobStatus.SUCCEEDED:
-                get_res: RimeGetFooTaskStatusResponse = (
-                    api.foo_xp_interface_get_foo_task_status(job_id)
-                )
-                return get_res.res.receive_time
-            elif final_status == StatedbJobStatus.FAILED:
-                raise ValueError(f"Job failed: {job_res.get('error_msg')}")
-
-            return None
-
     @property
     def info(self) -> ProjectInfo:
         """Return description, use case and ethical consideration of the Project."""
         project = self._get_project()
         return ProjectInfo(
             self._project_id,
             project.name,
@@ -840,14 +797,15 @@
         self,
         name: str,
         data_config: dict,
         integration_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         ct_info: Optional[dict] = None,
+        skip_validation: Optional[bool] = False,
     ) -> str:
         """Register a new dataset in this Project.
 
         Args:
             name: str
                 The chosen name of the dataset.
             data_config: dict
@@ -860,14 +818,16 @@
                 An optional list of tags to associate with the dataset.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the dataset.
             ct_info: Optional[dict] = None,
                 An optional dictionary that contains the CT info.
                 The CT info must match the API specification of the `ct_info`
                 field in the `RegisterDataset` request.
+            skip_validation: Optional[bool] = False,
+                When set to True, the dataset will not be validated.
 
         Returns:
             str:
                 The ID of the newly registered dataset.
 
         Raises:
             ValueError
@@ -890,37 +850,41 @@
             self.project_id,
             name,
             data_config,
             integration_id=integration_id,
             tags=tags,
             metadata=metadata,
             ct_info=ct_info,
+            skip_validation=skip_validation,
         )
 
     def register_dataset_from_file(
         self,
         name: str,
         remote_path: str,
         data_params: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         ct_info: Optional[dict] = None,
+        skip_validation: Optional[bool] = False,
     ) -> str:
         """Register a new dataset in this Project.
 
         Args:
             name: str
                 The chosen name of the dataset.
             remote_path: str
                 The path to the dataset artifact.
 
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the dataset.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the dataset.
+            skip_validation: Optional[bool] = False,
+                When set to True, the dataset will not be validated.
 
         Returns:
             str:
                 The ID of the newly registered dataset.
 
         Raises:
             ValueError
@@ -935,24 +899,26 @@
         return self._registry.register_dataset(
             self.project_id,
             name,
             data_config,
             tags=tags,
             metadata=metadata,
             ct_info=ct_info,
+            skip_validation=skip_validation,
         )
 
     def register_model(
         self,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
         integration_id: Optional[str] = None,
+        skip_validation: Optional[bool] = False,
     ) -> str:
         """Register a new model in this Project.
 
         Args:
             name: str
                 The chosen name of the model.
             model_config: Optional[dict] = None,
@@ -965,14 +931,16 @@
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
             integration_id: Optional[str] = None,
                 Provide the integration ID for models that require an
                 integration for access.
+            skip_validation: Optional[bool] = False,
+                When set to True, the model will not be validated.
 
         Returns:
             str:
                 The ID of the newly registered model.
 
         Raises:
             ValueError
@@ -1003,24 +971,26 @@
             self.project_id,
             name,
             model_config=model_config,
             tags=tags,
             metadata=metadata,
             external_id=external_id,
             integration_id=integration_id,
+            skip_validation=skip_validation,
         )
 
     def register_model_from_path(
         self,
         name: str,
         remote_path: str,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
         integration_id: Optional[str] = None,
+        skip_validation: Optional[bool] = False,
     ) -> str:
         """Register a new model in this Project.
 
         Args:
             name: str
                 The chosen name of the model.
             remote_path: str
@@ -1030,14 +1000,16 @@
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
             integration_id: Optional[str] = None,
                 Provide the integration ID for models that require an
                 integration for access.
+            skip_validation: Optional[bool] = False,
+                When set to True, the model will not be validated.
 
         Returns:
             str:
                 The ID of the newly registered model.
 
         Raises:
             ValueError
@@ -1057,24 +1029,26 @@
             self.project_id,
             name,
             model_config,
             tags=tags,
             metadata=metadata,
             external_id=external_id,
             integration_id=integration_id,
+            skip_validation=skip_validation,
         )
 
     def register_predictions(
         self,
         dataset_id: str,
         model_id: str,
         pred_config: dict,
         integration_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
+        skip_validation: Optional[bool] = False,
     ) -> None:
         """Register a new prediction corresponding to a model and a dataset.
 
         Args:
             dataset_id: str,
                 The ID of the dataset used to generate the predictions.
             model_id: str,
@@ -1086,14 +1060,16 @@
             integration_id: Optional[str] = None,
                 Provide the integration ID for predictions that require an
                 integration to use.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the predictions.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the predictions.
+            skip_validation: Optional[bool] = False,
+                When set to True, the predictions will not be validated.
 
         Returns:
             None
 
         Raises:
             ValueError
                 This error is generated when the request to the Registry
@@ -1103,15 +1079,15 @@
             .. code-block:: python
 
                 project.register_predictions(
                     dataset_id=DATASET_ID,
                     model_id=MODEL_ID,
                     pred_config={
                         "connection_info": {
-                            "delta_lake": {
+                            "databricks": {
                                 # Unix timestamp equivalent to 02/08/2023
                                 "start_time": 1675922943,
                                 # Unix timestamp equivalent to 03/08/2023
                                 "end_time": 1678342145,
                                 "table_name": TABLE_NAME,
                                 "time_col": TIME_COL,
                             },
@@ -1126,25 +1102,27 @@
             self.project_id,
             dataset_id,
             model_id,
             pred_config,
             integration_id=integration_id,
             tags=tags,
             metadata=metadata,
+            skip_validation=skip_validation,
         )
 
     def register_predictions_from_file(
         self,
         dataset_id: str,
         model_id: str,
         remote_path: str,
         pred_params: Optional[dict] = None,
         integration_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
+        skip_validation: Optional[bool] = False,
     ) -> None:
         """Register a new set of predictions for a model on a dataset.
 
         Args:
             dataset_id: str,
                 The ID of the dataset used to generate the predictions.
             model_id: str,
@@ -1156,14 +1134,16 @@
             integration_id: Optional[str] = None,
                 Provide the integration ID for predictions that require an
                 integration to use.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the predictions.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the predictions.
+            skip_validation: Optional[bool] = False,
+                When set to True, the predictions will not be validated.
 
         Returns:
             None
 
         Raises:
             ValueError
                 This error is generated when the request to the Registry
@@ -1187,14 +1167,15 @@
             self.project_id,
             dataset_id,
             model_id,
             pred_config,
             integration_id=integration_id,
             tags=tags,
             metadata=metadata,
+            skip_validation=skip_validation,
         )
 
     def list_datasets(self) -> Iterator[Dict]:
         """Return a list of datasets registered in this Project.
 
         Returns:
             Iterator[Dict]:
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/registry.py` & `rime_sdk-2.1.0rc6/rime_sdk/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         project_id: str,
         name: str,
         data_config: dict,
         integration_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         ct_info: Optional[dict] = None,
+        skip_validation: Optional[bool] = False,
     ) -> str:
         """Register a new dataset in a Project.
 
         Args:
             project_id: str
                 The ID of the Project in which to register the dataset.
             name: str
@@ -76,14 +77,16 @@
                 An optional list of tags to associate with the dataset.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the dataset.
             ct_info: Optional[dict] = None,
                 An optional dictionary that contains the CT info.
                 The CT info must match the API specification of the `ct_info`
                 field in the `RegisterDataset` request.
+            skip_validation: Optional[bool] = False,
+                An optional boolean that indicates whether to skip validation.
 
         Returns:
             str:
                 The ID of the newly registered dataset.
 
         Raises:
             ValueError
@@ -100,15 +103,18 @@
                         "data_params": {"label_col": LABEL_COL},
                     },
                     integration_id=INTEGRATION_ID,
                 )
         """
         data_info_swagger = convert_single_data_info_to_swagger(data_config)
         req = ProjectIdUuidDatasetBody(
-            project_id=RimeUUID(uuid=project_id), name=name, data_info=data_info_swagger
+            project_id=RimeUUID(uuid=project_id),
+            name=name,
+            data_info=data_info_swagger,
+            skip_validation=skip_validation,
         )
 
         metadata_str: Optional[str] = None
         if metadata is not None:
             metadata_str = json.dumps(metadata)
         if tags is not None or metadata_str is not None:
             req.metadata = RegistryMetadata(tags=tags, extra_info=metadata_str)
@@ -140,14 +146,15 @@
         project_id: str,
         name: str,
         model_config: Optional[dict] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
         external_id: Optional[str] = None,
         integration_id: Optional[str] = None,
+        skip_validation: Optional[bool] = False,
     ) -> str:
         """Register a new model in a Project.
 
         Args:
             project_id: str
                 The ID of the Project in which to register the model.
             name: str
@@ -162,14 +169,16 @@
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the model.
             external_id: Optional[str] = None,
                 An optional external ID that can be used to identify the model.
             integration_id: Optional[str] = None,
                 Provide the integration ID for models that require an
                 integration for access.
+            skip_validation: Optional[bool] = False,
+                An optional boolean that indicates whether to skip validation.
 
         Returns:
             str:
                 The ID of the newly registered model.
 
         Raises:
             ValueError
@@ -195,14 +204,15 @@
                     metadata={KEY: VALUE},
                     external_id=EXTERNAL_ID,
                 )
         """
         req = ProjectIdUuidModelBody(
             project_id=RimeUUID(uuid=project_id),
             name=name,
+            skip_validation=skip_validation,
         )
 
         if model_config is not None:
             # When the `model_path` key is provided to the dictionary, the value
             # must be a dictionary whose `path` value points to a python
             # file that holds a `predict_dict` or `predict_df` function.
             # When the `model_loading` key is provided to the dictionary, the value
@@ -243,14 +253,15 @@
         project_id: str,
         dataset_id: str,
         model_id: str,
         pred_config: dict,
         integration_id: Optional[str] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[dict] = None,
+        skip_validation: Optional[bool] = False,
     ) -> None:
         """Register a new set of predictions for a model on a dataset.
 
         Args:
             project_id: str
                 The ID of the Project to which the models belong.
             dataset_id: str,
@@ -264,14 +275,16 @@
             integration_id: Optional[str] = None,
                 Provide the integration ID for predictions that require an
                 integration to use.
             tags: Optional[List[str]] = None,
                 An optional list of tags to associate with the predictions.
             metadata: Optional[dict] = None,
                 An optional dictionary of metadata to associate with the predictions.
+            skip_validation: Optional[bool] = False,
+                An optional boolean that indicates whether to skip validation.
 
         Returns:
             None
 
         Raises:
             ValueError
                 This error is generated when the request to the Registry
@@ -281,15 +294,15 @@
             .. code-block:: python
 
                 registry.register_predictions(
                     dataset_id=DATASET_ID,
                     model_id=MODEL_ID,
                     pred_config={
                         "connection_info": {
-                            "delta_lake": {
+                            "databricks": {
                                 # Unix timestamp equivalent to 02/08/2023
                                 "start_time": 1675922943,
                                 # Unix timestamp equivalent to 03/08/2023
                                 "end_time": 1678342145,
                                 "table_name": TABLE_NAME,
                                 "time_col": TIME_COL,
                             },
@@ -302,14 +315,15 @@
         """
         pred_info_swagger = convert_single_pred_info_to_swagger(pred_config)
 
         req = DatasetIdPredictionBody(
             project_id=RimeUUID(uuid=project_id),
             model_id=RimeUUID(uuid=model_id),
             pred_info=pred_info_swagger,
+            skip_validation=skip_validation,
         )
 
         metadata_str: Optional[str] = None
         if metadata is not None:
             metadata_str = json.dumps(metadata)
         if tags is not None or metadata_str is not None:
             req.metadata = RegistryMetadata(tags=tags, extra_info=metadata_str)
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,63 +1,38 @@
 # coding: utf-8
 
 # flake8: noqa
-
 """
     Robust Intelligence REST API
 
     API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import apis into sdk package
-from rime_sdk.swagger.swagger_client.api.agent_manager_api import AgentManagerApi
-from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
-from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
-from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
-from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
-from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
-from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
-from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
-from rime_sdk.swagger.swagger_client.api.foo_xp_interface_api import FooXPInterfaceApi
-from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
-from rime_sdk.swagger.swagger_client.api.integration_service_api import IntegrationServiceApi
-from rime_sdk.swagger.swagger_client.api.job_reader_api import JobReaderApi
-from rime_sdk.swagger.swagger_client.api.model_card_service_api import ModelCardServiceApi
-from rime_sdk.swagger.swagger_client.api.model_testing_api import ModelTestingApi
-from rime_sdk.swagger.swagger_client.api.monitor_service_api import MonitorServiceApi
-from rime_sdk.swagger.swagger_client.api.notification_setting_api import NotificationSettingApi
-from rime_sdk.swagger.swagger_client.api.project_service_api import ProjectServiceApi
-from rime_sdk.swagger.swagger_client.api.rime_info_api import RIMEInfoApi
-from rime_sdk.swagger.swagger_client.api.registry_service_api import RegistryServiceApi
-from rime_sdk.swagger.swagger_client.api.results_reader_api import ResultsReaderApi
-from rime_sdk.swagger.swagger_client.api.user_api import UserApi
-from rime_sdk.swagger.swagger_client.api.validation_service_api import ValidationServiceApi
-from rime_sdk.swagger.swagger_client.api.workspace_service_api import WorkspaceServiceApi
-# import ApiClient
-from rime_sdk.swagger.swagger_client.api_client import ApiClient
-from rime_sdk.swagger.swagger_client.configuration import Configuration
-# import models into sdk package
+# import models into model package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_azure_config import CreateAgentRequestAzureConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
+from rime_sdk.swagger.swagger_client.models.customermanagedkey_customer_managed_key_config import CustomermanagedkeyCustomerManagedKeyConfig
+from rime_sdk.swagger.swagger_client.models.customermanagedkey_key_provider import CustomermanagedkeyKeyProvider
+from rime_sdk.swagger.swagger_client.models.customermanagedkey_key_status import CustomermanagedkeyKeyStatus
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
 from rime_sdk.swagger.swagger_client.models.data_data_stream_id_uuid_body import DataDataStreamIdUuidBody
 from rime_sdk.swagger.swagger_client.models.data_params_feature_intersection import DataParamsFeatureIntersection
 from rime_sdk.swagger.swagger_client.models.data_params_ranking_info import DataParamsRankingInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_column_type_info import DataProfilingColumnTypeInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_feature_relationship_info import DataProfilingFeatureRelationshipInfo
 from rime_sdk.swagger.swagger_client.models.datacollector_datapoint import DatacollectorDatapoint
@@ -84,20 +59,17 @@
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
-from rime_sdk.swagger.swagger_client.models.fooexample_foo_request import FooexampleFooRequest
-from rime_sdk.swagger.swagger_client.models.fooexample_foo_response import FooexampleFooResponse
 from rime_sdk.swagger.swagger_client.models.generativestresstests_project_id_uuid_body import GenerativestresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
-from rime_sdk.swagger.swagger_client.models.integration_integration import IntegrationIntegration
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
 from rime_sdk.swagger.swagger_client.models.integrations_integration_id_uuid_body import IntegrationsIntegrationIdUuidBody
 from rime_sdk.swagger.swagger_client.models.job_data_continuous_incremental_test import JobDataContinuousIncrementalTest
 from rime_sdk.swagger.swagger_client.models.job_data_stress_test import JobDataStressTest
@@ -175,15 +147,16 @@
 from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
 from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
-from rime_sdk.swagger.swagger_client.models.registry_delta_lake_info import RegistryDeltaLakeInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
+from rime_sdk.swagger.swagger_client.models.registry_databricks_info import RegistryDatabricksInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
 from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
 from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
 from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
@@ -205,14 +178,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_job_progress import RimeContinuousTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_run_progress import RimeContinuousTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_request import RimeCreateAPITokenRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_response import RimeCreateAPITokenResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_request import RimeCreateAgentRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_response import RimeCreateAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_custom_monitor_response import RimeCreateCustomMonitorResponse
+from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_request import RimeCreateCustomerManagedKeyRequest
+from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_response import RimeCreateCustomerManagedKeyResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_request import RimeCreateFirewallRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_response import RimeCreateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_image_request import RimeCreateImageRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_image_response import RimeCreateImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_request import RimeCreateIntegrationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_response import RimeCreateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_request import RimeCreateModelCardRequest
@@ -239,39 +214,42 @@
 from rime_sdk.swagger.swagger_client.models.rime_ensure_image_existence_response import RimeEnsureImageExistenceResponse
 from rime_sdk.swagger.swagger_client.models.rime_failing_row import RimeFailingRow
 from rime_sdk.swagger.swagger_client.models.rime_failing_rows_result import RimeFailingRowsResult
 from rime_sdk.swagger.swagger_client.models.rime_feature_flags import RimeFeatureFlags
 from rime_sdk.swagger.swagger_client.models.rime_feature_type import RimeFeatureType
 from rime_sdk.swagger.swagger_client.models.rime_float_list import RimeFloatList
 from rime_sdk.swagger.swagger_client.models.rime_get_agent_response import RimeGetAgentResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_customer_managed_key_response import RimeGetCustomerManagedKeyResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_datapoints_response import RimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_response import RimeGetDatasetFileUploadURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_response import RimeGetDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_enabled_feature_response import RimeGetEnabledFeatureResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flag_jwt_response import RimeGetFeatureFlagJwtResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flags_response import RimeGetFeatureFlagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_firewall_response import RimeGetFirewallResponse
-from rime_sdk.swagger.swagger_client.models.rime_get_foo_task_status_response import RimeGetFooTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_image_response import RimeGetImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_integration_response import RimeGetIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_job_response import RimeGetJobResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_key_status_response import RimeGetKeyStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_latest_logs_response import RimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_limit_status_response import RimeGetLimitStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_card_response import RimeGetModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_directory_upload_urls_response import RimeGetModelDirectoryUploadURLsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_response import RimeGetModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_monitor_result_response import RimeGetMonitorResultResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_prediction_set_response import RimeGetPredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_predictions_response import RimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_project_id_response import RimeGetProjectIDResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_rime_info_response import RimeGetRIMEInfoResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_test_run_id_response import RimeGetTestRunIDResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_url_response import RimeGetURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_user_response import RimeGetUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_validate_dataset_task_status_response import RimeGetValidateDatasetTaskStatusResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_validate_model_task_status_response import RimeGetValidateModelTaskStatusResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_validate_predictions_task_status_response import RimeGetValidatePredictionsTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_workspace_response import RimeGetWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_heartbeat_response import RimeHeartbeatResponse
 from rime_sdk.swagger.swagger_client.models.rime_image_reference import RimeImageReference
 from rime_sdk.swagger.swagger_client.models.rime_int_list import RimeIntList
 from rime_sdk.swagger.swagger_client.models.rime_integration_info import RimeIntegrationInfo
 from rime_sdk.swagger.swagger_client.models.rime_job_data import RimeJobData
 from rime_sdk.swagger.swagger_client.models.rime_job_metadata import RimeJobMetadata
@@ -296,14 +274,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_response import RimeListJobsForProjectResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_metric_identifiers_response import RimeListMetricIdentifiersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_model_cards_response import RimeListModelCardsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_models_response import RimeListModelsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_monitors_response import RimeListMonitorsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_notifications_response import RimeListNotificationsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_prediction_sets_response import RimeListPredictionSetsResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_project_tags_in_workspace_response import RimeListProjectTagsInWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_uploaded_file_urls_response import RimeListUploadedFileURLsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_of_workspace_response import RimeListUsersOfWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_request_query import RimeListUsersRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_users_response import RimeListUsersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspace_integrations_response import RimeListWorkspaceIntegrationsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspace_tags_response import RimeListWorkspaceTagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspaces_request_query import RimeListWorkspacesRequestQuery
@@ -318,34 +297,37 @@
 from rime_sdk.swagger.swagger_client.models.rime_named_double import RimeNamedDouble
 from rime_sdk.swagger.swagger_client.models.rime_order import RimeOrder
 from rime_sdk.swagger.swagger_client.models.rime_parent_role_subject_role_pair import RimeParentRoleSubjectRolePair
 from rime_sdk.swagger.swagger_client.models.rime_ri_email_recipient import RimeRIEmailRecipient
 from rime_sdk.swagger.swagger_client.models.rime_ri_plan import RimeRIPlan
 from rime_sdk.swagger.swagger_client.models.rime_register_data_stream_response import RimeRegisterDataStreamResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_dataset_response import RimeRegisterDatasetResponse
+from rime_sdk.swagger.swagger_client.models.rime_register_external_agent_request import RimeRegisterExternalAgentRequest
 from rime_sdk.swagger.swagger_client.models.rime_register_internal_agent_response import RimeRegisterInternalAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_model_response import RimeRegisterModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_prediction_set_response import RimeRegisterPredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_remove_user_from_workspace_response import RimeRemoveUserFromWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_reset_password_response import RimeResetPasswordResponse
 from rime_sdk.swagger.swagger_client.models.rime_resolve_detection_event_response import RimeResolveDetectionEventResponse
 from rime_sdk.swagger.swagger_client.models.rime_safe_url import RimeSafeURL
 from rime_sdk.swagger.swagger_client.models.rime_send_ri_email_response import RimeSendRIEmailResponse
 from rime_sdk.swagger.swagger_client.models.rime_severity import RimeSeverity
 from rime_sdk.swagger.swagger_client.models.rime_severity_counts import RimeSeverityCounts
 from rime_sdk.swagger.swagger_client.models.rime_sort_spec import RimeSortSpec
 from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_response import RimeStartContinuousTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_request import RimeStartFileScanRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_response import RimeStartFileScanResponse
-from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_request import RimeStartFooTaskRequest
-from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_response import RimeStartFooTaskResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_generative_stress_test_response import RimeStartGenerativeStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_stress_test_response import RimeStartStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_validate_dataset_task_request import RimeStartValidateDatasetTaskRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_validate_dataset_task_response import RimeStartValidateDatasetTaskResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_model_task_request import RimeStartValidateModelTaskRequest
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_model_task_response import RimeStartValidateModelTaskResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_predictions_task_request import RimeStartValidatePredictionsTaskRequest
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_predictions_task_response import RimeStartValidatePredictionsTaskResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_datapoints_response import RimeStoreDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_request_prediction import RimeStorePredictionsRequestPrediction
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_response import RimeStorePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.rime_str_list import RimeStrList
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
 from rime_sdk.swagger.swagger_client.models.rime_suggestion import RimeSuggestion
@@ -378,14 +360,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_user_detail_with_role import RimeUserDetailWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_role import RimeUserRole
 from rime_sdk.swagger.swagger_client.models.rime_user_with_role import RimeUserWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_write_mask import RimeUserWriteMask
 from rime_sdk.swagger.swagger_client.models.rime_validate_test_config_response import RimeValidateTestConfigResponse
 from rime_sdk.swagger.swagger_client.models.rime_workspace import RimeWorkspace
 from rime_sdk.swagger.swagger_client.models.rime_workspace_write_mask import RimeWorkspaceWriteMask
+from rime_sdk.swagger.swagger_client.models.rischemaintegration_integration import RischemaintegrationIntegration
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_category_type import RiskscoreRiskCategoryType
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_score import RiskscoreRiskScore
 from rime_sdk.swagger.swagger_client.models.role_users_body import RoleUsersBody
 from rime_sdk.swagger.swagger_client.models.role_workspace_body import RoleWorkspaceBody
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image import RuntimeinfoCustomImage
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
@@ -447,12 +430,13 @@
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body1 import UsersUserUserIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.v1betaintegrationsintegration_id_uuid_integration import V1betaintegrationsintegrationIdUuidIntegration
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
-from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_request import ValidationValidateDatasetRequest
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
+from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
+from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_tags_body import WorkspaceIdUuidTagsBody
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import absolute_import
 
 # flake8: noqa
 
 # import apis into api package
 from rime_sdk.swagger.swagger_client.api.agent_manager_api import AgentManagerApi
 from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
+from rime_sdk.swagger.swagger_client.api.customer_managed_key_service_api import CustomerManagedKeyServiceApi
 from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
 from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
 from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
 from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
 from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
 from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
-from rime_sdk.swagger.swagger_client.api.foo_xp_interface_api import FooXPInterfaceApi
 from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
 from rime_sdk.swagger.swagger_client.api.integration_service_api import IntegrationServiceApi
 from rime_sdk.swagger.swagger_client.api.job_reader_api import JobReaderApi
 from rime_sdk.swagger.swagger_client.api.model_card_service_api import ModelCardServiceApi
 from rime_sdk.swagger.swagger_client.api.model_testing_api import ModelTestingApi
 from rime_sdk.swagger.swagger_client.api.monitor_service_api import MonitorServiceApi
 from rime_sdk.swagger.swagger_client.api.notification_setting_api import NotificationSettingApi
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -614,14 +614,111 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def agent_manager_register_external_agent(self, body, **kwargs):  # noqa: E501
+        """RegisterExternalAgent is used by external agents during startup to upload the signing key to the backend. This call is idempotent; it will be called by the external agent upon every restart. No matter there is a signing key exists in the DB, the key is uploaded and created in the DB.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_register_external_agent(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeRegisterExternalAgentRequest body: (required)
+        :return: object
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.agent_manager_register_external_agent_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.agent_manager_register_external_agent_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def agent_manager_register_external_agent_with_http_info(self, body, **kwargs):  # noqa: E501
+        """RegisterExternalAgent is used by external agents during startup to upload the signing key to the backend. This call is idempotent; it will be called by the external agent upon every restart. No matter there is a signing key exists in the DB, the key is uploaded and created in the DB.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.agent_manager_register_external_agent_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param RimeRegisterExternalAgentRequest body: (required)
+        :return: object
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method agent_manager_register_external_agent" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `agent_manager_register_external_agent`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/internal/agents/external', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='object',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def agent_manager_register_internal_agent(self, **kwargs):  # noqa: E501
         """RegisterInternalAgent is used by internal agents during startup to obtain an ID. This call is idempotent; it will be called by internal agent upon every restart. If no record of an internal agent exists, a new agent is created in the DB.Otherwise, the Agent Management service returns the ID of the existing agent.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.agent_manager_register_internal_agent(async_req=True)
         >>> result = thread.get()
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -634,14 +634,109 @@
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def workspace_service_list_project_tags_in_workspace(self, workspace_id_uuid, **kwargs):  # noqa: E501
+        """ListProjectTagsInWorkspace  # noqa: E501
+
+        List the union of all tags in all projects in the workspace  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_list_project_tags_in_workspace(workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :return: RimeListProjectTagsInWorkspaceResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.workspace_service_list_project_tags_in_workspace_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
+        else:
+            (data) = self.workspace_service_list_project_tags_in_workspace_with_http_info(workspace_id_uuid, **kwargs)  # noqa: E501
+            return data
+
+    def workspace_service_list_project_tags_in_workspace_with_http_info(self, workspace_id_uuid, **kwargs):  # noqa: E501
+        """ListProjectTagsInWorkspace  # noqa: E501
+
+        List the union of all tags in all projects in the workspace  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.workspace_service_list_project_tags_in_workspace_with_http_info(workspace_id_uuid, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param str workspace_id_uuid: Unique object ID. (required)
+        :return: RimeListProjectTagsInWorkspaceResponse
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['workspace_id_uuid']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method workspace_service_list_project_tags_in_workspace" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'workspace_id_uuid' is set
+        if ('workspace_id_uuid' not in params or
+                params['workspace_id_uuid'] is None):
+            raise ValueError("Missing the required parameter `workspace_id_uuid` when calling `workspace_service_list_project_tags_in_workspace`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        if 'workspace_id_uuid' in params:
+            path_params['workspaceId.uuid'] = params['workspace_id_uuid']  # noqa: E501
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['rime-api-key']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/v1/workspace/{workspaceId.uuid}/tags/project', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='RimeListProjectTagsInWorkspaceResponse',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def workspace_service_list_users_of_workspace(self, workspace_id_uuid, **kwargs):  # noqa: E501
         """ListUsersOfWorkspace  # noqa: E501
 
         Lists all Users that have permissions to a Workspace.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.workspace_service_list_users_of_workspace(workspace_id_uuid, async_req=True)
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,66 @@
 # coding: utf-8
 
 # flake8: noqa
+
 """
     Robust Intelligence REST API
 
     API methods for Robust Intelligence. Users must authenticate using the `rime-api-key` header.  # noqa: E501
 
     OpenAPI spec version: 1.0
     Contact: dev@robustintelligence.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
-# import models into model package
+# import apis into sdk package
+from rime_sdk.swagger.swagger_client.api.agent_manager_api import AgentManagerApi
+from rime_sdk.swagger.swagger_client.api.config_validator_api import ConfigValidatorApi
+from rime_sdk.swagger.swagger_client.api.customer_managed_key_service_api import CustomerManagedKeyServiceApi
+from rime_sdk.swagger.swagger_client.api.data_collector_api import DataCollectorApi
+from rime_sdk.swagger.swagger_client.api.detection_api import DetectionApi
+from rime_sdk.swagger.swagger_client.api.feature_flag_api import FeatureFlagApi
+from rime_sdk.swagger.swagger_client.api.file_scanning_api import FileScanningApi
+from rime_sdk.swagger.swagger_client.api.file_upload_api import FileUploadApi
+from rime_sdk.swagger.swagger_client.api.firewall_service_api import FirewallServiceApi
+from rime_sdk.swagger.swagger_client.api.image_registry_api import ImageRegistryApi
+from rime_sdk.swagger.swagger_client.api.integration_service_api import IntegrationServiceApi
+from rime_sdk.swagger.swagger_client.api.job_reader_api import JobReaderApi
+from rime_sdk.swagger.swagger_client.api.model_card_service_api import ModelCardServiceApi
+from rime_sdk.swagger.swagger_client.api.model_testing_api import ModelTestingApi
+from rime_sdk.swagger.swagger_client.api.monitor_service_api import MonitorServiceApi
+from rime_sdk.swagger.swagger_client.api.notification_setting_api import NotificationSettingApi
+from rime_sdk.swagger.swagger_client.api.project_service_api import ProjectServiceApi
+from rime_sdk.swagger.swagger_client.api.rime_info_api import RIMEInfoApi
+from rime_sdk.swagger.swagger_client.api.registry_service_api import RegistryServiceApi
+from rime_sdk.swagger.swagger_client.api.results_reader_api import ResultsReaderApi
+from rime_sdk.swagger.swagger_client.api.user_api import UserApi
+from rime_sdk.swagger.swagger_client.api.validation_service_api import ValidationServiceApi
+from rime_sdk.swagger.swagger_client.api.workspace_service_api import WorkspaceServiceApi
+# import ApiClient
+from rime_sdk.swagger.swagger_client.api_client import ApiClient
+from rime_sdk.swagger.swagger_client.configuration import Configuration
+# import models into sdk package
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_category_test_identifier import ArtifactIdentifierCategoryTestIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_subset_test_metric_identifier import ArtifactIdentifierSubsetTestMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.artifact_identifier_test_case_metric_identifier import ArtifactIdentifierTestCaseMetricIdentifier
 from rime_sdk.swagger.swagger_client.models.configvalidator_config_type_body import ConfigvalidatorConfigTypeBody
 from rime_sdk.swagger.swagger_client.models.continuoustests_firewall_id_uuid_body import ContinuoustestsFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.create_agent_request_aws_config import CreateAgentRequestAWSConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_azure_config import CreateAgentRequestAzureConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_gcp_config import CreateAgentRequestGCPConfig
 from rime_sdk.swagger.swagger_client.models.create_agent_request_local_config import CreateAgentRequestLocalConfig
 from rime_sdk.swagger.swagger_client.models.create_firewall_request_scheduled_ct_parameters import CreateFirewallRequestScheduledCTParameters
 from rime_sdk.swagger.swagger_client.models.custom_image_pull_secret import CustomImagePullSecret
 from rime_sdk.swagger.swagger_client.models.custom_metric_custom_metric_metadata import CustomMetricCustomMetricMetadata
+from rime_sdk.swagger.swagger_client.models.customermanagedkey_customer_managed_key_config import CustomermanagedkeyCustomerManagedKeyConfig
+from rime_sdk.swagger.swagger_client.models.customermanagedkey_key_provider import CustomermanagedkeyKeyProvider
+from rime_sdk.swagger.swagger_client.models.customermanagedkey_key_status import CustomermanagedkeyKeyStatus
 from rime_sdk.swagger.swagger_client.models.custommonitors_name_body import CustommonitorsNameBody
 from rime_sdk.swagger.swagger_client.models.data_data_stream_id_uuid_body import DataDataStreamIdUuidBody
 from rime_sdk.swagger.swagger_client.models.data_params_feature_intersection import DataParamsFeatureIntersection
 from rime_sdk.swagger.swagger_client.models.data_params_ranking_info import DataParamsRankingInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_column_type_info import DataProfilingColumnTypeInfo
 from rime_sdk.swagger.swagger_client.models.data_profiling_feature_relationship_info import DataProfilingFeatureRelationshipInfo
 from rime_sdk.swagger.swagger_client.models.datacollector_datapoint import DatacollectorDatapoint
@@ -56,20 +87,17 @@
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report import FilescanningSecurityReport
 from rime_sdk.swagger.swagger_client.models.filescanning_security_report_import_result import FilescanningSecurityReportImportResult
 from rime_sdk.swagger.swagger_client.models.firewall_firewall import FirewallFirewall
 from rime_sdk.swagger.swagger_client.models.firewall_firewall_firewall_id_uuid_body import FirewallFirewallFirewallIdUuidBody
 from rime_sdk.swagger.swagger_client.models.firewall_latest_run_info import FirewallLatestRunInfo
 from rime_sdk.swagger.swagger_client.models.firewall_scheduled_ct_info import FirewallScheduledCTInfo
 from rime_sdk.swagger.swagger_client.models.firewall_test_category_severity import FirewallTestCategorySeverity
-from rime_sdk.swagger.swagger_client.models.fooexample_foo_request import FooexampleFooRequest
-from rime_sdk.swagger.swagger_client.models.fooexample_foo_response import FooexampleFooResponse
 from rime_sdk.swagger.swagger_client.models.generativestresstests_project_id_uuid_body import GenerativestresstestsProjectIdUuidBody
 from rime_sdk.swagger.swagger_client.models.googlerpc_status import GooglerpcStatus
 from rime_sdk.swagger.swagger_client.models.image_reference_reference_type import ImageReferenceReferenceType
-from rime_sdk.swagger.swagger_client.models.integration_integration import IntegrationIntegration
 from rime_sdk.swagger.swagger_client.models.integration_integration_level import IntegrationIntegrationLevel
 from rime_sdk.swagger.swagger_client.models.integration_integration_schema import IntegrationIntegrationSchema
 from rime_sdk.swagger.swagger_client.models.integration_integration_type import IntegrationIntegrationType
 from rime_sdk.swagger.swagger_client.models.integration_variable_sensitivity import IntegrationVariableSensitivity
 from rime_sdk.swagger.swagger_client.models.integrations_integration_id_uuid_body import IntegrationsIntegrationIdUuidBody
 from rime_sdk.swagger.swagger_client.models.job_data_continuous_incremental_test import JobDataContinuousIncrementalTest
 from rime_sdk.swagger.swagger_client.models.job_data_stress_test import JobDataStressTest
@@ -147,15 +175,16 @@
 from rime_sdk.swagger.swagger_client.models.rca_test_case_id import RcaTestCaseID
 from rime_sdk.swagger.swagger_client.models.registry_connection_info import RegistryConnectionInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_collector_info import RegistryDataCollectorInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_file_info import RegistryDataFileInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_info import RegistryDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_loading_info import RegistryDataLoadingInfo
 from rime_sdk.swagger.swagger_client.models.registry_data_params import RegistryDataParams
-from rime_sdk.swagger.swagger_client.models.registry_delta_lake_info import RegistryDeltaLakeInfo
+from rime_sdk.swagger.swagger_client.models.registry_data_type import RegistryDataType
+from rime_sdk.swagger.swagger_client.models.registry_databricks_info import RegistryDatabricksInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_data_info import RegistryHuggingFaceDataInfo
 from rime_sdk.swagger.swagger_client.models.registry_hugging_face_model_info import RegistryHuggingFaceModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_metadata import RegistryMetadata
 from rime_sdk.swagger.swagger_client.models.registry_model_info import RegistryModelInfo
 from rime_sdk.swagger.swagger_client.models.registry_model_path_info import RegistryModelPathInfo
 from rime_sdk.swagger.swagger_client.models.registry_pred_info import RegistryPredInfo
 from rime_sdk.swagger.swagger_client.models.registry_prediction_params import RegistryPredictionParams
@@ -177,14 +206,16 @@
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_job_progress import RimeContinuousTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_continuous_test_run_progress import RimeContinuousTestRunProgress
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_request import RimeCreateAPITokenRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_api_token_response import RimeCreateAPITokenResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_request import RimeCreateAgentRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_agent_response import RimeCreateAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_custom_monitor_response import RimeCreateCustomMonitorResponse
+from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_request import RimeCreateCustomerManagedKeyRequest
+from rime_sdk.swagger.swagger_client.models.rime_create_customer_managed_key_response import RimeCreateCustomerManagedKeyResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_request import RimeCreateFirewallRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_firewall_response import RimeCreateFirewallResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_image_request import RimeCreateImageRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_image_response import RimeCreateImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_request import RimeCreateIntegrationRequest
 from rime_sdk.swagger.swagger_client.models.rime_create_integration_response import RimeCreateIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_create_model_card_request import RimeCreateModelCardRequest
@@ -211,39 +242,42 @@
 from rime_sdk.swagger.swagger_client.models.rime_ensure_image_existence_response import RimeEnsureImageExistenceResponse
 from rime_sdk.swagger.swagger_client.models.rime_failing_row import RimeFailingRow
 from rime_sdk.swagger.swagger_client.models.rime_failing_rows_result import RimeFailingRowsResult
 from rime_sdk.swagger.swagger_client.models.rime_feature_flags import RimeFeatureFlags
 from rime_sdk.swagger.swagger_client.models.rime_feature_type import RimeFeatureType
 from rime_sdk.swagger.swagger_client.models.rime_float_list import RimeFloatList
 from rime_sdk.swagger.swagger_client.models.rime_get_agent_response import RimeGetAgentResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_customer_managed_key_response import RimeGetCustomerManagedKeyResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_datapoints_response import RimeGetDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_file_upload_url_response import RimeGetDatasetFileUploadURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_dataset_response import RimeGetDatasetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_enabled_feature_response import RimeGetEnabledFeatureResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flag_jwt_response import RimeGetFeatureFlagJwtResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_feature_flags_response import RimeGetFeatureFlagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_firewall_response import RimeGetFirewallResponse
-from rime_sdk.swagger.swagger_client.models.rime_get_foo_task_status_response import RimeGetFooTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_image_response import RimeGetImageResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_integration_response import RimeGetIntegrationResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_job_response import RimeGetJobResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_key_status_response import RimeGetKeyStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_latest_logs_response import RimeGetLatestLogsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_limit_status_response import RimeGetLimitStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_card_response import RimeGetModelCardResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_directory_upload_urls_response import RimeGetModelDirectoryUploadURLsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_model_response import RimeGetModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_monitor_result_response import RimeGetMonitorResultResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_prediction_set_response import RimeGetPredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_predictions_response import RimeGetPredictionsResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_project_id_response import RimeGetProjectIDResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_rime_info_response import RimeGetRIMEInfoResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_test_run_id_response import RimeGetTestRunIDResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_url_response import RimeGetURLResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_user_response import RimeGetUserResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_validate_dataset_task_status_response import RimeGetValidateDatasetTaskStatusResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_validate_model_task_status_response import RimeGetValidateModelTaskStatusResponse
+from rime_sdk.swagger.swagger_client.models.rime_get_validate_predictions_task_status_response import RimeGetValidatePredictionsTaskStatusResponse
 from rime_sdk.swagger.swagger_client.models.rime_get_workspace_response import RimeGetWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_heartbeat_response import RimeHeartbeatResponse
 from rime_sdk.swagger.swagger_client.models.rime_image_reference import RimeImageReference
 from rime_sdk.swagger.swagger_client.models.rime_int_list import RimeIntList
 from rime_sdk.swagger.swagger_client.models.rime_integration_info import RimeIntegrationInfo
 from rime_sdk.swagger.swagger_client.models.rime_job_data import RimeJobData
 from rime_sdk.swagger.swagger_client.models.rime_job_metadata import RimeJobMetadata
@@ -268,14 +302,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_list_jobs_for_project_response import RimeListJobsForProjectResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_metric_identifiers_response import RimeListMetricIdentifiersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_model_cards_response import RimeListModelCardsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_models_response import RimeListModelsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_monitors_response import RimeListMonitorsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_notifications_response import RimeListNotificationsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_prediction_sets_response import RimeListPredictionSetsResponse
+from rime_sdk.swagger.swagger_client.models.rime_list_project_tags_in_workspace_response import RimeListProjectTagsInWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_uploaded_file_urls_response import RimeListUploadedFileURLsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_of_workspace_response import RimeListUsersOfWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_users_request_query import RimeListUsersRequestQuery
 from rime_sdk.swagger.swagger_client.models.rime_list_users_response import RimeListUsersResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspace_integrations_response import RimeListWorkspaceIntegrationsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspace_tags_response import RimeListWorkspaceTagsResponse
 from rime_sdk.swagger.swagger_client.models.rime_list_workspaces_request_query import RimeListWorkspacesRequestQuery
@@ -290,34 +325,37 @@
 from rime_sdk.swagger.swagger_client.models.rime_named_double import RimeNamedDouble
 from rime_sdk.swagger.swagger_client.models.rime_order import RimeOrder
 from rime_sdk.swagger.swagger_client.models.rime_parent_role_subject_role_pair import RimeParentRoleSubjectRolePair
 from rime_sdk.swagger.swagger_client.models.rime_ri_email_recipient import RimeRIEmailRecipient
 from rime_sdk.swagger.swagger_client.models.rime_ri_plan import RimeRIPlan
 from rime_sdk.swagger.swagger_client.models.rime_register_data_stream_response import RimeRegisterDataStreamResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_dataset_response import RimeRegisterDatasetResponse
+from rime_sdk.swagger.swagger_client.models.rime_register_external_agent_request import RimeRegisterExternalAgentRequest
 from rime_sdk.swagger.swagger_client.models.rime_register_internal_agent_response import RimeRegisterInternalAgentResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_model_response import RimeRegisterModelResponse
 from rime_sdk.swagger.swagger_client.models.rime_register_prediction_set_response import RimeRegisterPredictionSetResponse
 from rime_sdk.swagger.swagger_client.models.rime_remove_user_from_workspace_response import RimeRemoveUserFromWorkspaceResponse
 from rime_sdk.swagger.swagger_client.models.rime_reset_password_response import RimeResetPasswordResponse
 from rime_sdk.swagger.swagger_client.models.rime_resolve_detection_event_response import RimeResolveDetectionEventResponse
 from rime_sdk.swagger.swagger_client.models.rime_safe_url import RimeSafeURL
 from rime_sdk.swagger.swagger_client.models.rime_send_ri_email_response import RimeSendRIEmailResponse
 from rime_sdk.swagger.swagger_client.models.rime_severity import RimeSeverity
 from rime_sdk.swagger.swagger_client.models.rime_severity_counts import RimeSeverityCounts
 from rime_sdk.swagger.swagger_client.models.rime_sort_spec import RimeSortSpec
 from rime_sdk.swagger.swagger_client.models.rime_start_continuous_test_response import RimeStartContinuousTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_request import RimeStartFileScanRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_file_scan_response import RimeStartFileScanResponse
-from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_request import RimeStartFooTaskRequest
-from rime_sdk.swagger.swagger_client.models.rime_start_foo_task_response import RimeStartFooTaskResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_generative_stress_test_response import RimeStartGenerativeStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_stress_test_response import RimeStartStressTestResponse
 from rime_sdk.swagger.swagger_client.models.rime_start_validate_dataset_task_request import RimeStartValidateDatasetTaskRequest
 from rime_sdk.swagger.swagger_client.models.rime_start_validate_dataset_task_response import RimeStartValidateDatasetTaskResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_model_task_request import RimeStartValidateModelTaskRequest
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_model_task_response import RimeStartValidateModelTaskResponse
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_predictions_task_request import RimeStartValidatePredictionsTaskRequest
+from rime_sdk.swagger.swagger_client.models.rime_start_validate_predictions_task_response import RimeStartValidatePredictionsTaskResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_datapoints_response import RimeStoreDatapointsResponse
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_request_prediction import RimeStorePredictionsRequestPrediction
 from rime_sdk.swagger.swagger_client.models.rime_store_predictions_response import RimeStorePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.rime_str_list import RimeStrList
 from rime_sdk.swagger.swagger_client.models.rime_stress_test_job_progress import RimeStressTestJobProgress
 from rime_sdk.swagger.swagger_client.models.rime_subject_type import RimeSubjectType
 from rime_sdk.swagger.swagger_client.models.rime_suggestion import RimeSuggestion
@@ -350,14 +388,15 @@
 from rime_sdk.swagger.swagger_client.models.rime_user_detail_with_role import RimeUserDetailWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_role import RimeUserRole
 from rime_sdk.swagger.swagger_client.models.rime_user_with_role import RimeUserWithRole
 from rime_sdk.swagger.swagger_client.models.rime_user_write_mask import RimeUserWriteMask
 from rime_sdk.swagger.swagger_client.models.rime_validate_test_config_response import RimeValidateTestConfigResponse
 from rime_sdk.swagger.swagger_client.models.rime_workspace import RimeWorkspace
 from rime_sdk.swagger.swagger_client.models.rime_workspace_write_mask import RimeWorkspaceWriteMask
+from rime_sdk.swagger.swagger_client.models.rischemaintegration_integration import RischemaintegrationIntegration
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_category_type import RiskscoreRiskCategoryType
 from rime_sdk.swagger.swagger_client.models.riskscore_risk_score import RiskscoreRiskScore
 from rime_sdk.swagger.swagger_client.models.role_users_body import RoleUsersBody
 from rime_sdk.swagger.swagger_client.models.role_workspace_body import RoleWorkspaceBody
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image import RuntimeinfoCustomImage
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_custom_image_type import RuntimeinfoCustomImageType
 from rime_sdk.swagger.swagger_client.models.runtimeinfo_resource_request import RuntimeinfoResourceRequest
@@ -419,12 +458,13 @@
 from rime_sdk.swagger.swagger_client.models.users_user_user_id_uuid_body1 import UsersUserUserIdUuidBody1
 from rime_sdk.swagger.swagger_client.models.v1betaintegrationsintegration_id_uuid_integration import V1betaintegrationsintegrationIdUuidIntegration
 from rime_sdk.swagger.swagger_client.models.v1betamodelcardsmodel_card_model_card_id_uuid_model_card import V1betamodelcardsmodelCardModelCardIdUuidModelCard
 from rime_sdk.swagger.swagger_client.models.v1firewallfirewall_firewall_id_uuid_firewall import V1firewallfirewallFirewallIdUuidFirewall
 from rime_sdk.swagger.swagger_client.models.v1projectsproject_id_uuidroleusersuser_user_id_uuid_user import V1projectsprojectIdUuidroleusersuserUserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1usersuser_id_uuid_user import V1usersuserIdUuidUser
 from rime_sdk.swagger.swagger_client.models.v1workspaceworkspace_workspace_id_uuid_workspace import V1workspaceworkspaceWorkspaceIdUuidWorkspace
-from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_request import ValidationValidateDatasetRequest
 from rime_sdk.swagger.swagger_client.models.validation_validate_dataset_response import ValidationValidateDatasetResponse
+from rime_sdk.swagger.swagger_client.models.validation_validate_model_response import ValidationValidateModelResponse
+from rime_sdk.swagger.swagger_client.models.validation_validate_predictions_response import ValidationValidatePredictionsResponse
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_tags_body import WorkspaceIdUuidTagsBody
 from rime_sdk.swagger.swagger_client.models.workspace_id_uuid_users_body import WorkspaceIdUuidUsersBody
 from rime_sdk.swagger.swagger_client.models.workspace_workspace_workspace_id_uuid_body import WorkspaceWorkspaceWorkspaceIdUuidBody
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,43 +28,48 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'object',
         'model_id': 'object',
         'metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
-        'pred_info': 'RegistryPredInfo'
+        'pred_info': 'RegistryPredInfo',
+        'skip_validation': 'bool'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'model_id': 'modelId',
         'metadata': 'metadata',
         'integration_id': 'integrationId',
-        'pred_info': 'predInfo'
+        'pred_info': 'predInfo',
+        'skip_validation': 'skipValidation'
     }
 
-    def __init__(self, project_id=None, model_id=None, metadata=None, integration_id=None, pred_info=None):  # noqa: E501
+    def __init__(self, project_id=None, model_id=None, metadata=None, integration_id=None, pred_info=None, skip_validation=None):  # noqa: E501
         """DatasetIdPredictionBody - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
         self._model_id = None
         self._metadata = None
         self._integration_id = None
         self._pred_info = None
+        self._skip_validation = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
         if model_id is not None:
             self.model_id = model_id
         if metadata is not None:
             self.metadata = metadata
         if integration_id is not None:
             self.integration_id = integration_id
         if pred_info is not None:
             self.pred_info = pred_info
+        if skip_validation is not None:
+            self.skip_validation = skip_validation
 
     @property
     def project_id(self):
         """Gets the project_id of this DatasetIdPredictionBody.  # noqa: E501
 
         Uniquely specifies a Project.  # noqa: E501
 
@@ -167,14 +172,35 @@
 
         :param pred_info: The pred_info of this DatasetIdPredictionBody.  # noqa: E501
         :type: RegistryPredInfo
         """
 
         self._pred_info = pred_info
 
+    @property
+    def skip_validation(self):
+        """Gets the skip_validation of this DatasetIdPredictionBody.  # noqa: E501
+
+
+        :return: The skip_validation of this DatasetIdPredictionBody.  # noqa: E501
+        :rtype: bool
+        """
+        return self._skip_validation
+
+    @skip_validation.setter
+    def skip_validation(self, skip_validation):
+        """Sets the skip_validation of this DatasetIdPredictionBody.
+
+
+        :param skip_validation: The skip_validation of this DatasetIdPredictionBody.  # noqa: E501
+        :type: bool
+        """
+
+        self._skip_validation = skip_validation
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_huggingface_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_model_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_pytorch_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,61 +11,35 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FooexampleFooRequest(object):
+class RimeSendRIEmailResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'should_fail': 'bool'
     }
 
     attribute_map = {
-        'should_fail': 'shouldFail'
     }
 
-    def __init__(self, should_fail=None):  # noqa: E501
-        """FooexampleFooRequest - a model defined in Swagger"""  # noqa: E501
-        self._should_fail = None
+    def __init__(self):  # noqa: E501
+        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if should_fail is not None:
-            self.should_fail = should_fail
-
-    @property
-    def should_fail(self):
-        """Gets the should_fail of this FooexampleFooRequest.  # noqa: E501
-
-
-        :return: The should_fail of this FooexampleFooRequest.  # noqa: E501
-        :rtype: bool
-        """
-        return self._should_fail
-
-    @should_fail.setter
-    def should_fail(self, should_fail):
-        """Sets the should_fail of this FooexampleFooRequest.
-
-
-        :param should_fail: The should_fail of this FooexampleFooRequest.  # noqa: E501
-        :type: bool
-        """
-
-        self._should_fail = should_fail
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FooexampleFooRequest, dict):
+        if issubclass(RimeSendRIEmailResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FooexampleFooRequest):
+        if not isinstance(other, RimeSendRIEmailResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class FooexampleFooResponse(object):
+class RimeFloatList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'receive_time': 'datetime'
+        'values': 'list[float]'
     }
 
     attribute_map = {
-        'receive_time': 'receiveTime'
+        'values': 'values'
     }
 
-    def __init__(self, receive_time=None):  # noqa: E501
-        """FooexampleFooResponse - a model defined in Swagger"""  # noqa: E501
-        self._receive_time = None
+    def __init__(self, values=None):  # noqa: E501
+        """RimeFloatList - a model defined in Swagger"""  # noqa: E501
+        self._values = None
         self.discriminator = None
-        if receive_time is not None:
-            self.receive_time = receive_time
+        if values is not None:
+            self.values = values
 
     @property
-    def receive_time(self):
-        """Gets the receive_time of this FooexampleFooResponse.  # noqa: E501
+    def values(self):
+        """Gets the values of this RimeFloatList.  # noqa: E501
 
 
-        :return: The receive_time of this FooexampleFooResponse.  # noqa: E501
-        :rtype: datetime
+        :return: The values of this RimeFloatList.  # noqa: E501
+        :rtype: list[float]
         """
-        return self._receive_time
+        return self._values
 
-    @receive_time.setter
-    def receive_time(self, receive_time):
-        """Sets the receive_time of this FooexampleFooResponse.
+    @values.setter
+    def values(self, values):
+        """Sets the values of this RimeFloatList.
 
 
-        :param receive_time: The receive_time of this FooexampleFooResponse.  # noqa: E501
-        :type: datetime
+        :param values: The values of this RimeFloatList.  # noqa: E501
+        :type: list[float]
         """
 
-        self._receive_time = receive_time
+        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(FooexampleFooResponse, dict):
+        if issubclass(RimeFloatList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FooexampleFooResponse):
+        if not isinstance(other, RimeFloatList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class IntegrationIntegration(object):
+class RischemaintegrationIntegration(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -44,15 +44,15 @@
         'name': 'name',
         'type': 'type',
         'schema': 'schema',
         'level': 'level'
     }
 
     def __init__(self, id=None, workspace_id=None, creation_time=None, name=None, type=None, schema=None, level=None):  # noqa: E501
-        """IntegrationIntegration - a model defined in Swagger"""  # noqa: E501
+        """RischemaintegrationIntegration - a model defined in Swagger"""  # noqa: E501
         self._id = None
         self._workspace_id = None
         self._creation_time = None
         self._name = None
         self._type = None
         self._schema = None
         self._level = None
@@ -70,154 +70,154 @@
         if schema is not None:
             self.schema = schema
         if level is not None:
             self.level = level
 
     @property
     def id(self):
-        """Gets the id of this IntegrationIntegration.  # noqa: E501
+        """Gets the id of this RischemaintegrationIntegration.  # noqa: E501
 
 
-        :return: The id of this IntegrationIntegration.  # noqa: E501
+        :return: The id of this RischemaintegrationIntegration.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._id
 
     @id.setter
     def id(self, id):
-        """Sets the id of this IntegrationIntegration.
+        """Sets the id of this RischemaintegrationIntegration.
 
 
-        :param id: The id of this IntegrationIntegration.  # noqa: E501
+        :param id: The id of this RischemaintegrationIntegration.  # noqa: E501
         :type: RimeUUID
         """
 
         self._id = id
 
     @property
     def workspace_id(self):
-        """Gets the workspace_id of this IntegrationIntegration.  # noqa: E501
+        """Gets the workspace_id of this RischemaintegrationIntegration.  # noqa: E501
 
 
-        :return: The workspace_id of this IntegrationIntegration.  # noqa: E501
+        :return: The workspace_id of this RischemaintegrationIntegration.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._workspace_id
 
     @workspace_id.setter
     def workspace_id(self, workspace_id):
-        """Sets the workspace_id of this IntegrationIntegration.
+        """Sets the workspace_id of this RischemaintegrationIntegration.
 
 
-        :param workspace_id: The workspace_id of this IntegrationIntegration.  # noqa: E501
+        :param workspace_id: The workspace_id of this RischemaintegrationIntegration.  # noqa: E501
         :type: RimeUUID
         """
 
         self._workspace_id = workspace_id
 
     @property
     def creation_time(self):
-        """Gets the creation_time of this IntegrationIntegration.  # noqa: E501
+        """Gets the creation_time of this RischemaintegrationIntegration.  # noqa: E501
 
 
-        :return: The creation_time of this IntegrationIntegration.  # noqa: E501
+        :return: The creation_time of this RischemaintegrationIntegration.  # noqa: E501
         :rtype: datetime
         """
         return self._creation_time
 
     @creation_time.setter
     def creation_time(self, creation_time):
-        """Sets the creation_time of this IntegrationIntegration.
+        """Sets the creation_time of this RischemaintegrationIntegration.
 
 
-        :param creation_time: The creation_time of this IntegrationIntegration.  # noqa: E501
+        :param creation_time: The creation_time of this RischemaintegrationIntegration.  # noqa: E501
         :type: datetime
         """
 
         self._creation_time = creation_time
 
     @property
     def name(self):
-        """Gets the name of this IntegrationIntegration.  # noqa: E501
+        """Gets the name of this RischemaintegrationIntegration.  # noqa: E501
 
 
-        :return: The name of this IntegrationIntegration.  # noqa: E501
+        :return: The name of this RischemaintegrationIntegration.  # noqa: E501
         :rtype: str
         """
         return self._name
 
     @name.setter
     def name(self, name):
-        """Sets the name of this IntegrationIntegration.
+        """Sets the name of this RischemaintegrationIntegration.
 
 
-        :param name: The name of this IntegrationIntegration.  # noqa: E501
+        :param name: The name of this RischemaintegrationIntegration.  # noqa: E501
         :type: str
         """
 
         self._name = name
 
     @property
     def type(self):
-        """Gets the type of this IntegrationIntegration.  # noqa: E501
+        """Gets the type of this RischemaintegrationIntegration.  # noqa: E501
 
 
-        :return: The type of this IntegrationIntegration.  # noqa: E501
+        :return: The type of this RischemaintegrationIntegration.  # noqa: E501
         :rtype: IntegrationIntegrationType
         """
         return self._type
 
     @type.setter
     def type(self, type):
-        """Sets the type of this IntegrationIntegration.
+        """Sets the type of this RischemaintegrationIntegration.
 
 
-        :param type: The type of this IntegrationIntegration.  # noqa: E501
+        :param type: The type of this RischemaintegrationIntegration.  # noqa: E501
         :type: IntegrationIntegrationType
         """
 
         self._type = type
 
     @property
     def schema(self):
-        """Gets the schema of this IntegrationIntegration.  # noqa: E501
+        """Gets the schema of this RischemaintegrationIntegration.  # noqa: E501
 
 
-        :return: The schema of this IntegrationIntegration.  # noqa: E501
+        :return: The schema of this RischemaintegrationIntegration.  # noqa: E501
         :rtype: IntegrationIntegrationSchema
         """
         return self._schema
 
     @schema.setter
     def schema(self, schema):
-        """Sets the schema of this IntegrationIntegration.
+        """Sets the schema of this RischemaintegrationIntegration.
 
 
-        :param schema: The schema of this IntegrationIntegration.  # noqa: E501
+        :param schema: The schema of this RischemaintegrationIntegration.  # noqa: E501
         :type: IntegrationIntegrationSchema
         """
 
         self._schema = schema
 
     @property
     def level(self):
-        """Gets the level of this IntegrationIntegration.  # noqa: E501
+        """Gets the level of this RischemaintegrationIntegration.  # noqa: E501
 
 
-        :return: The level of this IntegrationIntegration.  # noqa: E501
+        :return: The level of this RischemaintegrationIntegration.  # noqa: E501
         :rtype: IntegrationIntegrationLevel
         """
         return self._level
 
     @level.setter
     def level(self, level):
-        """Sets the level of this IntegrationIntegration.
+        """Sets the level of this RischemaintegrationIntegration.
 
 
-        :param level: The level of this IntegrationIntegration.  # noqa: E501
+        :param level: The level of this RischemaintegrationIntegration.  # noqa: E501
         :type: IntegrationIntegrationLevel
         """
 
         self._level = level
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -236,15 +236,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(IntegrationIntegration, dict):
+        if issubclass(RischemaintegrationIntegration, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -252,15 +252,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, IntegrationIntegration):
+        if not isinstance(other, RischemaintegrationIntegration):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
     """
     allowed enum values
     """
     UNSPECIFIED = "INTEGRATION_LEVEL_UNSPECIFIED"
     ORGANIZATION = "INTEGRATION_LEVEL_ORGANIZATION"
     WORKSPACE = "INTEGRATION_LEVEL_WORKSPACE"
+    AGENT = "INTEGRATION_LEVEL_AGENT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/object_containing_the_updates_only_the_fields_specified_in_the_mask_will_be_used_by_the_backend_note_the_id_field_is_necessary_to_find_the_given_notification_setting_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,46 +29,51 @@
     """
     swagger_types = {
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'integration_id': 'RimeUUID',
         'data_info': 'RegistryDataInfo',
-        'ct_info': 'DatasetCTInfo'
+        'ct_info': 'DatasetCTInfo',
+        'skip_validation': 'bool'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'name': 'name',
         'metadata': 'metadata',
         'integration_id': 'integrationId',
         'data_info': 'dataInfo',
-        'ct_info': 'ctInfo'
+        'ct_info': 'ctInfo',
+        'skip_validation': 'skipValidation'
     }
 
-    def __init__(self, project_id=None, name=None, metadata=None, integration_id=None, data_info=None, ct_info=None):  # noqa: E501
+    def __init__(self, project_id=None, name=None, metadata=None, integration_id=None, data_info=None, ct_info=None, skip_validation=None):  # noqa: E501
         """ProjectIdUuidDatasetBody - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
         self._name = None
         self._metadata = None
         self._integration_id = None
         self._data_info = None
         self._ct_info = None
+        self._skip_validation = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
         self.name = name
         if metadata is not None:
             self.metadata = metadata
         if integration_id is not None:
             self.integration_id = integration_id
         if data_info is not None:
             self.data_info = data_info
         if ct_info is not None:
             self.ct_info = ct_info
+        if skip_validation is not None:
+            self.skip_validation = skip_validation
 
     @property
     def project_id(self):
         """Gets the project_id of this ProjectIdUuidDatasetBody.  # noqa: E501
 
         Uniquely specifies a Project.  # noqa: E501
 
@@ -194,14 +199,35 @@
 
         :param ct_info: The ct_info of this ProjectIdUuidDatasetBody.  # noqa: E501
         :type: DatasetCTInfo
         """
 
         self._ct_info = ct_info
 
+    @property
+    def skip_validation(self):
+        """Gets the skip_validation of this ProjectIdUuidDatasetBody.  # noqa: E501
+
+
+        :return: The skip_validation of this ProjectIdUuidDatasetBody.  # noqa: E501
+        :rtype: bool
+        """
+        return self._skip_validation
+
+    @skip_validation.setter
+    def skip_validation(self, skip_validation):
+        """Sets the skip_validation of this ProjectIdUuidDatasetBody.
+
+
+        :param skip_validation: The skip_validation of this ProjectIdUuidDatasetBody.  # noqa: E501
+        :type: bool
+        """
+
+        self._skip_validation = skip_validation
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,46 +29,51 @@
     """
     swagger_types = {
         'project_id': 'object',
         'name': 'str',
         'metadata': 'RegistryMetadata',
         'external_id': 'str',
         'model_info': 'RegistryModelInfo',
-        'integration_id': 'RimeUUID'
+        'integration_id': 'RimeUUID',
+        'skip_validation': 'bool'
     }
 
     attribute_map = {
         'project_id': 'projectId',
         'name': 'name',
         'metadata': 'metadata',
         'external_id': 'externalId',
         'model_info': 'modelInfo',
-        'integration_id': 'integrationId'
+        'integration_id': 'integrationId',
+        'skip_validation': 'skipValidation'
     }
 
-    def __init__(self, project_id=None, name=None, metadata=None, external_id=None, model_info=None, integration_id=None):  # noqa: E501
+    def __init__(self, project_id=None, name=None, metadata=None, external_id=None, model_info=None, integration_id=None, skip_validation=None):  # noqa: E501
         """ProjectIdUuidModelBody - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
         self._name = None
         self._metadata = None
         self._external_id = None
         self._model_info = None
         self._integration_id = None
+        self._skip_validation = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
         self.name = name
         if metadata is not None:
             self.metadata = metadata
         if external_id is not None:
             self.external_id = external_id
         if model_info is not None:
             self.model_info = model_info
         if integration_id is not None:
             self.integration_id = integration_id
+        if skip_validation is not None:
+            self.skip_validation = skip_validation
 
     @property
     def project_id(self):
         """Gets the project_id of this ProjectIdUuidModelBody.  # noqa: E501
 
         Uniquely specifies a Project.  # noqa: E501
 
@@ -196,14 +201,35 @@
 
         :param integration_id: The integration_id of this ProjectIdUuidModelBody.  # noqa: E501
         :type: RimeUUID
         """
 
         self._integration_id = integration_id
 
+    @property
+    def skip_validation(self):
+        """Gets the skip_validation of this ProjectIdUuidModelBody.  # noqa: E501
+
+
+        :return: The skip_validation of this ProjectIdUuidModelBody.  # noqa: E501
+        :rtype: bool
+        """
+        return self._skip_validation
+
+    @skip_validation.setter
+    def skip_validation(self, skip_validation):
+        """Sets the skip_validation of this ProjectIdUuidModelBody.
+
+
+        :param skip_validation: The skip_validation of this ProjectIdUuidModelBody.  # noqa: E501
+        :type: bool
+        """
+
+        self._skip_validation = skip_validation
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_feature_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_result.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_rca_role.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_rca_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_cause.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rca_test_case_id.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,42 +27,42 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'data_file': 'RegistryDataFileInfo',
         'data_loading': 'RegistryDataLoadingInfo',
         'data_collector': 'RegistryDataCollectorInfo',
-        'delta_lake': 'RegistryDeltaLakeInfo',
+        'databricks': 'RegistryDatabricksInfo',
         'hugging_face': 'RegistryHuggingFaceDataInfo'
     }
 
     attribute_map = {
         'data_file': 'dataFile',
         'data_loading': 'dataLoading',
         'data_collector': 'dataCollector',
-        'delta_lake': 'deltaLake',
+        'databricks': 'databricks',
         'hugging_face': 'huggingFace'
     }
 
-    def __init__(self, data_file=None, data_loading=None, data_collector=None, delta_lake=None, hugging_face=None):  # noqa: E501
+    def __init__(self, data_file=None, data_loading=None, data_collector=None, databricks=None, hugging_face=None):  # noqa: E501
         """RegistryConnectionInfo - a model defined in Swagger"""  # noqa: E501
         self._data_file = None
         self._data_loading = None
         self._data_collector = None
-        self._delta_lake = None
+        self._databricks = None
         self._hugging_face = None
         self.discriminator = None
         if data_file is not None:
             self.data_file = data_file
         if data_loading is not None:
             self.data_loading = data_loading
         if data_collector is not None:
             self.data_collector = data_collector
-        if delta_lake is not None:
-            self.delta_lake = delta_lake
+        if databricks is not None:
+            self.databricks = databricks
         if hugging_face is not None:
             self.hugging_face = hugging_face
 
     @property
     def data_file(self):
         """Gets the data_file of this RegistryConnectionInfo.  # noqa: E501
 
@@ -122,33 +122,33 @@
         :param data_collector: The data_collector of this RegistryConnectionInfo.  # noqa: E501
         :type: RegistryDataCollectorInfo
         """
 
         self._data_collector = data_collector
 
     @property
-    def delta_lake(self):
-        """Gets the delta_lake of this RegistryConnectionInfo.  # noqa: E501
+    def databricks(self):
+        """Gets the databricks of this RegistryConnectionInfo.  # noqa: E501
 
 
-        :return: The delta_lake of this RegistryConnectionInfo.  # noqa: E501
-        :rtype: RegistryDeltaLakeInfo
+        :return: The databricks of this RegistryConnectionInfo.  # noqa: E501
+        :rtype: RegistryDatabricksInfo
         """
-        return self._delta_lake
+        return self._databricks
 
-    @delta_lake.setter
-    def delta_lake(self, delta_lake):
-        """Sets the delta_lake of this RegistryConnectionInfo.
+    @databricks.setter
+    def databricks(self, databricks):
+        """Sets the databricks of this RegistryConnectionInfo.
 
 
-        :param delta_lake: The delta_lake of this RegistryConnectionInfo.  # noqa: E501
-        :type: RegistryDeltaLakeInfo
+        :param databricks: The databricks of this RegistryConnectionInfo.  # noqa: E501
+        :type: RegistryDatabricksInfo
         """
 
-        self._delta_lake = delta_lake
+        self._databricks = databricks
 
     @property
     def hugging_face(self):
         """Gets the hugging_face of this RegistryConnectionInfo.  # noqa: E501
 
 
         :return: The hugging_face of this RegistryConnectionInfo.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RegistryDataFileInfo(object):
+class RegistryModelPathInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,41 +32,38 @@
     }
 
     attribute_map = {
         'path': 'path'
     }
 
     def __init__(self, path=None):  # noqa: E501
-        """RegistryDataFileInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryModelPathInfo - a model defined in Swagger"""  # noqa: E501
         self._path = None
         self.discriminator = None
-        self.path = path
+        if path is not None:
+            self.path = path
 
     @property
     def path(self):
-        """Gets the path of this RegistryDataFileInfo.  # noqa: E501
+        """Gets the path of this RegistryModelPathInfo.  # noqa: E501
 
-        The path to the data file.  # noqa: E501
 
-        :return: The path of this RegistryDataFileInfo.  # noqa: E501
+        :return: The path of this RegistryModelPathInfo.  # noqa: E501
         :rtype: str
         """
         return self._path
 
     @path.setter
     def path(self, path):
-        """Sets the path of this RegistryDataFileInfo.
+        """Sets the path of this RegistryModelPathInfo.
 
-        The path to the data file.  # noqa: E501
 
-        :param path: The path of this RegistryDataFileInfo.  # noqa: E501
+        :param path: The path of this RegistryModelPathInfo.  # noqa: E501
         :type: str
         """
-        if path is None:
-            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
         self._path = path
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -83,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RegistryDataFileInfo, dict):
+        if issubclass(RegistryModelPathInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RegistryDataFileInfo):
+        if not isinstance(other, RegistryModelPathInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RegistryDeltaLakeInfo(object):
+class RegistryDatabricksInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,37 +32,37 @@
     }
 
     attribute_map = {
         'table_name': 'tableName'
     }
 
     def __init__(self, table_name=None):  # noqa: E501
-        """RegistryDeltaLakeInfo - a model defined in Swagger"""  # noqa: E501
+        """RegistryDatabricksInfo - a model defined in Swagger"""  # noqa: E501
         self._table_name = None
         self.discriminator = None
         self.table_name = table_name
 
     @property
     def table_name(self):
-        """Gets the table_name of this RegistryDeltaLakeInfo.  # noqa: E501
+        """Gets the table_name of this RegistryDatabricksInfo.  # noqa: E501
 
         The database table name to use.  # noqa: E501
 
-        :return: The table_name of this RegistryDeltaLakeInfo.  # noqa: E501
+        :return: The table_name of this RegistryDatabricksInfo.  # noqa: E501
         :rtype: str
         """
         return self._table_name
 
     @table_name.setter
     def table_name(self, table_name):
-        """Sets the table_name of this RegistryDeltaLakeInfo.
+        """Sets the table_name of this RegistryDatabricksInfo.
 
         The database table name to use.  # noqa: E501
 
-        :param table_name: The table_name of this RegistryDeltaLakeInfo.  # noqa: E501
+        :param table_name: The table_name of this RegistryDatabricksInfo.  # noqa: E501
         :type: str
         """
         if table_name is None:
             raise ValueError("Invalid value for `table_name`, must not be `None`")  # noqa: E501
 
         self._table_name = table_name
 
@@ -83,15 +83,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RegistryDeltaLakeInfo, dict):
+        if issubclass(RegistryDatabricksInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -99,15 +99,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RegistryDeltaLakeInfo):
+        if not isinstance(other, RegistryDatabricksInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,61 +11,43 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RegistryModelPathInfo(object):
+class RimeSeverity(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "SEVERITY_UNSPECIFIED"
+    PASS = "SEVERITY_PASS"
+    WARNING = "SEVERITY_WARNING"
+    ALERT = "SEVERITY_ALERT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'path': 'str'
     }
 
     attribute_map = {
-        'path': 'path'
     }
 
-    def __init__(self, path=None):  # noqa: E501
-        """RegistryModelPathInfo - a model defined in Swagger"""  # noqa: E501
-        self._path = None
+    def __init__(self):  # noqa: E501
+        """RimeSeverity - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if path is not None:
-            self.path = path
-
-    @property
-    def path(self):
-        """Gets the path of this RegistryModelPathInfo.  # noqa: E501
-
-
-        :return: The path of this RegistryModelPathInfo.  # noqa: E501
-        :rtype: str
-        """
-        return self._path
-
-    @path.setter
-    def path(self, path):
-        """Sets the path of this RegistryModelPathInfo.
-
-
-        :param path: The path of this RegistryModelPathInfo.  # noqa: E501
-        :type: str
-        """
-
-        self._path = path
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RegistryModelPathInfo, dict):
+        if issubclass(RimeSeverity, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RegistryModelPathInfo):
+        if not isinstance(other, RimeSeverity):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,35 +26,40 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'name': 'str',
         'workspace_id': 'RimeUUID',
-        'token_type': 'RimeTokenType'
+        'token_type': 'RimeTokenType',
+        'agent_id': 'RimeUUID'
     }
 
     attribute_map = {
         'name': 'name',
         'workspace_id': 'workspaceId',
-        'token_type': 'tokenType'
+        'token_type': 'tokenType',
+        'agent_id': 'agentId'
     }
 
-    def __init__(self, name=None, workspace_id=None, token_type=None):  # noqa: E501
+    def __init__(self, name=None, workspace_id=None, token_type=None, agent_id=None):  # noqa: E501
         """RimeCreateAPITokenRequest - a model defined in Swagger"""  # noqa: E501
         self._name = None
         self._workspace_id = None
         self._token_type = None
+        self._agent_id = None
         self.discriminator = None
         if name is not None:
             self.name = name
         if workspace_id is not None:
             self.workspace_id = workspace_id
         if token_type is not None:
             self.token_type = token_type
+        if agent_id is not None:
+            self.agent_id = agent_id
 
     @property
     def name(self):
         """Gets the name of this RimeCreateAPITokenRequest.  # noqa: E501
 
         Name of the API token.  # noqa: E501
 
@@ -113,14 +118,35 @@
 
         :param token_type: The token_type of this RimeCreateAPITokenRequest.  # noqa: E501
         :type: RimeTokenType
         """
 
         self._token_type = token_type
 
+    @property
+    def agent_id(self):
+        """Gets the agent_id of this RimeCreateAPITokenRequest.  # noqa: E501
+
+
+        :return: The agent_id of this RimeCreateAPITokenRequest.  # noqa: E501
+        :rtype: RimeUUID
+        """
+        return self._agent_id
+
+    @agent_id.setter
+    def agent_id(self, agent_id):
+        """Sets the agent_id of this RimeCreateAPITokenRequest.
+
+
+        :param agent_id: The agent_id of this RimeCreateAPITokenRequest.  # noqa: E501
+        :type: RimeUUID
+        """
+
+        self._agent_id = agent_id
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'integration': 'IntegrationIntegration'
+        'integration': 'RischemaintegrationIntegration'
     }
 
     attribute_map = {
         'integration': 'integration'
     }
 
     def __init__(self, integration=None):  # noqa: E501
@@ -44,25 +44,25 @@
 
     @property
     def integration(self):
         """Gets the integration of this RimeCreateIntegrationRequest.  # noqa: E501
 
 
         :return: The integration of this RimeCreateIntegrationRequest.  # noqa: E501
-        :rtype: IntegrationIntegration
+        :rtype: RischemaintegrationIntegration
         """
         return self._integration
 
     @integration.setter
     def integration(self, integration):
         """Sets the integration of this RimeCreateIntegrationRequest.
 
 
         :param integration: The integration of this RimeCreateIntegrationRequest.  # noqa: E501
-        :type: IntegrationIntegration
+        :type: RischemaintegrationIntegration
         """
 
         self._integration = integration
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_create_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_deactivate_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_delete_workspace_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,58 +11,58 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeFloatList(object):
+class RimeIntList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'values': 'list[float]'
+        'values': 'list[str]'
     }
 
     attribute_map = {
         'values': 'values'
     }
 
     def __init__(self, values=None):  # noqa: E501
-        """RimeFloatList - a model defined in Swagger"""  # noqa: E501
+        """RimeIntList - a model defined in Swagger"""  # noqa: E501
         self._values = None
         self.discriminator = None
         if values is not None:
             self.values = values
 
     @property
     def values(self):
-        """Gets the values of this RimeFloatList.  # noqa: E501
+        """Gets the values of this RimeIntList.  # noqa: E501
 
 
-        :return: The values of this RimeFloatList.  # noqa: E501
-        :rtype: list[float]
+        :return: The values of this RimeIntList.  # noqa: E501
+        :rtype: list[str]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this RimeFloatList.
+        """Sets the values of this RimeIntList.
 
 
-        :param values: The values of this RimeFloatList.  # noqa: E501
-        :type: list[float]
+        :param values: The values of this RimeIntList.  # noqa: E501
+        :type: list[str]
         """
 
         self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeFloatList, dict):
+        if issubclass(RimeIntList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeFloatList):
+        if not isinstance(other, RimeIntList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,87 +11,87 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeGetFooTaskStatusResponse(object):
+class RimeGetValidateModelTaskStatusResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'res': 'FooexampleFooResponse',
-        'job': 'RimeJobMetadata'
+        'resp': 'ValidationValidateModelResponse',
+        'job_metadata': 'RimeJobMetadata'
     }
 
     attribute_map = {
-        'res': 'res',
-        'job': 'job'
+        'resp': 'resp',
+        'job_metadata': 'jobMetadata'
     }
 
-    def __init__(self, res=None, job=None):  # noqa: E501
-        """RimeGetFooTaskStatusResponse - a model defined in Swagger"""  # noqa: E501
-        self._res = None
-        self._job = None
+    def __init__(self, resp=None, job_metadata=None):  # noqa: E501
+        """RimeGetValidateModelTaskStatusResponse - a model defined in Swagger"""  # noqa: E501
+        self._resp = None
+        self._job_metadata = None
         self.discriminator = None
-        if res is not None:
-            self.res = res
-        if job is not None:
-            self.job = job
+        if resp is not None:
+            self.resp = resp
+        if job_metadata is not None:
+            self.job_metadata = job_metadata
 
     @property
-    def res(self):
-        """Gets the res of this RimeGetFooTaskStatusResponse.  # noqa: E501
+    def resp(self):
+        """Gets the resp of this RimeGetValidateModelTaskStatusResponse.  # noqa: E501
 
 
-        :return: The res of this RimeGetFooTaskStatusResponse.  # noqa: E501
-        :rtype: FooexampleFooResponse
+        :return: The resp of this RimeGetValidateModelTaskStatusResponse.  # noqa: E501
+        :rtype: ValidationValidateModelResponse
         """
-        return self._res
+        return self._resp
 
-    @res.setter
-    def res(self, res):
-        """Sets the res of this RimeGetFooTaskStatusResponse.
+    @resp.setter
+    def resp(self, resp):
+        """Sets the resp of this RimeGetValidateModelTaskStatusResponse.
 
 
-        :param res: The res of this RimeGetFooTaskStatusResponse.  # noqa: E501
-        :type: FooexampleFooResponse
+        :param resp: The resp of this RimeGetValidateModelTaskStatusResponse.  # noqa: E501
+        :type: ValidationValidateModelResponse
         """
 
-        self._res = res
+        self._resp = resp
 
     @property
-    def job(self):
-        """Gets the job of this RimeGetFooTaskStatusResponse.  # noqa: E501
+    def job_metadata(self):
+        """Gets the job_metadata of this RimeGetValidateModelTaskStatusResponse.  # noqa: E501
 
 
-        :return: The job of this RimeGetFooTaskStatusResponse.  # noqa: E501
+        :return: The job_metadata of this RimeGetValidateModelTaskStatusResponse.  # noqa: E501
         :rtype: RimeJobMetadata
         """
-        return self._job
+        return self._job_metadata
 
-    @job.setter
-    def job(self, job):
-        """Sets the job of this RimeGetFooTaskStatusResponse.
+    @job_metadata.setter
+    def job_metadata(self, job_metadata):
+        """Sets the job_metadata of this RimeGetValidateModelTaskStatusResponse.
 
 
-        :param job: The job of this RimeGetFooTaskStatusResponse.  # noqa: E501
+        :param job_metadata: The job_metadata of this RimeGetValidateModelTaskStatusResponse.  # noqa: E501
         :type: RimeJobMetadata
         """
 
-        self._job = job
+        self._job_metadata = job_metadata
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeGetFooTaskStatusResponse, dict):
+        if issubclass(RimeGetValidateModelTaskStatusResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -122,15 +122,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeGetFooTaskStatusResponse):
+        if not isinstance(other, RimeGetValidateModelTaskStatusResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeIntList(object):
+class RimeStrList(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'values': 'values'
     }
 
     def __init__(self, values=None):  # noqa: E501
-        """RimeIntList - a model defined in Swagger"""  # noqa: E501
+        """RimeStrList - a model defined in Swagger"""  # noqa: E501
         self._values = None
         self.discriminator = None
         if values is not None:
             self.values = values
 
     @property
     def values(self):
-        """Gets the values of this RimeIntList.  # noqa: E501
+        """Gets the values of this RimeStrList.  # noqa: E501
 
 
-        :return: The values of this RimeIntList.  # noqa: E501
+        :return: The values of this RimeStrList.  # noqa: E501
         :rtype: list[str]
         """
         return self._values
 
     @values.setter
     def values(self, values):
-        """Sets the values of this RimeIntList.
+        """Sets the values of this RimeStrList.
 
 
-        :param values: The values of this RimeIntList.  # noqa: E501
+        :param values: The values of this RimeStrList.  # noqa: E501
         :type: list[str]
         """
 
         self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeIntList, dict):
+        if issubclass(RimeStrList, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeIntList):
+        if not isinstance(other, RimeStrList):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'integration': 'IntegrationIntegration',
+        'integration': 'RischemaintegrationIntegration',
         'configured': 'bool'
     }
 
     attribute_map = {
         'integration': 'integration',
         'configured': 'configured'
     }
@@ -49,25 +49,25 @@
 
     @property
     def integration(self):
         """Gets the integration of this RimeIntegrationInfo.  # noqa: E501
 
 
         :return: The integration of this RimeIntegrationInfo.  # noqa: E501
-        :rtype: IntegrationIntegration
+        :rtype: RischemaintegrationIntegration
         """
         return self._integration
 
     @integration.setter
     def integration(self, integration):
         """Sets the integration of this RimeIntegrationInfo.
 
 
         :param integration: The integration of this RimeIntegrationInfo.  # noqa: E501
-        :type: IntegrationIntegration
+        :type: RischemaintegrationIntegration
         """
 
         self._integration = integration
 
     @property
     def configured(self):
         """Gets the configured of this RimeIntegrationInfo.  # noqa: E501
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSendRIEmailResponse(object):
+class RimeUpdateWorkspaceTagResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeSendRIEmailResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSendRIEmailResponse, dict):
+        if issubclass(RimeUpdateWorkspaceTagResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSendRIEmailResponse):
+        if not isinstance(other, RimeUpdateWorkspaceTagResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,42 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeSeverity(object):
+class RimeTestCaseStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "SEVERITY_UNSPECIFIED"
-    PASS = "SEVERITY_PASS"
-    WARNING = "SEVERITY_WARNING"
-    ALERT = "SEVERITY_ALERT"
+    PASS_UNSPECIFIED = "TEST_CASE_STATUS_PASS_UNSPECIFIED"
+    WARNING = "TEST_CASE_STATUS_WARNING"
+    FAIL = "TEST_CASE_STATUS_FAIL"
+    SKIP = "TEST_CASE_STATUS_SKIP"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeSeverity - a model defined in Swagger"""  # noqa: E501
+        """RimeTestCaseStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeSeverity, dict):
+        if issubclass(RimeTestCaseStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeSeverity):
+        if not isinstance(other, RimeTestCaseStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,109 +11,109 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStartFooTaskRequest(object):
+class RimeStartValidateModelTaskRequest(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'project_id': 'RimeUUID',
-        'req': 'FooexampleFooRequest',
+        'model_id': 'RimeUUID',
         'agent_id': 'RimeUUID'
     }
 
     attribute_map = {
         'project_id': 'projectId',
-        'req': 'req',
+        'model_id': 'modelId',
         'agent_id': 'agentId'
     }
 
-    def __init__(self, project_id=None, req=None, agent_id=None):  # noqa: E501
-        """RimeStartFooTaskRequest - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, project_id=None, model_id=None, agent_id=None):  # noqa: E501
+        """RimeStartValidateModelTaskRequest - a model defined in Swagger"""  # noqa: E501
         self._project_id = None
-        self._req = None
+        self._model_id = None
         self._agent_id = None
         self.discriminator = None
         if project_id is not None:
             self.project_id = project_id
-        if req is not None:
-            self.req = req
+        if model_id is not None:
+            self.model_id = model_id
         if agent_id is not None:
             self.agent_id = agent_id
 
     @property
     def project_id(self):
-        """Gets the project_id of this RimeStartFooTaskRequest.  # noqa: E501
+        """Gets the project_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
 
 
-        :return: The project_id of this RimeStartFooTaskRequest.  # noqa: E501
+        :return: The project_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._project_id
 
     @project_id.setter
     def project_id(self, project_id):
-        """Sets the project_id of this RimeStartFooTaskRequest.
+        """Sets the project_id of this RimeStartValidateModelTaskRequest.
 
 
-        :param project_id: The project_id of this RimeStartFooTaskRequest.  # noqa: E501
+        :param project_id: The project_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
         :type: RimeUUID
         """
 
         self._project_id = project_id
 
     @property
-    def req(self):
-        """Gets the req of this RimeStartFooTaskRequest.  # noqa: E501
+    def model_id(self):
+        """Gets the model_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
 
 
-        :return: The req of this RimeStartFooTaskRequest.  # noqa: E501
-        :rtype: FooexampleFooRequest
+        :return: The model_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
+        :rtype: RimeUUID
         """
-        return self._req
+        return self._model_id
 
-    @req.setter
-    def req(self, req):
-        """Sets the req of this RimeStartFooTaskRequest.
+    @model_id.setter
+    def model_id(self, model_id):
+        """Sets the model_id of this RimeStartValidateModelTaskRequest.
 
 
-        :param req: The req of this RimeStartFooTaskRequest.  # noqa: E501
-        :type: FooexampleFooRequest
+        :param model_id: The model_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
+        :type: RimeUUID
         """
 
-        self._req = req
+        self._model_id = model_id
 
     @property
     def agent_id(self):
-        """Gets the agent_id of this RimeStartFooTaskRequest.  # noqa: E501
+        """Gets the agent_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
 
 
-        :return: The agent_id of this RimeStartFooTaskRequest.  # noqa: E501
+        :return: The agent_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._agent_id
 
     @agent_id.setter
     def agent_id(self, agent_id):
-        """Sets the agent_id of this RimeStartFooTaskRequest.
+        """Sets the agent_id of this RimeStartValidateModelTaskRequest.
 
 
-        :param agent_id: The agent_id of this RimeStartFooTaskRequest.  # noqa: E501
+        :param agent_id: The agent_id of this RimeStartValidateModelTaskRequest.  # noqa: E501
         :type: RimeUUID
         """
 
         self._agent_id = agent_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -132,15 +132,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStartFooTaskRequest, dict):
+        if issubclass(RimeStartValidateModelTaskRequest, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +148,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStartFooTaskRequest):
+        if not isinstance(other, RimeStartValidateModelTaskRequest):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStartFooTaskResponse(object):
+class RimeStartValidateDatasetTaskResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'job_id': 'jobId'
     }
 
     def __init__(self, job_id=None):  # noqa: E501
-        """RimeStartFooTaskResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeStartValidateDatasetTaskResponse - a model defined in Swagger"""  # noqa: E501
         self._job_id = None
         self.discriminator = None
         if job_id is not None:
             self.job_id = job_id
 
     @property
     def job_id(self):
-        """Gets the job_id of this RimeStartFooTaskResponse.  # noqa: E501
+        """Gets the job_id of this RimeStartValidateDatasetTaskResponse.  # noqa: E501
 
 
-        :return: The job_id of this RimeStartFooTaskResponse.  # noqa: E501
+        :return: The job_id of this RimeStartValidateDatasetTaskResponse.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._job_id
 
     @job_id.setter
     def job_id(self, job_id):
-        """Sets the job_id of this RimeStartFooTaskResponse.
+        """Sets the job_id of this RimeStartValidateDatasetTaskResponse.
 
 
-        :param job_id: The job_id of this RimeStartFooTaskResponse.  # noqa: E501
+        :param job_id: The job_id of this RimeStartValidateDatasetTaskResponse.  # noqa: E501
         :type: RimeUUID
         """
 
         self._job_id = job_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStartFooTaskResponse, dict):
+        if issubclass(RimeStartValidateDatasetTaskResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStartFooTaskResponse):
+        if not isinstance(other, RimeStartValidateDatasetTaskResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_tag.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,113 +11,120 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStartValidateDatasetTaskRequest(object):
+class RimeTag(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'project_id': 'RimeUUID',
-        'req': 'ValidationValidateDatasetRequest',
-        'agent_id': 'RimeUUID'
+        'name': 'str',
+        'creation_time': 'datetime',
+        'num_projects': 'str'
     }
 
     attribute_map = {
-        'project_id': 'projectId',
-        'req': 'req',
-        'agent_id': 'agentId'
+        'name': 'name',
+        'creation_time': 'creationTime',
+        'num_projects': 'numProjects'
     }
 
-    def __init__(self, project_id=None, req=None, agent_id=None):  # noqa: E501
-        """RimeStartValidateDatasetTaskRequest - a model defined in Swagger"""  # noqa: E501
-        self._project_id = None
-        self._req = None
-        self._agent_id = None
+    def __init__(self, name=None, creation_time=None, num_projects=None):  # noqa: E501
+        """RimeTag - a model defined in Swagger"""  # noqa: E501
+        self._name = None
+        self._creation_time = None
+        self._num_projects = None
         self.discriminator = None
-        if project_id is not None:
-            self.project_id = project_id
-        if req is not None:
-            self.req = req
-        if agent_id is not None:
-            self.agent_id = agent_id
+        self.name = name
+        if creation_time is not None:
+            self.creation_time = creation_time
+        if num_projects is not None:
+            self.num_projects = num_projects
 
     @property
-    def project_id(self):
-        """Gets the project_id of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
+    def name(self):
+        """Gets the name of this RimeTag.  # noqa: E501
 
+        Name of the Tag.  # noqa: E501
 
-        :return: The project_id of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The name of this RimeTag.  # noqa: E501
+        :rtype: str
         """
-        return self._project_id
+        return self._name
 
-    @project_id.setter
-    def project_id(self, project_id):
-        """Sets the project_id of this RimeStartValidateDatasetTaskRequest.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this RimeTag.
 
+        Name of the Tag.  # noqa: E501
 
-        :param project_id: The project_id of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
-        :type: RimeUUID
+        :param name: The name of this RimeTag.  # noqa: E501
+        :type: str
         """
+        if name is None:
+            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._project_id = project_id
+        self._name = name
 
     @property
-    def req(self):
-        """Gets the req of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
+    def creation_time(self):
+        """Gets the creation_time of this RimeTag.  # noqa: E501
 
+        Creation time of the Workspace.  # noqa: E501
 
-        :return: The req of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
-        :rtype: ValidationValidateDatasetRequest
+        :return: The creation_time of this RimeTag.  # noqa: E501
+        :rtype: datetime
         """
-        return self._req
+        return self._creation_time
 
-    @req.setter
-    def req(self, req):
-        """Sets the req of this RimeStartValidateDatasetTaskRequest.
+    @creation_time.setter
+    def creation_time(self, creation_time):
+        """Sets the creation_time of this RimeTag.
 
+        Creation time of the Workspace.  # noqa: E501
 
-        :param req: The req of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
-        :type: ValidationValidateDatasetRequest
+        :param creation_time: The creation_time of this RimeTag.  # noqa: E501
+        :type: datetime
         """
 
-        self._req = req
+        self._creation_time = creation_time
 
     @property
-    def agent_id(self):
-        """Gets the agent_id of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
+    def num_projects(self):
+        """Gets the num_projects of this RimeTag.  # noqa: E501
 
+        Number of Projects associated with the Workspace.  # noqa: E501
 
-        :return: The agent_id of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
-        :rtype: RimeUUID
+        :return: The num_projects of this RimeTag.  # noqa: E501
+        :rtype: str
         """
-        return self._agent_id
+        return self._num_projects
 
-    @agent_id.setter
-    def agent_id(self, agent_id):
-        """Sets the agent_id of this RimeStartValidateDatasetTaskRequest.
+    @num_projects.setter
+    def num_projects(self, num_projects):
+        """Sets the num_projects of this RimeTag.
 
+        Number of Projects associated with the Workspace.  # noqa: E501
 
-        :param agent_id: The agent_id of this RimeStartValidateDatasetTaskRequest.  # noqa: E501
-        :type: RimeUUID
+        :param num_projects: The num_projects of this RimeTag.  # noqa: E501
+        :type: str
         """
 
-        self._agent_id = agent_id
+        self._num_projects = num_projects
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -132,15 +139,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStartValidateDatasetTaskRequest, dict):
+        if issubclass(RimeTag, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -148,15 +155,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStartValidateDatasetTaskRequest):
+        if not isinstance(other, RimeTag):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStartValidateDatasetTaskResponse(object):
+class RimeStartValidateModelTaskResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'job_id': 'jobId'
     }
 
     def __init__(self, job_id=None):  # noqa: E501
-        """RimeStartValidateDatasetTaskResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeStartValidateModelTaskResponse - a model defined in Swagger"""  # noqa: E501
         self._job_id = None
         self.discriminator = None
         if job_id is not None:
             self.job_id = job_id
 
     @property
     def job_id(self):
-        """Gets the job_id of this RimeStartValidateDatasetTaskResponse.  # noqa: E501
+        """Gets the job_id of this RimeStartValidateModelTaskResponse.  # noqa: E501
 
 
-        :return: The job_id of this RimeStartValidateDatasetTaskResponse.  # noqa: E501
+        :return: The job_id of this RimeStartValidateModelTaskResponse.  # noqa: E501
         :rtype: RimeUUID
         """
         return self._job_id
 
     @job_id.setter
     def job_id(self, job_id):
-        """Sets the job_id of this RimeStartValidateDatasetTaskResponse.
+        """Sets the job_id of this RimeStartValidateModelTaskResponse.
 
 
-        :param job_id: The job_id of this RimeStartValidateDatasetTaskResponse.  # noqa: E501
+        :param job_id: The job_id of this RimeStartValidateModelTaskResponse.  # noqa: E501
         :type: RimeUUID
         """
 
         self._job_id = job_id
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStartValidateDatasetTaskResponse, dict):
+        if issubclass(RimeStartValidateModelTaskResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStartValidateDatasetTaskResponse):
+        if not isinstance(other, RimeStartValidateModelTaskResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,61 +11,41 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeStrList(object):
+class RimeTestType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
+    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'values': 'list[str]'
     }
 
     attribute_map = {
-        'values': 'values'
     }
 
-    def __init__(self, values=None):  # noqa: E501
-        """RimeStrList - a model defined in Swagger"""  # noqa: E501
-        self._values = None
+    def __init__(self):  # noqa: E501
+        """RimeTestType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
-        if values is not None:
-            self.values = values
-
-    @property
-    def values(self):
-        """Gets the values of this RimeStrList.  # noqa: E501
-
-
-        :return: The values of this RimeStrList.  # noqa: E501
-        :rtype: list[str]
-        """
-        return self._values
-
-    @values.setter
-    def values(self, values):
-        """Sets the values of this RimeStrList.
-
-
-        :param values: The values of this RimeStrList.  # noqa: E501
-        :type: list[str]
-        """
-
-        self._values = values
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeStrList, dict):
+        if issubclass(RimeTestType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeStrList):
+        if not isinstance(other, RimeTestType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_tag.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files 21% similar despite different names*

```diff
@@ -11,120 +11,115 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTag(object):
+class RiskscoreRiskScore(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'name': 'str',
-        'creation_time': 'datetime',
-        'num_projects': 'str'
+        'type': 'RiskscoreRiskCategoryType',
+        'severity': 'RimeSeverity',
+        'score': 'float'
     }
 
     attribute_map = {
-        'name': 'name',
-        'creation_time': 'creationTime',
-        'num_projects': 'numProjects'
+        'type': 'type',
+        'severity': 'severity',
+        'score': 'score'
     }
 
-    def __init__(self, name=None, creation_time=None, num_projects=None):  # noqa: E501
-        """RimeTag - a model defined in Swagger"""  # noqa: E501
-        self._name = None
-        self._creation_time = None
-        self._num_projects = None
+    def __init__(self, type=None, severity=None, score=None):  # noqa: E501
+        """RiskscoreRiskScore - a model defined in Swagger"""  # noqa: E501
+        self._type = None
+        self._severity = None
+        self._score = None
         self.discriminator = None
-        self.name = name
-        if creation_time is not None:
-            self.creation_time = creation_time
-        if num_projects is not None:
-            self.num_projects = num_projects
+        if type is not None:
+            self.type = type
+        if severity is not None:
+            self.severity = severity
+        if score is not None:
+            self.score = score
 
     @property
-    def name(self):
-        """Gets the name of this RimeTag.  # noqa: E501
+    def type(self):
+        """Gets the type of this RiskscoreRiskScore.  # noqa: E501
 
-        Name of the Tag.  # noqa: E501
 
-        :return: The name of this RimeTag.  # noqa: E501
-        :rtype: str
+        :return: The type of this RiskscoreRiskScore.  # noqa: E501
+        :rtype: RiskscoreRiskCategoryType
         """
-        return self._name
+        return self._type
 
-    @name.setter
-    def name(self, name):
-        """Sets the name of this RimeTag.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this RiskscoreRiskScore.
 
-        Name of the Tag.  # noqa: E501
 
-        :param name: The name of this RimeTag.  # noqa: E501
-        :type: str
+        :param type: The type of this RiskscoreRiskScore.  # noqa: E501
+        :type: RiskscoreRiskCategoryType
         """
-        if name is None:
-            raise ValueError("Invalid value for `name`, must not be `None`")  # noqa: E501
 
-        self._name = name
+        self._type = type
 
     @property
-    def creation_time(self):
-        """Gets the creation_time of this RimeTag.  # noqa: E501
+    def severity(self):
+        """Gets the severity of this RiskscoreRiskScore.  # noqa: E501
 
-        Creation time of the Workspace.  # noqa: E501
 
-        :return: The creation_time of this RimeTag.  # noqa: E501
-        :rtype: datetime
+        :return: The severity of this RiskscoreRiskScore.  # noqa: E501
+        :rtype: RimeSeverity
         """
-        return self._creation_time
+        return self._severity
 
-    @creation_time.setter
-    def creation_time(self, creation_time):
-        """Sets the creation_time of this RimeTag.
+    @severity.setter
+    def severity(self, severity):
+        """Sets the severity of this RiskscoreRiskScore.
 
-        Creation time of the Workspace.  # noqa: E501
 
-        :param creation_time: The creation_time of this RimeTag.  # noqa: E501
-        :type: datetime
+        :param severity: The severity of this RiskscoreRiskScore.  # noqa: E501
+        :type: RimeSeverity
         """
 
-        self._creation_time = creation_time
+        self._severity = severity
 
     @property
-    def num_projects(self):
-        """Gets the num_projects of this RimeTag.  # noqa: E501
+    def score(self):
+        """Gets the score of this RiskscoreRiskScore.  # noqa: E501
 
-        Number of Projects associated with the Workspace.  # noqa: E501
+        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
 
-        :return: The num_projects of this RimeTag.  # noqa: E501
-        :rtype: str
+        :return: The score of this RiskscoreRiskScore.  # noqa: E501
+        :rtype: float
         """
-        return self._num_projects
+        return self._score
 
-    @num_projects.setter
-    def num_projects(self, num_projects):
-        """Sets the num_projects of this RimeTag.
+    @score.setter
+    def score(self, score):
+        """Sets the score of this RiskscoreRiskScore.
 
-        Number of Projects associated with the Workspace.  # noqa: E501
+        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
 
-        :param num_projects: The num_projects of this RimeTag.  # noqa: E501
-        :type: str
+        :param score: The score of this RiskscoreRiskScore.  # noqa: E501
+        :type: float
         """
 
-        self._num_projects = num_projects
+        self._score = score
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -139,15 +134,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTag, dict):
+        if issubclass(RiskscoreRiskScore, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -155,15 +150,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTag):
+        if not isinstance(other, RiskscoreRiskScore):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,42 +11,34 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTestCaseStatus(object):
+class RimeUpdateBuildInfoResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    PASS_UNSPECIFIED = "TEST_CASE_STATUS_PASS_UNSPECIFIED"
-    WARNING = "TEST_CASE_STATUS_WARNING"
-    FAIL = "TEST_CASE_STATUS_FAIL"
-    SKIP = "TEST_CASE_STATUS_SKIP"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTestCaseStatus - a model defined in Swagger"""  # noqa: E501
+        """RimeUpdateBuildInfoResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTestCaseStatus, dict):
+        if issubclass(RimeUpdateBuildInfoResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTestCaseStatus):
+        if not isinstance(other, RimeUpdateBuildInfoResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,40 +11,40 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTestType(object):
+class RegistryDataType(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    STRESS_TESTING_UNSPECIFIED = "TEST_TYPE_STRESS_TESTING_UNSPECIFIED"
-    CONTINUOUS_TESTING = "TEST_TYPE_CONTINUOUS_TESTING"
+    UNSPECIFIED = "DATA_TYPE_UNSPECIFIED"
+    DELTA_TABLE = "DATA_TYPE_DELTA_TABLE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTestType - a model defined in Swagger"""  # noqa: E501
+        """RegistryDataType - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -60,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTestType, dict):
+        if issubclass(RegistryDataType, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -76,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTestType):
+        if not isinstance(other, RegistryDataType):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,41 +11,34 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeTokenType(object):
+class RimeUpsertFeatureFlagsResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "TOKEN_TYPE_UNSPECIFIED"
-    USER = "TOKEN_TYPE_USER"
-    AGENT = "TOKEN_TYPE_AGENT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeTokenType - a model defined in Swagger"""  # noqa: E501
+        """RimeUpsertFeatureFlagsResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -61,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeTokenType, dict):
+        if issubclass(RimeUpsertFeatureFlagsResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -77,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeTokenType):
+        if not isinstance(other, RimeUpsertFeatureFlagsResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,34 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateBuildInfoResponse(object):
+class UserRole(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "ROLE_UNSPECIFIED"
+    ADMIN = "ROLE_ADMIN"
+    TRIAL_USER = "ROLE_TRIAL_USER"
+    SUPPORT = "ROLE_SUPPORT"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateBuildInfoResponse - a model defined in Swagger"""  # noqa: E501
+        """UserRole - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateBuildInfoResponse, dict):
+        if issubclass(UserRole, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateBuildInfoResponse):
+        if not isinstance(other, UserRole):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_update_workspace_tag_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpdateWorkspaceTagResponse(object):
+class RimeValidateTestConfigResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpdateWorkspaceTagResponse - a model defined in Swagger"""  # noqa: E501
+        """RimeValidateTestConfigResponse - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpdateWorkspaceTagResponse, dict):
+        if issubclass(RimeValidateTestConfigResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpdateWorkspaceTagResponse):
+        if not isinstance(other, RimeValidateTestConfigResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,34 +11,42 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeUpsertFeatureFlagsResponse(object):
+class TestrunTestSensitivity(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
+    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
+    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
+    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeUpsertFeatureFlagsResponse - a model defined in Swagger"""  # noqa: E501
+        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +62,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeUpsertFeatureFlagsResponse, dict):
+        if issubclass(TestrunTestSensitivity, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +78,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeUpsertFeatureFlagsResponse):
+        if not isinstance(other, TestrunTestSensitivity):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,34 +11,45 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RimeValidateTestConfigResponse(object):
+class StatedbJobStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
+
+    """
+    allowed enum values
+    """
+    UNSPECIFIED = "JOB_STATUS_UNSPECIFIED"
+    PENDING = "JOB_STATUS_PENDING"
+    RUNNING = "JOB_STATUS_RUNNING"
+    FAILED = "JOB_STATUS_FAILED"
+    SUCCEEDED = "JOB_STATUS_SUCCEEDED"
+    REQUESTED = "JOB_STATUS_REQUESTED"
+    CANCELLED = "JOB_STATUS_CANCELLED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """RimeValidateTestConfigResponse - a model defined in Swagger"""  # noqa: E501
+        """StatedbJobStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +65,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RimeValidateTestConfigResponse, dict):
+        if issubclass(StatedbJobStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +81,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RimeValidateTestConfigResponse):
+        if not isinstance(other, StatedbJobStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,115 +11,89 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class RiskscoreRiskScore(object):
+class V1projectsprojectIdUuidroleusersuserUserIdUuidUser(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'type': 'RiskscoreRiskCategoryType',
-        'severity': 'RimeSeverity',
-        'score': 'float'
+        'user_id': 'object',
+        'user_role': 'RimeActorRole'
     }
 
     attribute_map = {
-        'type': 'type',
-        'severity': 'severity',
-        'score': 'score'
+        'user_id': 'userId',
+        'user_role': 'userRole'
     }
 
-    def __init__(self, type=None, severity=None, score=None):  # noqa: E501
-        """RiskscoreRiskScore - a model defined in Swagger"""  # noqa: E501
-        self._type = None
-        self._severity = None
-        self._score = None
+    def __init__(self, user_id=None, user_role=None):  # noqa: E501
+        """V1projectsprojectIdUuidroleusersuserUserIdUuidUser - a model defined in Swagger"""  # noqa: E501
+        self._user_id = None
+        self._user_role = None
         self.discriminator = None
-        if type is not None:
-            self.type = type
-        if severity is not None:
-            self.severity = severity
-        if score is not None:
-            self.score = score
+        if user_id is not None:
+            self.user_id = user_id
+        if user_role is not None:
+            self.user_role = user_role
 
     @property
-    def type(self):
-        """Gets the type of this RiskscoreRiskScore.  # noqa: E501
+    def user_id(self):
+        """Gets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :return: The type of this RiskscoreRiskScore.  # noqa: E501
-        :rtype: RiskscoreRiskCategoryType
+        :return: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: object
         """
-        return self._type
+        return self._user_id
 
-    @type.setter
-    def type(self, type):
-        """Sets the type of this RiskscoreRiskScore.
+    @user_id.setter
+    def user_id(self, user_id):
+        """Sets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
+        Unique ID of an object in RIME.  # noqa: E501
 
-        :param type: The type of this RiskscoreRiskScore.  # noqa: E501
-        :type: RiskscoreRiskCategoryType
+        :param user_id: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: object
         """
 
-        self._type = type
+        self._user_id = user_id
 
     @property
-    def severity(self):
-        """Gets the severity of this RiskscoreRiskScore.  # noqa: E501
+    def user_role(self):
+        """Gets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
 
 
-        :return: The severity of this RiskscoreRiskScore.  # noqa: E501
-        :rtype: RimeSeverity
+        :return: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :rtype: RimeActorRole
         """
-        return self._severity
+        return self._user_role
 
-    @severity.setter
-    def severity(self, severity):
-        """Sets the severity of this RiskscoreRiskScore.
+    @user_role.setter
+    def user_role(self, user_role):
+        """Sets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
 
 
-        :param severity: The severity of this RiskscoreRiskScore.  # noqa: E501
-        :type: RimeSeverity
+        :param user_role: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+        :type: RimeActorRole
         """
 
-        self._severity = severity
-
-    @property
-    def score(self):
-        """Gets the score of this RiskscoreRiskScore.  # noqa: E501
-
-        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
-
-        :return: The score of this RiskscoreRiskScore.  # noqa: E501
-        :rtype: float
-        """
-        return self._score
-
-    @score.setter
-    def score(self, score):
-        """Sets the score of this RiskscoreRiskScore.
-
-        A risk score is a value between 0 and 1, where 0 is the lowest risk and 1 is the highest risk.  # noqa: E501
-
-        :param score: The score of this RiskscoreRiskScore.  # noqa: E501
-        :type: float
-        """
-
-        self._score = score
+        self._user_role = user_role
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -134,15 +108,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(RiskscoreRiskScore, dict):
+        if issubclass(V1projectsprojectIdUuidroleusersuserUserIdUuidUser, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -150,15 +124,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, RiskscoreRiskScore):
+        if not isinstance(other, V1projectsprojectIdUuidroleusersuserUserIdUuidUser):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,46 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class StatedbJobStatus(object):
+class TestrunresultGetTestRunResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
-
-    """
-    allowed enum values
-    """
-    UNSPECIFIED = "JOB_STATUS_UNSPECIFIED"
-    PENDING = "JOB_STATUS_PENDING"
-    RUNNING = "JOB_STATUS_RUNNING"
-    FAILED = "JOB_STATUS_FAILED"
-    SUCCEEDED = "JOB_STATUS_SUCCEEDED"
-    REQUESTED = "JOB_STATUS_REQUESTED"
-    CANCELLED = "JOB_STATUS_CANCELLED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'test_run': 'TestrunresultTestRunDetail'
     }
 
     attribute_map = {
+        'test_run': 'testRun'
     }
 
-    def __init__(self):  # noqa: E501
-        """StatedbJobStatus - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, test_run=None):  # noqa: E501
+        """TestrunresultGetTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        self._test_run = None
         self.discriminator = None
+        if test_run is not None:
+            self.test_run = test_run
+
+    @property
+    def test_run(self):
+        """Gets the test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+
+
+        :return: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :rtype: TestrunresultTestRunDetail
+        """
+        return self._test_run
+
+    @test_run.setter
+    def test_run(self, test_run):
+        """Sets the test_run of this TestrunresultGetTestRunResponse.
+
+
+        :param test_run: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :type: TestrunresultTestRunDetail
+        """
+
+        self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -65,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(StatedbJobStatus, dict):
+        if issubclass(TestrunresultGetTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -81,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, StatedbJobStatus):
+        if not isinstance(other, TestrunresultGetTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/tags_name_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/tags_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,67 +24,44 @@
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'category_id': 'str',
         'test_category': 'TestrunTestCategoryType',
+        'category_id': 'str',
         'name': 'str',
         'value': 'float'
     }
 
     attribute_map = {
-        'category_id': 'categoryId',
         'test_category': 'testCategory',
+        'category_id': 'categoryId',
         'name': 'name',
         'value': 'value'
     }
 
-    def __init__(self, category_id=None, test_category=None, name=None, value=None):  # noqa: E501
+    def __init__(self, test_category=None, category_id=None, name=None, value=None):  # noqa: E501
         """TestRunMetricsCategorySummaryMetric - a model defined in Swagger"""  # noqa: E501
-        self._category_id = None
         self._test_category = None
+        self._category_id = None
         self._name = None
         self._value = None
         self.discriminator = None
-        if category_id is not None:
-            self.category_id = category_id
         if test_category is not None:
             self.test_category = test_category
+        if category_id is not None:
+            self.category_id = category_id
         if name is not None:
             self.name = name
         if value is not None:
             self.value = value
 
     @property
-    def category_id(self):
-        """Gets the category_id of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
-
-        Uniquely specifies a Category.  # noqa: E501
-
-        :return: The category_id of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
-        :rtype: str
-        """
-        return self._category_id
-
-    @category_id.setter
-    def category_id(self, category_id):
-        """Sets the category_id of this TestRunMetricsCategorySummaryMetric.
-
-        Uniquely specifies a Category.  # noqa: E501
-
-        :param category_id: The category_id of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
-        :type: str
-        """
-
-        self._category_id = category_id
-
-    @property
     def test_category(self):
         """Gets the test_category of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
 
 
         :return: The test_category of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
         :rtype: TestrunTestCategoryType
         """
@@ -98,14 +75,37 @@
         :param test_category: The test_category of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
         :type: TestrunTestCategoryType
         """
 
         self._test_category = test_category
 
     @property
+    def category_id(self):
+        """Gets the category_id of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
+
+        The string field `category` is deprecated in v2.1 and will be removed in v2.3. Please use the enum field test_category instead, which provides the same info.  # noqa: E501
+
+        :return: The category_id of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
+        :rtype: str
+        """
+        return self._category_id
+
+    @category_id.setter
+    def category_id(self, category_id):
+        """Sets the category_id of this TestRunMetricsCategorySummaryMetric.
+
+        The string field `category` is deprecated in v2.1 and will be removed in v2.3. Please use the enum field test_category instead, which provides the same info.  # noqa: E501
+
+        :param category_id: The category_id of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
+        :type: str
+        """
+
+        self._category_id = category_id
+
+    @property
     def name(self):
         """Gets the name of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
 
         The name of the category.  # noqa: E501
 
         :return: The name of this TestRunMetricsCategorySummaryMetric.  # noqa: E501
         :rtype: str
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_generative_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,16 @@
     MODEL_PERFORMANCE = "TEST_CATEGORY_TYPE_MODEL_PERFORMANCE"
     DATA_POISONING_DETECTION = "TEST_CATEGORY_TYPE_DATA_POISONING_DETECTION"
     SUBSET_PERFORMANCE = "TEST_CATEGORY_TYPE_SUBSET_PERFORMANCE"
     SUBSET_PERFORMANCE_DEGRADATION = "TEST_CATEGORY_TYPE_SUBSET_PERFORMANCE_DEGRADATION"
     TRANSFORMATIONS = "TEST_CATEGORY_TYPE_TRANSFORMATIONS"
     EVASION_ATTACK_DETECTION = "TEST_CATEGORY_TYPE_EVASION_ATTACK_DETECTION"
     CUSTOM = "TEST_CATEGORY_TYPE_CUSTOM"
+    MODEL_ALIGNMENT = "TEST_CATEGORY_TYPE_MODEL_ALIGNMENT"
+    FACTUAL_AWARENESS = "TEST_CATEGORY_TYPE_FACTUAL_AWARENESS"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,42 +11,41 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunTestSensitivity(object):
+class CustomermanagedkeyKeyStatus(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "TEST_SENSITIVITY_UNSPECIFIED"
-    LESS_SENSITIVE = "TEST_SENSITIVITY_LESS_SENSITIVE"
-    DEFAULT = "TEST_SENSITIVITY_DEFAULT"
-    MORE_SENSITIVE = "TEST_SENSITIVITY_MORE_SENSITIVE"
+    UNSPECIFIED = "KEY_STATUS_UNSPECIFIED"
+    ACTIVE = "KEY_STATUS_ACTIVE"
+    REVOKED = "KEY_STATUS_REVOKED"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """TestrunTestSensitivity - a model defined in Swagger"""  # noqa: E501
+        """CustomermanagedkeyKeyStatus - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +61,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunTestSensitivity, dict):
+        if issubclass(CustomermanagedkeyKeyStatus, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +77,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunTestSensitivity):
+        if not isinstance(other, CustomermanagedkeyKeyStatus):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultGetTestRunResponse(object):
+class TestrunresultRenameTestRunResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -32,36 +32,36 @@
     }
 
     attribute_map = {
         'test_run': 'testRun'
     }
 
     def __init__(self, test_run=None):  # noqa: E501
-        """TestrunresultGetTestRunResponse - a model defined in Swagger"""  # noqa: E501
+        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
         self._test_run = None
         self.discriminator = None
         if test_run is not None:
             self.test_run = test_run
 
     @property
     def test_run(self):
-        """Gets the test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
 
 
-        :return: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
         :rtype: TestrunresultTestRunDetail
         """
         return self._test_run
 
     @test_run.setter
     def test_run(self, test_run):
-        """Sets the test_run of this TestrunresultGetTestRunResponse.
+        """Sets the test_run of this TestrunresultRenameTestRunResponse.
 
 
-        :param test_run: The test_run of this TestrunresultGetTestRunResponse.  # noqa: E501
+        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
         :type: TestrunresultTestRunDetail
         """
 
         self._test_run = test_run
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultGetTestRunResponse, dict):
+        if issubclass(TestrunresultRenameTestRunResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultGetTestRunResponse):
+        if not isinstance(other, TestrunresultRenameTestRunResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,61 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TestrunresultRenameTestRunResponse(object):
+class UserPrivateInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'test_run': 'TestrunresultTestRunDetail'
+        'favorite_projects': 'list[UserFavoriteProjects]'
     }
 
     attribute_map = {
-        'test_run': 'testRun'
+        'favorite_projects': 'favoriteProjects'
     }
 
-    def __init__(self, test_run=None):  # noqa: E501
-        """TestrunresultRenameTestRunResponse - a model defined in Swagger"""  # noqa: E501
-        self._test_run = None
+    def __init__(self, favorite_projects=None):  # noqa: E501
+        """UserPrivateInfo - a model defined in Swagger"""  # noqa: E501
+        self._favorite_projects = None
         self.discriminator = None
-        if test_run is not None:
-            self.test_run = test_run
+        if favorite_projects is not None:
+            self.favorite_projects = favorite_projects
 
     @property
-    def test_run(self):
-        """Gets the test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
+    def favorite_projects(self):
+        """Gets the favorite_projects of this UserPrivateInfo.  # noqa: E501
 
 
-        :return: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :rtype: TestrunresultTestRunDetail
+        :return: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :rtype: list[UserFavoriteProjects]
         """
-        return self._test_run
+        return self._favorite_projects
 
-    @test_run.setter
-    def test_run(self, test_run):
-        """Sets the test_run of this TestrunresultRenameTestRunResponse.
+    @favorite_projects.setter
+    def favorite_projects(self, favorite_projects):
+        """Sets the favorite_projects of this UserPrivateInfo.
 
 
-        :param test_run: The test_run of this TestrunresultRenameTestRunResponse.  # noqa: E501
-        :type: TestrunresultTestRunDetail
+        :param favorite_projects: The favorite_projects of this UserPrivateInfo.  # noqa: E501
+        :type: list[UserFavoriteProjects]
         """
 
-        self._test_run = test_run
+        self._favorite_projects = favorite_projects
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -80,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TestrunresultRenameTestRunResponse, dict):
+        if issubclass(UserPrivateInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -96,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TestrunresultRenameTestRunResponse):
+        if not isinstance(other, UserPrivateInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'test_run_id': 'str',
         'test_type': 'str',
         'test_name': 'str',
         'description': 'str',
+        'test_category': 'TestrunTestCategoryType',
         'category': 'str',
         'duration_in_millis': 'str',
         'severity': 'RimeSeverity',
         'summary_counts': 'TestrunresultResultSummaryCounts',
         'failing_features': 'list[str]',
         'metrics': 'list[RimeTestMetric]',
         'show_in_test_comparisons': 'bool',
@@ -45,32 +46,34 @@
     }
 
     attribute_map = {
         'test_run_id': 'testRunId',
         'test_type': 'testType',
         'test_name': 'testName',
         'description': 'description',
+        'test_category': 'testCategory',
         'category': 'category',
         'duration_in_millis': 'durationInMillis',
         'severity': 'severity',
         'summary_counts': 'summaryCounts',
         'failing_features': 'failingFeatures',
         'metrics': 'metrics',
         'show_in_test_comparisons': 'showInTestComparisons',
         'display': 'display',
         'failing_rows_result': 'failingRowsResult',
         'security_test_details': 'securityTestDetails'
     }
 
-    def __init__(self, test_run_id=None, test_type=None, test_name=None, description=None, category=None, duration_in_millis=None, severity=None, summary_counts=None, failing_features=None, metrics=None, show_in_test_comparisons=None, display=None, failing_rows_result=None, security_test_details=None):  # noqa: E501
+    def __init__(self, test_run_id=None, test_type=None, test_name=None, description=None, test_category=None, category=None, duration_in_millis=None, severity=None, summary_counts=None, failing_features=None, metrics=None, show_in_test_comparisons=None, display=None, failing_rows_result=None, security_test_details=None):  # noqa: E501
         """TestrunresultTestBatchResult - a model defined in Swagger"""  # noqa: E501
         self._test_run_id = None
         self._test_type = None
         self._test_name = None
         self._description = None
+        self._test_category = None
         self._category = None
         self._duration_in_millis = None
         self._severity = None
         self._summary_counts = None
         self._failing_features = None
         self._metrics = None
         self._show_in_test_comparisons = None
@@ -82,14 +85,16 @@
             self.test_run_id = test_run_id
         if test_type is not None:
             self.test_type = test_type
         if test_name is not None:
             self.test_name = test_name
         if description is not None:
             self.description = description
+        if test_category is not None:
+            self.test_category = test_category
         if category is not None:
             self.category = category
         if duration_in_millis is not None:
             self.duration_in_millis = duration_in_millis
         if severity is not None:
             self.severity = severity
         if summary_counts is not None:
@@ -194,27 +199,50 @@
         :param description: The description of this TestrunresultTestBatchResult.  # noqa: E501
         :type: str
         """
 
         self._description = description
 
     @property
+    def test_category(self):
+        """Gets the test_category of this TestrunresultTestBatchResult.  # noqa: E501
+
+
+        :return: The test_category of this TestrunresultTestBatchResult.  # noqa: E501
+        :rtype: TestrunTestCategoryType
+        """
+        return self._test_category
+
+    @test_category.setter
+    def test_category(self, test_category):
+        """Sets the test_category of this TestrunresultTestBatchResult.
+
+
+        :param test_category: The test_category of this TestrunresultTestBatchResult.  # noqa: E501
+        :type: TestrunTestCategoryType
+        """
+
+        self._test_category = test_category
+
+    @property
     def category(self):
         """Gets the category of this TestrunresultTestBatchResult.  # noqa: E501
 
+        The string field `category` is deprecated in v2.1 and will be removed in v2.3. Please use the enum field test_category instead, which provides the same info.  # noqa: E501
 
         :return: The category of this TestrunresultTestBatchResult.  # noqa: E501
         :rtype: str
         """
         return self._category
 
     @category.setter
     def category(self, category):
         """Sets the category of this TestrunresultTestBatchResult.
 
+        The string field `category` is deprecated in v2.1 and will be removed in v2.3. Please use the enum field test_category instead, which provides the same info.  # noqa: E501
 
         :param category: The category of this TestrunresultTestBatchResult.  # noqa: E501
         :type: str
         """
 
         self._category = category
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,47 +30,47 @@
     swagger_types = {
         'test_run_id': 'str',
         'features': 'list[str]',
         'test_batch_type': 'str',
         'status': 'RimeTestCaseStatus',
         'severity': 'RimeSeverity',
         'importance_score': 'float',
-        'category': 'str',
         'test_category': 'TestrunTestCategoryType',
+        'category': 'str',
         'metrics': 'list[RimeTestMetric]',
         'url_safe_feature_id': 'str',
         'test_case_id': 'str',
         'display': 'TestrunresultTestCaseDisplay'
     }
 
     attribute_map = {
         'test_run_id': 'testRunId',
         'features': 'features',
         'test_batch_type': 'testBatchType',
         'status': 'status',
         'severity': 'severity',
         'importance_score': 'importanceScore',
-        'category': 'category',
         'test_category': 'testCategory',
+        'category': 'category',
         'metrics': 'metrics',
         'url_safe_feature_id': 'urlSafeFeatureId',
         'test_case_id': 'testCaseId',
         'display': 'display'
     }
 
-    def __init__(self, test_run_id=None, features=None, test_batch_type=None, status=None, severity=None, importance_score=None, category=None, test_category=None, metrics=None, url_safe_feature_id=None, test_case_id=None, display=None):  # noqa: E501
+    def __init__(self, test_run_id=None, features=None, test_batch_type=None, status=None, severity=None, importance_score=None, test_category=None, category=None, metrics=None, url_safe_feature_id=None, test_case_id=None, display=None):  # noqa: E501
         """TestrunresultTestCase - a model defined in Swagger"""  # noqa: E501
         self._test_run_id = None
         self._features = None
         self._test_batch_type = None
         self._status = None
         self._severity = None
         self._importance_score = None
-        self._category = None
         self._test_category = None
+        self._category = None
         self._metrics = None
         self._url_safe_feature_id = None
         self._test_case_id = None
         self._display = None
         self.discriminator = None
         if test_run_id is not None:
             self.test_run_id = test_run_id
@@ -80,18 +80,18 @@
             self.test_batch_type = test_batch_type
         if status is not None:
             self.status = status
         if severity is not None:
             self.severity = severity
         if importance_score is not None:
             self.importance_score = importance_score
-        if category is not None:
-            self.category = category
         if test_category is not None:
             self.test_category = test_category
+        if category is not None:
+            self.category = category
         if metrics is not None:
             self.metrics = metrics
         if url_safe_feature_id is not None:
             self.url_safe_feature_id = url_safe_feature_id
         if test_case_id is not None:
             self.test_case_id = test_case_id
         if display is not None:
@@ -228,35 +228,14 @@
         :param importance_score: The importance_score of this TestrunresultTestCase.  # noqa: E501
         :type: float
         """
 
         self._importance_score = importance_score
 
     @property
-    def category(self):
-        """Gets the category of this TestrunresultTestCase.  # noqa: E501
-
-
-        :return: The category of this TestrunresultTestCase.  # noqa: E501
-        :rtype: str
-        """
-        return self._category
-
-    @category.setter
-    def category(self, category):
-        """Sets the category of this TestrunresultTestCase.
-
-
-        :param category: The category of this TestrunresultTestCase.  # noqa: E501
-        :type: str
-        """
-
-        self._category = category
-
-    @property
     def test_category(self):
         """Gets the test_category of this TestrunresultTestCase.  # noqa: E501
 
 
         :return: The test_category of this TestrunresultTestCase.  # noqa: E501
         :rtype: TestrunTestCategoryType
         """
@@ -270,14 +249,37 @@
         :param test_category: The test_category of this TestrunresultTestCase.  # noqa: E501
         :type: TestrunTestCategoryType
         """
 
         self._test_category = test_category
 
     @property
+    def category(self):
+        """Gets the category of this TestrunresultTestCase.  # noqa: E501
+
+        The string field `category` is deprecated in v2.1 and will be removed in v2.3. Please use the enum field test_category instead, which provides the same info.  # noqa: E501
+
+        :return: The category of this TestrunresultTestCase.  # noqa: E501
+        :rtype: str
+        """
+        return self._category
+
+    @category.setter
+    def category(self, category):
+        """Sets the category of this TestrunresultTestCase.
+
+        The string field `category` is deprecated in v2.1 and will be removed in v2.3. Please use the enum field test_category instead, which provides the same info.  # noqa: E501
+
+        :param category: The category of this TestrunresultTestCase.  # noqa: E501
+        :type: str
+        """
+
+        self._category = category
+
+    @property
     def metrics(self):
         """Gets the metrics of this TestrunresultTestCase.  # noqa: E501
 
 
         :return: The metrics of this TestrunresultTestCase.  # noqa: E501
         :rtype: list[RimeTestMetric]
         """
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/the_updates_to_the_monitor_.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,42 +11,40 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class UserRole(object):
+class CustomermanagedkeyKeyProvider(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
 
     """
     allowed enum values
     """
-    UNSPECIFIED = "ROLE_UNSPECIFIED"
-    ADMIN = "ROLE_ADMIN"
-    TRIAL_USER = "ROLE_TRIAL_USER"
-    SUPPORT = "ROLE_SUPPORT"
+    UNSPECIFIED = "KEY_PROVIDER_UNSPECIFIED"
+    AWS_KMS = "KEY_PROVIDER_AWS_KMS"
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """UserRole - a model defined in Swagger"""  # noqa: E501
+        """CustomermanagedkeyKeyProvider - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -62,15 +60,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(UserRole, dict):
+        if issubclass(CustomermanagedkeyKeyProvider, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -78,15 +76,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, UserRole):
+        if not isinstance(other, CustomermanagedkeyKeyProvider):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,89 +11,90 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class V1projectsprojectIdUuidroleusersuserUserIdUuidUser(object):
+class RegistryDataFileInfo(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'user_id': 'object',
-        'user_role': 'RimeActorRole'
+        'path': 'str',
+        'data_type': 'RegistryDataType'
     }
 
     attribute_map = {
-        'user_id': 'userId',
-        'user_role': 'userRole'
+        'path': 'path',
+        'data_type': 'dataType'
     }
 
-    def __init__(self, user_id=None, user_role=None):  # noqa: E501
-        """V1projectsprojectIdUuidroleusersuserUserIdUuidUser - a model defined in Swagger"""  # noqa: E501
-        self._user_id = None
-        self._user_role = None
+    def __init__(self, path=None, data_type=None):  # noqa: E501
+        """RegistryDataFileInfo - a model defined in Swagger"""  # noqa: E501
+        self._path = None
+        self._data_type = None
         self.discriminator = None
-        if user_id is not None:
-            self.user_id = user_id
-        if user_role is not None:
-            self.user_role = user_role
+        self.path = path
+        if data_type is not None:
+            self.data_type = data_type
 
     @property
-    def user_id(self):
-        """Gets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+    def path(self):
+        """Gets the path of this RegistryDataFileInfo.  # noqa: E501
 
-        Unique ID of an object in RIME.  # noqa: E501
+        The path to the data file.  # noqa: E501
 
-        :return: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
-        :rtype: object
+        :return: The path of this RegistryDataFileInfo.  # noqa: E501
+        :rtype: str
         """
-        return self._user_id
+        return self._path
 
-    @user_id.setter
-    def user_id(self, user_id):
-        """Sets the user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this RegistryDataFileInfo.
 
-        Unique ID of an object in RIME.  # noqa: E501
+        The path to the data file.  # noqa: E501
 
-        :param user_id: The user_id of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
-        :type: object
+        :param path: The path of this RegistryDataFileInfo.  # noqa: E501
+        :type: str
         """
+        if path is None:
+            raise ValueError("Invalid value for `path`, must not be `None`")  # noqa: E501
 
-        self._user_id = user_id
+        self._path = path
 
     @property
-    def user_role(self):
-        """Gets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
+    def data_type(self):
+        """Gets the data_type of this RegistryDataFileInfo.  # noqa: E501
 
 
-        :return: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
-        :rtype: RimeActorRole
+        :return: The data_type of this RegistryDataFileInfo.  # noqa: E501
+        :rtype: RegistryDataType
         """
-        return self._user_role
+        return self._data_type
 
-    @user_role.setter
-    def user_role(self, user_role):
-        """Sets the user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.
+    @data_type.setter
+    def data_type(self, data_type):
+        """Sets the data_type of this RegistryDataFileInfo.
 
 
-        :param user_role: The user_role of this V1projectsprojectIdUuidroleusersuserUserIdUuidUser.  # noqa: E501
-        :type: RimeActorRole
+        :param data_type: The data_type of this RegistryDataFileInfo.  # noqa: E501
+        :type: RegistryDataType
         """
 
-        self._user_role = user_role
+        self._data_type = data_type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -108,15 +109,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(V1projectsprojectIdUuidroleusersuserUserIdUuidUser, dict):
+        if issubclass(RegistryDataFileInfo, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -124,15 +125,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, V1projectsprojectIdUuidroleusersuserUserIdUuidUser):
+        if not isinstance(other, RegistryDataFileInfo):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_request.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,35 +11,61 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class ValidationValidateDatasetRequest(object):
+class RimeGetKeyStatusResponse(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
+        'status': 'CustomermanagedkeyKeyStatus'
     }
 
     attribute_map = {
+        'status': 'status'
     }
 
-    def __init__(self):  # noqa: E501
-        """ValidationValidateDatasetRequest - a model defined in Swagger"""  # noqa: E501
+    def __init__(self, status=None):  # noqa: E501
+        """RimeGetKeyStatusResponse - a model defined in Swagger"""  # noqa: E501
+        self._status = None
         self.discriminator = None
+        if status is not None:
+            self.status = status
+
+    @property
+    def status(self):
+        """Gets the status of this RimeGetKeyStatusResponse.  # noqa: E501
+
+
+        :return: The status of this RimeGetKeyStatusResponse.  # noqa: E501
+        :rtype: CustomermanagedkeyKeyStatus
+        """
+        return self._status
+
+    @status.setter
+    def status(self, status):
+        """Sets the status of this RimeGetKeyStatusResponse.
+
+
+        :param status: The status of this RimeGetKeyStatusResponse.  # noqa: E501
+        :type: CustomermanagedkeyKeyStatus
+        """
+
+        self._status = status
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -54,15 +80,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(ValidationValidateDatasetRequest, dict):
+        if issubclass(RimeGetKeyStatusResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +96,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ValidationValidateDatasetRequest):
+        if not isinstance(other, RimeGetKeyStatusResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.1.0rc6/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/test_batch.py` & `rime_sdk-2.1.0rc6/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk/test_run.py` & `rime_sdk-2.1.0rc6/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.1.0rc5/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.1.0rc6/rime_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.1.0rc5
+Version: 2.1.0rc6
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.1.0rc5/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.1.0rc6/rime_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,21 @@
 rime_sdk/swagger/swagger_client/__init__.py
 rime_sdk/swagger/swagger_client/api_client.py
 rime_sdk/swagger/swagger_client/configuration.py
 rime_sdk/swagger/swagger_client/rest.py
 rime_sdk/swagger/swagger_client/api/__init__.py
 rime_sdk/swagger/swagger_client/api/agent_manager_api.py
 rime_sdk/swagger/swagger_client/api/config_validator_api.py
+rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
 rime_sdk/swagger/swagger_client/api/data_collector_api.py
 rime_sdk/swagger/swagger_client/api/detection_api.py
 rime_sdk/swagger/swagger_client/api/feature_flag_api.py
 rime_sdk/swagger/swagger_client/api/file_scanning_api.py
 rime_sdk/swagger/swagger_client/api/file_upload_api.py
 rime_sdk/swagger/swagger_client/api/firewall_service_api.py
-rime_sdk/swagger/swagger_client/api/foo_xp_interface_api.py
 rime_sdk/swagger/swagger_client/api/image_registry_api.py
 rime_sdk/swagger/swagger_client/api/integration_service_api.py
 rime_sdk/swagger/swagger_client/api/job_reader_api.py
 rime_sdk/swagger/swagger_client/api/model_card_service_api.py
 rime_sdk/swagger/swagger_client/api/model_testing_api.py
 rime_sdk/swagger/swagger_client/api/monitor_service_api.py
 rime_sdk/swagger/swagger_client/api/notification_setting_api.py
@@ -74,14 +74,17 @@
 rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
 rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
 rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
 rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
 rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
 rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
 rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
 rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
 rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
 rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
 rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
@@ -108,20 +111,17 @@
 rime_sdk/swagger/swagger_client/models/filescanning_security_report.py
 rime_sdk/swagger/swagger_client/models/filescanning_security_report_import_result.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall.py
 rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
 rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
 rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
-rime_sdk/swagger/swagger_client/models/fooexample_foo_request.py
-rime_sdk/swagger/swagger_client/models/fooexample_foo_response.py
 rime_sdk/swagger/swagger_client/models/generativestresstests_project_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/googlerpc_status.py
 rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
-rime_sdk/swagger/swagger_client/models/integration_integration.py
 rime_sdk/swagger/swagger_client/models/integration_integration_level.py
 rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
 rime_sdk/swagger/swagger_client/models/integration_integration_type.py
 rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
 rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
 rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
 rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
@@ -199,15 +199,16 @@
 rime_sdk/swagger/swagger_client/models/rca_test_case_id.py
 rime_sdk/swagger/swagger_client/models/registry_connection_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
 rime_sdk/swagger/swagger_client/models/registry_data_params.py
-rime_sdk/swagger/swagger_client/models/registry_delta_lake_info.py
+rime_sdk/swagger/swagger_client/models/registry_data_type.py
+rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
 rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_metadata.py
 rime_sdk/swagger/swagger_client/models/registry_model_info.py
 rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
 rime_sdk/swagger/swagger_client/models/registry_pred_info.py
 rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
@@ -229,14 +230,16 @@
 rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
 rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
 rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
 rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
@@ -263,39 +266,42 @@
 rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
 rime_sdk/swagger/swagger_client/models/rime_failing_row.py
 rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
 rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
 rime_sdk/swagger/swagger_client/models/rime_feature_type.py
 rime_sdk/swagger/swagger_client/models/rime_float_list.py
 rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
-rime_sdk/swagger/swagger_client/models/rime_get_foo_task_status_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
 rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
 rime_sdk/swagger/swagger_client/models/rime_image_reference.py
 rime_sdk/swagger/swagger_client/models/rime_int_list.py
 rime_sdk/swagger/swagger_client/models/rime_integration_info.py
 rime_sdk/swagger/swagger_client/models/rime_job_data.py
 rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
@@ -320,14 +326,15 @@
 rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
 rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_workspace_tags_response.py
 rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
@@ -340,14 +347,15 @@
 rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
 rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
 rime_sdk/swagger/swagger_client/models/rime_named_double.py
 rime_sdk/swagger/swagger_client/models/rime_order.py
 rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
 rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
 rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
 rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
 rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
 rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
 rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
 rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
@@ -356,20 +364,22 @@
 rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
 rime_sdk/swagger/swagger_client/models/rime_severity.py
 rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
 rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
 rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
 rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
-rime_sdk/swagger/swagger_client/models/rime_start_foo_task_request.py
-rime_sdk/swagger/swagger_client/models/rime_start_foo_task_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_generative_stress_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
 rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
 rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
 rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
 rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
 rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
 rime_sdk/swagger/swagger_client/models/rime_str_list.py
 rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
 rime_sdk/swagger/swagger_client/models/rime_subject_type.py
 rime_sdk/swagger/swagger_client/models/rime_suggestion.py
@@ -402,14 +412,15 @@
 rime_sdk/swagger/swagger_client/models/rime_user_role.py
 rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
 rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
 rime_sdk/swagger/swagger_client/models/rime_uuid.py
 rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
 rime_sdk/swagger/swagger_client/models/rime_workspace.py
 rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
 rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
 rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
 rime_sdk/swagger/swagger_client/models/role_users_body.py
 rime_sdk/swagger/swagger_client/models/role_workspace_body.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
 rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
@@ -471,12 +482,13 @@
 rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
 rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
 rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
 rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
 rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
 rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
-rime_sdk/swagger/swagger_client/models/validation_validate_dataset_request.py
 rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
 rime_sdk/swagger/swagger_client/models/workspace_id_uuid_tags_body.py
 rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
 rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
```

### Comparing `rime_sdk-2.1.0rc5/setup.py` & `rime_sdk-2.1.0rc6/setup.py`

 * *Files identical despite different names*

