# Comparing `tmp/Mongeasy-0.1.9.tar.gz` & `tmp/mongeasy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mongeasy-0.1.9.tar", last modified: Fri Jun 16 12:08:47 2023, max compression
+gzip compressed data, was "mongeasy-0.2.0.tar", last modified: Thu Jun 22 11:20:02 2023, max compression
```

## Comparing `Mongeasy-0.1.9.tar` & `mongeasy-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,44 @@
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.744907 Mongeasy-0.1.9/
--rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/LICENSE
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.718171 Mongeasy-0.1.9/Mongeasy.egg-info/
--rw-r--r--   0 javv       (501) staff       (20)    11039 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)      599 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/SOURCES.txt
--rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/dependency_links.txt
--rw-r--r--   0 javv       (501) staff       (20)       47 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/entry_points.txt
--rw-r--r--   0 javv       (501) staff       (20)       15 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/requires.txt
--rw-r--r--   0 javv       (501) staff       (20)       15 2023-06-16 12:08:47.000000 Mongeasy-0.1.9/Mongeasy.egg-info/top_level.txt
--rw-r--r--   0 javv       (501) staff       (20)    11039 2023-06-16 12:08:47.745078 Mongeasy-0.1.9/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)    10228 2023-06-16 12:03:09.000000 Mongeasy-0.1.9/README.md
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.726863 Mongeasy-0.1.9/mongeasy/
--rw-r--r--   0 javv       (501) staff       (20)     2235 2023-06-03 05:07:09.000000 Mongeasy-0.1.9/mongeasy/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/base_dict.py
--rw-r--r--   0 javv       (501) staff       (20)     2809 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/connection.py
--rw-r--r--   0 javv       (501) staff       (20)     4690 2023-06-16 10:02:45.000000 Mongeasy-0.1.9/mongeasy/core.py
--rw-r--r--   0 javv       (501) staff       (20)    12539 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/document.py
--rw-r--r--   0 javv       (501) staff       (20)     2601 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/dynamics.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.730061 Mongeasy-0.1.9/mongeasy/examples/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/examples/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/exceptions.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.731047 Mongeasy-0.1.9/mongeasy/extensions/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/extensions/__init__.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.732038 Mongeasy-0.1.9/mongeasy/plugins/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/plugins/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/resultlist.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.735211 Mongeasy-0.1.9/mongeasy/utils/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/utils/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/mongeasy/utils/utils.py
--rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/pyproject.toml
--rw-r--r--   0 javv       (501) staff       (20)     1013 2023-06-16 12:08:47.746351 Mongeasy-0.1.9/setup.cfg
--rw-r--r--   0 javv       (501) staff       (20)     1072 2023-06-16 12:04:34.000000 Mongeasy-0.1.9/setup.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-16 12:08:47.741997 Mongeasy-0.1.9/tests/
--rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 Mongeasy-0.1.9/tests/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)    13041 2023-06-16 10:09:31.000000 Mongeasy-0.1.9/tests/test_mongeasy.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.565595 mongeasy-0.2.0/
+-rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 mongeasy-0.2.0/LICENSE
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.486252 mongeasy-0.2.0/Mongeasy.egg-info/
+-rw-r--r--   0 javv       (501) staff       (20)    19200 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)     1070 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 javv       (501) staff       (20)       47 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/entry_points.txt
+-rw-r--r--   0 javv       (501) staff       (20)       15 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/requires.txt
+-rw-r--r--   0 javv       (501) staff       (20)       30 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/top_level.txt
+-rw-r--r--   0 javv       (501) staff       (20)    19200 2023-06-22 11:20:02.565718 mongeasy-0.2.0/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)    18389 2023-06-22 10:57:41.000000 mongeasy-0.2.0/README.md
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.517148 mongeasy-0.2.0/mongeasy/
+-rw-r--r--   0 javv       (501) staff       (20)      645 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/base_dict.py
+-rw-r--r--   0 javv       (501) staff       (20)     3557 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/connection.py
+-rw-r--r--   0 javv       (501) staff       (20)     4349 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/core.py
+-rw-r--r--   0 javv       (501) staff       (20)    14041 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/document.py
+-rw-r--r--   0 javv       (501) staff       (20)     2696 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/dynamics.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.518563 mongeasy-0.2.0/mongeasy/examples/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/examples/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/exceptions.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.523055 mongeasy-0.2.0/mongeasy/plugins/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     4101 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/plugins/registry.py
+-rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/resultlist.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.527867 mongeasy-0.2.0/mongeasy/utils/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/utils/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/utils/utils.py
+-rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 mongeasy-0.2.0/pyproject.toml
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.555198 mongeasy-0.2.0/sample_plugins/
+-rw-r--r--   0 javv       (501) staff       (20)      786 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)      366 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/connection_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      290 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/delete_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      299 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/init_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      576 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/pydantic_validator.py
+-rw-r--r--   0 javv       (501) staff       (20)      356 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/query_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      295 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/save_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      347 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/validator_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)     1013 2023-06-22 11:20:02.566931 mongeasy-0.2.0/setup.cfg
+-rw-r--r--   0 javv       (501) staff       (20)     1072 2023-06-22 10:57:41.000000 mongeasy-0.2.0/setup.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.564971 mongeasy-0.2.0/tests/
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 mongeasy-0.2.0/tests/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)    13161 2023-06-22 10:57:41.000000 mongeasy-0.2.0/tests/test_mongeasy.py
+-rw-r--r--   0 javv       (501) staff       (20)     2508 2023-06-22 10:57:41.000000 mongeasy-0.2.0/tests/test_plugins.py
```

### Comparing `Mongeasy-0.1.9/LICENSE` & `mongeasy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.9/mongeasy/base_dict.py` & `mongeasy-0.2.0/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.9/mongeasy/connection.py` & `mongeasy-0.2.0/mongeasy/connection.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,46 @@
-import yaml
 import os
