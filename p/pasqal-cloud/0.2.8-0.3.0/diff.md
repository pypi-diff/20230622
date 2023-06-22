# Comparing `tmp/pasqal-cloud-0.2.8.tar.gz` & `tmp/pasqal-cloud-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pasqal-cloud-0.2.8.tar", last modified: Mon Jun 19 16:12:46 2023, max compression
+gzip compressed data, was "pasqal-cloud-0.3.0.tar", last modified: Thu Jun 22 15:02:59 2023, max compression
```

## Comparing `pasqal-cloud-0.2.8.tar` & `pasqal-cloud-0.3.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7556 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     6013 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud/device/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/emu_free.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/emu_tn.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/device/emulator_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/job.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/pasqal_cloud/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/utils/jsend.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pasqal_cloud/utils/strenum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.836451 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 16:12:46.000000 pasqal-cloud-0.2.8/pasqal_cloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/device/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/device/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/device/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/device/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_cloud_sdk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_device_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:46.840451 pasqal-cloud-0.2.8/tests/test_doubles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_doubles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_doubles/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-19 16:12:38.000000 pasqal-cloud-0.2.8/tests/test_project_renaming_compatibility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.840326 pasqal-cloud-0.3.0/pasqal_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.840326 pasqal-cloud-0.3.0/pasqal_cloud/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/emu_free.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/emu_tn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/device/emulator_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/pasqal_cloud/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/utils/jsend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pasqal_cloud/utils/strenum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.840326 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 15:02:59.000000 pasqal-cloud-0.3.0/pasqal_cloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/device/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/device/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/device/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.844326 pasqal-cloud-0.3.0/sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_cloud_sdk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_device_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:59.848326 pasqal-cloud-0.3.0/tests/test_doubles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_doubles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_doubles/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-22 15:02:46.000000 pasqal-cloud-0.3.0/tests/test_project_renaming_compatibility.py
```

### Comparing `pasqal-cloud-0.2.8/LICENSE` & `pasqal-cloud-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/PKG-INFO` & `pasqal-cloud-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: pasqal-cloud
-Version: 0.2.8
-Summary: Software development kit for Pasqal cloud platform.
-Home-page: https://github.com/pasqal-io/pasqal-cloud
-Maintainer: Pasqal Cloud Services
-Maintainer-email: pcs@pasqal.io
-License: Apache 2.0
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
 
 To install the latest release of the `pasqal-cloud` (formerly pasqal-sdk), have Python 3.8.0 or higher installed, then use pip:
@@ -40,16 +25,14 @@
 
 To run the tutorials or the test suite locally, run the following to install the development requirements:
 
 ```bash
 pip install -e .[dev]
 ```
 
