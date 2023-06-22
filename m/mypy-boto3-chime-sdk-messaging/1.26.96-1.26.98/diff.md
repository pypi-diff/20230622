# Comparing `tmp/mypy-boto3-chime-sdk-messaging-1.26.96.tar.gz` & `tmp/mypy-boto3-chime-sdk-messaging-1.26.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.26.96.tar", last modified: Tue Mar 21 19:19:40 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-messaging-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-messaging-1.26.96.tar` & `mypy-boto3-chime-sdk-messaging-1.26.98.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.917032 mypy-boto3-chime-sdk-messaging-1.26.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18168 2023-03-21 19:19:40.917032 mypy-boto3-chime-sdk-messaging-1.26.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.889032 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37174 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37118 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    46572 2023-03-21 19:18:31.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46513 2023-03-21 19:18:31.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 19:19:40.917032 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18168 2023-03-21 19:19:40.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-21 19:19:40.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 19:19:40.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-21 19:19:40.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-21 19:19:40.000000 mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 19:19:40.917032 mypy-boto3-chime-sdk-messaging-1.26.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-21 19:18:30.000000 mypy-boto3-chime-sdk-messaging-1.26.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16765 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38174 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38117 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-03-23 19:32:02.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    48068 2023-03-23 19:32:03.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48007 2023-03-23 19:32:03.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.423627 mypy-boto3-chime-sdk-messaging-1.26.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-03-23 19:32:01.000000 mypy-boto3-chime-sdk-messaging-1.26.98/setup.py
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/LICENSE` & `mypy-boto3-chime-sdk-messaging-1.26.98/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.26.98/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.26.96
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.26.96 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -285,14 +285,15 @@
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
     ChannelMessageStatusType,
     ChannelMessageTypeType,
     ChannelModeType,
     ChannelPrivacyType,
     ErrorCodeType,
+    ExpirationCriterionType,
     FallbackActionType,
     InvocationTypeType,
     MessagingDataTypeType,
     PushNotificationTypeType,
     SearchFieldKeyType,
     SearchFieldOperatorType,
     SortOrderType,
@@ -325,14 +326,15 @@
     ChannelAssociatedWithFlowSummaryTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
     ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
@@ -401,14 +403,16 @@
     SendChannelMessageRequestRequestTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
+    PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
@@ -450,42 +454,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/README.md` & `mypy-boto3-chime-sdk-messaging-1.26.98/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -253,14 +253,15 @@
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
     ChannelMessageStatusType,
     ChannelMessageTypeType,
     ChannelModeType,
     ChannelPrivacyType,
     ErrorCodeType,
+    ExpirationCriterionType,
     FallbackActionType,
     InvocationTypeType,
     MessagingDataTypeType,
     PushNotificationTypeType,
     SearchFieldKeyType,
     SearchFieldOperatorType,
     SortOrderType,
@@ -293,14 +294,15 @@
     ChannelAssociatedWithFlowSummaryTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
     ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
@@ -369,14 +371,16 @@
     SendChannelMessageRequestRequestTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
+    PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
@@ -418,42 +422,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/__main__.py` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKMessaging 1.26.96\nVersion:         1.26.96\nBuilder"
-        " version: 7.13.0\nDocs:           "
+        "Type annotations for boto3.ChimeSDKMessaging 1.26.98\nVersion:         1.26.98\nBuilder"
+        " version: 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.96")
+    print("1.26.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/client.py` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ElasticChannelConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
+    ExpirationSettingsTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     ListChannelBansResponseTypeDef,
     ListChannelFlowsResponseTypeDef,
@@ -60,14 +61,15 @@
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageAttributeValueTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
+    PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
@@ -135,15 +137,15 @@
         ChannelArn: str,
         MemberArns: Sequence[str],
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
         SubChannelId: str = ...
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
-        Adds a specified number of users to a channel.
+        Adds a specified number of users and bots to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.batch_create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#batch_create_channel_membership)
         """
 
     def can_paginate(self, operation_name: str) -> bool:
         """
@@ -186,15 +188,16 @@
         Mode: ChannelModeType = ...,
         Privacy: ChannelPrivacyType = ...,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ChannelId: str = ...,
         MemberArns: Sequence[str] = ...,
         ModeratorArns: Sequence[str] = ...,
