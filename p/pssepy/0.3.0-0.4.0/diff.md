# Comparing `tmp/pssepy-0.3.0.tar.gz` & `tmp/pssepy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/PyPSSE/PyPSSE/dist/tmpdx8feo22/pssepy-0.3.0.tar", last modified: Thu Sep 15 17:52:22 2022, max compression
+gzip compressed data, was "/home/runner/work/PyPSSE/PyPSSE/dist/.tmp-h997nc5a/pssepy-0.4.0.tar", last modified: Wed Jun 21 22:36:39 2023, max compression
```

## Comparing `pssepy-0.3.0.tar` & `pssepy-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-09-15 17:52:09.000000 pssepy-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-09-15 17:52:22.000000 pssepy-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      864 2022-09-15 17:52:09.000000 pssepy-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pssepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-09-15 17:52:22.000000 pssepy-0.3.0/pssepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-09-15 17:52:22.000000 pssepy-0.3.0/pssepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 17:52:22.000000 pssepy-0.3.0/pssepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-09-15 17:52:22.000000 pssepy-0.3.0/pssepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-09-15 17:52:22.000000 pssepy-0.3.0/pssepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-09-15 17:52:22.000000 pssepy-0.3.0/pssepy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5393 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/api/pypsse.py
--rw-r--r--   0 runner    (1001) docker     (121)     2601 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/api/server.py
--rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/channel_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     6627 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/contingencies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/data_writers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/data_writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/data_writers/csv.py
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/data_writers/data_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3724 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/data_writers/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     2131 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/data_writers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/defaults/
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/defaults/export_settings.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/defaults/simulation_settings.toml
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    21285 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/helics_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/modes/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/modes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    40351 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/modes/abstract_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     7490 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/modes/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    14963 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/modes/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)    12954 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/modes/snap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2248 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/modes/static.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6634 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/parsers/gic_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/parsers/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/profile_manager/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/profile_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/profile_manager/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/profile_manager/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     7527 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/profile_manager/profile_store.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/pylogger.py
--rw-r--r--   0 runner    (1001) docker     (121)    18025 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/pypsse_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/pypsse_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     7903 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/pypsse_project.py
--rw-r--r--   0 runner    (1001) docker     (121)     3995 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/result_container.py
--rw-r--r--   0 runner    (1001) docker     (121)      713 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/simulation_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 17:52:22.000000 pssepy-0.3.0/pypsse/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5401 2022-09-15 17:52:09.000000 pssepy-0.3.0/pypsse/utils/dynamic_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-09-15 17:52:09.000000 pssepy-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 17:52:22.000000 pssepy-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2023 2022-09-15 17:52:09.000000 pssepy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-21 22:36:27.000000 pssepy-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-21 22:36:39.000000 pssepy-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-21 22:36:27.000000 pssepy-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pssepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-21 22:36:39.000000 pssepy-0.4.0/pssepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-06-21 22:36:39.000000 pssepy-0.4.0/pssepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:36:39.000000 pssepy-0.4.0/pssepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-21 22:36:39.000000 pssepy-0.4.0/pssepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-21 22:36:39.000000 pssepy-0.4.0/pssepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 22:36:39.000000 pssepy-0.4.0/pssepy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/api/pypsse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/api/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/channel_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/contingencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/data_writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/data_writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/data_writers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/data_writers/data_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/data_writers/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/data_writers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/defaults/export_settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/defaults/simulation_settings.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23236 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/helics_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/mdao.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/modes/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/modes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41420 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/modes/abstract_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/modes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/modes/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/modes/pcm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/modes/snap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/modes/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6634 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/parsers/gic_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/parsers/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/profile_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/profile_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/profile_manager/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/profile_manager/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7527 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/profile_manager/profile_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/pylogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16948 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/pypsse_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/pypsse_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7903 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/pypsse_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/result_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/simulation_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/pypsse/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-06-21 22:36:27.000000 pssepy-0.4.0/pypsse/utils/dynamic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-21 22:36:27.000000 pssepy-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:36:39.000000 pssepy-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-21 22:36:27.000000 pssepy-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:39.000000 pssepy-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:36:27.000000 pssepy-0.4.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-21 22:36:27.000000 pssepy-0.4.0/tests/test_create_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-21 22:36:27.000000 pssepy-0.4.0/tests/test_dynamic_utils.py
```

### Comparing `pssepy-0.3.0/PKG-INFO` & `pssepy-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pssepy
-Version: 0.3.0
+Version: 0.4.0
 Summary: A high-level python interface for PSS/E
 Home-page: http://www.github.com/nrel/pypsse
 Author: Aadil Latif
 Author-email: Aadil.Latif@nrel.gov
 License: BSD 3 clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: ==3.7.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ﻿## :blush: Welcome to the PyPSSE Repository
 
 > A python wrapper around psspy (python API for PSSE simulator) to perform
 > time series powerflow and dynamic simulation for power system fault
```

### Comparing `pssepy-0.3.0/README.md` & `pssepy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pssepy.egg-info/PKG-INFO` & `pssepy-0.4.0/pssepy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pssepy
-Version: 0.3.0
+Version: 0.4.0
 Summary: A high-level python interface for PSS/E
 Home-page: http://www.github.com/nrel/pypsse
 Author: Aadil Latif
 Author-email: Aadil.Latif@nrel.gov
 License: BSD 3 clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: ==3.7.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 ﻿## :blush: Welcome to the PyPSSE Repository
 
 > A python wrapper around psspy (python API for PSSE simulator) to perform
 > time series powerflow and dynamic simulation for power system fault