-
-
 ## Basic usage
 
 The package main component is a python object called `SDK` which can be used to create a `Batch` and send it automatically
 to Pasqal APIs using an API token generated in the [user portal](https://portal.pasqal.cloud).
 
 A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.  
 The batch sequence can be generated using [Pulser](https://github.com/pasqal-io/Pulser). See their [documentation](https://pulser.readthedocs.io/en/stable/),
@@ -87,14 +70,20 @@
 from pasqal_cloud.device import EmulatorType
 batch = sdk.create_batch(serialized_sequence, [job1,job2], emulator=EmulatorType.EMU_FREE)
 
 # Once the QPU has returned the results, you can access them with the following:
 for job in batch.jobs.values():
     print(job.result)
 
+# Note that this results are extracted from the "counter" key of the results.
+# To access the full results, or in the event that the results aren't expected
+# to contain a "counter" you can do:
+for job in batch.jobs.values():
+    print(job.full_result)
+
 ```
 
 ## Advanced usage
 
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
@@ -127,15 +116,15 @@
 class CustomTokenProvider(TokenProvider):
     def get_token(self):
         return "your-token" # Replace this value with your token
 
 
 sdk = SDK(token_provider=CustomTokenProvider(), project_id=project_id)
 
-""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a 
+""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a
     custom _query_token method which fetches your token. See Auth0TokenProvider implementation for an example.
 """
 ```
 
 ### Extra emulator configuration (Soon publicly available)
 
 Some emulators, such as EMU_TN and EMU_FREE, accept further configuration to control the emulation.
@@ -172,25 +161,25 @@
 ```python
 sdk.get_device_specs_dict()
 ```
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
-
 ### Target different API endpoints
 
-This is intended to the package developers or users which were given access to non-prod 
+This is intended to the package developers or users which were given access to non-prod
 environments of the PASQAL cloud platform.
 
-To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
-`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
+To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using
+`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for
 `auth0` with env being the environment you want to target.
 
 Example:
+
 ```python
 from pasqal_cloud import AUTH0_CONFIG, SDK, PASQAL_ENDPOINTS
 
 sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH0_CONFIG['preprod'])
 ```
 
 By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.8/README.md` & `pasqal-cloud-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: pasqal-cloud
+Version: 0.3.0
+Summary: Software development kit for Pasqal cloud platform.
+Home-page: https://github.com/pasqal-io/pasqal-cloud
+Maintainer: Pasqal Cloud Services
+Maintainer-email: pcs@pasqal.io
+License: Apache 2.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 # PASQAL Cloud
 
 SDK to be used to access Pasqal Cloud Services.
 
 ## Installation
 
 To install the latest release of the `pasqal-cloud` (formerly pasqal-sdk), have Python 3.8.0 or higher installed, then use pip:
@@ -25,16 +40,14 @@
 
 To run the tutorials or the test suite locally, run the following to install the development requirements:
 
 ```bash
 pip install -e .[dev]
 ```
 
-
-
 ## Basic usage
 
 The package main component is a python object called `SDK` which can be used to create a `Batch` and send it automatically
 to Pasqal APIs using an API token generated in the [user portal](https://portal.pasqal.cloud).
 
 A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.  
 The batch sequence can be generated using [Pulser](https://github.com/pasqal-io/Pulser). See their [documentation](https://pulser.readthedocs.io/en/stable/),
@@ -72,14 +85,20 @@
 from pasqal_cloud.device import EmulatorType
 batch = sdk.create_batch(serialized_sequence, [job1,job2], emulator=EmulatorType.EMU_FREE)
 
 # Once the QPU has returned the results, you can access them with the following:
 for job in batch.jobs.values():
     print(job.result)
 
+# Note that this results are extracted from the "counter" key of the results.
+# To access the full results, or in the event that the results aren't expected
+# to contain a "counter" you can do:
+for job in batch.jobs.values():
+    print(job.full_result)
+
 ```
 
 ## Advanced usage
 
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
@@ -112,15 +131,15 @@
 class CustomTokenProvider(TokenProvider):
     def get_token(self):
         return "your-token" # Replace this value with your token
 
 
 sdk = SDK(token_provider=CustomTokenProvider(), project_id=project_id)
 
-""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a 
+""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a
     custom _query_token method which fetches your token. See Auth0TokenProvider implementation for an example.
 """
 ```
 
 ### Extra emulator configuration (Soon publicly available)
 
 Some emulators, such as EMU_TN and EMU_FREE, accept further configuration to control the emulation.
@@ -157,25 +176,25 @@
 ```python
 sdk.get_device_specs_dict()
 ```
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
-
 ### Target different API endpoints
 
-This is intended to the package developers or users which were given access to non-prod 
+This is intended to the package developers or users which were given access to non-prod
 environments of the PASQAL cloud platform.
 
-To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
-`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
+To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using
+`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for
 `auth0` with env being the environment you want to target.
 
 Example:
+
 ```python
 from pasqal_cloud import AUTH0_CONFIG, SDK, PASQAL_ENDPOINTS
 
 sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH0_CONFIG['preprod'])
 ```
 
 By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/__init__.py` & `pasqal-cloud-0.3.0/pasqal_cloud/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -103,21 +103,25 @@
                 (#TODO: Make optional after Iroise MVP)
             emulator: The type of emulator to use,
               If set to None, the device_type will be set to the one
               stored in the serialized sequence
             configuration: A dictionary with extra configuration for the emulators
                 that accept it.
             wait: Whether to wait for the batch to be done
-            fetch_results: Whether to download the results. Implies waiting
-                for the batch.
 
 
         Returns:
             Batch: The new batch that has been created in the database.
         """
+        if fetch_results:
+            warn(
+                ("The parameter fetch_results has no effect and is deprecated."),
+                DeprecationWarning,
+                stacklevel=2,
+            )
 
         req = {
             "sequence_builder": serialized_sequence,
             "webhook": self.webhook,
             "jobs": jobs,
         }
 
@@ -127,43 +131,43 @@
             req.update({"emulator": emulator})
 
         # The configuration field is only added in the case
         # it's requested
         if configuration:
             req.update({"configuration": configuration.to_dict()})  # type: ignore
 
-        batch_rsp, jobs_rsp = self._client._send_batch(req)
+        batch_rsp = self._client._send_batch(req)
         batch_id = batch_rsp["id"]
-        if wait or fetch_results:
+        if wait:
             while batch_rsp["status"] in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
-                batch_rsp, jobs_rsp = self._client._get_batch(batch_id)
+                batch_rsp = self._client._get_batch(batch_id)
 
-            if fetch_results:
-                batch_rsp, jobs_rsp = self._client._get_batch(
-                    batch_id, fetch_results=True
-                )
-        batch = Batch(**batch_rsp, jobs=jobs_rsp, _client=self._client)
+        batch = Batch(**batch_rsp, _client=self._client)
 
         self.batches[batch.id] = batch
         return batch
 
     def get_batch(self, id: str, fetch_results: bool = False) -> Batch:
         """Retrieve a batch's data and all its jobs.
 
         Args:
             id: ID of the batch.
-            fetch_results: whether to download job results
 
         Returns:
             Batch: the batch stored in the PCS database.
         """
-
-        batch_rsp, jobs_rsp = self._client._get_batch(id, fetch_results=fetch_results)
-        batch = Batch(**batch_rsp, jobs=jobs_rsp, _client=self._client)
+        if fetch_results:
+            warn(
+                ("The parameter fetch_results has no effect and is deprecated."),
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        batch_rsp = self._client._get_batch(id)
+        batch = Batch(**batch_rsp, _client=self._client)
         self.batches[batch.id] = batch
         return batch
 
     def cancel_batch(self, id: str) -> Batch:
         """Cancel the given batch on the PCS
 
         Args:
```

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/_version.py` & `pasqal-cloud-0.3.0/pasqal_cloud/_version.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.8"
+__version__ = "0.3.0"
```

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/authentication.py` & `pasqal-cloud-0.3.0/pasqal_cloud/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/batch.py` & `pasqal-cloud-0.3.0/pasqal_cloud/batch.py`

 * *Files 6% similar despite different names*

```diff
@@ -119,40 +119,33 @@
         if wait:
             while job.status in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
                 job_rsp = self._client._get_job(job.id)
                 job = Job(**job_rsp)
         return job
 
-    def declare_complete(
-        self, wait: bool = False, fetch_results: bool = False
-    ) -> Dict[str, Any]:
+    def declare_complete(self, wait: bool = False) -> Dict[str, Any]:
         """Declare to PCS that the batch is complete.
 
         Args:
             wait: Whether to wait for the batch to be done.
-            fetch_results: Whether to download the results. Implies waiting for the batch.
 
         A batch that is complete awaits no extra jobs. All jobs previously added
         will be executed before the batch is terminated. When all its jobs are done,
         the complete batch is unassigned to its running device.
         """
         batch_rsp = self._client._complete_batch(self.id)
         self.complete = True
-        if wait or fetch_results:
+        if wait:
             while batch_rsp["status"] in ["PENDING", "RUNNING"]:
                 time.sleep(RESULT_POLLING_INTERVAL)
-                batch_rsp, jobs_rsp = self._client._get_batch(
+                batch_rsp = self._client._get_batch(
                     self.id,
                 )
-            if fetch_results:
-                batch_rsp, jobs_rsp = self._client._get_batch(
-                    self.id, fetch_results=True
-                )
-            for job_rsp in jobs_rsp:
+            for job_rsp in batch_rsp["jobs"]:
                 self.jobs[job_rsp["id"]] = Job(**job_rsp)
         return batch_rsp
 
     def cancel(self) -> Dict[str, Any]:
         """Cancel the current batch on the PCS."""
         batch_rsp = self._client._cancel_batch(self.id)
         self.status = batch_rsp.get("status", "CANCELED")
```

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/client.py` & `pasqal-cloud-0.3.0/pasqal_cloud/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from __future__ import annotations
 
 from getpass import getpass
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, Optional
 
 import requests
 from requests.auth import AuthBase
 
 from pasqal_cloud.authentication import (
     TokenProvider,
     Auth0TokenProvider,
@@ -110,40 +110,28 @@
         )
         data: JSendPayload = rsp.json()
         if rsp.status_code >= 400:
             raise HTTPError(data)
 
         return data
 
-    def _send_batch(
-        self, batch_data: Dict[str, Any]
-    ) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
+    def _send_batch(self, batch_data: Dict[str, Any]) -> Dict[str, Any]:
         batch_data.update({"project_id": self.project_id})
         batch_data = self._request(
             "POST",
             f"{self.endpoints.core}/api/v1/batches",
             batch_data,
         )["data"]
-        jobs_data = batch_data.pop("jobs", [])
-        return batch_data, jobs_data
+        return batch_data
 
-    def _get_batch(
-        self, id: str, fetch_results: bool = False
-    ) -> Tuple[Dict[str, Any], List[Dict[str, Any]]]:
+    def _get_batch(self, id: str) -> Dict[str, Any]:
         batch_data: Dict[str, Any] = self._request(
             "GET", f"{self.endpoints.core}/api/v1/batches/{id}"
         )["data"]
-        jobs_data = batch_data.pop("jobs", [])
-        if fetch_results:
-            results = self._request(
-                "GET", f"{self.endpoints.core}/api/v1/batches/{id}/results"
-            )["data"]
-            for job_data in jobs_data:
-                job_data["result"] = results.get(str(job_data["id"]), None)
-        return batch_data, jobs_data
+        return batch_data
 
     def _complete_batch(self, batch_id: str) -> Dict[str, Any]:
         response: Dict[str, Any] = self._request(
             "PUT", f"{self.endpoints.core}/api/v1/batches/{batch_id}/complete"
         )["data"]
         return response
```

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/base_config.py` & `pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/base_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/device/configuration/emu_tn.py` & `pasqal-cloud-0.3.0/pasqal_cloud/device/configuration/emu_tn.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/endpoints.py` & `pasqal-cloud-0.3.0/pasqal_cloud/endpoints.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/errors.py` & `pasqal-cloud-0.3.0/pasqal_cloud/errors.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/job.py` & `pasqal-cloud-0.3.0/pasqal_cloud/job.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     _client: Client
     created_at: str
     updated_at: str
     errors: Optional[List[str]] = None
     start_timestamp: Optional[str] = None
     end_timestamp: Optional[str] = None
     result: Optional[Dict[str, Any]] = None
+    full_result: Optional[Dict[str, Any]] = None
     variables: Optional[Dict[str, Any]] = None
     # Ticket (#622)
     group_id: Optional[str] = None
 
     class Config:
         extra = Extra.allow
         arbitrary_types_allowed = True
```

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud/utils/jsend.py` & `pasqal-cloud-0.3.0/pasqal_cloud/utils/jsend.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud.egg-info/PKG-INFO` & `pasqal-cloud-0.3.0/pasqal_cloud.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pasqal-cloud
-Version: 0.2.8
+Version: 0.3.0
 Summary: Software development kit for Pasqal cloud platform.
 Home-page: https://github.com/pasqal-io/pasqal-cloud
 Maintainer: Pasqal Cloud Services
 Maintainer-email: pcs@pasqal.io
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
@@ -40,16 +40,14 @@
 
 To run the tutorials or the test suite locally, run the following to install the development requirements:
 
 ```bash
 pip install -e .[dev]
 ```
 
-
-
 ## Basic usage
 
 The package main component is a python object called `SDK` which can be used to create a `Batch` and send it automatically
 to Pasqal APIs using an API token generated in the [user portal](https://portal.pasqal.cloud).
 
 A `Batch` is a group of jobs with the same sequence that will run on the same QPU. For each job of a given batch you must set a value for each variable, if any, defined in your sequence.  
 The batch sequence can be generated using [Pulser](https://github.com/pasqal-io/Pulser). See their [documentation](https://pulser.readthedocs.io/en/stable/),
@@ -87,14 +85,20 @@
 from pasqal_cloud.device import EmulatorType
 batch = sdk.create_batch(serialized_sequence, [job1,job2], emulator=EmulatorType.EMU_FREE)
 
 # Once the QPU has returned the results, you can access them with the following:
 for job in batch.jobs.values():
     print(job.result)
 
+# Note that this results are extracted from the "counter" key of the results.
+# To access the full results, or in the event that the results aren't expected
+# to contain a "counter" you can do:
+for job in batch.jobs.values():
+    print(job.full_result)
+
 ```
 
 ## Advanced usage
 
 ### Authentication
 
 There are several ways to provide a correct authentication using the SDK.
@@ -127,15 +131,15 @@
 class CustomTokenProvider(TokenProvider):
     def get_token(self):
         return "your-token" # Replace this value with your token
 
 
 sdk = SDK(token_provider=CustomTokenProvider(), project_id=project_id)
 
-""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a 
+""" Alternatively, create a custom TokenProvider that inherits from ExpiringTokenProvider. You should define a
     custom _query_token method which fetches your token. See Auth0TokenProvider implementation for an example.
 """
 ```
 
 ### Extra emulator configuration (Soon publicly available)
 
 Some emulators, such as EMU_TN and EMU_FREE, accept further configuration to control the emulation.
@@ -172,25 +176,25 @@
 ```python
 sdk.get_device_specs_dict()
 ```
 
 The method returns a dict object mapping a device type to a serialized device specs. These specs can be used
 to instantiate a `Device` instance in the `Pulser` library.
 
-
 ### Target different API endpoints
 
-This is intended to the package developers or users which were given access to non-prod 
+This is intended to the package developers or users which were given access to non-prod
 environments of the PASQAL cloud platform.
 
-To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using 
-`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for 
+To target a specific environment (`prod`, `preprod` or `dev`), instantiate the SDK class using
+`PASQAL_ENDPOINTS['env']` for the parameter `endpoints` and `AUTH0_CONFIG['env']` for
 `auth0` with env being the environment you want to target.
 
 Example:
+
 ```python
 from pasqal_cloud import AUTH0_CONFIG, SDK, PASQAL_ENDPOINTS
 
 sdk = SDK(..., endpoints=PASQAL_ENDPOINTS['preprod'], auth0=AUTH0_CONFIG['preprod'])
 ```
 
 By default, the targeted environment for `endpoints` and `auth0` is `prod`.
```

### Comparing `pasqal-cloud-0.2.8/pasqal_cloud.egg-info/SOURCES.txt` & `pasqal-cloud-0.3.0/pasqal_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/sdk/setup.py` & `pasqal-cloud-0.3.0/sdk/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/setup.py` & `pasqal-cloud-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/conftest.py` & `pasqal-cloud-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/test_batch.py` & `pasqal-cloud-0.3.0/tests/test_batch.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     def init_sdk(self, start_mock_request):
         self.sdk = SDK(
             username="me@test.com", password="password", project_id=str(uuid4())
         )
         self.pulser_sequence = "pulser_test_sequence"
         self.batch_id = "00000000-0000-0000-0000-000000000001"
         self.job_result = {"1001": 12, "0110": 35, "1111": 1}
+        self.job_full_result = {
+            "counter": {"1001": 12, "0110": 35, "1111": 1},
+            "raw": ["1001", "1001", "0110", "1001", "0110"],
+        }
         self.n_job_runs = 50
         self.job_id = "00000000-0000-0000-0000-000000022010"
         self.job_variables = {"Omega_max": 14.4, "last_target": "q1", "ts": [200, 500]}
 
     @pytest.mark.parametrize("emulator", [None] + [e.value for e in EmulatorType])
     def test_create_batch(self, emulator):
         job = {"runs": self.n_job_runs, "variables": self.job_variables}
@@ -46,34 +50,16 @@
             batch.id == "00000000-0000-0000-0000-000000000001"
         )  # the batch_id used in the mock data
         assert batch.sequence_builder == self.pulser_sequence
         assert batch.complete
         assert batch.jobs
         for job_id, job in batch.jobs.items():
             assert self.job_id == job_id
-            assert job.result is None
-        assert request_mock.last_request.method == "GET"
-
-    def test_create_batch_and_fetch_results(self, request_mock):
-        job = {"runs": self.n_job_runs, "variables": self.job_variables}
-        batch = self.sdk.create_batch(
-            serialized_sequence=self.pulser_sequence,
-            jobs=[job],
-            wait=True,
-            fetch_results=True,
-        )
-        assert (
-            batch.id == "00000000-0000-0000-0000-000000000001"
-        )  # the batch_id used in the mock data
-        assert batch.sequence_builder == self.pulser_sequence
-        assert batch.complete
-        assert batch.jobs
-        for job_id, job in batch.jobs.items():
-            assert self.job_id == job_id
             assert job.result == self.job_result
+            assert job.full_result == self.job_full_result
         assert request_mock.last_request.method == "GET"
 
     def test_get_batch(self, batch):
         batch_requested = self.sdk.get_batch(batch.id)
         assert batch_requested.id == self.batch_id
 
     def test_cancel_batch_self(self, request_mock, batch):
@@ -146,14 +132,15 @@
         assert job.runs == self.n_job_runs
         assert request_mock.last_request.method == "GET"
         assert (
             request_mock.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}"
         )
         assert job.result == self.job_result
+        assert job.full_result == self.job_full_result
 
     @pytest.mark.skip(reason="Not enabled during Iroise MVP")
     def test_batch_declare_complete(self):
         batch = self.sdk.create_batch(
             serialized_sequence=self.pulser_sequence,
         )
         rsp = batch.declare_complete(wait=False)
@@ -170,14 +157,15 @@
         assert request_mock.last_request.method == "GET"
         assert (
             request_mock.last_request.url
             == f"{self.sdk._client.endpoints.core}/api/v1/jobs/{self.job_id}"
         )
         assert batch.jobs[self.job_id].batch_id == batch.id
         assert batch.jobs[self.job_id].result == self.job_result
+        assert batch.jobs[self.job_id].full_result == self.job_full_result
 
     @pytest.mark.parametrize(
         "emulator, configuration, expected",
         [
             (EmulatorType.EMU_TN, EmuTNConfig(), EmuTNConfig()),
             (None, None, None),
             (
@@ -213,7 +201,24 @@
         # We add an extra field to mimick the API exposing new values to the user
         batch_dict["new_field"] = "any_value"
 
         new_batch = Batch(**batch_dict)  # this should raise no error
         assert (
             new_batch.new_field == "any_value"
         )  # The new value should be stored regardless
+
+    def test_create_batch_fetch_results_deprecated(
+        self,
+    ):
+        job = {"runs": self.n_job_runs, "variables": self.job_variables}
+        with pytest.warns(DeprecationWarning):
+            self.sdk.create_batch(
+                serialized_sequence=self.pulser_sequence,
+                jobs=[job],
+                fetch_results=True,
+            )
+
+    def test_get_batch_fetch_results_deprecated(
+        self,
+    ):
+        with pytest.warns(DeprecationWarning):
+            self.sdk.get_batch(self.batch_id, fetch_results=True)
```

### Comparing `pasqal-cloud-0.2.8/tests/test_client.py` & `pasqal-cloud-0.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/test_cloud_sdk_import.py` & `pasqal-cloud-0.3.0/tests/test_cloud_sdk_import.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/test_config.py` & `pasqal-cloud-0.3.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/test_device_specs.py` & `pasqal-cloud-0.3.0/tests/test_device_specs.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/test_doubles/authentication.py` & `pasqal-cloud-0.3.0/tests/test_doubles/authentication.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/test_job.py` & `pasqal-cloud-0.3.0/tests/test_job.py`

 * *Files identical despite different names*

### Comparing `pasqal-cloud-0.2.8/tests/test_project_renaming_compatibility.py` & `pasqal-cloud-0.3.0/tests/test_project_renaming_compatibility.py`

 * *Files identical despite different names*

