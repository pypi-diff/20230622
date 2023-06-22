# Comparing `tmp/python-esileapclient-0.2.1.tar.gz` & `tmp/python-esileapclient-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-esileapclient-0.2.1.tar", last modified: Fri Aug 19 19:27:59 2022, max compression
+gzip compressed data, was "/home/tzumainn/development/python-esileapclient/dist/tmpuu0xn759/python-esileapclient-0.2.2.tar", last modified: Thu Jun 22 16:06:39 2023, max compression
```

## Comparing `python-esileapclient-0.2.1.tar` & `python-esileapclient-0.2.2.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      305 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/AUTHORS
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3423 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/PKG-INFO
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/osc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/osc/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1711 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/node.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/mdc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8043 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/mdc/mdc_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/mdc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3553 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/mdc/mdc_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7375 2022-08-19 19:27:22.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9125 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/osc/v1/offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2033 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/osc/plugin.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      674 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3453 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/common/http.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6595 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/common/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/common/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2140 2022-08-19 19:27:22.000000 python-esileapclient-0.2.1/esileapclient/v1/node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1702 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/v1/client.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3258 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/v1/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3792 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/v1/offer.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2326 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/test_plugin.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1059 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/base.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/mdc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13350 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/mdc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5676 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9880 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/test_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2266 2022-08-19 19:27:22.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2713 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/fakes.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11180 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/test_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9479 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/common/test_base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/common/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3007 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/common/test_http.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1505 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/unit/v1/test_client.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7658 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/base.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/utils/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1404 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/utils/output_utils.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/utils/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1056 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/utils/dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2909 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/utils/esi_interfaces.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    25162 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_time.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    17508 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_basic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9801 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_policy.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10562 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_sublease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2730 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/esileapclient/tests/functional/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1169 2022-06-16 16:55:03.000000 python-esileapclient-0.2.1/setup.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      969 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/tox.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2157 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/ChangeLog
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2054 2022-07-25 14:22:51.000000 python-esileapclient-0.2.1/README.md
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/.github/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/.github/workflows/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      601 2022-06-16 16:55:03.000000 python-esileapclient-0.2.1/.github/workflows/tests.yml
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      259 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/test-requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2022-06-16 16:55:03.000000 python-esileapclient-0.2.1/LICENSE
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1684 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/setup.cfg
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      932 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/conftest.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       74 2022-06-16 16:54:31.000000 python-esileapclient-0.2.1/requirements.txt
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3423 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/PKG-INFO
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/pbr.json
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-07-25 14:25:40.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/not-zip-safe
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      846 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/entry_points.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2393 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/SOURCES.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       14 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/top_level.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/dependency_links.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       62 2022-08-19 19:27:59.000000 python-esileapclient-0.2.1/python_esileapclient.egg-info/requires.txt
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/.github/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/.github/workflows/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      616 2023-06-02 12:59:58.000000 python-esileapclient-0.2.2/.github/workflows/tests.yml
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6595 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/common/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3453 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/common/http.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/osc/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/mdc/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/mdc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3765 2023-06-22 16:04:44.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/mdc/mdc_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8043 2022-07-25 14:22:51.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/mdc/mdc_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7756 2023-06-22 16:04:44.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1711 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9125 2022-07-25 14:22:51.000000 python-esileapclient-0.2.2/esileapclient/osc/v1/offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/osc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2033 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/osc/plugin.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/utils/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/utils/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1056 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/utils/dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3162 2023-06-02 12:59:58.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/utils/esi_interfaces.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1404 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/utils/output_utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    19558 2023-06-02 12:59:58.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_basic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9801 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_policy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10562 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_sublease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    25162 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_time.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2730 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7658 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/functional/base.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9296 2023-06-02 12:59:58.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/common/test_base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3007 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/common/test_http.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/mdc/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/mdc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5936 2023-06-22 16:04:44.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13531 2023-06-22 16:04:44.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1059 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2775 2023-06-22 16:04:44.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/fakes.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10298 2023-06-22 16:04:44.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/test_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2266 2022-08-19 19:27:22.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11180 2022-07-25 14:22:51.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/test_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2326 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/osc/test_plugin.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1505 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/v1/test_client.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/unit/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/tests/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/esileapclient/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1702 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/v1/client.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3329 2023-06-22 16:04:44.000000 python-esileapclient-0.2.2/esileapclient/v1/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2140 2022-08-19 19:27:22.000000 python-esileapclient-0.2.2/esileapclient/v1/node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3792 2022-07-25 14:22:51.000000 python-esileapclient-0.2.2/esileapclient/v1/offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      674 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/esileapclient/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3032 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/PKG-INFO
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2393 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      846 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/entry_points.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-07-25 14:25:40.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/not-zip-safe
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/pbr.json
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       62 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/requires.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       14 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/python_esileapclient.egg-info/top_level.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      358 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/AUTHORS
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2297 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/ChangeLog
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2022-06-16 16:55:03.000000 python-esileapclient-0.2.2/LICENSE
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2054 2022-07-25 14:22:51.000000 python-esileapclient-0.2.2/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      932 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/conftest.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       74 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1684 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/setup.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1169 2022-06-16 16:55:03.000000 python-esileapclient-0.2.2/setup.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      259 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/test-requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      969 2022-06-16 16:54:31.000000 python-esileapclient-0.2.2/tox.ini
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3032 2023-06-22 16:06:39.000000 python-esileapclient-0.2.2/PKG-INFO
```

### Comparing `python-esileapclient-0.2.1/PKG-INFO` & `python-esileapclient-0.2.2/python_esileapclient.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,15 @@
 Metadata-Version: 2.1
 Name: python-esileapclient
