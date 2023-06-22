# Comparing `tmp/mypy-boto3-stepfunctions-1.26.159.tar.gz` & `tmp/mypy-boto3-stepfunctions-1.26.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-stepfunctions-1.26.159.tar", last modified: Thu Jun 22 19:47:24 2023, max compression
+gzip compressed data, was "mypy-boto3-stepfunctions-1.26.21.tar", last modified: Thu Dec  1 20:25:43 2022, max compression
```

## Comparing `mypy-boto3-stepfunctions-1.26.159.tar` & `mypy-boto3-stepfunctions-1.26.21.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:47:24.513522 mypy-boto3-stepfunctions-1.26.159/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-06-22 19:47:24.513522 mypy-boto3-stepfunctions-1.26.159/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16650 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:47:24.509522 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28378 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28332 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10811 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10809 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43887 2023-06-22 19:47:13.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43822 2023-06-22 19:47:12.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:47:24.513522 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18153 2023-06-22 19:47:24.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-22 19:47:24.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:47:24.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:47:24.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-22 19:47:24.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 19:47:24.000000 mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 19:47:24.513522 mypy-boto3-stepfunctions-1.26.159/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 19:47:11.000000 mypy-boto3-stepfunctions-1.26.159/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.830803 mypy-boto3-stepfunctions-1.26.21/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    17347 2022-12-01 20:25:43.822803 mypy-boto3-stepfunctions-1.26.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    15896 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.818803 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1395 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      912 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22270 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22232 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    10402 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10400 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     6344 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6337 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)    37018 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36963 2022-12-01 20:25:35.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-01 20:25:43.822803 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    17347 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      794 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-12-01 20:25:43.000000 mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-01 20:25:43.830803 mypy-boto3-stepfunctions-1.26.21/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1985 2022-12-01 20:25:34.000000 mypy-boto3-stepfunctions-1.26.21/setup.py
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/LICENSE` & `mypy-boto3-stepfunctions-1.26.21/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/PKG-INFO` & `mypy-boto3-stepfunctions-1.26.21/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.26.159
-Summary: Type annotations for boto3.SFN 1.26.159 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.21
+Summary: Type annotations for boto3.SFN 1.26.21 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.26.159](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,26 +354,22 @@
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    RoutingConfigurationListItemTypeDef,
     TracingConfigurationTypeDef,
     DeleteActivityInputRequestTypeDef,
-    DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
-    DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
-    DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
@@ -394,22 +389,17 @@
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
     ListActivitiesInputRequestTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
-    ListStateMachineAliasesInputRequestTypeDef,
-    StateMachineAliasListItemTypeDef,
-    ListStateMachineVersionsInputRequestTypeDef,
-    StateMachineVersionListItemTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PublishStateMachineVersionInputRequestTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
@@ -423,42 +413,34 @@
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateActivityOutputTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     ListActivitiesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
-    CreateStateMachineAliasInputRequestTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
-    UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
     GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     ListActivitiesInputListActivitiesPaginateTypeDef,
     ListExecutionsInputListExecutionsPaginateTypeDef,
     ListMapRunsInputListMapRunsPaginateTypeDef,
     ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
-    ListStateMachineAliasesOutputTypeDef,
-    ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     UpdateStateMachineInputRequestTypeDef,
@@ -473,42 +455,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/README.md` & `mypy-boto3-stepfunctions-1.26.21/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.26.159](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,26 +323,22 @@
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    RoutingConfigurationListItemTypeDef,
     TracingConfigurationTypeDef,
     DeleteActivityInputRequestTypeDef,
-    DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
-    DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
-    DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
@@ -362,22 +358,17 @@
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
     ListActivitiesInputRequestTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
-    ListStateMachineAliasesInputRequestTypeDef,
-    StateMachineAliasListItemTypeDef,
-    ListStateMachineVersionsInputRequestTypeDef,
-    StateMachineVersionListItemTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PublishStateMachineVersionInputRequestTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
@@ -391,42 +382,34 @@
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateActivityOutputTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     ListActivitiesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
-    CreateStateMachineAliasInputRequestTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
-    UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
     GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     ListActivitiesInputListActivitiesPaginateTypeDef,
     ListExecutionsInputListExecutionsPaginateTypeDef,
     ListMapRunsInputListMapRunsPaginateTypeDef,
     ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
-    ListStateMachineAliasesOutputTypeDef,
-    ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     UpdateStateMachineInputRequestTypeDef,
@@ -441,42 +424,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/__init__.py` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/__init__.pyi` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/__main__.py` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SFN 1.26.159\nVersion:         1.26.159\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for boto3.SFN 1.26.21\nVersion:         1.26.21\nBuilder version:"
+        " 7.11.11\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.159")
+    print("1.26.21")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/client.py` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,40 +24,33 @@
     ListActivitiesPaginator,
     ListExecutionsPaginator,
     ListMapRunsPaginator,
     ListStateMachinesPaginator,
 )
 from .type_defs import (
     CreateActivityOutputTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     DescribeMapRunOutputTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     GetExecutionHistoryOutputTypeDef,
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
-    ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
-    ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -75,29 +68,27 @@
 
 
 class Exceptions:
     ActivityDoesNotExist: Type[BotocoreClientError]
     ActivityLimitExceeded: Type[BotocoreClientError]
     ActivityWorkerLimitExceeded: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
-    ConflictException: Type[BotocoreClientError]
     ExecutionAlreadyExists: Type[BotocoreClientError]
     ExecutionDoesNotExist: Type[BotocoreClientError]
     ExecutionLimitExceeded: Type[BotocoreClientError]
     InvalidArn: Type[BotocoreClientError]
     InvalidDefinition: Type[BotocoreClientError]
     InvalidExecutionInput: Type[BotocoreClientError]
     InvalidLoggingConfiguration: Type[BotocoreClientError]
     InvalidName: Type[BotocoreClientError]
     InvalidOutput: Type[BotocoreClientError]
     InvalidToken: Type[BotocoreClientError]
     InvalidTracingConfiguration: Type[BotocoreClientError]
     MissingRequiredParameter: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
-    ServiceQuotaExceededException: Type[BotocoreClientError]
     StateMachineAlreadyExists: Type[BotocoreClientError]
     StateMachineDeleting: Type[BotocoreClientError]
     StateMachineDoesNotExist: Type[BotocoreClientError]
     StateMachineLimitExceeded: Type[BotocoreClientError]
     StateMachineTypeNotSupported: Type[BotocoreClientError]
     TaskDoesNotExist: Type[BotocoreClientError]
     TaskTimedOut: Type[BotocoreClientError]
@@ -153,43 +144,23 @@
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...,
-        publish: bool = ...,
-        versionDescription: str = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine)
         """
 
-    def create_state_machine_alias(
-        self,
-        *,
-        name: str,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
-        description: str = ...
-    ) -> CreateStateMachineAliasOutputTypeDef:
-        """
-        Creates an [alias](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-alias.html)_ for a state machine that
-        points to one or two [versions](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-version.html)_ of the same state
-        machine.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine_alias)
-        """
-
     def delete_activity(self, *, activityArn: str) -> Dict[str, Any]:
         """
         Deletes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_activity)
         """
@@ -198,45 +169,27 @@
         """
         Deletes a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine)
         """
 
-    def delete_state_machine_alias(self, *, stateMachineAliasArn: str) -> Dict[str, Any]:
-        """
-        Deletes a state machine [alias](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-alias.html)_.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_alias)
-        """
-
-    def delete_state_machine_version(self, *, stateMachineVersionArn: str) -> Dict[str, Any]:
-        """
-        Deletes a state machine [version](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-version.html)_.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_version)
-        """
-
     def describe_activity(self, *, activityArn: str) -> DescribeActivityOutputTypeDef:
         """
         Describes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_activity)
         """
 
     def describe_execution(self, *, executionArn: str) -> DescribeExecutionOutputTypeDef:
         """
-        Provides information about a state machine execution, such as the state machine
-        associated with the execution, the execution input and output, and relevant
-        execution metadata.
+        Provides all information about a state machine execution, such as the state
+        machine associated with the execution, the execution input and output, and
+        relevant execution metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_execution)
         """
 
     def describe_map_run(self, *, mapRunArn: str) -> DescribeMapRunOutputTypeDef:
         """
@@ -251,25 +204,14 @@
         Provides information about a state machine's definition, its IAM role Amazon
         Resource Name (ARN), and configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine)
         """
 
-    def describe_state_machine_alias(
-        self, *, stateMachineAliasArn: str
-    ) -> DescribeStateMachineAliasOutputTypeDef:
-        """
-        Returns details about a state machine [alias](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-alias.html)_.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine_alias)
-        """
-
     def describe_state_machine_for_execution(
         self, *, executionArn: str
     ) -> DescribeStateMachineForExecutionOutputTypeDef:
         """
         Provides information about a state machine's definition, its execution role ARN,
         and configuration.
 