-        ElasticChannelConfiguration: ElasticChannelConfigurationTypeDef = ...
+        ElasticChannelConfiguration: ElasticChannelConfigurationTypeDef = ...,
+        ExpirationSettings: ExpirationSettingsTypeDef = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel)
         """
@@ -231,15 +234,15 @@
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
         ChimeBearer: str,
         SubChannelId: str = ...
     ) -> CreateChannelMembershipResponseTypeDef:
         """
-        Adds a user to a channel.
+        Adds a member to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_membership)
         """
 
     def create_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
@@ -262,15 +265,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel)
         """
 
     def delete_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Removes a user from a channel's ban list.
+        Removes a member from a channel's ban list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_ban)
         """
 
     def delete_channel_flow(self, *, ChannelFlowArn: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -320,15 +323,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_messaging_streaming_configurations)
         """
 
     def describe_channel(
         self, *, ChannelArn: str, ChimeBearer: str
     ) -> DescribeChannelResponseTypeDef:
         """
-        Returns the full details of a channel in an Amazon Chime `AppInstance` .
+        Returns the full details of a channel in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel)
         """
 
     def describe_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
@@ -359,26 +362,26 @@
         """
 
     def describe_channel_membership_for_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:
         """
         Returns the details of a channel based on the membership of the specified
-        `AppInstanceUser` .
+        `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_membership_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_membership_for_app_instance_user)
         """
 
     def describe_channel_moderated_by_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:
         """
         Returns the full details of a channel moderated by the specified
-        `AppInstanceUser` .
+        `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_moderated_by_app_instance_user)
         """
 
     def describe_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
@@ -414,16 +417,16 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#generate_presigned_url)
         """
 
     def get_channel_membership_preferences(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> GetChannelMembershipPreferencesResponseTypeDef:
         """
-        Gets the membership preferences of an `AppInstanceUser` for the specified
-        channel.
+        Gets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
+        the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_membership_preferences)
         """
 
     def get_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
@@ -463,15 +466,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_messaging_streaming_configurations)
         """
 
     def list_channel_bans(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelBansResponseTypeDef:
         """
-        Lists all the users banned from a particular channel.
+        Lists all the users and bots banned from a particular channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_bans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_bans)
         """
 
     def list_channel_flows(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
@@ -505,15 +508,15 @@
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
-        Lists all channels that a particular `AppInstanceUser` is a part of.
+        Lists all channels that anr `AppInstanceUser` or `AppInstanceBot` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_memberships_for_app_instance_user)
         """
 
     def list_channel_messages(
         self,
@@ -575,15 +578,15 @@
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
-        A list of the channels moderated by an `AppInstanceUser` .
+        A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels_moderated_by_app_instance_user)
         """
 
     def list_sub_channels(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
@@ -599,25 +602,39 @@
         """
         Lists the tags applied to an Amazon Chime SDK messaging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_tags_for_resource)
         """
 
+    def put_channel_expiration_settings(
+        self,
+        *,
+        ChannelArn: str,
+        ChimeBearer: str = ...,
+        ExpirationSettings: ExpirationSettingsTypeDef = ...
+    ) -> PutChannelExpirationSettingsResponseTypeDef:
+        """
+        Sets the number of days before the channel is automatically deleted.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_expiration_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_expiration_settings)
+        """
+
     def put_channel_membership_preferences(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         ChimeBearer: str,
         Preferences: ChannelMembershipPreferencesTypeDef
     ) -> PutChannelMembershipPreferencesResponseTypeDef:
         """
-        Sets the membership preferences of an `AppInstanceUser` for the specified
-        channel.
+        Sets the membership preferences of an `AppInstanceUser` or `AppIntanceBot` for
+        the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_membership_preferences)
         """
 
     def put_messaging_streaming_configurations(
         self,
@@ -647,15 +664,15 @@
         *,
         Fields: Sequence[SearchFieldTypeDef],
         ChimeBearer: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SearchChannelsResponseTypeDef:
         """
-        Allows `ChimeBearer` to search channels by channel members.
+        Allows the `ChimeBearer` to search channels by channel members.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.search_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#search_channels)
         """
 
     def send_channel_message(
         self,
@@ -665,15 +682,16 @@
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
+        ContentType: str = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.send_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#send_channel_message)
         """
