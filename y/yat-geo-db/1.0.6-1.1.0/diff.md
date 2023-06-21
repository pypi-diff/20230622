# Comparing `tmp/yat_geo_db-1.0.6.tar.gz` & `tmp/yat_geo_db-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yat_geo_db-1.0.6.tar", last modified: Sat May  6 13:19:33 2023, max compression
+gzip compressed data, was "yat_geo_db-1.1.0.tar", last modified: Wed Jun 21 22:00:27 2023, max compression
```

## Comparing `yat_geo_db-1.0.6.tar` & `yat_geo_db-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 13:19:33.476481 yat_geo_db-1.0.6/
--rw-rw-rw-   0        0        0     1100 2022-12-26 18:53:07.000000 yat_geo_db-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     4880 2023-05-06 13:19:33.476481 yat_geo_db-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4214 2023-01-17 19:31:53.000000 yat_geo_db-1.0.6/README.md
--rw-rw-rw-   0        0        0      682 2023-05-06 13:18:55.000000 yat_geo_db-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 13:19:33.477492 yat_geo_db-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-05-06 13:18:55.000000 yat_geo_db-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:19:33.459929 yat_geo_db-1.0.6/yat_geo_db/
--rw-rw-rw-   0        0        0       60 2023-05-06 13:18:56.000000 yat_geo_db-1.0.6/yat_geo_db/__init__.py
--rw-rw-rw-   0        0        0     1011 2022-10-10 16:54:18.000000 yat_geo_db-1.0.6/yat_geo_db/fuzzy.py
--rw-rw-rw-   0        0        0    27570 2023-05-06 13:18:31.000000 yat_geo_db-1.0.6/yat_geo_db/geo_manager.py
--rw-rw-rw-   0        0        0     2321 2022-12-26 17:19:52.000000 yat_geo_db-1.0.6/yat_geo_db/geometry.py
--rw-rw-rw-   0        0        0      107 2022-12-28 17:50:48.000000 yat_geo_db-1.0.6/yat_geo_db/settings.py
--rw-rw-rw-   0        0        0      450 2022-12-26 17:21:13.000000 yat_geo_db-1.0.6/yat_geo_db/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-06 13:19:33.474974 yat_geo_db-1.0.6/yat_geo_db.egg-info/
--rw-rw-rw-   0        0        0     4880 2023-05-06 13:19:33.000000 yat_geo_db-1.0.6/yat_geo_db.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-05-06 13:19:33.000000 yat_geo_db-1.0.6/yat_geo_db.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 13:19:33.000000 yat_geo_db-1.0.6/yat_geo_db.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-06 13:19:33.000000 yat_geo_db-1.0.6/yat_geo_db.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-06 13:19:33.000000 yat_geo_db-1.0.6/yat_geo_db.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-01-11 17:08:51.000000 yat_geo_db-1.0.6/yat_geo_db.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-06-21 22:00:27.194497 yat_geo_db-1.1.0/
+-rw-rw-rw-   0        0        0     1100 2022-12-26 18:53:07.000000 yat_geo_db-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4944 2023-06-21 22:00:27.193498 yat_geo_db-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4278 2023-06-21 21:53:49.000000 yat_geo_db-1.1.0/README.md
+-rw-rw-rw-   0        0        0      682 2023-06-21 21:35:24.000000 yat_geo_db-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-21 22:00:27.194497 yat_geo_db-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-06-21 21:35:28.000000 yat_geo_db-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-21 22:00:27.168914 yat_geo_db-1.1.0/yat_geo_db/
+-rw-rw-rw-   0        0        0       60 2023-06-21 21:35:33.000000 yat_geo_db-1.1.0/yat_geo_db/__init__.py
+-rw-rw-rw-   0        0        0     1011 2022-10-10 16:54:18.000000 yat_geo_db-1.1.0/yat_geo_db/fuzzy.py
+-rw-rw-rw-   0        0        0    29558 2023-06-21 21:55:44.000000 yat_geo_db-1.1.0/yat_geo_db/geo_manager.py
+-rw-rw-rw-   0        0        0     2321 2022-12-26 17:19:52.000000 yat_geo_db-1.1.0/yat_geo_db/geometry.py
+-rw-rw-rw-   0        0        0      107 2022-12-28 17:50:48.000000 yat_geo_db-1.1.0/yat_geo_db/settings.py
+-rw-rw-rw-   0        0        0      450 2022-12-26 17:21:13.000000 yat_geo_db-1.1.0/yat_geo_db/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-21 22:00:27.192498 yat_geo_db-1.1.0/yat_geo_db.egg-info/
+-rw-rw-rw-   0        0        0     4944 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-21 22:00:27.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-01-11 17:08:51.000000 yat_geo_db-1.1.0/yat_geo_db.egg-info/zip-safe
```

### Comparing `yat_geo_db-1.0.6/LICENSE` & `yat_geo_db-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.6/PKG-INFO` & `yat_geo_db-1.1.0/yat_geo_db.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yat_geo_db
-Version: 1.0.6
+Name: yat-geo-db
+Version: 1.1.0
 Summary: A simple and effective Python wrapper around the Open Geo DB managed by YAT
 Home-page: https://github.com/yat-co/yat-geo-db
 Author: YAT, LLC
 Author-email: Robert Goss <rgoss@yat.ai>, Jarod Hart <jhart@yat.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/yat-co/yat-geo-db
 Project-URL: Bug Tracker, https://github.com/yat-co/yat-geo-db/issues
