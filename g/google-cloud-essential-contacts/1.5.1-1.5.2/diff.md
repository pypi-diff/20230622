# Comparing `tmp/google-cloud-essential-contacts-1.5.1.tar.gz` & `tmp/google-cloud-essential-contacts-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-essential-contacts-1.5.1.tar", last modified: Mon Mar 27 15:58:21 2023, max compression
+gzip compressed data, was "google-cloud-essential-contacts-1.5.2.tar", last modified: Thu Jun 22 18:46:26 2023, max compression
```

## Comparing `google-cloud-essential-contacts-1.5.1.tar` & `google-cloud-essential-contacts-1.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4905 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3956 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.827404 google-cloud-essential-contacts-1.5.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.827404 google-cloud-essential-contacts-1.5.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.827404 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts/
--rw-rw-r--   0 root         (0)     1003     1835 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.831403 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/
--rw-rw-r--   0 root         (0)     1003     1616 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3282 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       92 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.831403 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.831403 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/
--rw-rw-r--   0 root         (0)     1003      809 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    39240 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    48378 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py
--rw-rw-r--   0 root         (0)     1003    10815 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.831403 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/
--rw-rw-r--   0 root         (0)     1003     1561 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9298 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18645 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19035 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    42857 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.831403 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/types/
--rw-rw-r--   0 root         (0)     1003     1211 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     3467 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/types/enums.py
--rw-rw-r--   0 root         (0)     1003    12471 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/types/service.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/
--rw-r--r--   0 root         (0)     1003     4905 2023-03-27 15:58:21.000000 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1973 2023-03-27 15:58:21.000000 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:58:21.000000 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 15:58:21.000000 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 15:58:21.000000 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 15:58:21.000000 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 15:58:21.000000 google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2971 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 15:58:21.835403 google-cloud-essential-contacts-1.5.1/tests/unit/gapic/essential_contacts_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/tests/unit/gapic/essential_contacts_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   193125 2023-03-27 15:55:48.000000 google-cloud-essential-contacts-1.5.1/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4863 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3920 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.897609 google-cloud-essential-contacts-1.5.2/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.897609 google-cloud-essential-contacts-1.5.2/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.901608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/
+-rw-rw-r--   0 root         (0)     1003     1835 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.901608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/
+-rw-rw-r--   0 root         (0)     1003     1616 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3282 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       92 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.901608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/
+-rw-rw-r--   0 root         (0)     1003      809 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    39816 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    48954 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10815 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1561 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9298 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18645 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19035 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    42857 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1211 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3467 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/enums.py
+-rw-rw-r--   0 root         (0)     1003    12529 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/service.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/
+-rw-r--r--   0 root         (0)     1003     4863 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1973 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      315 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-22 18:46:26.000000 google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2965 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.905608 google-cloud-essential-contacts-1.5.2/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-22 18:46:26.909608 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   193125 2023-06-22 18:43:45.000000 google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py
```

### Comparing `google-cloud-essential-contacts-1.5.1/LICENSE` & `google-cloud-essential-contacts-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/MANIFEST.in` & `google-cloud-essential-contacts-1.5.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/PKG-INFO` & `google-cloud-essential-contacts-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-essential-contacts
-Version: 1.5.1
+Version: 1.5.2
 Summary: Google Cloud Essential Contacts API client library
-Home-page: https://github.com/googleapis/python-essential-contacts
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Essential Contacts API
-========================================
+Python Client for Essential Contacts
+====================================
 
 |stable| |pypi| |versions|
 
-`Essential Contacts API`_: helps you customize who receives notifications by providing your own list of contacts in many Google Cloud services.
+`Essential Contacts`_: helps you customize who receives notifications by providing your own list of contacts in many Google Cloud services.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-essential-contacts.svg
    :target: https://pypi.org/project/google-cloud-essential-contacts/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-essential-contacts.svg
    :target: https://pypi.org/project/google-cloud-essential-contacts/
-.. _Essential Contacts API: https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Essential Contacts: https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/essentialcontacts/latest
 .. _Product Documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Essential Contacts API.`_
+3. `Enable the Essential Contacts.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Essential Contacts API.:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Enable the Essential Contacts.:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-essential-contacts
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Essential Contacts API
+-  Read the `Client Library Documentation`_ for Essential Contacts
    to see other available methods on the client.
--  Read the `Essential Contacts API Product documentation`_ to learn
+-  Read the `Essential Contacts Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Essential Contacts API Product documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Essential Contacts Product documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-essential-contacts-1.5.1/README.rst` & `google-cloud-essential-contacts-1.5.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-Python Client for Essential Contacts API
-========================================
+Python Client for Essential Contacts
+====================================
 
 |stable| |pypi| |versions|
 
-`Essential Contacts API`_: helps you customize who receives notifications by providing your own list of contacts in many Google Cloud services.
+`Essential Contacts`_: helps you customize who receives notifications by providing your own list of contacts in many Google Cloud services.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-essential-contacts.svg
    :target: https://pypi.org/project/google-cloud-essential-contacts/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-essential-contacts.svg
    :target: https://pypi.org/project/google-cloud-essential-contacts/
-.. _Essential Contacts API: https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Essential Contacts: https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/essentialcontacts/latest
 .. _Product Documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Essential Contacts API.`_