```

### Comparing `pssepy-0.3.0/pssepy.egg-info/SOURCES.txt` & `pssepy-0.4.0/pssepy.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pssepy.egg-info/top_level.txt
 pypsse/__init__.py
 pypsse/channel_map.py
 pypsse/common.py
 pypsse/contingencies.py
 pypsse/exceptions.py
 pypsse/helics_interface.py
+pypsse/mdao.py
 pypsse/pylogger.py
 pypsse/pypsse_instance.py
 pypsse/pypsse_logger.py
 pypsse/pypsse_project.py
 pypsse/result_container.py
 pypsse/simulation_controller.py
 pypsse/api/__init__.py
@@ -30,18 +31,22 @@
 pypsse/data_writers/json.py
 pypsse/defaults/export_settings.toml
 pypsse/defaults/simulation_settings.toml
 pypsse/modes/__init__.py
 pypsse/modes/abstract_mode.py
 pypsse/modes/constants.py
 pypsse/modes/dynamic.py
+pypsse/modes/pcm.py
 pypsse/modes/snap.py
 pypsse/modes/static.py
 pypsse/parsers/__init__.py
 pypsse/parsers/gic_parser.py
 pypsse/parsers/reader.py
 pypsse/profile_manager/__init__.py
 pypsse/profile_manager/common.py
 pypsse/profile_manager/profile.py
 pypsse/profile_manager/profile_store.py
 pypsse/utils/__init__.py
-pypsse/utils/dynamic_utils.py
+pypsse/utils/dynamic_utils.py
+tests/test_api.py
+tests/test_create_project.py
+tests/test_dynamic_utils.py
```

### Comparing `pssepy-0.3.0/pypsse/api/pypsse.py` & `pssepy-0.4.0/pypsse/api/pypsse.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/api/server.py` & `pssepy-0.4.0/pypsse/api/server.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/channel_map.py` & `pssepy-0.4.0/pypsse/channel_map.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/common.py` & `pssepy-0.4.0/pypsse/common.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/contingencies.py` & `pssepy-0.4.0/pypsse/contingencies.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/data_writers/csv.py` & `pssepy-0.4.0/pypsse/data_writers/csv.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,20 +36,18 @@
             Data = powerflow_output[obj_type]
             if obj_type not in self.dfs:
                 self.dfs[obj_type] = [Data]
             else:
                 if self.dfs[obj_type] is None:
                     self.dfs[obj_type] = [Data]
                 else:
-                    self.dfs[obj_type].appenf(Data)
+                    self.dfs[obj_type].append(Data)
 
             if self.step % self.chunkRows == self.chunkRows - 1:
                 fpath = os.path.join(self.log_dir, f'{obj_type}.csv')
-                print(fpath)
                 self.dfs[obj_type] =  pd.DataFrame(self.dfs[obj_type], index=self.timestamps)
-                print(self.dfs[obj_type])
                 self.dfs[obj_type].to_csv(fpath, mode='a')
                 
                 self.dfs[obj_type] = None
             self.Timestamp[self.step-1] = np.string_(str(currenttime))
         self.step += 1
```

### Comparing `pssepy-0.3.0/pypsse/data_writers/data_writer.py` & `pssepy-0.4.0/pypsse/data_writers/data_writer.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/data_writers/hdf5.py` & `pssepy-0.4.0/pypsse/data_writers/hdf5.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,23 +51,27 @@
             Data = Data.fillna(0)
             
             if obj_type not in self.row:
                 self.row[obj_type] = 0
                 self.store_groups[obj_type] = self.store.create_group(obj_type)
                 self.store_datasets[obj_type] = {}
                 for colName in powerflow_output[obj_type].keys():
+                    dtype = Data[colName].dtype
+                    if dtype == object:
+                        dtype = "S30"
+            
                     self.store_datasets[obj_type][colName] = self.store_groups[obj_type].create_dataset(
-                        str(colName) + "_test",
+                        str(colName) ,
                         shape=(self.columnLength, ),
                         maxshape=(None, ),
                         chunks=True,
                         compression="gzip",
                         compression_opts=4,
                         shuffle=True,
-                        dtype=Data[colName].dtype
+                        dtype=dtype
                     )
             
             if obj_type not in self.dfs:
                 self.dfs[obj_type] = Data
             else:
                 if self.dfs[obj_type] is None:
                     self.dfs[obj_type] = Data
```

### Comparing `pssepy-0.3.0/pypsse/data_writers/json.py` & `pssepy-0.4.0/pypsse/data_writers/json.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/defaults/export_settings.toml` & `pssepy-0.4.0/pypsse/defaults/export_settings.toml`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/defaults/simulation_settings.toml` & `pssepy-0.4.0/pypsse/defaults/simulation_settings.toml`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 [Loads.reactive_load]
 "% constant current" = 50.0
 "% constant admittance" = 50.0
 
 [Generators]
 "Missing machine model" = 1 # 0: treat as a fatal error 1: replace with net machine power
 
+[MDAO]
+"use_microservices" = false
+
 # [contingencies.bus_fault.bf_1]
 # "time" = 1.0
 # "bus_id" = 25048#25824, 25059
 # "duration" = 0.1
 # "bus_trip" = true
 # "trip_delay" = 5.0
 # "fault_impedance" = [0.0001, 0.00000001]
```

### Comparing `pssepy-0.3.0/pypsse/helics_interface.py` & `pssepy-0.4.0/pypsse/helics_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,30 @@
 import helics as h
 import time
 import ast
 import os
 
 class helics_interface:
 