@@ -726,18 +744,19 @@
         """
 
     def update_channel_message(
         self,
         *,
         ChannelArn: str,
         MessageId: str,
+        Content: str,
         ChimeBearer: str,
-        Content: str = ...,
         Metadata: str = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
+        ContentType: str = ...
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_message)
         """
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/client.pyi` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     ElasticChannelConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
+    ExpirationSettingsTypeDef,
     GetChannelMembershipPreferencesResponseTypeDef,
     GetChannelMessageResponseTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     ListChannelBansResponseTypeDef,
     ListChannelFlowsResponseTypeDef,
@@ -60,14 +61,15 @@
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageAttributeValueTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
+    PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
     SearchFieldTypeDef,
     SendChannelMessageResponseTypeDef,
     StreamingConfigurationTypeDef,
@@ -130,15 +132,15 @@
         ChannelArn: str,
         MemberArns: Sequence[str],
         ChimeBearer: str,
         Type: ChannelMembershipTypeType = ...,
         SubChannelId: str = ...
     ) -> BatchCreateChannelMembershipResponseTypeDef:
         """
-        Adds a specified number of users to a channel.
+        Adds a specified number of users and bots to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.batch_create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#batch_create_channel_membership)
         """
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
@@ -177,15 +179,16 @@
         Mode: ChannelModeType = ...,
         Privacy: ChannelPrivacyType = ...,
         Metadata: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ChannelId: str = ...,
         MemberArns: Sequence[str] = ...,
         ModeratorArns: Sequence[str] = ...,
-        ElasticChannelConfiguration: ElasticChannelConfigurationTypeDef = ...
+        ElasticChannelConfiguration: ElasticChannelConfigurationTypeDef = ...,
+        ExpirationSettings: ExpirationSettingsTypeDef = ...
     ) -> CreateChannelResponseTypeDef:
         """
         Creates a channel to which you can add users and send messages.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel)
         """
@@ -219,15 +222,15 @@
         ChannelArn: str,
         MemberArn: str,
         Type: ChannelMembershipTypeType,
         ChimeBearer: str,
         SubChannelId: str = ...
     ) -> CreateChannelMembershipResponseTypeDef:
         """
-        Adds a user to a channel.
+        Adds a member to a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.create_channel_membership)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#create_channel_membership)
         """
     def create_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> CreateChannelModeratorResponseTypeDef:
@@ -247,15 +250,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel)
         """
     def delete_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> EmptyResponseMetadataTypeDef:
         """
-        Removes a user from a channel's ban list.
+        Removes a member from a channel's ban list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_channel_ban)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_channel_ban)
         """
     def delete_channel_flow(self, *, ChannelFlowArn: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a channel flow, an irreversible process.
@@ -299,15 +302,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.delete_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#delete_messaging_streaming_configurations)
         """
     def describe_channel(
         self, *, ChannelArn: str, ChimeBearer: str
     ) -> DescribeChannelResponseTypeDef:
         """
-        Returns the full details of a channel in an Amazon Chime `AppInstance` .
+        Returns the full details of a channel in an Amazon Chime `AppInstance`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel)
         """
     def describe_channel_ban(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> DescribeChannelBanResponseTypeDef:
@@ -334,25 +337,25 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_membership)
         """
     def describe_channel_membership_for_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelMembershipForAppInstanceUserResponseTypeDef:
         """
         Returns the details of a channel based on the membership of the specified
-        `AppInstanceUser` .
+        `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_membership_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_membership_for_app_instance_user)
         """
     def describe_channel_moderated_by_app_instance_user(
         self, *, ChannelArn: str, AppInstanceUserArn: str, ChimeBearer: str
     ) -> DescribeChannelModeratedByAppInstanceUserResponseTypeDef:
         """
         Returns the full details of a channel moderated by the specified
