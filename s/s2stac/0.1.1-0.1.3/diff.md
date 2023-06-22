# Comparing `tmp/s2stac-0.1.1.tar.gz` & `tmp/s2stac-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s2stac-0.1.1.tar", max compression
+gzip compressed data, was "s2stac-0.1.3.tar", max compression
```

## Comparing `s2stac-0.1.1.tar` & `s2stac-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1071 2023-05-12 11:45:52.630479 s2stac-0.1.1/LICENSE
--rw-r--r--   0        0        0     2706 2023-06-02 15:15:37.888859 s2stac-0.1.1/README.md
--rw-r--r--   0        0        0      843 2023-06-02 15:24:35.301230 s2stac-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      257 2023-06-02 14:18:31.109651 s2stac-0.1.1/src/s2stac/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-02 14:01:10.199802 s2stac-0.1.1/src/s2stac/_asset.py
--rw-r--r--   0        0        0     2083 2023-06-02 14:04:14.981564 s2stac-0.1.1/src/s2stac/_aux_data.py
--rw-r--r--   0        0        0     5341 2023-06-02 14:11:15.429545 s2stac-0.1.1/src/s2stac/_catalog.py
--rw-r--r--   0        0        0     1897 2023-06-02 14:12:37.734322 s2stac-0.1.1/src/s2stac/_img_data.py
--rw-r--r--   0        0        0     8005 2023-06-02 14:11:18.809577 s2stac-0.1.1/src/s2stac/_mtd_tl.py
--rw-r--r--   0        0        0     2147 2023-06-02 13:07:54.221429 s2stac-0.1.1/src/s2stac/_preview.py
--rw-r--r--   0        0        0     5299 2023-06-02 14:07:20.715326 s2stac-0.1.1/src/s2stac/_qi_data.py
--rw-r--r--   0        0        0     1347 2023-06-02 14:24:16.588701 s2stac-0.1.1/src/s2stac/_stacify.py
--rw-r--r--   0        0        0     4016 1970-01-01 00:00:00.000000 s2stac-0.1.1/setup.py
--rw-r--r--   0        0        0     3916 1970-01-01 00:00:00.000000 s2stac-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-12 11:45:52.630479 s2stac-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3922 2023-06-09 14:47:23.109769 s2stac-0.1.3/README.md
+-rw-r--r--   0        0        0      928 2023-06-22 11:55:54.498608 s2stac-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-06-02 14:18:31.109651 s2stac-0.1.3/src/s2stac/__init__.py
+-rw-r--r--   0        0        0     1547 2023-06-02 14:01:10.199802 s2stac-0.1.3/src/s2stac/_asset.py
+-rw-r--r--   0        0        0     2083 2023-06-22 07:43:44.951124 s2stac-0.1.3/src/s2stac/_aux_data.py
+-rw-r--r--   0        0        0     6300 2023-06-09 14:34:47.515390 s2stac-0.1.3/src/s2stac/_catalog.py
+-rw-r--r--   0        0        0     1897 2023-06-02 14:12:37.734322 s2stac-0.1.3/src/s2stac/_img_data.py
+-rw-r--r--   0        0        0     8005 2023-06-12 15:58:47.760733 s2stac-0.1.3/src/s2stac/_mtd_tl.py
+-rw-r--r--   0        0        0     2147 2023-06-02 13:07:54.221429 s2stac-0.1.3/src/s2stac/_preview.py
+-rw-r--r--   0        0        0     5299 2023-06-12 16:11:47.744852 s2stac-0.1.3/src/s2stac/_qi_data.py
+-rw-r--r--   0        0        0     9297 2023-06-12 10:00:04.730983 s2stac-0.1.3/src/s2stac/_srtm.py
+-rw-r--r--   0        0        0     1768 2023-06-12 12:20:49.684033 s2stac-0.1.3/src/s2stac/_stacify.py
+-rw-r--r--   0        0        0     5274 1970-01-01 00:00:00.000000 s2stac-0.1.3/setup.py
+-rw-r--r--   0        0        0     5131 1970-01-01 00:00:00.000000 s2stac-0.1.3/PKG-INFO
```

### Comparing `s2stac-0.1.1/LICENSE` & `s2stac-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.1/pyproject.toml` & `s2stac-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "s2stac"
-version = "0.1.1"
+version = "0.1.3"
 description = "Create a STAC from local S2 data."
 authors = ["Pierre Louvart <pierre.louvart@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10.5"
+python = ">=3.10.5,<3.12"
 xarray = "^2023.4.2"
 pystac = "^1.7.3"
 shapely = "1.8.5"
 rasterio = "^1.3.6"
 rioxarray = "^0.14.1"
 numpy = "^1.24.3"
 stackstac = "^0.4.3"
@@ -30,11 +30,14 @@
 geopandas = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 pytest = "^7.3.1"
 black = "^23.3.0"
 ipykernel = "^6.23.0"
+ipympl = "^0.9.3"
+notebook = "^6.5.4"
+jupyter-contrib-nbextensions = "^0.7.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `s2stac-0.1.1/src/s2stac/_asset.py` & `s2stac-0.1.3/src/s2stac/_asset.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.1/src/s2stac/_aux_data.py` & `s2stac-0.1.3/src/s2stac/_aux_data.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.1/src/s2stac/_catalog.py` & `s2stac-0.1.3/src/s2stac/_catalog.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from datetime import datetime, timezone
 from shapely.geometry import Polygon, mapping
 from ._aux_data import add_ecmwf
 
 from ._img_data import add_img_data_bands
 from ._mtd_tl import add_mtd_tl
 from ._qi_data import add_qi_data
+from ._srtm import add_srtm
 
 
 class __TmpFolderPersistence:
     def __init__(self):
         self.tmp_folders = []
 
     def add_tmp_folder(
@@ -40,14 +41,17 @@
     include_img_data: bool = True,
     include_aux_data: bool = True,
     include_qi_data: bool = True,
     include_footprint: bool = True,
     include_cloud_proba: bool = True,
     include_ecmwf: bool = True,
     include_mtd_tl: bool = True,
+    include_srtm: bool = False,
+    usgs_username: str | None = None,
+    usgs_password: str | None = None,
 ) -> pystac.Item:
     target_da_10m = rioxarray.open_rasterio(
         list(safe_folder.glob("GRANULE/*/IMG_DATA/*10*/*B02*"))[0]
     )
     target_da_20m = rioxarray.open_rasterio(
         list(safe_folder.glob("GRANULE/*/IMG_DATA/*20*/*B02*"))[0]
     )
@@ -118,14 +122,31 @@
     if include_mtd_tl:
         bands += add_mtd_tl(
             item=item,
             mtd_tl_path=list(safe_folder.glob("GRANULE/*/MTD_TL.xml"))[0],
             target_da=target_da_10m,
             tmp_folder=catalog_folder,
         )
+    if include_srtm:
+        if usgs_username is None:
+            raise Exception(
+                "No username specified to access srtm data from USGS database"
+            )
+        if usgs_password is None:
+            raise Exception(
+                "No password specified to access srtm data from USGS database"
+            )
+        bands += add_srtm(
+            item=item,
+            srtm_label="srtm",
+            target_da=target_da_10m,
+            tmp_folder=catalog_folder,
+            usgs_username=usgs_username,
+            usgs_password=usgs_password,
+        )
 
     eo_extension.apply(
         bands=bands,
     )
 
     # Add Projection
     projection_extension = ProjectionExtension.ext(item, add_if_missing=True)
@@ -146,14 +167,17 @@
     include_img_data: bool = True,
     include_qi_data: bool = True,
     include_aux_data: bool = True,
     include_footprint: bool = True,
     include_cloud_proba: bool = True,
     include_ecmwf: bool = True,
     include_mtd_tl: bool = True,
+    include_srtm: bool = False,
+    usgs_username: str | None = None,
+    usgs_password: str | None = None,
 ) -> pystac.Catalog:
     if catalog_folder is None:
         catalog_folder = __tmp_folder_persistence.add_tmp_folder()
     elif overwrite_catalog_folder:
         shutil.rmtree(path=str(catalog_folder))
     catalog_folder.mkdir(exist_ok=True, parents=True)
 