+    all_sub_results = {}
+    all_pub_results = {}
+    
     dynamic_iter_const = 1000.0
     n_states = 5
     init_state = 1
     dynamic_params = ['FmA', 'FmB', 'FmC', 'FmD', 'Fel']
 
     def __init__(self, PSSE, sim, settings, export_settings, bus_subsystems, logger):
         self.bus_pubs = ['bus_id', 'bus_Vmag', 'bus_Vang', 'bus_dev']
         self.PSSE = PSSE
         self.logger = logger
         self.settings = settings
         self.export_settings = export_settings
         self.bus_subsystems = bus_subsystems
         self.sim = sim
-        self.itr = 0
         self.c_seconds = 0
         self.c_seconds_old = -1
 
         if self.settings["Simulation"]["Simulation mode"] in ["Dynamic", "Snap"]:
             self.create_replica_model_for_coupled_loads(['FmD'])
             
         self._co_convergance_error_tolerance = settings['HELICS']['Error tolerance']
@@ -36,15 +38,15 @@
         self.publications = {}
         self.subscriptions = {}
        
         return
     
     def create_replica_model_for_coupled_loads(self, components_to_replace):
         components_to_stay = [x for x in self.dynamic_params if x not in components_to_replace]
-        loads = self.get_coupled_loads()
+        loads = self._get_coupled_loads()
         loads = self._get_load_static_data(loads)
         loads = self._get_load_dynamic_data(loads)
         loads = self._replicate_coupled_load(loads, components_to_replace)
         self._update_dynamic_parameters(loads, components_to_stay, components_to_replace)
         return 
 
     def _update_dynamic_parameters(self, loads, components_to_stay, components_to_replace):
@@ -65,16 +67,14 @@
                 settings[idx] =  v
                 #self.PSSE.change_ldmod_con(load['bus'], 'XX' ,r"""CMLDBLU2""" ,idx ,v)
             values = list(settings.values())
             self.PSSE.add_load_model(load['bus'], 'XX', 0, 1, r"""CMLDBLU2""", 2, [0,0], ["",""], 133, values)
             self.logger.info(f"Dynamic model parameters for load {load['name']} at bus 'XX' changed.")
 
     def _get_load_dynamic_properties(self, load):
-        print("Load name: ", load['name'])
-        print("Load bus: ", load['bus'])
         settings = {}
         for i in range(133):
             irr, con_index = self.PSSE.lmodind(load["bus"], load['name'], 'CHARAC', 'CON')
             if con_index is not None:
                 act_con_index = con_index + i
                 irr, value = self.PSSE.dsrval('CON', act_con_index)
                 settings[i] = value
@@ -148,15 +148,25 @@
                     if con_index is not None:
                         act_con_index = con_index + con_ind
                         irr, value = self.PSSE.dsrval('CON', act_con_index)
                         load[v] = value
         return loads
 
     def enter_execution_mode(self):
-        h.helicsFederateEnterExecutingMode(self.PSSEfederate)
+        itr = 0
+        itr_flag = h.helics_iteration_request_iterate_if_needed
+        while True:
+            itr_status = h.helicsFederateEnterExecutingModeIterative(
+                self.PSSEfederate, 
+                itr_flag
+                ) 
+            self.logger.debug(f"--- Iter {itr}: Iteration Status = {itr_status}, Passed Iteration Requestion = {itr_flag}")
+            if itr_status == h.helics_iteration_result_next_step:
+                break
+        
         return
 
     def create_federate(self):
         self.fedinfo = h.helicsCreateFederateInfo()
         h.helicsFederateInfoSetCoreName(self.fedinfo, self.settings["HELICS"]['Federate name'])
         h.helicsFederateInfoSetCoreTypeFromString(self.fedinfo, self.settings["HELICS"]['Core type'])
         h.helicsFederateInfoSetCoreInitString(self.fedinfo, "--federates=1")
@@ -180,15 +190,14 @@
         self.PSSEfederate = h.helicsCreateValueFederate(self.settings["HELICS"]['Federate name'], self.fedinfo)
         return
 
     def register_publications(self, bus_subsystems):
         self.publications = {}
         self.pub_struc = []
         for publicationDict in self.settings['HELICS']["Publications"]:
-            print(publicationDict)
             bus_subsystem_ids = publicationDict["bus_subsystems"]
             if not set(bus_subsystem_ids).issubset(self.bus_subsystems):
                 raise Exception(f"One or more invalid bus subsystem ID pass in {bus_subsystem_ids}."
                                 f"Valid subsystem IDs are  '{list(self.bus_subsystems.keys())}'.")
 
             elmClass = publicationDict["class"]
             if elmClass not in self.export_settings:
@@ -306,39 +315,67 @@
                     if r not in self.psse_dict[row['bus']][row['element_type']][element_id]:
                         self.psse_dict[row['bus']][row['element_type']][element_id][r] = 0
 
         return
 
     def request_time(self, t):
         r_seconds = self.sim.GetTotalSeconds()  # - self._dss_solver.GetStepResolutionSeconds()
+        if self.sim.getTime() not in self.all_sub_results:
+            self.all_sub_results[self.sim.getTime()] = {}
+            self.all_pub_results[self.sim.getTime()] = {}
+        
         if not self.settings['HELICS']['Iterative Mode']:
             while self.c_seconds < r_seconds:
                 self.c_seconds = h.helicsFederateRequestTime(self.PSSEfederate, r_seconds)
             self.logger.info('Time requested: {} - time granted: {} '.format(r_seconds, self.c_seconds))
             return True, self.c_seconds
         else:
-            error = max([abs(x["dStates"][0] - x["dStates"][1]) for k, x in self.subscriptions.items()])
-            if self.itr == 0:
-                while self.c_seconds < r_seconds:
-                    self.c_seconds = h.helicsFederateRequestTime(self.PSSEfederate, r_seconds)
-            else:
-                self.c_seconds, iteration_state = h.helicsFederateRequestTimeIterative(
+            itr = 0
+            epsilon = 1e-6
+            while True:
+                
+                self.c_seconds, itr_state = h.helicsFederateRequestTimeIterative(
                     self.PSSEfederate,
                     r_seconds,
-                    h.helics_iteration_request_force_iteration
+                    h.helics_iteration_request_iterate_if_needed
                 )
-            self.logger.info('Time requested: {} - time granted: {} error: {} it: {}'.format(
-                r_seconds, self.c_seconds, error, self.itr))
-            # self._co_convergance_error_tolerance
-            if error > -1 and self.itr < self._co_convergance_max_iterations - 1:   #self._co_convergance_error_tolerance 
-                self.itr += 1
-                return False, self.c_seconds
-            else:
-                self.itr = 0
-                return True, self.c_seconds
+                if (itr_state == h.helics_iteration_result_next_step):
+                    self.logger.debug("\tIteration complete!")
+                    break
+                
+                error = max([abs(x["dStates"][0] - x["dStates"][1]) for k, x in self.subscriptions.items()])                
+                
+                subscriptions = self.subscribe() 
+                for sub_name, sub_value in subscriptions.items():
+                    if sub_name not in self.all_sub_results[self.sim.getTime()]:
+                        self.all_sub_results[self.sim.getTime()][sub_name] = []
+                    self.all_sub_results[self.sim.getTime()][sub_name].append(sub_value)
+             
+                self.sim.resolveStep(r_seconds)       
+                
+                publications = self.publish()
+                for pub_name, pub_value in publications.items():
+                    if pub_name not in self.all_pub_results[self.sim.getTime()]:
+                        self.all_pub_results[self.sim.getTime()][pub_name] = []
+                    self.all_pub_results[self.sim.getTime()][pub_name].append(pub_value)
+                
+                itr += 1
+                self.logger.debug(f"\titr = {itr}")
+                
+                if itr > self.settings['HELICS']['Max co-iterations']:
+                    self.c_seconds, itr_state = h.helicsFederateRequestTimeIterative(
+                        self.PSSEfederate,
+                        r_seconds,
+                        h.helics_iteration_request_no_iteration
+                    )
+                else:
+                    pass
+                
+            return True, self.c_seconds
+
 
     def get_restructured_results(self, results):
         results_dict = {}
         for k, d in results.items():
             c, p = k.split("_")
             if c not in results_dict:
                 results_dict[c] = {}
@@ -346,23 +383,26 @@
                 if isinstance(n, str):
                     n = n.replace(" ", "")
                 if n not in results_dict[c]:
                     results_dict[c][n] = {p:v}
         return results_dict
 
     def publish(self):
+        pub_results = {}
         for quantities, subsystem_buses in self.pub_struc:
             temp_res = self.sim.read_subsystems(quantities, subsystem_buses)
             temp_res = self.get_restructured_results(temp_res)
             for cName, elmInfo in temp_res.items():
                 for Name, vInfo in elmInfo.items():
                     for pName, val in vInfo.items():
                         pub_tag = "{}.{}.{}.{}".format(self.settings["HELICS"]['Federate name'], cName, Name, pName)
+                        pub_tag_reduced = f"{cName}.{Name}.{pName}" 
                         pub = self.publications[pub_tag]
                         dtype_matched = True
+                        pub_results[pub_tag_reduced] = val
                         if isinstance(val, float):
                             h.helicsPublicationPublishDouble(pub, val)
                         elif isinstance(val, complex):
                             h.helicsPublicationPublishComplex(pub, val.real, val.imag)
                         elif isinstance(val, int):
                             h.helicsPublicationPublishInteger(pub, val)
                         elif isinstance(val, list):
@@ -370,59 +410,62 @@
                         elif isinstance(val, str):
                             h.helicsPublicationPublishString(pub, val)
                         else:
                             dtype_matched = False
                             self.logger.warning(f"Publication {pub_tag} not updated")
                         if dtype_matched:
                             self.logger.debug(f"Publication {pub_tag} published: {val}")
-        return
+        return pub_results
 
     def subscribe(self):
         for sub_tag, sub_data in self.subscriptions.items():
             if isinstance(sub_data["property"], str):
                 sub_data['value'] = h.helicsInputGetDouble(sub_data['subscription'])
                 self.psse_dict[sub_data['bus']][sub_data['element_type']][sub_data['element_id']][sub_data["property"]] = (sub_data['value'], sub_data['scaler'])
             elif isinstance(sub_data["property"], list):
                 sub_data['value'] = h.helicsInputGetVector(sub_data['subscription'])
                 if isinstance(sub_data['value'], list) and len(sub_data['value']) == len(sub_data["property"]):
                     for i, p in enumerate(sub_data["property"]):
                         self.psse_dict[sub_data['bus']][sub_data['element_type']][sub_data['element_id']][p] = (sub_data['value'][i], sub_data['scaler'][i])
 
-
             self.logger.debug('Data received {} for tag {}'.format(sub_data['value'], sub_tag))
             if self.settings['HELICS']['Iterative Mode']:
                 if self.c_seconds != self.c_seconds_old:
                     sub_data['dStates'] = [self.init_state] * self.n_states
                 else:
                     sub_data['dStates'].insert(0, sub_data['dStates'].pop())
-
+        all_values = {}
         for b, bInfo in self.psse_dict.items():
             for t, tInfo in bInfo.items():
                 for i, vDict in tInfo.items():
                     values = {}
                     j = 0
                     for p, v in vDict.items():
                         if isinstance(v, tuple):
                             v , scale = v
+                            all_values[f'{t}.{b}.{i}.{p}'] = v
                             if isinstance(p, str):
                                 ppty = f'realar{PROFILE_VALIDATION[t].index(p) + 1}'
                                 values[ppty] = v * scale
                             elif isinstance(p, list):
                                 for alpha, ppt in enumerate(p):
                                     ppty = f'realar{PROFILE_VALIDATION[t].index(ppt) + 1}'
                                     values[ppty] = v * scale
                         j += 1
 
                     isEmpty = [0 if not vx else 1 for vx in values.values()]
-                    if sum(isEmpty) != 0:
+                    if sum(isEmpty) != 0 and sum(values.values()) < 1e6 and sum(values.values()) > -1e6:
                         self.sim.update_object(t, b, i, values)
-
+                        self.logger.debug(f'{t}.{b}.{i} = {values}')
+                        
+                    else:
+                        self.logger.debug('write failed')
 
         self.c_seconds_old = self.c_seconds
-        return self.subscriptions
+        return all_values
 
     def fill_missing_values(self, value):
         idx = [f'realar{PROFILE_VALIDATION[self.dType].index(c) + 1}' for c in self.Columns]
         x = dict(zip(idx, list(value)))
         return x
 
     def __del__(self):
```

### Comparing `pssepy-0.3.0/pypsse/modes/abstract_mode.py` & `pssepy-0.4.0/pypsse/modes/abstract_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,16 @@
                                 'SBASE1', 'NOMV1', 'NOMV2', 'NOMV2', 'GMAGNT', 'BMAGNT', 'RG1', 'XG1', 'R01', 'X01', 'RG2',
                                 'XG2', 'R02', 'X02', 'RNUTRL', 'XNUTRL'],
                     'tr3dt2': ['RX1-2', 'RX2-3', 'RX3-1', 'YMAGNT', 'ZG1', 'Z01', 'ZG2', 'Z02', 'ZG3', 'Z03', 'ZNUTRL' ],
                     'trfnofunc': ['FROMBUSNUM_3WDG','FROMBUSNUM_2WDG','TOBUSNUM_3WDG','TOBUSNUM_2WDG', 'TOBUS2NUM_3WDG', \
                         'FROMBUSNAME_3WDG','FROMBUSNAME_2WDG','TOBUSNAME_3WDG','TOBUSNAME_2WDG', 'TOBUS2NAME_3WDG','CIRCUIT_2WDG', 'CIRCUIT_3WDG']
                 }
             }
