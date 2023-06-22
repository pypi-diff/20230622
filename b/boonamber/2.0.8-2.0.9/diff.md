# Comparing `tmp/boonamber-2.0.8.tar.gz` & `tmp/boonamber-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boonamber-2.0.8.tar", last modified: Thu Jun  8 11:47:16 2023, max compression
+gzip compressed data, was "boonamber-2.0.9.tar", last modified: Thu Jun 22 21:09:15 2023, max compression
```

## Comparing `boonamber-2.0.8.tar` & `boonamber-2.0.9.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.619071 boonamber-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 11:47:05.000000 boonamber-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 11:47:16.619071 boonamber-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-08 11:47:05.000000 boonamber-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/util/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/util/ambererror.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    48323 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/amber_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber/v2/api/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92075 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.619071 boonamber-2.0.8/boonamber/v2/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/amber_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/analytic_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/autotuning.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/delete_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/feature_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/feature_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/feature_root_cause.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/fusion_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_models_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_nano_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_pretrain_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_root_cause_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_status_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_summary_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/get_version_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_amber_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_autotune.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_buffer_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_nano.py
--rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_nano_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_nano_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_pattern_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_ams.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_analytics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_floats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_recent_times.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_streaming_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/m_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/magic_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/mncp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/model_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/nano_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/percent_variation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_config_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_config_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_data_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_learning_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_learning_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_model_copy_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_model_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_pretrain_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/post_pretrain_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/pretrain_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/put_data_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/put_data_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/put_model_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/streaming_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/training_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/models/version_number.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-06-08 11:47:05.000000 boonamber-2.0.8/boonamber/v2/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:47:16.611071 boonamber-2.0.8/boonamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 11:47:16.000000 boonamber-2.0.8/boonamber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-08 11:47:05.000000 boonamber-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:47:16.619071 boonamber-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.733766 boonamber-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 21:09:07.000000 boonamber-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 21:09:15.733766 boonamber-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-22 21:09:07.000000 boonamber-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.713766 boonamber-2.0.9/boonamber/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.717766 boonamber-2.0.9/boonamber/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/util/ambererror.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.717766 boonamber-2.0.9/boonamber/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    48323 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.717766 boonamber-2.0.9/boonamber/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22682 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/amber_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.717766 boonamber-2.0.9/boonamber/v2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92075 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.733766 boonamber-2.0.9/boonamber/v2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/amber_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12863 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/analytic_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/autotune_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/delete_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/feature_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/feature_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/feature_root_cause.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/fusion_feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/get_models_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/get_nano_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/get_pretrain_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/get_root_cause_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/get_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/get_summary_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8967 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/get_version_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9710 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_amber_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_autotune.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_buffer_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6625 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_nano.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7210 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_nano_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_nano_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_pattern_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_recent_ams.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_recent_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_recent_floats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_recent_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_recent_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_recent_times.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_streaming_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/m_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/magic_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/mncp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/model_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/nano_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/percent_variation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_config_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_config_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_learning_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_learning_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_model_copy_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3131 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_model_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_oauth2_access_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_oauth2_access_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_oauth2_refresh_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_oauth2_refresh_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_pretrain_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/post_pretrain_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/pretrain_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/put_data_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/put_data_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/put_model_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/streaming_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/training_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/models/version_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-06-22 21:09:07.000000 boonamber-2.0.9/boonamber/v2/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:15.713766 boonamber-2.0.9/boonamber.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 21:09:15.000000 boonamber-2.0.9/boonamber.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-22 21:09:15.000000 boonamber-2.0.9/boonamber.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:09:15.000000 boonamber-2.0.9/boonamber.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 21:09:15.000000 boonamber-2.0.9/boonamber.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 21:09:15.000000 boonamber-2.0.9/boonamber.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-22 21:09:07.000000 boonamber-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 21:09:15.733766 boonamber-2.0.9/setup.cfg
```

### Comparing `boonamber-2.0.8/LICENSE` & `boonamber-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/PKG-INFO` & `boonamber-2.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boonamber
-Version: 2.0.8
+Version: 2.0.9
 Summary: An SDK for Boon Amber sensor analytics
 Author: BoonLogic
 Author-email: amber-support@boonlogic.com
 License: MIT
 Project-URL: repository, https://github.com/boonlogic/amber-python-sdk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boonamber-2.0.8/README.md` & `boonamber-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/__init__.py` & `boonamber-2.0.9/boonamber/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v1/__init__.py` & `boonamber-2.0.9/boonamber/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/__init__.py` & `boonamber-2.0.9/boonamber/v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from boonamber.v2.api.default_api import DefaultApi
 # import ApiClient
 from boonamber.v2.api_client import ApiClient
 from boonamber.v2.configuration import Configuration
 # import models into sdk package
 from boonamber.v2.models.amber_state import AmberState
 from boonamber.v2.models.analytic_results import AnalyticResults
