# Comparing `tmp/ul-data-logger-api-sdk-1.3.4.tar.gz` & `tmp/ul-data-logger-api-sdk-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ul-data-logger-api-sdk-1.3.4.tar", last modified: Thu Jun 22 15:25:48 2023, max compression
+gzip compressed data, was "ul-data-logger-api-sdk-1.3.5.tar", last modified: Thu Jun 22 16:39:29 2023, max compression
```

## Comparing `ul-data-logger-api-sdk-1.3.4.tar` & `ul-data-logger-api-sdk-1.3.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/
--rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      344 2022-05-25 10:25:14.000000 ul-data-logger-api-sdk-1.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.537928 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2023-06-19 08:03:41.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/data_logger_api_sdk.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/data_logger_sdk_config.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2023-06-19 08:03:41.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_device_data_history.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-06-19 08:03:41.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_packet_types.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-05-18 07:23:08.000000 ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_protocol_types.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3116 2023-06-22 15:17:43.000000 ul-data-logger-api-sdk-1.3.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 15:25:48.541928 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      582 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 15:25:48.000000 ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:39:29.120690 ul-data-logger-api-sdk-1.3.5/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 16:39:29.120690 ul-data-logger-api-sdk-1.3.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      344 2022-05-23 17:20:18.000000 ul-data-logger-api-sdk-1.3.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:39:29.112690 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3078 2023-06-22 15:54:39.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/data_logger_api_sdk.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/data_logger_sdk_config.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:39:29.120690 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/types/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-10 08:23:01.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/types/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1200 2023-06-22 15:54:39.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/types/api_device_data_history.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-06-22 15:54:39.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/types/api_packet_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-06-22 15:54:39.000000 ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/types/api_protocol_types.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 16:39:29.120690 ul-data-logger-api-sdk-1.3.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3116 2023-06-22 16:38:04.000000 ul-data-logger-api-sdk-1.3.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:39:29.120690 ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      909 2023-06-22 16:39:28.000000 ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-22 16:39:28.000000 ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:39:28.000000 ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 16:39:28.000000 ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-22 16:39:28.000000 ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/top_level.txt
```

### Comparing `ul-data-logger-api-sdk-1.3.4/PKG-INFO` & `ul-data-logger-api-sdk-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-logger-api-sdk
-Version: 1.3.4
+Version: 1.3.5
 Summary: Data logger API sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/data_logger_api_sdk.py` & `ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/data_logger_api_sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import time
 from datetime import datetime
 from functools import lru_cache
 from typing import List, Type, Optional
 
-from api_utils.internal_api.internal_api import InternalApi
-from api_utils.internal_api.internal_api_response import TPyloadType
-from api_utils.utils.api_method import ApiMethod
+from ul_api_utils.internal_api.internal_api import InternalApi
+from ul_api_utils.internal_api.internal_api_response import TPyloadType
+from ul_api_utils.utils.api_method import ApiMethod
 
 from data_logger_api_sdk.types.api_device_data_history import ApiDeviceDataHistoryResponse, ApiDeviceDataHistoryBody
 from data_logger_api_sdk.types.api_packet_types import ApiPacketTypesListResponse
 from data_logger_api_sdk.types.api_protocol_types import ApiProtocolTypesListResponse
 from data_logger_api_sdk.data_logger_sdk_config import DataLoggerApiSdkConfig
```

### Comparing `ul-data-logger-api-sdk-1.3.4/data_logger_api_sdk/types/api_device_data_history.py` & `ul-data-logger-api-sdk-1.3.5/data_logger_api_sdk/types/api_device_data_history.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from typing import Optional
 from uuid import UUID
 
-from api_utils.api_resource.api_response import JsonApiResponsePayload
+from ul_api_utils.api_resource.api_response import JsonApiResponsePayload
 from data_aggregator_sdk.integration_message import IntegrationV0MessageMeta
 from pydantic import BaseModel, validator
 
 
 class ApiDeviceDataHistoryBody(BaseModel):
     period_from: datetime
     period_to: datetime
```

### Comparing `ul-data-logger-api-sdk-1.3.4/setup.py` & `ul-data-logger-api-sdk-1.3.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
                 # "ul-data-gateway-sdk==0.4.5",
             ],
         )
     elif 'api_sdk' in set(sys.argv):
         sys.argv.remove("api_sdk")
         setup(
             name='ul-data-logger-api-sdk',
-            version='1.3.4',
+            version='1.3.5',
             description='Data logger API sdk',
             author='Unic-lab',
             long_description=long_description,
             long_description_content_type="text/markdown",
             packages=find_packages(include=['data_logger_api_sdk*']),
             include_package_data=True,
             package_data={
```

### Comparing `ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/PKG-INFO` & `ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ul-data-logger-api-sdk
-Version: 1.3.4
+Version: 1.3.5
 Summary: Data logger API sdk
 Author: Unic-lab
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `ul-data-logger-api-sdk-1.3.4/ul_data_logger_api_sdk.egg-info/SOURCES.txt` & `ul-data-logger-api-sdk-1.3.5/ul_data_logger_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

