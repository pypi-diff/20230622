# Comparing `tmp/macrometa-source-collection-0.0.51.tar.gz` & `tmp/macrometa-source-collection-0.0.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.51.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.52.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.51.tar` & `macrometa-source-collection-0.0.52.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    11137 2023-06-19 03:18:54.842554 macrometa-source-collection-0.0.51/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0    10129 2023-06-19 03:18:54.842554 macrometa-source-collection-0.0.51/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1626 2023-06-19 03:18:55.094558 macrometa-source-collection-0.0.51/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.51/setup.py
--rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.51/PKG-INFO
+-rw-r--r--   0        0        0    11137 2023-06-22 10:25:12.576261 macrometa-source-collection-0.0.52/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0    10153 2023-06-22 10:25:12.576261 macrometa-source-collection-0.0.52/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1626 2023-06-22 10:25:12.892263 macrometa-source-collection-0.0.52/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.52/setup.py
+-rw-r--r--   0        0        0     1160 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.52/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.51/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.52/macrometa_source_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.51/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.52/macrometa_source_collection/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             "https",
             host=self._host,
             port=443,
             geofabric=self._fabric,
             apikey=_apikey
         )
         self._auth = pulsar.AuthenticationToken(_apikey)
-        self._tenant = os.getenv('GDN_TENANT')
+        self._tenant = os.getenv('MACROMETA_SOURCE_COLLECTION_TENANT')
         try:
             # try to enable collection stream on the source collection.
             self._c8_client.update_collection_properties(self._collection, has_stream=True)
         except:
             pass
 
         self.exported_bytes = Counter("exported_bytes", "Total number of bytes exported from GDN collections", ['region', 'tenant', 'fabric', 'workflow'])
```

### Comparing `macrometa-source-collection-0.0.51/pyproject.toml` & `macrometa-source-collection-0.0.52/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.51'
+version='0.0.52'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.51/setup.py` & `macrometa-source-collection-0.0.52/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.51',
+    'version': '0.0.52',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.51/PKG-INFO` & `macrometa-source-collection-0.0.52/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.51
+Version: 0.0.52
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

