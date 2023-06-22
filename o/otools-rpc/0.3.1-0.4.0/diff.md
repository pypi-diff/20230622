# Comparing `tmp/otools-rpc-0.3.1.tar.gz` & `tmp/otools-rpc-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otools-rpc-0.3.1.tar", last modified: Tue Jun 20 08:50:11 2023, max compression
+gzip compressed data, was "otools-rpc-0.4.0.tar", last modified: Thu Jun 22 08:39:52 2023, max compression
```

## Comparing `otools-rpc-0.3.1.tar` & `otools-rpc-0.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1326 2023-05-30 13:44:29.000000 otools-rpc-0.3.1/LICENSE.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     4072 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     3450 2023-05-30 13:44:29.000000 otools-rpc-0.3.1/README.md
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.214897 otools-rpc-0.3.1/otools_rpc/
--rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.3.1/otools_rpc/__init__.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/otools_rpc/db_manager/
--rw-r--r--   0 opennet   (1000) opennet   (1000)       38 2023-05-30 12:59:41.000000 otools-rpc-0.3.1/otools_rpc/db_manager/__init__.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1168 2023-05-30 13:44:29.000000 otools-rpc-0.3.1/otools_rpc/db_manager/database_utils.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/otools_rpc/external_api/
--rw-r--r--   0 opennet   (1000) opennet   (1000)       62 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/__init__.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     3402 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/cache.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1969 2023-06-16 14:20:26.000000 otools-rpc-0.3.1/otools_rpc/external_api/common.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     5257 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/environment.py
--rw-r--r--   0 opennet   (1000) opennet   (1000)     6930 2023-06-20 08:47:34.000000 otools-rpc-0.3.1/otools_rpc/external_api/recordset.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/otools_rpc.egg-info/
--rw-r--r--   0 opennet   (1000) opennet   (1000)     4072 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/PKG-INFO
--rw-r--r--   0 opennet   (1000) opennet   (1000)      475 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/SOURCES.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/dependency_links.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       63 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/requires.txt
--rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-06-20 08:50:11.000000 otools-rpc-0.3.1/otools_rpc.egg-info/top_level.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-06-20 08:50:11.218897 otools-rpc-0.3.1/setup.cfg
--rw-r--r--   0 opennet   (1000) opennet   (1000)     1047 2023-06-20 08:47:33.000000 otools-rpc-0.3.1/setup.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-22 08:39:52.979374 otools-rpc-0.4.0/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1326 2023-05-30 13:44:29.000000 otools-rpc-0.4.0/LICENSE.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     4072 2023-06-22 08:39:52.979374 otools-rpc-0.4.0/PKG-INFO
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     3450 2023-05-30 13:44:29.000000 otools-rpc-0.4.0/README.md
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-22 08:39:52.979374 otools-rpc-0.4.0/otools_rpc/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.4.0/otools_rpc/__init__.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-22 08:39:52.979374 otools-rpc-0.4.0/otools_rpc/db_manager/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       38 2023-05-30 12:59:41.000000 otools-rpc-0.4.0/otools_rpc/db_manager/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1168 2023-05-30 13:44:29.000000 otools-rpc-0.4.0/otools_rpc/db_manager/database_utils.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-22 08:39:52.979374 otools-rpc-0.4.0/otools_rpc/external_api/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       95 2023-06-21 14:02:09.000000 otools-rpc-0.4.0/otools_rpc/external_api/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     6060 2023-06-22 08:37:36.000000 otools-rpc-0.4.0/otools_rpc/external_api/cache.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     2085 2023-06-21 14:02:09.000000 otools-rpc-0.4.0/otools_rpc/external_api/common.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     3994 2023-06-22 08:37:36.000000 otools-rpc-0.4.0/otools_rpc/external_api/environment.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     7046 2023-06-21 14:02:09.000000 otools-rpc-0.4.0/otools_rpc/external_api/recordset.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-06-22 08:39:52.979374 otools-rpc-0.4.0/otools_rpc.egg-info/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     4072 2023-06-22 08:39:52.000000 otools-rpc-0.4.0/otools_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      475 2023-06-22 08:39:52.000000 otools-rpc-0.4.0/otools_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-06-22 08:39:52.000000 otools-rpc-0.4.0/otools_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       63 2023-06-22 08:39:52.000000 otools-rpc-0.4.0/otools_rpc.egg-info/requires.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-06-22 08:39:52.000000 otools-rpc-0.4.0/otools_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-06-22 08:39:52.979374 otools-rpc-0.4.0/setup.cfg
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1047 2023-06-22 08:38:01.000000 otools-rpc-0.4.0/setup.py
```

### Comparing `otools-rpc-0.3.1/LICENSE.txt` & `otools-rpc-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.3.1/PKG-INFO` & `otools-rpc-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.3.1
+Version: 0.4.0
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `otools-rpc-0.3.1/README.md` & `otools-rpc-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.3.1/otools_rpc/db_manager/database_utils.py` & `otools-rpc-0.4.0/otools_rpc/db_manager/database_utils.py`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.3.1/otools_rpc/external_api/common.py` & `otools-rpc-0.4.0/otools_rpc/external_api/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,16 +22,18 @@
             return fn(self, other)
         return wrapper
     return decorator
 
 def cache(op=None):
     def decorator(fn):
         def wrapper(self, *args, **kwargs):