-Version: 0.2.1
+Version: 0.2.2
 Summary: ESI-LEAP CLI
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
-Description: # python-esileapclient
-        
-        Python API for interacting with [ESI-Leap](https://github.com/CCI-MOC/esi-leap)
-        
-        ### Overview
-        
-        This is a client for the OpenStack Lease API. It provides:
-        
-           - a openstack command-line plugin: `openstack lease`
-        
-        python-esileapclient is licensed under the Apache License, Version 2.0, like the rest of OpenStack.
-        
-        ### Installation
-        
-        To install as a package:
-        ```
-        # pip install python-esileapclient`
-        ```
-        
-        To install from source:
-        ```
-        $ git clone https://github.com/CCI-MOC/python-esileapclient
-        $ cd python-esileapclient
-        # python setup.py install
-        ```
-        
-        ### `openstack lease` CLI
-        
-        The `openstack lease` command-line interface is available when the lease plugin (included in this package) is used with the [OpenStackClient](https://docs.openstack.org/python-openstackclient/latest/)
-        
-        The client uses the OpenStack Identity API (Keystone) to authenticate users with an OpenStack cloud and to locate the lease service endpoint (see [here](https://docs.openstack.org/keystone/latest/admin/manage-services.html) for more info). Currently, overriding this endpoint is not supported. Credentials for authentication can be provided via command-line parameters (e.g. `--os-username, --os-password, etc.`) or by setting environment variables (e.g. `OS_USERNAME, OS_PASSWORD`).
-        
-        Usage Examples:
-        
-            openstack esi offer list
-        
-        will make a GET request to ESI-Leap and print to screen a list of all the offers in the ESI-Leap database.
-        
-            openstack esi offer show <uuid>
-        
-        will make a GET request and print fields for offer with the given uuid.
-        
-            openstack esi offer create --resource-type dummy_node --resource-uuid 1718
-        
-        will make a POST request to ESI-Leap to create the offer with the given credentials. Prints to the screen the newly created offer with resource type 'dummy\_node' and resource uuid '1718'.
-        
-            openstack esi offer delete <uuid>
-        
-        will make a DELETE request to ESI-Leap to delete the request with the given uuid. Prints to the screen whether the command was a success or not.
-        
-        
-        This repository is currently a work in progress.
-        
-        
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
@@ -72,7 +18,65 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# python-esileapclient
+
+Python API for interacting with [ESI-Leap](https://github.com/CCI-MOC/esi-leap)
+
+### Overview
+
+This is a client for the OpenStack Lease API. It provides:
+
+   - a openstack command-line plugin: `openstack lease`
+
+python-esileapclient is licensed under the Apache License, Version 2.0, like the rest of OpenStack.
+
+### Installation
+
+To install as a package:
+```
+# pip install python-esileapclient`
+```
+
+To install from source:
+```
+$ git clone https://github.com/CCI-MOC/python-esileapclient
+$ cd python-esileapclient
+# python setup.py install
+```
+
+### `openstack lease` CLI
+
+The `openstack lease` command-line interface is available when the lease plugin (included in this package) is used with the [OpenStackClient](https://docs.openstack.org/python-openstackclient/latest/)
+
+The client uses the OpenStack Identity API (Keystone) to authenticate users with an OpenStack cloud and to locate the lease service endpoint (see [here](https://docs.openstack.org/keystone/latest/admin/manage-services.html) for more info). Currently, overriding this endpoint is not supported. Credentials for authentication can be provided via command-line parameters (e.g. `--os-username, --os-password, etc.`) or by setting environment variables (e.g. `OS_USERNAME, OS_PASSWORD`).
+
+Usage Examples:
+
+    openstack esi offer list
+
+will make a GET request to ESI-Leap and print to screen a list of all the offers in the ESI-Leap database.
+
+    openstack esi offer show <uuid>
+
+will make a GET request and print fields for offer with the given uuid.
+
+    openstack esi offer create --resource-type dummy_node --resource-uuid 1718
+
+will make a POST request to ESI-Leap to create the offer with the given credentials. Prints to the screen the newly created offer with resource type 'dummy\_node' and resource uuid '1718'.
+
+    openstack esi offer delete <uuid>
+
+will make a DELETE request to ESI-Leap to delete the request with the given uuid. Prints to the screen whether the command was a success or not.
+
+
+This repository is currently a work in progress.
+
+
+
```

### Comparing `python-esileapclient-0.2.1/esileapclient/osc/v1/node.py` & `python-esileapclient-0.2.2/esileapclient/osc/v1/node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/osc/v1/mdc/mdc_offer.py` & `python-esileapclient-0.2.2/esileapclient/osc/v1/mdc/mdc_offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/osc/v1/mdc/mdc_lease.py` & `python-esileapclient-0.2.2/esileapclient/osc/v1/mdc/mdc_lease.py`

 * *Files 19% similar despite different names*

```diff
@@ -59,15 +59,19 @@
             required=False,
             help="Show all leases with given resource-type.")
         parser.add_argument(
             '--resource-class',
             dest='resource_class',
             required=False,
             help="Show all leases with given resource-class.")
-
+        parser.add_argument(
+            '--purpose',
+            dest='purpose',
+            required=False,
+            help="Show all the leases with given purpose")
         return parser
 
     def take_action(self, parsed_args):
         data = []
 
         cloud_regions = openstack.config.loader.OpenStackConfig().\
             get_all_clouds()
@@ -78,14 +82,15 @@
             'status': parsed_args.status,
             'start_time': str(parsed_args.time_range[0]) if
             parsed_args.time_range else None,
             'end_time': str(parsed_args.time_range[1]) if
             parsed_args.time_range else None,
             'resource_type': parsed_args.resource_type,
             'resource_class': parsed_args.resource_class,
+            'purpose': parsed_args.purpose,
         }
 
         for c in cloud_regions:
             client = esileapclient.Client(session=c.get_session())
 
             leases = client.lease.list(filters)
             for lease in leases:
```

### Comparing `python-esileapclient-0.2.1/esileapclient/osc/v1/lease.py` & `python-esileapclient-0.2.2/esileapclient/osc/v1/lease.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,14 +59,19 @@
             required=False,
             help="Use this resource type instead of the default.")
         parser.add_argument(
             '--start-time',
             dest='start_time',
             required=False,
             help="Time when the resource will become usable.")
