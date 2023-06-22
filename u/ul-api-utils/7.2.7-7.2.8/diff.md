# Comparing `tmp/ul-api-utils-7.2.7.tar.gz` & `tmp/ul-api-utils-7.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-api-utils-7.2.7.tar", last modified: Thu Jun 22 12:49:58 2023, max compression
+gzip compressed data, was "ul-api-utils-7.2.8.tar", last modified: Thu Jun 22 15:00:15 2023, max compression
```

## Comparing `ul-api-utils-7.2.7.tar` & `ul-api-utils-7.2.8.tar`

### file list

```diff
@@ -1,163 +1,163 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.185772 ul-api-utils-7.2.7/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2022-02-08 08:28:45.000000 ul-api-utils-7.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)    13527 2023-06-22 12:49:58.185772 ul-api-utils-7.2.7/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    12938 2023-04-11 10:27:02.000000 ul-api-utils-7.2.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.161771 ul-api-utils-7.2.7/example/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-15 22:48:45.000000 ul-api-utils-7.2.7/example/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/example/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/example/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.161771 ul-api-utils-7.2.7/example/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-01 08:27:51.000000 ul-api-utils-7.2.7/example/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/example/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-15 22:48:45.000000 ul-api-utils-7.2.7/example/pure_flask_example.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-15 22:48:45.000000 ul-api-utils-7.2.7/example/rate_limit_load.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.161771 ul-api-utils-7.2.7/example/routes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-08 14:57:28.000000 ul-api-utils-7.2.7/example/routes/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11234 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/example/routes/api_some.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.165771 ul-api-utils-7.2.7/example/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 20:31:49.000000 ul-api-utils-7.2.7/example/workers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/example/workers/worker.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 12:49:58.185772 ul-api-utils-7.2.7/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.165771 ul-api-utils-7.2.7/ul_api_utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.165771 ul-api-utils-7.2.7/ul_api_utils/access/
--rw-rw-rw-   0 root         (0) root         (0)     4274 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/access/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.169771 ul-api-utils-7.2.7/ul_api_utils/api_resource/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_request.py
--rw-rw-rw-   0 root         (0) root         (0)    17179 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_resource.py
--rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_resource_config.py
--rw-rw-rw-   0 root         (0) root         (0)    17241 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_resource_fn_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_resource_type.py
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_response_db.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/api_response_payload_alias.py
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/db_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/api_resource/signature_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.169771 ul-api-utils-7.2.7/ul_api_utils/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8453 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/cmd_enc_keys.py
--rw-rw-rw-   0 root         (0) root         (0)     2732 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/cmd_gen_api_user_token.py
--rw-rw-rw-   0 root         (0) root         (0)     4549 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/cmd_gen_new_api_user.py
--rw-rw-rw-   0 root         (0) root         (0)     4453 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/cmd_start.py
--rw-rw-rw-   0 root         (0) root         (0)     2593 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/cmd_worker_start.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.169771 ul-api-utils-7.2.7/ul_api_utils/commands/start/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/start/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/start/gunicorn.conf.py
--rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/commands/start/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.173771 ul-api-utils-7.2.7/ul_api_utils/conf/
--rw-rw-rw-   0 root         (0) root         (0)   999747 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/conf/ul-debugger-main.js
--rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/conf/ul-debugger-ui.js
--rw-rw-rw-   0 root         (0) root         (0)     3008 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.173771 ul-api-utils-7.2.7/ul_api_utils/debug/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/debug/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/debug/debugger.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/debug/malloc.py
--rw-rw-rw-   0 root         (0) root         (0)    14591 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/debug/stat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.173771 ul-api-utils-7.2.7/ul_api_utils/encrypt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/encrypt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
--rw-rw-rw-   0 root         (0) root         (0)     8137 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.173771 ul-api-utils-7.2.7/ul_api_utils/internal_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.173771 ul-api-utils-7.2.7/ul_api_utils/internal_api/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/__tests__/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
--rw-rw-rw-   0 root         (0) root         (0)    14067 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/internal_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/internal_api_check_context.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/internal_api_error.py
--rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/internal_api/internal_api_response.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.177772 ul-api-utils-7.2.7/ul_api_utils/modules/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.177772 ul-api-utils-7.2.7/ul_api_utils/modules/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10719 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)    20122 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/api_sdk_jwt.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/intermediate_state.py
--rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/worker_context.py
--rw-rw-rw-   0 root         (0) root         (0)     4611 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/worker_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/modules/worker_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.177772 ul-api-utils-7.2.7/ul_api_utils/resources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5074 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/debugger_scripts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.177772 ul-api-utils-7.2.7/ul_api_utils/resources/health_check/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/health_check/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/health_check/const.py
--rw-rw-rw-   0 root         (0) root         (0)    18739 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/health_check/health_check.py
--rw-rw-rw-   0 root         (0) root         (0)     2572 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/health_check/health_check_template.py
--rw-rw-rw-   0 root         (0) root         (0)     4199 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/health_check/resource.py
--rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/not_implemented.py
--rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     3358 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/rate_limitter.py
--rw-rw-rw-   0 root         (0) root         (0)     5142 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/resources/swagger.py
--rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/sentry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.181772 ul-api-utils-7.2.7/ul_api_utils/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.181772 ul-api-utils-7.2.7/ul_api_utils/utils/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/__tests__/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/__tests__/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/api_encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/api_format.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/api_method.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/api_pagination.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/api_path_version.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/api_request_info.py
--rw-rw-rw-   0 root         (0) root         (0)     5021 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/avro.py
--rw-rw-rw-   0 root         (0) root         (0)      670 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/cached_per_request.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/colors.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/constants.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/decode_base64.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/deprecated.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.181772 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.181772 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)    28921 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.181772 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2603 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
--rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
--rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/imports.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.185772 ul-api-utils-7.2.7/ul_api_utils/utils/jinja/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/jinja/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/jinja/t_url_for.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/jinja/to_pretty_json.py
--rw-rw-rw-   0 root         (0) root         (0)     4114 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/load_modules.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/token_check.py
--rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/token_check_through_request.py
--rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/unwrap_typing.py
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/utils/uuid_converter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.185772 ul-api-utils-7.2.7/ul_api_utils/validators/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/validators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.185772 ul-api-utils-7.2.7/ul_api_utils/validators/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/validators/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1447 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/validators/__tests__/test_custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)     4023 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/validators/custom_fields.py
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/validators/validate_empty_object.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-22 12:49:56.000000 ul-api-utils-7.2.7/ul_api_utils/validators/validate_uuid.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 12:49:58.165771 ul-api-utils-7.2.7/ul_api_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13527 2023-06-22 12:49:57.000000 ul-api-utils-7.2.7/ul_api_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5370 2023-06-22 12:49:57.000000 ul-api-utils-7.2.7/ul_api_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 12:49:57.000000 ul-api-utils-7.2.7/ul_api_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-06-22 12:49:57.000000 ul-api-utils-7.2.7/ul_api_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      430 2023-06-22 12:49:57.000000 ul-api-utils-7.2.7/ul_api_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-06-22 12:49:57.000000 ul-api-utils-7.2.7/ul_api_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.731852 ul-api-utils-7.2.8/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2022-01-13 12:55:17.000000 ul-api-utils-7.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13527 2023-06-22 15:00:15.731852 ul-api-utils-7.2.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    12938 2023-06-20 10:17:45.000000 ul-api-utils-7.2.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.687850 ul-api-utils-7.2.8/example/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-16 17:17:46.000000 ul-api-utils-7.2.8/example/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/example/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/example/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.687850 ul-api-utils-7.2.8/example/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-27 07:29:34.000000 ul-api-utils-7.2.8/example/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/example/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2022-08-16 17:17:46.000000 ul-api-utils-7.2.8/example/pure_flask_example.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-08-11 16:20:02.000000 ul-api-utils-7.2.8/example/rate_limit_load.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.691851 ul-api-utils-7.2.8/example/routes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-08 14:49:18.000000 ul-api-utils-7.2.8/example/routes/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11237 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/example/routes/api_some.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.691851 ul-api-utils-7.2.8/example/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-18 19:02:57.000000 ul-api-utils-7.2.8/example/workers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/example/workers/worker.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 15:00:15.731852 ul-api-utils-7.2.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.691851 ul-api-utils-7.2.8/ul_api_utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.695851 ul-api-utils-7.2.8/ul_api_utils/access/
+-rw-rw-rw-   0 root         (0) root         (0)     4274 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/access/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.699851 ul-api-utils-7.2.8/ul_api_utils/api_resource/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3279 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    17185 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      760 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_resource_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    17241 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_resource_fn_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_resource_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      888 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_response_db.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/api_response_payload_alias.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/db_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/api_resource/signature_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.699851 ul-api-utils-7.2.8/ul_api_utils/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8453 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/cmd_enc_keys.py
+-rw-rw-rw-   0 root         (0) root         (0)     2732 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/cmd_gen_api_user_token.py
+-rw-rw-rw-   0 root         (0) root         (0)     4549 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/cmd_gen_new_api_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     4453 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/cmd_start.py
+-rw-rw-rw-   0 root         (0) root         (0)     2593 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/cmd_worker_start.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.703851 ul-api-utils-7.2.8/ul_api_utils/commands/start/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/start/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/start/gunicorn.conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      681 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/commands/start/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.703851 ul-api-utils-7.2.8/ul_api_utils/conf/
+-rw-rw-rw-   0 root         (0) root         (0)   999747 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/conf/ul-debugger-main.js
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/conf/ul-debugger-ui.js
+-rw-rw-rw-   0 root         (0) root         (0)     3008 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2532 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.703851 ul-api-utils-7.2.8/ul_api_utils/debug/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/debug/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/debug/debugger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3274 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/debug/malloc.py
+-rw-rw-rw-   0 root         (0) root         (0)    14591 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/debug/stat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.707851 ul-api-utils-7.2.8/ul_api_utils/encrypt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/encrypt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/encrypt/encrypt_decrypt_abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.707851 ul-api-utils-7.2.8/ul_api_utils/internal_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.707851 ul-api-utils-7.2.8/ul_api_utils/internal_api/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1116 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/__tests__/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/__tests__/internal_api_content_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    14067 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/internal_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/internal_api_check_context.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/internal_api_error.py
+-rw-rw-rw-   0 root         (0) root         (0)    11583 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/internal_api/internal_api_response.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.711851 ul-api-utils-7.2.8/ul_api_utils/modules/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.711851 ul-api-utils-7.2.8/ul_api_utils/modules/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10719 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)    20131 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15112 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/api_sdk_jwt.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/intermediate_state.py
+-rw-rw-rw-   0 root         (0) root         (0)      802 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/worker_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     4620 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/worker_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/modules/worker_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.715851 ul-api-utils-7.2.8/ul_api_utils/resources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5077 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/debugger_scripts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.715851 ul-api-utils-7.2.8/ul_api_utils/resources/health_check/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/health_check/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/health_check/const.py
+-rw-rw-rw-   0 root         (0) root         (0)    18739 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/health_check/health_check.py
+-rw-rw-rw-   0 root         (0) root         (0)     2572 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/health_check/health_check_template.py
+-rw-rw-rw-   0 root         (0) root         (0)     4199 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/health_check/resource.py
+-rw-rw-rw-   0 root         (0) root         (0)      973 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/not_implemented.py
+-rw-rw-rw-   0 root         (0) root         (0)     1436 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3358 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/rate_limitter.py
+-rw-rw-rw-   0 root         (0) root         (0)     5142 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/resources/swagger.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/sentry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.723852 ul-api-utils-7.2.8/ul_api_utils/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.723852 ul-api-utils-7.2.8/ul_api_utils/utils/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/__tests__/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/__tests__/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/api_encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/api_format.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/api_method.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/api_pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/api_path_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/api_request_info.py
+-rw-rw-rw-   0 root         (0) root         (0)     5021 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/avro.py
+-rw-rw-rw-   0 root         (0) root         (0)      670 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/cached_per_request.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/colors.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/decode_base64.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/deprecated.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.723852 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.723852 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    28921 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.727852 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2603 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      294 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/schema_type.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/imports.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.727852 ul-api-utils-7.2.8/ul_api_utils/utils/jinja/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/jinja/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/jinja/t_url_for.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/jinja/to_pretty_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     4123 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/load_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/token_check.py
+-rw-rw-rw-   0 root         (0) root         (0)      663 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/token_check_through_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4161 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/unwrap_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      565 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/utils/uuid_converter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.731852 ul-api-utils-7.2.8/ul_api_utils/validators/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/validators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.731852 ul-api-utils-7.2.8/ul_api_utils/validators/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/validators/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/validators/__tests__/test_custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)     4023 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/validators/custom_fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/validators/validate_empty_object.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-06-22 15:00:14.000000 ul-api-utils-7.2.8/ul_api_utils/validators/validate_uuid.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:00:15.695851 ul-api-utils-7.2.8/ul_api_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13527 2023-06-22 15:00:15.000000 ul-api-utils-7.2.8/ul_api_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5370 2023-06-22 15:00:15.000000 ul-api-utils-7.2.8/ul_api_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 15:00:15.000000 ul-api-utils-7.2.8/ul_api_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-22 15:00:15.000000 ul-api-utils-7.2.8/ul_api_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2023-06-22 15:00:15.000000 ul-api-utils-7.2.8/ul_api_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-22 15:00:15.000000 ul-api-utils-7.2.8/ul_api_utils.egg-info/top_level.txt
```

### Comparing `ul-api-utils-7.2.7/LICENSE` & `ul-api-utils-7.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/PKG-INFO` & `ul-api-utils-7.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.2.7
+Version: 7.2.8
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.2.7/README.md` & `ul-api-utils-7.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/example/pure_flask_example.py` & `ul-api-utils-7.2.8/example/pure_flask_example.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/example/routes/api_some.py` & `ul-api-utils-7.2.8/example/routes/api_some.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime, timedelta
 from time import sleep
 from typing import List, Optional, Tuple
 
