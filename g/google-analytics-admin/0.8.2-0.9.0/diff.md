# Comparing `tmp/google-analytics-admin-0.8.2.tar.gz` & `tmp/google-analytics-admin-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-analytics-admin-0.8.2.tar", last modified: Mon Jun  6 21:28:27 2022, max compression
+gzip compressed data, was "google-analytics-admin-0.9.0.tar", last modified: Wed Jul 20 13:08:13 2022, max compression
```

## Comparing `google-analytics-admin-0.8.2.tar` & `google-analytics-admin-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,72 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.904902 google-analytics-admin-0.8.2/
--rw-rw-r--   0 root         (0)     1003    11358 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3498 2022-06-06 21:28:27.904902 google-analytics-admin-0.8.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2715 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.892902 google-analytics-admin-0.8.2/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.896902 google-analytics-admin-0.8.2/google/analytics/
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.896902 google-analytics-admin-0.8.2/google/analytics/admin/
--rw-rw-r--   0 root         (0)     1003     9218 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin/__init__.py
--rw-rw-r--   0 root         (0)     1003       83 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.896902 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/
--rw-rw-r--   0 root         (0)     1003     9028 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003    20666 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       83 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.896902 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/
--rw-rw-r--   0 root         (0)     1003      797 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/__init__.py
--rw-rw-r--   0 root         (0)     1003   280502 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   311072 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/client.py
--rw-rw-r--   0 root         (0)     1003    80985 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/
--rw-rw-r--   0 root         (0)     1003     1264 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    41504 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003   103620 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003   105773 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/types/
--rw-rw-r--   0 root         (0)     1003     8819 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    69628 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/types/analytics_admin.py
--rw-rw-r--   0 root         (0)     1003    52855 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/types/resources.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/
--rw-r--r--   0 root         (0)     1003     3498 2022-06-06 21:28:27.000000 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1610 2022-06-06 21:28:27.000000 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-06-06 21:28:27.000000 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       24 2022-06-06 21:28:27.000000 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-06-06 21:28:27.000000 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      128 2022-06-06 21:28:27.000000 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-06-06 21:28:27.000000 google-analytics-admin-0.8.2/google_analytics_admin.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2022-06-06 21:28:27.904902 google-analytics-admin-0.8.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2367 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-06-06 21:28:27.900902 google-analytics-admin-0.8.2/tests/unit/gapic/admin_v1alpha/
--rw-rw-r--   0 root         (0)     1003      600 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/tests/unit/gapic/admin_v1alpha/__init__.py
--rw-rw-r--   0 root         (0)     1003   783584 2022-06-06 21:25:56.000000 google-analytics-admin-0.8.2/tests/unit/gapic/admin_v1alpha/test_analytics_admin_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.818628 google-analytics-admin-0.9.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4387 2022-07-20 13:08:13.818628 google-analytics-admin-0.9.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3654 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.806630 google-analytics-admin-0.9.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.806630 google-analytics-admin-0.9.0/google/analytics/
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.806630 google-analytics-admin-0.9.0/google/analytics/admin/
+-rw-rw-r--   0 root         (0)     1003     9218 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin/__init__.py
+-rw-rw-r--   0 root         (0)     1003       83 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.806630 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/
+-rw-rw-r--   0 root         (0)     1003     9028 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20666 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       83 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.806630 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.810630 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/
+-rw-rw-r--   0 root         (0)     1003      797 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   280502 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   311130 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/client.py
+-rw-rw-r--   0 root         (0)     1003    80985 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.810630 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1264 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41823 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003   103703 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003   105856 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.810630 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/types/
+-rw-rw-r--   0 root         (0)     1003     8819 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    69628 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/types/analytics_admin.py
+-rw-rw-r--   0 root         (0)     1003    52855 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/types/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.810630 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/
+-rw-rw-r--   0 root         (0)     1003     5832 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13338 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       83 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.810630 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.814629 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/
+-rw-rw-r--   0 root         (0)     1003      797 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003   188890 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   211264 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/client.py
+-rw-rw-r--   0 root         (0)     1003    58634 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.814629 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1264 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28588 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    69673 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    71215 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/analytics_admin_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.814629 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     5623 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    46286 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/types/analytics_admin.py
+-rw-rw-r--   0 root         (0)     1003    39619 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/google/analytics/admin_v1beta/types/resources.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.814629 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/
+-rw-r--r--   0 root         (0)     1003     4387 2022-07-20 13:08:13.000000 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2688 2022-07-20 13:08:13.000000 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-07-20 13:08:13.000000 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       24 2022-07-20 13:08:13.000000 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-07-20 13:08:13.000000 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      160 2022-07-20 13:08:13.000000 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-07-20 13:08:13.000000 google-analytics-admin-0.9.0/google_analytics_admin.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2022-07-20 13:08:13.818628 google-analytics-admin-0.9.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2166 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.814629 google-analytics-admin-0.9.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.814629 google-analytics-admin-0.9.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.814629 google-analytics-admin-0.9.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.818628 google-analytics-admin-0.9.0/tests/unit/gapic/admin_v1alpha/
+-rw-rw-r--   0 root         (0)     1003      600 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/tests/unit/gapic/admin_v1alpha/__init__.py
+-rw-rw-r--   0 root         (0)     1003   785641 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/tests/unit/gapic/admin_v1alpha/test_analytics_admin_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-07-20 13:08:13.818628 google-analytics-admin-0.9.0/tests/unit/gapic/admin_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/tests/unit/gapic/admin_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   547127 2022-07-20 13:05:37.000000 google-analytics-admin-0.9.0/tests/unit/gapic/admin_v1beta/test_analytics_admin_service.py
```

### Comparing `google-analytics-admin-0.8.2/LICENSE` & `google-analytics-admin-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/MANIFEST.in` & `google-analytics-admin-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/PKG-INFO` & `google-analytics-admin-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Metadata-Version: 2.1
 Name: google-analytics-admin