-from boonamber.v2.models.autotuning import Autotuning
+from boonamber.v2.models.autotune_config import AutotuneConfig
 from boonamber.v2.models.config_response import ConfigResponse
 from boonamber.v2.models.delete_model_response import DeleteModelResponse
 from boonamber.v2.models.error import Error
 from boonamber.v2.models.feature_config import FeatureConfig
 from boonamber.v2.models.feature_config_response import FeatureConfigResponse
 from boonamber.v2.models.feature_root_cause import FeatureRootCause
 from boonamber.v2.models.fusion_feature import FusionFeature
```

### Comparing `boonamber-2.0.8/boonamber/v2/amber_client.py` & `boonamber-2.0.9/boonamber/v2/amber_client.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/api/default_api.py` & `boonamber-2.0.9/boonamber/v2/api/default_api.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/api_client.py` & `boonamber-2.0.9/boonamber/v2/api_client.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/configuration.py` & `boonamber-2.0.9/boonamber/v2/configuration.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/__init__.py` & `boonamber-2.0.9/boonamber/v2/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 """
 
 from __future__ import absolute_import
 
 # import models into model package
 from boonamber.v2.models.amber_state import AmberState
 from boonamber.v2.models.analytic_results import AnalyticResults
-from boonamber.v2.models.autotuning import Autotuning
+from boonamber.v2.models.autotune_config import AutotuneConfig
 from boonamber.v2.models.config_response import ConfigResponse
 from boonamber.v2.models.delete_model_response import DeleteModelResponse
 from boonamber.v2.models.error import Error
 from boonamber.v2.models.feature_config import FeatureConfig
 from boonamber.v2.models.feature_config_response import FeatureConfigResponse
 from boonamber.v2.models.feature_root_cause import FeatureRootCause
 from boonamber.v2.models.fusion_feature import FusionFeature
```

### Comparing `boonamber-2.0.8/boonamber/v2/models/amber_state.py` & `boonamber-2.0.9/boonamber/v2/models/amber_state.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/analytic_results.py` & `boonamber-2.0.9/boonamber/v2/models/analytic_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,42 +33,45 @@
         'aw': 'list[int]',
         'id': 'list[int]',
         'ni': 'list[int]',
         'ns': 'list[int]',
         'nw': 'list[float]',
         'om': 'list[float]',
         'ri': 'list[int]',
-        'si': 'list[int]'
+        'si': 'list[int]',
+        'pi': 'list[int]'
     }
 
     attribute_map = {
         'ad': 'AD',
         'ah': 'AH',
         'aw': 'AW',
         'id': 'ID',
         'ni': 'NI',
         'ns': 'NS',
         'nw': 'NW',
         'om': 'OM',
         'ri': 'RI',
-        'si': 'SI'
+        'si': 'SI',
+        'pi': 'PI'
     }
 
-    def __init__(self, ad=None, ah=None, aw=None, id=None, ni=None, ns=None, nw=None, om=None, ri=None, si=None):
+    def __init__(self, ad=None, ah=None, aw=None, id=None, ni=None, ns=None, nw=None, om=None, ri=None, si=None, pi=None):
         """AnalyticResults - a model defined in Swagger"""
         self._ad = None
         self._ah = None
         self._aw = None
         self._id = None
         self._ni = None
         self._ns = None
         self._nw = None
         self._om = None
         self._ri = None
         self._si = None
+        self._pi = None
         self.discriminator = None
         if ad is not None:
             self.ad = ad
         if ah is not None:
             self.ah = ah
         if aw is not None:
             self.aw = aw
@@ -82,14 +85,16 @@
             self.nw = nw
         if om is not None:
             self.om = om
         if ri is not None:
             self.ri = ri
         if si is not None:
             self.si = si
+        if pi is not None:
+            self.pi = pi
 
     @property
     def ad(self):
         """Gets the ad of this AnalyticResults.
 
         A binary array where 1 means a pattern was anomalous and 0 means normal. This value is derived by thresholding the `anomalyIndex`.
 
