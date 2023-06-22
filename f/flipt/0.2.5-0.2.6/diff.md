# Comparing `tmp/flipt-0.2.5.tar.gz` & `tmp/flipt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipt-0.2.5.tar", max compression
+gzip compressed data, was "flipt-0.2.6.tar", max compression
```

## Comparing `flipt-0.2.5.tar` & `flipt-0.2.6.tar`

### file list

```diff
@@ -1,88 +1,90 @@
--rw-r--r--   0        0        0      407 2023-05-23 15:32:50.499207 flipt-0.2.5/pyproject.toml
--rw-r--r--   0        0        0     2491 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/__init__.py
--rw-r--r--   0        0        0     5307 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/client.py
--rw-r--r--   0        0        0      348 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/core/__init__.py
--rw-r--r--   0        0        0      326 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/core/datetime_utils.py
--rw-r--r--   0        0        0     3507 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      158 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/environment.py
--rw-r--r--   0        0        0        0 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/py.typed
--rw-r--r--   0        0        0     2513 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/__init__.py
--rw-r--r--   0        0        0      261 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth/__init__.py
--rw-r--r--   0        0        0     8838 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth/client.py
--rw-r--r--   0        0        0      369 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth/types/__init__.py
--rw-r--r--   0        0        0     1128 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth/types/authentication.py
--rw-r--r--   0        0        0      943 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth/types/authentication_list.py
--rw-r--r--   0        0        0      988 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth/types/authentication_method.py
--rw-r--r--   0        0        0     1015 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth/types/authentication_token.py
--rw-r--r--   0        0        0       65 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_k_8_s/__init__.py
--rw-r--r--   0        0        0     2837 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_k_8_s/client.py
--rw-r--r--   0        0        0      195 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_oidc/__init__.py
--rw-r--r--   0        0        0     4595 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_oidc/client.py
--rw-r--r--   0        0        0      252 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_oidc/types/__init__.py
--rw-r--r--   0        0        0      854 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py
--rw-r--r--   0        0        0      923 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py
--rw-r--r--   0        0        0       65 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_token/__init__.py
--rw-r--r--   0        0        0     2973 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/auth_method_token/client.py
--rw-r--r--   0        0        0      117 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/commons/__init__.py
--rw-r--r--   0        0        0      120 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/commons/types/__init__.py
--rw-r--r--   0        0        0      933 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/commons/types/pageable.py
--rw-r--r--   0        0        0      279 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/constraints/__init__.py
--rw-r--r--   0        0        0     6649 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/constraints/client.py
--rw-r--r--   0        0        0      399 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/constraints/types/__init__.py
--rw-r--r--   0        0        0     1148 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/constraints/types/constraint.py
--rw-r--r--   0        0        0     1454 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/constraints/types/constraint_comparison_type.py
--rw-r--r--   0        0        0      951 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/constraints/types/constraint_create_request.py
--rw-r--r--   0        0        0      951 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/constraints/types/constraint_update_request.py
--rw-r--r--   0        0        0      237 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/distributions/__init__.py
--rw-r--r--   0        0        0     7184 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/distributions/client.py
--rw-r--r--   0        0        0      324 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/distributions/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/distributions/types/distribution.py
--rw-r--r--   0        0        0      868 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/distributions/types/distribution_create_request.py
--rw-r--r--   0        0        0      868 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/distributions/types/distribution_update_request.py
--rw-r--r--   0        0        0      365 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/__init__.py
--rw-r--r--   0        0        0     4878 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/client.py
--rw-r--r--   0        0        0      490 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/types/__init__.py
--rw-r--r--   0        0        0     1045 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/types/batch_evaluation_request.py
--rw-r--r--   0        0        0     1029 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/types/batch_evaluation_response.py
--rw-r--r--   0        0        0     1446 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/types/evaluation_reason.py
--rw-r--r--   0        0        0      999 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/types/evaluation_request.py
--rw-r--r--   0        0        0     1328 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/evaluate/types/evaluation_response.py
--rw-r--r--   0        0        0      211 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/flags/__init__.py
--rw-r--r--   0        0        0     9920 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/flags/client.py
--rw-r--r--   0        0        0      296 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/flags/types/__init__.py
--rw-r--r--   0        0        0     1047 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/flags/types/flag.py
--rw-r--r--   0        0        0      839 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/flags/types/flag_create_request.py
--rw-r--r--   0        0        0      951 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/flags/types/flag_list.py
--rw-r--r--   0        0        0      826 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/flags/types/flag_update_request.py
--rw-r--r--   0        0        0      251 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/namespaces/__init__.py
--rw-r--r--   0        0        0     9630 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/namespaces/client.py
--rw-r--r--   0        0        0      356 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/namespaces/types/__init__.py
--rw-r--r--   0        0        0      973 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/namespaces/types/namespace.py
--rw-r--r--   0        0        0      809 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/namespaces/types/namespace_create_request.py
--rw-r--r--   0        0        0      976 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/namespaces/types/namespace_list.py
--rw-r--r--   0        0        0      796 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/namespaces/types/namespace_update_request.py
--rw-r--r--   0        0        0      249 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/__init__.py
--rw-r--r--   0        0        0    12302 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/client.py
--rw-r--r--   0        0        0      365 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/types/__init__.py
--rw-r--r--   0        0        0     1142 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/types/rule.py
--rw-r--r--   0        0        0      857 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/types/rule_create_request.py
--rw-r--r--   0        0        0      951 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/types/rule_list.py
--rw-r--r--   0        0        0      849 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/types/rule_order_request.py
--rw-r--r--   0        0        0      843 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/rules/types/rule_update_request.py
--rw-r--r--   0        0        0      273 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/__init__.py
--rw-r--r--   0        0        0    10154 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/client.py
--rw-r--r--   0        0        0      401 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/types/__init__.py
--rw-r--r--   0        0        0     1165 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/types/segment.py
--rw-r--r--   0        0        0      954 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/types/segment_create_request.py
--rw-r--r--   0        0        0      966 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/types/segment_list.py
--rw-r--r--   0        0        0      566 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/types/segment_match_type.py
--rw-r--r--   0        0        0      941 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/segments/types/segment_update_request.py
--rw-r--r--   0        0        0      207 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/variants/__init__.py
--rw-r--r--   0        0        0     6568 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/variants/client.py
--rw-r--r--   0        0        0      279 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/variants/types/__init__.py
--rw-r--r--   0        0        0     1035 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/variants/types/variant.py
--rw-r--r--   0        0        0      861 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/variants/types/variant_create_request.py
--rw-r--r--   0        0        0      861 2023-05-23 15:32:50.499207 flipt-0.2.5/src/flipt/resources/variants/types/variant_update_request.py
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 flipt-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-06-22 18:40:07.522438 flipt-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1354 2023-06-22 18:40:07.522438 flipt-0.2.6/README.md
+-rw-r--r--   0        0        0      365 2023-06-22 18:40:07.522438 flipt-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0     2491 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/__init__.py
+-rw-r--r--   0        0        0     3836 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/client.py
+-rw-r--r--   0        0        0      348 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      158 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/environment.py
+-rw-r--r--   0        0        0        0 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/py.typed
+-rw-r--r--   0        0        0     2513 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/__init__.py
+-rw-r--r--   0        0        0      261 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/__init__.py
+-rw-r--r--   0        0        0     9429 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/client.py
+-rw-r--r--   0        0        0      369 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/__init__.py
+-rw-r--r--   0        0        0     1128 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication.py
+-rw-r--r--   0        0        0      943 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication_list.py
+-rw-r--r--   0        0        0      988 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication_method.py
+-rw-r--r--   0        0        0      925 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth/types/authentication_token.py
+-rw-r--r--   0        0        0       65 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth_method_k_8_s/__init__.py
+-rw-r--r--   0        0        0     2889 2023-06-22 18:40:07.522438 flipt-0.2.6/src/flipt/resources/auth_method_k_8_s/client.py
+-rw-r--r--   0        0        0      195 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/__init__.py
+-rw-r--r--   0        0        0     4699 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/client.py
+-rw-r--r--   0        0        0      252 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/__init__.py
+-rw-r--r--   0        0        0      854 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py
+-rw-r--r--   0        0        0      833 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py
+-rw-r--r--   0        0        0       65 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_token/__init__.py
+-rw-r--r--   0        0        0     3352 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/auth_method_token/client.py
+-rw-r--r--   0        0        0      117 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/commons/__init__.py
+-rw-r--r--   0        0        0      120 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0      933 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/commons/types/pageable.py
+-rw-r--r--   0        0        0      279 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/__init__.py
+-rw-r--r--   0        0        0     6805 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/client.py
+-rw-r--r--   0        0        0      399 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/__init__.py
+-rw-r--r--   0        0        0     1148 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint.py
+-rw-r--r--   0        0        0     1454 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint_comparison_type.py
+-rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint_create_request.py
+-rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/constraints/types/constraint_update_request.py
+-rw-r--r--   0        0        0      237 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/__init__.py
+-rw-r--r--   0        0        0     7340 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/client.py
+-rw-r--r--   0        0        0      324 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/distribution.py
+-rw-r--r--   0        0        0      868 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/distribution_create_request.py
+-rw-r--r--   0        0        0      868 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/distributions/types/distribution_update_request.py
+-rw-r--r--   0        0        0      365 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/__init__.py
+-rw-r--r--   0        0        0     4982 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/client.py
+-rw-r--r--   0        0        0      490 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/__init__.py
+-rw-r--r--   0        0        0     1045 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_request.py
+-rw-r--r--   0        0        0     1029 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_response.py
+-rw-r--r--   0        0        0     1446 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_reason.py
+-rw-r--r--   0        0        0      999 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_request.py
+-rw-r--r--   0        0        0     1328 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_response.py
+-rw-r--r--   0        0        0      211 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/__init__.py
+-rw-r--r--   0        0        0    10180 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/client.py
+-rw-r--r--   0        0        0      296 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/__init__.py
+-rw-r--r--   0        0        0     1047 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag.py
+-rw-r--r--   0        0        0      839 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag_create_request.py
+-rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag_list.py
+-rw-r--r--   0        0        0      826 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/flags/types/flag_update_request.py
+-rw-r--r--   0        0        0      251 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/__init__.py
+-rw-r--r--   0        0        0     9890 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/client.py
+-rw-r--r--   0        0        0      356 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/__init__.py
+-rw-r--r--   0        0        0      973 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace.py
+-rw-r--r--   0        0        0      809 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_create_request.py
+-rw-r--r--   0        0        0      976 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_list.py
+-rw-r--r--   0        0        0      796 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_update_request.py
+-rw-r--r--   0        0        0      249 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/__init__.py
+-rw-r--r--   0        0        0    12614 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/client.py
+-rw-r--r--   0        0        0      365 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/__init__.py
+-rw-r--r--   0        0        0     1142 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule.py
+-rw-r--r--   0        0        0      857 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_create_request.py
+-rw-r--r--   0        0        0      951 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_list.py
+-rw-r--r--   0        0        0      849 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_order_request.py
+-rw-r--r--   0        0        0      843 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/rules/types/rule_update_request.py
+-rw-r--r--   0        0        0      273 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/__init__.py
+-rw-r--r--   0        0        0    10414 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/client.py
+-rw-r--r--   0        0        0      401 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/__init__.py
+-rw-r--r--   0        0        0     1165 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment.py
+-rw-r--r--   0        0        0      954 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_create_request.py
+-rw-r--r--   0        0        0      966 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_list.py
+-rw-r--r--   0        0        0      566 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_match_type.py
+-rw-r--r--   0        0        0      941 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/segments/types/segment_update_request.py
+-rw-r--r--   0        0        0      207 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/__init__.py
+-rw-r--r--   0        0        0     6724 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/client.py
+-rw-r--r--   0        0        0      279 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/__init__.py
+-rw-r--r--   0        0        0     1035 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/variant.py
+-rw-r--r--   0        0        0      861 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/variant_create_request.py
+-rw-r--r--   0        0        0      861 2023-06-22 18:40:07.526438 flipt-0.2.6/src/flipt/resources/variants/types/variant_update_request.py
+-rw-r--r--   0        0        0     1856 1970-01-01 00:00:00.000000 flipt-0.2.6/PKG-INFO
```

### Comparing `flipt-0.2.5/src/flipt/__init__.py` & `flipt-0.2.6/src/flipt/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,115 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .environment import FliptApiEnvironment
 from .resources import (
+    Authentication,
+    AuthenticationList,
+    AuthenticationMethod,
+    AuthenticationToken,
+    BatchEvaluationRequest,
+    BatchEvaluationResponse,
+    Constraint,
+    ConstraintComparisonType,
+    ConstraintCreateRequest,
+    ConstraintUpdateRequest,
+    Distribution,
+    DistributionCreateRequest,
+    DistributionUpdateRequest,
+    EvaluationReason,
+    EvaluationRequest,
+    EvaluationResponse,
+    Flag,
+    FlagCreateRequest,
+    FlagList,
+    FlagUpdateRequest,
+    Namespace,
+    NamespaceCreateRequest,
+    NamespaceList,
+    NamespaceUpdateRequest,
+    OidcAuthorizeUrlResponse,
+    OidcCallbackResponse,
     Pageable,
+    Rule,
+    RuleCreateRequest,
+    RuleList,
+    RuleOrderRequest,
+    RuleUpdateRequest,
+    Segment,
+    SegmentCreateRequest,
+    SegmentList,
+    SegmentMatchType,
+    SegmentUpdateRequest,
+    Variant,
+    VariantCreateRequest,
+    VariantUpdateRequest,
     auth,
     auth_method_k_8_s,
     auth_method_oidc,
     auth_method_token,
-    authentication,
-    authenticationList,
-    authenticationMethod,
-    authenticationToken,
-    batchEvaluationRequest,
-    batchEvaluationResponse,
     commons,
-    constraint,
-    constraintComparisonType,
-    constraintCreateRequest,
     constraints,
-    constraintUpdateRequest,
-    distribution,
-    distributionCreateRequest,
     distributions,
-    distributionUpdateRequest,
     evaluate,
-    evaluationReason,
-    evaluationRequest,
-    evaluationResponse,
-    flag,
-    flagCreateRequest,
-    flagList,
     flags,
-    flagUpdateRequest,
-    namespace,
-    namespaceCreateRequest,
-    namespaceList,
     namespaces,
-    namespaceUpdateRequest,
-    oidcAuthorizeURLResponse,
-    oidcCallbackResponse,
-    rule,
-    ruleCreateRequest,
-    ruleList,
-    ruleOrderRequest,
     rules,
-    ruleUpdateRequest,
-    segment,
-    segmentCreateRequest,
-    segmentList,
-    segmentMatchType,
     segments,
-    segmentUpdateRequest,
-    variant,
-    variantCreateRequest,
     variants,
-    variantUpdateRequest,
 )
 
 __all__ = [
+    "Authentication",
+    "AuthenticationList",
+    "AuthenticationMethod",
+    "AuthenticationToken",
+    "BatchEvaluationRequest",
+    "BatchEvaluationResponse",
+    "Constraint",
+    "ConstraintComparisonType",
+    "ConstraintCreateRequest",
+    "ConstraintUpdateRequest",
+    "Distribution",
+    "DistributionCreateRequest",
+    "DistributionUpdateRequest",
+    "EvaluationReason",
+    "EvaluationRequest",
+    "EvaluationResponse",
+    "Flag",
+    "FlagCreateRequest",
+    "FlagList",
+    "FlagUpdateRequest",
     "FliptApiEnvironment",
+    "Namespace",
+    "NamespaceCreateRequest",
+    "NamespaceList",
+    "NamespaceUpdateRequest",
+    "OidcAuthorizeUrlResponse",
+    "OidcCallbackResponse",
     "Pageable",
+    "Rule",
+    "RuleCreateRequest",
+    "RuleList",
+    "RuleOrderRequest",
+    "RuleUpdateRequest",
+    "Segment",
+    "SegmentCreateRequest",
+    "SegmentList",
+    "SegmentMatchType",
+    "SegmentUpdateRequest",
+    "Variant",
+    "VariantCreateRequest",
+    "VariantUpdateRequest",
     "auth",
     "auth_method_k_8_s",
     "auth_method_oidc",
     "auth_method_token",
-    "authentication",
-    "authenticationList",
-    "authenticationMethod",
-    "authenticationToken",
-    "batchEvaluationRequest",
-    "batchEvaluationResponse",
     "commons",
-    "constraint",
-    "constraintComparisonType",
-    "constraintCreateRequest",
-    "constraintUpdateRequest",
     "constraints",
-    "distribution",
-    "distributionCreateRequest",
-    "distributionUpdateRequest",
     "distributions",
     "evaluate",
-    "evaluationReason",
-    "evaluationRequest",
-    "evaluationResponse",
-    "flag",
-    "flagCreateRequest",
-    "flagList",
-    "flagUpdateRequest",
     "flags",
-    "namespace",
-    "namespaceCreateRequest",
-    "namespaceList",
-    "namespaceUpdateRequest",
     "namespaces",
-    "oidcAuthorizeURLResponse",
-    "oidcCallbackResponse",
-    "rule",
-    "ruleCreateRequest",
-    "ruleList",
-    "ruleOrderRequest",
-    "ruleUpdateRequest",
     "rules",
-    "segment",
-    "segmentCreateRequest",
-    "segmentList",
-    "segmentMatchType",
-    "segmentUpdateRequest",
     "segments",
-    "variant",
-    "variantCreateRequest",
-    "variantUpdateRequest",
     "variants",
 ]
