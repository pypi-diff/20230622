# Comparing `tmp/eodc-2023.6.4.tar.gz` & `tmp/eodc-2023.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc-2023.6.4.tar", max compression
+gzip compressed data, was "eodc-2023.6.5.tar", max compression
```

## Comparing `eodc-2023.6.4.tar` & `eodc-2023.6.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      513 2023-06-21 12:47:52.984963 eodc-2023.6.4/README.md
--rw-r--r--   0        0        0      213 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/__init__.py
--rw-r--r--   0        0        0     1102 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/dask.py
--rw-r--r--   0        0        0     9399 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/faas.py
--rw-r--r--   0        0        0      469 2023-06-21 12:47:52.984963 eodc-2023.6.4/eodc/settings.py
--rw-r--r--   0        0        0     1208 2023-06-21 12:47:52.984963 eodc-2023.6.4/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 eodc-2023.6.4/PKG-INFO
+-rw-r--r--   0        0        0      513 2023-06-22 12:02:20.709724 eodc-2023.6.5/README.md
+-rw-r--r--   0        0        0      213 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/__init__.py
+-rw-r--r--   0        0        0     1102 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/dask.py
+-rw-r--r--   0        0        0     9754 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/faas.py
+-rw-r--r--   0        0        0      469 2023-06-22 12:02:20.709724 eodc-2023.6.5/eodc/settings.py
+-rw-r--r--   0        0        0     1204 2023-06-22 12:02:20.709724 eodc-2023.6.5/pyproject.toml
+-rw-r--r--   0        0        0     1759 1970-01-01 00:00:00.000000 eodc-2023.6.5/PKG-INFO
```

### Comparing `eodc-2023.6.4/README.md` & `eodc-2023.6.5/README.md`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.4/eodc/dask.py` & `eodc-2023.6.5/eodc/dask.py`

 * *Files identical despite different names*

### Comparing `eodc-2023.6.4/eodc/faas.py` & `eodc-2023.6.5/eodc/faas.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,16 +235,23 @@
     ):
         return super().submit_workflow(
             openeo_executor_parameters=openeo_parameters.json(),
             openeo_user_id=openeo_user_id,
             openeo_job_id=openeo_job_id,
         )
 
-    def get_output_stac_items(self):
-        raise NotImplementedError()
+    def get_output_stac_items(self, openeo_parameters: OpenEOExecutorParameters):
+        collection_file = list(openeo_parameters.stac_path.glob("*_collection.json"))[0]
+        openeo_output_collection = Collection.from_file(str(collection_file))
+        stac_items = [
+            Item.from_file(link.get_absolute_href())
+            for link in openeo_output_collection.get_item_links()
+        ]
+
+        return stac_items
 
 
 class Snap(FaasProcessorBase):
     @classmethod
     def get_instance(cls):
         return cls(processor_details=FaasProcessor.Snap.value)
```

### Comparing `eodc-2023.6.4/pyproject.toml` & `eodc-2023.6.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc"
-version = "2023.6.4"
+version = "2023.6.5"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -23,15 +23,15 @@
 python = ">=3.9,<3.12"
 requests = "^2.28.2"
 pydantic = "^1.10.7"
 argo-workflows = "6.3.9"
 dask-gateway = "^2022.11.0"
 eodc-faas-force = "2023.6.2"
 eodc-faas-sen2like = "2023.6.2"
-eodc-faas-openeo = "^2023.6.5rc1"
+eodc-faas-openeo = "2023.6.6"
 pystac = "^1.7.3"
 eodc-faas-snap = "^2023.6.2"
 pyproj = "^3.6.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.0"
 pytest = "^7.2.2"
```

### Comparing `eodc-2023.6.4/PKG-INFO` & `eodc-2023.6.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc
-Version: 2023.6.4
+Version: 2023.6.5
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.9,<3.12
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: argo-workflows (==6.3.9)
 Requires-Dist: dask-gateway (>=2022.11.0,<2023.0.0)
 Requires-Dist: eodc-faas-force (==2023.6.2)
-Requires-Dist: eodc-faas-openeo (>=2023.6.5rc1,<2024.0.0)
+Requires-Dist: eodc-faas-openeo (==2023.6.6)
 Requires-Dist: eodc-faas-sen2like (==2023.6.2)
 Requires-Dist: eodc-faas-snap (>=2023.6.2,<2024.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: pyproj (>=3.6.0,<4.0.0)
 Requires-Dist: pystac (>=1.7.3,<2.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Project-URL: Repository, https://github.com/eodcgmbh/eodc-sdk
```