-Version: 0.8.2
+Version: 0.9.0
 Home-page: https://github.com/googleapis/python-analytics-admin
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Analytics Admin API
 =====================================
 
-|alpha| |pypi| |versions|
+|preview| |pypi| |versions|
 
-`Analytics Admin API`_
+`Analytics Admin API`_: allows you to manage Google Analytics accounts and properties.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
-.. |alpha| image:: https://img.shields.io/badge/support-alpha-orange.svg
-   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#alpha-support
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-analytics-admin.svg
    :target: https://pypi.org/project/google-analytics-admin/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-analytics-admin.svg
    :target: https://pypi.org/project/google-analytics-admin/
 .. _Analytics Admin API: https://developers.google.com/analytics/
 .. _Client Library Documentation: https://googleapis.dev/python/analyticsadmin/latest
 .. _Product Documentation:  https://developers.google.com/analytics/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
-1. `Enable the Analytics Admin API.`_
-2. `Setup Authentication.`_
-3. `Install the library.`_
-
-.. _Enable the Analytics Admin API.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_1_enable_the_api
-.. _Setup Authentication.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_2_configure_authentication
-.. _Install the library.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_3_install_the_client_library
-
+1. `Select or create a Cloud Platform project.`_
+2. `Enable billing for your project.`_
+3. `Enable the Analytics Admin API.`_
+4. `Setup Authentication.`_
+
+.. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
+.. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
+.. _Enable the Analytics Admin API.:  https://developers.google.com/analytics/
+.. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
 dependencies and versions, and indirectly permissions.