+        parser.add_argument(
+            '--purpose',
+            dest='purpose',
+            required=False,
+            help="Specify the purpose for leasing the node")
         return parser
 
     def take_action(self, parsed_args):
         client = self.app.client_manager.lease
 
         field_list = LEASE_RESOURCE._creation_attributes
         fields = dict((k, v) for (k, v) in vars(parsed_args).items()
@@ -143,15 +148,19 @@
             required=False,
             help="Show all leases with given resource-uuid.")
         parser.add_argument(
             '--resource-class',
             dest='resource_class',
             required=False,
             help="Show all leases with given resource-class.")
-
+        parser.add_argument(
+            '--purpose',
+            dest='purpose',
+            required=False,
+            help="Show the purpose of leasing the node")
         return parser
 
     def take_action(self, parsed_args):
 
         client = self.app.client_manager.lease
 
         filters = {
@@ -162,15 +171,16 @@
             'end_time': str(parsed_args.time_range[1]) if
             parsed_args.time_range else None,
             'project_id': parsed_args.project_id,
             'owner_id': parsed_args.owner_id,
             'view': 'all' if parsed_args.all else None,
             'resource_type': parsed_args.resource_type,
             'resource_uuid': parsed_args.resource_uuid,
-            'resource_class': parsed_args.resource_class
+            'resource_class': parsed_args.resource_class,
+            'purpose': parsed_args.purpose
         }
 
         data = client.lease.list(filters)
 
         if parsed_args.long:
             columns = LEASE_RESOURCE.detailed_fields.keys()
             labels = LEASE_RESOURCE.detailed_fields.values()
```

### Comparing `python-esileapclient-0.2.1/esileapclient/osc/v1/offer.py` & `python-esileapclient-0.2.2/esileapclient/osc/v1/offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/osc/plugin.py` & `python-esileapclient-0.2.2/esileapclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/__init__.py` & `python-esileapclient-0.2.2/esileapclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/common/http.py` & `python-esileapclient-0.2.2/esileapclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/common/base.py` & `python-esileapclient-0.2.2/esileapclient/common/base.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/v1/node.py` & `python-esileapclient-0.2.2/esileapclient/v1/node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/v1/client.py` & `python-esileapclient-0.2.2/esileapclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/v1/lease.py` & `python-esileapclient-0.2.2/esileapclient/v1/lease.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,30 +35,32 @@
         'resource': "Resource",
         'resource_class': "Resource Class",
         'resource_type': "Resource Type",
         'resource_uuid': "Resource UUID",
         'start_time': "Start Time",
         'status': "Status",
         'uuid': "UUID",
+        'purpose': "Purpose",
     }
 
     fields = {
         'uuid': "UUID",
         'resource': "Resource",
         'resource_class': "Resource Class",
         'project': "Project",
         'start_time': "Start Time",
         'end_time': "End Time",
         'offer_uuid': "Offer UUID",
         'status': "Status",
+        'purpose': "Purpose",
     }
 
     _creation_attributes = ['start_time', 'end_time', 'status', 'name',
                             'properties', 'project_id', 'resource_type',
-                            'resource_uuid']
+                            'resource_uuid', 'purpose']
 
     def __repr__(self):
         return "<Lease %s>" % self._info
 
 
 class LeaseManager(base.Manager):
     resource_class = Lease
```

### Comparing `python-esileapclient-0.2.1/esileapclient/v1/offer.py` & `python-esileapclient-0.2.2/esileapclient/v1/offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/test_plugin.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/base.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py`

 * *Files 2% similar despite different names*

```diff
@@ -231,37 +231,40 @@
             "Resource",
             "Resource Class",
             "Project",
             "Start Time",
             "End Time",
             "Offer UUID",
             "Status",
+            "Purpose",
         ]
 
         self.assertEqual(collist, list(columns))
 
         cloud1_lease = ('cloud1', 'regionOne',
                         fakes.lease_uuid,
                         fakes.lease_resource,
                         fakes.lease_resource_class,
                         fakes.lease_project,
                         fakes.lease_start_time,
                         fakes.lease_end_time,
                         fakes.offer_uuid,
-                        fakes.lease_status
+                        fakes.lease_status,
+                        fakes.lease_purpose
                         )
         cloud2_lease = ('cloud2', 'regionTwo',
                         fakes.lease_uuid,
                         fakes.lease_resource,
                         fakes.lease_resource_class,
                         fakes.lease_project,
                         fakes.lease_start_time,
                         fakes.lease_end_time,
                         fakes.offer_uuid,
-                        fakes.lease_status
+                        fakes.lease_status,
+                        fakes.lease_purpose
                         )
 
         parsed_data = tuple(data)
         self.assertEqual(3, len(parsed_data))
         self.assertEqual(2, parsed_data.count(cloud1_lease))
         self.assertEqual(1, parsed_data.count(cloud2_lease))
 
@@ -301,27 +304,29 @@
             "Resource",
             "Resource Class",
             "Project",
             "Start Time",
             "End Time",
             "Offer UUID",
             "Status",
+            "Purpose",
         ]
 
         self.assertEqual(collist, list(columns))
 
         cloud1_lease = ('cloud1', 'regionOne',
                         fakes.lease_uuid,
                         fakes.lease_resource,
                         fakes.lease_resource_class,
                         fakes.lease_project,
                         fakes.lease_start_time,
                         fakes.lease_end_time,
                         fakes.offer_uuid,
                         fakes.lease_status,
+                        fakes.lease_purpose,
                         )
 
         parsed_data = tuple(data)
         self.assertEqual(2, len(parsed_data))
         self.assertEqual(2, parsed_data.count(cloud1_lease))
 
     @mock.patch('esileapclient.v1.client.Client')