@@ -313,14 +318,37 @@
 
         :param si: The si of this AnalyticResults.
         :type: list[int]
         """
 
         self._si = si
 
+    @property
+    def pi(self):
+        """Gets the pi of this AnalyticResults.
+
+        An anomaly index that represents the probability within the model of getting that cluster. PI is scaled so that 0 is the most probable cluster (least anomalous) and values close to 1000 represent very improbable clusters, that is, that very rarely occurred during training.
+
+        :return: The pi of this AnalyticResults.
+        :rtype: list[int]
+        """
+        return self._pi
+
+    @pi.setter
+    def pi(self, pi):
+        """Sets the pi of this AnalyticResults.
+
+        An anomaly index that represents the probability within the model of getting that cluster. PI is scaled so that 0 is the most probable cluster (least anomalous) and values close to 1000 represent very improbable clusters, that is, that very rarely occurred during training.
+
+        :param pi: The pi of this AnalyticResults.
+        :type: list[int]
+        """
+
+        self._pi = pi
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `boonamber-2.0.8/boonamber/v2/models/autotuning.py` & `boonamber-2.0.9/boonamber/v2/models/autotune_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Autotuning(object):
+class AutotuneConfig(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -34,60 +34,60 @@
 
     attribute_map = {
         'range': 'range',
         'percent_variation': 'percentVariation'
     }
 
     def __init__(self, range=True, percent_variation=True):
-        """Autotuning - a model defined in Swagger"""
+        """AutotuneConfig - a model defined in Swagger"""
         self._range = None
         self._percent_variation = None
         self.discriminator = None
         if range is not None:
             self.range = range
         if percent_variation is not None:
             self.percent_variation = percent_variation
 
     @property
     def range(self):
-        """Gets the range of this Autotuning.
+        """Gets the range of this AutotuneConfig.
 
 
-        :return: The range of this Autotuning.
+        :return: The range of this AutotuneConfig.
         :rtype: bool
         """
         return self._range
 
     @range.setter
     def range(self, range):
-        """Sets the range of this Autotuning.
+        """Sets the range of this AutotuneConfig.
 
 
-        :param range: The range of this Autotuning.
+        :param range: The range of this AutotuneConfig.
         :type: bool
         """
 
         self._range = range
 
     @property
     def percent_variation(self):
-        """Gets the percent_variation of this Autotuning.
+        """Gets the percent_variation of this AutotuneConfig.
 
 
-        :return: The percent_variation of this Autotuning.
+        :return: The percent_variation of this AutotuneConfig.
         :rtype: bool
         """
         return self._percent_variation
 
     @percent_variation.setter
     def percent_variation(self, percent_variation):