@@ -350,37 +292,14 @@
         """
         Lists all Map Runs that were started by a given state machine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_map_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_map_runs)
         """
 
-    def list_state_machine_aliases(
-        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
-    ) -> ListStateMachineAliasesOutputTypeDef:
-        """
-        Lists [aliases](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
-        state-machine-alias.html)_ for a specified state machine ARN.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_aliases)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_aliases)
-        """
-
-    def list_state_machine_versions(
-        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
-    ) -> ListStateMachineVersionsOutputTypeDef:
-        """
-        Lists [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
-        state-machine-version.html)_ for the specified state machine Amazon Resource
-        Name (ARN).
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_versions)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_versions)
-        """
-
     def list_state_machines(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStateMachinesOutputTypeDef:
         """
         Lists the existing state machines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machines)
@@ -391,26 +310,14 @@
         """
         List tags for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_tags_for_resource)
         """
 
-    def publish_state_machine_version(
-        self, *, stateMachineArn: str, revisionId: str = ..., description: str = ...
-    ) -> PublishStateMachineVersionOutputTypeDef:
-        """
-        Creates a [version](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-version.html)_ from the current
-        revision of a state machine.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.publish_state_machine_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#publish_state_machine_version)
-        """
-
     def send_task_failure(
         self, *, taskToken: str, error: str = ..., cause: str = ...
     ) -> Dict[str, Any]:
         """
         Used by activity workers and task states using the
         [callback](https://docs.aws.amazon.com/step-functions/latest/dg/connect-to-
         resource.html#connect-wait-token)_ pattern to report that the task identified by
@@ -508,42 +415,24 @@
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...,
-        publish: bool = ...,
-        versionDescription: str = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
-        Updates an existing state machine by modifying its `definition`, `roleArn`, or
+        Updates an existing state machine by modifying its `definition` , `roleArn` , or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine)
         """
 
-    def update_state_machine_alias(
-        self,
-        *,
-        stateMachineAliasArn: str,
-        description: str = ...,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
-    ) -> UpdateStateMachineAliasOutputTypeDef:
-        """
-        Updates the configuration of an existing state machine
-        [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-
-        machine-alias.html)_ by modifying its `description` or `routingConfiguration`.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine_alias)
-        """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_execution_history"]
     ) -> GetExecutionHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_paginator)
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/client.pyi` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/client.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -24,40 +24,33 @@
     ListActivitiesPaginator,
     ListExecutionsPaginator,
     ListMapRunsPaginator,
     ListStateMachinesPaginator,
 )
 from .type_defs import (
     CreateActivityOutputTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     DescribeMapRunOutputTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     GetExecutionHistoryOutputTypeDef,
     ListActivitiesOutputTypeDef,
     ListExecutionsOutputTypeDef,
     ListMapRunsOutputTypeDef,
-    ListStateMachineAliasesOutputTypeDef,
     ListStateMachinesOutputTypeDef,
-    ListStateMachineVersionsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     LoggingConfigurationTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
-    RoutingConfigurationListItemTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
     TagTypeDef,
     TracingConfigurationTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -72,29 +65,27 @@
         self.operation_name: str
 
 class Exceptions:
     ActivityDoesNotExist: Type[BotocoreClientError]
     ActivityLimitExceeded: Type[BotocoreClientError]
     ActivityWorkerLimitExceeded: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
-    ConflictException: Type[BotocoreClientError]
     ExecutionAlreadyExists: Type[BotocoreClientError]
     ExecutionDoesNotExist: Type[BotocoreClientError]
     ExecutionLimitExceeded: Type[BotocoreClientError]
     InvalidArn: Type[BotocoreClientError]
     InvalidDefinition: Type[BotocoreClientError]
     InvalidExecutionInput: Type[BotocoreClientError]
     InvalidLoggingConfiguration: Type[BotocoreClientError]
     InvalidName: Type[BotocoreClientError]
     InvalidOutput: Type[BotocoreClientError]
     InvalidToken: Type[BotocoreClientError]
     InvalidTracingConfiguration: Type[BotocoreClientError]
     MissingRequiredParameter: Type[BotocoreClientError]
     ResourceNotFound: Type[BotocoreClientError]
-    ServiceQuotaExceededException: Type[BotocoreClientError]
     StateMachineAlreadyExists: Type[BotocoreClientError]
     StateMachineDeleting: Type[BotocoreClientError]
     StateMachineDoesNotExist: Type[BotocoreClientError]
     StateMachineLimitExceeded: Type[BotocoreClientError]
     StateMachineTypeNotSupported: Type[BotocoreClientError]
     TaskDoesNotExist: Type[BotocoreClientError]
     TaskTimedOut: Type[BotocoreClientError]
@@ -145,83 +136,48 @@
         *,
         name: str,
         definition: str,
         roleArn: str,
         type: StateMachineTypeType = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
         tags: Sequence[TagTypeDef] = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...,
-        publish: bool = ...,
-        versionDescription: str = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...
     ) -> CreateStateMachineOutputTypeDef:
         """
         Creates a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine)
         """
-    def create_state_machine_alias(
-        self,
-        *,
-        name: str,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef],
-        description: str = ...
-    ) -> CreateStateMachineAliasOutputTypeDef:
-        """
-        Creates an [alias](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-alias.html)_ for a state machine that
-        points to one or two [versions](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-version.html)_ of the same state
-        machine.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.create_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#create_state_machine_alias)
-        """
     def delete_activity(self, *, activityArn: str) -> Dict[str, Any]:
         """
         Deletes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_activity)
         """
     def delete_state_machine(self, *, stateMachineArn: str) -> Dict[str, Any]:
         """
         Deletes a state machine.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine)
         """
-    def delete_state_machine_alias(self, *, stateMachineAliasArn: str) -> Dict[str, Any]:
-        """
-        Deletes a state machine [alias](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-alias.html)_.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_alias)
-        """
-    def delete_state_machine_version(self, *, stateMachineVersionArn: str) -> Dict[str, Any]:
-        """
-        Deletes a state machine [version](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-version.html)_.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.delete_state_machine_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#delete_state_machine_version)
-        """
     def describe_activity(self, *, activityArn: str) -> DescribeActivityOutputTypeDef:
         """
         Describes an activity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_activity)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_activity)
         """
     def describe_execution(self, *, executionArn: str) -> DescribeExecutionOutputTypeDef:
         """
-        Provides information about a state machine execution, such as the state machine
-        associated with the execution, the execution input and output, and relevant
-        execution metadata.
+        Provides all information about a state machine execution, such as the state
+        machine associated with the execution, the execution input and output, and
+        relevant execution metadata.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_execution)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_execution)
         """
     def describe_map_run(self, *, mapRunArn: str) -> DescribeMapRunOutputTypeDef:
         """
         Provides information about a Map Run's configuration, progress, and results.
@@ -233,24 +189,14 @@
         """
         Provides information about a state machine's definition, its IAM role Amazon
         Resource Name (ARN), and configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine)
         """
-    def describe_state_machine_alias(
-        self, *, stateMachineAliasArn: str
-    ) -> DescribeStateMachineAliasOutputTypeDef:
-        """
-        Returns details about a state machine [alias](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-alias.html)_.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.describe_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#describe_state_machine_alias)
-        """
     def describe_state_machine_for_execution(
         self, *, executionArn: str
     ) -> DescribeStateMachineForExecutionOutputTypeDef:
         """
         Provides information about a state machine's definition, its execution role ARN,
         and configuration.
 
@@ -324,35 +270,14 @@
     ) -> ListMapRunsOutputTypeDef:
         """
         Lists all Map Runs that were started by a given state machine execution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_map_runs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_map_runs)
         """
-    def list_state_machine_aliases(
-        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
-    ) -> ListStateMachineAliasesOutputTypeDef:
-        """
-        Lists [aliases](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
-        state-machine-alias.html)_ for a specified state machine ARN.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_aliases)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_aliases)
-        """
-    def list_state_machine_versions(
-        self, *, stateMachineArn: str, nextToken: str = ..., maxResults: int = ...
-    ) -> ListStateMachineVersionsOutputTypeDef:
-        """
-        Lists [versions](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-
-        state-machine-version.html)_ for the specified state machine Amazon Resource
-        Name (ARN).
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machine_versions)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_state_machine_versions)
-        """
     def list_state_machines(
         self, *, maxResults: int = ..., nextToken: str = ...
     ) -> ListStateMachinesOutputTypeDef:
         """
         Lists the existing state machines.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_state_machines)