```

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             'status': parsed_args.status,
             'start_time': str(parsed_args.time_range[0]) if
             parsed_args.time_range else None,
             'end_time': str(parsed_args.time_range[1]) if
             parsed_args.time_range else None,
             'resource_type': parsed_args.resource_type,
             'resource_class': parsed_args.resource_class,
+            'purpose': parsed_args.purpose,
         }
 
         self.client_mock.lease.list.assert_called_with(filters)
 
         collist = [
             "Cloud",
             "Region",
@@ -78,37 +79,40 @@
             "Resource",
             "Resource Class",
             "Project",
             "Start Time",
             "End Time",
             "Offer UUID",
             "Status",
+            "Purpose",
         ]
 
         self.assertEqual(collist, list(columns))
 
         datalist = (('cloud1', 'regionOne',
                      fakes.lease_uuid,
                      fakes.lease_resource,
                      fakes.lease_resource_class,
                      fakes.lease_project,
                      fakes.lease_start_time,
                      fakes.lease_end_time,
                      fakes.offer_uuid,
                      fakes.lease_status,
+                     fakes.lease_purpose,
                      ),
                     ('cloud2', 'regionTwo',
                      fakes.lease_uuid,
                      fakes.lease_resource,
                      fakes.lease_resource_class,
                      fakes.lease_project,
                      fakes.lease_start_time,
                      fakes.lease_end_time,
                      fakes.offer_uuid,
                      fakes.lease_status,
+                     fakes.lease_purpose,
                      ))
         self.assertEqual(datalist, tuple(data))
 
     @mock.patch('esileapclient.v1.client.Client')
     @mock.patch('openstack.config.loader.OpenStackConfig.get_all_clouds')
     def test_mdc_lease_list_filter(self, mock_clouds, mock_client):
         mock_clouds.return_value = [self.cloud1, self.cloud2]
@@ -125,14 +129,15 @@
             'status': parsed_args.status,
             'start_time': str(parsed_args.time_range[0]) if
             parsed_args.time_range else None,
             'end_time': str(parsed_args.time_range[1]) if
             parsed_args.time_range else None,
             'resource_type': parsed_args.resource_type,
             'resource_class': parsed_args.resource_class,
+            'purpose': parsed_args.purpose,
         }
 
         self.client_mock.lease.list.assert_called_with(filters)
 
         collist = [
             "Cloud",
             "Region",
@@ -140,22 +145,24 @@
             "Resource",
             "Resource Class",
             "Project",
             "Start Time",
             "End Time",
             "Offer UUID",
             "Status",
+            "Purpose",
         ]
 
         self.assertEqual(collist, list(columns))
 
         datalist = (('cloud2', 'regionTwo',
                      fakes.lease_uuid,
                      fakes.lease_resource,
                      fakes.lease_resource_class,
                      fakes.lease_project,
                      fakes.lease_start_time,
                      fakes.lease_end_time,
                      fakes.offer_uuid,
                      fakes.lease_status,
+                     fakes.lease_purpose,
                      ),)
         self.assertEqual(datalist, tuple(data))
```

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/test_lease.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/test_lease.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,38 +46,41 @@
             fakes.lease_resource_uuid,
             fakes.lease_project_id,
             '--end-time', fakes.lease_end_time,
             '--name', fakes.lease_name,
             '--properties', fakes.lease_properties,
             '--resource-type', fakes.lease_resource_type,
             '--start-time', fakes.lease_start_time,
+            '--purpose', fakes.lease_purpose,
         ]
 
         verifylist = [
             ('end_time', fakes.lease_end_time),
             ('name', fakes.lease_name),
             ('project_id', fakes.lease_project_id),
             ('properties', fakes.lease_properties),
             ('resource_type', fakes.lease_resource_type),
             ('resource_uuid', fakes.lease_resource_uuid),
             ('start_time', fakes.lease_start_time),
+            ('purpose', fakes.lease_purpose),
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         self.cmd.take_action(parsed_args)
 
         args = {
             'resource_type': fakes.lease_resource_type,
             'resource_uuid': fakes.lease_resource_uuid,
             'project_id': fakes.lease_project_id,
             'end_time': fakes.lease_end_time,
             'name': fakes.lease_name,
             'properties': json.loads(fakes.lease_properties),
             'start_time': fakes.lease_start_time,
+            'purpose': fakes.lease_purpose,
         }
 
         self.client_mock.lease.create.assert_called_once_with(**args)
 
 
 class TestLeaseList(TestLease):
 
@@ -104,40 +107,43 @@
             'end_time': str(parsed_args.time_range[1]) if
             parsed_args.time_range else None,
             'project_id': parsed_args.project_id,
             'owner_id': parsed_args.owner_id,
             'view': 'all' if parsed_args.all else None,
             'resource_type': parsed_args.resource_type,
             'resource_uuid': parsed_args.resource_uuid,
-            'resource_class': parsed_args.resource_class
+            'resource_class': parsed_args.resource_class,
+            'purpose': parsed_args.purpose
         }
 
         self.client_mock.lease.list.assert_called_with(filters)
 
         collist = [
             "UUID",
             "Resource",
             "Resource Class",
             "Project",
             "Start Time",
             "End Time",
             "Offer UUID",
             "Status",
+            "Purpose",
         ]
 
         self.assertEqual(collist, list(columns))
 
         datalist = ((fakes.lease_uuid,
                      fakes.lease_resource,
                      fakes.lease_resource_class,
                      fakes.lease_project,
                      fakes.lease_start_time,
                      fakes.lease_end_time,
                      fakes.offer_uuid,
-                     fakes.lease_status
+                     fakes.lease_status,
+                     fakes.lease_purpose
                      ),)
         self.assertEqual(datalist, tuple(data))
 
     def test_lease_list_long(self):
         arglist = ['--long']
         verifylist = [('long', True)]
 
@@ -152,15 +158,16 @@
             'end_time': str(parsed_args.time_range[1]) if
             parsed_args.time_range else None,
             'project_id': parsed_args.project_id,
             'owner_id': parsed_args.owner_id,
             'view': 'all' if parsed_args.all else None,
             'resource_type': parsed_args.resource_type,
             'resource_uuid': parsed_args.resource_uuid,
