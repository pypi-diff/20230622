# Comparing `tmp/stac_collection_search-0.0.4.tar.gz` & `tmp/stac_collection_search-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_collection_search-0.0.4.tar", last modified: Wed Jun 21 18:52:10 2023, max compression
+gzip compressed data, was "stac_collection_search-0.0.5.tar", last modified: Wed Jun 21 21:30:55 2023, max compression
```

## Comparing `stac_collection_search-0.0.4.tar` & `stac_collection_search-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:52:10.322627 stac_collection_search-0.0.4/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 18:52:10.318627 stac_collection_search-0.0.4/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      946 2023-06-21 17:54:21.000000 stac_collection_search-0.0.4/README.md
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-21 18:52:10.322627 stac_collection_search-0.0.4/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-06-21 18:51:33.000000 stac_collection_search-0.0.4/setup.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:52:10.318627 stac_collection_search-0.0.4/stac_collection_search/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       83 2023-06-21 18:14:31.000000 stac_collection_search-0.0.4/stac_collection_search/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     4006 2023-06-21 18:46:42.000000 stac_collection_search-0.0.4/stac_collection_search/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 18:52:10.318627 stac_collection_search-0.0.4/stac_collection_search.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1425 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      314 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/requires.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-06-21 18:52:10.000000 stac_collection_search-0.0.4/stac_collection_search.egg-info/top_level.txt
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 21:30:55.217773 stac_collection_search-0.0.5/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1094 2023-06-21 21:29:21.000000 stac_collection_search-0.0.5/LICENSE.md
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1450 2023-06-21 21:30:55.217773 stac_collection_search-0.0.5/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      946 2023-06-21 17:54:21.000000 stac_collection_search-0.0.5/README.md
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-21 21:30:55.217773 stac_collection_search-0.0.5/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-06-21 21:30:51.000000 stac_collection_search-0.0.5/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 21:30:55.213773 stac_collection_search-0.0.5/stac_collection_search/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       83 2023-06-21 18:14:31.000000 stac_collection_search-0.0.5/stac_collection_search/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     4253 2023-06-21 21:26:10.000000 stac_collection_search-0.0.5/stac_collection_search/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-21 21:30:55.217773 stac_collection_search-0.0.5/stac_collection_search.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1450 2023-06-21 21:30:55.000000 stac_collection_search-0.0.5/stac_collection_search.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      325 2023-06-21 21:30:55.000000 stac_collection_search-0.0.5/stac_collection_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-21 21:30:55.000000 stac_collection_search-0.0.5/stac_collection_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-06-21 21:30:55.000000 stac_collection_search-0.0.5/stac_collection_search.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-06-21 21:30:55.000000 stac_collection_search-0.0.5/stac_collection_search.egg-info/top_level.txt
```

### Comparing `stac_collection_search-0.0.4/PKG-INFO` & `stac_collection_search-0.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: stac_collection_search
-Version: 0.0.4
+Version: 0.0.5
 Summary: STAC Collection Search helper utility
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 Keywords: python,azure,stac,fastapi,eo,earth observation,spatial,search,collection
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 
 # STAC Collection Search
 Quick utility which enables you to search for STAC collections with a given bbox and datetime extent.
 
 ## How to use
```

### Comparing `stac_collection_search-0.0.4/README.md` & `stac_collection_search-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `stac_collection_search-0.0.4/setup.py` & `stac_collection_search-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'STAC Collection Search helper utility'
 LONG_DESCRIPTION = 'STAC Collection Search helper which enables a collection search on the stac-fastapi'
 
 requirements = []
 requirements_file = "./requirements.txt"
 if os.path.isfile(requirements_file):
     with open(requirements_file) as f:
```

