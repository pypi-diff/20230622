# Comparing `tmp/ul-data-logger-api-sdk-1.3.3.tar.gz` & `tmp/ul-data-logger-api-sdk-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-logger-api-sdk-1.3.3.tar", last modified: Thu Jun 22 14:10:52 2023, max compression
+gzip compressed data, was "ul-data-logger-api-sdk-1.3.4.tar", last modified: Thu Jun 22 15:25:48 2023, max compression
```

## Comparing `ul-data-logger-api-sdk-1.3.3.tar` & `ul-data-logger-api-sdk-1.3.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:10:52.446937 ul-data-logger-api-sdk-1.3.3/
--rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 14:10:52.442937 ul-data-logger-api-sdk-1.3.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      344 2022-08-07 11:32:24.000000 ul-data-logger-api-sdk-1.3.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:10:52.430936 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 07:42:50.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2023-06-19 08:03:42.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/data_logger_api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-03 07:16:28.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/data_logger_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 07:16:28.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:10:52.442937 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-30 07:42:50.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-06-16 11:14:49.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/types/api_device_data_history.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-16 11:14:49.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/types/api_packet_types.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-19 15:55:15.000000 ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/types/api_protocol_types.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:10:52.446937 ul-data-logger-api-sdk-1.3.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3156 2023-06-22 14:10:45.000000 ul-data-logger-api-sdk-1.3.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:10:52.442937 ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 14:10:52.000000 ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-22 14:10:52.000000 ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:10:52.000000 ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-06-22 14:10:52.000000 ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 14:10:52.000000 ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      344 2022-05-25 10:25:14.000000 ul-data-logger-api-sdk-1.3.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.537928 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2023-06-19 08:03:41.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/data_logger_api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/data_logger_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2023-06-19 08:03:41.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_device_data_history.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-19 08:03:41.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_packet_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-18 07:23:08.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_protocol_types.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2023-06-22 15:17:43.000000 ul-data-logger-api-sdk-1.3.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-logger-api-sdk-1.3.3/PKG-INFO` & `ul-data-logger-api-sdk-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-logger-api-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: Data logger API sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/data_logger_api_sdk.py` & `ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/data_logger_api_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-data-logger-api-sdk-1.3.3/data_logger_api_sdk/types/api_device_data_history.py` & `ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_device_data_history.py`

 * *Files identical despite different names*

### Comparing `ul-data-logger-api-sdk-1.3.3/setup.py` & `ul-data-logger-api-sdk-1.3.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,26 +33,26 @@
                 "Programming Language :: Python :: 3.8",
                 "Programming Language :: Python :: 3.9",
                 "Operating System :: OS Independent",
             ],
             platforms='any',
             install_requires=[
                 "unipipeline>=1.4.5",
-                # "ul-data-aggregator-sdk==8.9.5",
+                # "ul-data-aggregator-sdk==8.10.2,
                 # "ul-py-tool==1.15.20",
                 # "ul-db-utils==2.10.7",
-                # "ul-api-utils==7.2.7",
+                # "ul-api-utils==7.2.8",
                 # "ul-data-gateway-sdk==0.4.5",
             ],
         )
     elif 'api_sdk' in set(sys.argv):
         sys.argv.remove("api_sdk")
         setup(
             name='ul-data-logger-api-sdk',
-            version='1.3.3',
+            version='1.3.4',
             description='Data logger API sdk',
             author='Unic-lab',
             long_description=long_description,
             long_description_content_type="text/markdown",
             packages=find_packages(include=['data_logger_api_sdk*']),
             include_package_data=True,
             package_data={
@@ -69,15 +69,14 @@
                 "Programming Language :: Python :: 3.8",
                 "Programming Language :: Python :: 3.9",
                 "Operating System :: OS Independent",
             ],
             platforms='any',
             install_requires=[
                 "unipipeline>=1.4.5",
-                "ul-data-aggregator-sdk>=8.9.5",
-                # "ul-data-aggregator-sdk==8.9.5",
+                "ul-data-aggregator-sdk>=8.10.2",
+                # "ul-data-aggregator-sdk==8.10.2,
                 # "ul-py-tool==1.15.20",
-                # "ul-db-utils==2.10.7",
-                # "ul-api-utils==7.2.7",
+                # "ul-api-utils==7.2.8",
                 # "ul-data-gateway-sdk==0.4.5",
             ],
         )
```

### Comparing `ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/PKG-INFO` & `ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-logger-api-sdk
-Version: 1.3.3
+Version: 1.3.4
 Summary: Data logger API sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-logger-api-sdk-1.3.3/ul_data_logger_api_sdk.egg-info/SOURCES.txt` & `ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