-        #self.disable_load_models_for_coupled_buses()
+        #self.
+        # ()
         self.initialization_complete = False
 
     # def disable_load_models_for_coupled_buses(self):
     #     if self.settings['HELICS']['Cosimulation mode']:
     #         sub_data = pd.read_csv(
     #         os.path.join(
     #             self.settings["Simulation"]["Project Path"], 'Settings', self.settings["HELICS"]["Subscriptions file"]
@@ -114,15 +115,33 @@
     #     self.psse_dict = {}
     #     for ix, row in sub_data.iterrows():
     #         bus = row['bus']
     #         load = row['element_id']
     #         ierr = self.PSSE.ldmod_status(0,int(bus),str(load),1,0)
     #         self.logger.error(f"Dynamic model for load {load} connected to bus {bus} has been disabled")
 
-
+    def save_model(self):
+        
+        export_path = os.path.join( self.settings["Simulation"]["Project Path"], 'Case_study' )
+        i = 0
+        while os.path.exists(os.path.join(export_path, f"modified_steady_state_{i}.sav")):
+            i += 1
+        
+        savfile = os.path.join(export_path, f"modified_steady_state_{i}.sav")
+        rawfile = os.path.join(export_path, f"modified_steady_state_{i}.raw")
+        #self.PSSE.save(savfile)    
+        self.PSSE.rawd_2(0,1,[1,1,1,0,0,0,0], 0, rawfile)         
+        if self.settings["Simulation"]["Simulation mode"] in ["Dynamic", "Snap"]:
+            snpfile = os.path.join(export_path, f"modified_dynamic_{i}.snp")
+            self.PSSE.snap([-1,-1,-1,-1,-1], snpfile)
+            return savfile, snpfile
+    
+        else:
+            return savfile, None
+    
 
     def init(self, bus_subsystems):
         self.export_path = os.path.join(self.settings["Simulation"]["Project Path"], 'Exports')
         self.study_case_path = os.path.join(
             self.settings["Simulation"]["Project Path"], 'Case_study', self.settings["Simulation"]["Case study"]
         )
         self.dyr_path = os.path.join(
@@ -635,14 +654,21 @@
         return results_dict
 
     def update_object(self, dType, bus, id, values):
         #print(dType, bus, id, values)
         val = sum([x for x in values.values()])
         if val > -1000000.0 and val < 100000.0:
             if dType == "Load":
+                # print(dType, bus, id, values)
+                # import math
+                # pf = 0.9
+                # s = values['realar1'] / pf
+                # a = math.sin(math.acos(pf)) 
+                # q = s * a
+                # #values['realar2'] = q
                 ierr = self.PSSE.load_chng_5(ibus=int(bus), id=id, **values)
             elif dType == "Induction_machine":
                 ierr = self.PSSE.induction_machine_data(ibus=int(bus), id=id, **values)
             elif dType == "Machine":
                 ierr = self.PSSE.machine_data_2(i=int(bus), id=id, **values)
             elif dType == "Plant":
                 ierr = self.PSSE.plant_data_4(ibus=int(bus), inode=id, **values)
```

### Comparing `pssepy-0.3.0/pypsse/modes/constants.py` & `pssepy-0.4.0/pypsse/modes/constants.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/modes/dynamic.py` & `pssepy-0.4.0/pypsse/modes/dynamic.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,14 @@
                 load = row['element_id']
                 ierr = self.PSSE.ldmod_status(0, int(bus), str(load), 1, 0)
                 self.logger.error(f"Dynamic model for load {load} connected to bus {bus} has been disabled")
 
     def step(self, t):
         self.time = self.time + datetime.timedelta(seconds=self.incTime)
         self.xTime = 0
-        print(t)
         return self.PSSE.run(0, t, 1, 1, 1)
 
     def setup_machine_channels(self, machines, properties):
         for i, qty in enumerate(properties):
             if qty not in self.channel_map:
                 nqty = f"MACHINE_{qty}"
                 self.channel_map[nqty] = {}
@@ -241,16 +240,14 @@
                     'Bus name': load_data[1, i],
                     'Bus name (ext)': load_data[2, i],
                 }
             all_bus_ids[id] = load_info
         return all_bus_ids
 
     def resolveStep(self, t):