@@ -63,14 +63,39 @@
 With `virtualenv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
 .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
 
+Code samples and snippets
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Code samples and snippets live in the `samples/` folder.
+
+
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
+Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
+Python.
+
+Python >= 3.7
+
+.. _active: https://devguide.python.org/devcycle/#in-development-main-branch
+.. _maintenance: https://devguide.python.org/devcycle/#maintenance-branches
+
+Unsupported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Python <= 3.6
+
+If you are using an `end-of-life`_
+version of Python, we recommend that you update as soon as possible to an actively supported version.
+
+.. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
+
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
@@ -91,9 +116,12 @@
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Analytics Admin API
    to see other available methods on the client.
 -  Read the `Analytics Admin API Product documentation`_ to learn
    more about the product and see How-to Guides.
+-  View this `README`_ to see the full list of Cloud
+   APIs that we cover.
 
 .. _Analytics Admin API Product documentation:  https://developers.google.com/analytics/
+.. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-analytics-admin-0.8.2/README.rst` & `google-analytics-admin-0.9.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Python Client for Analytics Admin API
 =====================================
 
-|alpha| |pypi| |versions|
+|preview| |pypi| |versions|
 
-`Analytics Admin API`_
+`Analytics Admin API`_: allows you to manage Google Analytics accounts and properties.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
-.. |alpha| image:: https://img.shields.io/badge/support-alpha-orange.svg
-   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#alpha-support
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-analytics-admin.svg
    :target: https://pypi.org/project/google-analytics-admin/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-analytics-admin.svg
    :target: https://pypi.org/project/google-analytics-admin/
 .. _Analytics Admin API: https://developers.google.com/analytics/
 .. _Client Library Documentation: https://googleapis.dev/python/analyticsadmin/latest
 .. _Product Documentation:  https://developers.google.com/analytics/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
-1. `Enable the Analytics Admin API.`_
-2. `Setup Authentication.`_
-3. `Install the library.`_
-
-.. _Enable the Analytics Admin API.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_1_enable_the_api
-.. _Setup Authentication.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_2_configure_authentication
-.. _Install the library.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_3_install_the_client_library
-
+1. `Select or create a Cloud Platform project.`_
+2. `Enable billing for your project.`_
+3. `Enable the Analytics Admin API.`_
+4. `Setup Authentication.`_
+
+.. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
+.. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
+.. _Enable the Analytics Admin API.:  https://developers.google.com/analytics/
+.. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
 dependencies and versions, and indirectly permissions.
@@ -42,14 +43,39 @@
 With `virtualenv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
 .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
 
+Code samples and snippets
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Code samples and snippets live in the `samples/` folder.
+
+
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
+Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
+Python.
+
+Python >= 3.7
+
+.. _active: https://devguide.python.org/devcycle/#in-development-main-branch
+.. _maintenance: https://devguide.python.org/devcycle/#maintenance-branches
+
+Unsupported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Python <= 3.6
+
+If you are using an `end-of-life`_
+version of Python, we recommend that you update as soon as possible to an actively supported version.
+
+.. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
+
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
@@ -70,9 +96,12 @@
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Analytics Admin API
    to see other available methods on the client.
 -  Read the `Analytics Admin API Product documentation`_ to learn
    more about the product and see How-to Guides.
+-  View this `README`_ to see the full list of Cloud
+   APIs that we cover.
 
 .. _Analytics Admin API Product documentation:  https://developers.google.com/analytics/
+.. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin/__init__.py` & `google-analytics-admin-0.9.0/google/analytics/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/__init__.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/gapic_metadata.json` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/__init__.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/__init__.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/async_client.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/client.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -711,14 +711,15 @@
                 credentials_file=client_options.credentials_file,
                 host=api_endpoint,
                 scopes=client_options.scopes,
                 client_cert_source_for_mtls=client_cert_source_func,
                 quota_project_id=client_options.quota_project_id,
                 client_info=client_info,
                 always_use_jwt_access=True,
+                api_audience=client_options.api_audience,
             )
 
     def get_account(
         self,
         request: Union[analytics_admin.GetAccountRequest, dict] = None,
         *,
         name: str = None,
```

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/pagers.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/__init__.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/base.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         host: str = DEFAULT_HOST,
         credentials: ga_credentials.Credentials = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
         **kwargs,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