### Comparing `stac_collection_search-0.0.4/stac_collection_search/utils.py` & `stac_collection_search-0.0.5/stac_collection_search/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,67 +45,69 @@
     if timestamp is None:
         return None
     for fmt in [
         "%Y-%m-%dT%H:%M:%S%Z",
         "%Y-%m-%dT%H:%M:%S%z",
         "%Y-%m-%dT%H:%M:%S.%f%z",
         "%Y-%m-%dT%H:%M:%S.%f",
+        "%Y-%m-%dT%H:%M:%S",
     ]:
         try:
             return datetime.datetime.strptime(timestamp, fmt)
         except ValueError:
             continue
     raise ValueError(f"timestamp {timestamp} does not match any known formats")
 
 
 def search_collections(
     collection_json_dict: dict,
     spatial_extent: shapely.geometry.Polygon = None,
     temporal_extent_start=None,
     temporal_extent_end=None,
 ) -> List[Dict[AnyStr, Any]]:
-    # Ensure that temporal_extent_start and temporal_extent_end are timezone-aware (in UTC)
-    if temporal_extent_start and temporal_extent_start.tzinfo is None:
-        temporal_extent_start = temporal_extent_start.replace(
-            tzinfo=datetime.timezone.utc
-        )
-    if temporal_extent_end and temporal_extent_end.tzinfo is None:
-        temporal_extent_end = temporal_extent_end.replace(tzinfo=datetime.timezone.utc)
-
     collection_list = _get_collections(collection_json_dict)
-
-    # First, we filter by spatial extent
     collections_spatially_filtered = (
         [
             collection
             for collection in collection_list
             if spatial_extent.intersects(collection["spatial_extent"])
         ]
         if spatial_extent
         else collection_list
     )
-
-    # Now we apply time-based filter on spatially filtered collections
-    ids = [
-        collection["id"]
-        for collection in collections_spatially_filtered
-        if (
-            temporal_extent_start is None
-            or collection["temporal_extent"]["end"] is None
-            or collection["temporal_extent"]["end"] >= temporal_extent_start
-        )
-        and (
-            temporal_extent_end is None
-            or collection["temporal_extent"]["start"] is None
-            or collection["temporal_extent"]["start"] <= temporal_extent_end
-        )
-    ]
+    ids = []
+    for collection in collections_spatially_filtered:
+        try: 
+            if (
+                temporal_extent_start is None
+                or collection["temporal_extent"]["end"] is None
+                or collection["temporal_extent"]["end"] >= temporal_extent_start
+            ) and (
+                temporal_extent_end is None
+                or collection["temporal_extent"]["start"] is None
+                or collection["temporal_extent"]["start"] <= temporal_extent_end
+            ):
+                ids.append(collection["id"])
+        except TypeError:
+            temporal_extent_start_utc = temporal_extent_start.replace(tzinfo=datetime.timezone.utc)
+            temporal_extent_end_utc = temporal_extent_end.replace(tzinfo=datetime.timezone.utc)
+            if (
+                temporal_extent_start is None
+                or collection["temporal_extent"]["end"] is None
+                or collection["temporal_extent"]["end"] >= temporal_extent_start_utc
+            ) and (
+                temporal_extent_end is None
+                or collection["temporal_extent"]["start"] is None
+                or collection["temporal_extent"]["start"] <= temporal_extent_end_utc
+            ):
+                ids.append(collection["id"])
     return ids
 
 
+
 def search_collections_verbose(
     collection_json_dict: dict,
     spatial_extent: shapely.geometry.Polygon = None,
     temporal_extent_start=None,
     temporal_extent_end=None,
 ) -> List[AnyStr]:
```

### Comparing `stac_collection_search-0.0.4/stac_collection_search.egg-info/PKG-INFO` & `stac_collection_search-0.0.5/stac_collection_search.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: stac-collection-search
-Version: 0.0.4
+Version: 0.0.5
 Summary: STAC Collection Search helper utility
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
 Keywords: python,azure,stac,fastapi,eo,earth observation,spatial,search,collection
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 
 # STAC Collection Search
 Quick utility which enables you to search for STAC collections with a given bbox and datetime extent.
 
 ## How to use
```

