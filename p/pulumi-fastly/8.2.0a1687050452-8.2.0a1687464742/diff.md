# Comparing `tmp/pulumi_fastly-8.2.0a1687050452.tar.gz` & `tmp/pulumi_fastly-8.2.0a1687464742.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_fastly-8.2.0a1687050452.tar", last modified: Sun Jun 18 01:12:45 2023, max compression
+gzip compressed data, was "pulumi_fastly-8.2.0a1687464742.tar", last modified: Thu Jun 22 20:17:37 2023, max compression
```

## Comparing `pulumi_fastly-8.2.0a1687050452.tar` & `pulumi_fastly-8.2.0a1687464742.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:45.112874 pulumi_fastly-8.2.0a1687050452/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-18 01:12:45.112874 pulumi_fastly-8.2.0a1687050452/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:45.112874 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   508272 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:45.112874 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/configstore.py
--rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/configstore_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_datacenters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_fastly_ip_ranges.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_package_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_activation_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_configuration_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_platform_certificate_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_private_key_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_subscription_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_waf_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)   452937 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_acl_entries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)    96684 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_dictionary_items.py
--rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_dynamic_snippet_content.py
--rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_vcl.py
--rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_waf_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_mutual_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_platform_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_private_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_subscription_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 01:12:45.112874 pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-18 01:12:45.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-18 01:12:45.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:12:45.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 01:12:45.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 01:12:45.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-18 01:12:45.000000 pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 01:12:45.112874 pulumi_fastly-8.2.0a1687050452/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-18 01:12:44.000000 pulumi_fastly-8.2.0a1687050452/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:17:37.090606 pulumi_fastly-8.2.0a1687464742/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-22 20:17:37.090606 pulumi_fastly-8.2.0a1687464742/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:17:37.086606 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   509608 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:17:37.090606 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12971 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/configstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11398 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/configstore_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_datacenters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_fastly_ip_ranges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_package_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_activation_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_configuration_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4992 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_platform_certificate_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_private_key_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_subscription_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_waf_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)   454051 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13944 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_acl_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11775 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96684 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_dictionary_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14198 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_dynamic_snippet_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)   124679 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_vcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81770 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_waf_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23023 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_mutual_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26052 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_platform_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_private_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34762 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_subscription_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:17:37.090606 pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-22 20:17:37.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-22 20:17:37.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:17:37.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:17:37.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 20:17:37.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 20:17:37.000000 pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:17:37.090606 pulumi_fastly-8.2.0a1687464742/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-22 20:17:36.000000 pulumi_fastly-8.2.0a1687464742/setup.py
```

### Comparing `pulumi_fastly-8.2.0a1687050452/PKG-INFO` & `pulumi_fastly-8.2.0a1687464742/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_fastly
-Version: 8.2.0a1687050452
+Version: 8.2.0a1687464742
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.2.0a1687050452/README.md` & `pulumi_fastly-8.2.0a1687464742/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/__init__.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/_inputs.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3248,14 +3248,15 @@
 class ServiceComputeLoggingS3Args:
     def __init__(__self__, *,
                  bucket_name: pulumi.Input[str],
                  name: pulumi.Input[str],
                  acl: Optional[pulumi.Input[str]] = None,
                  compression_codec: Optional[pulumi.Input[str]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
+                 file_max_bytes: Optional[pulumi.Input[int]] = None,
                  gzip_level: Optional[pulumi.Input[int]] = None,
                  message_type: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  period: Optional[pulumi.Input[int]] = None,
                  public_key: Optional[pulumi.Input[str]] = None,
                  redundancy: Optional[pulumi.Input[str]] = None,
                  s3_access_key: Optional[pulumi.Input[str]] = None,
@@ -3266,14 +3267,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
+        :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param pulumi.Input[str] public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param pulumi.Input[str] redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param pulumi.Input[str] s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
@@ -3287,14 +3289,16 @@
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
+        if file_max_bytes is not None:
+            pulumi.set(__self__, "file_max_bytes", file_max_bytes)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
             pulumi.set(__self__, "message_type", message_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if period is not None:
@@ -3373,14 +3377,26 @@
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
+    @pulumi.getter(name="fileMaxBytes")
+    def file_max_bytes(self) -> Optional[pulumi.Input[int]]:
+        """
+        Maximum size of an uploaded log file, if non-zero.
+        """
+        return pulumi.get(self, "file_max_bytes")
+
+    @file_max_bytes.setter
+    def file_max_bytes(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "file_max_bytes", value)
+
+    @property
     @pulumi.getter(name="gzipLevel")
     def gzip_level(self) -> Optional[pulumi.Input[int]]:
         """
         Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         """
         return pulumi.get(self, "gzip_level")
 
@@ -9548,14 +9564,15 @@
 class ServiceVclLoggingS3Args:
     def __init__(__self__, *,
                  bucket_name: pulumi.Input[str],
                  name: pulumi.Input[str],
                  acl: Optional[pulumi.Input[str]] = None,
                  compression_codec: Optional[pulumi.Input[str]] = None,
                  domain: Optional[pulumi.Input[str]] = None,
+                 file_max_bytes: Optional[pulumi.Input[int]] = None,
                  format: Optional[pulumi.Input[str]] = None,
                  format_version: Optional[pulumi.Input[int]] = None,
                  gzip_level: Optional[pulumi.Input[int]] = None,
                  message_type: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  period: Optional[pulumi.Input[int]] = None,
                  placement: Optional[pulumi.Input[str]] = None,
@@ -9570,14 +9587,15 @@
                  timestamp_format: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] bucket_name: The name of the bucket in which to store the logs
         :param pulumi.Input[str] name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param pulumi.Input[str] acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
         :param pulumi.Input[str] compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param pulumi.Input[str] domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
+        :param pulumi.Input[int] file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param pulumi.Input[str] format: Apache-style string or VCL variables to use for log formatting.
         :param pulumi.Input[int] format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2).
         :param pulumi.Input[int] gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param pulumi.Input[str] message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param pulumi.Input[str] path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param pulumi.Input[int] period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param pulumi.Input[str] placement: Where in the generated VCL the logging call should be placed.
@@ -9595,14 +9613,16 @@
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
+        if file_max_bytes is not None:
+            pulumi.set(__self__, "file_max_bytes", file_max_bytes)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if format_version is not None:
             pulumi.set(__self__, "format_version", format_version)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
@@ -9689,14 +9709,26 @@
         return pulumi.get(self, "domain")
 
     @domain.setter
     def domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain", value)
 
     @property
+    @pulumi.getter(name="fileMaxBytes")
+    def file_max_bytes(self) -> Optional[pulumi.Input[int]]:
+        """
+        Maximum size of an uploaded log file, if non-zero.
+        """
+        return pulumi.get(self, "file_max_bytes")
+
+    @file_max_bytes.setter
+    def file_max_bytes(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "file_max_bytes", value)
+
+    @property
     @pulumi.getter
     def format(self) -> Optional[pulumi.Input[str]]:
         """
         Apache-style string or VCL variables to use for log formatting.
         """
         return pulumi.get(self, "format")
```

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/_utilities.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/config/vars.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/configstore.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/configstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/configstore_entries.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/configstore_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_datacenters.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_datacenters.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_dictionaries.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_dictionaries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_fastly_ip_ranges.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_fastly_ip_ranges.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_package_hash.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_package_hash.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_services.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_activation.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_activation_ids.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_activation_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_certificate.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_certificate_ids.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_configuration.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_configuration_ids.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_configuration_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_domain.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_platform_certificate.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_platform_certificate_ids.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_platform_certificate_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_private_key.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_private_key_ids.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_private_key_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_subscription.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_tls_subscription_ids.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_tls_subscription_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/get_waf_rules.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/get_waf_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/kvstore.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/kvstore.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/outputs.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/outputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -2916,14 +2916,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bucketName":
             suggest = "bucket_name"
         elif key == "compressionCodec":
             suggest = "compression_codec"
+        elif key == "fileMaxBytes":
+            suggest = "file_max_bytes"
         elif key == "gzipLevel":
             suggest = "gzip_level"
         elif key == "messageType":
             suggest = "message_type"
         elif key == "publicKey":
             suggest = "public_key"
         elif key == "s3AccessKey":
@@ -2952,14 +2954,15 @@
 
     def __init__(__self__, *,
                  bucket_name: str,
                  name: str,
                  acl: Optional[str] = None,
                  compression_codec: Optional[str] = None,
                  domain: Optional[str] = None,
+                 file_max_bytes: Optional[int] = None,
                  gzip_level: Optional[int] = None,
                  message_type: Optional[str] = None,
                  path: Optional[str] = None,
                  period: Optional[int] = None,
                  public_key: Optional[str] = None,
                  redundancy: Optional[str] = None,
                  s3_access_key: Optional[str] = None,
@@ -2970,14 +2973,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param str domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
+        :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param str public_key: A PGP public key that Fastly will use to encrypt your log files before writing them to disk
         :param str redundancy: The S3 storage class (redundancy level). Should be one of: `standard`, `intelligent_tiering`, `standard_ia`, `onezone_ia`, `glacier`, `glacier_ir`, `deep_archive`, or `reduced_redundancy`
         :param str s3_access_key: AWS Access Key of an account with the required permissions to post logs. It is **strongly** recommended you create a separate IAM user with permissions to only operate on this Bucket. This key will be not be encrypted. Not required if `iam_role` is provided. You can provide this key via an environment variable, `FASTLY_S3_ACCESS_KEY`
@@ -2991,14 +2995,16 @@
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
+        if file_max_bytes is not None:
+            pulumi.set(__self__, "file_max_bytes", file_max_bytes)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
             pulumi.set(__self__, "message_type", message_type)
         if path is not None:
             pulumi.set(__self__, "path", path)
         if period is not None:
@@ -3057,14 +3063,22 @@
     def domain(self) -> Optional[str]:
         """
         If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
         """
         return pulumi.get(self, "domain")
 
     @property
+    @pulumi.getter(name="fileMaxBytes")
+    def file_max_bytes(self) -> Optional[int]:
+        """
+        Maximum size of an uploaded log file, if non-zero.
+        """
+        return pulumi.get(self, "file_max_bytes")
+
+    @property
     @pulumi.getter(name="gzipLevel")
     def gzip_level(self) -> Optional[int]:
         """
         Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         """
         return pulumi.get(self, "gzip_level")
 
@@ -8585,14 +8599,16 @@
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "bucketName":
             suggest = "bucket_name"
         elif key == "compressionCodec":
             suggest = "compression_codec"
+        elif key == "fileMaxBytes":
+            suggest = "file_max_bytes"
         elif key == "formatVersion":
             suggest = "format_version"
         elif key == "gzipLevel":
             suggest = "gzip_level"
         elif key == "messageType":
             suggest = "message_type"
         elif key == "publicKey":
@@ -8625,14 +8641,15 @@
 
     def __init__(__self__, *,
                  bucket_name: str,
                  name: str,
                  acl: Optional[str] = None,
                  compression_codec: Optional[str] = None,
                  domain: Optional[str] = None,
+                 file_max_bytes: Optional[int] = None,
                  format: Optional[str] = None,
                  format_version: Optional[int] = None,
                  gzip_level: Optional[int] = None,
                  message_type: Optional[str] = None,
                  path: Optional[str] = None,
                  period: Optional[int] = None,
                  placement: Optional[str] = None,
@@ -8647,14 +8664,15 @@
                  timestamp_format: Optional[str] = None):
         """
         :param str bucket_name: The name of the bucket in which to store the logs
         :param str name: The unique name of the S3 logging endpoint. It is important to note that changing this attribute will delete and recreate the resource
         :param str acl: The AWS [Canned ACL](https://docs.aws.amazon.com/AmazonS3/latest/userguide/acl-overview.html#canned-acl) to use for objects uploaded to the S3 bucket. Options are: `private`, `public-read`, `public-read-write`, `aws-exec-read`, `authenticated-read`, `bucket-owner-read`, `bucket-owner-full-control`
         :param str compression_codec: The codec used for compression of your logs. Valid values are zstd, snappy, and gzip. If the specified codec is "gzip", gzip*level will default to 3. To specify a different level, leave compression*codec blank and explicitly set the level using gzip*level. Specifying both compression*codec and gzip_level in the same API request will result in an error.
         :param str domain: If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
+        :param int file_max_bytes: Maximum size of an uploaded log file, if non-zero.
         :param str format: Apache-style string or VCL variables to use for log formatting.
         :param int format_version: The version of the custom logging format used for the configured endpoint. Can be either 1 or 2. (Default: 2).
         :param int gzip_level: Level of Gzip compression from `0-9`. `0` means no compression. `1` is the fastest and the least compressed version, `9` is the slowest and the most compressed version. Default `0`
         :param str message_type: How the message should be formatted. Can be either `classic`, `loggly`, `logplex` or `blank`. Default is `classic`
         :param str path: Path to store the files. Must end with a trailing slash. If this field is left empty, the files will be saved in the bucket's root path
         :param int period: How frequently the logs should be transferred, in seconds. Default `3600`
         :param str placement: Where in the generated VCL the logging call should be placed.
@@ -8672,14 +8690,16 @@
         pulumi.set(__self__, "name", name)
         if acl is not None:
             pulumi.set(__self__, "acl", acl)
         if compression_codec is not None:
             pulumi.set(__self__, "compression_codec", compression_codec)
         if domain is not None:
             pulumi.set(__self__, "domain", domain)
+        if file_max_bytes is not None:
+            pulumi.set(__self__, "file_max_bytes", file_max_bytes)
         if format is not None:
             pulumi.set(__self__, "format", format)
         if format_version is not None:
             pulumi.set(__self__, "format_version", format_version)
         if gzip_level is not None:
             pulumi.set(__self__, "gzip_level", gzip_level)
         if message_type is not None:
@@ -8746,14 +8766,22 @@
     def domain(self) -> Optional[str]:
         """
         If you created the S3 bucket outside of `us-east-1`, then specify the corresponding bucket endpoint. Example: `s3-us-west-2.amazonaws.com`
         """
         return pulumi.get(self, "domain")
 
     @property
+    @pulumi.getter(name="fileMaxBytes")
+    def file_max_bytes(self) -> Optional[int]:
+        """
+        Maximum size of an uploaded log file, if non-zero.
+        """
+        return pulumi.get(self, "file_max_bytes")
+
+    @property
     @pulumi.getter
     def format(self) -> Optional[str]:
         """
         Apache-style string or VCL variables to use for log formatting.
         """
         return pulumi.get(self, "format")
```

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/provider.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_acl_entries.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_acl_entries.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_authorization.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_compute.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_compute.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_dictionary_items.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_dictionary_items.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_dynamic_snippet_content.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_dynamic_snippet_content.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_vcl.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_vcl.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/service_waf_configuration.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/service_waf_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_activation.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_activation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_certificate.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_mutual_authentication.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_mutual_authentication.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_platform_certificate.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_platform_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_private_key.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_subscription.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/tls_subscription_validation.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/tls_subscription_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly/user.py` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/PKG-INFO` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-fastly
-Version: 8.2.0a1687050452
+Version: 8.2.0a1687464742
 Summary: A Pulumi package for creating and managing fastly cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-fastly
 Keywords: pulumi fastly
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_fastly-8.2.0a1687050452/pulumi_fastly.egg-info/SOURCES.txt` & `pulumi_fastly-8.2.0a1687464742/pulumi_fastly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_fastly-8.2.0a1687050452/setup.py` & `pulumi_fastly-8.2.0a1687464742/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "8.2.0a1687050452"
-PLUGIN_VERSION = "8.2.0-alpha.1687050452+4f478efb"
+VERSION = "8.2.0a1687464742"
+PLUGIN_VERSION = "8.2.0-alpha.1687464742+c7d23450"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'fastly', PLUGIN_VERSION])
         except OSError as error:
```