-        print(t)
-        print(self.xTime * self.incTime / self.iter_const)
         err = self.PSSE.run(0, t + self.xTime * self.incTime / self.iter_const, 1, 1, 1)
         self.xTime += 1
         return err
 
     def getTime(self):
         return self.time
```

### Comparing `pssepy-0.3.0/pypsse/modes/snap.py` & `pssepy-0.4.0/pypsse/modes/snap.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         ierr = self.PSSE.rstr(self.snp_file)
         assert ierr == 0, "error={}".format(ierr)
         ierr = self.PSSE.strt_2([0, 1],  self.outx_path)
 
         self.disable_load_models_for_coupled_buses()
         self.disable_generation_for_coupled_buses()
 
+        #self.save_model()
 
         if ierr==1:
             self.PSSE.cong(0)
             ierr = self.PSSE.strt_2([0, 1],  self.outx_path)
             assert ierr == 0, "error={}".format(ierr)
         
         elif ierr >1:
@@ -232,15 +233,15 @@
                 self.PSSE.conl(0, 1, 1, [0, 0], [P1, P2, Q1, Q2]) # initialize for load conversion.
                 self.PSSE.conl(0, 1, 2, [0, 0], [P1, P2, Q1, Q2]) # convert loads.
                 self.PSSE.conl(0, 1, 3, [0, 0], [P1, P2, Q1, Q2]) # postprocessing housekeeping.
 
 
     @converter
     def read_subsystems(self, quantities, subsystem_buses, ext_string2_info={}, mapping_dict={}):
-        #print(ext_string2_info, mapping_dict)
+
         results = super(Snap, self).read_subsystems(
             quantities,
             subsystem_buses,
             mapping_dict=mapping_dict,
             ext_string2_info=ext_string2_info
         )
 
@@ -260,15 +261,15 @@
                                         ierr, ld_id = self.PSSE.nxtlod(int(bus))
                                         if ld_id is not None:
                                             irr, con_index = getattr(self.PSSE, funcName)(int(bus), ld_id, 'CHARAC',
                                                                                           'CON')
                                             if con_index is not None:
                                                 act_con_index = con_index + con_ind
                                                 irr, value = self.PSSE.dsrval('CON', act_con_index)
-                                                # print(class_name, funcName, bus, ld_id, con_index, con_num, v, value)
+
                                                 res_base = f"{class_name}_{v}"
                                                 if res_base not in results:
                                                     results[res_base] = {}
                                                 obj_name = f"{bus}_{ld_id}"
                                                 results[res_base][obj_name] = value
             else:
                 self.logger.warning("Extend function 'read_subsystems' in the Snap class (Snap.py)")
```

### Comparing `pssepy-0.3.0/pypsse/modes/static.py` & `pssepy-0.4.0/pypsse/modes/static.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/parsers/gic_parser.py` & `pssepy-0.4.0/pypsse/parsers/gic_parser.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/parsers/reader.py` & `pssepy-0.4.0/pypsse/parsers/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 
     def __init__(self, psse_instance, logger):
 
         self.psse = psse_instance
         self.logger = logger
         self.buses = self.get_data('abus', tails=['int'], strings=["NUMBER"], flags=[2])
         self.loads = self.get_data('aload', tails=['int','char'], strings=["NUMBER","ID"], flags=[4,4])
+        self.loads = self.get_data('aload', tails=['int','char'], strings=["NUMBER","ID"], flags=[4,4])
         self.fixed_stunts = self.get_data('afxshunt',tails=['int','char'], strings=["NUMBER","ID"], flags=[4,4])
         self.generators = self.get_data('amach',tails=['int','char'], strings=["NUMBER","ID"], flags=[4,4])
-        self.branches = self.get_data('abrn',tails=['int','int'], strings=["FROMNUMBER","TONUMBER"], flags=[2,2])
+        self.branches = self.get_data('abrn',tails=['int','int','char'], strings=["FROMNUMBER","TONUMBER", "ID"], flags=[2,2,2])
         self.transformers = self.get_data('atr3',tails=['int','int','int'], strings=["WIND1NUMBER","WIND2NUMBER","WIND3NUMBER"], flags=[2,2,2])
         self.Area = self.get_data('aarea',tails=['int','char'], strings=["NUMBER","AREANAME"], flags=[2,2])  # Talk to Aadil
         self.DC_branch = self.get_data('a2trmdc',tails=['int','int'], strings=["FROMNUMBER","TONUMBER"], flags=[2,2])  # three terminal dc lines not implemented
         self.multi_term_dc = self.get_data('amultitrmdc',tails=['int','int'], strings=["VCNPOSNUMBER","VCNNEGNUMBER"], flags=[2,2])
         self.switched_shunt = self.get_data('aswsh', tails=['int','char'], strings=["NUMBER","DEVICENAME"], flags=[4,4])
         self.zones = self.get_data('azone',tails=['int','char'], strings=["NUMBER","ZONENAME"], flags=[2,2])
         self.owners = self.get_data('aowner',tails=['int','char'], strings=["NUMBER","OWNERNAME"], flags=[2,2])