@@ -83,19 +84,14 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
         """
 
-        # Save the hostname. Default to port 443 (HTTPS) if none is specified.
-        if ":" not in host:
-            host += ":443"
-        self._host = host
-
         scopes_kwargs = {"scopes": scopes, "default_scopes": self.AUTH_SCOPES}
 
         # Save the scopes.
         self._scopes = scopes
 
         # If no credentials are provided, then determine the appropriate
         # defaults.
@@ -108,26 +104,36 @@
             credentials, _ = google.auth.load_credentials_from_file(
                 credentials_file, **scopes_kwargs, quota_project_id=quota_project_id
             )
         elif credentials is None:
             credentials, _ = google.auth.default(
                 **scopes_kwargs, quota_project_id=quota_project_id
             )
+            # Don't apply audience if the credentials file passed from user.
+            if hasattr(credentials, "with_gdch_audience"):
+                credentials = credentials.with_gdch_audience(
+                    api_audience if api_audience else host
+                )
 
         # If the credentials are service account credentials, then always try to use self signed JWT.
         if (
             always_use_jwt_access
             and isinstance(credentials, service_account.Credentials)
             and hasattr(service_account.Credentials, "with_always_use_jwt_access")
         ):
             credentials = credentials.with_always_use_jwt_access(True)
 
         # Save the credentials.
         self._credentials = credentials
 
+        # Save the hostname. Default to port 443 (HTTPS) if none is specified.
+        if ":" not in host:
+            host += ":443"
+        self._host = host
+
     def _prep_wrapped_messages(self, client_info):
         # Precompute the wrapped methods.
         self._wrapped_methods = {
             self.get_account: gapic_v1.method.wrap_method(
                 self.get_account,
                 default_timeout=None,
                 client_info=client_info,
```

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         api_mtls_endpoint: str = None,
         client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
         ssl_channel_credentials: grpc.ChannelCredentials = None,
         client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
             credentials (Optional[google.auth.credentials.Credentials]): The
@@ -149,14 +150,15 @@
             host=host,
             credentials=credentials,
             credentials_file=credentials_file,
             scopes=scopes,
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
+            api_audience=api_audience,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
```

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc_asyncio.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,15 @@
         api_mtls_endpoint: str = None,
         client_cert_source: Callable[[], Tuple[bytes, bytes]] = None,
         ssl_channel_credentials: grpc.ChannelCredentials = None,
         client_cert_source_for_mtls: Callable[[], Tuple[bytes, bytes]] = None,
         quota_project_id=None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
+        api_audience: Optional[str] = None,
     ) -> None:
         """Instantiate the transport.
 
         Args:
             host (Optional[str]):
                  The hostname to connect to.
             credentials (Optional[google.auth.credentials.Credentials]): The
@@ -194,14 +195,15 @@
             host=host,
             credentials=credentials,
             credentials_file=credentials_file,
             scopes=scopes,
             quota_project_id=quota_project_id,
             client_info=client_info,
             always_use_jwt_access=always_use_jwt_access,