+import import_string
+import yaml
 import pymongo
 from mongeasy.exceptions import MongeasyDBConnectionError
+from mongeasy.plugins.registry import Hook
+
 
 class MongeasyConnection:
-    def __init__(self, uri=None, database=None, connection_options=None):
+    def __init__(self, uri=None, database=None, connection_options=None, registry=None):
         self.uri = uri
         self.database = database
         self.connection_options = {} if connection_options is None else connection_options
         self.connection_options.setdefault('maxPoolSize', 100)
         self.connection_options.setdefault('retryWrites', True)
         self.connection_options.setdefault('retryReads', True)
         self.check_env()
         self.check_conf_file()
 
         if self.uri is None:
             raise ValueError("No connection string provided.")
         if self.database is None:
             raise ValueError("No database name provided.")
         
+        self.registry = registry
+
+        if registry is not None:
+                registry.dispatch(Hook.BEFORE_CONNECT)
+
         try:
             self.client = pymongo.MongoClient(self.uri, **self.connection_options)
             self.db = self.client[self.database]
         except (pymongo.errors.ConnectionFailure,
                 pymongo.errors.ServerSelectionTimeoutError,
                 pymongo.errors.ConfigurationError,
                 pymongo.errors.InvalidURI) as e:
             raise MongeasyDBConnectionError(f'Failed to connect to database: {e}')
-        
+        if registry is not None:
+                registry.dispatch(Hook.AFTER_CONNECT)
         
     def check_env(self):
         if self.uri is None:
             self.uri = os.environ.get('MONGOEASY_CONNECTION_STRING')
         if self.database is None:
             self.database = os.environ.get('MONGOEASY_DATABASE_NAME')
         if self.connection_options is None:
@@ -50,21 +59,33 @@
             if self.uri is None:
                 self.uri = db_config.get('uri', None)
             if self.database is None:
                 self.database = db_config.get('database', None)
             if self.connection_options is None:
                 self.connection_options = db_config.get('connection_options', None)
 
+            # Handle plugins
+            from mongeasy import registry
+            plugins_paths = config.get('plugins', [])
+            for plugin_path in plugins_paths:
+                plugin = import_string(plugin_path)()
+                registry.register_plugin(plugin)
+
+
     def connect(self, uri=None, database=None, connection_options=None):
         if uri is not None:
             self.uri = uri
         if database is not None:
             self.database = database
         if connection_options is not None:
             self.connection_options = connection_options
 
         self.client = pymongo.MongoClient(self.uri, **self.connection_options)
         self.db = self.client[self.database]
         return self.db
 
     def disconnect(self):
+        if self.registry is not None:
+                self.registry.dispatch(Hook.BEFORE_CLOSE)
         self.client.close()