```

### Comparing `pssepy-0.3.0/pypsse/profile_manager/common.py` & `pssepy-0.4.0/pypsse/profile_manager/common.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/profile_manager/profile.py` & `pssepy-0.4.0/pypsse/profile_manager/profile.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/profile_manager/profile_store.py` & `pssepy-0.4.0/pypsse/profile_manager/profile_store.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/pylogger.py` & `pssepy-0.4.0/pypsse/pylogger.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/pypsse_instance.py` & `pssepy-0.4.0/pypsse/pypsse_instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,43 +23,40 @@
 import time
 
 USING_NAERM = 0
 
 class pyPSSE_instance:
 
     def __init__(self, settinigs_toml_path='', psse_path=''):
-      
+        self.settings = self.read_settings(settinigs_toml_path)
         if psse_path != '':
+            self.settings["Simulation"]["PSSE_path"] = psse_path.lower()
             sys.path.append(psse_path)
             os.environ['PATH'] += ';' + psse_path
 
         else:
-        
-            self.settings = self.read_settings(settinigs_toml_path)
+            self.settings["Simulation"]["PSSE_path"]
             if self.settings["Simulation"]["Simulation mode"] == "Dynamic":
                 assert self.settings["Simulation"]["Use profile manager"] == False,\
                     "Profile manager can not be used for dynamic simulations. Set 'Use profile manager' to False"
 
-
             sys.path.append(self.settings["Simulation"]["PSSE_path"])
             os.environ['PATH'] += ';' + self.settings["Simulation"]["PSSE_path"]
-
-        
+       
         try:
             nBus = 200000
             if "psse34" in self.settings["Simulation"]["PSSE_path"].lower():
                 import psse34
             elif "psse35" in self.settings["Simulation"]["PSSE_path"].lower():
                 import psse35
             else:
                 import psse36
             import psspy
             import dyntools
 
-
             self.dyntools = dyntools
             self.PSSE = psspy
             # self.logger.debug('Initializing PSS/E. connecting to license server')
             ierr = self.PSSE.psseinit(nBus)
 
             self.PSSE.psseinit(nBus)
             self.initComplete = True
@@ -149,28 +146,14 @@
 
     def disable_generation_for_coupled_buses(self):
         if self.settings['HELICS']['Cosimulation mode'] and self.settings['HELICS'][
             "Disable_generation_on_coupled_buses"]:
             pass
         return
 
-    def initialize_loads(self):
-        #         data = pd.read_csv(r'C:\NAERM-global\init_Conditions_3_new.csv', header=0, index_col=None)
-        # data = data.values
-        # r, c = data.shape
-        # for i in range(r):
-        #     bus_data = data[i, :]
-        #     bus_id = bus_data[0]
-        #     P = bus_data[3]
-        #     Q = bus_data[4]
-        #
-        #     ierr = self.PSSE.load_chng_5(ibus=int(bus_id), id='1', realar=[P, Q, 0, 0, 0, 0, 0, 0])
-        #     if ierr:
-        #         self.logger.debug('ERROR: Load not updated')
-        return
 
     def init(self):
         sucess = self.sim.init(self.bus_subsystems)
         # if sucess:
         #     self.load_info = self.sim.load_info
         # else:
         #     self.load_info = None
@@ -240,15 +223,15 @@
     def run(self):
       
         if self.sim.initialization_complete:
             if self.settings['Plotting']["Enable dynamic plots"]:
                 bokeh_server_proc = subprocess.Popen(["bokeh", "serve"], stdout=subprocess.PIPE)
             else:
                 bokeh_server_proc = None
-            self.initialize_loads()
+            #self.initialize_loads()
             self.logger.debug('Running dynamic simulation for time {} sec'.format(
                 self.settings["Simulation"]["Simulation time (sec)"])
             )
             self.logger.debug(
                 'Simulation time step {} sec'.format(self.settings["Simulation"]["Step resolution (sec)"]))
             T = self.settings["Simulation"]["Simulation time (sec)"]
             t = 0
@@ -259,15 +242,18 @@
                 if t >= T:
                     break
 
             self.PSSE.pssehalt_2()
             if not self.export_settings["Export results using channels"]:
                 self.results.export_results()
             else:
+                
                 self.sim.export()
+            
+            export_path = os.path.join(self.settings["Simulation"]["Project Path"], 'Exports')
 
             if bokeh_server_proc != None:
                 bokeh_server_proc.terminate()
         else:
             self.logger.error(
                 'Run init() command to initialize models before running the simulation')
         return
@@ -286,15 +272,15 @@
             if self.settings["HELICS"]["Create subscriptions"]:
                 self.update_subscriptions()
                 self.logger.debug('Time requested: {}'.format(t))
                 self.inc_time, helics_time = self.update_federate_time(t)
                 self.logger.debug('Time granted: {}'.format(helics_time))
 
         if self.inc_time:
-            self.sim.step(t)
+            a = self.sim.step(t)
         else:
             self.sim.resolveStep(t)
 
         if self.settings["HELICS"]["Cosimulation mode"]:
             self.publish_data()
         if self.export_settings['Defined bus subsystems only']:
             curr_results = self.sim.read_subsystems(self.exp_vars, self.all_subsysten_buses)
@@ -405,44 +391,26 @@
             c.update(t)
 
     def inject_contingencies_external(self,temp):
         print("external settings : ", temp , flush=True)
         contingencies = c.build_contingencies(self.PSSE, temp, self.logger)
         self.contingencies.update(contingencies)
     