```

### Comparing `flipt-0.2.5/src/flipt/core/datetime_utils.py` & `flipt-0.2.6/src/flipt/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.5/src/flipt/core/jsonable_encoder.py` & `flipt-0.2.6/src/flipt/core/jsonable_encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 (e.g. datetimes to strings, Pydantic models to dicts).
 
 Taken from FastAPI, and made a bit simpler
 https://github.com/tiangolo/fastapi/blob/master/fastapi/encoders.py
 """
 
 import dataclasses
+import datetime as dt
 from collections import defaultdict
 from enum import Enum
 from pathlib import PurePath
 from types import GeneratorType
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
 
 from pydantic import BaseModel
 from pydantic.json import ENCODERS_BY_TYPE
 
+from .datetime_utils import serialize_datetime
+
 SetIntStr = Set[Union[int, str]]
 DictIntStrAny = Dict[Union[int, str], Any]
 
 
 def generate_encoders_by_class_tuples(
     type_encoder_map: Dict[Any, Callable[[Any], Any]]
 ) -> Dict[Callable[[Any], Any], Tuple[Any, ...]]:
@@ -56,14 +59,18 @@
         return jsonable_encoder(obj_dict, custom_encoder=custom_encoder)
     if isinstance(obj, Enum):
         return obj.value
     if isinstance(obj, PurePath):
         return str(obj)
     if isinstance(obj, (str, int, float, type(None))):
         return obj
+    if isinstance(obj, dt.date):
+        return str(obj)
+    if isinstance(obj, dt.datetime):
+        return serialize_datetime(obj)
     if isinstance(obj, dict):
         encoded_dict = {}
         allowed_keys = set(obj.keys())
         for key, value in obj.items():
             if key in allowed_keys:
                 encoded_key = jsonable_encoder(key, custom_encoder=custom_encoder)
                 encoded_value = jsonable_encoder(value, custom_encoder=custom_encoder)
```

### Comparing `flipt-0.2.5/src/flipt/resources/__init__.py` & `flipt-0.2.6/src/flipt/resources/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,80 +11,80 @@
     evaluate,
     flags,
     namespaces,
     rules,
     segments,
     variants,
 )
-from .auth import authentication, authenticationList, authenticationMethod, authenticationToken
-from .auth_method_oidc import oidcAuthorizeURLResponse, oidcCallbackResponse
+from .auth import Authentication, AuthenticationList, AuthenticationMethod, AuthenticationToken
+from .auth_method_oidc import OidcAuthorizeUrlResponse, OidcCallbackResponse
 from .commons import Pageable
-from .constraints import constraint, constraintComparisonType, constraintCreateRequest, constraintUpdateRequest
-from .distributions import distribution, distributionCreateRequest, distributionUpdateRequest
+from .constraints import Constraint, ConstraintComparisonType, ConstraintCreateRequest, ConstraintUpdateRequest
+from .distributions import Distribution, DistributionCreateRequest, DistributionUpdateRequest
 from .evaluate import (
-    batchEvaluationRequest,
-    batchEvaluationResponse,
-    evaluationReason,
-    evaluationRequest,
-    evaluationResponse,
+    BatchEvaluationRequest,
+    BatchEvaluationResponse,
+    EvaluationReason,
+    EvaluationRequest,
+    EvaluationResponse,
 )
-from .flags import flag, flagCreateRequest, flagList, flagUpdateRequest
-from .namespaces import namespace, namespaceCreateRequest, namespaceList, namespaceUpdateRequest
-from .rules import rule, ruleCreateRequest, ruleList, ruleOrderRequest, ruleUpdateRequest
-from .segments import segment, segmentCreateRequest, segmentList, segmentMatchType, segmentUpdateRequest
-from .variants import variant, variantCreateRequest, variantUpdateRequest
+from .flags import Flag, FlagCreateRequest, FlagList, FlagUpdateRequest
+from .namespaces import Namespace, NamespaceCreateRequest, NamespaceList, NamespaceUpdateRequest
+from .rules import Rule, RuleCreateRequest, RuleList, RuleOrderRequest, RuleUpdateRequest
+from .segments import Segment, SegmentCreateRequest, SegmentList, SegmentMatchType, SegmentUpdateRequest
+from .variants import Variant, VariantCreateRequest, VariantUpdateRequest
 
 __all__ = [
+    "Authentication",
+    "AuthenticationList",
+    "AuthenticationMethod",
+    "AuthenticationToken",
+    "BatchEvaluationRequest",
+    "BatchEvaluationResponse",
+    "Constraint",
+    "ConstraintComparisonType",
+    "ConstraintCreateRequest",
+    "ConstraintUpdateRequest",
+    "Distribution",
+    "DistributionCreateRequest",
+    "DistributionUpdateRequest",
+    "EvaluationReason",
+    "EvaluationRequest",
+    "EvaluationResponse",
+    "Flag",
+    "FlagCreateRequest",
+    "FlagList",
+    "FlagUpdateRequest",
+    "Namespace",
+    "NamespaceCreateRequest",
+    "NamespaceList",
+    "NamespaceUpdateRequest",
+    "OidcAuthorizeUrlResponse",
+    "OidcCallbackResponse",
     "Pageable",
+    "Rule",
+    "RuleCreateRequest",
+    "RuleList",
+    "RuleOrderRequest",
+    "RuleUpdateRequest",
+    "Segment",
+    "SegmentCreateRequest",
+    "SegmentList",
+    "SegmentMatchType",
+    "SegmentUpdateRequest",
+    "Variant",
+    "VariantCreateRequest",
+    "VariantUpdateRequest",
     "auth",
     "auth_method_k_8_s",
     "auth_method_oidc",
     "auth_method_token",
-    "authentication",
-    "authenticationList",
-    "authenticationMethod",
-    "authenticationToken",
-    "batchEvaluationRequest",
-    "batchEvaluationResponse",
     "commons",
-    "constraint",
-    "constraintComparisonType",
-    "constraintCreateRequest",
-    "constraintUpdateRequest",
     "constraints",
-    "distribution",
-    "distributionCreateRequest",
-    "distributionUpdateRequest",
     "distributions",
     "evaluate",
-    "evaluationReason",
-    "evaluationRequest",
-    "evaluationResponse",
-    "flag",
-    "flagCreateRequest",
-    "flagList",
-    "flagUpdateRequest",
     "flags",
-    "namespace",
-    "namespaceCreateRequest",
-    "namespaceList",
-    "namespaceUpdateRequest",
     "namespaces",
-    "oidcAuthorizeURLResponse",
-    "oidcCallbackResponse",
-    "rule",
-    "ruleCreateRequest",
-    "ruleList",
-    "ruleOrderRequest",
-    "ruleUpdateRequest",
     "rules",
-    "segment",
-    "segmentCreateRequest",
-    "segmentList",
-    "segmentMatchType",
-    "segmentUpdateRequest",
     "segments",
-    "variant",
-    "variantCreateRequest",
-    "variantUpdateRequest",
     "variants",
 ]
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth/client.py` & `flipt-0.2.6/src/flipt/resources/auth/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,97 +8,108 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.authentication import authentication
-from .types.authentication_list import authenticationList
+from .types.authentication import Authentication
+from .types.authentication_list import AuthenticationList
+
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
 
 class AuthClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def list_tokens(self) -> authenticationList:
+    def list_tokens(self) -> AuthenticationList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/tokens"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authenticationList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AuthenticationList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_token(self, id: str) -> authentication:
+    def get_token(self, id: str) -> Authentication:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/tokens/{id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authentication, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Authentication, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_token(self, id: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/tokens/{id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get_self(self) -> authentication:
+    def get_self(self) -> Authentication:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/self"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authentication, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Authentication, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def expire_self(self, *, expires_at: typing.Optional[dt.datetime] = None) -> None:
+    def expire_self(self, *, expires_at: typing.Optional[dt.datetime] = OMIT) -> None:
+        _request: typing.Dict[str, typing.Any] = {}
+        if expires_at is not OMIT:
+            _request["expiresAt"] = expires_at
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/self/expire"),
-            json=jsonable_encoder({"expiresAt": expires_at}),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -108,91 +119,99 @@
 class AsyncAuthClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def list_tokens(self) -> authenticationList:
+    async def list_tokens(self) -> AuthenticationList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/tokens"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authenticationList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AuthenticationList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_token(self, id: str) -> authentication:
+    async def get_token(self, id: str) -> Authentication:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/tokens/{id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authentication, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Authentication, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_token(self, id: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/tokens/{id}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get_self(self) -> authentication:
+    async def get_self(self) -> Authentication:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/self"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authentication, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Authentication, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def expire_self(self, *, expires_at: typing.Optional[dt.datetime] = None) -> None:
+    async def expire_self(self, *, expires_at: typing.Optional[dt.datetime] = OMIT) -> None:
+        _request: typing.Dict[str, typing.Any] = {}
+        if expires_at is not OMIT:
+            _request["expiresAt"] = expires_at
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/self/expire"),
-                json=jsonable_encoder({"expiresAt": expires_at}),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth/types/authentication.py` & `flipt-0.2.6/src/flipt/resources/auth/types/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .authentication_method import authenticationMethod
+from .authentication_method import AuthenticationMethod
 
 
-class authentication(pydantic.BaseModel):
+class Authentication(pydantic.BaseModel):
     id: str
-    method: authenticationMethod
+    method: AuthenticationMethod
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
     expires_at: typing.Optional[dt.datetime] = pydantic.Field(alias="expiresAt")
     metadata: typing.Dict[str, str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth/types/authentication_list.py` & `flipt-0.2.6/src/flipt/resources/auth/types/authentication_list.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .authentication import authentication
+from .authentication import Authentication
 
 
-class authenticationList(pydantic.BaseModel):
-    authentications: typing.List[authentication]
+class AuthenticationList(pydantic.BaseModel):
+    authentications: typing.List[Authentication]
     next_page_token: str = pydantic.Field(alias="nextPageToken")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth/types/authentication_method.py` & `flipt-0.2.6/src/flipt/resources/auth/types/authentication_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class authenticationMethod(str, enum.Enum):
+class AuthenticationMethod(str, enum.Enum):
     """
     The default is METHOD_NONE
     """
 
     METHOD_NONE = "METHOD_NONE"
     METHOD_TOKEN = "METHOD_TOKEN"
     METHOD_OIDC = "METHOD_OIDC"
@@ -19,15 +19,15 @@
     def visit(
         self,
         method_none: typing.Callable[[], T_Result],
         method_token: typing.Callable[[], T_Result],
         method_oidc: typing.Callable[[], T_Result],
         method_kubernetes: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is authenticationMethod.METHOD_NONE:
+        if self is AuthenticationMethod.METHOD_NONE:
             return method_none()
-        if self is authenticationMethod.METHOD_TOKEN:
+        if self is AuthenticationMethod.METHOD_TOKEN:
             return method_token()
-        if self is authenticationMethod.METHOD_OIDC:
+        if self is AuthenticationMethod.METHOD_OIDC:
             return method_oidc()
-        if self is authenticationMethod.METHOD_KUBERNETES:
+        if self is AuthenticationMethod.METHOD_KUBERNETES:
             return method_kubernetes()
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth/types/authentication_token.py` & `flipt-0.2.6/src/flipt/resources/auth/types/authentication_token.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .authentication import authentication as resources_auth_types_authentication_authentication
+from .authentication import Authentication
 
 
-class authenticationToken(pydantic.BaseModel):
+class AuthenticationToken(pydantic.BaseModel):
     client_token: str = pydantic.Field(alias="clientToken")
-    authentication: resources_auth_types_authentication_authentication
+    authentication: Authentication
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth_method_k_8_s/client.py` & `flipt-0.2.6/src/flipt/resources/auth_method_k_8_s/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,59 +7,61 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from ..auth.types.authentication_token import authenticationToken
+from ..auth.types.authentication_token import AuthenticationToken
 
 
 class AuthMethodK8SClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def verify_service_account(self, *, service_account_token: str) -> authenticationToken:
+    def verify_service_account(self, *, service_account_token: str) -> AuthenticationToken:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/method/kubernetes/serviceaccount"),
             json=jsonable_encoder({"serviceAccountToken": service_account_token}),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authenticationToken, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AuthenticationToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAuthMethodK8SClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def verify_service_account(self, *, service_account_token: str) -> authenticationToken:
+    async def verify_service_account(self, *, service_account_token: str) -> AuthenticationToken:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/method/kubernetes/serviceaccount"),
                 json=jsonable_encoder({"serviceAccountToken": service_account_token}),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authenticationToken, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AuthenticationToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth_method_oidc/client.py` & `flipt-0.2.6/src/flipt/resources/auth_method_oidc/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,95 +6,99 @@
 
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.oidc_authorize_url_response import oidcAuthorizeURLResponse
-from .types.oidc_callback_response import oidcCallbackResponse
+from .types.oidc_authorize_url_response import OidcAuthorizeUrlResponse
+from .types.oidc_callback_response import OidcCallbackResponse
 
 
 class AuthMethodOidcClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def authorize_url(self, provider: str, *, state: str) -> oidcAuthorizeURLResponse:
+    def authorize_url(self, provider: str, *, state: str) -> OidcAuthorizeUrlResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/method/oidc/{provider}/authorize"),
             params={"state": state},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(oidcAuthorizeURLResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(OidcAuthorizeUrlResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def callback(self, provider: str, *, code: str, state: str) -> oidcCallbackResponse:
+    def callback(self, provider: str, *, code: str, state: str) -> OidcCallbackResponse:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/method/oidc/{provider}/callback"),
             params={"code": code, "state": state},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(oidcCallbackResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(OidcCallbackResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncAuthMethodOidcClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def authorize_url(self, provider: str, *, state: str) -> oidcAuthorizeURLResponse:
+    async def authorize_url(self, provider: str, *, state: str) -> OidcAuthorizeUrlResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/method/oidc/{provider}/authorize"),
                 params={"state": state},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(oidcAuthorizeURLResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(OidcAuthorizeUrlResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def callback(self, provider: str, *, code: str, state: str) -> oidcCallbackResponse:
+    async def callback(self, provider: str, *, code: str, state: str) -> OidcCallbackResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"auth/v1/method/oidc/{provider}/callback"),
                 params={"code": code, "state": state},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(oidcCallbackResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(OidcCallbackResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py` & `flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_authorize_url_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class oidcAuthorizeURLResponse(pydantic.BaseModel):
+class OidcAuthorizeUrlResponse(pydantic.BaseModel):
     authorize_url: str = pydantic.Field(alias="authorizeUrl")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py` & `flipt-0.2.6/src/flipt/resources/variants/types/variant_update_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...auth.types.authentication import authentication as resources_auth_types_authentication_authentication
 
 
-class oidcCallbackResponse(pydantic.BaseModel):
-    authentication: resources_auth_types_authentication_authentication
+class VariantUpdateRequest(pydantic.BaseModel):
+    key: str
+    name: typing.Optional[str]
+    description: typing.Optional[str]
+    attachment: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/auth_method_token/client.py` & `flipt-0.2.6/src/flipt/resources/auth_method_token/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,37 +8,44 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from ..auth.types.authentication_token import authenticationToken
+from ..auth.types.authentication_token import AuthenticationToken
+
+# this is used as the default value for optional parameters
+OMIT = typing.cast(typing.Any, ...)
 
 
 class AuthMethodTokenClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
     def create_token(
-        self, *, name: str, description: str, expires_at: typing.Optional[dt.datetime] = None
-    ) -> authenticationToken:
+        self, *, name: str, description: str, expires_at: typing.Optional[dt.datetime] = OMIT
+    ) -> AuthenticationToken:
+        _request: typing.Dict[str, typing.Any] = {"name": name, "description": description}
+        if expires_at is not OMIT:
+            _request["expiresAt"] = expires_at
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/method/token"),
-            json=jsonable_encoder({"name": name, "description": description, "expiresAt": expires_at}),
+            json=jsonable_encoder(_request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authenticationToken, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AuthenticationToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -46,25 +53,29 @@
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
     async def create_token(
-        self, *, name: str, description: str, expires_at: typing.Optional[dt.datetime] = None
-    ) -> authenticationToken:
+        self, *, name: str, description: str, expires_at: typing.Optional[dt.datetime] = OMIT
+    ) -> AuthenticationToken:
+        _request: typing.Dict[str, typing.Any] = {"name": name, "description": description}
+        if expires_at is not OMIT:
+            _request["expiresAt"] = expires_at
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "auth/v1/method/token"),
-                json=jsonable_encoder({"name": name, "description": description, "expiresAt": expires_at}),
+                json=jsonable_encoder(_request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(authenticationToken, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(AuthenticationToken, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/commons/types/pageable.py` & `flipt-0.2.6/src/flipt/resources/commons/types/pageable.py`

 * *Files identical despite different names*

### Comparing `flipt-0.2.5/src/flipt/resources/constraints/client.py` & `flipt-0.2.6/src/flipt/resources/constraints/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.constraint import constraint
-from .types.constraint_create_request import constraintCreateRequest
-from .types.constraint_update_request import constraintUpdateRequest
+from .types.constraint import Constraint
+from .types.constraint_create_request import ConstraintCreateRequest
+from .types.constraint_update_request import ConstraintUpdateRequest
 
 
 class ConstraintsClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def create(self, namespace_key: str, segment_key: str, *, request: constraintCreateRequest) -> constraint:
+    def create(self, namespace_key: str, segment_key: str, *, request: ConstraintCreateRequest) -> Constraint:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments/{segment_key}/constraints"
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(constraint, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Constraint, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, namespace_key: str, segment_key: str, id: str) -> None:
@@ -48,34 +49,36 @@
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
                 f"api/v1/namespaces/{namespace_key}/segments/{segment_key}/constraints/{id}",
             ),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, namespace_key: str, segment_key: str, id: str, *, request: constraintUpdateRequest) -> None:
+    def update(self, namespace_key: str, segment_key: str, id: str, *, request: ConstraintUpdateRequest) -> None:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
                 f"api/v1/namespaces/{namespace_key}/segments/{segment_key}/constraints/{id}",
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -85,29 +88,30 @@
 class AsyncConstraintsClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def create(self, namespace_key: str, segment_key: str, *, request: constraintCreateRequest) -> constraint:
+    async def create(self, namespace_key: str, segment_key: str, *, request: ConstraintCreateRequest) -> Constraint:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/",
                     f"api/v1/namespaces/{namespace_key}/segments/{segment_key}/constraints",
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(constraint, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Constraint, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, namespace_key: str, segment_key: str, id: str) -> None:
@@ -117,35 +121,37 @@
                 urllib.parse.urljoin(
                     f"{self._environment.value}/",
                     f"api/v1/namespaces/{namespace_key}/segments/{segment_key}/constraints/{id}",
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, namespace_key: str, segment_key: str, id: str, *, request: constraintUpdateRequest) -> None:
+    async def update(self, namespace_key: str, segment_key: str, id: str, *, request: ConstraintUpdateRequest) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/",
                     f"api/v1/namespaces/{namespace_key}/segments/{segment_key}/constraints/{id}",
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `flipt-0.2.5/src/flipt/resources/constraints/types/constraint.py` & `flipt-0.2.6/src/flipt/resources/segments/types/segment.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .constraint_comparison_type import constraintComparisonType
+from ...constraints.types.constraint import Constraint
+from .segment_match_type import SegmentMatchType
 
 
-class constraint(pydantic.BaseModel):
-    id: str
-    segment_key: str = pydantic.Field(alias="segmentKey")
-    type: constraintComparisonType
-    property: str
-    operator: str
-    value: str
+class Segment(pydantic.BaseModel):
+    key: str
+    name: str
     description: str
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+    constraints: typing.List[Constraint]
+    match_type: SegmentMatchType = pydantic.Field(alias="matchType")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/constraints/types/constraint_comparison_type.py` & `flipt-0.2.6/src/flipt/resources/constraints/types/constraint_comparison_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class constraintComparisonType(str, enum.Enum):
+class ConstraintComparisonType(str, enum.Enum):
     """
     The default is UNKNOWN_COMPARISON_TYPE
     """
 
     UNKNOWN_COMPARISON_TYPE = "UNKNOWN_COMPARISON_TYPE"
     STRING_COMPARISON_TYPE = "STRING_COMPARISON_TYPE"
     NUMBER_COMPARISON_TYPE = "NUMBER_COMPARISON_TYPE"
@@ -21,17 +21,17 @@
         self,
         unknown_comparison_type: typing.Callable[[], T_Result],
         string_comparison_type: typing.Callable[[], T_Result],
         number_comparison_type: typing.Callable[[], T_Result],
         boolean_comparison_type: typing.Callable[[], T_Result],
         datetime_comparison_type: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is constraintComparisonType.UNKNOWN_COMPARISON_TYPE:
+        if self is ConstraintComparisonType.UNKNOWN_COMPARISON_TYPE:
             return unknown_comparison_type()
-        if self is constraintComparisonType.STRING_COMPARISON_TYPE:
+        if self is ConstraintComparisonType.STRING_COMPARISON_TYPE:
             return string_comparison_type()
-        if self is constraintComparisonType.NUMBER_COMPARISON_TYPE:
+        if self is ConstraintComparisonType.NUMBER_COMPARISON_TYPE:
             return number_comparison_type()
-        if self is constraintComparisonType.BOOLEAN_COMPARISON_TYPE:
+        if self is ConstraintComparisonType.BOOLEAN_COMPARISON_TYPE:
             return boolean_comparison_type()
-        if self is constraintComparisonType.DATETIME_COMPARISON_TYPE:
+        if self is ConstraintComparisonType.DATETIME_COMPARISON_TYPE:
             return datetime_comparison_type()
```

### Comparing `flipt-0.2.5/src/flipt/resources/constraints/types/constraint_create_request.py` & `flipt-0.2.6/src/flipt/resources/constraints/types/constraint_create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .constraint_comparison_type import constraintComparisonType
+from .constraint_comparison_type import ConstraintComparisonType
 
 
-class constraintCreateRequest(pydantic.BaseModel):
-    type: constraintComparisonType
+class ConstraintCreateRequest(pydantic.BaseModel):
+    type: ConstraintComparisonType
     property: str
     operator: str
     value: typing.Optional[str]
     description: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/constraints/types/constraint_update_request.py` & `flipt-0.2.6/src/flipt/resources/constraints/types/constraint_update_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .constraint_comparison_type import constraintComparisonType
+from .constraint_comparison_type import ConstraintComparisonType
 
 
-class constraintUpdateRequest(pydantic.BaseModel):
-    type: constraintComparisonType
+class ConstraintUpdateRequest(pydantic.BaseModel):
+    type: ConstraintComparisonType
     property: str
     operator: str
     value: typing.Optional[str]
     description: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/distributions/client.py` & `flipt-0.2.6/src/flipt/resources/distributions/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,42 +7,43 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.distribution import distribution
-from .types.distribution_create_request import distributionCreateRequest
-from .types.distribution_update_request import distributionUpdateRequest
+from .types.distribution import Distribution
+from .types.distribution_create_request import DistributionCreateRequest
+from .types.distribution_update_request import DistributionUpdateRequest
 
 
 class DistributionsClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
     def create(
-        self, namespace_key: str, flag_key: str, rule_id: str, *, request: distributionCreateRequest
-    ) -> distribution:
+        self, namespace_key: str, flag_key: str, rule_id: str, *, request: DistributionCreateRequest
+    ) -> Distribution:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
                 f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{rule_id}/distributions",
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(distribution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Distribution, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, namespace_key: str, flag_key: str, rule_id: str, id: str, *, variant_id: str) -> None:
@@ -52,39 +53,41 @@
                 f"{self._environment.value}/",
                 f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{rule_id}/distributions/{id}",
             ),
             params={"variantId": variant_id},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update(
-        self, namespace_key: str, flag_key: str, rule_id: str, id: str, *, request: distributionUpdateRequest
-    ) -> distribution:
+        self, namespace_key: str, flag_key: str, rule_id: str, id: str, *, request: DistributionUpdateRequest
+    ) -> Distribution:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._environment.value}/",
                 f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{rule_id}/distributions/{id}",
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(distribution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Distribution, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -92,30 +95,31 @@
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
     async def create(
-        self, namespace_key: str, flag_key: str, rule_id: str, *, request: distributionCreateRequest
-    ) -> distribution:
+        self, namespace_key: str, flag_key: str, rule_id: str, *, request: DistributionCreateRequest
+    ) -> Distribution:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/",
                     f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{rule_id}/distributions",
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(distribution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Distribution, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, namespace_key: str, flag_key: str, rule_id: str, id: str, *, variant_id: str) -> None:
@@ -126,38 +130,40 @@
                     f"{self._environment.value}/",
                     f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{rule_id}/distributions/{id}",
                 ),
                 params={"variantId": variant_id},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update(
-        self, namespace_key: str, flag_key: str, rule_id: str, id: str, *, request: distributionUpdateRequest
-    ) -> distribution:
+        self, namespace_key: str, flag_key: str, rule_id: str, id: str, *, request: DistributionUpdateRequest
+    ) -> Distribution:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/",
                     f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{rule_id}/distributions/{id}",
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(distribution, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Distribution, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/distributions/types/distribution.py` & `flipt-0.2.6/src/flipt/resources/distributions/types/distribution.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class distribution(pydantic.BaseModel):
+class Distribution(pydantic.BaseModel):
     id: str
     rule_id: str = pydantic.Field(alias="ruleId")
     variant_id: str = pydantic.Field(alias="variantId")
     rollout: float
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
```

### Comparing `flipt-0.2.5/src/flipt/resources/distributions/types/distribution_create_request.py` & `flipt-0.2.6/src/flipt/resources/distributions/types/distribution_create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class distributionCreateRequest(pydantic.BaseModel):
+class DistributionCreateRequest(pydantic.BaseModel):
     variant_id: str = pydantic.Field(alias="variantId")
     rollout: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/distributions/types/distribution_update_request.py` & `flipt-0.2.6/src/flipt/resources/distributions/types/distribution_update_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class distributionUpdateRequest(pydantic.BaseModel):
+class DistributionUpdateRequest(pydantic.BaseModel):
     variant_id: str = pydantic.Field(alias="variantId")
     rollout: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/evaluate/client.py` & `flipt-0.2.6/src/flipt/resources/evaluate/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,99 +7,103 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.batch_evaluation_request import batchEvaluationRequest
-from .types.batch_evaluation_response import batchEvaluationResponse
-from .types.evaluation_request import evaluationRequest
-from .types.evaluation_response import evaluationResponse
+from .types.batch_evaluation_request import BatchEvaluationRequest
+from .types.batch_evaluation_response import BatchEvaluationResponse
+from .types.evaluation_request import EvaluationRequest
+from .types.evaluation_response import EvaluationResponse
 
 
 class EvaluateClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def evaluate(self, namespace_key: str, *, request: evaluationRequest) -> evaluationResponse:
+    def evaluate(self, namespace_key: str, *, request: EvaluationRequest) -> EvaluationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/evaluate"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(evaluationResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EvaluationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def batch_evaluate(self, namespace_key: str, *, request: batchEvaluationRequest) -> batchEvaluationResponse:
+    def batch_evaluate(self, namespace_key: str, *, request: BatchEvaluationRequest) -> BatchEvaluationResponse:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/batch-evaluate"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(batchEvaluationResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BatchEvaluationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncEvaluateClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def evaluate(self, namespace_key: str, *, request: evaluationRequest) -> evaluationResponse:
+    async def evaluate(self, namespace_key: str, *, request: EvaluationRequest) -> EvaluationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/evaluate"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(evaluationResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(EvaluationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def batch_evaluate(self, namespace_key: str, *, request: batchEvaluationRequest) -> batchEvaluationResponse:
+    async def batch_evaluate(self, namespace_key: str, *, request: BatchEvaluationRequest) -> BatchEvaluationResponse:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/batch-evaluate"
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(batchEvaluationResponse, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(BatchEvaluationResponse, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/evaluate/types/batch_evaluation_request.py` & `flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .evaluation_request import evaluationRequest
+from .evaluation_request import EvaluationRequest
 
 
-class batchEvaluationRequest(pydantic.BaseModel):
+class BatchEvaluationRequest(pydantic.BaseModel):
     request_id: typing.Optional[str] = pydantic.Field(alias="requestId")
-    requests: typing.List[evaluationRequest]
+    requests: typing.List[EvaluationRequest]
     exclude_not_found: typing.Optional[bool] = pydantic.Field(alias="excludeNotFound")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flipt-0.2.5/src/flipt/resources/evaluate/types/batch_evaluation_response.py` & `flipt-0.2.6/src/flipt/resources/evaluate/types/batch_evaluation_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .evaluation_response import evaluationResponse
+from .evaluation_response import EvaluationResponse
 
 
-class batchEvaluationResponse(pydantic.BaseModel):
+class BatchEvaluationResponse(pydantic.BaseModel):
     request_id: str = pydantic.Field(alias="requestId")
-    responses: typing.List[evaluationResponse]
+    responses: typing.List[EvaluationResponse]
     request_duration_millis: float = pydantic.Field(alias="requestDurationMillis")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flipt-0.2.5/src/flipt/resources/evaluate/types/evaluation_reason.py` & `flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_reason.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class evaluationReason(str, enum.Enum):
+class EvaluationReason(str, enum.Enum):
     UNKNOWN_EVALUATION_REASON = "UNKNOWN_EVALUATION_REASON"
     FLAG_DISABLED_EVALUATION_REASON = "FLAG_DISABLED_EVALUATION_REASON"
     FLAG_NOT_FOUND_EVALUATION_REASON = "FLAG_NOT_FOUND_EVALUATION_REASON"
     MATCH_EVALUATION_REASON = "MATCH_EVALUATION_REASON"
     ERROR_EVALUATION_REASON = "ERROR_EVALUATION_REASON"
 
     def visit(
         self,
         unknown_evaluation_reason: typing.Callable[[], T_Result],
         flag_disabled_evaluation_reason: typing.Callable[[], T_Result],
         flag_not_found_evaluation_reason: typing.Callable[[], T_Result],
         match_evaluation_reason: typing.Callable[[], T_Result],
         error_evaluation_reason: typing.Callable[[], T_Result],
     ) -> T_Result:
-        if self is evaluationReason.UNKNOWN_EVALUATION_REASON:
+        if self is EvaluationReason.UNKNOWN_EVALUATION_REASON:
             return unknown_evaluation_reason()
-        if self is evaluationReason.FLAG_DISABLED_EVALUATION_REASON:
+        if self is EvaluationReason.FLAG_DISABLED_EVALUATION_REASON:
             return flag_disabled_evaluation_reason()
-        if self is evaluationReason.FLAG_NOT_FOUND_EVALUATION_REASON:
+        if self is EvaluationReason.FLAG_NOT_FOUND_EVALUATION_REASON:
             return flag_not_found_evaluation_reason()
-        if self is evaluationReason.MATCH_EVALUATION_REASON:
+        if self is EvaluationReason.MATCH_EVALUATION_REASON:
             return match_evaluation_reason()
-        if self is evaluationReason.ERROR_EVALUATION_REASON:
+        if self is EvaluationReason.ERROR_EVALUATION_REASON:
             return error_evaluation_reason()
```

### Comparing `flipt-0.2.5/src/flipt/resources/evaluate/types/evaluation_request.py` & `flipt-0.2.6/src/flipt/resources/evaluate/types/evaluation_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .evaluation_reason import EvaluationReason
 
 
-class evaluationRequest(pydantic.BaseModel):
-    request_id: typing.Optional[str] = pydantic.Field(alias="requestId")
-    flag_key: str = pydantic.Field(alias="flagKey")
+class EvaluationResponse(pydantic.BaseModel):
+    request_id: str = pydantic.Field(alias="requestId")
     entity_id: str = pydantic.Field(alias="entityId")
-    context: typing.Dict[str, str]
+    request_context: typing.Dict[str, str] = pydantic.Field(alias="requestContext")
+    match: bool
+    flag_key: str = pydantic.Field(alias="flagKey")
+    segment_key: str = pydantic.Field(alias="segmentKey")
+    timestamp: dt.datetime
+    value: str
+    request_duration_millis: float = pydantic.Field(alias="requestDurationMillis")
+    attachment: str
+    reason: EvaluationReason
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/evaluate/types/evaluation_response.py` & `flipt-0.2.6/src/flipt/resources/flags/types/flag_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,29 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .evaluation_reason import evaluationReason
+from .flag import Flag
 
 
-class evaluationResponse(pydantic.BaseModel):
-    request_id: str = pydantic.Field(alias="requestId")
-    entity_id: str = pydantic.Field(alias="entityId")
-    request_context: typing.Dict[str, str] = pydantic.Field(alias="requestContext")
-    match: bool
-    flag_key: str = pydantic.Field(alias="flagKey")
-    segment_key: str = pydantic.Field(alias="segmentKey")
-    timestamp: dt.datetime
-    value: str
-    request_duration_millis: float = pydantic.Field(alias="requestDurationMillis")
-    attachment: str
-    reason: evaluationReason
+class FlagList(pydantic.BaseModel):
+    flags: typing.List[Flag]
+    next_page_token: str = pydantic.Field(alias="nextPageToken")
+    total_count: int = pydantic.Field(alias="totalCount")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/flags/client.py` & `flipt-0.2.6/src/flipt/resources/flags/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.flag import flag
-from .types.flag_create_request import flagCreateRequest
-from .types.flag_list import flagList
-from .types.flag_update_request import flagUpdateRequest
+from .types.flag import Flag
+from .types.flag_create_request import FlagCreateRequest
+from .types.flag_list import FlagList
+from .types.flag_update_request import FlagUpdateRequest
 
 
 class FlagsClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -27,91 +27,96 @@
     def list(
         self,
         namespace_key: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> flagList:
+    ) -> FlagList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags"),
             params={"limit": limit, "offset": offset, "pageToken": page_token},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flagList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(FlagList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, namespace_key: str, *, request: flagCreateRequest) -> flag:
+    def create(self, namespace_key: str, *, request: FlagCreateRequest) -> Flag:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Flag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, namespace_key: str, key: str) -> flag:
+    def get(self, namespace_key: str, key: str) -> Flag:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{key}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Flag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, namespace_key: str, key: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{key}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, namespace_key: str, key: str, *, request: flagUpdateRequest) -> flag:
+    def update(self, namespace_key: str, key: str, *, request: FlagUpdateRequest) -> Flag:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{key}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Flag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -125,94 +130,99 @@
     async def list(
         self,
         namespace_key: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> flagList:
+    ) -> FlagList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags"),
                 params={"limit": limit, "offset": offset, "pageToken": page_token},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flagList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(FlagList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, namespace_key: str, *, request: flagCreateRequest) -> flag:
+    async def create(self, namespace_key: str, *, request: FlagCreateRequest) -> Flag:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Flag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, namespace_key: str, key: str) -> flag:
+    async def get(self, namespace_key: str, key: str) -> Flag:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{key}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Flag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, namespace_key: str, key: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{key}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, namespace_key: str, key: str, *, request: flagUpdateRequest) -> flag:
+    async def update(self, namespace_key: str, key: str, *, request: FlagUpdateRequest) -> Flag:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{key}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(flag, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Flag, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/flags/types/flag.py` & `flipt-0.2.6/src/flipt/resources/flags/types/flag.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...variants.types.variant import variant
+from ...variants.types.variant import Variant
 
 
-class flag(pydantic.BaseModel):
+class Flag(pydantic.BaseModel):
     key: str
     name: str
     description: str
     enabled: bool
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    variants: typing.List[variant]
+    variants: typing.List[Variant]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/flags/types/flag_create_request.py` & `flipt-0.2.6/src/flipt/resources/flags/types/flag_create_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class flagCreateRequest(pydantic.BaseModel):
+class FlagCreateRequest(pydantic.BaseModel):
     key: str
     name: str
     description: typing.Optional[str]
     enabled: typing.Optional[bool]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/flags/types/flag_list.py` & `flipt-0.2.6/src/flipt/resources/segments/types/segment_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .flag import flag
+from .segment import Segment
 
 
-class flagList(pydantic.BaseModel):
-    flags: typing.List[flag]
+class SegmentList(pydantic.BaseModel):
+    segments: typing.List[Segment]
     next_page_token: str = pydantic.Field(alias="nextPageToken")
     total_count: int = pydantic.Field(alias="totalCount")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/flags/types/flag_update_request.py` & `flipt-0.2.6/src/flipt/resources/flags/types/flag_update_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class flagUpdateRequest(pydantic.BaseModel):
+class FlagUpdateRequest(pydantic.BaseModel):
     name: str
     description: typing.Optional[str]
     enabled: typing.Optional[bool]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/namespaces/client.py` & `flipt-0.2.6/src/flipt/resources/namespaces/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.namespace import namespace
-from .types.namespace_create_request import namespaceCreateRequest
-from .types.namespace_list import namespaceList
-from .types.namespace_update_request import namespaceUpdateRequest
+from .types.namespace import Namespace
+from .types.namespace_create_request import NamespaceCreateRequest
+from .types.namespace_list import NamespaceList
+from .types.namespace_update_request import NamespaceUpdateRequest
 
 
 class NamespacesClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -26,91 +26,96 @@
 
     def list(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> namespaceList:
+    ) -> NamespaceList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/v1/namespaces"),
             params={"limit": limit, "offset": offset, "pageToken": page_token},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespaceList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(NamespaceList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, *, request: namespaceCreateRequest) -> namespace:
+    def create(self, *, request: NamespaceCreateRequest) -> Namespace:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", "api/v1/namespaces"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespace, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Namespace, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, key: str) -> namespace:
+    def get(self, key: str) -> Namespace:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{key}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespace, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Namespace, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, key: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{key}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, key: str, *, request: namespaceUpdateRequest) -> namespace:
+    def update(self, key: str, *, request: NamespaceUpdateRequest) -> Namespace:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{key}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespace, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Namespace, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -123,94 +128,99 @@
 
     async def list(
         self,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> namespaceList:
+    ) -> NamespaceList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/v1/namespaces"),
                 params={"limit": limit, "offset": offset, "pageToken": page_token},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespaceList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(NamespaceList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, *, request: namespaceCreateRequest) -> namespace:
+    async def create(self, *, request: NamespaceCreateRequest) -> Namespace:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", "api/v1/namespaces"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespace, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Namespace, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, key: str) -> namespace:
+    async def get(self, key: str) -> Namespace:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{key}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespace, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Namespace, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, key: str) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "DELETE",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{key}"),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, key: str, *, request: namespaceUpdateRequest) -> namespace:
+    async def update(self, key: str, *, request: NamespaceUpdateRequest) -> Namespace:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{key}"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(namespace, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Namespace, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/namespaces/types/namespace.py` & `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class namespace(pydantic.BaseModel):
+class Namespace(pydantic.BaseModel):
     key: str
     name: str
     description: str
     protected: bool
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
```

### Comparing `flipt-0.2.5/src/flipt/resources/namespaces/types/namespace_create_request.py` & `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_create_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class namespaceCreateRequest(pydantic.BaseModel):
+class NamespaceCreateRequest(pydantic.BaseModel):
     key: str
     name: str
     description: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/namespaces/types/namespace_list.py` & `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .namespace import namespace
+from .namespace import Namespace
 
 
-class namespaceList(pydantic.BaseModel):
-    namespaces: typing.List[namespace]
+class NamespaceList(pydantic.BaseModel):
+    namespaces: typing.List[Namespace]
     next_page_token: str = pydantic.Field(alias="nextPageToken")
     total_count: int = pydantic.Field(alias="totalCount")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/namespaces/types/namespace_update_request.py` & `flipt-0.2.6/src/flipt/resources/namespaces/types/namespace_update_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class namespaceUpdateRequest(pydantic.BaseModel):
+class NamespaceUpdateRequest(pydantic.BaseModel):
     name: str
     description: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/rules/client.py` & `flipt-0.2.6/src/flipt/resources/rules/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.rule import rule
-from .types.rule_create_request import ruleCreateRequest
-from .types.rule_list import ruleList
-from .types.rule_order_request import ruleOrderRequest
-from .types.rule_update_request import ruleUpdateRequest
+from .types.rule import Rule
+from .types.rule_create_request import RuleCreateRequest
+from .types.rule_list import RuleList
+from .types.rule_order_request import RuleOrderRequest
+from .types.rule_update_request import RuleUpdateRequest
 
 
 class RulesClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -29,83 +29,87 @@
         self,
         namespace_key: str,
         flag_key: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> ruleList:
+    ) -> RuleList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules"
             ),
             params={"limit": limit, "offset": offset, "pageToken": page_token},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ruleList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RuleList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, namespace_key: str, flag_key: str, *, request: ruleCreateRequest) -> rule:
+    def create(self, namespace_key: str, flag_key: str, *, request: RuleCreateRequest) -> Rule:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules"
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(rule, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Rule, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def order(self, namespace_key: str, flag_key: str, *, request: ruleOrderRequest) -> None:
+    def order(self, namespace_key: str, flag_key: str, *, request: RuleOrderRequest) -> None:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/order"
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, namespace_key: str, flag_key: str, id: str) -> rule:
+    def get(self, namespace_key: str, flag_key: str, id: str) -> Rule:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{id}"
             ),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(rule, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Rule, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, namespace_key: str, flag_key: str, id: str) -> None:
@@ -113,33 +117,35 @@
             "DELETE",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{id}"
             ),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, namespace_key: str, flag_key: str, id: str, *, request: ruleUpdateRequest) -> None:
+    def update(self, namespace_key: str, flag_key: str, id: str, *, request: RuleUpdateRequest) -> None:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{id}"
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
@@ -157,87 +163,91 @@
         self,
         namespace_key: str,
         flag_key: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> ruleList:
+    ) -> RuleList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules"
                 ),
                 params={"limit": limit, "offset": offset, "pageToken": page_token},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(ruleList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(RuleList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, namespace_key: str, flag_key: str, *, request: ruleCreateRequest) -> rule:
+    async def create(self, namespace_key: str, flag_key: str, *, request: RuleCreateRequest) -> Rule:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules"
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(rule, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Rule, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def order(self, namespace_key: str, flag_key: str, *, request: ruleOrderRequest) -> None:
+    async def order(self, namespace_key: str, flag_key: str, *, request: RuleOrderRequest) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/order"
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, namespace_key: str, flag_key: str, id: str) -> rule:
+    async def get(self, namespace_key: str, flag_key: str, id: str) -> Rule:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{id}"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(rule, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Rule, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, namespace_key: str, flag_key: str, id: str) -> None:
@@ -246,34 +256,36 @@
                 "DELETE",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{id}"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, namespace_key: str, flag_key: str, id: str, *, request: ruleUpdateRequest) -> None:
+    async def update(self, namespace_key: str, flag_key: str, id: str, *, request: RuleUpdateRequest) -> None:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/rules/{id}"
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
```

### Comparing `flipt-0.2.5/src/flipt/resources/rules/types/rule.py` & `flipt-0.2.6/src/flipt/resources/rules/types/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...distributions.types.distribution import distribution
+from ...distributions.types.distribution import Distribution
 
 
-class rule(pydantic.BaseModel):
+class Rule(pydantic.BaseModel):
     id: str
     flag_key: str = pydantic.Field(alias="flagKey")
     segment_key: str = pydantic.Field(alias="segmentKey")
-    distributions: typing.List[distribution]
+    distributions: typing.List[Distribution]
     rank: int
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `flipt-0.2.5/src/flipt/resources/rules/types/rule_create_request.py` & `flipt-0.2.6/src/flipt/resources/rules/types/rule_update_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class ruleCreateRequest(pydantic.BaseModel):
+class RuleUpdateRequest(pydantic.BaseModel):
     segment_key: str = pydantic.Field(alias="segmentKey")
-    rank: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/rules/types/rule_list.py` & `flipt-0.2.6/src/flipt/resources/segments/types/segment_update_request.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .rule import rule
+from .segment_match_type import SegmentMatchType
 
 
-class ruleList(pydantic.BaseModel):
-    rules: typing.List[rule]
-    next_page_token: str = pydantic.Field(alias="nextPageToken")
-    total_count: int = pydantic.Field(alias="totalCount")
+class SegmentUpdateRequest(pydantic.BaseModel):
+    name: str
+    description: str
+    match_type: SegmentMatchType = pydantic.Field(alias="matchType")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/rules/types/rule_order_request.py` & `flipt-0.2.6/src/flipt/resources/rules/types/rule_order_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class ruleOrderRequest(pydantic.BaseModel):
+class RuleOrderRequest(pydantic.BaseModel):
     rule_ids: typing.List[str] = pydantic.Field(alias="ruleIds")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `flipt-0.2.5/src/flipt/resources/rules/types/rule_update_request.py` & `flipt-0.2.6/src/flipt/resources/rules/types/rule_create_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class ruleUpdateRequest(pydantic.BaseModel):
+class RuleCreateRequest(pydantic.BaseModel):
     segment_key: str = pydantic.Field(alias="segmentKey")
+    rank: int
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/segments/client.py` & `flipt-0.2.6/src/flipt/resources/segments/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.segment import segment
-from .types.segment_create_request import segmentCreateRequest
-from .types.segment_list import segmentList
-from .types.segment_update_request import segmentUpdateRequest
+from .types.segment import Segment
+from .types.segment_create_request import SegmentCreateRequest
+from .types.segment_list import SegmentList
+from .types.segment_update_request import SegmentUpdateRequest
 
 
 class SegmentsClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
@@ -27,91 +27,96 @@
     def list(
         self,
         namespace_key: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> segmentList:
+    ) -> SegmentList:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments"),
             params={"limit": limit, "offset": offset, "pageToken": page_token},
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segmentList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SegmentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def create(self, namespace_key: str, *, request: segmentCreateRequest) -> segment:
+    def create(self, namespace_key: str, *, request: SegmentCreateRequest) -> Segment:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segment, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Segment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def get(self, namespace_key: str, key: str) -> segment:
+    def get(self, namespace_key: str, key: str) -> Segment:
         _response = httpx.request(
             "GET",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments/{key}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segment, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Segment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, namespace_key: str, key: str) -> None:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments/{key}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, namespace_key: str, key: str, *, request: segmentUpdateRequest) -> segment:
+    def update(self, namespace_key: str, key: str, *, request: SegmentUpdateRequest) -> Segment:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments/{key}"),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segment, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Segment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
@@ -125,63 +130,66 @@
     async def list(
         self,
         namespace_key: str,
         *,
         limit: typing.Optional[int] = None,
         offset: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
-    ) -> segmentList:
+    ) -> SegmentList:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments"),
                 params={"limit": limit, "offset": offset, "pageToken": page_token},
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segmentList, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(SegmentList, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def create(self, namespace_key: str, *, request: segmentCreateRequest) -> segment:
+    async def create(self, namespace_key: str, *, request: SegmentCreateRequest) -> Segment:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments"),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segment, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Segment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def get(self, namespace_key: str, key: str) -> segment:
+    async def get(self, namespace_key: str, key: str) -> Segment:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "GET",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments/{key}"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segment, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Segment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, namespace_key: str, key: str) -> None:
@@ -190,35 +198,37 @@
                 "DELETE",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments/{key}"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, namespace_key: str, key: str, *, request: segmentUpdateRequest) -> segment:
+    async def update(self, namespace_key: str, key: str, *, request: SegmentUpdateRequest) -> Segment:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/segments/{key}"
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(segment, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Segment, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/segments/types/segment.py` & `flipt-0.2.6/src/flipt/resources/variants/types/variant_create_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,32 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...constraints.types.constraint import constraint
-from .segment_match_type import segmentMatchType
 
 
-class segment(pydantic.BaseModel):
+class VariantCreateRequest(pydantic.BaseModel):
     key: str
-    name: str
-    description: str
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    constraints: typing.List[constraint]
-    match_type: segmentMatchType = pydantic.Field(alias="matchType")
+    name: typing.Optional[str]
+    description: typing.Optional[str]
+    attachment: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `flipt-0.2.5/src/flipt/resources/segments/types/segment_create_request.py` & `flipt-0.2.6/src/flipt/resources/segments/types/segment_create_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .segment_match_type import segmentMatchType
+from .segment_match_type import SegmentMatchType
 
 
-class segmentCreateRequest(pydantic.BaseModel):
+class SegmentCreateRequest(pydantic.BaseModel):
     key: str
     name: str
     description: str
-    match_type: segmentMatchType = pydantic.Field(alias="matchType")
+    match_type: SegmentMatchType = pydantic.Field(alias="matchType")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/segments/types/segment_list.py` & `flipt-0.2.6/src/flipt/resources/variants/types/variant.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .segment import segment
 
 
-class segmentList(pydantic.BaseModel):
-    segments: typing.List[segment]
-    next_page_token: str = pydantic.Field(alias="nextPageToken")
-    total_count: int = pydantic.Field(alias="totalCount")
+class Variant(pydantic.BaseModel):
+    id: str
+    flag_key: str = pydantic.Field(alias="flagKey")
+    key: str
+    name: str
+    description: str
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+    attachment: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `flipt-0.2.5/src/flipt/resources/segments/types/segment_match_type.py` & `flipt-0.2.6/src/flipt/resources/segments/types/segment_match_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import enum
 import typing
 
 T_Result = typing.TypeVar("T_Result")
 
 
-class segmentMatchType(str, enum.Enum):
+class SegmentMatchType(str, enum.Enum):
     ALL_MATCH_TYPE = "ALL_MATCH_TYPE"
     ANY_MATCH_TYPE = "ANY_MATCH_TYPE"
 
     def visit(
         self, all_match_type: typing.Callable[[], T_Result], any_match_type: typing.Callable[[], T_Result]
     ) -> T_Result:
-        if self is segmentMatchType.ALL_MATCH_TYPE:
+        if self is SegmentMatchType.ALL_MATCH_TYPE:
             return all_match_type()
-        if self is segmentMatchType.ANY_MATCH_TYPE:
+        if self is SegmentMatchType.ANY_MATCH_TYPE:
             return any_match_type()
```

### Comparing `flipt-0.2.5/src/flipt/resources/segments/types/segment_update_request.py` & `flipt-0.2.6/src/flipt/resources/auth_method_oidc/types/oidc_callback_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .segment_match_type import segmentMatchType
+from ...auth.types.authentication import Authentication
 
 
-class segmentUpdateRequest(pydantic.BaseModel):
-    name: str
-    description: str
-    match_type: segmentMatchType = pydantic.Field(alias="matchType")
+class OidcCallbackResponse(pydantic.BaseModel):
+    authentication: Authentication
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `flipt-0.2.5/src/flipt/resources/variants/client.py` & `flipt-0.2.6/src/flipt/resources/variants/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 import httpx
 import pydantic
 
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import FliptApiEnvironment
-from .types.variant import variant
-from .types.variant_create_request import variantCreateRequest
-from .types.variant_update_request import variantUpdateRequest
+from .types.variant import Variant
+from .types.variant_create_request import VariantCreateRequest
+from .types.variant_update_request import VariantUpdateRequest
 
 
 class VariantsClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    def create(self, namespace_key: str, flag_key: str, *, request: variantCreateRequest) -> variant:
+    def create(self, namespace_key: str, flag_key: str, *, request: VariantCreateRequest) -> Variant:
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/variants"
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(variant, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Variant, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, namespace_key: str, flag_key: str, id: str) -> None:
@@ -47,64 +48,67 @@
             "DELETE",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/variants/{id}"
             ),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    def update(self, namespace_key: str, flag_key: str, id: str, *, request: variantUpdateRequest) -> variant:
+    def update(self, namespace_key: str, flag_key: str, id: str, *, request: VariantUpdateRequest) -> Variant:
         _response = httpx.request(
             "PUT",
             urllib.parse.urljoin(
                 f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/variants/{id}"
             ),
             json=jsonable_encoder(request),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
+            timeout=60,
         )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(variant, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Variant, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncVariantsClient:
     def __init__(
         self, *, environment: FliptApiEnvironment = FliptApiEnvironment.PRODUCTION, token: typing.Optional[str] = None
     ):
         self._environment = environment
         self._token = token
 
-    async def create(self, namespace_key: str, flag_key: str, *, request: variantCreateRequest) -> variant:
+    async def create(self, namespace_key: str, flag_key: str, *, request: VariantCreateRequest) -> Variant:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/variants"
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(variant, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Variant, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete(self, namespace_key: str, flag_key: str, id: str) -> None:
@@ -113,35 +117,37 @@
                 "DELETE",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/variants/{id}"
                 ),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
-    async def update(self, namespace_key: str, flag_key: str, id: str, *, request: variantUpdateRequest) -> variant:
+    async def update(self, namespace_key: str, flag_key: str, id: str, *, request: VariantUpdateRequest) -> Variant:
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "PUT",
                 urllib.parse.urljoin(
                     f"{self._environment.value}/", f"api/v1/namespaces/{namespace_key}/flags/{flag_key}/variants/{id}"
                 ),
                 json=jsonable_encoder(request),
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
+                timeout=60,
             )
         if 200 <= _response.status_code < 300:
-            return pydantic.parse_obj_as(variant, _response.json())  # type: ignore
+            return pydantic.parse_obj_as(Variant, _response.json())  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `flipt-0.2.5/src/flipt/resources/variants/types/variant.py` & `flipt-0.2.6/src/flipt/resources/constraints/types/constraint.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .constraint_comparison_type import ConstraintComparisonType
 
 
-class variant(pydantic.BaseModel):
+class Constraint(pydantic.BaseModel):
     id: str
-    flag_key: str = pydantic.Field(alias="flagKey")
-    key: str
-    name: str
+    segment_key: str = pydantic.Field(alias="segmentKey")
+    type: ConstraintComparisonType
+    property: str
+    operator: str
+    value: str
     description: str
     created_at: dt.datetime = pydantic.Field(alias="createdAt")
     updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
-    attachment: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