+            api_audience=api_audience,
         )
 
         if not self._grpc_channel:
             self._grpc_channel = type(self).create_channel(
                 self._host,
                 # use the credentials which are saved
                 credentials=self._credentials,
```

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/types/__init__.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/types/analytics_admin.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/types/analytics_admin.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google/analytics/admin_v1alpha/types/resources.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1alpha/types/resources.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/google_analytics_admin.egg-info/PKG-INFO` & `google-analytics-admin-0.9.0/google_analytics_admin.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,61 @@
 Metadata-Version: 2.1
 Name: google-analytics-admin
-Version: 0.8.2
+Version: 0.9.0
 Home-page: https://github.com/googleapis/python-analytics-admin
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 License-File: LICENSE
 
 Python Client for Analytics Admin API
 =====================================
 
-|alpha| |pypi| |versions|
+|preview| |pypi| |versions|
 
-`Analytics Admin API`_
+`Analytics Admin API`_: allows you to manage Google Analytics accounts and properties.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
-.. |alpha| image:: https://img.shields.io/badge/support-alpha-orange.svg
-   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#alpha-support
+.. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
+   :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-analytics-admin.svg
    :target: https://pypi.org/project/google-analytics-admin/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-analytics-admin.svg
    :target: https://pypi.org/project/google-analytics-admin/
 .. _Analytics Admin API: https://developers.google.com/analytics/
 .. _Client Library Documentation: https://googleapis.dev/python/analyticsadmin/latest
 .. _Product Documentation:  https://developers.google.com/analytics/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
-1. `Enable the Analytics Admin API.`_
-2. `Setup Authentication.`_
-3. `Install the library.`_
-
-.. _Enable the Analytics Admin API.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_1_enable_the_api
-.. _Setup Authentication.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_2_configure_authentication
-.. _Install the library.: https://developers.google.com/analytics/devguides/config/admin/v1/quickstart-client-libraries#step_3_install_the_client_library
-
+1. `Select or create a Cloud Platform project.`_
+2. `Enable billing for your project.`_
+3. `Enable the Analytics Admin API.`_
+4. `Setup Authentication.`_
+
+.. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
+.. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
+.. _Enable the Analytics Admin API.:  https://developers.google.com/analytics/
+.. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
 dependencies and versions, and indirectly permissions.
@@ -63,14 +63,39 @@
 With `virtualenv`_, it's possible to install this library without needing system
 install permissions, and without clashing with the installed system
 dependencies.
 
 .. _`virtualenv`: https://virtualenv.pypa.io/en/latest/
 
 
+Code samples and snippets
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Code samples and snippets live in the `samples/` folder.
+
+
+Supported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^
+Our client libraries are compatible with all current `active`_ and `maintenance`_ versions of
+Python.
+
+Python >= 3.7
+
+.. _active: https://devguide.python.org/devcycle/#in-development-main-branch
+.. _maintenance: https://devguide.python.org/devcycle/#maintenance-branches
+
+Unsupported Python Versions
+^^^^^^^^^^^^^^^^^^^^^^^^^^^
+Python <= 3.6
+
+If you are using an `end-of-life`_
+version of Python, we recommend that you update as soon as possible to an actively supported version.
+
+.. _end-of-life: https://devguide.python.org/devcycle/#end-of-life-branches
+
 Mac/Linux
 ^^^^^^^^^
 
 .. code-block:: console
 
     pip install virtualenv
     virtualenv <your-env>
@@ -91,9 +116,12 @@
 Next Steps
 ~~~~~~~~~~
 
 -  Read the `Client Library Documentation`_ for Analytics Admin API
    to see other available methods on the client.
 -  Read the `Analytics Admin API Product documentation`_ to learn
    more about the product and see How-to Guides.
+-  View this `README`_ to see the full list of Cloud
+   APIs that we cover.
 
 .. _Analytics Admin API Product documentation:  https://developers.google.com/analytics/
+.. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-analytics-admin-0.8.2/google_analytics_admin.egg-info/SOURCES.txt` & `google-analytics-admin-0.9.0/google_analytics_admin.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -16,19 +16,36 @@
 google/analytics/admin_v1alpha/services/analytics_admin_service/transports/__init__.py
 google/analytics/admin_v1alpha/services/analytics_admin_service/transports/base.py
 google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc.py
 google/analytics/admin_v1alpha/services/analytics_admin_service/transports/grpc_asyncio.py
 google/analytics/admin_v1alpha/types/__init__.py
 google/analytics/admin_v1alpha/types/analytics_admin.py
 google/analytics/admin_v1alpha/types/resources.py
+google/analytics/admin_v1beta/__init__.py
+google/analytics/admin_v1beta/gapic_metadata.json
+google/analytics/admin_v1beta/py.typed
+google/analytics/admin_v1beta/services/__init__.py
+google/analytics/admin_v1beta/services/analytics_admin_service/__init__.py
+google/analytics/admin_v1beta/services/analytics_admin_service/async_client.py
+google/analytics/admin_v1beta/services/analytics_admin_service/client.py
+google/analytics/admin_v1beta/services/analytics_admin_service/pagers.py
+google/analytics/admin_v1beta/services/analytics_admin_service/transports/__init__.py
+google/analytics/admin_v1beta/services/analytics_admin_service/transports/base.py
+google/analytics/admin_v1beta/services/analytics_admin_service/transports/grpc.py
+google/analytics/admin_v1beta/services/analytics_admin_service/transports/grpc_asyncio.py
+google/analytics/admin_v1beta/types/__init__.py
+google/analytics/admin_v1beta/types/analytics_admin.py
+google/analytics/admin_v1beta/types/resources.py
 google_analytics_admin.egg-info/PKG-INFO
 google_analytics_admin.egg-info/SOURCES.txt
 google_analytics_admin.egg-info/dependency_links.txt
 google_analytics_admin.egg-info/namespace_packages.txt
 google_analytics_admin.egg-info/not-zip-safe
 google_analytics_admin.egg-info/requires.txt
 google_analytics_admin.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/gapic/__init__.py
 tests/unit/gapic/admin_v1alpha/__init__.py
-tests/unit/gapic/admin_v1alpha/test_analytics_admin_service.py
+tests/unit/gapic/admin_v1alpha/test_analytics_admin_service.py
+tests/unit/gapic/admin_v1beta/__init__.py
+tests/unit/gapic/admin_v1beta/test_analytics_admin_service.py
```

### Comparing `google-analytics-admin-0.8.2/setup.py` & `google-analytics-admin-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 
 import io
 import os
 
 import setuptools  # type: ignore
 
-version = "0.8.2"
+version = "0.9.0"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
@@ -42,27 +42,23 @@
         for package in setuptools.PEP420PackageFinder.find()
         if package.startswith("google")
     ],
     namespace_packages=("google", "google.analytics"),
     platforms="Posix; MacOS X; Windows",
     include_package_data=True,
     install_requires=(
-        # NOTE: Maintainers, please do not require google-api-core>=2.x.x
-        # Until this issue is closed
-        # https://github.com/googleapis/google-cloud-python/issues/10566
-        "google-api-core[grpc] >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
+        "google-api-core[grpc] >= 1.32.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*",
         "proto-plus >= 1.15.0, <2.0.0dev",
         "protobuf >= 3.19.0, <4.0.0dev",
     ),
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Topic :: Internet",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
```

### Comparing `google-analytics-admin-0.8.2/tests/__init__.py` & `google-analytics-admin-0.9.0/google/analytics/admin_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/tests/unit/__init__.py` & `google-analytics-admin-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/tests/unit/gapic/__init__.py` & `google-analytics-admin-0.9.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/tests/unit/gapic/admin_v1alpha/__init__.py` & `google-analytics-admin-0.9.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-analytics-admin-0.8.2/tests/unit/gapic/admin_v1alpha/test_analytics_admin_service.py` & `google-analytics-admin-0.9.0/tests/unit/gapic/admin_v1alpha/test_analytics_admin_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
             credentials_file=None,
             host="squid.clam.whelk",
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT is
     # "never".
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "never"}):
         with mock.patch.object(transport_class, "__init__") as patched:
             patched.return_value = None
