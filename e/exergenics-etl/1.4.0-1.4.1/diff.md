# Comparing `tmp/exergenics-etl-1.4.0.tar.gz` & `tmp/exergenics-etl-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.4.0.tar", last modified: Thu Jun 22 00:06:35 2023, max compression
+gzip compressed data, was "exergenics-etl-1.4.1.tar", last modified: Thu Jun 22 02:24:32 2023, max compression
```

## Comparing `exergenics-etl-1.4.0.tar` & `exergenics-etl-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54195 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    39213 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-22 00:06:29.000000 exergenics-etl-1.4.0/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:06:35.401674 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 00:06:35.000000 exergenics-etl-1.4.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:06:35.405675 exergenics-etl-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-22 00:06:33.000000 exergenics-etl-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:32.164073 exergenics-etl-1.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 02:24:32.164073 exergenics-etl-1.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:32.160072 exergenics-etl-1.4.1/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:32.160072 exergenics-etl-1.4.1/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:32.160072 exergenics-etl-1.4.1/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54195 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:32.160072 exergenics-etl-1.4.1/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39213 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-22 02:24:29.000000 exergenics-etl-1.4.1/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:24:32.160072 exergenics-etl-1.4.1/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 02:24:32.000000 exergenics-etl-1.4.1/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-22 02:24:32.000000 exergenics-etl-1.4.1/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:24:32.000000 exergenics-etl-1.4.1/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 02:24:32.000000 exergenics-etl-1.4.1/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 02:24:32.000000 exergenics-etl-1.4.1/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:24:32.164073 exergenics-etl-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-22 02:24:31.000000 exergenics-etl-1.4.1/setup.py
```

### Comparing `exergenics-etl-1.4.0/LICENSE` & `exergenics-etl-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.4.0/app/exergenics_etl/__init__.py` & `exergenics-etl-1.4.1/app/exergenics_etl/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     generate_CSV_name,
     strftime_for_NaT,
     generate_one_manifest_row,
     generate_output_file_path,
     get_file_name_list,
     SkipRowsMachine,
     InputValidation,
+    find_timestamp_columns,
     calculate_time_interval,
     DatetimeParser,
     transform_columns_to_long_dataframes,
     get_point_summary,
     get_statistical_summary,
     merge_long_dataframes,
     merge_wide_dataframes,
```

### Comparing `exergenics-etl-1.4.0/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.4.1/app/exergenics_etl/src/exergenics_etl.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.4.0/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.4.1/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.4.0/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.4.1/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.4.0/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.4.1/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.4.0/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.4.1/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.4.0/setup.py` & `exergenics-etl-1.4.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.4.0",
+    version="v1.4.1",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