-            'resource_class': parsed_args.resource_class
+            'resource_class': parsed_args.resource_class,
+            'purpose': parsed_args.purpose
         }
 
         self.client_mock.lease.list.assert_called_with(filters)
 
         long_collist = [
             "End Time",
             "Expire Time",
@@ -176,14 +183,15 @@
             "Resource",
             "Resource Class",
             "Resource Type",
             "Resource UUID",
             "Start Time",
             "Status",
             "UUID",
+            "Purpose",
         ]
 
         self.assertEqual(long_collist, list(columns))
 
         datalist = ((fakes.lease_end_time,
                      fakes.lease_expire_time,
                      fakes.lease_fulfill_time,
@@ -197,15 +205,16 @@
                      json.loads(fakes.lease_properties),
                      fakes.lease_resource,
                      fakes.lease_resource_class,
                      fakes.lease_resource_type,
                      fakes.lease_resource_uuid,
                      fakes.lease_start_time,
                      fakes.lease_status,
-                     fakes.lease_uuid
+                     fakes.lease_uuid,
+                     fakes.lease_purpose
                      ),)
         self.assertEqual(datalist, tuple(data))
 
 
 class TestLeaseShow(TestLease):
     def setUp(self):
         super(TestLeaseShow, self).setUp()
@@ -233,14 +242,15 @@
             "offer_uuid",
             "owner",
             "owner_id",
             "parent_lease_uuid",
             "project",
             "project_id",
             "properties",
+            "purpose",
             "resource",
             "resource_class",
             "resource_type",
             "resource_uuid",
             "start_time",
             "status",
             "uuid"
@@ -255,14 +265,15 @@
                     fakes.offer_uuid,
                     fakes.lease_owner,
                     fakes.lease_owner_id,
                     fakes.parent_lease_uuid,
                     fakes.lease_project,
                     fakes.lease_project_id,
                     json.loads(fakes.lease_properties),
+                    fakes.lease_purpose,
                     fakes.lease_resource,
                     fakes.lease_resource_class,
                     fakes.lease_resource_type,
                     fakes.lease_resource_uuid,
                     fakes.lease_start_time,
                     fakes.lease_status,
                     fakes.lease_uuid
```

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/test_node.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/test_node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/fakes.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 lease_resource_type = "dummy_node"
 lease_resource_uuid = "1213123123"
 lease_resource_class = 'baremetal'
 lease_start_time = "2010"
 lease_fulfill_time = "2010"
 lease_status = "fake_status"
 lease_uuid = "9999999"
+lease_purpose = "fake_purpose"
 offer_uuid = "111111111"
 offer_lessee = 'lease-project'
 offer_lessee_id = "zzzzzzzz-zzzz-zzzz-zzzz-zzzzzzzzzzzz"
 offer_name = "o1"
 parent_lease_uuid = "parent-lease-uuid"
 lease_name = "c1"
 node_name = "fake-node"
@@ -72,15 +73,16 @@
     'properties': json.loads(lease_properties),
     'resource': lease_resource,
     'resource_type': lease_resource_type,
     'resource_uuid': lease_resource_uuid,
     'resource_class': lease_resource_class,
     'start_time': lease_start_time,
     'status': lease_status,
-    'uuid': lease_uuid
+    'uuid': lease_uuid,
+    'purpose': lease_purpose,
 }
 
 NODE = {
     'name': node_name,
     'uuid': node_uuid,
     'owner': node_owner
 }
```

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/osc/v1/test_offer.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/osc/v1/test_offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/common/test_base.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/common/test_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,30 +13,30 @@
 import testtools
 import copy
 from unittest import mock
 
 from esileapclient.common import base
 
 
-TESTABLE_RESOURCE = {
+FAKE_RESOURCE = {
     'uuid': '11111111-2222-3333-4444-555555555555',
     'attribute1': '1',
     'attribute2': '2',
 }
-TESTABLE_RESOURCE2 = {
+FAKE_RESOURCE_2 = {
     'uuid': '66666666-7777-8888-9999-000000000000',
     'attribute1': '3',
     'attribute2': '4',
 }
 
 
-CREATE_TESTABLE_RESOURCE = copy.deepcopy(TESTABLE_RESOURCE)
-del CREATE_TESTABLE_RESOURCE['uuid']
+CREATE_FAKE_RESOURCE = copy.deepcopy(FAKE_RESOURCE)
+del CREATE_FAKE_RESOURCE['uuid']
 
-INVALID_ATTRIBUTE_TESTABLE_RESOURCE = {
+INVALID_ATTRIBUTE_FAKE_RESOURCE = {
     'non-existent-attribute': 'bad',
     'attribute1': '1',
     'attribute2': '2',
 }
 
 
 class FakeResponse(object):
@@ -53,15 +53,15 @@
         self.request.headers = request_headers
 
 
 VALID_CREATE_RESPONSE = FakeResponse(status=201)
 VALID_RESPONSE = FakeResponse(status=200)
 
 
-class TestableResource(base.Resource):
+class FakeResource(base.Resource):
 
     fields = {
         'uuid': 'UUID',
         'attribute1': 'Attribute 1',
         'attribute2': 'Attribute 2',
     }
 
@@ -71,212 +71,212 @@
         'attribute2': 'Attribute 2',
         'attribute3': 'Attribute 3',
     }
 
     _creation_attributes = ['attribute1', 'attribute2']
 
     def __repr__(self):
-        return "<TestableResource %s>" % self._info
+        return "<FakeResource %s>" % self._info
 
 
-class TestableManager(base.Manager):
-    resource_class = TestableResource
-    _resource_name = 'testableresources'
+class FakeResourceManager(base.Manager):
+    resource_class = FakeResource
+    _resource_name = 'fakeresources'
 
 
 class ManagerTestCase(testtools.TestCase):
 
     def test__create(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_CREATE_RESPONSE,
-                TESTABLE_RESOURCE)
+                FAKE_RESOURCE)
 
-            resource = manager._create(**CREATE_TESTABLE_RESOURCE)
+            resource = manager._create(**CREATE_FAKE_RESOURCE)
 
             mock_api.json_request.assert_called_once_with(
-                'POST', '/v1/testableresources',
-                **{'body': CREATE_TESTABLE_RESOURCE})
+                'POST', '/v1/fakeresources',
+                **{'body': CREATE_FAKE_RESOURCE})
 
