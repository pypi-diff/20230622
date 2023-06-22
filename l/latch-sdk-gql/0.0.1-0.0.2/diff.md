# Comparing `tmp/latch-sdk-gql-0.0.1.tar.gz` & `tmp/latch-sdk-gql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch-sdk-gql-0.0.1.tar", last modified: Thu Jun 22 20:22:24 2023, max compression
+gzip compressed data, was "latch-sdk-gql-0.0.2.tar", last modified: Thu Jun 22 20:30:56 2023, max compression
```

## Comparing `latch-sdk-gql-0.0.1.tar` & `latch-sdk-gql-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:22:24.772127 latch-sdk-gql-0.0.1/
--rw-r--r--   0 ayush      (504) staff       (20)     1065 2023-06-22 20:20:17.000000 latch-sdk-gql-0.0.1/LICENSE
--rw-r--r--   0 ayush      (504) staff       (20)      325 2023-06-22 20:22:24.771831 latch-sdk-gql-0.0.1/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)       15 2023-06-22 20:20:17.000000 latch-sdk-gql-0.0.1/README.md
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:22:24.769487 latch-sdk-gql-0.0.1/latch_sdk_gql/
--rw-r--r--   0 ayush      (504) staff       (20)       49 2023-06-22 20:02:17.000000 latch-sdk-gql-0.0.1/latch_sdk_gql/__init__.py
--rw-r--r--   0 ayush      (504) staff       (20)     1343 2023-06-22 20:02:17.000000 latch-sdk-gql-0.0.1/latch_sdk_gql/_execute.py
--rw-r--r--   0 ayush      (504) staff       (20)     2233 2023-06-22 20:02:17.000000 latch-sdk-gql-0.0.1/latch_sdk_gql/_utils.py
-drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:22:24.771415 latch-sdk-gql-0.0.1/latch_sdk_gql.egg-info/
--rw-r--r--   0 ayush      (504) staff       (20)      325 2023-06-22 20:22:24.000000 latch-sdk-gql-0.0.1/latch_sdk_gql.egg-info/PKG-INFO
--rw-r--r--   0 ayush      (504) staff       (20)      286 2023-06-22 20:22:24.000000 latch-sdk-gql-0.0.1/latch_sdk_gql.egg-info/SOURCES.txt
--rw-r--r--   0 ayush      (504) staff       (20)        1 2023-06-22 20:22:24.000000 latch-sdk-gql-0.0.1/latch_sdk_gql.egg-info/dependency_links.txt
--rw-r--r--   0 ayush      (504) staff       (20)       57 2023-06-22 20:22:24.000000 latch-sdk-gql-0.0.1/latch_sdk_gql.egg-info/requires.txt
--rw-r--r--   0 ayush      (504) staff       (20)       14 2023-06-22 20:22:24.000000 latch-sdk-gql-0.0.1/latch_sdk_gql.egg-info/top_level.txt
--rw-r--r--   0 ayush      (504) staff       (20)       38 2023-06-22 20:22:24.772220 latch-sdk-gql-0.0.1/setup.cfg
--rw-r--r--   0 ayush      (504) staff       (20)      573 2023-06-22 20:18:51.000000 latch-sdk-gql-0.0.1/setup.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:30:56.354830 latch-sdk-gql-0.0.2/
+-rw-r--r--   0 ayush      (504) staff       (20)     1065 2023-06-22 20:20:17.000000 latch-sdk-gql-0.0.2/LICENSE
+-rw-r--r--   0 ayush      (504) staff       (20)      325 2023-06-22 20:30:56.354445 latch-sdk-gql-0.0.2/PKG-INFO
+-rw-r--r--   0 ayush      (504) staff       (20)       15 2023-06-22 20:20:17.000000 latch-sdk-gql-0.0.2/README.md
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:30:56.351374 latch-sdk-gql-0.0.2/latch_sdk_gql/
+-rw-r--r--   0 ayush      (504) staff       (20)      442 2023-06-22 20:29:14.000000 latch-sdk-gql-0.0.2/latch_sdk_gql/__init__.py
+-rw-r--r--   0 ayush      (504) staff       (20)     1319 2023-06-22 20:29:26.000000 latch-sdk-gql-0.0.2/latch_sdk_gql/execute.py
+-rw-r--r--   0 ayush      (504) staff       (20)     2233 2023-06-22 20:02:17.000000 latch-sdk-gql-0.0.2/latch_sdk_gql/utils.py
+drwxr-xr-x   0 ayush      (504) staff       (20)        0 2023-06-22 20:30:56.353911 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/
+-rw-r--r--   0 ayush      (504) staff       (20)      325 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/PKG-INFO
+-rw-r--r--   0 ayush      (504) staff       (20)      284 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/SOURCES.txt
+-rw-r--r--   0 ayush      (504) staff       (20)        1 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/dependency_links.txt
+-rw-r--r--   0 ayush      (504) staff       (20)       81 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/requires.txt
+-rw-r--r--   0 ayush      (504) staff       (20)       14 2023-06-22 20:30:56.000000 latch-sdk-gql-0.0.2/latch_sdk_gql.egg-info/top_level.txt
+-rw-r--r--   0 ayush      (504) staff       (20)       38 2023-06-22 20:30:56.354948 latch-sdk-gql-0.0.2/setup.cfg
+-rw-r--r--   0 ayush      (504) staff       (20)      608 2023-06-22 20:29:50.000000 latch-sdk-gql-0.0.2/setup.py
```

### Comparing `latch-sdk-gql-0.0.1/LICENSE` & `latch-sdk-gql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `latch-sdk-gql-0.0.1/latch_sdk_gql/_execute.py` & `latch-sdk-gql-0.0.2/latch_sdk_gql/execute.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,18 @@
     from functools import lru_cache as cache
 
 from typing import Dict, Optional
 
 import gql
 from gql.transport.requests import RequestsHTTPTransport
 from graphql import DocumentNode
+from latch_sdk_config.latch import config
+from latch_sdk_config.user import user_config
 
-from latch.gql import AuthenticationError
-from latch.types.json import JsonValue
-from latch_cli.config.latch import config
-from latch_cli.config.user import user_config
+from latch_sdk_gql import AuthenticationError, JsonValue
 
 
 @cache
 def _get_client():
     auth_header: Optional[str] = None
 
     if auth_header is None:
```

### Comparing `latch-sdk-gql-0.0.1/latch_sdk_gql/_utils.py` & `latch-sdk-gql-0.0.2/latch_sdk_gql/utils.py`

 * *Files identical despite different names*

### Comparing `latch-sdk-gql-0.0.1/setup.py` & `latch-sdk-gql-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from setuptools import find_packages, setup
 
 setup(
     name="latch-sdk-gql",
-    version="v0.0.1",
+    version="v0.0.2",
     author_email="ayush@latch.bio",
     description="Internal Latch GQL package",
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.8,<3.11",
     install_requires=[
+        "latch-sdk-config==0.0.1",
         "gql==3.4.0",
         "graphql-core==3.2.3",
         "requests-toolbelt==0.10.1",
     ],
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