-        `AppInstanceUser` .
+        `AppInstanceUser` or `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.describe_channel_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#describe_channel_moderated_by_app_instance_user)
         """
     def describe_channel_moderator(
         self, *, ChannelArn: str, ChannelModeratorArn: str, ChimeBearer: str
     ) -> DescribeChannelModeratorResponseTypeDef:
@@ -384,16 +387,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.generate_presigned_url)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#generate_presigned_url)
         """
     def get_channel_membership_preferences(
         self, *, ChannelArn: str, MemberArn: str, ChimeBearer: str
     ) -> GetChannelMembershipPreferencesResponseTypeDef:
         """
-        Gets the membership preferences of an `AppInstanceUser` for the specified
-        channel.
+        Gets the membership preferences of an `AppInstanceUser` or `AppInstanceBot` for
+        the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_channel_membership_preferences)
         """
     def get_channel_message(
         self, *, ChannelArn: str, MessageId: str, ChimeBearer: str, SubChannelId: str = ...
     ) -> GetChannelMessageResponseTypeDef:
@@ -428,15 +431,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.get_messaging_streaming_configurations)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#get_messaging_streaming_configurations)
         """
     def list_channel_bans(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelBansResponseTypeDef:
         """
-        Lists all the users banned from a particular channel.
+        Lists all the users and bots banned from a particular channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_bans)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_bans)
         """
     def list_channel_flows(
         self, *, AppInstanceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChannelFlowsResponseTypeDef:
@@ -467,15 +470,15 @@
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelMembershipsForAppInstanceUserResponseTypeDef:
         """
-        Lists all channels that a particular `AppInstanceUser` is a part of.
+        Lists all channels that anr `AppInstanceUser` or `AppInstanceBot` is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channel_memberships_for_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channel_memberships_for_app_instance_user)
         """
     def list_channel_messages(
         self,
         *,
@@ -532,15 +535,15 @@
         *,
         ChimeBearer: str,
         AppInstanceUserArn: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListChannelsModeratedByAppInstanceUserResponseTypeDef:
         """
-        A list of the channels moderated by an `AppInstanceUser` .
+        A list of the channels moderated by an `AppInstanceUser`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_channels_moderated_by_app_instance_user)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_channels_moderated_by_app_instance_user)
         """
     def list_sub_channels(
         self, *, ChannelArn: str, ChimeBearer: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListSubChannelsResponseTypeDef:
@@ -553,25 +556,38 @@
     def list_tags_for_resource(self, *, ResourceARN: str) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags applied to an Amazon Chime SDK messaging resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#list_tags_for_resource)
         """
+    def put_channel_expiration_settings(
+        self,
+        *,
+        ChannelArn: str,
+        ChimeBearer: str = ...,
+        ExpirationSettings: ExpirationSettingsTypeDef = ...
+    ) -> PutChannelExpirationSettingsResponseTypeDef:
+        """
+        Sets the number of days before the channel is automatically deleted.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_expiration_settings)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_expiration_settings)
+        """
     def put_channel_membership_preferences(
         self,
         *,
         ChannelArn: str,
         MemberArn: str,
         ChimeBearer: str,
         Preferences: ChannelMembershipPreferencesTypeDef
     ) -> PutChannelMembershipPreferencesResponseTypeDef:
         """
-        Sets the membership preferences of an `AppInstanceUser` for the specified
-        channel.
+        Sets the membership preferences of an `AppInstanceUser` or `AppIntanceBot` for
+        the specified channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.put_channel_membership_preferences)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#put_channel_membership_preferences)
         """
     def put_messaging_streaming_configurations(
         self,
         *,
@@ -598,15 +614,15 @@
         *,
         Fields: Sequence[SearchFieldTypeDef],
         ChimeBearer: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> SearchChannelsResponseTypeDef:
         """
-        Allows `ChimeBearer` to search channels by channel members.
+        Allows the `ChimeBearer` to search channels by channel members.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.search_channels)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#search_channels)
         """
     def send_channel_message(
         self,
         *,
@@ -615,15 +631,16 @@
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
         MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
+        ContentType: str = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.send_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#send_channel_message)
         """
@@ -671,18 +688,19 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_flow)
         """
     def update_channel_message(
         self,
         *,
         ChannelArn: str,
         MessageId: str,
+        Content: str,
         ChimeBearer: str,
-        Content: str = ...,
         Metadata: str = ...,
-        SubChannelId: str = ...
+        SubChannelId: str = ...,
+        ContentType: str = ...
     ) -> UpdateChannelMessageResponseTypeDef:
         """
         Updates the content of a message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging.Client.update_channel_message)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/client/#update_channel_message)
         """
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/literals.py` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "ChannelMembershipTypeType",
     "ChannelMessagePersistenceTypeType",
     "ChannelMessageStatusType",
     "ChannelMessageTypeType",
     "ChannelModeType",
     "ChannelPrivacyType",
     "ErrorCodeType",
+    "ExpirationCriterionType",
     "FallbackActionType",
     "InvocationTypeType",
     "MessagingDataTypeType",
     "PushNotificationTypeType",
     "SearchFieldKeyType",
     "SearchFieldOperatorType",
     "SortOrderType",