@@ -248,14 +249,15 @@
                 credentials_file=None,
                 host=client.DEFAULT_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT is
     # "always".
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "always"}):
         with mock.patch.object(transport_class, "__init__") as patched:
             patched.return_value = None
@@ -265,14 +267,15 @@
                 credentials_file=None,
                 host=client.DEFAULT_MTLS_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case api_endpoint is not provided and GOOGLE_API_USE_MTLS_ENDPOINT has
     # unsupported value.
     with mock.patch.dict(os.environ, {"GOOGLE_API_USE_MTLS_ENDPOINT": "Unsupported"}):
         with pytest.raises(MutualTLSChannelError):
             client = client_class(transport=transport_name)
@@ -294,14 +297,33 @@
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id="octopus",
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
+        )
+    # Check the case api_endpoint is provided
+    options = client_options.ClientOptions(
+        api_audience="https://language.googleapis.com"
+    )
+    with mock.patch.object(transport_class, "__init__") as patched:
+        patched.return_value = None
+        client = client_class(client_options=options, transport=transport_name)
+        patched.assert_called_once_with(
+            credentials=None,
+            credentials_file=None,
+            host=client.DEFAULT_ENDPOINT,
+            scopes=None,
+            client_cert_source_for_mtls=None,
+            quota_project_id=None,
+            client_info=transports.base.DEFAULT_CLIENT_INFO,
+            always_use_jwt_access=True,
+            api_audience="https://language.googleapis.com",
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,use_client_cert_env",
     [
         (
@@ -371,14 +393,15 @@
                 credentials_file=None,
                 host=expected_host,
                 scopes=None,
                 client_cert_source_for_mtls=expected_client_cert_source,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
 
     # Check the case ADC client cert is provided. Whether client cert is used depends on
     # GOOGLE_API_USE_CLIENT_CERTIFICATE value.
     with mock.patch.dict(
         os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": use_client_cert_env}
     ):
@@ -405,14 +428,15 @@
                         credentials_file=None,
                         host=expected_host,
                         scopes=None,
                         client_cert_source_for_mtls=expected_client_cert_source,
                         quota_project_id=None,
                         client_info=transports.base.DEFAULT_CLIENT_INFO,
                         always_use_jwt_access=True,
+                        api_audience=None,
                     )
 
     # Check the case client_cert_source and ADC client cert are not provided.
     with mock.patch.dict(
         os.environ, {"GOOGLE_API_USE_CLIENT_CERTIFICATE": use_client_cert_env}
     ):
         with mock.patch.object(transport_class, "__init__") as patched:
@@ -427,14 +451,15 @@
                     credentials_file=None,
                     host=client.DEFAULT_ENDPOINT,
                     scopes=None,
                     client_cert_source_for_mtls=None,
                     quota_project_id=None,
                     client_info=transports.base.DEFAULT_CLIENT_INFO,
                     always_use_jwt_access=True,
+                    api_audience=None,
                 )
 
 
 @pytest.mark.parametrize(
     "client_class", [AnalyticsAdminServiceClient, AnalyticsAdminServiceAsyncClient]
 )
 @mock.patch.object(
@@ -545,14 +570,15 @@
             credentials_file=None,
             host=client.DEFAULT_ENDPOINT,
             scopes=["1", "2"],
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,grpc_helpers",
     [
         (
@@ -583,14 +609,15 @@
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 def test_analytics_admin_service_client_client_options_from_dict():
     with mock.patch(
         "google.analytics.admin_v1alpha.services.analytics_admin_service.transports.AnalyticsAdminServiceGrpcTransport.__init__"
     ) as grpc_transport:
@@ -603,14 +630,15 @@
             credentials_file=None,
             host="squid.clam.whelk",
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
 
 @pytest.mark.parametrize(
     "client_class,transport_class,transport_name,grpc_helpers",
     [
         (
@@ -641,14 +669,15 @@
             credentials_file="credentials.json",
             host=client.DEFAULT_ENDPOINT,
             scopes=None,
             client_cert_source_for_mtls=None,
             quota_project_id=None,
             client_info=transports.base.DEFAULT_CLIENT_INFO,
             always_use_jwt_access=True,
+            api_audience=None,
         )
 
     # test that the credentials from file are saved and used as the credentials.
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch.object(
         google.auth, "default", autospec=True
@@ -20546,14 +20575,36 @@
                 "https://www.googleapis.com/auth/analytics.readonly",
             ),
             quota_project_id="octopus",
         )
 
 
 @pytest.mark.parametrize(
+    "transport_class",
+    [
+        transports.AnalyticsAdminServiceGrpcTransport,
+        transports.AnalyticsAdminServiceGrpcAsyncIOTransport,
+    ],
+)
+def test_analytics_admin_service_transport_auth_gdch_credentials(transport_class):
+    host = "https://language.com"
+    api_audience_tests = [None, "https://language2.com"]
+    api_audience_expect = [host, "https://language2.com"]
+    for t, e in zip(api_audience_tests, api_audience_expect):
+        with mock.patch.object(google.auth, "default", autospec=True) as adc:
+            gdch_mock = mock.MagicMock()
+            type(gdch_mock).with_gdch_audience = mock.PropertyMock(
+                return_value=gdch_mock
+            )
+            adc.return_value = (gdch_mock, None)
+            transport_class(host=host, api_audience=t)
+            gdch_mock.with_gdch_audience.assert_called_once_with(e)
+
+
+@pytest.mark.parametrize(
     "transport_class,grpc_helpers",
     [
         (transports.AnalyticsAdminServiceGrpcTransport, grpc_helpers),
         (transports.AnalyticsAdminServiceGrpcAsyncIOTransport, grpc_helpers_async),
     ],
 )
 def test_analytics_admin_service_transport_create_channel(
@@ -21391,8 +21442,9 @@
                 credentials_file=None,
                 host=client.DEFAULT_ENDPOINT,
                 scopes=None,
                 client_cert_source_for_mtls=None,
                 quota_project_id=None,
                 client_info=transports.base.DEFAULT_CLIENT_INFO,
                 always_use_jwt_access=True,
+                api_audience=None,
             )
```