-            self.env.logger.log("FTRACE", f"[CACHE] {op or fn.__name__} on {self}")
-            return fn(self, *args, **kwargs)
+            res = fn(self, *args, **kwargs)
+            self.env.logger.log("FTRACE", f"[CACHE] {op or fn.__name__} on {self} {args} {kwargs}")
+            self.env.cache[self._name].update(op, self, res, *args, **kwargs)
+            return res
         return wrapper
     return decorator
 
 
 
 # --------------------------------------------
 #               frozendict stuff
```

### Comparing `otools-rpc-0.3.1/otools_rpc/external_api/environment.py` & `otools-rpc-0.4.0/otools_rpc/external_api/environment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,69 +1,61 @@
 import sys
 import xmlrpc.client
 import re
-import copy
-from typing import Union
 from loguru import logger as loguru_logger
 from .recordset import RecordSet
 from .common import frozendict
 from .cache import Cache
 
 
 class Environment(dict):
-    # Todo: Add a cache system
 
     def __init__(
             self,
             url: str,
             username: str,
             password: str,
             db: str = None,
             auto_auth: bool = True,
             logger: loguru_logger = None,
             log_level: str = None,
+
+            cache_default_expiration: int = 10,
             **kw
     ):
         super().__init__(**kw)
 
         self._url = url[:-1] if url[-1] == "/" else url
         self._username = username
         self._password = password
         self._db = db or self._extract_db_from_url()
 
+        # We need logger first
+        self.logger = logger if isinstance(logger, type(loguru_logger)) else loguru_logger
+        if logger is None:
+            self.logger.remove()
+            self.logger.add(sys.stderr, level=log_level or "INFO")
+        self.logger.level("FTRACE", no=3, color="<blue>")
+
         self.common = xmlrpc.client.ServerProxy(f"{self._url}/xmlrpc/2/common", allow_none=True)
         self.models = None
 
         self.requests = list()
-        # self.cache = Cache(self)
-        self.cache = dict()
+        self.cache = Cache(self, cache_default_expiration)
         self._context = frozendict()
 
         # Todo: make it an object
         self.user = None
 
-        self.logger = logger if isinstance(logger, type(loguru_logger)) else loguru_logger
-        if logger is None:
-            self.logger.remove()
-            self.logger.level("FTRACE", no=3, color="<blue>")
-            self.logger.add(sys.stderr, level=log_level or "INFO")
 
         if auto_auth:
             self.authenticate()
 
     def __missing__(self, key):
-        res = RecordSet(key, self, context=self._context)
-        if self._has_missing_cache(key):
-            self.cache.update({
-                key: {
-                    'fields': res.fields_get(),
-                    'records': dict(),
-                }
-            })
-        return res
+        return RecordSet(key, self, context=self._context)
 
     def __getitem__(self, key):
         assert self.user or key == 'res.users', "You must be authenticated to access models"
         return super(Environment, self).__getitem__(key)
 
     def __str__(self):
         return f"{self.__class__.__name__}<{id(self)}>"
@@ -135,35 +127,7 @@
 
     def _extract_db_from_url(self, url: str = None) -> str:
         url = url or self._url
         db_re = r"(https?:\/\/)?([w]{3}\.)?([\w-]*)(.\w*)([\/\w]*)"
         return re.search(db_re, url).group(3)
 
 