@@ -62,14 +63,15 @@
     "ServiceUnavailable",
     "Throttled",
     "Throttling",
     "Unauthorized",
     "Unprocessable",
     "VoiceConnectorGroupAssociationsExist",
 ]
+ExpirationCriterionType = Literal["CREATED_TIMESTAMP", "LAST_MESSAGE_TIMESTAMP"]
 FallbackActionType = Literal["ABORT", "CONTINUE"]
 InvocationTypeType = Literal["ASYNC"]
 MessagingDataTypeType = Literal["Channel", "ChannelMessage"]
 PushNotificationTypeType = Literal["DEFAULT", "VOIP"]
 SearchFieldKeyType = Literal["MEMBERS"]
 SearchFieldOperatorType = Literal["EQUALS", "INCLUDES"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
@@ -237,14 +239,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/literals.pyi` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     "ChannelMembershipTypeType",
     "ChannelMessagePersistenceTypeType",
     "ChannelMessageStatusType",
     "ChannelMessageTypeType",
     "ChannelModeType",
     "ChannelPrivacyType",
     "ErrorCodeType",
+    "ExpirationCriterionType",
     "FallbackActionType",
     "InvocationTypeType",
     "MessagingDataTypeType",
     "PushNotificationTypeType",
     "SearchFieldKeyType",
     "SearchFieldOperatorType",
     "SortOrderType",
@@ -60,14 +61,15 @@
     "ServiceUnavailable",
     "Throttled",
     "Throttling",
     "Unauthorized",
     "Unprocessable",
     "VoiceConnectorGroupAssociationsExist",
 ]
+ExpirationCriterionType = Literal["CREATED_TIMESTAMP", "LAST_MESSAGE_TIMESTAMP"]
 FallbackActionType = Literal["ABORT", "CONTINUE"]
 InvocationTypeType = Literal["ASYNC"]
 MessagingDataTypeType = Literal["Channel", "ChannelMessage"]
 PushNotificationTypeType = Literal["DEFAULT", "VOIP"]
 SearchFieldKeyType = Literal["MEMBERS"]
 SearchFieldOperatorType = Literal["EQUALS", "INCLUDES"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
@@ -235,14 +237,15 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/type_defs.py` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
     ChannelMessageStatusType,
     ChannelMessageTypeType,
     ChannelModeType,
     ChannelPrivacyType,
     ErrorCodeType,
+    ExpirationCriterionType,
     FallbackActionType,
     MessagingDataTypeType,
     PushNotificationTypeType,
     SearchFieldOperatorType,
     SortOrderType,
 )
 
@@ -51,14 +52,15 @@
     "ChannelAssociatedWithFlowSummaryTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
     "ElasticChannelConfigurationTypeDef",
+    "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
@@ -127,14 +129,16 @@
     "SendChannelMessageRequestRequestTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "ChannelTypeDef",
+    "PutChannelExpirationSettingsRequestRequestTypeDef",
+    "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
@@ -320,14 +324,22 @@
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
 )
 