@@ -167,14 +191,17 @@
                 include_img_data=include_img_data,
                 include_aux_data=include_aux_data,
                 include_qi_data=include_qi_data,
                 include_footprint=include_footprint,
                 include_cloud_proba=include_cloud_proba,
                 include_ecmwf=include_ecmwf,
                 include_mtd_tl=include_mtd_tl,
+                include_srtm=include_srtm,
+                usgs_username=usgs_username,
+                usgs_password=usgs_password,
             )
         )
 
     catalog.normalize_hrefs(str(catalog_folder))
     catalog.save(catalog_type=pystac.CatalogType.RELATIVE_PUBLISHED)
 
     return catalog
```

### Comparing `s2stac-0.1.1/src/s2stac/_img_data.py` & `s2stac-0.1.3/src/s2stac/_img_data.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.1/src/s2stac/_mtd_tl.py` & `s2stac-0.1.3/src/s2stac/_mtd_tl.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.1/src/s2stac/_preview.py` & `s2stac-0.1.3/src/s2stac/_preview.py`

 * *Files identical despite different names*

### Comparing `s2stac-0.1.1/src/s2stac/_qi_data.py` & `s2stac-0.1.3/src/s2stac/_qi_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             ("10", "MSK_DETFOO_B04", "", target_da_10m),
             ("20", "MSK_DETFOO_B05", "", target_da_20m),
             ("20", "MSK_DETFOO_B06", "", target_da_20m),
             ("20", "MSK_DETFOO_B07", "", target_da_20m),
             ("10", "MSK_DETFOO_B08", "", target_da_10m),
             ("20", "MSK_DETFOO_B8A", "", target_da_20m),
             ("60", "MSK_DETFOO_B09", "", target_da_60m),
