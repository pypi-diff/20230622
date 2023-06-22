# Comparing `tmp/botobackoff-0.0.1.tar.gz` & `tmp/botobackoff-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botobackoff-0.0.1.tar", last modified: Thu Jun 22 20:32:14 2023, max compression
+gzip compressed data, was "botobackoff-0.0.2.tar", last modified: Thu Jun 22 20:45:20 2023, max compression
```

## Comparing `botobackoff-0.0.1.tar` & `botobackoff-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 20:32:14.159300 botobackoff-0.0.1/
--rw-rw-r--   0 eric      (1000) eric      (1000)     1055 2023-06-22 15:35:52.000000 botobackoff-0.0.1/LICENSE.md
--rw-rw-r--   0 eric      (1000) eric      (1000)     2118 2023-06-22 20:32:14.159300 botobackoff-0.0.1/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)     1807 2023-06-22 20:30:24.000000 botobackoff-0.0.1/README.md
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 20:32:14.159300 botobackoff-0.0.1/botobackoff/
--rw-rw-r--   0 eric      (1000) eric      (1000)       50 2023-06-22 19:48:54.000000 botobackoff-0.0.1/botobackoff/__init__.py
--rw-r--r--   0 eric      (1000) eric      (1000)     6506 2023-06-22 20:27:27.000000 botobackoff-0.0.1/botobackoff/botobackoff.py
-drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 20:32:14.159300 botobackoff-0.0.1/botobackoff.egg-info/
--rw-rw-r--   0 eric      (1000) eric      (1000)     2118 2023-06-22 20:32:14.000000 botobackoff-0.0.1/botobackoff.egg-info/PKG-INFO
--rw-rw-r--   0 eric      (1000) eric      (1000)      254 2023-06-22 20:32:14.000000 botobackoff-0.0.1/botobackoff.egg-info/SOURCES.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-22 20:32:14.000000 botobackoff-0.0.1/botobackoff.egg-info/dependency_links.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       23 2023-06-22 20:32:14.000000 botobackoff-0.0.1/botobackoff.egg-info/requires.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       12 2023-06-22 20:32:14.000000 botobackoff-0.0.1/botobackoff.egg-info/top_level.txt
--rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-22 20:32:14.159300 botobackoff-0.0.1/setup.cfg
--rw-rw-r--   0 eric      (1000) eric      (1000)      713 2023-06-22 20:31:22.000000 botobackoff-0.0.1/setup.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 20:45:20.614360 botobackoff-0.0.2/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     1055 2023-06-22 15:35:52.000000 botobackoff-0.0.2/LICENSE.md
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2476 2023-06-22 20:45:20.614360 botobackoff-0.0.2/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2165 2023-06-22 20:41:38.000000 botobackoff-0.0.2/README.md
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 20:45:20.614360 botobackoff-0.0.2/botobackoff/
+-rw-rw-r--   0 eric      (1000) eric      (1000)       50 2023-06-22 19:48:54.000000 botobackoff-0.0.2/botobackoff/__init__.py
+-rw-r--r--   0 eric      (1000) eric      (1000)     7176 2023-06-22 20:43:50.000000 botobackoff-0.0.2/botobackoff/botobackoff.py
+drwxrwxr-x   0 eric      (1000) eric      (1000)        0 2023-06-22 20:45:20.614360 botobackoff-0.0.2/botobackoff.egg-info/
+-rw-rw-r--   0 eric      (1000) eric      (1000)     2476 2023-06-22 20:45:20.000000 botobackoff-0.0.2/botobackoff.egg-info/PKG-INFO
+-rw-rw-r--   0 eric      (1000) eric      (1000)      254 2023-06-22 20:45:20.000000 botobackoff-0.0.2/botobackoff.egg-info/SOURCES.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)        1 2023-06-22 20:45:20.000000 botobackoff-0.0.2/botobackoff.egg-info/dependency_links.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       23 2023-06-22 20:45:20.000000 botobackoff-0.0.2/botobackoff.egg-info/requires.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       12 2023-06-22 20:45:20.000000 botobackoff-0.0.2/botobackoff.egg-info/top_level.txt
+-rw-rw-r--   0 eric      (1000) eric      (1000)       38 2023-06-22 20:45:20.614360 botobackoff-0.0.2/setup.cfg
+-rw-rw-r--   0 eric      (1000) eric      (1000)      713 2023-06-22 20:41:38.000000 botobackoff-0.0.2/setup.py
```

### Comparing `botobackoff-0.0.1/LICENSE.md` & `botobackoff-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `botobackoff-0.0.1/PKG-INFO` & `botobackoff-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botobackoff
-Version: 0.0.1
+Version: 0.0.2
 Summary: boto3 retry and backoff utility
 Home-page: https://github.com/ericmaustin/botobackoff
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -31,24 +31,32 @@
 ## Usage
 
 Example with the client wrapper:
 
 ```python
 from botobackoff import BotoBackoff
 
-import boto3
-
-wrapped_client = BotoBackoff(
-    boto3.client("s3"),
-    max_retries=5,
-)
+# `BotoBackoff` can be instantiated with a boto3 client or service name
+wrapped_client = BotoBackoff("s3", max_retries=5)
 
 print(wrapped_client.list_objects(Bucket="my-bucket"))
 ```
 
+Example as context manager:
+```python
+from botobackoff import BotoBackoff
+
+wrapped_client = BotoBackoff("s3", max_retries=2)
+
+# use `with_options` to change any of the options for the context manager instance
+with wrapped_client.with_options(max_retries=5) as client:
+    print(client.list_objects(Bucket="my-bucket"))
+
+```
+
 Example with the decorator:
 ```python
 from botobackoff import botobackoff
 
 import boto3
 
 @botobackoff(max_retries=5)