+        if self.registry is not None:
+                self.registry.dispatch(Hook.AFTER_CLOSE)
```

### Comparing `Mongeasy-0.1.9/mongeasy/core.py` & `mongeasy-0.2.0/mongeasy/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,47 +43,37 @@
         number = Word(nums).setParseAction(lambda t: int(t[0]))
         string = QuotedString('"')
         value = string | number
 
         # Define the operators
         operators = ['>=', '<=', '==', '!=', 'in', 'not in', '<', '>']
         condition = Group(variable + Or(map(Literal, operators)) + value)       
+        
         # Define the operators
         expr = Forward()
         and_ = Literal('and')
         or_ = Literal('or')
         not_ = Literal('not')
         expr << infixNotation(condition, [(not_, 1, opAssoc.RIGHT, lambda t: {'$not': t[0][0]}), 
                                           (and_, 2, opAssoc.LEFT, lambda t: {'$and': [t[0][0], t[0][2]]}), 
                                           (or_, 2, opAssoc.LEFT, lambda t: {'$or': [t[0][0], t[0][2]]})])
 
-
         try:
             # Parse the query
             parsed_query = expr.parseString(self.query_str, parseAll=True)[0]
         except ParseException as e:
             raise ValueError(f"Invalid query string: {self.query_str}. Reason: {str(e)}")
 
         # Convert the parsed query into a MongoDB query
         try:
             mongo_query = self._to_mongo_query_rec(parsed_query)
         except Exception as e:
             raise ValueError(f"Failed to convert parsed query to MongoDB query. Reason: {str(e)}")
 
-        return mongo_query
-    
-
-    # def to_mongo_query(self):
-    #     try:
-    #         # ...rest of your code...
-    #         parsed_query = expr.parseString(self.query_str, parseAll=True)[0]
-    #         # ...rest of your code...
-    #     except ParseException as e:
-    #         raise ValueError(f"Invalid query string: {self.query_str}. Reason: {str(e)}")
-        
+        return mongo_query   
 
     def _to_mongo_query_rec(self, parsed_query):
         if isinstance(parsed_query, str):
             return parsed_query
         elif isinstance(parsed_query, ParseResults) and len(parsed_query) == 3:
             operator = parsed_query[1]
             if operator == '==':
```

### Comparing `Mongeasy-0.1.9/mongeasy/document.py` & `mongeasy-0.2.0/mongeasy/document.py`

 * *Files 26% similar despite different names*

```diff
@@ -20,31 +20,40 @@
 
 from datetime import datetime
 from copy import copy, deepcopy
 from typing import Union, List, Dict, Any
 import logging
 import json
 import bson
-from .exceptions import MongeasyDBCollectionError, MongeasyFieldError, MongeasyDBDocumentError, MongeasyIndexException
-from .base_dict import BaseDict
-from .core import Query
-from .resultlist import ResultList
+from mongeasy.exceptions import MongeasyDBCollectionError, MongeasyFieldError, MongeasyDBDocumentError, MongeasyIndexException
+from mongeasy.plugins.registry import Hook, plugin_dispatcher
+from mongeasy.base_dict import BaseDict
+from mongeasy.core import Query
+from mongeasy.resultlist import ResultList
 import pymongo
 
+
 class Document(BaseDict):
     """
     This class acts as the base class for collection classes. Each instance of the subclasses
     will represent a single document
     """
     collection = None
+    registry = None
     logger = logging.getLogger('mongeasy')
 
-    def __init__(self, *args, **kwargs):
+    @plugin_dispatcher([
+        {'hook': Hook.BEFORE_INIT_DOCUMENT, 'when': 'pre'},
+        {'hook': Hook.AFTER_INIT_DOCUMENT, 'when': 'post'},
+        {'hook': Hook.VALIDATE_DOCUMENT, 'when': 'pre'},
+        
+    ])
+    def __init__(self, *args,  **kwargs):
         super().__init__()
-
+        
         # Handle positional arguments
         if len(args) == 1 and isinstance(args[0], dict):
             as_dict = copy(args[0])
         elif len(args) == 0:
             as_dict = copy(kwargs)
         else:
             raise TypeError(f'Document() takes 1 positional argument or keyword arguments but {len(args) + len(kwargs)} were given')