-            self.assertIsInstance(resource, TestableResource)
-            self.assertEqual(resource._info, TESTABLE_RESOURCE)
+            self.assertIsInstance(resource, FakeResource)
+            self.assertEqual(resource._info, FAKE_RESOURCE)
 
     def test__create_microversion_override(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_CREATE_RESPONSE,
-                TESTABLE_RESOURCE)
+                FAKE_RESOURCE)
 
             resource = manager._create(os_esileap_api_version='1.10',
-                                       **CREATE_TESTABLE_RESOURCE)
+                                       **CREATE_FAKE_RESOURCE)
 
             mock_api.json_request.assert_called_once_with(
-                'POST', '/v1/testableresources',
-                **{'body': CREATE_TESTABLE_RESOURCE,
+                'POST', '/v1/fakeresources',
+                **{'body': CREATE_FAKE_RESOURCE,
                    'headers': {'X-OpenStack-ESI-Leap-API-Version': '1.10'}})
 
-            self.assertIsInstance(resource, TestableResource)
-            self.assertEqual(resource._info, TESTABLE_RESOURCE)
+            self.assertIsInstance(resource, FakeResource)
+            self.assertEqual(resource._info, FAKE_RESOURCE)
 
     def test__create_with_invalid_attribute(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api'):
 
             self.assertRaises(
                 Exception,
                 manager._create,
-                **INVALID_ATTRIBUTE_TESTABLE_RESOURCE)
+                **INVALID_ATTRIBUTE_FAKE_RESOURCE)
 
     def test__list(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_RESPONSE,
-                {'testableresources': [TESTABLE_RESOURCE, TESTABLE_RESOURCE2]})
+                {'fakeresources': [FAKE_RESOURCE, FAKE_RESOURCE_2]})
 
             resources_list = manager._list(manager._path())
 
             mock_api.json_request.assert_called_once_with(
-                'GET', '/v1/testableresources')
+                'GET', '/v1/fakeresources')
 
-            expected_resources = [TestableResource(None, TESTABLE_RESOURCE),
-                                  TestableResource(None, TESTABLE_RESOURCE2)]
+            expected_resources = [FakeResource(None, FAKE_RESOURCE),
+                                  FakeResource(None, FAKE_RESOURCE_2)]
 
             self.assertIsInstance(resources_list, list)
             assert (len(expected_resources) == 2)
 
-            self.assertIsInstance(resources_list[0], TestableResource)
+            self.assertIsInstance(resources_list[0], FakeResource)
 
             self.assertEqual(resources_list[0]._info,
                              expected_resources[0]._info)
             self.assertEqual(resources_list[1]._info,
                              expected_resources[1]._info)
 
     def test__list_microversion_override(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_RESPONSE,
-                {'testableresources': [TESTABLE_RESOURCE, TESTABLE_RESOURCE2]})
+                {'fakeresources': [FAKE_RESOURCE, FAKE_RESOURCE_2]})
 
             resources_list = manager._list(manager._path(),
                                            os_esileap_api_version='1.10')
 
             mock_api.json_request.assert_called_once_with(
-                'GET', '/v1/testableresources',
+                'GET', '/v1/fakeresources',
                 **{'headers': {'X-OpenStack-ESI-Leap-API-Version': '1.10'}})
 
-            expected_resources = [TestableResource(None, TESTABLE_RESOURCE),
-                                  TestableResource(None, TESTABLE_RESOURCE2)]
+            expected_resources = [FakeResource(None, FAKE_RESOURCE),
+                                  FakeResource(None, FAKE_RESOURCE_2)]
 
             self.assertIsInstance(resources_list, list)
             assert (len(expected_resources) == 2)
 
-            self.assertIsInstance(resources_list[0], TestableResource)
+            self.assertIsInstance(resources_list[0], FakeResource)
 
             self.assertEqual(resources_list[0]._info,
                              expected_resources[0]._info)
             self.assertEqual(resources_list[1]._info,
                              expected_resources[1]._info)
 
     def test__get(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_RESPONSE,
-                TESTABLE_RESOURCE)
+                FAKE_RESOURCE)
 
-            resource = manager._get(TESTABLE_RESOURCE['uuid'])
+            resource = manager._get(FAKE_RESOURCE['uuid'])
 
             mock_api.json_request.assert_called_once_with(
-                'GET', '/v1/testableresources/%s' % TESTABLE_RESOURCE['uuid'],)
+                'GET', '/v1/fakeresources/%s' % FAKE_RESOURCE['uuid'],)
 
-            self.assertIsInstance(resource, TestableResource)
-            self.assertEqual(TESTABLE_RESOURCE, resource._info)
+            self.assertIsInstance(resource, FakeResource)
+            self.assertEqual(FAKE_RESOURCE, resource._info)
 
     def test__get_microversion_override(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_RESPONSE,
-                TESTABLE_RESOURCE)
+                FAKE_RESOURCE)
 
