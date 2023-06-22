# Comparing `tmp/braincube-aws-core-0.0.3.tar.gz` & `tmp/braincube-aws-core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braincube-aws-core-0.0.3.tar", last modified: Thu Jun 22 09:25:33 2023, max compression
+gzip compressed data, was "braincube-aws-core-0.0.4.tar", last modified: Thu Jun 22 15:42:49 2023, max compression
```

## Comparing `braincube-aws-core-0.0.3.tar` & `braincube-aws-core-0.0.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.060478 braincube-aws-core-0.0.3/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/LICENSE
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 09:25:33.060745 braincube-aws-core-0.0.3/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.3/README.md
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/pyproject.toml
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-22 09:25:33.061977 braincube-aws-core-0.0.3/setup.cfg
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/setup.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.038099 braincube-aws-core-0.0.3/src/
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.042657 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/PKG-INFO
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/SOURCES.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/dependency_links.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/requires.txt
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-22 09:25:33.000000 braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/top_level.txt
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.043002 braincube-aws-core-0.0.3/src/core/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/__init__.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.046346 braincube-aws-core-0.0.3/src/core/app/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/app/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.3/src/core/app/app_controller.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.3/src/core/app/app_event.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6203 2023-06-21 20:01:55.000000 braincube-aws-core-0.0.3/src/core/app/app_module.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-22 09:23:59.000000 braincube-aws-core-0.0.3/src/core/app/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.3/src/core/app/exception_handler.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.050611 braincube-aws-core-0.0.3/src/core/dal/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/dal/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.3/src/core/dal/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.3/src/core/dal/database_errors.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.3/src/core/dal/postgres_connection.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)    33020 2023-05-31 12:25:52.000000 braincube-aws-core-0.0.3/src/core/dal/postgres_repository.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.053826 braincube-aws-core-0.0.3/src/core/di/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/di/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.3/src/core/di/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.3/src/core/di/injector.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.057334 braincube-aws-core-0.0.3/src/core/rules_engine/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/rules_engine/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.3/src/core/rules_engine/data.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.3/src/core/rules_engine/exceptions.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.3/src/core/rules_engine/rule_manager.py
-drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 09:25:33.059728 braincube-aws-core-0.0.3/src/core/utils/
--rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.3/src/core/utils/__init__.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.3/src/core/utils/convert.py
--rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.3/src/core/utils/data.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.717499 braincube-aws-core-0.0.4/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1066 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/LICENSE
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 15:42:49.717668 braincube-aws-core-0.0.4/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8009 2023-06-21 20:23:04.000000 braincube-aws-core-0.0.4/README.md
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      103 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/pyproject.toml
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      946 2023-06-22 15:42:49.718745 braincube-aws-core-0.0.4/setup.cfg
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       38 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/setup.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.698155 braincube-aws-core-0.0.4/src/
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.703203 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     8755 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/PKG-INFO
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      897 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/SOURCES.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        1 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/dependency_links.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)       67 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/requires.txt
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        5 2023-06-22 15:42:49.000000 braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/top_level.txt
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.703497 braincube-aws-core-0.0.4/src/core/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/__init__.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.707766 braincube-aws-core-0.0.4/src/core/app/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/app/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2793 2023-05-11 10:52:14.000000 braincube-aws-core-0.0.4/src/core/app/app_controller.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      664 2023-06-21 16:34:05.000000 braincube-aws-core-0.0.4/src/core/app/app_event.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6203 2023-06-21 20:01:55.000000 braincube-aws-core-0.0.4/src/core/app/app_module.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4665 2023-06-22 09:23:59.000000 braincube-aws-core-0.0.4/src/core/app/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      479 2023-06-21 17:15:33.000000 braincube-aws-core-0.0.4/src/core/app/exception_handler.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.711060 braincube-aws-core-0.0.4/src/core/dal/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/dal/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1990 2023-06-14 20:23:51.000000 braincube-aws-core-0.0.4/src/core/dal/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      241 2023-05-11 10:53:14.000000 braincube-aws-core-0.0.4/src/core/dal/database_errors.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     6191 2023-06-15 06:23:48.000000 braincube-aws-core-0.0.4/src/core/dal/postgres_connection.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)    33246 2023-06-22 15:26:24.000000 braincube-aws-core-0.0.4/src/core/dal/postgres_repository.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.713222 braincube-aws-core-0.0.4/src/core/di/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/di/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      561 2023-05-11 10:50:19.000000 braincube-aws-core-0.0.4/src/core/di/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     4122 2023-05-11 10:51:25.000000 braincube-aws-core-0.0.4/src/core/di/injector.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.715371 braincube-aws-core-0.0.4/src/core/rules_engine/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/rules_engine/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1017 2023-06-01 06:45:52.000000 braincube-aws-core-0.0.4/src/core/rules_engine/data.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      132 2023-06-01 06:45:21.000000 braincube-aws-core-0.0.4/src/core/rules_engine/exceptions.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     2752 2023-06-01 07:59:06.000000 braincube-aws-core-0.0.4/src/core/rules_engine/rule_manager.py
+drwxr-xr-x   0 evangelosboudis   (501) staff       (20)        0 2023-06-22 15:42:49.716879 braincube-aws-core-0.0.4/src/core/utils/
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)        0 2023-05-10 08:49:09.000000 braincube-aws-core-0.0.4/src/core/utils/__init__.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)      738 2023-05-15 14:42:55.000000 braincube-aws-core-0.0.4/src/core/utils/convert.py
+-rw-r--r--   0 evangelosboudis   (501) staff       (20)     1377 2023-05-11 10:53:41.000000 braincube-aws-core-0.0.4/src/core/utils/data.py
```

### Comparing `braincube-aws-core-0.0.3/LICENSE` & `braincube-aws-core-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/PKG-INFO` & `braincube-aws-core-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.3/README.md` & `braincube-aws-core-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/setup.cfg` & `braincube-aws-core-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = braincube-aws-core
-version = 0.0.3
+version = 0.0.4
 author = Braincube
 author_email = v.boudis@braincube.gr
 description = Microframework for python aws lambdas
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/braincube-common/core-aws.git
 license = MIT