@@ -42,15 +42,17 @@
 
 Import and load data
 ```python
 from yat_geo_db import GeoManager as GeoManagerImport
 
 GeoManager = GeoManagerImport()
 
-GeoManager.load_data()
+GeoManager.load_data(
+    force_db_fetch= False, cache_local=True, compressed=True
+)
 ```
 
 Refresh local data (current version)
 
 ```python
 from yat_geo_db import GeoManager as GeoManagerImport
```

### Comparing `yat_geo_db-1.0.6/README.md` & `yat_geo_db-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 Import and load data
 ```python
 from yat_geo_db import GeoManager as GeoManagerImport
 
 GeoManager = GeoManagerImport()
 
-GeoManager.load_data()
+GeoManager.load_data(
+    force_db_fetch= False, cache_local=True, compressed=True
+)
 ```
 
 Refresh local data (current version)
 
 ```python
 from yat_geo_db import GeoManager as GeoManagerImport
```

### Comparing `yat_geo_db-1.0.6/pyproject.toml` & `yat_geo_db-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yat_geo_db"
-version = "1.0.6"
+version = "1.1.0"
 authors = [
   { name="Robert Goss", email="rgoss@yat.ai" },
   { name="Jarod Hart", email="jhart@yat.ai" },
 ]
 description = "A simple and effective Python wrapper around the Open Geo DB managed by YAT"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `yat_geo_db-1.0.6/setup.py` & `yat_geo_db-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 
 install_requires = ['requests', 'numpy', 'jellyfish', 'pytz']
 
 setup(
     name='yat_geo_db',
-    version='1.0.6',
+    version='1.1.0',
     author='YAT, LLC',
     author_email='rgoss@yat.ai, jhart@yat.ai',
     packages=['yat_geo_db'],
     license="MIT",
     url='https://github.com/yat-co/yat-geo-db',
     install_requires=install_requires,
     classifiers=[
```

### Comparing `yat_geo_db-1.0.6/yat_geo_db/fuzzy.py` & `yat_geo_db-1.1.0/yat_geo_db/fuzzy.py`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.6/yat_geo_db/geo_manager.py` & `yat_geo_db-1.1.0/yat_geo_db/geo_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .settings import BASE_STORE_URL
 from .utils import get_key
 
 from jellyfish import damerau_levenshtein_distance
 
 from datetime import datetime
 from collections import Counter
+import gzip
 import logging
 from math import log
 import os
 import json
 from pathlib import Path
 import pytz
 import re
@@ -465,14 +466,36 @@
         else:
             fuzzy_score = self.entity_fuzzy_score(search_str, source_str)
 
         if population <= 0 or fuzzy_score <= 0.65:
             return fuzzy_score * .9
         return (fuzzy_score * .9) + (log(population) * .1)
 