-            resource = manager._get(TESTABLE_RESOURCE['uuid'],
+            resource = manager._get(FAKE_RESOURCE['uuid'],
                                     os_esileap_api_version='1.10')
 
             mock_api.json_request.assert_called_once_with(
-                'GET', '/v1/testableresources/%s' % TESTABLE_RESOURCE['uuid'],
+                'GET', '/v1/fakeresources/%s' % FAKE_RESOURCE['uuid'],
                 **{'headers': {'X-OpenStack-ESI-Leap-API-Version': '1.10'}})
 
-            self.assertIsInstance(resource, TestableResource)
-            self.assertEqual(TESTABLE_RESOURCE, resource._info)
+            self.assertIsInstance(resource, FakeResource)
+            self.assertEqual(FAKE_RESOURCE, resource._info)
 
     def test__get_invalid_resource_id_raises(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api'):
             resource_ids = [[], {}, False, '', 0, None, (), 'hi']
             for resource_id in resource_ids:
                 self.assertRaises(Exception, manager._get,
                                   resource_id=resource_id)
 
     def test__delete(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_RESPONSE,
                 None)
 
             resp = manager._delete(
-                resource_id=TESTABLE_RESOURCE['uuid'])
+                resource_id=FAKE_RESOURCE['uuid'])
 
             mock_api.json_request.assert_called_once_with(
                 'DELETE',
-                '/v1/testableresources/%s' % TESTABLE_RESOURCE['uuid'])
+                '/v1/fakeresources/%s' % FAKE_RESOURCE['uuid'])
 
             self.assertEqual(resp, None)
 
     def test__delete_microversion_override(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_RESPONSE,
                 None)
 
             resp = manager._delete(
-                resource_id=TESTABLE_RESOURCE['uuid'],
+                resource_id=FAKE_RESOURCE['uuid'],
                 os_esileap_api_version='1.10')
 
             mock_api.json_request.assert_called_once_with(
                 'DELETE',
-                '/v1/testableresources/%s' % TESTABLE_RESOURCE['uuid'],
+                '/v1/fakeresources/%s' % FAKE_RESOURCE['uuid'],
                 **{'headers': {'X-OpenStack-ESI-Leap-API-Version': '1.10'}})
 
             self.assertEqual(resp, None)
 
     def test__delete_invalid_resource_id_raises(self):
 
-        manager = TestableManager(None)
+        manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api'):
             resource_ids = [[], {}, False, '', 0, None, (), 'hi']
             for resource_id in resource_ids:
                 self.assertRaises(Exception, manager._delete,
                                   resource_id=resource_id)
```

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/common/test_http.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/common/test_http.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/unit/v1/test_client.py` & `python-esileapclient-0.2.2/esileapclient/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/base.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/utils/output_utils.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/utils/dummy_node.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/utils/dummy_node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/utils/esi_interfaces.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/utils/esi_interfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,21 @@
 def offer_claim(client, offer_uuid, parse=True, fail_ok=False, **kwargs):
     valid_flags = ('start_time', 'end_time', 'properties')
     return _execute(client, cmd='offer claim', valid_flags=valid_flags,
                     kwargs=kwargs, args=(offer_uuid,), parse=parse,
                     fail_ok=fail_ok)
 
 
+def node_list(client, parse=True, fail_ok=False, **kwargs):
+    valid_flags = ('long')
+    return _execute(client, cmd='node list', valid_flags=valid_flags,
+                    kwargs=kwargs, args=(), parse=parse,
+                    fail_ok=fail_ok)
+
+
 def lease_create(client, node_uuid, lessee, parse=True, fail_ok=False,
                  **kwargs):
     valid_flags = ('resource_type', 'start_time', 'end_time',
                    'name', 'properties')
     return _execute(client, cmd='lease create', valid_flags=valid_flags,
                     kwargs=kwargs, args=(node_uuid, lessee), parse=parse,
                     fail_ok=fail_ok)
```

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_time.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_time.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_basic.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_basic.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import pytest
+import unittest
+import os
 from tempest.lib.exceptions import CommandFailed
 from tempest.lib.common.utils import data_utils
 
 import esileapclient.tests.functional.utils.esi_interfaces as esi
 from esileapclient.tests.functional.base import ESIBaseTestClass
 from esileapclient.tests.functional.utils.dummy_node import DummyNode
 
@@ -209,14 +211,51 @@
                         lease['uuid'],
                         fail_ok=True)
 
         esi.offer_delete(self.clients['parent-owner'], offer['uuid'])
         details = esi.lease_show(self.clients['child-lessee'], lease['uuid'])
         self.assertEqual(details['status'], 'deleted')
 