@@ -84,41 +93,58 @@
 
     def is_saved(self) -> bool:
         """
         Checks if this document has been saved to the database
         :return: bool, True if the document has been saved, False otherwise
         """
         return not bool(self.has_changed())
-
+    
+    @plugin_dispatcher([
+        {'hook': Hook.BEFORE_SAVE_DOCUMENT, 'when': 'pre'},
+        {'hook': Hook.AFTER_SAVE_DOCUMENT, 'when': 'post'},
+        {'hook': Hook.VALIDATE_DOCUMENT, 'when': 'pre'},
+        ])
     def save(self):
         """
         Saves the current object to the database
         :return: The saved object
         """
         if self.collection is None:
             Document.logger.error("The collection does not exist")
             raise MongeasyDBCollectionError('The collection does not exist')
 
+        # Call the before_save hook
+        # if self.registry:
+        #     self.registry.dispatch(Hook.BEFORE_SAVE_DOCUMENT, self)
+
+
         # If _id is None, this is a new document
         if self._id is None:
             del self._id
             res = self.collection.insert_one(self.__dict__)
             self._id = res.inserted_id
+            
+            # if self.registry:
+            #     self.registry.dispatch(Hook.AFTER_SAVE_DOCUMENT, self)
             return self
 
         # if no fields have changed, return the document unchanged
         if not (changed_fields := self.has_changed()):
+            # if self.registry:
+            #     self.registry.dispatch(Hook.AFTER_SAVE_DOCUMENT, self)
             return self
 
         # update the document
         update_result = self.collection.update_one({'_id': self._id}, {'$set': changed_fields})
         if update_result.matched_count == 0:
             Document.logger.error(f"Document with _id {self._id} does not exist")
             raise MongeasyDBDocumentError(f"Document with _id {self._id} does not exist")
         else:
+            # if self.registry:
+            #     self.registry.dispatch(Hook.AFTER_SAVE_DOCUMENT, self)
             return self
 
     def reload(self):
         """
         Fetches the latest state of the document from the database and updates the current instance with the changes.
         """
         if self._id is None:
@@ -148,14 +174,18 @@
         try:
             self.collection.update_one({'_id': self._id}, {"$unset": {field: ""}})
         except Exception as e:
             Document.logger.error(f"Error deleting field '{field}' from document with id '{self._id}': {e}")
         else:
             Document.logger.info(f"Field '{field}' deleted from document with id '{self._id}'")
 
+    @plugin_dispatcher([
+        {'hook': Hook.BEFORE_DELETE_DOCUMENT, 'when': 'pre'},
+        {'hook': Hook.AFTER_DELETE_DOCUMENT, 'when': 'post'},
+        ])
     def delete(self):
         """
         Delete the current object from the database
         :return: None
         """
         if self.collection is None:
             raise MongeasyDBCollectionError('The collection does not exist')
@@ -254,14 +284,18 @@
         for item in items:
             try:
                 cls(item).save()
             except pymongo.errors.PyMongoError as e:
                 Document.logger.exception(f"Error inserting item: {item}. Exception: {e}")
 
     @classmethod
+    @plugin_dispatcher([
+        {'hook': Hook.BEFORE_QUERY_DOCUMENT, 'when': 'pre'},
+        {'hook': Hook.AFTER_QUERY_DOCUMENT, 'when': 'post'},
+        ])
     def find(cls, *args, **kwargs):
         """
         Find a document that matches the keywords
         :param arg: positional arguments
         :param kwargs: keyword arguments or dict to match
         :return: ResultList
         """
@@ -299,15 +333,19 @@
         Retrieve all documents from the collection as an iterator
         :yields: dict representation of next document
         """
         for item in cls.collection.find({}):
             yield cls(**item)
 
     @classmethod
-    def delete(cls, *args, **kwargs) -> None:
+    @plugin_dispatcher([
+        {'hook': Hook.BEFORE_DELETE_DOCUMENT, 'when': 'pre'},
+        {'hook': Hook.AFTER_DELETE_DOCUMENT, 'when': 'post'},
+    ])
+    def delete_many(cls, *args, **kwargs) -> None:
         """
         Delete the document that matches the keywords
 
         :param args: positional arguments
         :param kwargs: keyword arguments or dict to match
         :return: None
         """
```

### Comparing `Mongeasy-0.1.9/mongeasy/dynamics.py` & `mongeasy-0.2.0/mongeasy/dynamics.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 """
 import inspect
 from typing import Union
 from .utils.utils import pascal_to_snake
 from .document import Document
 from .exceptions import MongeasyValidationException, MongeasyFieldError