+    def best_fuzzy_search(self,
+                          search_entity: str,
+                          partition: str = None,
+                          score_threshold: float = .90,
+                          filters: Dict = None) -> Union[Dict, None]:
+        """
+        Wrapper around fuzzy_search to fetch the best result above a predefined
+        threshold.  Intended to be a Best Result Search
+        """
+        res_ls = self.fuzzy_search(
+            search_entity=search_entity, partition=partition, num_results=1,
+            filters=filters
+        )
+
+        # Return Best Result if above threshold
+        if len(res_ls) == 0:
+            return None
+        res = res_ls[0]
+        if res["score"] >= score_threshold:
+            return res
+        return None
+
     def fuzzy_search(self,
                      search_entity: str,
                      partition: str = None,
                      num_results: int = 50,
                      filters: Dict = None):
         """
         Sample values to compare against by passing the parameter `filters` to search
@@ -617,42 +640,76 @@
 
     def get_base_url(self, version: str = None):
         version_path = ''
         if version is not None:
             version_path = f"v/{version}/"
         return f"{BASE_STORE_URL}/{version_path}"
 
-    def load_data(self, version: str = None, force_db_fetch: bool = False, cache_local: bool = True):
+    def load_data(self,
+                  version: str = None,
+                  force_db_fetch: bool = False,
+                  cache_local: bool = True,
+                  compressed: bool = False):
+        """
+        Load Data
+        
+        Parameters
+        ------------
+            version str optional
+                Version of Geo Database Dump
+            force_db_fetch bool false
+                Force database refresh/fetch
+            cache_local bool true
+                Cache files locally, default is true
+            compressed bool false
+                To be depreciated for always true, fetch compressed files
+        """
         search_file_name = 'geo_manager_ngram_search.json'
         geo_shape_file_name = 'geo_manager_shape.json'
-        
+
+        fetch_search_file_name = search_file_name
+        fetch_geo_shape_file_name = geo_shape_file_name
+        if compressed:
+            fetch_search_file_name += ".gz"
+            fetch_geo_shape_file_name += ".gz"
+
         # Load Local
         local_path = os.path.join(self.data_dir, "geo_db", version or "current")
         if os.path.exists(local_path) and not force_db_fetch:
             with open(os.path.join(local_path, search_file_name), 'r') as f:
                 self.search_dict = json.load(f)
 
             with open(os.path.join(local_path, geo_shape_file_name), 'r') as f:
                 self.geo_shape_dict = json.load(f)
             
             # Radius Search
             self._generate_maps()
             return
         
         # Load Search File
-        response = requests.get(f'{self.get_base_url(version=version)}{search_file_name}')
+        response = requests.get(f'{self.get_base_url(version=version)}{fetch_search_file_name}')
         if response.status_code == 200: 
-            self.search_dict = response.json()
+            if compressed:
+                self.search_dict = json.loads(
+                    gzip.decompress(response.content).decode("utf-8")
+                )
+            else:
+                self.search_dict = response.json()
         else:
             raise ValueError(f"Unable to load search file reason={response.text}")
 
         # Load Shape File
-        response = requests.get(f'{self.get_base_url(version=version)}{geo_shape_file_name}')
+        response = requests.get(f'{self.get_base_url(version=version)}{fetch_geo_shape_file_name}')
         if response.status_code == 200: 
-            self.geo_shape_dict = response.json()
+            if compressed:
+                self.geo_shape_dict = json.loads(
+                    gzip.decompress(response.content).decode("utf-8")
+                )
+            else:
+                self.geo_shape_dict = response.json()
         else:
             raise ValueError(f"Unable to load shape file reason={response.text}")
 
         # Cache Files to Local Disk
         if cache_local:
             Path(local_path).mkdir(parents=True, exist_ok=True)
             # Write to local
```

### Comparing `yat_geo_db-1.0.6/yat_geo_db/geometry.py` & `yat_geo_db-1.1.0/yat_geo_db/geometry.py`

 * *Files identical despite different names*

### Comparing `yat_geo_db-1.0.6/yat_geo_db.egg-info/PKG-INFO` & `yat_geo_db-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yat-geo-db
-Version: 1.0.6
+Name: yat_geo_db
+Version: 1.1.0
 Summary: A simple and effective Python wrapper around the Open Geo DB managed by YAT
 Home-page: https://github.com/yat-co/yat-geo-db
 Author: YAT, LLC
 Author-email: Robert Goss <rgoss@yat.ai>, Jarod Hart <jhart@yat.ai>
 License: MIT
 Project-URL: Homepage, https://github.com/yat-co/yat-geo-db
 Project-URL: Bug Tracker, https://github.com/yat-co/yat-geo-db/issues
@@ -42,15 +42,17 @@
 
 Import and load data
 ```python
 from yat_geo_db import GeoManager as GeoManagerImport
 
 GeoManager = GeoManagerImport()
 
-GeoManager.load_data()
+GeoManager.load_data(
+    force_db_fetch= False, cache_local=True, compressed=True
+)
 ```
 
 Refresh local data (current version)
 
 ```python
 from yat_geo_db import GeoManager as GeoManagerImport
```