+    @unittest.skipIf(list(map(lambda x: os.getenv('OS_FUNCTIONAL_NODE_%s' % x),
+                              ['NAME', 'UUID'])) == [None, None],
+                     'Neither env variable OS_FUNCTIONAL_NODE_UUID \
+                      nor OS_FUNCTIONAL_NODE_NAME is set')
+    def test_node_list_long(self):
+        """ Tests functionality "esi node list" using node_uuid or node name.
+            checks node_uuid or node_name is present in node list or not.
+            Test steps:
+            1) Set either of the environment variables using
+               export OS_FUNCTIONAL_NODE_UUID=node_uuid or
+               export OS_FUNCTIONAL_NODE_NAME=node_name
+            2) Checks that the output of "node list" contains
+               the node uuid or node name it's tested with. """
+        node_uuid = os.getenv('OS_FUNCTIONAL_NODE_UUID')
+        node_name = os.getenv('OS_FUNCTIONAL_NODE_NAME')
+        listings = esi.node_list(self.clients['admin'], long=True)
+        self.assertNotEqual(listings, [])
+        if node_uuid is not None:
+            self.assertIn(node_uuid, [x['UUID'] for x in listings])
+        if node_name is not None:
+            self.assertIn(node_name, [x['Name'] for x in listings])
+
+    @unittest.skipIf('OS_FUNCTIONAL_NODE_NAME' not in os.environ.keys(),
+                     'Environment variable OS_FUNCTIONAL_NODE_NAME not set')
+    def test_node_list_basic(self):
+        """ Tests basic functionality of "esi node list" when default behavior
+            is invoked. Checks if node_name is present in node list.
+            Test steps:
+            1) Set the environment variable using
+               export OS_FUNCTIONAL_NODE_IDENT_NAME=node_name
+            2) Checks that the output of "node list" contains
+               the node name it's tested with. """
+        node_name = os.getenv('OS_FUNCTIONAL_NODE_IDENT_NAME')
+        listings = esi.node_list(self.clients['admin'])
+        self.assertNotEqual(listings, [])
+        self.assertIn(node_name, [x['Name'] for x in listings])
+
     @pytest.mark.negative
     def test_offer_show_invalid_id(self):
         """ Tests that "esi offer show" properly handles being passed an
                 offer uuid that does not exist.
             Test steps:
             1) Attempt to show details of an offer that does not exist.
             2) Check that the command failed. (returned non-zero exit code)
```

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_policy.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_policy.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/v1/test_sublease.py` & `python-esileapclient-0.2.2/esileapclient/tests/functional/v1/test_sublease.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/esileapclient/tests/functional/README.md` & `python-esileapclient-0.2.2/esileapclient/tests/functional/README.md`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/setup.py` & `python-esileapclient-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/tox.ini` & `python-esileapclient-0.2.2/tox.ini`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/ChangeLog` & `python-esileapclient-0.2.2/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+0.2.2
+-----
+
+* add purpose field to esi lease command
+* functional-test-for-esi-node-list
+* Updated CI, resolved pytest collection warning
+
 0.2.1
 -----
 
 * Add node state information
 * update lease list tooltip
 
 0.2.0
```

### Comparing `python-esileapclient-0.2.1/README.md` & `python-esileapclient-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/.github/workflows/tests.yml` & `python-esileapclient-0.2.2/.github/workflows/tests.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 name: python-esileapclient
 
 on: [push, pull_request]
 
 jobs:
   build:
 
-    runs-on: ubuntu-latest
+    runs-on: ubuntu-20.04
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9"]
+        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox
       - name: Lint
```

### Comparing `python-esileapclient-0.2.1/LICENSE` & `python-esileapclient-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/setup.cfg` & `python-esileapclient-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/conftest.py` & `python-esileapclient-0.2.2/conftest.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/python_esileapclient.egg-info/PKG-INFO` & `python-esileapclient-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,15 @@
 Metadata-Version: 2.1
 Name: python-esileapclient
-Version: 0.2.1
+Version: 0.2.2
 Summary: ESI-LEAP CLI
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
-Description: # python-esileapclient
-        
-        Python API for interacting with [ESI-Leap](https://github.com/CCI-MOC/esi-leap)
-        
-        ### Overview
-        
-        This is a client for the OpenStack Lease API. It provides:
-        
-           - a openstack command-line plugin: `openstack lease`
-        
-        python-esileapclient is licensed under the Apache License, Version 2.0, like the rest of OpenStack.
-        
-        ### Installation
-        
-        To install as a package:
-        ```
-        # pip install python-esileapclient`
-        ```
-        
-        To install from source:
-        ```
-        $ git clone https://github.com/CCI-MOC/python-esileapclient
-        $ cd python-esileapclient
-        # python setup.py install
-        ```
-        
-        ### `openstack lease` CLI
-        
-        The `openstack lease` command-line interface is available when the lease plugin (included in this package) is used with the [OpenStackClient](https://docs.openstack.org/python-openstackclient/latest/)
-        
-        The client uses the OpenStack Identity API (Keystone) to authenticate users with an OpenStack cloud and to locate the lease service endpoint (see [here](https://docs.openstack.org/keystone/latest/admin/manage-services.html) for more info). Currently, overriding this endpoint is not supported. Credentials for authentication can be provided via command-line parameters (e.g. `--os-username, --os-password, etc.`) or by setting environment variables (e.g. `OS_USERNAME, OS_PASSWORD`).
-        
-        Usage Examples:
-        
-            openstack esi offer list
-        
-        will make a GET request to ESI-Leap and print to screen a list of all the offers in the ESI-Leap database.
-        
-            openstack esi offer show <uuid>
-        
-        will make a GET request and print fields for offer with the given uuid.
-        
-            openstack esi offer create --resource-type dummy_node --resource-uuid 1718
-        
-        will make a POST request to ESI-Leap to create the offer with the given credentials. Prints to the screen the newly created offer with resource type 'dummy\_node' and resource uuid '1718'.
-        
-            openstack esi offer delete <uuid>
-        
-        will make a DELETE request to ESI-Leap to delete the request with the given uuid. Prints to the screen whether the command was a success or not.
-        
-        
-        This repository is currently a work in progress.
-        
-        
 Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
@@ -72,7 +18,65 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# python-esileapclient
+
+Python API for interacting with [ESI-Leap](https://github.com/CCI-MOC/esi-leap)
+
+### Overview
+
+This is a client for the OpenStack Lease API. It provides:
+
+   - a openstack command-line plugin: `openstack lease`
+
+python-esileapclient is licensed under the Apache License, Version 2.0, like the rest of OpenStack.
+
+### Installation
+
+To install as a package:
+```
+# pip install python-esileapclient`
+```
+
+To install from source:
+```
+$ git clone https://github.com/CCI-MOC/python-esileapclient
+$ cd python-esileapclient
+# python setup.py install
+```
+
+### `openstack lease` CLI
+
+The `openstack lease` command-line interface is available when the lease plugin (included in this package) is used with the [OpenStackClient](https://docs.openstack.org/python-openstackclient/latest/)
+
+The client uses the OpenStack Identity API (Keystone) to authenticate users with an OpenStack cloud and to locate the lease service endpoint (see [here](https://docs.openstack.org/keystone/latest/admin/manage-services.html) for more info). Currently, overriding this endpoint is not supported. Credentials for authentication can be provided via command-line parameters (e.g. `--os-username, --os-password, etc.`) or by setting environment variables (e.g. `OS_USERNAME, OS_PASSWORD`).
+
+Usage Examples:
+
+    openstack esi offer list
+
+will make a GET request to ESI-Leap and print to screen a list of all the offers in the ESI-Leap database.
+
+    openstack esi offer show <uuid>
+
+will make a GET request and print fields for offer with the given uuid.
+
+    openstack esi offer create --resource-type dummy_node --resource-uuid 1718
+
+will make a POST request to ESI-Leap to create the offer with the given credentials. Prints to the screen the newly created offer with resource type 'dummy\_node' and resource uuid '1718'.
+
+    openstack esi offer delete <uuid>
+
+will make a DELETE request to ESI-Leap to delete the request with the given uuid. Prints to the screen whether the command was a success or not.
+
+
+This repository is currently a work in progress.
+
+
+
```

### Comparing `python-esileapclient-0.2.1/python_esileapclient.egg-info/entry_points.txt` & `python-esileapclient-0.2.2/python_esileapclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.1/python_esileapclient.egg-info/SOURCES.txt` & `python-esileapclient-0.2.2/python_esileapclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