-from db_utils.modules.db import db
+from ul_db_utils.modules.db import db
 from flask import jsonify
 from pydantic import BaseModel
 
 from werkzeug import Response as BaseResponse
 from ul_api_utils.api_resource.api_request import ApiRequestQuery
 from ul_api_utils.api_resource.api_resource import ApiResource
 from ul_api_utils.api_resource.api_resource_config import ApiResourceConfig
```

### Comparing `ul-api-utils-7.2.7/example/workers/worker.py` & `ul-api-utils-7.2.8/example/workers/worker.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/setup.py` & `ul-api-utils-7.2.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-api-utils',
-    version='7.2.7',
+    version='7.2.8',
     description='Python api utils',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='',
     packages=find_packages(),
     package_data={
```

### Comparing `ul-api-utils-7.2.7/ul_api_utils/access/__init__.py` & `ul-api-utils-7.2.8/ul_api_utils/access/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/api_request.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/api_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/api_resource.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/api_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,16 +182,16 @@
 
         if isinstance(err, InvalidContentTypeError):
             return JsonApiResponse._internal_use_response_error(self._fn_typing.response_payload_many, 400, [
                 self._mk_error("validation-error", str(err), False),
             ])
 
         if self._db_initialized:
-            from db_utils.errors.db_filter_error import DBFiltersError
-            from db_utils.errors.db_sort_error import DBSortError
+            from ul_db_utils.errors.db_filter_error import DBFiltersError
+            from ul_db_utils.errors.db_sort_error import DBSortError
             from sqlalchemy.exc import NoResultFound as NoResultFoundError
             if isinstance(err, (DBFiltersError, DBSortError)):
                 return JsonApiResponse._internal_use_response_error(self._fn_typing.response_payload_many, 400, [
                     self._mk_error("query-validation-error", str(err), False),
                 ])
             if isinstance(err, NoResultFoundError):
                 e = self._mk_error("validation-error", err._message() if err.args else "Resource not found", False)  # type: ignore
```

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/api_resource_config.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/api_resource_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/api_resource_fn_typing.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/api_resource_fn_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/api_response.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/api_response_db.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/api_response_db.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/api_response_payload_alias.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/api_response_payload_alias.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/api_resource/signature_check.py` & `ul-api-utils-7.2.8/ul_api_utils/api_resource/signature_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/commands/cmd_enc_keys.py` & `ul-api-utils-7.2.8/ul_api_utils/commands/cmd_enc_keys.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/commands/cmd_gen_api_user_token.py` & `ul-api-utils-7.2.8/ul_api_utils/commands/cmd_gen_api_user_token.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/commands/cmd_gen_new_api_user.py` & `ul-api-utils-7.2.8/ul_api_utils/commands/cmd_gen_new_api_user.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/commands/cmd_start.py` & `ul-api-utils-7.2.8/ul_api_utils/commands/cmd_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/commands/cmd_worker_start.py` & `ul-api-utils-7.2.8/ul_api_utils/commands/cmd_worker_start.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/commands/start/wsgi.py` & `ul-api-utils-7.2.8/ul_api_utils/commands/start/wsgi.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/conf/ul-debugger-main.js` & `ul-api-utils-7.2.8/ul_api_utils/conf/ul-debugger-main.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/conf/ul-debugger-ui.js` & `ul-api-utils-7.2.8/ul_api_utils/conf/ul-debugger-ui.js`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/conf.py` & `ul-api-utils-7.2.8/ul_api_utils/conf.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/const.py` & `ul-api-utils-7.2.8/ul_api_utils/const.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/debug/debugger.py` & `ul-api-utils-7.2.8/ul_api_utils/debug/debugger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/debug/malloc.py` & `ul-api-utils-7.2.8/ul_api_utils/debug/malloc.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/debug/stat.py` & `ul-api-utils-7.2.8/ul_api_utils/debug/stat.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py` & `ul-api-utils-7.2.8/ul_api_utils/encrypt/encrypt_decrypt_aes_xtea.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/errors.py` & `ul-api-utils-7.2.8/ul_api_utils/errors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/internal_api/__tests__/internal_api.py` & `ul-api-utils-7.2.8/ul_api_utils/internal_api/__tests__/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/internal_api/__tests__/internal_api_content_type.py` & `ul-api-utils-7.2.8/ul_api_utils/internal_api/__tests__/internal_api_content_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/internal_api/internal_api.py` & `ul-api-utils-7.2.8/ul_api_utils/internal_api/internal_api.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/internal_api/internal_api_check_context.py` & `ul-api-utils-7.2.8/ul_api_utils/internal_api/internal_api_check_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/internal_api/internal_api_response.py` & `ul-api-utils-7.2.8/ul_api_utils/internal_api/internal_api_response.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/main.py` & `ul-api-utils-7.2.8/ul_api_utils/main.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py` & `ul-api-utils-7.2.8/ul_api_utils/modules/__tests__/test_api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/modules/api_sdk.py` & `ul-api-utils-7.2.8/ul_api_utils/modules/api_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 from ul_api_utils.utils.jinja.to_pretty_json import to_pretty_json
 from ul_api_utils.utils.json_encoder import CustomJSONEncoder
 from ul_api_utils.utils.load_modules import load_modules_by_template
 from ul_api_utils.utils.uuid_converter import UUID4Converter
 
 if TYPE_CHECKING:
     import flask_sqlalchemy
-    from db_utils.modules.db import DbConfig
+    from ul_db_utils.modules.db import DbConfig
 
 TFn = TypeVar("TFn", bound=Callable[..., ApiResponse])
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -111,16 +111,16 @@
     def config(self) -> ApiSdkConfig:
         return self._config
 
     def init_with_flask(self, app_name: str, *, db_config: Optional['DbConfig'] = None) -> Flask:
         self._initialized_flask_name = try_init(self, app_name)
 
         if db_config is not None:
-            from db_utils.utils.waiting_for_postgres import waiting_for_postgres
-            from db_utils.modules.db import db
+            from ul_db_utils.utils.waiting_for_postgres import waiting_for_postgres
+            from ul_db_utils.modules.db import db
             db_config._init_from_sdk_with_flask(self)
             waiting_for_postgres(db_config.uri)
             self._db = db
 
         self._limiter_enabled = init_rate_limiter(
             flask_app=self._flask_app,
             debugger_enabled=self._debugger_enabled_with_pin,
```

### Comparing `ul-api-utils-7.2.7/ul_api_utils/modules/api_sdk_config.py` & `ul-api-utils-7.2.8/ul_api_utils/modules/api_sdk_config.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/modules/api_sdk_jwt.py` & `ul-api-utils-7.2.8/ul_api_utils/modules/api_sdk_jwt.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/modules/intermediate_state.py` & `ul-api-utils-7.2.8/ul_api_utils/modules/intermediate_state.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/modules/worker_context.py` & `ul-api-utils-7.2.8/ul_api_utils/modules/worker_context.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/modules/worker_sdk.py` & `ul-api-utils-7.2.8/ul_api_utils/modules/worker_sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from ul_api_utils.conf import APPLICATION_START_DT
 from ul_api_utils.modules.intermediate_state import try_init, try_configure
 from ul_api_utils.modules.worker_context import WorkerContext
 from ul_api_utils.modules.worker_sdk_config import WorkerSdkConfig
 from ul_api_utils.sentry import sentry
 
 if TYPE_CHECKING:
-    from db_utils.modules.db import DbConfig
+    from ul_db_utils.modules.db import DbConfig
 
 TI = TypeVar('TI', bound=UniMessage)
 TO = TypeVar('TO', bound=UniMessage)
 
 
 class WorkerSdk:
     __slots__ = (
@@ -48,15 +48,15 @@
 
         return self._flask_app_cache
 
     def init(self, app_name: str, *, db_config: Optional['DbConfig'] = None) -> 'WorkerSdk':
         self._initialized_flask_name = try_init(self, app_name)
 
         if db_config is not None:
-            from db_utils.utils.waiting_for_postgres import waiting_for_postgres
+            from ul_db_utils.utils.waiting_for_postgres import waiting_for_postgres
             self._db_initialized = True
             db_config._init_from_sdk_with_flask(self)
             waiting_for_postgres(db_config.uri)
         return self
 
     def init_with_flask(self, app_name: str, *, db_config: Optional['DbConfig'] = None) -> Tuple['WorkerSdk', Flask]:
         self.init(app_name, db_config=db_config)
@@ -80,15 +80,15 @@
                     sentry_scope.set_tag('app_uptime', f'{(datetime.now() - APPLICATION_START_DT).seconds // 60}s')
                     sentry_scope.set_tag('app_worker_name', type(wrk).__name__)
                     if message.worker_creator:
                         sentry_scope.set_tag('app_worker_creator', message.worker_creator)
 
                     db_instance = None
                     if self._db_initialized:
-                        from db_utils.modules import db
+                        from ul_db_utils.modules import db
                         db_instance = db.db
 
                     ctx = WorkerContext(
                         logger=logger,
                         sentry_scope=sentry_scope,  # type: ignore
                         db=db_instance,
                     )
```

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/debugger_scripts.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/debugger_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             for k, api in internal_api_registry.items():
                 if req_url.startswith(k):
                     api_body = body.dict()
                     api_body['requests_hierarchy'] = []
                     api_result = api.request_post('/debugger-explain', v=ApiPathVersion.NO_VERSION, json=api_body).check().typed(DebuggerExplainResponse)
                     return api_resource.response_ok(api_result.payload)
 
-        from db_utils.modules.db import db
+        from ul_db_utils.modules.db import db
         options = 'COSTS ' + ('TRUE' if body.costs else 'FALSE')
         options += ', SUMMARY ' + ('TRUE' if body.summary else 'FALSE')
         options += ', VERBOSE ' + ('TRUE' if body.verbose else 'FALSE')
         options += ', BUFFERS ' + ('TRUE' if body.buffers else 'FALSE')
 
         sql = f'EXPLAIN ({options})\n{body.sql.strip().strip(";").strip()};'
```

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/health_check/health_check.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/health_check/health_check.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/health_check/health_check_template.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/health_check/health_check_template.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/health_check/resource.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/health_check/resource.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/not_implemented.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/not_implemented.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/permissions.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/permissions.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/rate_limitter.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/rate_limitter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/resources/swagger.py` & `ul-api-utils-7.2.8/ul_api_utils/resources/swagger.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/sentry.py` & `ul-api-utils-7.2.8/ul_api_utils/sentry.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/__tests__/api_path_version.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/__tests__/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/__tests__/unwrap_typing.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/__tests__/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/api_encoding.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/api_encoding.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/api_format.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/api_format.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/api_method.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/api_method.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/api_pagination.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/api_pagination.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/api_path_version.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/api_path_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/avro.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/avro.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/cached_per_request.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/cached_per_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/colors.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/deprecated.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_models.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_three_specifier.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/specifiers/swagger_version.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/input_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/parameter_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/replace_in_dict.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/request_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/flask_swagger_generator/utils/security_type.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/json_encoder.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/json_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
     if isinstance(obj, tuple) and hasattr(obj, '_asdict'):  # NamedTuple
         return obj._asdict()  # type: ignore
     if dataclasses.is_dataclass(obj):
         return dataclasses.asdict(obj)
     if isinstance(obj, BaseModel):
         return obj.dict()
     if has_already_imported_db():
-        from db_utils.modules.db import DbModel
+        from ul_db_utils.modules.db import DbModel
         from flask_sqlalchemy import BaseQuery, Model
         from sqlalchemy.orm import registry
-        from db_utils.model.base_model import BaseModel as DbBaseModel
+        from ul_db_utils.model.base_model import BaseModel as DbBaseModel
 
         if isinstance(obj, DbBaseModel) or isinstance(obj, DbModel):
             return obj.to_dict()
         if isinstance(obj, Model):
             fields = {}
             for field in (x for x in dir(obj) if not x.startswith('_') and x != 'metadata'):
                 val = obj.__getattribute__(field)
@@ -69,15 +69,15 @@
             return list(obj)
         if dataclasses.is_dataclass(obj):
             return dataclasses.asdict(obj)
         if hasattr(obj, "__html__"):  # it needs for Flask ?
             return str(obj.__html__())  # type: ignore
 
         if has_already_imported_db():
-            from db_utils.model.base_model import BaseModel as DbBaseModel
+            from ul_db_utils.model.base_model import BaseModel as DbBaseModel
             from flask_sqlalchemy import BaseQuery, Model, DefaultMeta
             from sqlalchemy.orm import Query, registry
 
             if isinstance(obj, DbBaseModel):
                 return obj.to_dict()
             if isinstance(obj, Query) or isinstance(obj, DefaultMeta):
                 return None
```

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/load_modules.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/load_modules.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/token_check_through_request.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/token_check_through_request.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/unwrap_typing.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/unwrap_typing.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/utils/uuid_converter.py` & `ul-api-utils-7.2.8/ul_api_utils/utils/uuid_converter.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/validators/__tests__/test_custom_fields.py` & `ul-api-utils-7.2.8/ul_api_utils/validators/__tests__/test_custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils/validators/custom_fields.py` & `ul-api-utils-7.2.8/ul_api_utils/validators/custom_fields.py`

 * *Files identical despite different names*

### Comparing `ul-api-utils-7.2.7/ul_api_utils.egg-info/PKG-INFO` & `ul-api-utils-7.2.8/ul_api_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-api-utils
-Version: 7.2.7
+Version: 7.2.8
 Summary: Python api utils
 Author: Unic-lab
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ul-api-utils-7.2.7/ul_api_utils.egg-info/SOURCES.txt` & `ul-api-utils-7.2.8/ul_api_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