@@ -361,25 +286,14 @@
     def list_tags_for_resource(self, *, resourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         List tags for a given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#list_tags_for_resource)
         """
-    def publish_state_machine_version(
-        self, *, stateMachineArn: str, revisionId: str = ..., description: str = ...
-    ) -> PublishStateMachineVersionOutputTypeDef:
-        """
-        Creates a [version](https://docs.aws.amazon.com/step-
-        functions/latest/dg/concepts-state-machine-version.html)_ from the current
-        revision of a state machine.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.publish_state_machine_version)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#publish_state_machine_version)
-        """
     def send_task_failure(
         self, *, taskToken: str, error: str = ..., cause: str = ...
     ) -> Dict[str, Any]:
         """
         Used by activity workers and task states using the
         [callback](https://docs.aws.amazon.com/step-functions/latest/dg/connect-to-
         resource.html#connect-wait-token)_ pattern to report that the task identified by
@@ -468,40 +382,23 @@
     def update_state_machine(
         self,
         *,
         stateMachineArn: str,
         definition: str = ...,
         roleArn: str = ...,
         loggingConfiguration: LoggingConfigurationTypeDef = ...,
-        tracingConfiguration: TracingConfigurationTypeDef = ...,
-        publish: bool = ...,
-        versionDescription: str = ...
+        tracingConfiguration: TracingConfigurationTypeDef = ...
     ) -> UpdateStateMachineOutputTypeDef:
         """
-        Updates an existing state machine by modifying its `definition`, `roleArn`, or
+        Updates an existing state machine by modifying its `definition` , `roleArn` , or
         `loggingConfiguration`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine)
         """
-    def update_state_machine_alias(
-        self,
-        *,
-        stateMachineAliasArn: str,
-        description: str = ...,
-        routingConfiguration: Sequence[RoutingConfigurationListItemTypeDef] = ...
-    ) -> UpdateStateMachineAliasOutputTypeDef:
-        """
-        Updates the configuration of an existing state machine
-        [alias](https://docs.aws.amazon.com/step-functions/latest/dg/concepts-state-
-        machine-alias.html)_ by modifying its `description` or `routingConfiguration`.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.update_state_machine_alias)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#update_state_machine_alias)
-        """
     @overload
     def get_paginator(
         self, operation_name: Literal["get_execution_history"]
     ) -> GetExecutionHistoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/client/#get_paginator)
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/literals.py` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,34 +152,31 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
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
@@ -258,15 +255,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -277,38 +273,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -321,15 +313,14 @@
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
@@ -348,19 +339,16 @@
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
@@ -398,15 +386,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -440,21 +427,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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
@@ -490,15 +474,14 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/literals.pyi` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/literals.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -150,34 +150,31 @@
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
-    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
-    "cloudtrail-data",
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
@@ -256,15 +253,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -275,38 +271,34 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
-    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
-    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
-    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -319,15 +311,14 @@
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
@@ -346,19 +337,16 @@
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
@@ -396,15 +384,14 @@
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
     "sagemaker-geospatial",
-    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
@@ -438,21 +425,18 @@
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
-    "tnb",
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
@@ -488,15 +472,14 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/paginator.py` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/paginator.pyi` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/type_defs.py` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -26,39 +26,34 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActivityFailedEventDetailsTypeDef",
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "RoutingConfigurationListItemTypeDef",
     "TracingConfigurationTypeDef",
     "DeleteActivityInputRequestTypeDef",
-    "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
-    "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
-    "DescribeStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
@@ -78,22 +73,17 @@
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
     "ListActivitiesInputRequestTypeDef",
     "ListExecutionsInputRequestTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
-    "ListStateMachineAliasesInputRequestTypeDef",
-    "StateMachineAliasListItemTypeDef",
-    "ListStateMachineVersionsInputRequestTypeDef",
-    "StateMachineVersionListItemTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PublishStateMachineVersionInputRequestTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
@@ -107,42 +97,34 @@
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateActivityOutputTypeDef",
-    "CreateStateMachineAliasOutputTypeDef",
     "CreateStateMachineOutputTypeDef",
     "DescribeActivityOutputTypeDef",
     "DescribeExecutionOutputTypeDef",
     "GetActivityTaskOutputTypeDef",
     "ListActivitiesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "PublishStateMachineVersionOutputTypeDef",
     "StartExecutionOutputTypeDef",
     "StartSyncExecutionOutputTypeDef",
     "StopExecutionOutputTypeDef",
-    "UpdateStateMachineAliasOutputTypeDef",
     "UpdateStateMachineOutputTypeDef",
-    "CreateStateMachineAliasInputRequestTypeDef",
-    "DescribeStateMachineAliasOutputTypeDef",
-    "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
     "ListExecutionsOutputTypeDef",
     "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
     "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
-    "ListStateMachineAliasesOutputTypeDef",
-    "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
@@ -242,22 +224,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RoutingConfigurationListItemTypeDef = TypedDict(
-    "RoutingConfigurationListItemTypeDef",
-    {
-        "stateMachineVersionArn": str,
-        "weight": int,
-    },
-)
-
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
@@ -265,35 +239,21 @@
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
-DeleteStateMachineAliasInputRequestTypeDef = TypedDict(
-    "DeleteStateMachineAliasInputRequestTypeDef",
-    {
-        "stateMachineAliasArn": str,
-    },
-)
-
 DeleteStateMachineInputRequestTypeDef = TypedDict(
     "DeleteStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
-DeleteStateMachineVersionInputRequestTypeDef = TypedDict(
-    "DeleteStateMachineVersionInputRequestTypeDef",
-    {
-        "stateMachineVersionArn": str,
-    },
-)
-
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
@@ -335,21 +295,14 @@
         "timedOut": int,
         "aborted": int,
         "total": int,
         "resultsWritten": int,
     },
 )
 
-DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
-    "DescribeStateMachineAliasInputRequestTypeDef",
-    {
-        "stateMachineAliasArn": str,
-    },
-)
-
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -390,27 +343,23 @@
 )
 _OptionalExecutionListItemTypeDef = TypedDict(
     "_OptionalExecutionListItemTypeDef",
     {
         "stopDate": datetime,
         "mapRunArn": str,
         "itemCount": int,
-        "stateMachineVersionArn": str,
-        "stateMachineAliasArn": str,
     },
     total=False,
 )
 
-
 class ExecutionListItemTypeDef(
     _RequiredExecutionListItemTypeDef, _OptionalExecutionListItemTypeDef
 ):
     pass
 
-
 ExecutionTimedOutEventDetailsTypeDef = TypedDict(
     "ExecutionTimedOutEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -426,21 +375,19 @@
     "_OptionalGetActivityTaskInputRequestTypeDef",
     {
         "workerName": str,
     },
     total=False,
 )
 
-
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -460,21 +407,19 @@
         "reverseOrder": bool,
         "nextToken": str,
         "includeExecutionData": bool,
     },
     total=False,
 )
 
-
 class GetExecutionHistoryInputRequestTypeDef(
     _RequiredGetExecutionHistoryInputRequestTypeDef, _OptionalGetExecutionHistoryInputRequestTypeDef
 ):
     pass
 
-
 LambdaFunctionFailedEventDetailsTypeDef = TypedDict(
     "LambdaFunctionFailedEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -553,21 +498,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskFailedEventDetailsTypeDef(
     _RequiredTaskFailedEventDetailsTypeDef, _OptionalTaskFailedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskStartFailedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskStartFailedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -576,21 +519,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskStartFailedEventDetailsTypeDef(
     _RequiredTaskStartFailedEventDetailsTypeDef, _OptionalTaskStartFailedEventDetailsTypeDef
 ):
     pass
 
-
 TaskStartedEventDetailsTypeDef = TypedDict(
     "TaskStartedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -607,21 +548,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskSubmitFailedEventDetailsTypeDef(
     _RequiredTaskSubmitFailedEventDetailsTypeDef, _OptionalTaskSubmitFailedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskTimedOutEventDetailsTypeDef = TypedDict(
     "_RequiredTaskTimedOutEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -630,21 +569,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class TaskTimedOutEventDetailsTypeDef(
     _RequiredTaskTimedOutEventDetailsTypeDef, _OptionalTaskTimedOutEventDetailsTypeDef
 ):
     pass
 
-
 TaskCredentialsTypeDef = TypedDict(
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
@@ -681,21 +618,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListMapRunsInputRequestTypeDef(
     _RequiredListMapRunsInputRequestTypeDef, _OptionalListMapRunsInputRequestTypeDef
 ):
     pass
 
-
 _RequiredMapRunListItemTypeDef = TypedDict(
     "_RequiredMapRunListItemTypeDef",
     {
         "executionArn": str,
         "mapRunArn": str,
         "stateMachineArn": str,
         "startDate": datetime,
@@ -705,81 +640,17 @@
     "_OptionalMapRunListItemTypeDef",
     {
         "stopDate": datetime,
     },
     total=False,
 )
 
-
 class MapRunListItemTypeDef(_RequiredMapRunListItemTypeDef, _OptionalMapRunListItemTypeDef):
     pass
 
-
-_RequiredListStateMachineAliasesInputRequestTypeDef = TypedDict(
-    "_RequiredListStateMachineAliasesInputRequestTypeDef",
-    {
-        "stateMachineArn": str,
-    },
-)
-_OptionalListStateMachineAliasesInputRequestTypeDef = TypedDict(
-    "_OptionalListStateMachineAliasesInputRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListStateMachineAliasesInputRequestTypeDef(
-    _RequiredListStateMachineAliasesInputRequestTypeDef,
-    _OptionalListStateMachineAliasesInputRequestTypeDef,
-):
-    pass
-
-
-StateMachineAliasListItemTypeDef = TypedDict(
-    "StateMachineAliasListItemTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-    },
-)
-
-_RequiredListStateMachineVersionsInputRequestTypeDef = TypedDict(
-    "_RequiredListStateMachineVersionsInputRequestTypeDef",
-    {
-        "stateMachineArn": str,
-    },
-)
-_OptionalListStateMachineVersionsInputRequestTypeDef = TypedDict(
-    "_OptionalListStateMachineVersionsInputRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-
-class ListStateMachineVersionsInputRequestTypeDef(
-    _RequiredListStateMachineVersionsInputRequestTypeDef,
-    _OptionalListStateMachineVersionsInputRequestTypeDef,
-):
-    pass
-
-
-StateMachineVersionListItemTypeDef = TypedDict(
-    "StateMachineVersionListItemTypeDef",
-    {
-        "stateMachineVersionArn": str,
-        "creationDate": datetime,
-    },
-)
-
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -798,37 +669,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
-    "_RequiredPublishStateMachineVersionInputRequestTypeDef",
-    {
-        "stateMachineArn": str,
-    },
-)
-_OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
-    "_OptionalPublishStateMachineVersionInputRequestTypeDef",
-    {
-        "revisionId": str,
-        "description": str,
-    },
-    total=False,
-)
-
-
-class PublishStateMachineVersionInputRequestTypeDef(
-    _RequiredPublishStateMachineVersionInputRequestTypeDef,
-    _OptionalPublishStateMachineVersionInputRequestTypeDef,
-):
-    pass
-
-
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -836,21 +684,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class SendTaskFailureInputRequestTypeDef(
     _RequiredSendTaskFailureInputRequestTypeDef, _OptionalSendTaskFailureInputRequestTypeDef
 ):
     pass
 
-
 SendTaskHeartbeatInputRequestTypeDef = TypedDict(
     "SendTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 
@@ -874,21 +720,19 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
-
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
-
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalStartSyncExecutionInputRequestTypeDef = TypedDict(
@@ -897,21 +741,19 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
-
 class StartSyncExecutionInputRequestTypeDef(
     _RequiredStartSyncExecutionInputRequestTypeDef, _OptionalStartSyncExecutionInputRequestTypeDef
 ):
     pass
 
-
 _RequiredStopExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalStopExecutionInputRequestTypeDef = TypedDict(
@@ -919,21 +761,19 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
-
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -950,21 +790,19 @@
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
     },
     total=False,
 )
 
-
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
-
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalActivityScheduledEventDetailsTypeDef = TypedDict(
@@ -974,21 +812,19 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
     },
     total=False,
 )
 
-
 class ActivityScheduledEventDetailsTypeDef(
     _RequiredActivityScheduledEventDetailsTypeDef, _OptionalActivityScheduledEventDetailsTypeDef
 ):
     pass
 
-
 ActivitySucceededEventDetailsTypeDef = TypedDict(
     "ActivitySucceededEventDetailsTypeDef",
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
@@ -996,16 +832,14 @@
 
 ExecutionStartedEventDetailsTypeDef = TypedDict(
     "ExecutionStartedEventDetailsTypeDef",
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "roleArn": str,
-        "stateMachineAliasArn": str,
-        "stateMachineVersionArn": str,
     },
     total=False,
 )
 
 ExecutionSucceededEventDetailsTypeDef = TypedDict(
     "ExecutionSucceededEventDetailsTypeDef",
     {
@@ -1035,21 +869,19 @@
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class StateEnteredEventDetailsTypeDef(
     _RequiredStateEnteredEventDetailsTypeDef, _OptionalStateEnteredEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredStateExitedEventDetailsTypeDef = TypedDict(
     "_RequiredStateExitedEventDetailsTypeDef",
     {
         "name": str,
     },
 )
 _OptionalStateExitedEventDetailsTypeDef = TypedDict(
@@ -1057,21 +889,19 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class StateExitedEventDetailsTypeDef(
     _RequiredStateExitedEventDetailsTypeDef, _OptionalStateExitedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskSubmittedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSubmittedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -1080,21 +910,19 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class TaskSubmittedEventDetailsTypeDef(
     _RequiredTaskSubmittedEventDetailsTypeDef, _OptionalTaskSubmittedEventDetailsTypeDef
 ):
     pass
 
-
 _RequiredTaskSucceededEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSucceededEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -1103,21 +931,19 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
-
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
-
 LogDestinationTypeDef = TypedDict(
     "LogDestinationTypeDef",
     {
         "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
@@ -1132,21 +958,19 @@
     "_OptionalCreateActivityInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateActivityInputRequestTypeDef(
     _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1156,29 +980,19 @@
     {
         "activityArn": str,
         "creationDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStateMachineAliasOutputTypeDef = TypedDict(
-    "CreateStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateStateMachineOutputTypeDef = TypedDict(
     "CreateStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
         "creationDate": datetime,
-        "stateMachineVersionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeActivityOutputTypeDef = TypedDict(
     "DescribeActivityOutputTypeDef",
     {
@@ -1202,16 +1016,14 @@
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
-        "stateMachineVersionArn": str,
-        "stateMachineAliasArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetActivityTaskOutputTypeDef = TypedDict(
     "GetActivityTaskOutputTypeDef",
     {
@@ -1234,23 +1046,14 @@
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PublishStateMachineVersionOutputTypeDef = TypedDict(
-    "PublishStateMachineVersionOutputTypeDef",
-    {
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartExecutionOutputTypeDef = TypedDict(
     "StartExecutionOutputTypeDef",
     {
         "executionArn": str,
         "startDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1281,91 +1084,22 @@
     "StopExecutionOutputTypeDef",
     {
         "stopDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateStateMachineAliasOutputTypeDef = TypedDict(
-    "UpdateStateMachineAliasOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateStateMachineOutputTypeDef = TypedDict(
     "UpdateStateMachineOutputTypeDef",
     {
         "updateDate": datetime,
-        "revisionId": str,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineAliasInputRequestTypeDef",
-    {
-        "name": str,
-        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
-    },
-)
-_OptionalCreateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineAliasInputRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-
-class CreateStateMachineAliasInputRequestTypeDef(
-    _RequiredCreateStateMachineAliasInputRequestTypeDef,
-    _OptionalCreateStateMachineAliasInputRequestTypeDef,
-):
-    pass
-
-
-DescribeStateMachineAliasOutputTypeDef = TypedDict(
-    "DescribeStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "name": str,
-        "description": str,
-        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
-        "creationDate": datetime,
-        "updateDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
-    {
-        "stateMachineAliasArn": str,
-    },
-)
-_OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateStateMachineAliasInputRequestTypeDef",
-    {
-        "description": str,
-        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateStateMachineAliasInputRequestTypeDef(
-    _RequiredUpdateStateMachineAliasInputRequestTypeDef,
-    _OptionalUpdateStateMachineAliasInputRequestTypeDef,
-):
-    pass
-
-
 DescribeMapRunOutputTypeDef = TypedDict(
     "DescribeMapRunOutputTypeDef",
     {
         "mapRunArn": str,
         "executionArn": str,
         "status": MapRunStatusType,
         "startDate": datetime,
@@ -1400,22 +1134,20 @@
         "reverseOrder": bool,
         "includeExecutionData": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
     _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
 ):
     pass
 
-
 ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
     "ListActivitiesInputListActivitiesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1441,22 +1173,20 @@
     "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListMapRunsInputListMapRunsPaginateTypeDef(
     _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
     _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
 ):
     pass
 
-
 ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1474,22 +1204,20 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class LambdaFunctionScheduledEventDetailsTypeDef(
     _RequiredLambdaFunctionScheduledEventDetailsTypeDef,
     _OptionalLambdaFunctionScheduledEventDetailsTypeDef,
 ):
     pass
 
-
 _RequiredTaskScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredTaskScheduledEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
         "region": str,
         "parameters": str,
@@ -1501,48 +1229,28 @@
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
-
 class TaskScheduledEventDetailsTypeDef(
     _RequiredTaskScheduledEventDetailsTypeDef, _OptionalTaskScheduledEventDetailsTypeDef
 ):
     pass
 
-
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListStateMachineAliasesOutputTypeDef = TypedDict(
-    "ListStateMachineAliasesOutputTypeDef",
-    {
-        "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStateMachineVersionsOutputTypeDef = TypedDict(
-    "ListStateMachineVersionsOutputTypeDef",
-    {
-        "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1604,19 +1312,17 @@
         "stateExitedEventDetails": StateExitedEventDetailsTypeDef,
         "mapRunStartedEventDetails": MapRunStartedEventDetailsTypeDef,
         "mapRunFailedEventDetails": MapRunFailedEventDetailsTypeDef,
     },
     total=False,
 )
 
-
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
-
 _RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineInputRequestTypeDef",
     {
         "name": str,
         "definition": str,
         "roleArn": str,
     },
@@ -1624,40 +1330,35 @@
 _OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalCreateStateMachineInputRequestTypeDef",
     {
         "type": StateMachineTypeType,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
     },
     total=False,
 )
 
-
 class CreateStateMachineInputRequestTypeDef(
     _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
 ):
     pass
 
-
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
-        "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
@@ -1667,16 +1368,14 @@
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
-        "revisionId": str,
-        "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
@@ -1686,27 +1385,23 @@
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalUpdateStateMachineInputRequestTypeDef",
     {
         "definition": str,
         "roleArn": str,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
     },
     total=False,
 )
 
-
 class UpdateStateMachineInputRequestTypeDef(
     _RequiredUpdateStateMachineInputRequestTypeDef, _OptionalUpdateStateMachineInputRequestTypeDef
 ):
     pass
 
-
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions/type_defs.pyi` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions/type_defs.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,38 +26,35 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActivityFailedEventDetailsTypeDef",
     "ActivityListItemTypeDef",
     "ActivityScheduleFailedEventDetailsTypeDef",
     "HistoryEventExecutionDataDetailsTypeDef",
     "ActivityStartedEventDetailsTypeDef",
     "ActivityTimedOutEventDetailsTypeDef",
     "BillingDetailsTypeDef",
     "CloudWatchEventsExecutionDataDetailsTypeDef",
     "CloudWatchLogsLogGroupTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
-    "RoutingConfigurationListItemTypeDef",
     "TracingConfigurationTypeDef",
     "DeleteActivityInputRequestTypeDef",
-    "DeleteStateMachineAliasInputRequestTypeDef",
     "DeleteStateMachineInputRequestTypeDef",
-    "DeleteStateMachineVersionInputRequestTypeDef",
     "DescribeActivityInputRequestTypeDef",
     "DescribeExecutionInputRequestTypeDef",
     "DescribeMapRunInputRequestTypeDef",
     "MapRunExecutionCountsTypeDef",
     "MapRunItemCountsTypeDef",
-    "DescribeStateMachineAliasInputRequestTypeDef",
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     "DescribeStateMachineInputRequestTypeDef",
     "ExecutionAbortedEventDetailsTypeDef",
     "ExecutionFailedEventDetailsTypeDef",
     "ExecutionListItemTypeDef",
     "ExecutionTimedOutEventDetailsTypeDef",
     "GetActivityTaskInputRequestTypeDef",
@@ -77,22 +74,17 @@
     "TaskSubmitFailedEventDetailsTypeDef",
     "TaskTimedOutEventDetailsTypeDef",
     "TaskCredentialsTypeDef",
     "ListActivitiesInputRequestTypeDef",
     "ListExecutionsInputRequestTypeDef",
     "ListMapRunsInputRequestTypeDef",
     "MapRunListItemTypeDef",
-    "ListStateMachineAliasesInputRequestTypeDef",
-    "StateMachineAliasListItemTypeDef",
-    "ListStateMachineVersionsInputRequestTypeDef",
-    "StateMachineVersionListItemTypeDef",
     "ListStateMachinesInputRequestTypeDef",
     "StateMachineListItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "PublishStateMachineVersionInputRequestTypeDef",
     "SendTaskFailureInputRequestTypeDef",
     "SendTaskHeartbeatInputRequestTypeDef",
     "SendTaskSuccessInputRequestTypeDef",
     "StartExecutionInputRequestTypeDef",
     "StartSyncExecutionInputRequestTypeDef",
     "StopExecutionInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
@@ -106,42 +98,34 @@
     "StateExitedEventDetailsTypeDef",
     "TaskSubmittedEventDetailsTypeDef",
     "TaskSucceededEventDetailsTypeDef",
     "LogDestinationTypeDef",
     "CreateActivityInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateActivityOutputTypeDef",
-    "CreateStateMachineAliasOutputTypeDef",
     "CreateStateMachineOutputTypeDef",
     "DescribeActivityOutputTypeDef",
     "DescribeExecutionOutputTypeDef",
     "GetActivityTaskOutputTypeDef",
     "ListActivitiesOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
-    "PublishStateMachineVersionOutputTypeDef",
     "StartExecutionOutputTypeDef",
     "StartSyncExecutionOutputTypeDef",
     "StopExecutionOutputTypeDef",
-    "UpdateStateMachineAliasOutputTypeDef",
     "UpdateStateMachineOutputTypeDef",
-    "CreateStateMachineAliasInputRequestTypeDef",
-    "DescribeStateMachineAliasOutputTypeDef",
-    "UpdateStateMachineAliasInputRequestTypeDef",
     "DescribeMapRunOutputTypeDef",
     "ListExecutionsOutputTypeDef",
     "GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef",
     "ListActivitiesInputListActivitiesPaginateTypeDef",
     "ListExecutionsInputListExecutionsPaginateTypeDef",
     "ListMapRunsInputListMapRunsPaginateTypeDef",
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     "LambdaFunctionScheduledEventDetailsTypeDef",
     "TaskScheduledEventDetailsTypeDef",
     "ListMapRunsOutputTypeDef",
-    "ListStateMachineAliasesOutputTypeDef",
-    "ListStateMachineVersionsOutputTypeDef",
     "ListStateMachinesOutputTypeDef",
     "LoggingConfigurationTypeDef",
     "HistoryEventTypeDef",
     "CreateStateMachineInputRequestTypeDef",
     "DescribeStateMachineForExecutionOutputTypeDef",
     "DescribeStateMachineOutputTypeDef",
     "UpdateStateMachineInputRequestTypeDef",
@@ -241,22 +225,14 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-RoutingConfigurationListItemTypeDef = TypedDict(
-    "RoutingConfigurationListItemTypeDef",
-    {
-        "stateMachineVersionArn": str,
-        "weight": int,
-    },
-)
-
 TracingConfigurationTypeDef = TypedDict(
     "TracingConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
@@ -264,35 +240,21 @@
 DeleteActivityInputRequestTypeDef = TypedDict(
     "DeleteActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
-DeleteStateMachineAliasInputRequestTypeDef = TypedDict(
-    "DeleteStateMachineAliasInputRequestTypeDef",
-    {
-        "stateMachineAliasArn": str,
-    },
-)
-
 DeleteStateMachineInputRequestTypeDef = TypedDict(
     "DeleteStateMachineInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 
-DeleteStateMachineVersionInputRequestTypeDef = TypedDict(
-    "DeleteStateMachineVersionInputRequestTypeDef",
-    {
-        "stateMachineVersionArn": str,
-    },
-)
-
 DescribeActivityInputRequestTypeDef = TypedDict(
     "DescribeActivityInputRequestTypeDef",
     {
         "activityArn": str,
     },
 )
 
@@ -334,21 +296,14 @@
         "timedOut": int,
         "aborted": int,
         "total": int,
         "resultsWritten": int,
     },
 )
 
-DescribeStateMachineAliasInputRequestTypeDef = TypedDict(
-    "DescribeStateMachineAliasInputRequestTypeDef",
-    {
-        "stateMachineAliasArn": str,
-    },
-)
-
 DescribeStateMachineForExecutionInputRequestTypeDef = TypedDict(
     "DescribeStateMachineForExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 
@@ -389,25 +344,25 @@
 )
 _OptionalExecutionListItemTypeDef = TypedDict(
     "_OptionalExecutionListItemTypeDef",
     {
         "stopDate": datetime,
         "mapRunArn": str,
         "itemCount": int,
-        "stateMachineVersionArn": str,
-        "stateMachineAliasArn": str,
     },
     total=False,
 )
 
+
 class ExecutionListItemTypeDef(
     _RequiredExecutionListItemTypeDef, _OptionalExecutionListItemTypeDef
 ):
     pass
 
+
 ExecutionTimedOutEventDetailsTypeDef = TypedDict(
     "ExecutionTimedOutEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -423,19 +378,21 @@
     "_OptionalGetActivityTaskInputRequestTypeDef",
     {
         "workerName": str,
     },
     total=False,
 )
 
+
 class GetActivityTaskInputRequestTypeDef(
     _RequiredGetActivityTaskInputRequestTypeDef, _OptionalGetActivityTaskInputRequestTypeDef
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -455,19 +412,21 @@
         "reverseOrder": bool,
         "nextToken": str,
         "includeExecutionData": bool,
     },
     total=False,
 )
 
+
 class GetExecutionHistoryInputRequestTypeDef(
     _RequiredGetExecutionHistoryInputRequestTypeDef, _OptionalGetExecutionHistoryInputRequestTypeDef
 ):
     pass
 
+
 LambdaFunctionFailedEventDetailsTypeDef = TypedDict(
     "LambdaFunctionFailedEventDetailsTypeDef",
     {
         "error": str,
         "cause": str,
     },
     total=False,
@@ -546,19 +505,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskFailedEventDetailsTypeDef(
     _RequiredTaskFailedEventDetailsTypeDef, _OptionalTaskFailedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskStartFailedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskStartFailedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -567,19 +528,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskStartFailedEventDetailsTypeDef(
     _RequiredTaskStartFailedEventDetailsTypeDef, _OptionalTaskStartFailedEventDetailsTypeDef
 ):
     pass
 
+
 TaskStartedEventDetailsTypeDef = TypedDict(
     "TaskStartedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -596,19 +559,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskSubmitFailedEventDetailsTypeDef(
     _RequiredTaskSubmitFailedEventDetailsTypeDef, _OptionalTaskSubmitFailedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskTimedOutEventDetailsTypeDef = TypedDict(
     "_RequiredTaskTimedOutEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -617,19 +582,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class TaskTimedOutEventDetailsTypeDef(
     _RequiredTaskTimedOutEventDetailsTypeDef, _OptionalTaskTimedOutEventDetailsTypeDef
 ):
     pass
 
+
 TaskCredentialsTypeDef = TypedDict(
     "TaskCredentialsTypeDef",
     {
         "roleArn": str,
     },
     total=False,
 )
@@ -666,19 +633,21 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListMapRunsInputRequestTypeDef(
     _RequiredListMapRunsInputRequestTypeDef, _OptionalListMapRunsInputRequestTypeDef
 ):
     pass
 
+
 _RequiredMapRunListItemTypeDef = TypedDict(
     "_RequiredMapRunListItemTypeDef",
     {
         "executionArn": str,
         "mapRunArn": str,
         "stateMachineArn": str,
         "startDate": datetime,
@@ -688,74 +657,18 @@
     "_OptionalMapRunListItemTypeDef",
     {
         "stopDate": datetime,
     },
     total=False,
 )
 
-class MapRunListItemTypeDef(_RequiredMapRunListItemTypeDef, _OptionalMapRunListItemTypeDef):
-    pass
-
-_RequiredListStateMachineAliasesInputRequestTypeDef = TypedDict(
-    "_RequiredListStateMachineAliasesInputRequestTypeDef",
-    {
-        "stateMachineArn": str,
-    },
-)
-_OptionalListStateMachineAliasesInputRequestTypeDef = TypedDict(
-    "_OptionalListStateMachineAliasesInputRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListStateMachineAliasesInputRequestTypeDef(
-    _RequiredListStateMachineAliasesInputRequestTypeDef,
-    _OptionalListStateMachineAliasesInputRequestTypeDef,
-):
-    pass
-
-StateMachineAliasListItemTypeDef = TypedDict(
-    "StateMachineAliasListItemTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-    },
-)
 
-_RequiredListStateMachineVersionsInputRequestTypeDef = TypedDict(
-    "_RequiredListStateMachineVersionsInputRequestTypeDef",
-    {
-        "stateMachineArn": str,
-    },
-)
-_OptionalListStateMachineVersionsInputRequestTypeDef = TypedDict(
-    "_OptionalListStateMachineVersionsInputRequestTypeDef",
-    {
-        "nextToken": str,
-        "maxResults": int,
-    },
-    total=False,
-)
-
-class ListStateMachineVersionsInputRequestTypeDef(
-    _RequiredListStateMachineVersionsInputRequestTypeDef,
-    _OptionalListStateMachineVersionsInputRequestTypeDef,
-):
+class MapRunListItemTypeDef(_RequiredMapRunListItemTypeDef, _OptionalMapRunListItemTypeDef):
     pass
 
-StateMachineVersionListItemTypeDef = TypedDict(
-    "StateMachineVersionListItemTypeDef",
-    {
-        "stateMachineVersionArn": str,
-        "creationDate": datetime,
-    },
-)
 
 ListStateMachinesInputRequestTypeDef = TypedDict(
     "ListStateMachinesInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
@@ -775,35 +688,14 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredPublishStateMachineVersionInputRequestTypeDef = TypedDict(
-    "_RequiredPublishStateMachineVersionInputRequestTypeDef",
-    {
-        "stateMachineArn": str,
-    },
-)
-_OptionalPublishStateMachineVersionInputRequestTypeDef = TypedDict(
-    "_OptionalPublishStateMachineVersionInputRequestTypeDef",
-    {
-        "revisionId": str,
-        "description": str,
-    },
-    total=False,
-)
-
-class PublishStateMachineVersionInputRequestTypeDef(
-    _RequiredPublishStateMachineVersionInputRequestTypeDef,
-    _OptionalPublishStateMachineVersionInputRequestTypeDef,
-):
-    pass
-
 _RequiredSendTaskFailureInputRequestTypeDef = TypedDict(
     "_RequiredSendTaskFailureInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 _OptionalSendTaskFailureInputRequestTypeDef = TypedDict(
@@ -811,19 +703,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class SendTaskFailureInputRequestTypeDef(
     _RequiredSendTaskFailureInputRequestTypeDef, _OptionalSendTaskFailureInputRequestTypeDef
 ):
     pass
 
+
 SendTaskHeartbeatInputRequestTypeDef = TypedDict(
     "SendTaskHeartbeatInputRequestTypeDef",
     {
         "taskToken": str,
     },
 )
 
@@ -847,19 +741,21 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
+
 class StartExecutionInputRequestTypeDef(
     _RequiredStartExecutionInputRequestTypeDef, _OptionalStartExecutionInputRequestTypeDef
 ):
     pass
 
+
 _RequiredStartSyncExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStartSyncExecutionInputRequestTypeDef",
     {
         "stateMachineArn": str,
     },
 )
 _OptionalStartSyncExecutionInputRequestTypeDef = TypedDict(
@@ -868,19 +764,21 @@
         "name": str,
         "input": str,
         "traceHeader": str,
     },
     total=False,
 )
 
+
 class StartSyncExecutionInputRequestTypeDef(
     _RequiredStartSyncExecutionInputRequestTypeDef, _OptionalStartSyncExecutionInputRequestTypeDef
 ):
     pass
 
+
 _RequiredStopExecutionInputRequestTypeDef = TypedDict(
     "_RequiredStopExecutionInputRequestTypeDef",
     {
         "executionArn": str,
     },
 )
 _OptionalStopExecutionInputRequestTypeDef = TypedDict(
@@ -888,19 +786,21 @@
     {
         "error": str,
         "cause": str,
     },
     total=False,
 )
 
+
 class StopExecutionInputRequestTypeDef(
     _RequiredStopExecutionInputRequestTypeDef, _OptionalStopExecutionInputRequestTypeDef
 ):
     pass
 
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -917,19 +817,21 @@
         "maxConcurrency": int,
         "toleratedFailurePercentage": float,
         "toleratedFailureCount": int,
     },
     total=False,
 )
 
+
 class UpdateMapRunInputRequestTypeDef(
     _RequiredUpdateMapRunInputRequestTypeDef, _OptionalUpdateMapRunInputRequestTypeDef
 ):
     pass
 
+
 _RequiredActivityScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredActivityScheduledEventDetailsTypeDef",
     {
         "resource": str,
     },
 )
 _OptionalActivityScheduledEventDetailsTypeDef = TypedDict(
@@ -939,19 +841,21 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
     },
     total=False,
 )
 
+
 class ActivityScheduledEventDetailsTypeDef(
     _RequiredActivityScheduledEventDetailsTypeDef, _OptionalActivityScheduledEventDetailsTypeDef
 ):
     pass
 
+
 ActivitySucceededEventDetailsTypeDef = TypedDict(
     "ActivitySucceededEventDetailsTypeDef",
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
@@ -959,16 +863,14 @@
 
 ExecutionStartedEventDetailsTypeDef = TypedDict(
     "ExecutionStartedEventDetailsTypeDef",
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "roleArn": str,
-        "stateMachineAliasArn": str,
-        "stateMachineVersionArn": str,
     },
     total=False,
 )
 
 ExecutionSucceededEventDetailsTypeDef = TypedDict(
     "ExecutionSucceededEventDetailsTypeDef",
     {
@@ -998,19 +900,21 @@
     {
         "input": str,
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class StateEnteredEventDetailsTypeDef(
     _RequiredStateEnteredEventDetailsTypeDef, _OptionalStateEnteredEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredStateExitedEventDetailsTypeDef = TypedDict(
     "_RequiredStateExitedEventDetailsTypeDef",
     {
         "name": str,
     },
 )
 _OptionalStateExitedEventDetailsTypeDef = TypedDict(
@@ -1018,19 +922,21 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class StateExitedEventDetailsTypeDef(
     _RequiredStateExitedEventDetailsTypeDef, _OptionalStateExitedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskSubmittedEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSubmittedEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -1039,19 +945,21 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class TaskSubmittedEventDetailsTypeDef(
     _RequiredTaskSubmittedEventDetailsTypeDef, _OptionalTaskSubmittedEventDetailsTypeDef
 ):
     pass
 
+
 _RequiredTaskSucceededEventDetailsTypeDef = TypedDict(
     "_RequiredTaskSucceededEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
     },
 )
@@ -1060,19 +968,21 @@
     {
         "output": str,
         "outputDetails": HistoryEventExecutionDataDetailsTypeDef,
     },
     total=False,
 )
 
+
 class TaskSucceededEventDetailsTypeDef(
     _RequiredTaskSucceededEventDetailsTypeDef, _OptionalTaskSucceededEventDetailsTypeDef
 ):
     pass
 
+
 LogDestinationTypeDef = TypedDict(
     "LogDestinationTypeDef",
     {
         "cloudWatchLogsLogGroup": CloudWatchLogsLogGroupTypeDef,
     },
     total=False,
 )
@@ -1087,19 +997,21 @@
     "_OptionalCreateActivityInputRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateActivityInputRequestTypeDef(
     _RequiredCreateActivityInputRequestTypeDef, _OptionalCreateActivityInputRequestTypeDef
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -1109,29 +1021,19 @@
     {
         "activityArn": str,
         "creationDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateStateMachineAliasOutputTypeDef = TypedDict(
-    "CreateStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "creationDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateStateMachineOutputTypeDef = TypedDict(
     "CreateStateMachineOutputTypeDef",
     {
         "stateMachineArn": str,
         "creationDate": datetime,
-        "stateMachineVersionArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeActivityOutputTypeDef = TypedDict(
     "DescribeActivityOutputTypeDef",
     {
@@ -1155,16 +1057,14 @@
         "inputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "output": str,
         "outputDetails": CloudWatchEventsExecutionDataDetailsTypeDef,
         "traceHeader": str,
         "mapRunArn": str,
         "error": str,
         "cause": str,
-        "stateMachineVersionArn": str,
-        "stateMachineAliasArn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetActivityTaskOutputTypeDef = TypedDict(
     "GetActivityTaskOutputTypeDef",
     {
@@ -1187,23 +1087,14 @@
     "ListTagsForResourceOutputTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PublishStateMachineVersionOutputTypeDef = TypedDict(
-    "PublishStateMachineVersionOutputTypeDef",
-    {
-        "creationDate": datetime,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 StartExecutionOutputTypeDef = TypedDict(
     "StartExecutionOutputTypeDef",
     {
         "executionArn": str,
         "startDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1234,87 +1125,22 @@
     "StopExecutionOutputTypeDef",
     {
         "stopDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateStateMachineAliasOutputTypeDef = TypedDict(
-    "UpdateStateMachineAliasOutputTypeDef",
-    {
-        "updateDate": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateStateMachineOutputTypeDef = TypedDict(
     "UpdateStateMachineOutputTypeDef",
     {
         "updateDate": datetime,
-        "revisionId": str,
-        "stateMachineVersionArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_RequiredCreateStateMachineAliasInputRequestTypeDef",
-    {
-        "name": str,
-        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
-    },
-)
-_OptionalCreateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_OptionalCreateStateMachineAliasInputRequestTypeDef",
-    {
-        "description": str,
-    },
-    total=False,
-)
-
-class CreateStateMachineAliasInputRequestTypeDef(
-    _RequiredCreateStateMachineAliasInputRequestTypeDef,
-    _OptionalCreateStateMachineAliasInputRequestTypeDef,
-):
-    pass
-
-DescribeStateMachineAliasOutputTypeDef = TypedDict(
-    "DescribeStateMachineAliasOutputTypeDef",
-    {
-        "stateMachineAliasArn": str,
-        "name": str,
-        "description": str,
-        "routingConfiguration": List[RoutingConfigurationListItemTypeDef],
-        "creationDate": datetime,
-        "updateDate": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateStateMachineAliasInputRequestTypeDef",
-    {
-        "stateMachineAliasArn": str,
-    },
-)
-_OptionalUpdateStateMachineAliasInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateStateMachineAliasInputRequestTypeDef",
-    {
-        "description": str,
-        "routingConfiguration": Sequence[RoutingConfigurationListItemTypeDef],
-    },
-    total=False,
-)
-
-class UpdateStateMachineAliasInputRequestTypeDef(
-    _RequiredUpdateStateMachineAliasInputRequestTypeDef,
-    _OptionalUpdateStateMachineAliasInputRequestTypeDef,
-):
-    pass
-
 DescribeMapRunOutputTypeDef = TypedDict(
     "DescribeMapRunOutputTypeDef",
     {
         "mapRunArn": str,
         "executionArn": str,
         "status": MapRunStatusType,
         "startDate": datetime,
@@ -1349,20 +1175,22 @@
         "reverseOrder": bool,
         "includeExecutionData": bool,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef(
     _RequiredGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     _OptionalGetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
 ):
     pass
 
+
 ListActivitiesInputListActivitiesPaginateTypeDef = TypedDict(
     "ListActivitiesInputListActivitiesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1388,20 +1216,22 @@
     "_OptionalListMapRunsInputListMapRunsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListMapRunsInputListMapRunsPaginateTypeDef(
     _RequiredListMapRunsInputListMapRunsPaginateTypeDef,
     _OptionalListMapRunsInputListMapRunsPaginateTypeDef,
 ):
     pass
 
+
 ListStateMachinesInputListStateMachinesPaginateTypeDef = TypedDict(
     "ListStateMachinesInputListStateMachinesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1419,20 +1249,22 @@
         "inputDetails": HistoryEventExecutionDataDetailsTypeDef,
         "timeoutInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class LambdaFunctionScheduledEventDetailsTypeDef(
     _RequiredLambdaFunctionScheduledEventDetailsTypeDef,
     _OptionalLambdaFunctionScheduledEventDetailsTypeDef,
 ):
     pass
 
+
 _RequiredTaskScheduledEventDetailsTypeDef = TypedDict(
     "_RequiredTaskScheduledEventDetailsTypeDef",
     {
         "resourceType": str,
         "resource": str,
         "region": str,
         "parameters": str,
@@ -1444,46 +1276,30 @@
         "timeoutInSeconds": int,
         "heartbeatInSeconds": int,
         "taskCredentials": TaskCredentialsTypeDef,
     },
     total=False,
 )
 
+
 class TaskScheduledEventDetailsTypeDef(
     _RequiredTaskScheduledEventDetailsTypeDef, _OptionalTaskScheduledEventDetailsTypeDef
 ):
     pass
 
+
 ListMapRunsOutputTypeDef = TypedDict(
     "ListMapRunsOutputTypeDef",
     {
         "mapRuns": List[MapRunListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListStateMachineAliasesOutputTypeDef = TypedDict(
-    "ListStateMachineAliasesOutputTypeDef",
-    {
-        "stateMachineAliases": List[StateMachineAliasListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListStateMachineVersionsOutputTypeDef = TypedDict(
-    "ListStateMachineVersionsOutputTypeDef",
-    {
-        "stateMachineVersions": List[StateMachineVersionListItemTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListStateMachinesOutputTypeDef = TypedDict(
     "ListStateMachinesOutputTypeDef",
     {
         "stateMachines": List[StateMachineListItemTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1545,17 +1361,19 @@
         "stateExitedEventDetails": StateExitedEventDetailsTypeDef,
         "mapRunStartedEventDetails": MapRunStartedEventDetailsTypeDef,
         "mapRunFailedEventDetails": MapRunFailedEventDetailsTypeDef,
     },
     total=False,
 )
 
+
 class HistoryEventTypeDef(_RequiredHistoryEventTypeDef, _OptionalHistoryEventTypeDef):
     pass
 
+
 _RequiredCreateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredCreateStateMachineInputRequestTypeDef",
     {
         "name": str,
         "definition": str,
         "roleArn": str,
     },
@@ -1563,38 +1381,37 @@
 _OptionalCreateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalCreateStateMachineInputRequestTypeDef",
     {
         "type": StateMachineTypeType,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tags": Sequence[TagTypeDef],
         "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
     },
     total=False,
 )
 
+
 class CreateStateMachineInputRequestTypeDef(
     _RequiredCreateStateMachineInputRequestTypeDef, _OptionalCreateStateMachineInputRequestTypeDef
 ):
     pass
 
+
 DescribeStateMachineForExecutionOutputTypeDef = TypedDict(
     "DescribeStateMachineForExecutionOutputTypeDef",
     {
         "stateMachineArn": str,
         "name": str,
         "definition": str,
         "roleArn": str,
         "updateDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "mapRunArn": str,
         "label": str,
-        "revisionId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStateMachineOutputTypeDef = TypedDict(
     "DescribeStateMachineOutputTypeDef",
     {
@@ -1604,16 +1421,14 @@
         "definition": str,
         "roleArn": str,
         "type": StateMachineTypeType,
         "creationDate": datetime,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
         "label": str,
-        "revisionId": str,
-        "description": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_RequiredUpdateStateMachineInputRequestTypeDef",
     {
@@ -1623,25 +1438,25 @@
 _OptionalUpdateStateMachineInputRequestTypeDef = TypedDict(
     "_OptionalUpdateStateMachineInputRequestTypeDef",
     {
         "definition": str,
         "roleArn": str,
         "loggingConfiguration": LoggingConfigurationTypeDef,
         "tracingConfiguration": TracingConfigurationTypeDef,
-        "publish": bool,
-        "versionDescription": str,
     },
     total=False,
 )
 
+
 class UpdateStateMachineInputRequestTypeDef(
     _RequiredUpdateStateMachineInputRequestTypeDef, _OptionalUpdateStateMachineInputRequestTypeDef
 ):
     pass
 
+
 GetExecutionHistoryOutputTypeDef = TypedDict(
     "GetExecutionHistoryOutputTypeDef",
     {
         "events": List[HistoryEventTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/PKG-INFO` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-stepfunctions
-Version: 1.26.159
-Summary: Type annotations for boto3.SFN 1.26.159 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.21
+Summary: Type annotations for boto3.SFN 1.26.21 service generated with mypy-boto3-builder 7.11.11
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,44 +18,43 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-stepfunctions"></a>
 
 # mypy-boto3-stepfunctions
 
 [![PyPI - mypy-boto3-stepfunctions](https://img.shields.io/pypi/v/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-stepfunctions.svg?color=blue)](https://pypi.org/project/mypy-boto3-stepfunctions)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-stepfunctions?color=blue)](https://pypistats.org/packages/mypy-boto3-stepfunctions)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SFN 1.26.159](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
+[boto3.SFN 1.26.21](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/stepfunctions.html#SFN)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.11.11](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-stepfunctions docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -355,26 +354,22 @@
     ActivityStartedEventDetailsTypeDef,
     ActivityTimedOutEventDetailsTypeDef,
     BillingDetailsTypeDef,
     CloudWatchEventsExecutionDataDetailsTypeDef,
     CloudWatchLogsLogGroupTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
-    RoutingConfigurationListItemTypeDef,
     TracingConfigurationTypeDef,
     DeleteActivityInputRequestTypeDef,
-    DeleteStateMachineAliasInputRequestTypeDef,
     DeleteStateMachineInputRequestTypeDef,
-    DeleteStateMachineVersionInputRequestTypeDef,
     DescribeActivityInputRequestTypeDef,
     DescribeExecutionInputRequestTypeDef,
     DescribeMapRunInputRequestTypeDef,
     MapRunExecutionCountsTypeDef,
     MapRunItemCountsTypeDef,
-    DescribeStateMachineAliasInputRequestTypeDef,
     DescribeStateMachineForExecutionInputRequestTypeDef,
     DescribeStateMachineInputRequestTypeDef,
     ExecutionAbortedEventDetailsTypeDef,
     ExecutionFailedEventDetailsTypeDef,
     ExecutionListItemTypeDef,
     ExecutionTimedOutEventDetailsTypeDef,
     GetActivityTaskInputRequestTypeDef,
@@ -394,22 +389,17 @@
     TaskSubmitFailedEventDetailsTypeDef,
     TaskTimedOutEventDetailsTypeDef,
     TaskCredentialsTypeDef,
     ListActivitiesInputRequestTypeDef,
     ListExecutionsInputRequestTypeDef,
     ListMapRunsInputRequestTypeDef,
     MapRunListItemTypeDef,
-    ListStateMachineAliasesInputRequestTypeDef,
-    StateMachineAliasListItemTypeDef,
-    ListStateMachineVersionsInputRequestTypeDef,
-    StateMachineVersionListItemTypeDef,
     ListStateMachinesInputRequestTypeDef,
     StateMachineListItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    PublishStateMachineVersionInputRequestTypeDef,
     SendTaskFailureInputRequestTypeDef,
     SendTaskHeartbeatInputRequestTypeDef,
     SendTaskSuccessInputRequestTypeDef,
     StartExecutionInputRequestTypeDef,
     StartSyncExecutionInputRequestTypeDef,
     StopExecutionInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
@@ -423,42 +413,34 @@
     StateExitedEventDetailsTypeDef,
     TaskSubmittedEventDetailsTypeDef,
     TaskSucceededEventDetailsTypeDef,
     LogDestinationTypeDef,
     CreateActivityInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     CreateActivityOutputTypeDef,
-    CreateStateMachineAliasOutputTypeDef,
     CreateStateMachineOutputTypeDef,
     DescribeActivityOutputTypeDef,
     DescribeExecutionOutputTypeDef,
     GetActivityTaskOutputTypeDef,
     ListActivitiesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
-    PublishStateMachineVersionOutputTypeDef,
     StartExecutionOutputTypeDef,
     StartSyncExecutionOutputTypeDef,
     StopExecutionOutputTypeDef,
-    UpdateStateMachineAliasOutputTypeDef,
     UpdateStateMachineOutputTypeDef,
-    CreateStateMachineAliasInputRequestTypeDef,
-    DescribeStateMachineAliasOutputTypeDef,
-    UpdateStateMachineAliasInputRequestTypeDef,
     DescribeMapRunOutputTypeDef,
     ListExecutionsOutputTypeDef,
     GetExecutionHistoryInputGetExecutionHistoryPaginateTypeDef,
     ListActivitiesInputListActivitiesPaginateTypeDef,
     ListExecutionsInputListExecutionsPaginateTypeDef,
     ListMapRunsInputListMapRunsPaginateTypeDef,
     ListStateMachinesInputListStateMachinesPaginateTypeDef,
     LambdaFunctionScheduledEventDetailsTypeDef,
     TaskScheduledEventDetailsTypeDef,
     ListMapRunsOutputTypeDef,
-    ListStateMachineAliasesOutputTypeDef,
-    ListStateMachineVersionsOutputTypeDef,
     ListStateMachinesOutputTypeDef,
     LoggingConfigurationTypeDef,
     HistoryEventTypeDef,
     CreateStateMachineInputRequestTypeDef,
     DescribeStateMachineForExecutionOutputTypeDef,
     DescribeStateMachineOutputTypeDef,
     UpdateStateMachineInputRequestTypeDef,
@@ -473,42 +455,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-stepfunctions-1.26.159/mypy_boto3_stepfunctions.egg-info/SOURCES.txt` & `mypy-boto3-stepfunctions-1.26.21/mypy_boto3_stepfunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-stepfunctions-1.26.159/setup.py` & `mypy-boto3-stepfunctions-1.26.21/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 """
 Setup script for mypy-boto3-stepfunctions.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-stepfunctions",
-    version="1.26.159",
+    version="1.26.21",
     packages=["mypy_boto3_stepfunctions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SFN 1.26.159 service generated with mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.SFN 1.26.21 service generated with mypy-boto3-builder 7.11.11"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
-        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 stepfunctions type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"mypy_boto3_stepfunctions": ["py.typed", "*.pyi"]},
+    package_data={"": ["LICENSE"], "mypy_boto3_stepfunctions": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_stepfunctions/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

