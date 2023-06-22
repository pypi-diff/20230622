# Comparing `tmp/djongo-fixed-1.3.6.tar.gz` & `tmp/djongo-fixed-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djongo-fixed-1.3.6.tar", last modified: Mon May 15 08:26:48 2023, max compression
+gzip compressed data, was "djongo-fixed-1.3.7.tar", last modified: Thu Jun 22 13:14:44 2023, max compression
```

## Comparing `djongo-fixed-1.3.6.tar` & `djongo-fixed-1.3.7.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-05-15 08:26:48.002265 djongo-fixed-1.3.6/
--rw-r--r--   0 binn       (501) staff       (20)    34481 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/LICENSE
--rw-r--r--   0 binn       (501) staff       (20)      267 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/MANIFEST.in
--rw-r--r--   0 binn       (501) staff       (20)     1592 2023-05-15 08:26:48.002320 djongo-fixed-1.3.6/PKG-INFO
--rw-r--r--   0 binn       (501) staff       (20)     2854 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/README.md
-drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-05-15 08:26:48.000150 djongo-fixed-1.3.6/djongo/
--rw-r--r--   0 binn       (501) staff       (20)      224 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/__init__.py
--rw-r--r--   0 binn       (501) staff       (20)      860 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/admin.py
--rw-r--r--   0 binn       (501) staff       (20)     6626 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/base.py
--rw-r--r--   0 binn       (501) staff       (20)      161 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/compiler.py
--rw-r--r--   0 binn       (501) staff       (20)     1301 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/creation.py
--rw-r--r--   0 binn       (501) staff       (20)     2019 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/cursor.py
--rw-r--r--   0 binn       (501) staff       (20)      782 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/database.py
--rw-r--r--   0 binn       (501) staff       (20)     1159 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/exceptions.py
--rw-r--r--   0 binn       (501) staff       (20)      434 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/features.py
--rw-r--r--   0 binn       (501) staff       (20)     3496 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/introspection.py
-drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-05-15 08:26:48.000609 djongo-fixed-1.3.6/djongo/models/
--rw-r--r--   0 binn       (501) staff       (20)      399 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/models/__init__.py
--rw-r--r--   0 binn       (501) staff       (20)    37132 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/models/fields.py
--rw-r--r--   0 binn       (501) staff       (20)       50 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/models/indexes.py
--rw-r--r--   0 binn       (501) staff       (20)      570 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/models/json.py
--rw-r--r--   0 binn       (501) staff       (20)     4419 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/operations.py
--rw-r--r--   0 binn       (501) staff       (20)      609 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/schema.py
-drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-05-15 08:26:48.001649 djongo-fixed-1.3.6/djongo/sql2mongo/
--rw-r--r--   0 binn       (501) staff       (20)        0 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/__init__.py
--rw-r--r--   0 binn       (501) staff       (20)       88 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/aggregation.py
--rw-r--r--   0 binn       (501) staff       (20)      214 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/constraints.py
--rw-r--r--   0 binn       (501) staff       (20)    12748 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/converters.py
--rw-r--r--   0 binn       (501) staff       (20)     2954 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/functions.py
--rw-r--r--   0 binn       (501) staff       (20)    15587 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/operators.py
--rw-r--r--   0 binn       (501) staff       (20)    32626 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/query.py
--rw-r--r--   0 binn       (501) staff       (20)    12682 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/sql_tokens.py
--rw-r--r--   0 binn       (501) staff       (20)      189 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/sql2mongo/validation.py
--rw-r--r--   0 binn       (501) staff       (20)     6238 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/storage.py
--rw-r--r--   0 binn       (501) staff       (20)      216 2023-05-15 08:20:51.000000 djongo-fixed-1.3.6/djongo/transaction.py
-drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-05-15 08:26:48.002172 djongo-fixed-1.3.6/djongo_fixed.egg-info/
--rw-r--r--   0 binn       (501) staff       (20)     1592 2023-05-15 08:26:47.000000 djongo-fixed-1.3.6/djongo_fixed.egg-info/PKG-INFO
--rw-r--r--   0 binn       (501) staff       (20)      862 2023-05-15 08:26:47.000000 djongo-fixed-1.3.6/djongo_fixed.egg-info/SOURCES.txt
--rw-r--r--   0 binn       (501) staff       (20)        1 2023-05-15 08:26:47.000000 djongo-fixed-1.3.6/djongo_fixed.egg-info/dependency_links.txt
--rw-r--r--   0 binn       (501) staff       (20)       94 2023-05-15 08:26:47.000000 djongo-fixed-1.3.6/djongo_fixed.egg-info/requires.txt
--rw-r--r--   0 binn       (501) staff       (20)        7 2023-05-15 08:26:47.000000 djongo-fixed-1.3.6/djongo_fixed.egg-info/top_level.txt
--rw-r--r--   0 binn       (501) staff       (20)       79 2023-05-15 08:26:48.002534 djongo-fixed-1.3.6/setup.cfg
--rw-r--r--   0 binn       (501) staff       (20)     2791 2023-05-15 08:25:23.000000 djongo-fixed-1.3.6/setup.py
+drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-06-22 13:14:44.557172 djongo-fixed-1.3.7/
+-rw-r--r--   0 binn       (501) staff       (20)    34481 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/LICENSE
+-rw-r--r--   0 binn       (501) staff       (20)      267 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/MANIFEST.in
+-rw-r--r--   0 binn       (501) staff       (20)     1592 2023-06-22 13:14:44.557263 djongo-fixed-1.3.7/PKG-INFO
+-rw-r--r--   0 binn       (501) staff       (20)     2854 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/README.md
+drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-06-22 13:14:44.554585 djongo-fixed-1.3.7/djongo/
+-rw-r--r--   0 binn       (501) staff       (20)      224 2023-06-22 13:10:11.000000 djongo-fixed-1.3.7/djongo/__init__.py
+-rw-r--r--   0 binn       (501) staff       (20)      860 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/admin.py
+-rw-r--r--   0 binn       (501) staff       (20)     6626 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/base.py
+-rw-r--r--   0 binn       (501) staff       (20)      161 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/compiler.py
+-rw-r--r--   0 binn       (501) staff       (20)     1301 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/creation.py
+-rw-r--r--   0 binn       (501) staff       (20)     2019 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/cursor.py
+-rw-r--r--   0 binn       (501) staff       (20)      782 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/database.py
+-rw-r--r--   0 binn       (501) staff       (20)     1159 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/exceptions.py
+-rw-r--r--   0 binn       (501) staff       (20)      434 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/features.py
+-rw-r--r--   0 binn       (501) staff       (20)     3496 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/introspection.py
+drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-06-22 13:14:44.555151 djongo-fixed-1.3.7/djongo/models/
+-rw-r--r--   0 binn       (501) staff       (20)      399 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/models/__init__.py
+-rw-r--r--   0 binn       (501) staff       (20)    37132 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/models/fields.py
+-rw-r--r--   0 binn       (501) staff       (20)       50 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/models/indexes.py
+-rw-r--r--   0 binn       (501) staff       (20)      570 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/models/json.py
+-rw-r--r--   0 binn       (501) staff       (20)     4419 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/operations.py
+-rw-r--r--   0 binn       (501) staff       (20)      609 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/schema.py
+drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-06-22 13:14:44.556465 djongo-fixed-1.3.7/djongo/sql2mongo/
+-rw-r--r--   0 binn       (501) staff       (20)        0 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/__init__.py
+-rw-r--r--   0 binn       (501) staff       (20)       88 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/aggregation.py
+-rw-r--r--   0 binn       (501) staff       (20)      214 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/constraints.py
+-rw-r--r--   0 binn       (501) staff       (20)    12748 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/converters.py
+-rw-r--r--   0 binn       (501) staff       (20)     2954 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/functions.py
+-rw-r--r--   0 binn       (501) staff       (20)    15587 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/operators.py
+-rw-r--r--   0 binn       (501) staff       (20)    32626 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/query.py
+-rw-r--r--   0 binn       (501) staff       (20)    13813 2023-06-22 11:26:08.000000 djongo-fixed-1.3.7/djongo/sql2mongo/sql_tokens.py
+-rw-r--r--   0 binn       (501) staff       (20)      189 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/sql2mongo/validation.py
+-rw-r--r--   0 binn       (501) staff       (20)     6238 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/storage.py
+-rw-r--r--   0 binn       (501) staff       (20)      216 2023-06-22 11:22:34.000000 djongo-fixed-1.3.7/djongo/transaction.py
+drwxr-xr-x   0 binn       (501) staff       (20)        0 2023-06-22 13:14:44.557041 djongo-fixed-1.3.7/djongo_fixed.egg-info/
+-rw-r--r--   0 binn       (501) staff       (20)     1592 2023-06-22 13:14:44.000000 djongo-fixed-1.3.7/djongo_fixed.egg-info/PKG-INFO
+-rw-r--r--   0 binn       (501) staff       (20)      862 2023-06-22 13:14:44.000000 djongo-fixed-1.3.7/djongo_fixed.egg-info/SOURCES.txt
+-rw-r--r--   0 binn       (501) staff       (20)        1 2023-06-22 13:14:44.000000 djongo-fixed-1.3.7/djongo_fixed.egg-info/dependency_links.txt
+-rw-r--r--   0 binn       (501) staff       (20)       94 2023-06-22 13:14:44.000000 djongo-fixed-1.3.7/djongo_fixed.egg-info/requires.txt
+-rw-r--r--   0 binn       (501) staff       (20)        7 2023-06-22 13:14:44.000000 djongo-fixed-1.3.7/djongo_fixed.egg-info/top_level.txt
+-rw-r--r--   0 binn       (501) staff       (20)       79 2023-06-22 13:14:44.557469 djongo-fixed-1.3.7/setup.cfg
+-rw-r--r--   0 binn       (501) staff       (20)     2791 2023-06-22 13:14:34.000000 djongo-fixed-1.3.7/setup.py
```

### Comparing `djongo-fixed-1.3.6/LICENSE` & `djongo-fixed-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/PKG-INFO` & `djongo-fixed-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djongo-fixed
-Version: 1.3.6
+Version: 1.3.7
 Summary: Driver for allowing Django to use MongoDB as the database backend.
 Home-page: https://www.djongomapper.com/
 Author: doableware
 Author-email: support@doableware.com
 License: AGPL
 Keywords: Django MongoDB driver connector
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `djongo-fixed-1.3.6/README.md` & `djongo-fixed-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/admin.py` & `djongo-fixed-1.3.7/djongo/admin.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/base.py` & `djongo-fixed-1.3.7/djongo/base.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/creation.py` & `djongo-fixed-1.3.7/djongo/creation.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/cursor.py` & `djongo-fixed-1.3.7/djongo/cursor.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/database.py` & `djongo-fixed-1.3.7/djongo/database.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/exceptions.py` & `djongo-fixed-1.3.7/djongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/introspection.py` & `djongo-fixed-1.3.7/djongo/introspection.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/models/fields.py` & `djongo-fixed-1.3.7/djongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/models/json.py` & `djongo-fixed-1.3.7/djongo/models/json.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/operations.py` & `djongo-fixed-1.3.7/djongo/operations.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/schema.py` & `djongo-fixed-1.3.7/djongo/schema.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/sql2mongo/converters.py` & `djongo-fixed-1.3.7/djongo/sql2mongo/converters.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/sql2mongo/functions.py` & `djongo-fixed-1.3.7/djongo/sql2mongo/functions.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/sql2mongo/operators.py` & `djongo-fixed-1.3.7/djongo/sql2mongo/operators.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/sql2mongo/query.py` & `djongo-fixed-1.3.7/djongo/sql2mongo/query.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo/sql2mongo/sql_tokens.py` & `djongo-fixed-1.3.7/djongo/sql2mongo/sql_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from pymongo import ASCENDING, DESCENDING
 from sqlparse import tokens, parse as sqlparse
 from sqlparse.sql import Token, Identifier, Function, Comparison, Parenthesis, IdentifierList, Statement
 from . import query as query_module
 from ..exceptions import SQLDecodeError, NotSupportedError
 
 all_token_types = U['SQLConstIdentifier',
+                    'SQLConstIntIdentifier',
+                    'SQLConstParameterizedIdentifier',
                     'djongo.sql2mongo.functions.CountFunc',
                     'djongo.sql2mongo.functions.SimpleFunc',
                     'SQLIdentifier',
                     'SQLComparison',
                     'SQLPlaceholder']
 
 
@@ -36,17 +38,22 @@
             # Bug fix for sql parse
             if isinstance(token[0], Parenthesis):
                 try:
                     int(token[0][1].value)
                 except ValueError:
                     yield SQLIdentifier(token[0][1], query)
                 else:
-                    yield SQLConstIdentifier(token, query)
+                    # TMiles-2022.XI.18 - Specify int identifier to match original functionality.
+                    yield SQLConstIntIdentifier(token, query)
             elif isinstance(token[0], Function):
                 yield SQLFunc.token2sql(token, query)
+            elif token[0].ttype == tokens.Name.Placeholder:
+                # TMiles-2022.XI.18
+                # Use a parameterized const identifier to handle newer django foreign key lookup queries.
+                yield SQLConstParameterizedIdentifier(token, query)
             else:
                 yield SQLIdentifier(token, query)
         elif isinstance(token, Function):
             yield SQLFunc.token2sql(token, query)
         elif isinstance(token, Comparison):
             yield SQLComparison(token, query)
         elif isinstance(token, IdentifierList):
@@ -148,25 +155,45 @@
     def column(self) -> str:
         name = self._token.get_real_name()
         if name is None:
             raise SQLDecodeError
         return name
 
 
+# TMiles-2022.XI.18
+# Break ConstIdentifier into Int and Parameterized subclasses to allow for django 4
+# foreign key lookups and for future expansion to other non-int constants.
 class SQLConstIdentifier(AliasableToken):
 
     def __init__(self, *args):
         super().__init__(*args)
 
+    def to_mongo(self) -> dict:
+        return {'$literal': self.value}
+
+class SQLConstIntIdentifier(SQLConstIdentifier):
+
+    def __init__(self, *args):
+        super().__init__(*args)
+
     @property
     def value(self) -> int:
         return int(self._token[0][1].value)
 
-    def to_mongo(self) -> dict:
-        return {'$literal': self.value}
+class SQLConstParameterizedIdentifier(SQLConstIdentifier):
+
+    def __init__(self, *args):
+        tok = args[0];
+        if (tok[0].ttype != tokens.Name.Placeholder):
+            raise Exception("Token is not a placeholder")
+        super().__init__(*args)
+
+    @property
+    def value(self):
+        return self.query.params[self.placeholder_index(self._token[0])]
 
 
 class SQLComparison(SQLToken):
 
     @property
     def left_table(self):
         lhs = SQLIdentifier(self._token.left, self.query)
@@ -406,8 +433,8 @@
 class SQLColumnConstraint(SQLColumnDef):
     pass
 
 
 ORDER_BY_MAP = {
     'ASC': ASCENDING,
     'DESC': DESCENDING
-}
+}
```

### Comparing `djongo-fixed-1.3.6/djongo/storage.py` & `djongo-fixed-1.3.7/djongo/storage.py`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/djongo_fixed.egg-info/PKG-INFO` & `djongo-fixed-1.3.7/djongo_fixed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djongo-fixed
-Version: 1.3.6
+Version: 1.3.7
 Summary: Driver for allowing Django to use MongoDB as the database backend.
 Home-page: https://www.djongomapper.com/
 Author: doableware
 Author-email: support@doableware.com
 License: AGPL
 Keywords: Django MongoDB driver connector
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `djongo-fixed-1.3.6/djongo_fixed.egg-info/SOURCES.txt` & `djongo-fixed-1.3.7/djongo_fixed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djongo-fixed-1.3.6/setup.py` & `djongo-fixed-1.3.7/setup.py`

 * *Files identical despite different names*