-        """Sets the percent_variation of this Autotuning.
+        """Sets the percent_variation of this AutotuneConfig.
 
 
-        :param percent_variation: The percent_variation of this Autotuning.
+        :param percent_variation: The percent_variation of this AutotuneConfig.
         :type: bool
         """
 
         self._percent_variation = percent_variation
 
     def to_dict(self):
         """Returns the model properties as a dict"""
@@ -106,15 +106,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Autotuning, dict):
+        if issubclass(AutotuneConfig, dict):
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
-        if not isinstance(other, Autotuning):
+        if not isinstance(other, AutotuneConfig):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `boonamber-2.0.8/boonamber/v2/models/config_response.py` & `boonamber-2.0.9/boonamber/v2/models/config_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'streaming_window': 'StreamingWindow',
         'percent_variation': 'PercentVariation',
         'features': 'list[FeatureConfigResponse]',
         'training': 'TrainingConfig',
-        'autotuning': 'Autotuning'
+        'autotuning': 'AutotuneConfig'
     }
 
     attribute_map = {
         'streaming_window': 'streamingWindow',
         'percent_variation': 'percentVariation',
         'features': 'features',
         'training': 'training',
@@ -148,25 +148,25 @@
 
     @property
     def autotuning(self):
         """Gets the autotuning of this ConfigResponse.
 
 
         :return: The autotuning of this ConfigResponse.
-        :rtype: Autotuning
+        :rtype: AutotuneConfig
         """
         return self._autotuning
 
     @autotuning.setter
     def autotuning(self, autotuning):
         """Sets the autotuning of this ConfigResponse.
 
 
         :param autotuning: The autotuning of this ConfigResponse.
-        :type: Autotuning
+        :type: AutotuneConfig
         """
 
         self._autotuning = autotuning
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `boonamber-2.0.8/boonamber/v2/models/delete_model_response.py` & `boonamber-2.0.9/boonamber/v2/models/delete_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/error.py` & `boonamber-2.0.9/boonamber/v2/models/error.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/feature_config.py` & `boonamber-2.0.9/boonamber/v2/models/feature_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/feature_config_response.py` & `boonamber-2.0.9/boonamber/v2/models/feature_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/feature_root_cause.py` & `boonamber-2.0.9/boonamber/v2/models/feature_root_cause.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/fusion_feature.py` & `boonamber-2.0.9/boonamber/v2/models/fusion_feature.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/get_models_response.py` & `boonamber-2.0.9/boonamber/v2/models/get_models_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/get_nano_status_response.py` & `boonamber-2.0.9/boonamber/v2/models/get_nano_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/get_pretrain_response.py` & `boonamber-2.0.9/boonamber/v2/models/get_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/get_root_cause_response.py` & `boonamber-2.0.9/boonamber/v2/models/get_root_cause_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/get_status_response.py` & `boonamber-2.0.9/boonamber/v2/models/get_status_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/get_summary_response.py` & `boonamber-2.0.9/boonamber/v2/models/get_summary_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/get_version_response.py` & `boonamber-2.0.9/boonamber/v2/models/get_version_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_amber_status.py` & `boonamber-2.0.9/boonamber/v2/models/m_amber_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_autotune.py` & `boonamber-2.0.9/boonamber/v2/models/m_autotune.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_buffer_stats.py` & `boonamber-2.0.9/boonamber/v2/models/m_buffer_stats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_nano.py` & `boonamber-2.0.9/boonamber/v2/models/m_nano.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_nano_backend.py` & `boonamber-2.0.9/boonamber/v2/models/m_nano_backend.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_nano_config.py` & `boonamber-2.0.9/boonamber/v2/models/m_nano_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_pattern_memory.py` & `boonamber-2.0.9/boonamber/v2/models/m_pattern_memory.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_recent_ams.py` & `boonamber-2.0.9/boonamber/v2/models/m_recent_ams.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_recent_analytics.py` & `boonamber-2.0.9/boonamber/v2/models/m_recent_analytics.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_recent_floats.py` & `boonamber-2.0.9/boonamber/v2/models/m_recent_floats.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_recent_ids.py` & `boonamber-2.0.9/boonamber/v2/models/m_recent_ids.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_recent_samples.py` & `boonamber-2.0.9/boonamber/v2/models/m_recent_samples.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_recent_times.py` & `boonamber-2.0.9/boonamber/v2/models/m_recent_times.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_streaming_parameters.py` & `boonamber-2.0.9/boonamber/v2/models/m_streaming_parameters.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/m_training.py` & `boonamber-2.0.9/boonamber/v2/models/m_training.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/magic_number.py` & `boonamber-2.0.9/boonamber/v2/models/magic_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/map.py` & `boonamber-2.0.9/boonamber/v2/models/map.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/mncp.py` & `boonamber-2.0.9/boonamber/v2/models/mncp.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/model.py` & `boonamber-2.0.9/boonamber/v2/models/model.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/model_status.py` & `boonamber-2.0.9/boonamber/v2/models/model_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,37 +30,40 @@
     swagger_types = {
         'state': 'AmberState',
         'warning_level': 'int',
         'sample_count': 'int',
         'cluster_count': 'int',
         'progress': 'int',
         'message': 'str',
+        'graduation': 'str',
         'last_modified': 'int',
         'last_modified_delta': 'int'
     }
 
     attribute_map = {
         'state': 'state',
         'warning_level': 'warningLevel',
         'sample_count': 'sampleCount',
         'cluster_count': 'clusterCount',
         'progress': 'progress',
         'message': 'message',
+        'graduation': 'graduation',
         'last_modified': 'lastModified',
         'last_modified_delta': 'lastModifiedDelta'
     }
 
-    def __init__(self, state=None, warning_level=None, sample_count=None, cluster_count=None, progress=None, message=None, last_modified=None, last_modified_delta=None):
+    def __init__(self, state=None, warning_level=None, sample_count=None, cluster_count=None, progress=None, message=None, graduation=None, last_modified=None, last_modified_delta=None):
         """ModelStatus - a model defined in Swagger"""
         self._state = None
         self._warning_level = None
         self._sample_count = None
         self._cluster_count = None
         self._progress = None
         self._message = None
+        self._graduation = None
         self._last_modified = None
         self._last_modified_delta = None
         self.discriminator = None
         if state is not None:
             self.state = state
         if warning_level is not None:
             self.warning_level = warning_level
@@ -68,14 +71,16 @@
             self.sample_count = sample_count
         if cluster_count is not None:
             self.cluster_count = cluster_count
         if progress is not None:
             self.progress = progress
         if message is not None:
             self.message = message
+        if graduation is not None:
+            self.graduation = graduation
         if last_modified is not None:
             self.last_modified = last_modified
         if last_modified_delta is not None:
             self.last_modified_delta = last_modified_delta
 
     @property
     def state(self):
@@ -210,14 +215,37 @@
         :param message: The message of this ModelStatus.
         :type: str
         """
 
         self._message = message
 
     @property