-
-    # --------------------------------------------
-    #                   CACHE
-    # --------------------------------------------
-
-
-    def _has_missing_cache(self, key):
-        return key not in self.cache
-
-    def _update_cache_records(self, key, vals_dict: dict):
-        self.cache[key]['records'].update(vals_dict)
-
-    def update_cache_records(self, key: str, vals_list: list):
-        """ Transform a read or search_read result into a usable dict and update the cache """
-        vals_dict = dict()
-        for r in copy.deepcopy(vals_list):
-            i = r.pop('id')
-            vals_dict[i] = r
-        self._update_cache_records(key, vals_dict)
-
-    def delete_cached_records(self, key: str, ids: Union[int, list[int]]):
-        ids = ids if isinstance(ids, list) else [ids]
-        for i in ids:
-            self.cache[key]['records'].pop(i)
-
-    # def get_cached_value(self, key: str, ids: Union[int, list] = None):
-    #     ids = ids if isinstance(ids, list) else [ids]
-    #     return self.cache[key]['records']
```

### Comparing `otools-rpc-0.3.1/otools_rpc/external_api/recordset.py` & `otools-rpc-0.4.0/otools_rpc/external_api/recordset.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,16 @@
     def __getitem__(self, item):
         if isinstance(item, slice):
             return self._recordset(self._ids[item])
         elif isinstance(item, str):
             return getattr(self, item)
 
     def __getattr__(self, attr):
-        if attr in self._env.cache.get(self._name, dict()).get('fields', list()):
-            # Todo: code this instead of having a weird patch
-            # self.ensure_one()
-            return self._env.cache[self._name]['records'].get(self.id, dict()).get(attr, False)
+        if attr != 'fields_get' and self._env.cache[self._name].field_exists(attr):
+            return self._env.cache[self._name][self.id][attr].get()
         else:
             def wrapper(*args, **kw):
                 return self._execute(attr, *args, **kw)
             return wrapper
 
     # --- Operators ---
     @assert_same_model('union')
@@ -159,61 +157,72 @@
 
 
     @model
     def search(self, domain: list[tuple], **kw):
         ids = self._execute('search', self._format_domain(domain), **kw)
         return self._recordset(ids)
 
+    @cache('read')
     def read(self, fields: list[str] = None, **kw):
         fields = fields or list()
         res = self._execute('read', fields=fields, **kw)
-        self._env.update_cache_records(self._name, res)
         return res
 
     @model
     def search_read(self, domain: list[tuple], fields: list[str] = None, **kw):
         fields = fields or list()
         res = self._execute('search_read', self._format_domain(domain), fields=fields, **kw)
-        self._env.update_cache_records(self._name, res)
         return self._recordset([r.get('id') for r in res])
 
     @model
     def search_count(self, domain: list[tuple]):
         return self._execute('search_count', self._format_domain(domain))
 
     @model
     @cache('create')
     def create(self, vals_list: Union[dict, list[dict]]):
         vals_list = vals_list if isinstance(vals_list, list) else [vals_list]
         ids = self._execute('create', vals_list)
         return self._recordset(ids)
 
+    @cache('write')
     def write(self, vals: dict):
         return self._execute('write', vals)
 
     @cache('delete')
     def unlink(self):
         res = self._execute('unlink')
-        # if res:
-        #     self._env.delete_cached_records(self._name, self._ids)
         return res
 
     def copy(self):
         res_id = self._execute('copy')
         return self._recordset(res_id)
 
 
     # --- ORM helpers ---
 
 
     def mapped(self, field: str):
+        """ Perform a read only if any of the record has dirty cache """
+        if self.cache_expired(field):
+            self.read([field])
         return [getattr(rec, field) for rec in self]
 
     def filtered(self, func: Union[callable, str]):
         if isinstance(func, str):
             name = func
             func = lambda rec: rec[name]
             # func = lambda rec: any(rec.mapped(name))      # Odoo behavior
         return self.browse([rec.id for rec in self if func(rec)])
 
     def filtered_domain(self, domain: list[tuple]):
         return self.search([('id', 'in', self.ids)] + domain)
+
+
+
+    # --------------------------------------------
+    #              CACHE HELPERS
+    # --------------------------------------------
+
+
+    def cache_expired(self, field: str):
+        return self.env.cache[self._name].cache_expired(field, self.ids)
```

### Comparing `otools-rpc-0.3.1/otools_rpc.egg-info/PKG-INFO` & `otools-rpc-0.4.0/otools_rpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.3.1
+Version: 0.4.0
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `otools-rpc-0.3.1/setup.py` & `otools-rpc-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="otools-rpc",
-    version="0.3.1",
+    version="0.4.0",
     description="A tool to interact with Odoo's external API.",
     packages=find_packages(exclude=["tests"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MrFaBemol/otools-rpc",
     author="Gautier Casabona",
     author_email="gcasabona.pro@gmail.com",
```