```

### Comparing `braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/PKG-INFO` & `braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: braincube-aws-core
-Version: 0.0.3
+Version: 0.0.4
 Summary: Microframework for python aws lambdas
 Home-page: https://bitbucket.org/braincube-common/core-aws.git
 Author: Braincube
 Author-email: v.boudis@braincube.gr
 License: MIT
 Keywords: python,amazon,aws,lambda,routing,dal,injection
 Classifier: Intended Audience :: Developers
```

### Comparing `braincube-aws-core-0.0.3/src/braincube_aws_core.egg-info/SOURCES.txt` & `braincube-aws-core-0.0.4/src/braincube_aws_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/app/app_controller.py` & `braincube-aws-core-0.0.4/src/core/app/app_controller.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/app/app_event.py` & `braincube-aws-core-0.0.4/src/core/app/app_event.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/app/app_module.py` & `braincube-aws-core-0.0.4/src/core/app/app_module.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/app/data.py` & `braincube-aws-core-0.0.4/src/core/app/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/dal/data.py` & `braincube-aws-core-0.0.4/src/core/dal/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/dal/postgres_connection.py` & `braincube-aws-core-0.0.4/src/core/dal/postgres_connection.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/dal/postgres_repository.py` & `braincube-aws-core-0.0.4/src/core/dal/postgres_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import time
 import math
 import itertools
+from json import dumps
 from typing import TypeVar
 
 from pydantic import BaseModel
 from pypika.queries import QueryBuilder
 from pypika import PostgreSQLQuery, Table, Field, Criterion, EmptyCriterion, CustomFunction, functions as fn
 
+from ..utils.convert import JSONEncoder
 from ..utils.data import Order, OrderType, Condition, ConditionType, Page, Pageable, Paging, Top, Metadata
 from .data import Key, Schema, SaveType, TableData, FieldData, RelatedTableData, OrderData, FieldType
 from .database_errors import DatabaseError, DeleteError, SaveError
 from .postgres_connection import Pool, Connection, create_connection
 
 T = TypeVar("T", bound=BaseModel)
 
@@ -96,14 +98,23 @@
         else:
             self._order_by.extend([OrderData(pk.field, OrderType.asc) for pk in self._primary_key.values()])
 
     @staticmethod
     def __base_model_aliases(cls: type[T]) -> list[str]:
         return [f.alias for f in cls.__fields__.values()]
 
+    @staticmethod
+    def __convert_data(param: BaseModel | dict) -> dict:
+        data = param.dict(by_alias=True, exclude_unset=True) if isinstance(param, BaseModel) else param.copy()
+        for k, v in data.items():
+            if not isinstance(v, dict):
+                continue
+            data[k] = dumps(v, cls=JSONEncoder)
+        return data
+
     async def fetch(self, q: str, params: list = None, connection: Connection = None):
         """Retrieve records from raw PSQL query.
         :param q: Query.
         :param params: Query parameters.
         :param connection: (asyncpg) Connection that will execute the query.
         :return: Records as dictionary.
         """
@@ -507,18 +518,15 @@
         :param data: Master column aliases with values.
         :param returning_aliases: Query returning data.
         :param connection: (asyncpg) Connection that will execute the generated query.
         :raise SaveError: When does not adjust to insert-constraints or no master column is specified.
         :return: Execution results as dictionary.
         """
 
-        data_ = self._filter_save_data(
-            data.dict(by_alias=True, exclude_unset=True) if isinstance(data, BaseModel) else data.copy(),
-            SaveType.insert
-        )
+        data_ = self._filter_save_data(self.__convert_data(data), SaveType.insert)
 
         iq = PostgreSQLQuery \
             .into(self._master_table.name) \
             .columns(list(data_.keys())) \
             .insert(list(data_.values()))
 
         records = await self._execute(iq, returning_aliases, connection)
@@ -599,17 +607,15 @@
             raise DeleteError("update without conditions is not allowed")
 
         criterion = conditions if isinstance(conditions, Criterion) \
             else self._conditions_to_criterion(conditions, select=False)
 
         uq = PostgreSQLQuery.update(self._master_table.name)
 
-        data_ = data.dict(by_alias=True, exclude_unset=True) if isinstance(data, BaseModel) else data.copy()
-
-        for v, k in self._filter_save_data(data_, SaveType.update).items():
+        for v, k in self._filter_save_data(self.__convert_data(data), SaveType.update).items():
             uq = uq.set(v, k)
 
         uq = uq.where(criterion)
 
         return await self._execute(uq, returning_aliases, connection)
 
     async def update_by_pk(self, key: Key,
```

### Comparing `braincube-aws-core-0.0.3/src/core/di/data.py` & `braincube-aws-core-0.0.4/src/core/di/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/di/injector.py` & `braincube-aws-core-0.0.4/src/core/di/injector.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/rules_engine/data.py` & `braincube-aws-core-0.0.4/src/core/rules_engine/data.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/rules_engine/rule_manager.py` & `braincube-aws-core-0.0.4/src/core/rules_engine/rule_manager.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/utils/convert.py` & `braincube-aws-core-0.0.4/src/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `braincube-aws-core-0.0.3/src/core/utils/data.py` & `braincube-aws-core-0.0.4/src/core/utils/data.py`

 * *Files identical despite different names*

