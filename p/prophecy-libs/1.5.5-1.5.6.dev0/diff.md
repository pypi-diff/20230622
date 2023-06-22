# Comparing `tmp/prophecy-libs-1.5.5.tar.gz` & `tmp/prophecy-libs-1.5.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.5.5.tar", last modified: Fri Jun  9 08:12:53 2023, max compression
+gzip compressed data, was "prophecy-libs-1.5.6.dev0.tar", last modified: Thu Jun 22 20:09:58 2023, max compression
```

## Comparing `prophecy-libs-1.5.5.tar` & `prophecy-libs-1.5.6.dev0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.130308 prophecy-libs-1.5.5/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.130308 prophecy-libs-1.5.5/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.5.5/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.130308 prophecy-libs-1.5.5/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.5/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.5/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.134308 prophecy-libs-1.5.5/prophecy/transpiler/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      147 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/transpiler/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/abi_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/abi_core_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1585 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/abi_fcn_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6515 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/dataframe_fcns.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     6393 2023-05-29 13:41:07.000000 prophecy-libs-1.5.5/prophecy/transpiler/fixed_file_schema.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.5/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/udfs/scala_udf_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)    16532 2023-05-26 15:20:32.000000 prophecy-libs-1.5.5/prophecy/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)      992 2023-06-09 08:12:53.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-06-09 08:12:52.000000 prophecy-libs-1.5.5/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-06-09 08:12:53.138308 prophecy-libs-1.5.5/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-06-09 08:12:50.000000 prophecy-libs-1.5.5/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.249495 prophecy-libs-1.5.6.dev0/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-06-22 20:09:58.249495 prophecy-libs-1.5.6.dev0/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4442 2023-06-09 08:12:50.000000 prophecy-libs-1.5.6.dev0/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3551 2023-06-22 20:08:07.000000 prophecy-libs-1.5.6.dev0/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.6.dev0/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.6.dev0/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      147 2023-05-26 15:20:32.000000 prophecy-libs-1.5.6.dev0/prophecy/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      789 2023-05-29 13:41:07.000000 prophecy-libs-1.5.6.dev0/prophecy/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22828 2023-05-29 13:41:07.000000 prophecy-libs-1.5.6.dev0/prophecy/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1585 2023-05-29 13:41:07.000000 prophecy-libs-1.5.6.dev0/prophecy/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6515 2023-05-29 13:41:07.000000 prophecy-libs-1.5.6.dev0/prophecy/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6393 2023-05-29 13:41:07.000000 prophecy-libs-1.5.6.dev0/prophecy/transpiler/fixed_file_schema.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.245495 prophecy-libs-1.5.6.dev0/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.6.dev0/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.6.dev0/prophecy/udfs/scala_udf_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    16532 2023-05-26 15:20:32.000000 prophecy-libs-1.5.6.dev0/prophecy/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-06-22 20:09:58.249495 prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      318 2023-06-22 20:09:58.000000 prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      992 2023-06-22 20:09:58.000000 prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-06-22 20:09:58.000000 prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-06-22 20:09:58.000000 prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-06-22 20:09:58.000000 prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-06-22 20:09:58.249495 prophecy-libs-1.5.6.dev0/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      479 2023-06-22 20:09:57.000000 prophecy-libs-1.5.6.dev0/setup.py
```

### Comparing `prophecy-libs-1.5.5/prophecy/config/config_base.py` & `prophecy-libs-1.5.6.dev0/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/config/utils.py` & `prophecy-libs-1.5.6.dev0/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.5.6.dev0/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/random_data_creator.py` & `prophecy-libs-1.5.6.dev0/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.5.6.dev0/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/test/base_test_case.py` & `prophecy-libs-1.5.6.dev0/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/test/utils.py` & `prophecy-libs-1.5.6.dev0/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/transpiler/abi_base.py` & `prophecy-libs-1.5.6.dev0/prophecy/transpiler/abi_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/transpiler/abi_core_fcns.py` & `prophecy-libs-1.5.6.dev0/prophecy/transpiler/abi_core_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/transpiler/abi_fcn_wrapper.py` & `prophecy-libs-1.5.6.dev0/prophecy/transpiler/abi_fcn_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/transpiler/dataframe_fcns.py` & `prophecy-libs-1.5.6.dev0/prophecy/transpiler/dataframe_fcns.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/transpiler/fixed_file_schema.py` & `prophecy-libs-1.5.6.dev0/prophecy/transpiler/fixed_file_schema.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.5.6.dev0/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.5.6.dev0/prophecy/udfs/scala_udf_wrapper.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy/utils.py` & `prophecy-libs-1.5.6.dev0/prophecy/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.5/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.5.6.dev0/prophecy_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

