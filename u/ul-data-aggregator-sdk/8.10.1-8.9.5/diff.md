# Comparing `tmp/ul-data-aggregator-sdk-8.10.1.tar.gz` & `tmp/ul-data-aggregator-sdk-8.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-aggregator-sdk-8.10.1.tar", last modified: Thu Jun 22 14:32:00 2023, max compression
+gzip compressed data, was "ul-data-aggregator-sdk-8.9.5.tar", last modified: Thu Jun 22 13:30:39 2023, max compression
```

## Comparing `ul-data-aggregator-sdk-8.10.1.tar` & `ul-data-aggregator-sdk-8.9.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.564037 ul-data-aggregator-sdk-8.10.1/
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-22 14:32:00.564037 ul-data-aggregator-sdk-8.10.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-13 09:34:59.000000 ul-data-aggregator-sdk-8.10.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.532035 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.532035 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/__tests__/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/__tests__/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-21 09:12:57.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/__tests__/test_integration_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.532035 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/brokers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/brokers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.540036 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     3777 2023-04-10 10:59:35.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/clock_timezones.py
--rw-rw-rw-   0 root         (0) root         (0)    17477 2023-06-16 07:41:25.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/enums.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/names.py
--rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-05 17:07:26.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/dag.yml
--rw-rw-rw-   0 root         (0) root         (0)    66991 2023-06-22 14:31:53.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/data_aggregator_api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-06-22 14:31:53.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/data_aggregator_api_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/data_aggregator_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/data_aggregator_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 09:11:15.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    26940 2023-06-22 14:31:53.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/integration_message.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/lib.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-25 10:42:53.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/runtime_conf.py
--rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/self_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.544036 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3194 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/types/device.py
--rw-rw-rw-   0 root         (0) root         (0)     3398 2023-06-08 09:55:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.556036 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/devices_info_box_to_json.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/internal_api_error_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2022-11-08 19:19:34.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/internal_api_error_handler_old.py
--rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/query_params.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-21 13:15:25.000000 ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/round_dt.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:32:00.564037 ul-data-aggregator-sdk-8.10.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1235 2023-06-22 14:21:57.000000 ul-data-aggregator-sdk-8.10.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:32:00.564037 ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1604 2023-06-22 14:32:00.000000 ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-22 14:32:00.000000 ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:32:00.000000 ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       95 2023-06-22 14:32:00.000000 ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 14:32:00.000000 ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2022-01-13 09:34:59.000000 ul-data-aggregator-sdk-8.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2023-04-21 09:12:57.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/test_integration_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.042590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/brokers/data_aggregator_input_broker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.046590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     3777 2023-04-10 10:59:35.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/clock_timezones.py
+-rw-rw-rw-   0 root         (0) root         (0)    17477 2023-06-16 07:41:25.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/names.py
+-rw-rw-rw-   0 root         (0) root         (0)      675 2022-08-05 17:07:26.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/dag.yml
+-rw-rw-rw-   0 root         (0) root         (0)    50635 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_api_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      826 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2022-08-17 09:11:15.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    26718 2023-06-22 13:20:40.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/integration_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-25 10:42:53.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      152 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/runtime_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      169 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/self_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.046590 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3194 2023-03-10 11:33:05.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/device.py
+-rw-rw-rw-   0 root         (0) root         (0)     3398 2023-06-08 09:55:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/get_data_gateway_network_device_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.050591 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2022-07-04 09:50:06.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/devices_info_box_to_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2022-10-12 09:48:20.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2022-11-08 19:19:34.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler_old.py
+-rw-rw-rw-   0 root         (0) root         (0)      685 2022-08-03 16:22:52.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/query_params.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-21 13:15:25.000000 ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/round_dt.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2023-06-22 13:26:15.000000 ul-data-aggregator-sdk-8.9.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 13:30:39.054591 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1603 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       95 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 13:30:38.000000 ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-aggregator-sdk-8.10.1/PKG-INFO` & `ul-data-aggregator-sdk-8.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 8.10.1
+Version: 8.9.5
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-8.10.1/README.md` & `ul-data-aggregator-sdk-8.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/__init__.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/__tests__/test_integration_message.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/__tests__/test_integration_message.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/clock_timezones.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/clock_timezones.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/constants/enums.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/constants/enums.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/dag.yml` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/dag.yml`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/data_aggregator_sdk.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/data_aggregator_sdk.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/errors.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/integration_message.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/integration_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from datetime import datetime
 from enum import Enum, IntEnum, unique
-from ipaddress import IPv4Address
 from typing import Optional, List, Tuple, Dict, Any
 
 from api_utils.errors import ValidateApiError
 from pydantic import BaseModel, UUID4, root_validator, Field  # pylint: disable=no-name-in-module
 from unipipeline.message.uni_message import UniMessage
 
 from data_aggregator_sdk.types.device import NetworkSysTypeEnum
@@ -657,19 +656,14 @@
         description="Sender software / hardware version",
     )
     note: str = Field(
         ...,
         title="Note about sender",
         description="Any usefull information about sender",
     )
-    ipv4: IPv4Address = Field(
-        ...,
-        title='IPv4 sender address',
-        description="A unique numerical identifier for every sender that send through the internet",
-    )
 
 
 class IntegrationV0MessageMeta(BaseModel):
     nbfi_bs0: Optional[IntegrationV0MessageMetaNbFiBS0] = Field(
         None,
         title="NBFi BS0 meta message structure",
         description="NBFi BS0 meta message structure",
```

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/types/device.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/device.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/types/get_data_gateway_network_device_list.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/types/get_data_gateway_network_device_list.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/internal_api_error_handler.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/internal_api_error_handler_old.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/internal_api_error_handler_old.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/data_aggregator_sdk/utils/query_params.py` & `ul-data-aggregator-sdk-8.9.5/data_aggregator_sdk/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `ul-data-aggregator-sdk-8.10.1/setup.py` & `ul-data-aggregator-sdk-8.9.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='ul-data-aggregator-sdk',
-    version='8.10.1',
+    version='8.9.5',
     description='Data aggregator sdk',
     author='Unic-lab',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_data={
         '': ['*.yml'],
         'data_aggregator_sdk': ['py.typed'],
```

### Comparing `ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/PKG-INFO` & `ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-aggregator-sdk
-Version: 8.10.1
+Version: 8.9.5
 Summary: Data aggregator sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-aggregator-sdk-8.10.1/ul_data_aggregator_sdk.egg-info/SOURCES.txt` & `ul-data-aggregator-sdk-8.9.5/ul_data_aggregator_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

