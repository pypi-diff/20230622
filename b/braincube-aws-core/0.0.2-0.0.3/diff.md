# Comparing `tmp/braincube-aws-core-0.0.2.tar.gz` & `tmp/braincube-aws-core-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-0.0.2.tar", last modified: Wed Jun 21 20:21:58 2023, max compression
+gzip compressed data, was "braincube-aws-core-0.0.3.tar", last modified: Thu Jun 22 09:25:33 2023, max compression
```

## Comparing `braincube-aws-core-0.0.2.tar` & `braincube-aws-core-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.892466 braincube-aws-core-0.0.2/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8761 2023-06-21 20:21:58.892617 braincube-aws-core-0.0.2/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8015 2023-06-21 20:10:09.000000 braincube-aws-core-0.0.2/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-21 20:21:58.893230 braincube-aws-core-0.0.2/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.874910 braincube-aws-core-0.0.2/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.878912 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8761 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-21 20:21:58.000000 braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.879192 braincube-aws-core-0.0.2/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.882194 braincube-aws-core-0.0.2/src/core/app/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/app/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.2/src/core/app/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.2/src/core/app/app_event.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6203 2023-06-21 20:01:55.000000 braincube-aws-core-0.0.2/src/core/app/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-21 13:21:21.000000 braincube-aws-core-0.0.2/src/core/app/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.2/src/core/app/exception_handler.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.886295 braincube-aws-core-0.0.2/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.2/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.2/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.2/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-0.0.2/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.888123 braincube-aws-core-0.0.2/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.2/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.2/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.890224 braincube-aws-core-0.0.2/src/core/rules_engine/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/rules_engine/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.2/src/core/rules_engine/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.2/src/core/rules_engine/exceptions.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.2/src/core/rules_engine/rule_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-21 20:21:58.891925 braincube-aws-core-0.0.2/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.2/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.2/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.2/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.060478 braincube-aws-core-0.0.3/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 09:25:33.060745 braincube-aws-core-0.0.3/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.3/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-22 09:25:33.061977 braincube-aws-core-0.0.3/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.038099 braincube-aws-core-0.0.3/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.042657 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.043002 braincube-aws-core-0.0.3/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.046346 braincube-aws-core-0.0.3/src/core/app/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/app/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.3/src/core/app/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.3/src/core/app/app_event.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6203 2023-06-21 20:01:55.000000 braincube-aws-core-0.0.3/src/core/app/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-22 09:23:59.000000 braincube-aws-core-0.0.3/src/core/app/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.3/src/core/app/exception_handler.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.050611 braincube-aws-core-0.0.3/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.3/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.3/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.3/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-0.0.3/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.053826 braincube-aws-core-0.0.3/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.3/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.3/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.057334 braincube-aws-core-0.0.3/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.3/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.3/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.3/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.059728 braincube-aws-core-0.0.3/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.3/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.3/src/core/utils/data.py
```

### Comparing `braincube-aws-core-0.0.2/LICENSE` & `braincube-aws-core-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/PKG-INFO` & `braincube-aws-core-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 License-File: LICENSE
 
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
-[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core.svg)](https://pypi.org/project/braincube-aws-core/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Installation
 
 ```bash
 pip install braincube-aws-core
 ```
```

### Comparing `braincube-aws-core-0.0.2/README.md` & `braincube-aws-core-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
-[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core.svg)](https://pypi.org/project/braincube-aws-core/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Installation
 
 ```bash
 pip install braincube-aws-core
 ```
```

### Comparing `braincube-aws-core-0.0.2/setup.cfg` & `braincube-aws-core-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core
-version = 0.0.2
+version = 0.0.3
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/PKG-INFO` & `braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.2
+Version: 0.0.3
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
@@ -19,15 +19,15 @@
 License-File: LICENSE
 
 # braincube-aws-core
 
 Microframework for Python AWS lambdas.
 
 [![Language](https://img.shields.io/badge/language-Python-blue.svg)](https://www.python.org/)
-[![pypi](https://img.shields.io/pypi/v/braincube-aws-core-alpha.svg)](https://pypi.org/project/braincube-aws-core/)
+[![pypi](https://img.shields.io/pypi/v/braincube-aws-core.svg)](https://pypi.org/project/braincube-aws-core/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 
 ## Installation
 
 ```bash
 pip install braincube-aws-core
 ```
```

### Comparing `braincube-aws-core-0.0.2/src/braincube_aws_core.egg-info/SOURCES.txt` & `braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/app/app_controller.py` & `braincube-aws-core-0.0.3/src/core/app/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/app/app_event.py` & `braincube-aws-core-0.0.3/src/core/app/app_event.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/app/app_module.py` & `braincube-aws-core-0.0.3/src/core/app/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/app/data.py` & `braincube-aws-core-0.0.3/src/core/app/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
 
     request = HTTPRequest(body=cls(**data) if cls is not dict else data,
                           headers=event.get("headers"),
                           path_params=event.get("pathParameters"))
 
     if "authorizer" in event["requestContext"]:
         claims = event["requestContext"]["authorizer"]["claims"]
-        request.user = AuthUser(claims["sub"], claims["email"], claims["email_verified"] == "True")
+        request.user = AuthUser(claims["sub"], claims["email"], claims["email_verified"] == "true")
 
     params: dict[str, any] | None = event.get("queryStringParameters")
 
     if params:
         fields = params["fields"].replace(" ", "").split(",") if params.get("fields") else list()
         pageable = Pageable(page_param(params, alias="pageNo"),
                             page_param(params, alias="pageSize", default=20, max_=50, min_=1),
```

### Comparing `braincube-aws-core-0.0.2/src/core/dal/data.py` & `braincube-aws-core-0.0.3/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/dal/postgres_connection.py` & `braincube-aws-core-0.0.3/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/dal/postgres_repository.py` & `braincube-aws-core-0.0.3/src/core/dal/postgres_repository.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/di/data.py` & `braincube-aws-core-0.0.3/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/di/injector.py` & `braincube-aws-core-0.0.3/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/rules_engine/data.py` & `braincube-aws-core-0.0.3/src/core/rules_engine/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/rules_engine/rule_manager.py` & `braincube-aws-core-0.0.3/src/core/rules_engine/rule_manager.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/utils/convert.py` & `braincube-aws-core-0.0.3/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.2/src/core/utils/data.py` & `braincube-aws-core-0.0.3/src/core/utils/data.py`

 * *Files identical despite different names*