+from .plugins.registry import PluginRegistry
 
 
 def create_document_class(class_name: str, collection_name: str = None, base_classes: tuple = ()):
     """
     Dynamically create a document class and register it in the calling module's namespace.
     Args:
         class_name (str): Name of the class to create.
@@ -43,14 +44,14 @@
     # Dynamically generate the document class
     from . import connection
     if collection_name is None:
         collection_name = pascal_to_snake(class_name) + 's'
     
     # Create the collection object
     collection = connection.db[collection_name]
-    
-    doc_class = type(class_name, base_classes + (Document, ), {'collection':collection})
+    from mongeasy import registry
+    doc_class = type(class_name, base_classes + (Document, ), {'collection':collection, 'registry':registry})
 
     # Register the document class in the calling module's namespace
     setattr(calling_module, class_name, doc_class)
     
     return doc_class
```

### Comparing `Mongeasy-0.1.9/mongeasy/exceptions.py` & `mongeasy-0.2.0/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.9/mongeasy/resultlist.py` & `mongeasy-0.2.0/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.9/mongeasy/utils/utils.py` & `mongeasy-0.2.0/mongeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Mongeasy-0.1.9/setup.cfg` & `mongeasy-0.2.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mongeasy
-version = 0.1.9
+version = 0.2.0
 author = Joakim Wassberg
 author_email = joakim.wassberg@arthead.se
 description = Easy to use wrapper around pymongo for easy access to MongoDB.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/artheadsweden/mongeasy
 project_urls =
```

### Comparing `Mongeasy-0.1.9/setup.py` & `mongeasy-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
-    name="Mongeasy",
-    version="0.1.9",
+    name="mongeasy",
+    version="0.2.0",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
```

### Comparing `Mongeasy-0.1.9/tests/test_mongeasy.py` & `mongeasy-0.2.0/tests/test_mongeasy.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 """Tests for `mongeasy` package."""
 # Do this before importing mongeasy as it will try to connect to the database
 import os
 os.environ['MONGOEASY_CONNECTION_STRING'] = 'mongodb://localhost:27017'
 os.environ['MONGOEASY_DATABASE_NAME'] = 'mongeasy_pytest'
 from pymongo import MongoClient
 import pytest
-
-
 from mongeasy import create_document_class
+from mongeasy.exceptions import MongeasyDBDocumentError
 
 
 @pytest.fixture(scope='function')
 def clean_mongo():
     # Connect to MongoDB
     client = MongoClient('mongodb://localhost:27017')
     db = client['mongeasy_pytest']
@@ -156,17 +155,18 @@
     stored_user = User.find({'first_name': 'John'}).first()
     assert stored_user is None
 
 
 def test_document_delete_unsaved_document(clean_mongo):
     User = create_document_class('User', 'users')
     user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
-    user.delete()
-    stored_user = User.find({'first_name': 'John'}).first()
-    assert stored_user is None
+    with pytest.raises(MongeasyDBDocumentError):
+        user.delete()
+        stored_user = User.find({'first_name': 'John'}).first()
+        assert stored_user is None
 
 
 def test_document_to_json(clean_mongo):
     User = create_document_class('User', 'users')
     user = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
     user.save()
     json_user = user.to_json()
@@ -251,15 +251,15 @@
     User = create_document_class('User', 'users')
     user1 = User({'first_name': 'John', 'last_name': 'Doe', 'age': 30})
     user1.save()
     user2 = User({'first_name': 'Alice', 'last_name': 'Smith', 'age': 25})
     user2.save()
     user3 = User({'first_name': 'Bob', 'last_name': 'Jones', 'age': 35})
     user3.save()
-    User.delete({'first_name': 'Alice'})
+    User.delete_many({'first_name': 'Alice'})
     stored_users = User.all()
     assert len(stored_users) == 2
     assert user1.first_name in [user.first_name for user in stored_users]
     assert user2.first_name not in [user.first_name for user in stored_users]
     assert user3.first_name in [user.first_name for user in stored_users]
```