+3. `Enable the Essential Contacts.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Essential Contacts API.:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Enable the Essential Contacts.:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -92,16 +92,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-essential-contacts
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Essential Contacts API
+-  Read the `Client Library Documentation`_ for Essential Contacts
    to see other available methods on the client.
--  Read the `Essential Contacts API Product documentation`_ to learn
+-  Read the `Essential Contacts Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Essential Contacts API Product documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Essential Contacts Product documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts/__init__.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts/gapic_version.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts/gapic_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/__init__.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/gapic_metadata.json` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/gapic_version.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/gapic_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "1.5.1"  # {x-release-please-version}
+__version__ = "1.5.2"  # {x-release-please-version}
```

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/__init__.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,16 +248,22 @@
             from google.cloud import essential_contacts_v1
 
             async def sample_create_contact():
                 # Create a client
                 client = essential_contacts_v1.EssentialContactsServiceAsyncClient()
 
                 # Initialize request argument(s)
+                contact = essential_contacts_v1.Contact()
+                contact.email = "email_value"
+                contact.notification_category_subscriptions = ['TECHNICAL_INCIDENTS']
+                contact.language_tag = "language_tag_value"
+
                 request = essential_contacts_v1.CreateContactRequest(
                     parent="parent_value",
+                    contact=contact,
                 )
 
                 # Make the request
                 response = await client.create_contact(request=request)
 
                 # Handle the response
                 print(response)
@@ -363,15 +369,21 @@
             from google.cloud import essential_contacts_v1
 
             async def sample_update_contact():
                 # Create a client
                 client = essential_contacts_v1.EssentialContactsServiceAsyncClient()
 
                 # Initialize request argument(s)
+                contact = essential_contacts_v1.Contact()
+                contact.email = "email_value"
+                contact.notification_category_subscriptions = ['TECHNICAL_INCIDENTS']
+                contact.language_tag = "language_tag_value"
+
                 request = essential_contacts_v1.UpdateContactRequest(
+                    contact=contact,
                 )
 
                 # Make the request
                 response = await client.update_contact(request=request)
 
                 # Handle the response
                 print(response)