+ExpirationSettingsTypeDef = TypedDict(
+    "ExpirationSettingsTypeDef",
+    {
+        "ExpirationDays": int,
+        "ExpirationCriterion": ExpirationCriterionType,
+    },
+)
+
 CreateChannelBanRequestRequestTypeDef = TypedDict(
     "CreateChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -947,23 +959,24 @@
 )
 
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
+        "Content": str,
         "ChimeBearer": str,
     },
 )
 _OptionalUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelMessageRequestRequestTypeDef",
     {
-        "Content": str,
         "Metadata": str,
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
@@ -1248,14 +1261,15 @@
     "_OptionalChannelMessageCallbackTypeDef",
     {
         "Content": str,
         "Metadata": str,
         "PushNotification": PushNotificationConfigurationTypeDef,
         "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 
 class ChannelMessageCallbackTypeDef(
     _RequiredChannelMessageCallbackTypeDef, _OptionalChannelMessageCallbackTypeDef
@@ -1277,14 +1291,15 @@
 _OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendChannelMessageRequestRequestTypeDef",
     {
         "Metadata": str,
         "PushNotification": PushNotificationConfigurationTypeDef,
         "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
@@ -1303,14 +1318,15 @@
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "ContentType": str,
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1324,14 +1340,15 @@
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
@@ -1372,18 +1389,51 @@
         "Metadata": str,
         "CreatedBy": IdentityTypeDef,
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ChannelFlowArn": str,
         "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
+_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+    },
+)
+_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
+    {
+        "ChimeBearer": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+    },
+    total=False,
+)
+
+
+class PutChannelExpirationSettingsRequestRequestTypeDef(
+    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
+    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
+):
+    pass
+
+
+PutChannelExpirationSettingsResponseTypeDef = TypedDict(
+    "PutChannelExpirationSettingsResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "ClientRequestToken": str,
         "ChimeBearer": str,
@@ -1396,14 +1446,15 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "Tags": Sequence[TagTypeDef],
         "ChannelId": str,
         "MemberArns": Sequence[str],
         "ModeratorArns": Sequence[str],
         "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging/type_defs.pyi` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
     ChannelMessageStatusType,
     ChannelMessageTypeType,
     ChannelModeType,
     ChannelPrivacyType,
     ErrorCodeType,
+    ExpirationCriterionType,
     FallbackActionType,
     MessagingDataTypeType,
     PushNotificationTypeType,
     SearchFieldOperatorType,
     SortOrderType,
 )
 
@@ -50,14 +51,15 @@
     "ChannelAssociatedWithFlowSummaryTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
     "ElasticChannelConfigurationTypeDef",
+    "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
     "DeleteChannelBanRequestRequestTypeDef",
     "DeleteChannelFlowRequestRequestTypeDef",
     "DeleteChannelMembershipRequestRequestTypeDef",
@@ -126,14 +128,16 @@
     "SendChannelMessageRequestRequestTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
     "ChannelTypeDef",
+    "PutChannelExpirationSettingsRequestRequestTypeDef",
+    "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
     "GetMessagingStreamingConfigurationsResponseTypeDef",
     "PutMessagingStreamingConfigurationsRequestRequestTypeDef",
     "PutMessagingStreamingConfigurationsResponseTypeDef",
@@ -315,14 +319,22 @@
     {
         "MaximumSubChannels": int,
         "TargetMembershipsPerSubChannel": int,
         "MinimumMembershipPercentage": int,
     },
 )
 
+ExpirationSettingsTypeDef = TypedDict(
+    "ExpirationSettingsTypeDef",
+    {
+        "ExpirationDays": int,
+        "ExpirationCriterion": ExpirationCriterionType,
+    },
+)
+
 CreateChannelBanRequestRequestTypeDef = TypedDict(
     "CreateChannelBanRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MemberArn": str,
         "ChimeBearer": str,
     },
@@ -906,23 +918,24 @@
 )
 
 _RequiredUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