+    def graduation(self):
+        """Gets the graduation of this ModelStatus.
+
+        Reason for learning being turned off.
+
+        :return: The graduation of this ModelStatus.
+        :rtype: str
+        """
+        return self._graduation
+
+    @graduation.setter
+    def graduation(self, graduation):
+        """Sets the graduation of this ModelStatus.
+
+        Reason for learning being turned off.
+
+        :param graduation: The graduation of this ModelStatus.
+        :type: str
+        """
+
+        self._graduation = graduation
+
+    @property
     def last_modified(self):
         """Gets the last_modified of this ModelStatus.
 
         Unix time stamp of the last posted stream data
 
         :return: The last_modified of this ModelStatus.
         :rtype: int
```

### Comparing `boonamber-2.0.8/boonamber/v2/models/nano_status.py` & `boonamber-2.0.9/boonamber/v2/models/nano_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/percent_variation.py` & `boonamber-2.0.9/boonamber/v2/models/percent_variation.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_config_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_config_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'streaming_window': 'StreamingWindow',
         'percent_variation': 'PercentVariation',
         'features': 'list[FeatureConfig]',
         'training': 'TrainingConfig',
-        'autotuning': 'Autotuning'
+        'autotuning': 'AutotuneConfig'
     }
 
     attribute_map = {
         'streaming_window': 'streamingWindow',
         'percent_variation': 'percentVariation',
         'features': 'features',
         'training': 'training',
@@ -150,25 +150,25 @@
 
     @property
     def autotuning(self):
         """Gets the autotuning of this PostConfigRequest.
 
 
         :return: The autotuning of this PostConfigRequest.