```

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -467,16 +467,22 @@
             from google.cloud import essential_contacts_v1
 
             def sample_create_contact():
                 # Create a client
                 client = essential_contacts_v1.EssentialContactsServiceClient()
 
                 # Initialize request argument(s)
+                contact = essential_contacts_v1.Contact()
+                contact.email = "email_value"
+                contact.notification_category_subscriptions = ['TECHNICAL_INCIDENTS']
+                contact.language_tag = "language_tag_value"
+
                 request = essential_contacts_v1.CreateContactRequest(
                     parent="parent_value",
+                    contact=contact,
                 )
 
                 # Make the request
                 response = client.create_contact(request=request)
 
                 # Handle the response
                 print(response)
@@ -582,15 +588,21 @@
             from google.cloud import essential_contacts_v1
 
             def sample_update_contact():
                 # Create a client
                 client = essential_contacts_v1.EssentialContactsServiceClient()
 
                 # Initialize request argument(s)
+                contact = essential_contacts_v1.Contact()
+                contact.email = "email_value"
+                contact.notification_category_subscriptions = ['TECHNICAL_INCIDENTS']
+                contact.language_tag = "language_tag_value"
+
                 request = essential_contacts_v1.UpdateContactRequest(
+                    contact=contact,
                 )
 
                 # Make the request
                 response = client.update_contact(request=request)
 
                 # Handle the response
                 print(response)
```

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/services/essential_contacts_service/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/types/__init__.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/types/enums.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/enums.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/google/cloud/essential_contacts_v1/types/service.py` & `google-cloud-essential-contacts-1.5.2/google/cloud/essential_contacts_v1/types/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,26 +41,27 @@
 
 
 class Contact(proto.Message):
     r"""A contact that will receive notifications from Google Cloud.
 
     Attributes:
         name (str):
-            The identifier for the contact. Format:
+            Output only. The identifier for the contact. Format:
             {resource_type}/{resource_id}/contacts/{contact_id}
         email (str):
             Required. The email address to send
-            notifications to. This does not need to be a
-            Google account.
+            notifications to. The email address does not
+            need to be a Google Account.
         notification_category_subscriptions (MutableSequence[google.cloud.essential_contacts_v1.types.NotificationCategory]):
-            The categories of notifications that the
-            contact will receive communications for.
+            Required. The categories of notifications
+            that the contact will receive communications
+            for.
         language_tag (str):
-            The preferred language for notifications, as a ISO 639-1
-            language code. See `Supported
+            Required. The preferred language for notifications, as a ISO
+            639-1 language code. See `Supported
             languages <https://cloud.google.com/resource-manager/docs/managing-notification-contacts#supported-languages>`__
             for a list of supported languages.
         validation_state (google.cloud.essential_contacts_v1.types.ValidationState):
             The validity of the contact. A contact is
             considered valid if it is the correct recipient
             for notifications for a particular resource.
         validate_time (google.protobuf.timestamp_pb2.Timestamp):
```

### Comparing `google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/PKG-INFO` & `google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: google-cloud-essential-contacts
-Version: 1.5.1
+Version: 1.5.2
 Summary: Google Cloud Essential Contacts API client library
-Home-page: https://github.com/googleapis/python-essential-contacts
+Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,47 +18,47 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet
 Requires-Python: >=3.7
 License-File: LICENSE
 
-Python Client for Essential Contacts API
-========================================
+Python Client for Essential Contacts
+====================================
 
 |stable| |pypi| |versions|
 
-`Essential Contacts API`_: helps you customize who receives notifications by providing your own list of contacts in many Google Cloud services.
+`Essential Contacts`_: helps you customize who receives notifications by providing your own list of contacts in many Google Cloud services.
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |stable| image:: https://img.shields.io/badge/support-stable-gold.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
 .. |pypi| image:: https://img.shields.io/pypi/v/google-cloud-essential-contacts.svg
    :target: https://pypi.org/project/google-cloud-essential-contacts/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/google-cloud-essential-contacts.svg
    :target: https://pypi.org/project/google-cloud-essential-contacts/
-.. _Essential Contacts API: https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Essential Contacts: https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/essentialcontacts/latest
 .. _Product Documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 
 Quick Start
 -----------
 
 In order to use this library, you first need to go through the following steps:
 
 1. `Select or create a Cloud Platform project.`_
 2. `Enable billing for your project.`_
-3. `Enable the Essential Contacts API.`_
+3. `Enable the Essential Contacts.`_
 4. `Setup Authentication.`_
 
 .. _Select or create a Cloud Platform project.: https://console.cloud.google.com/project
 .. _Enable billing for your project.: https://cloud.google.com/billing/docs/how-to/modify-project#enable_billing_for_a_project
-.. _Enable the Essential Contacts API.:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Enable the Essential Contacts.:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _Setup Authentication.: https://googleapis.dev/python/google-api-core/latest/auth.html
 
 Installation
 ~~~~~~~~~~~~
 
 Install this library in a `virtualenv`_ using pip. `virtualenv`_ is a tool to
 create isolated Python environments. The basic problem it addresses is one of
@@ -116,16 +116,16 @@
     virtualenv <your-env>
     <your-env>\Scripts\activate
     <your-env>\Scripts\pip.exe install google-cloud-essential-contacts
 
 Next Steps
 ~~~~~~~~~~
 
--  Read the `Client Library Documentation`_ for Essential Contacts API
+-  Read the `Client Library Documentation`_ for Essential Contacts
    to see other available methods on the client.
--  Read the `Essential Contacts API Product documentation`_ to learn
+-  Read the `Essential Contacts Product documentation`_ to learn
    more about the product and see How-to Guides.
 -  View this `README`_ to see the full list of Cloud
    APIs that we cover.
 
-.. _Essential Contacts API Product documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
+.. _Essential Contacts Product documentation:  https://cloud.google.com/resource-manager/docs/managing-notification-contacts/
 .. _README: https://github.com/googleapis/google-cloud-python/blob/main/README.rst
```

### Comparing `google-cloud-essential-contacts-1.5.1/google_cloud_essential_contacts.egg-info/SOURCES.txt` & `google-cloud-essential-contacts-1.5.2/google_cloud_essential_contacts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/setup.py` & `google-cloud-essential-contacts-1.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
 ]
-url = "https://github.com/googleapis/python-essential-contacts"
+url = "https://github.com/googleapis/google-cloud-python"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
     readme = readme_file.read()
```

### Comparing `google-cloud-essential-contacts-1.5.1/tests/__init__.py` & `google-cloud-essential-contacts-1.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/tests/unit/__init__.py` & `google-cloud-essential-contacts-1.5.2/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/tests/unit/gapic/__init__.py` & `google-cloud-essential-contacts-1.5.2/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/tests/unit/gapic/essential_contacts_v1/__init__.py` & `google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-essential-contacts-1.5.1/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py` & `google-cloud-essential-contacts-1.5.2/tests/unit/gapic/essential_contacts_v1/test_essential_contacts_service.py`

 * *Files identical despite different names*