+        "Content": str,
         "ChimeBearer": str,
     },
 )
 _OptionalUpdateChannelMessageRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateChannelMessageRequestRequestTypeDef",
     {
-        "Content": str,
         "Metadata": str,
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 class UpdateChannelMessageRequestRequestTypeDef(
     _RequiredUpdateChannelMessageRequestRequestTypeDef,
     _OptionalUpdateChannelMessageRequestRequestTypeDef,
@@ -1201,14 +1214,15 @@
     "_OptionalChannelMessageCallbackTypeDef",
     {
         "Content": str,
         "Metadata": str,
         "PushNotification": PushNotificationConfigurationTypeDef,
         "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 class ChannelMessageCallbackTypeDef(
     _RequiredChannelMessageCallbackTypeDef, _OptionalChannelMessageCallbackTypeDef
 ):
@@ -1228,14 +1242,15 @@
 _OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
     "_OptionalSendChannelMessageRequestRequestTypeDef",
     {
         "Metadata": str,
         "PushNotification": PushNotificationConfigurationTypeDef,
         "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 class SendChannelMessageRequestRequestTypeDef(
     _RequiredSendChannelMessageRequestRequestTypeDef,
     _OptionalSendChannelMessageRequestRequestTypeDef,
@@ -1252,14 +1267,15 @@
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
+        "ContentType": str,
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
     "ChannelMessageTypeDef",
     {
@@ -1273,14 +1289,15 @@
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
         "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
+        "ContentType": str,
     },
     total=False,
 )
 
 GetChannelMessageStatusResponseTypeDef = TypedDict(
     "GetChannelMessageStatusResponseTypeDef",
     {
@@ -1321,18 +1338,49 @@
         "Metadata": str,
         "CreatedBy": IdentityTypeDef,
         "CreatedTimestamp": datetime,
         "LastMessageTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "ChannelFlowArn": str,
         "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
+_RequiredPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutChannelExpirationSettingsRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+    },
+)
+_OptionalPutChannelExpirationSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutChannelExpirationSettingsRequestRequestTypeDef",
+    {
+        "ChimeBearer": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+    },
+    total=False,
+)
+
+class PutChannelExpirationSettingsRequestRequestTypeDef(
+    _RequiredPutChannelExpirationSettingsRequestRequestTypeDef,
+    _OptionalPutChannelExpirationSettingsRequestRequestTypeDef,
+):
+    pass
+
+PutChannelExpirationSettingsResponseTypeDef = TypedDict(
+    "PutChannelExpirationSettingsResponseTypeDef",
+    {
+        "ChannelArn": str,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateChannelRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "ClientRequestToken": str,
         "ChimeBearer": str,
@@ -1345,14 +1393,15 @@
         "Privacy": ChannelPrivacyType,
         "Metadata": str,
         "Tags": Sequence[TagTypeDef],
         "ChannelId": str,
         "MemberArns": Sequence[str],
         "ModeratorArns": Sequence[str],
         "ElasticChannelConfiguration": ElasticChannelConfigurationTypeDef,
+        "ExpirationSettings": ExpirationSettingsTypeDef,
     },
     total=False,
 )
 
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-messaging
-Version: 1.26.96
-Summary: Type annotations for boto3.ChimeSDKMessaging 1.26.96 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKMessaging 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-messaging.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-messaging)
 [![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-messaging?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-messaging)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKMessaging 1.26.96](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
+[boto3.ChimeSDKMessaging 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-messaging docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/).
 
 See how it helps to find and fix potential bugs:
 
@@ -285,14 +285,15 @@
     ChannelMembershipTypeType,
     ChannelMessagePersistenceTypeType,
     ChannelMessageStatusType,
     ChannelMessageTypeType,
     ChannelModeType,
     ChannelPrivacyType,
     ErrorCodeType,
+    ExpirationCriterionType,
     FallbackActionType,
     InvocationTypeType,
     MessagingDataTypeType,
     PushNotificationTypeType,
     SearchFieldKeyType,
     SearchFieldOperatorType,
     SortOrderType,
@@ -325,14 +326,15 @@
     ChannelAssociatedWithFlowSummaryTypeDef,
     ChannelSummaryTypeDef,
     PushNotificationPreferencesTypeDef,
     MessageAttributeValueTypeDef,
     PushNotificationConfigurationTypeDef,
     ChannelMessageStatusStructureTypeDef,
     ElasticChannelConfigurationTypeDef,
+    ExpirationSettingsTypeDef,
     CreateChannelBanRequestRequestTypeDef,
     TagTypeDef,
     CreateChannelMembershipRequestRequestTypeDef,
     CreateChannelModeratorRequestRequestTypeDef,
     DeleteChannelBanRequestRequestTypeDef,
     DeleteChannelFlowRequestRequestTypeDef,
     DeleteChannelMembershipRequestRequestTypeDef,
@@ -401,14 +403,16 @@
     SendChannelMessageRequestRequestTypeDef,
     ChannelMessageSummaryTypeDef,
     ChannelMessageTypeDef,
     GetChannelMessageStatusResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
     ChannelTypeDef,
+    PutChannelExpirationSettingsRequestRequestTypeDef,
+    PutChannelExpirationSettingsResponseTypeDef,
     CreateChannelRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     GetMessagingSessionEndpointResponseTypeDef,
     GetMessagingStreamingConfigurationsResponseTypeDef,
     PutMessagingStreamingConfigurationsRequestRequestTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
@@ -450,42 +454,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-messaging-1.26.98/mypy_boto3_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-messaging-1.26.96/setup.py` & `mypy-boto3-chime-sdk-messaging-1.26.98/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-chime-sdk-messaging.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-messaging",
-    version="1.26.96",
+    version="1.26.98",
     packages=["mypy_boto3_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKMessaging 1.26.96 service generated with"
-        " mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.ChimeSDKMessaging 1.26.98 service generated with"
+        " mypy-boto3-builder 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -47,11 +47,11 @@
         "Documentation": (
             "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_messaging/"
         ),
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

