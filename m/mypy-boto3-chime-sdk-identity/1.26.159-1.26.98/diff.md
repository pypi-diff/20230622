# Comparing `tmp/mypy-boto3-chime-sdk-identity-1.26.159.tar.gz` & `tmp/mypy-boto3-chime-sdk-identity-1.26.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-chime-sdk-identity-1.26.159.tar", last modified: Thu Jun 22 19:47:24 2023, max compression
+gzip compressed data, was "mypy-boto3-chime-sdk-identity-1.26.98.tar", last modified: Thu Mar 23 19:33:04 2023, max compression
```

## Comparing `mypy-boto3-chime-sdk-identity-1.26.159.tar` & `mypy-boto3-chime-sdk-identity-1.26.98.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:47:24.517522 mypy-boto3-chime-sdk-identity-1.26.159/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-22 19:47:24.513522 mypy-boto3-chime-sdk-identity-1.26.159/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:47:24.509522 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22841 2023-06-22 19:46:59.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22805 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-22 19:46:59.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-22 19:46:59.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25328 2023-06-22 19:46:59.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25299 2023-06-22 19:46:59.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:47:24.513522 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-06-22 19:47:24.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-22 19:47:24.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:47:24.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:47:24.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 19:47:24.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-22 19:47:24.000000 mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:47:24.517522 mypy-boto3-chime-sdk-identity-1.26.159/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-22 19:46:58.000000 mypy-boto3-chime-sdk-identity-1.26.159/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14092 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.403627 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22758 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22722 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7984 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24648 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24621 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-23 19:33:04.000000 mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 19:33:04.411627 mypy-boto3-chime-sdk-identity-1.26.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-23 19:31:58.000000 mypy-boto3-chime-sdk-identity-1.26.98/setup.py
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/LICENSE` & `mypy-boto3-chime-sdk-identity-1.26.98/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/PKG-INFO` & `mypy-boto3-chime-sdk-identity-1.26.98/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-identity
-Version: 1.26.159
-Summary: Type annotations for boto3.ChimeSDKIdentity 1.26.159 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKIdentity 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-identity"></a>
 
 # mypy-boto3-chime-sdk-identity
 
 [![PyPI - mypy-boto3-chime-sdk-identity](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKIdentity 1.26.159](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[boto3.ChimeSDKIdentity 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,16 +283,14 @@
 from mypy_boto3_chime_sdk_identity.literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
     ExpirationCriterionType,
     RespondsToType,
-    StandardMessagesType,
-    TargetedMessagesType,
     ChimeSDKIdentityServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -314,47 +312,49 @@
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
+    LexConfigurationTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
-    InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAppInstanceBotRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     AppInstanceRetentionSettingsTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
+    ConfigurationTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceBotResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     DescribeAppInstanceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListAppInstanceBotsResponseTypeDef,
@@ -366,27 +366,24 @@
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     ListAppInstanceUserEndpointsResponseTypeDef,
     DescribeAppInstanceUserEndpointResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
-    ConfigurationTypeDef,
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
-    UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
 def get_structure() -> IdentityTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/README.md` & `mypy-boto3-chime-sdk-identity-1.26.98/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-chime-sdk-identity"></a>
 
 # mypy-boto3-chime-sdk-identity
 
 [![PyPI - mypy-boto3-chime-sdk-identity](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKIdentity 1.26.159](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[boto3.ChimeSDKIdentity 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -251,16 +251,14 @@
 from mypy_boto3_chime_sdk_identity.literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
     ExpirationCriterionType,
     RespondsToType,
-    StandardMessagesType,
-    TargetedMessagesType,
     ChimeSDKIdentityServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -282,47 +280,49 @@
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
+    LexConfigurationTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
-    InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAppInstanceBotRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     AppInstanceRetentionSettingsTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
+    ConfigurationTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceBotResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     DescribeAppInstanceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListAppInstanceBotsResponseTypeDef,
@@ -334,27 +334,24 @@
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     ListAppInstanceUserEndpointsResponseTypeDef,
     DescribeAppInstanceUserEndpointResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
-    ConfigurationTypeDef,
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
-    UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
 def get_structure() -> IdentityTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/__main__.py` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ChimeSDKIdentity 1.26.159\nVersion:         1.26.159\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ChimeSDKIdentity 1.26.98\nVersion:         1.26.98\nBuilder"
+        " version: 7.14.2\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.159")
+    print("1.26.98")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/client.py` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,20 +411,15 @@
         Updates `AppInstance` metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance)
         """
 
     def update_app_instance_bot(
-        self,
-        *,
-        AppInstanceBotArn: str,
-        Name: str,
-        Metadata: str,
-        Configuration: ConfigurationTypeDef = ...
+        self, *, AppInstanceBotArn: str, Name: str, Metadata: str
     ) -> UpdateAppInstanceBotResponseTypeDef:
         """
         Updates the name and metadata of an `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance_bot)
         """
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/client.pyi` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -377,20 +377,15 @@
         """
         Updates `AppInstance` metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance)
         """
     def update_app_instance_bot(
-        self,
-        *,
-        AppInstanceBotArn: str,
-        Name: str,
-        Metadata: str,
-        Configuration: ConfigurationTypeDef = ...
+        self, *, AppInstanceBotArn: str, Name: str, Metadata: str
     ) -> UpdateAppInstanceBotResponseTypeDef:
         """
         Updates the name and metadata of an `AppInstanceBot`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity.Client.update_app_instance_bot)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/client/#update_app_instance_bot)
         """
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/literals.py` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,39 +14,33 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AllowMessagesType",
     "AppInstanceUserEndpointTypeType",
     "EndpointStatusReasonType",
     "EndpointStatusType",
     "ExpirationCriterionType",
     "RespondsToType",
-    "StandardMessagesType",
-    "TargetedMessagesType",
     "ChimeSDKIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AllowMessagesType = Literal["ALL", "NONE"]
 AppInstanceUserEndpointTypeType = Literal["APNS", "APNS_SANDBOX", "GCM"]
 EndpointStatusReasonType = Literal["INVALID_DEVICE_TOKEN", "INVALID_PINPOINT_ARN"]
 EndpointStatusType = Literal["ACTIVE", "INACTIVE"]
 ExpirationCriterionType = Literal["CREATED_TIMESTAMP"]
 RespondsToType = Literal["STANDARD_MESSAGES"]
-StandardMessagesType = Literal["ALL", "AUTO", "MENTIONS", "NONE"]
-TargetedMessagesType = Literal["ALL", "NONE"]
 ChimeSDKIdentityServiceName = Literal["chime-sdk-identity"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -102,15 +96,14 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -252,15 +245,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -279,19 +271,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -375,17 +364,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/literals.pyi` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,37 +14,35 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AllowMessagesType",
     "AppInstanceUserEndpointTypeType",
     "EndpointStatusReasonType",
     "EndpointStatusType",
     "ExpirationCriterionType",
     "RespondsToType",
-    "StandardMessagesType",
-    "TargetedMessagesType",
     "ChimeSDKIdentityServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AllowMessagesType = Literal["ALL", "NONE"]
 AppInstanceUserEndpointTypeType = Literal["APNS", "APNS_SANDBOX", "GCM"]
 EndpointStatusReasonType = Literal["INVALID_DEVICE_TOKEN", "INVALID_PINPOINT_ARN"]
 EndpointStatusType = Literal["ACTIVE", "INACTIVE"]
 ExpirationCriterionType = Literal["CREATED_TIMESTAMP"]
 RespondsToType = Literal["STANDARD_MESSAGES"]
-StandardMessagesType = Literal["ALL", "AUTO", "MENTIONS", "NONE"]
-TargetedMessagesType = Literal["ALL", "NONE"]
 ChimeSDKIdentityServiceName = Literal["chime-sdk-identity"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -100,15 +98,14 @@
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
-    "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
     "codestar-notifications",
     "cognito-identity",
     "cognito-idp",
@@ -250,15 +247,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -277,19 +273,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -373,17 +366,15 @@
     "textract",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
-    "verifiedpermissions",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/type_defs.py` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 from typing import Dict, List, Sequence
 
 from .literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
-    StandardMessagesType,
-    TargetedMessagesType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -40,47 +38,49 @@
     "ChannelRetentionSettingsTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "EndpointStateTypeDef",
     "EndpointAttributesTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "ExpirationSettingsTypeDef",
+    "LexConfigurationTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceBotRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeregisterAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceAdminRequestRequestTypeDef",
     "DescribeAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceRequestRequestTypeDef",
     "DescribeAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceUserRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
-    "InvokedByTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceBotsRequestRequestTypeDef",
     "ListAppInstanceUserEndpointsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAppInstanceBotRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
     "UpdateAppInstanceUserEndpointRequestRequestTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
     "AppInstanceUserEndpointSummaryTypeDef",
     "AppInstanceUserEndpointTypeDef",
     "RegisterAppInstanceUserEndpointRequestRequestTypeDef",
     "AppInstanceUserTypeDef",
     "PutAppInstanceUserExpirationSettingsRequestRequestTypeDef",
+    "ConfigurationTypeDef",
     "CreateAppInstanceAdminResponseTypeDef",
     "CreateAppInstanceBotResponseTypeDef",
     "CreateAppInstanceResponseTypeDef",
     "CreateAppInstanceUserResponseTypeDef",
     "DescribeAppInstanceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListAppInstanceBotsResponseTypeDef",
@@ -92,27 +92,24 @@
     "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserEndpointResponseTypeDef",
     "UpdateAppInstanceUserResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "LexConfigurationTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     "ListAppInstanceUserEndpointsResponseTypeDef",
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     "DescribeAppInstanceUserResponseTypeDef",
-    "ConfigurationTypeDef",
     "AppInstanceBotTypeDef",
     "CreateAppInstanceBotRequestRequestTypeDef",
-    "UpdateAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceBotResponseTypeDef",
 )
 
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "Arn": str,
@@ -215,14 +212,35 @@
     "ExpirationSettingsTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": Literal["CREATED_TIMESTAMP"],
     },
 )
 
+_RequiredLexConfigurationTypeDef = TypedDict(
+    "_RequiredLexConfigurationTypeDef",
+    {
+        "RespondsTo": Literal["STANDARD_MESSAGES"],
+        "LexBotAliasArn": str,
+        "LocaleId": str,
+    },
+)
+_OptionalLexConfigurationTypeDef = TypedDict(
+    "_OptionalLexConfigurationTypeDef",
+    {
+        "WelcomeIntent": str,
+    },
+    total=False,
+)
+
+
+class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
+    pass
+
+
 CreateAppInstanceAdminRequestRequestTypeDef = TypedDict(
     "CreateAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
         "AppInstanceArn": str,
     },
 )
@@ -323,22 +341,14 @@
 GetAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
-InvokedByTypeDef = TypedDict(
-    "InvokedByTypeDef",
-    {
-        "StandardMessages": StandardMessagesType,
-        "TargetedMessages": TargetedMessagesType,
-    },
-)
-
 _RequiredListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppInstanceAdminsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 _OptionalListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
@@ -447,14 +457,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
+    "UpdateAppInstanceBotRequestRequestTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "Name": str,
+        "Metadata": str,
+    },
+)
+
 UpdateAppInstanceRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "Metadata": str,
     },
@@ -607,14 +626,21 @@
 class PutAppInstanceUserExpirationSettingsRequestRequestTypeDef(
     _RequiredPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
     _OptionalPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
 ):
     pass
 
 
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Lex": LexConfigurationTypeDef,
+    },
+)
+
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -801,36 +827,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredLexConfigurationTypeDef = TypedDict(
-    "_RequiredLexConfigurationTypeDef",
-    {
-        "LexBotAliasArn": str,
-        "LocaleId": str,
-    },
-)
-_OptionalLexConfigurationTypeDef = TypedDict(
-    "_OptionalLexConfigurationTypeDef",
-    {
-        "RespondsTo": Literal["STANDARD_MESSAGES"],
-        "InvokedBy": InvokedByTypeDef,
-        "WelcomeIntent": str,
-    },
-    total=False,
-)
-
-
-class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
-    pass
-
-
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -892,21 +896,14 @@
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Lex": LexConfigurationTypeDef,
-    },
-)
-
 AppInstanceBotTypeDef = TypedDict(
     "AppInstanceBotTypeDef",
     {
         "AppInstanceBotArn": str,
         "Name": str,
         "Configuration": ConfigurationTypeDef,
         "CreatedTimestamp": datetime,
@@ -938,38 +935,14 @@
 class CreateAppInstanceBotRequestRequestTypeDef(
     _RequiredCreateAppInstanceBotRequestRequestTypeDef,
     _OptionalCreateAppInstanceBotRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppInstanceBotRequestRequestTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "Name": str,
-        "Metadata": str,
-    },
-)
-_OptionalUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppInstanceBotRequestRequestTypeDef",
-    {
-        "Configuration": ConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateAppInstanceBotRequestRequestTypeDef(
-    _RequiredUpdateAppInstanceBotRequestRequestTypeDef,
-    _OptionalUpdateAppInstanceBotRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeAppInstanceBotResponseTypeDef = TypedDict(
     "DescribeAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBot": AppInstanceBotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity/type_defs.pyi` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 from typing import Dict, List, Sequence
 
 from .literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
-    StandardMessagesType,
-    TargetedMessagesType,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
@@ -39,47 +37,49 @@
     "ChannelRetentionSettingsTypeDef",
     "AppInstanceSummaryTypeDef",
     "AppInstanceTypeDef",
     "EndpointStateTypeDef",
     "EndpointAttributesTypeDef",
     "AppInstanceUserSummaryTypeDef",
     "ExpirationSettingsTypeDef",
+    "LexConfigurationTypeDef",
     "CreateAppInstanceAdminRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DeleteAppInstanceAdminRequestRequestTypeDef",
     "DeleteAppInstanceBotRequestRequestTypeDef",
     "DeleteAppInstanceRequestRequestTypeDef",
     "DeleteAppInstanceUserRequestRequestTypeDef",
     "DeregisterAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceAdminRequestRequestTypeDef",
     "DescribeAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceRequestRequestTypeDef",
     "DescribeAppInstanceUserEndpointRequestRequestTypeDef",
     "DescribeAppInstanceUserRequestRequestTypeDef",
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
-    "InvokedByTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceBotsRequestRequestTypeDef",
     "ListAppInstanceUserEndpointsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "UpdateAppInstanceBotRequestRequestTypeDef",
     "UpdateAppInstanceRequestRequestTypeDef",
     "UpdateAppInstanceUserEndpointRequestRequestTypeDef",
     "UpdateAppInstanceUserRequestRequestTypeDef",
     "AppInstanceAdminSummaryTypeDef",
     "AppInstanceAdminTypeDef",
     "AppInstanceRetentionSettingsTypeDef",
     "AppInstanceUserEndpointSummaryTypeDef",
     "AppInstanceUserEndpointTypeDef",
     "RegisterAppInstanceUserEndpointRequestRequestTypeDef",
     "AppInstanceUserTypeDef",
     "PutAppInstanceUserExpirationSettingsRequestRequestTypeDef",
+    "ConfigurationTypeDef",
     "CreateAppInstanceAdminResponseTypeDef",
     "CreateAppInstanceBotResponseTypeDef",
     "CreateAppInstanceResponseTypeDef",
     "CreateAppInstanceUserResponseTypeDef",
     "DescribeAppInstanceResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListAppInstanceBotsResponseTypeDef",
@@ -91,27 +91,24 @@
     "UpdateAppInstanceResponseTypeDef",
     "UpdateAppInstanceUserEndpointResponseTypeDef",
     "UpdateAppInstanceUserResponseTypeDef",
     "CreateAppInstanceRequestRequestTypeDef",
     "CreateAppInstanceUserRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "LexConfigurationTypeDef",
     "ListAppInstanceAdminsResponseTypeDef",
     "DescribeAppInstanceAdminResponseTypeDef",
     "GetAppInstanceRetentionSettingsResponseTypeDef",
     "PutAppInstanceRetentionSettingsRequestRequestTypeDef",
     "PutAppInstanceRetentionSettingsResponseTypeDef",
     "ListAppInstanceUserEndpointsResponseTypeDef",
     "DescribeAppInstanceUserEndpointResponseTypeDef",
     "DescribeAppInstanceUserResponseTypeDef",
-    "ConfigurationTypeDef",
     "AppInstanceBotTypeDef",
     "CreateAppInstanceBotRequestRequestTypeDef",
-    "UpdateAppInstanceBotRequestRequestTypeDef",
     "DescribeAppInstanceBotResponseTypeDef",
 )
 
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "Arn": str,
@@ -210,14 +207,33 @@
     "ExpirationSettingsTypeDef",
     {
         "ExpirationDays": int,
         "ExpirationCriterion": Literal["CREATED_TIMESTAMP"],
     },
 )
 
+_RequiredLexConfigurationTypeDef = TypedDict(
+    "_RequiredLexConfigurationTypeDef",
+    {
+        "RespondsTo": Literal["STANDARD_MESSAGES"],
+        "LexBotAliasArn": str,
+        "LocaleId": str,
+    },
+)
+_OptionalLexConfigurationTypeDef = TypedDict(
+    "_OptionalLexConfigurationTypeDef",
+    {
+        "WelcomeIntent": str,
+    },
+    total=False,
+)
+
+class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
+    pass
+
 CreateAppInstanceAdminRequestRequestTypeDef = TypedDict(
     "CreateAppInstanceAdminRequestRequestTypeDef",
     {
         "AppInstanceAdminArn": str,
         "AppInstanceArn": str,
     },
 )
@@ -318,22 +334,14 @@
 GetAppInstanceRetentionSettingsRequestRequestTypeDef = TypedDict(
     "GetAppInstanceRetentionSettingsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 
-InvokedByTypeDef = TypedDict(
-    "InvokedByTypeDef",
-    {
-        "StandardMessages": StandardMessagesType,
-        "TargetedMessages": TargetedMessagesType,
-    },
-)
-
 _RequiredListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppInstanceAdminsRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
     },
 )
 _OptionalListAppInstanceAdminsRequestRequestTypeDef = TypedDict(
@@ -434,14 +442,23 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
+UpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
+    "UpdateAppInstanceBotRequestRequestTypeDef",
+    {
+        "AppInstanceBotArn": str,
+        "Name": str,
+        "Metadata": str,
+    },
+)
+
 UpdateAppInstanceRequestRequestTypeDef = TypedDict(
     "UpdateAppInstanceRequestRequestTypeDef",
     {
         "AppInstanceArn": str,
         "Name": str,
         "Metadata": str,
     },
@@ -588,14 +605,21 @@
 
 class PutAppInstanceUserExpirationSettingsRequestRequestTypeDef(
     _RequiredPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
     _OptionalPutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
 ):
     pass
 
+ConfigurationTypeDef = TypedDict(
+    "ConfigurationTypeDef",
+    {
+        "Lex": LexConfigurationTypeDef,
+    },
+)
+
 CreateAppInstanceAdminResponseTypeDef = TypedDict(
     "CreateAppInstanceAdminResponseTypeDef",
     {
         "AppInstanceAdmin": IdentityTypeDef,
         "AppInstanceArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -778,34 +802,14 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
-_RequiredLexConfigurationTypeDef = TypedDict(
-    "_RequiredLexConfigurationTypeDef",
-    {
-        "LexBotAliasArn": str,
-        "LocaleId": str,
-    },
-)
-_OptionalLexConfigurationTypeDef = TypedDict(
-    "_OptionalLexConfigurationTypeDef",
-    {
-        "RespondsTo": Literal["STANDARD_MESSAGES"],
-        "InvokedBy": InvokedByTypeDef,
-        "WelcomeIntent": str,
-    },
-    total=False,
-)
-
-class LexConfigurationTypeDef(_RequiredLexConfigurationTypeDef, _OptionalLexConfigurationTypeDef):
-    pass
-
 ListAppInstanceAdminsResponseTypeDef = TypedDict(
     "ListAppInstanceAdminsResponseTypeDef",
     {
         "AppInstanceArn": str,
         "AppInstanceAdmins": List[AppInstanceAdminSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -867,21 +871,14 @@
     "DescribeAppInstanceUserResponseTypeDef",
     {
         "AppInstanceUser": AppInstanceUserTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConfigurationTypeDef = TypedDict(
-    "ConfigurationTypeDef",
-    {
-        "Lex": LexConfigurationTypeDef,
-    },
-)
-
 AppInstanceBotTypeDef = TypedDict(
     "AppInstanceBotTypeDef",
     {
         "AppInstanceBotArn": str,
         "Name": str,
         "Configuration": ConfigurationTypeDef,
         "CreatedTimestamp": datetime,
@@ -911,36 +908,14 @@
 
 class CreateAppInstanceBotRequestRequestTypeDef(
     _RequiredCreateAppInstanceBotRequestRequestTypeDef,
     _OptionalCreateAppInstanceBotRequestRequestTypeDef,
 ):
     pass
 
-_RequiredUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppInstanceBotRequestRequestTypeDef",
-    {
-        "AppInstanceBotArn": str,
-        "Name": str,
-        "Metadata": str,
-    },
-)
-_OptionalUpdateAppInstanceBotRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppInstanceBotRequestRequestTypeDef",
-    {
-        "Configuration": ConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateAppInstanceBotRequestRequestTypeDef(
-    _RequiredUpdateAppInstanceBotRequestRequestTypeDef,
-    _OptionalUpdateAppInstanceBotRequestRequestTypeDef,
-):
-    pass
-
 DescribeAppInstanceBotResponseTypeDef = TypedDict(
     "DescribeAppInstanceBotResponseTypeDef",
     {
         "AppInstanceBot": AppInstanceBotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-chime-sdk-identity
-Version: 1.26.159
-Summary: Type annotations for boto3.ChimeSDKIdentity 1.26.159 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.98
+Summary: Type annotations for boto3.ChimeSDKIdentity 1.26.98 service generated with mypy-boto3-builder 7.14.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-chime-sdk-identity"></a>
 
 # mypy-boto3-chime-sdk-identity
 
 [![PyPI - mypy-boto3-chime-sdk-identity](https://img.shields.io/pypi/v/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/mypy-boto3-chime-sdk-identity)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-chime-sdk-identity?color=blue)](https://pypistats.org/packages/mypy-boto3-chime-sdk-identity)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ChimeSDKIdentity 1.26.159](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
+[boto3.ChimeSDKIdentity 1.26.98](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-chime-sdk-identity docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -283,16 +283,14 @@
 from mypy_boto3_chime_sdk_identity.literals import (
     AllowMessagesType,
     AppInstanceUserEndpointTypeType,
     EndpointStatusReasonType,
     EndpointStatusType,
     ExpirationCriterionType,
     RespondsToType,
-    StandardMessagesType,
-    TargetedMessagesType,
     ChimeSDKIdentityServiceName,
     ServiceName,
     ResourceServiceName,
     RegionName,
 )
 
 
@@ -314,47 +312,49 @@
     ChannelRetentionSettingsTypeDef,
     AppInstanceSummaryTypeDef,
     AppInstanceTypeDef,
     EndpointStateTypeDef,
     EndpointAttributesTypeDef,
     AppInstanceUserSummaryTypeDef,
     ExpirationSettingsTypeDef,
+    LexConfigurationTypeDef,
     CreateAppInstanceAdminRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     TagTypeDef,
     DeleteAppInstanceAdminRequestRequestTypeDef,
     DeleteAppInstanceBotRequestRequestTypeDef,
     DeleteAppInstanceRequestRequestTypeDef,
     DeleteAppInstanceUserRequestRequestTypeDef,
     DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceAdminRequestRequestTypeDef,
     DescribeAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceRequestRequestTypeDef,
     DescribeAppInstanceUserEndpointRequestRequestTypeDef,
     DescribeAppInstanceUserRequestRequestTypeDef,
     GetAppInstanceRetentionSettingsRequestRequestTypeDef,
-    InvokedByTypeDef,
     ListAppInstanceAdminsRequestRequestTypeDef,
     ListAppInstanceBotsRequestRequestTypeDef,
     ListAppInstanceUserEndpointsRequestRequestTypeDef,
     ListAppInstanceUsersRequestRequestTypeDef,
     ListAppInstancesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    UpdateAppInstanceBotRequestRequestTypeDef,
     UpdateAppInstanceRequestRequestTypeDef,
     UpdateAppInstanceUserEndpointRequestRequestTypeDef,
     UpdateAppInstanceUserRequestRequestTypeDef,
     AppInstanceAdminSummaryTypeDef,
     AppInstanceAdminTypeDef,
     AppInstanceRetentionSettingsTypeDef,
     AppInstanceUserEndpointSummaryTypeDef,
     AppInstanceUserEndpointTypeDef,
     RegisterAppInstanceUserEndpointRequestRequestTypeDef,
     AppInstanceUserTypeDef,
     PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
+    ConfigurationTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceBotResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     DescribeAppInstanceResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListAppInstanceBotsResponseTypeDef,
@@ -366,27 +366,24 @@
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserEndpointResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     CreateAppInstanceRequestRequestTypeDef,
     CreateAppInstanceUserRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    LexConfigurationTypeDef,
     ListAppInstanceAdminsResponseTypeDef,
     DescribeAppInstanceAdminResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceRetentionSettingsRequestRequestTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     ListAppInstanceUserEndpointsResponseTypeDef,
     DescribeAppInstanceUserEndpointResponseTypeDef,
     DescribeAppInstanceUserResponseTypeDef,
-    ConfigurationTypeDef,
     AppInstanceBotTypeDef,
     CreateAppInstanceBotRequestRequestTypeDef,
-    UpdateAppInstanceBotRequestRequestTypeDef,
     DescribeAppInstanceBotResponseTypeDef,
 )
 
 
 def get_structure() -> IdentityTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt` & `mypy-boto3-chime-sdk-identity-1.26.98/mypy_boto3_chime_sdk_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-chime-sdk-identity-1.26.159/setup.py` & `mypy-boto3-chime-sdk-identity-1.26.98/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-chime-sdk-identity",
-    version="1.26.159",
+    version="1.26.98",
     packages=["mypy_boto3_chime_sdk_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ChimeSDKIdentity 1.26.159 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ChimeSDKIdentity 1.26.98 service generated with"
+        " mypy-boto3-builder 7.14.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