-    def save_model(self):
-        
-        export_path = os.path.join( self.settings["Simulation"]["Project Path"], 'Case_study' )
-        i = 0
-        while os.path.exists(f"modified_steady_state_{i}.sav") and os.path.exists(f"modified_dynamic_{i}.snp"):
-            i += 1
-        
-        savfile = os.path.join(export_path, f"modified_steady_state_{i}.sav")
-        self.PSSE.save(savfile)    
-                 
-        if self.settings["Simulation"]["Simulation mode"] in ["Dynamic", "Snap"]:
-            snpfile = os.path.join(export_path, f"modified_dynamic_{i}.snp")
-            self.PSSE.snap([-1,-1,-1,-1,-1], snpfile)
-            return savfile, snpfile
-    
-        else:
-            return savfile, None
-    
+   
     def __del__(self):
         if hasattr(self, "PSSE"):
             self.PSSE.pssehalt_2()
 
 if __name__ == '__main__':
     #x = pyPSSE_instance(r'C:\Users\alatif\Desktop\NEARM_sim\PSSE_studycase\PSSE_WECC_model\Settings\simulation_settings.toml')
     x = pyPSSE_instance(r'C:\Users\alatif\Desktop\PYPSSE\examples\dynamic_example\Settings\simulation_settings.toml')
     x.init()
     for i in range(10):
         t = i / 240.0
         res = x.step(t)
-        print(res)
         res = x.get_results({'Buses': ['PU', 'FREQ']})
 
     # scenarios = [14203, 14303, 14352, 15108, 15561, 17604, 17605, 37102, 37124, 37121]
     # for s in scenarios:
     #     x = pyPSSE_instance(f'C:\\Users\\alatif\\Desktop\\Naerm\\PyPSSE\\TransOnly\\Settings\{s}.toml')
     #     x.init()
     #     x.run()
```

### Comparing `pssepy-0.3.0/pypsse/pypsse_logger.py` & `pssepy-0.4.0/pypsse/pypsse_logger.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/pypsse_project.py` & `pssepy-0.4.0/pypsse/pypsse_project.py`

 * *Files identical despite different names*

### Comparing `pssepy-0.3.0/pypsse/result_container.py` & `pssepy-0.4.0/pypsse/result_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,25 +54,27 @@
         if self.export_settings["Write format"] not in self.BULK_WRITE_MODES:
             self.dataWriter.write(self.settings["HELICS"]["Federate name"], time, bus_data, index)
         else:
             for variable_name, bus_dict in bus_data.items():
                 if not isinstance(self.results['{}'.format(variable_name)], pd.DataFrame):
                     self.results['{}'.format(variable_name)] = pd.DataFrame(bus_data[variable_name], index=[0])
                 else:
-
-                    self.results['{}'.format(variable_name)] = self.results['{}'.format(variable_name)].append(
-                        bus_data[variable_name], ignore_index=True)
+                    df1 = self.results['{}'.format(variable_name)]
+                    df2 = pd.DataFrame.from_dict([bus_data[variable_name]]) 
+                    concatenated = pd.concat([df1, df2])
+                    self.results['{}'.format(variable_name)] = concatenated
         return
 
     def export_results(self):
         if self.export_settings["Write format"] in self.BULK_WRITE_MODES:
             for df_name, df in self.results.items():
                 export_path = os.path.join(
                     self.settings["Simulation"]["Project Path"],
                     'Exports',
                     '{}.{}'.format(df_name, self.export_settings["Write format"])
                 )
                 if self.export_settings["Write format"] == 'csv':
-                    df.to_csv(export_path)
+                    if isinstance(df, pd.DataFrame):
+                        df.to_csv(export_path)
                 elif self.export_settings["Write format"] == "pkl":
                     df.to_pickle(export_path)
         return
```

### Comparing `pssepy-0.3.0/pypsse/utils/dynamic_utils.py` & `pssepy-0.4.0/pypsse/utils/dynamic_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,22 +54,22 @@
             for comp in components_to_replace:
                 static_percentage += load[comp]
             remaining_load = 1 - static_percentage
             total_load = load['MVA'] 
             total_distribution_load = total_load * static_percentage
             total_transmission_load = total_load * remaining_load
             #ceate new load
-            self.PSSE.load_data_6(
+            self.PSSE.load_data_5(
                 load['bus'], "XX", 
                 realar=[total_transmission_load.real, total_transmission_load.imag, 0.0, 0.0, 0.0, 0.0],
                 lodtyp='replica'
                 )
             #ierr, cmpval = self.PSSE.loddt2(load["bus"], "XX" ,"MVA" , "ACT")
             #modify old load     
-            self.PSSE.load_data_6(
+            self.PSSE.load_data_5(
                 load['bus'], load['id'], 
                 realar=[total_distribution_load.real, total_distribution_load.imag, 0.0, 0.0, 0.0, 0.0],
                 lodtyp='original'
                 )   
             #ierr, cmpval = self.PSSE.loddt2(load["bus"], load["id"] ,"MVA" , "ACT")    
             self.logger.info(f"Original load {load['id']} @ bus {load['bus']}: {total_load}")
             self.logger.info(f"New load 'XX' @ bus {load['bus']} created successfully: {total_transmission_load}")
```

### Comparing `pssepy-0.3.0/setup.py` & `pssepy-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
       package_data={'pypsse': ['*.toml']},
         entry_points={
             "console_scripts": [
                 "pypsse=pypsse.cli.pypsse:cli",
             ],
         },
       license='BSD 3 clause',
-      python_requires='==3.7.*',
+      python_requires='>=3.9',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Environment :: Console',
           'Environment :: Web Environment',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'Operating System :: OS Independent',
```