-            ("20", "MSK_DETFOO_B10", "", target_da_20m),
+            ("60", "MSK_DETFOO_B10", "", target_da_60m),
             ("20", "MSK_DETFOO_B11", "", target_da_20m),
             ("20", "MSK_DETFOO_B12", "", target_da_20m),
         ]
     ]
 
 
 def add_msk_cldprb(
```

### Comparing `s2stac-0.1.1/src/s2stac/_stacify.py` & `s2stac-0.1.3/src/s2stac/_stacify.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 import pystac
 from pathlib import Path
 import xarray as xr
 import stackstac
 import numpy as np
-
+from typing import Literal
 
 from s2stac._catalog import create_stac_catalog
 
 
 def stacify(
     safe_folders: list[Path],
     catalog_folder: Path | None = None,
     # Include flags
     include_img_data: bool = True,
-    include_qi_data: bool = True,
-    include_aux_data: bool = True,
-    include_footprint: bool = True,
-    include_cloud_proba: bool = True,
-    include_ecmwf: bool = True,
-    include_mtd_tl: bool = True,
+    include_qi_data: bool = False,
+    include_aux_data: bool = False,
+    include_footprint: bool = False,
+    include_cloud_proba: bool = False,
+    include_ecmwf: bool = False,
+    include_mtd_tl: bool = False,
+    include_srtm: bool = False,
+    usgs_password: str | None = None,
+    usgs_username: str | None = None,
     # Stackstac parameters
     epsg: int | None = None,
+    chunksize: int
+    | Literal["auto"]
+    | str
+    | None
+    | tuple[int | Literal["auto"] | str | None, ...]
+    | dict[int, int | Literal["auto"] | str | None] = 1024,
     **kwargs,
 ) -> pystac.Catalog:
     catalog = create_stac_catalog(
         safe_folders=safe_folders,
         catalog_folder=catalog_folder,
         include_img_data=include_img_data,
         include_qi_data=include_qi_data,
         include_aux_data=include_aux_data,
         include_footprint=include_footprint,
         include_cloud_proba=include_cloud_proba,
         include_ecmwf=include_ecmwf,
         include_mtd_tl=include_mtd_tl,
+        include_srtm=include_srtm,
+        usgs_username=usgs_username,
+        usgs_password=usgs_password,
     )
     items = list(catalog.get_all_items())
 
     if len(set(item.properties["proj:epsg"] for item in items)) > 1 and epsg is None:
         epsg = items[0].properties["proj:epsg"]
-    stack = stackstac.stack(items, epsg=epsg, chunksize=(5000, 5000), **kwargs)
+    stack = stackstac.stack(items, epsg=epsg, chunksize=chunksize, **kwargs)
 
     # Turn no data (0) into NaNs
     stack = xr.where(stack, stack, np.nan)
     return stack
```