```

### Comparing `botobackoff-0.0.1/README.md` & `botobackoff-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,24 +19,32 @@
 ## Usage
 
 Example with the client wrapper:
 
 ```python
 from botobackoff import BotoBackoff
 
-import boto3
-
-wrapped_client = BotoBackoff(
-    boto3.client("s3"),
-    max_retries=5,
-)
+# `BotoBackoff` can be instantiated with a boto3 client or service name
+wrapped_client = BotoBackoff("s3", max_retries=5)
 
 print(wrapped_client.list_objects(Bucket="my-bucket"))
 ```
 
+Example as context manager:
+```python
+from botobackoff import BotoBackoff
+
+wrapped_client = BotoBackoff("s3", max_retries=2)
+
+# use `with_options` to change any of the options for the context manager instance
+with wrapped_client.with_options(max_retries=5) as client:
+    print(client.list_objects(Bucket="my-bucket"))
+
+```
+
 Example with the decorator:
 ```python
 from botobackoff import botobackoff
 
 import boto3
 
 @botobackoff(max_retries=5)
```

### Comparing `botobackoff-0.0.1/botobackoff/botobackoff.py` & `botobackoff-0.0.2/botobackoff/botobackoff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations, absolute_import
 
 import boto3
 import time
 import random
-import logging
 
 from functools import wraps
 from boto3.session import Session
 from typing import Optional, Union
 from botocore.exceptions import ClientError
 from botocore.client import BaseClient
 
@@ -36,17 +35,28 @@
             interval_seconds=0.2,
             max_retries=3,
             backoff_rate=2,
             jitter=0.5,
             max_retries_before_backoff=0,
             added_error_codes: list = None,
             ignore_error_codes: list = None,
-            logger: logging.Logger = None,
             boto_session: Session = None,
     ):
+        """
+        :param client: the boto3 client to wrap or the service name to create a client for
+        :param interval_seconds: the initial number of seconds to wait between retries
+        :param max_retries: the maximum number of retries to attempt
+        :param backoff_rate: the rate at which the interval increases
+        :param jitter: the amount of jitter to add to the interval
+        :param max_retries_before_backoff: maximum number of retries before applying backoff
+        :param added_error_codes: additional error codes to retry on
+        :param ignore_error_codes: error codes to ignore, and return `None` for
+        :param boto_session: the boto3 session to use. If not provided, the default session will be used.
+            Ignored if a client is provided.
+        """
         _boto_client = client
 
         if isinstance(client, str):
             # if we weren't provided a verbose client, create one
             # use the session if provided, otherwise use default session
             _boto_client = boto_session.client(client) \
                 if boto_session \
@@ -55,15 +65,14 @@
         self._client: BaseClient = _boto_client
 
         # if no backoff error codes are provided, use the default list
         self._added_backoff_error_codes = added_error_codes or []
         self._ignore_errors = ignore_error_codes or []
         self._backoff_rate = backoff_rate
         self._interval_seconds = interval_seconds
-        self._logger = logger if logger else logging.getLogger(__name__)
         self._max_retries = max_retries
         self._jitter = jitter
         self._max_retries_before_backoff = max_retries_before_backoff
 
     def with_options(
             self,
             *,
```

### Comparing `botobackoff-0.0.1/botobackoff.egg-info/PKG-INFO` & `botobackoff-0.0.2/botobackoff.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botobackoff
-Version: 0.0.1
+Version: 0.0.2
 Summary: boto3 retry and backoff utility
 Home-page: https://github.com/ericmaustin/botobackoff
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -31,24 +31,32 @@
 ## Usage
 
 Example with the client wrapper:
 
 ```python
 from botobackoff import BotoBackoff
 
-import boto3
-
-wrapped_client = BotoBackoff(
-    boto3.client("s3"),
-    max_retries=5,
-)
+# `BotoBackoff` can be instantiated with a boto3 client or service name
+wrapped_client = BotoBackoff("s3", max_retries=5)
 
 print(wrapped_client.list_objects(Bucket="my-bucket"))
 ```
 
+Example as context manager:
+```python
+from botobackoff import BotoBackoff
+
+wrapped_client = BotoBackoff("s3", max_retries=2)
+
+# use `with_options` to change any of the options for the context manager instance
+with wrapped_client.with_options(max_retries=5) as client:
+    print(client.list_objects(Bucket="my-bucket"))
+
+```
+
 Example with the decorator:
 ```python
 from botobackoff import botobackoff
 
 import boto3
 
 @botobackoff(max_retries=5)
```

### Comparing `botobackoff-0.0.1/setup.py` & `botobackoff-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Eric Austin",
     url="https://github.com/ericmaustin/botobackoff",
     license="MIT",
     author_email="eric.m.austin@gmail.com",
     python_requires=">=3.7",
-    version="0.0.1",
+    version="0.0.2",
     include_package_data=True,
     packages=find_packages(),
     install_requires=[
         "boto3>=1.16.0",
         "botocore"
     ]
 )
```