-        :rtype: Autotuning
+        :rtype: AutotuneConfig
         """
         return self._autotuning
 
     @autotuning.setter
     def autotuning(self, autotuning):
         """Sets the autotuning of this PostConfigRequest.
 
 
         :param autotuning: The autotuning of this PostConfigRequest.
-        :type: Autotuning
+        :type: AutotuneConfig
         """
 
         self._autotuning = autotuning
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
```

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_config_response.py` & `boonamber-2.0.9/boonamber/v2/models/post_config_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_data_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_data_response.py` & `boonamber-2.0.9/boonamber/v2/models/post_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_learning_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_learning_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_learning_response.py` & `boonamber-2.0.9/boonamber/v2/models/post_learning_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_model_copy_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_model_copy_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_model_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_model_response.py` & `boonamber-2.0.9/boonamber/v2/models/post_model_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_oauth2_access_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_oauth2_access_response.py` & `boonamber-2.0.9/boonamber/v2/models/post_oauth2_access_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_oauth2_refresh_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_oauth2_refresh_response.py` & `boonamber-2.0.9/boonamber/v2/models/post_oauth2_refresh_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_pretrain_request.py` & `boonamber-2.0.9/boonamber/v2/models/post_pretrain_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/post_pretrain_response.py` & `boonamber-2.0.9/boonamber/v2/models/post_pretrain_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/pretrain_status.py` & `boonamber-2.0.9/boonamber/v2/models/pretrain_status.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/put_data_request.py` & `boonamber-2.0.9/boonamber/v2/models/put_data_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/put_data_response.py` & `boonamber-2.0.9/boonamber/v2/models/put_data_response.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/put_model_request.py` & `boonamber-2.0.9/boonamber/v2/models/put_model_request.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/streaming_window.py` & `boonamber-2.0.9/boonamber/v2/models/streaming_window.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/training_config.py` & `boonamber-2.0.9/boonamber/v2/models/training_config.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/models/version_number.py` & `boonamber-2.0.9/boonamber/v2/models/version_number.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber/v2/rest.py` & `boonamber-2.0.9/boonamber/v2/rest.py`

 * *Files identical despite different names*

### Comparing `boonamber-2.0.8/boonamber.egg-info/PKG-INFO` & `boonamber-2.0.9/boonamber.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boonamber
-Version: 2.0.8
+Version: 2.0.9
 Summary: An SDK for Boon Amber sensor analytics
 Author: BoonLogic
 Author-email: amber-support@boonlogic.com
 License: MIT
 Project-URL: repository, https://github.com/boonlogic/amber-python-sdk
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `boonamber-2.0.8/boonamber.egg-info/SOURCES.txt` & `boonamber-2.0.9/boonamber.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 boonamber/v2/configuration.py
 boonamber/v2/rest.py
 boonamber/v2/api/__init__.py
 boonamber/v2/api/default_api.py
 boonamber/v2/models/__init__.py
 boonamber/v2/models/amber_state.py
 boonamber/v2/models/analytic_results.py
-boonamber/v2/models/autotuning.py
+boonamber/v2/models/autotune_config.py
 boonamber/v2/models/config_response.py
 boonamber/v2/models/delete_model_response.py
 boonamber/v2/models/error.py
 boonamber/v2/models/feature_config.py
 boonamber/v2/models/feature_config_response.py
 boonamber/v2/models/feature_root_cause.py
 boonamber/v2/models/fusion_feature.py
```

### Comparing `boonamber-2.0.8/pyproject.toml` & `boonamber-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "boonamber"
-version = "2.0.8"
+version = "2.0.9"
 authors = [
     {name = "BoonLogic"},
     {email = "amber-support@boonlogic.com"}
 ]
 urls = {repository = "https://github.com/boonlogic/amber-python-sdk"}
 license = {text = "MIT"}
 description = "An SDK for Boon Amber sensor analytics"
```

