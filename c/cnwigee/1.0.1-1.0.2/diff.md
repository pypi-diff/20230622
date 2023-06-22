# Comparing `tmp/cnwigee-1.0.1.tar.gz` & `tmp/cnwigee-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnwigee-1.0.1.tar", last modified: Fri May 26 12:54:58 2023, max compression
+gzip compressed data, was "cnwigee-1.0.2.tar", last modified: Thu Jun 22 14:11:00 2023, max compression
```

## Comparing `cnwigee-1.0.1.tar` & `cnwigee-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.843606 cnwigee-1.0.1/
--rw-rw-rw-   0        0        0     1091 2023-05-04 17:08:09.000000 cnwigee-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2518 2023-05-26 12:54:58.843606 cnwigee-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2023-05-04 17:08:09.000000 cnwigee-1.0.1/README.md
--rw-rw-rw-   0        0        0       82 2023-05-16 18:35:50.000000 cnwigee-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      492 2023-05-26 12:54:58.859584 cnwigee-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-05-16 18:35:50.000000 cnwigee-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.595882 cnwigee-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.783744 cnwigee-1.0.1/src/cnwi/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/__init__.py
--rw-rw-rw-   0        0        0     5574 2023-05-24 16:06:22.000000 cnwigee-1.0.1/src/cnwi/acas.py
--rw-rw-rw-   0        0        0     1837 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/cmap.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.786759 cnwigee-1.0.1/src/cnwi/data/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/data/__init__.py
--rw-rw-rw-   0        0        0     4422 2023-05-24 12:55:30.000000 cnwigee-1.0.1/src/cnwi/datacube.py
--rw-rw-rw-   0        0        0     3464 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/datasets.py
--rw-rw-rw-   0        0        0     7105 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/derivatives.py
--rw-rw-rw-   0        0        0     1843 2023-05-26 12:34:54.000000 cnwigee-1.0.1/src/cnwi/elev.py
--rw-rw-rw-   0        0        0     6246 2023-05-26 11:57:44.000000 cnwigee-1.0.1/src/cnwi/fourier.py
--rw-rw-rw-   0        0        0     3052 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/moa.py
--rw-rw-rw-   0        0        0     4694 2023-05-24 12:55:30.000000 cnwigee-1.0.1/src/cnwi/opt.py
--rw-rw-rw-   0        0        0     2904 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/prebuilt.py
--rw-rw-rw-   0        0        0     1490 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/rf.py
--rw-rw-rw-   0        0        0     1891 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/sar.py
--rw-rw-rw-   0        0        0     3810 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/sfilters.py
--rw-rw-rw-   0        0        0      429 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/stack.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.795915 cnwigee-1.0.1/src/cnwi/tools/
--rw-rw-rw-   0        0        0        0 2023-05-24 16:06:22.000000 cnwigee-1.0.1/src/cnwi/tools/__init__.py
--rw-rw-rw-   0        0        0     1983 2023-05-24 16:06:22.000000 cnwigee-1.0.1/src/cnwi/tools/prep_training_data.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.806931 cnwigee-1.0.1/src/cnwi/tools/to_cloud/
--rw-rw-rw-   0        0        0        0 2023-05-25 17:17:40.000000 cnwigee-1.0.1/src/cnwi/tools/to_cloud/__init__.py
--rw-rw-rw-   0        0        0     5104 2023-05-26 12:53:25.000000 cnwigee-1.0.1/src/cnwi/tools/to_cloud/variables.py
--rw-rw-rw-   0        0        0     3397 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/trainingd.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.843606 cnwigee-1.0.1/src/cnwigee.egg-info/
--rw-rw-rw-   0        0        0     2518 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.843606 cnwigee-1.0.1/tests/
--rw-rw-rw-   0        0        0     2018 2023-05-16 18:35:50.000000 cnwigee-1.0.1/tests/test_eecnwi_helpers.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.977754 cnwigee-1.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-05-04 17:08:09.000000 cnwigee-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2518 2023-06-22 14:11:00.977754 cnwigee-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2191 2023-05-04 17:08:09.000000 cnwigee-1.0.2/README.md
+-rw-rw-rw-   0        0        0       82 2023-05-16 18:35:50.000000 cnwigee-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      492 2023-06-22 14:11:00.979752 cnwigee-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-05-16 18:35:50.000000 cnwigee-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.913868 cnwigee-1.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.949411 cnwigee-1.0.2/src/cnwi/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/__init__.py
+-rw-rw-rw-   0        0        0     5574 2023-05-24 16:06:22.000000 cnwigee-1.0.2/src/cnwi/acas.py
+-rw-rw-rw-   0        0        0     1837 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/cmap.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.950413 cnwigee-1.0.2/src/cnwi/data/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/data/__init__.py
+-rw-rw-rw-   0        0        0     4422 2023-05-24 12:55:30.000000 cnwigee-1.0.2/src/cnwi/datacube.py
+-rw-rw-rw-   0        0        0     3464 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/datasets.py
+-rw-rw-rw-   0        0        0     7105 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/derivatives.py
+-rw-rw-rw-   0        0        0     1843 2023-05-26 12:34:54.000000 cnwigee-1.0.2/src/cnwi/elev.py
+-rw-rw-rw-   0        0        0     6246 2023-05-26 11:57:44.000000 cnwigee-1.0.2/src/cnwi/fourier.py
+-rw-rw-rw-   0        0        0     3052 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/moa.py
+-rw-rw-rw-   0        0        0     4694 2023-05-24 12:55:30.000000 cnwigee-1.0.2/src/cnwi/opt.py
+-rw-rw-rw-   0        0        0     2904 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/prebuilt.py
+-rw-rw-rw-   0        0        0     1490 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/rf.py
+-rw-rw-rw-   0        0        0     1891 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/sar.py
+-rw-rw-rw-   0        0        0     3810 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/sfilters.py
+-rw-rw-rw-   0        0        0      429 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/stack.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.953413 cnwigee-1.0.2/src/cnwi/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 16:06:22.000000 cnwigee-1.0.2/src/cnwi/tools/__init__.py
+-rw-rw-rw-   0        0        0     1983 2023-05-24 16:06:22.000000 cnwigee-1.0.2/src/cnwi/tools/prep_training_data.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.955417 cnwigee-1.0.2/src/cnwi/tools/to_cloud/
+-rw-rw-rw-   0        0        0        0 2023-05-25 17:17:40.000000 cnwigee-1.0.2/src/cnwi/tools/to_cloud/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-06-22 13:51:35.000000 cnwigee-1.0.2/src/cnwi/tools/to_cloud/variables.py
+-rw-rw-rw-   0        0        0     3397 2023-05-23 19:47:33.000000 cnwigee-1.0.2/src/cnwi/trainingd.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.975752 cnwigee-1.0.2/src/cnwigee.egg-info/
+-rw-rw-rw-   0        0        0     2518 2023-06-22 14:11:00.000000 cnwigee-1.0.2/src/cnwigee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-06-22 14:11:00.000000 cnwigee-1.0.2/src/cnwigee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 14:11:00.000000 cnwigee-1.0.2/src/cnwigee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-22 14:11:00.000000 cnwigee-1.0.2/src/cnwigee.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 14:11:00.976757 cnwigee-1.0.2/tests/
+-rw-rw-rw-   0        0        0     2018 2023-05-16 18:35:50.000000 cnwigee-1.0.2/tests/test_eecnwi_helpers.py
```

### Comparing `cnwigee-1.0.1/LICENSE` & `cnwigee-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/PKG-INFO` & `cnwigee-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnwigee
-Version: 1.0.1
+Version: 1.0.2
 Summary: Your description of the project
 Author: Ryan Hamilton
 Author-email: ryangilberthamilton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnwigee-1.0.1/README.md` & `cnwigee-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/acas.py` & `cnwigee-1.0.2/src/cnwi/acas.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/cmap.py` & `cnwigee-1.0.2/src/cnwi/cmap.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/datacube.py` & `cnwigee-1.0.2/src/cnwi/datacube.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/datasets.py` & `cnwigee-1.0.2/src/cnwi/datasets.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/derivatives.py` & `cnwigee-1.0.2/src/cnwi/derivatives.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/elev.py` & `cnwigee-1.0.2/src/cnwi/elev.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/fourier.py` & `cnwigee-1.0.2/src/cnwi/fourier.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/moa.py` & `cnwigee-1.0.2/src/cnwi/moa.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/opt.py` & `cnwigee-1.0.2/src/cnwi/opt.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/prebuilt.py` & `cnwigee-1.0.2/src/cnwi/prebuilt.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/rf.py` & `cnwigee-1.0.2/src/cnwi/rf.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/sar.py` & `cnwigee-1.0.2/src/cnwi/sar.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/sfilters.py` & `cnwigee-1.0.2/src/cnwi/sfilters.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/tools/prep_training_data.py` & `cnwigee-1.0.2/src/cnwi/tools/prep_training_data.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwi/tools/to_cloud/variables.py` & `cnwigee-1.0.2/src/cnwi/tools/to_cloud/variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             omega=1
         ).clip(region)
 
         task = ee.batch.Export.image.toCloudStorage(
             image=ft,
             description="",
             bucket=bucket,
-            fileNamePrefix=file_prefix + f'/{id}/{filename if filename is not None else "fourier-export"}',
+            fileNamePrefix=file_prefix + f'/{filename if filename is not None else "fourier-export"}/{id}/{filename}-{id}-',
             scale=10,
             crs='EPSG:4326',
             region=region,
             maxPixels=1e13,
             shardSize=256,
             fileDimensions=[4096, 4096],
             skipEmptyTiles=True,
@@ -117,15 +117,15 @@
         )
 
         ta_clp = ta.clip(geom)
         task = ee.batch.Export.image.toCloudStorage(
             image=ta_clp,
             description="",
             bucket=bucket,
-            fileNamePrefix=file_prefix + f'/{id}/{filename if filename is not None else "fourier-export"}',
+            fileNamePrefix=file_prefix + f'/{filename if filename is not None else "terrain-export"}/{grid_id}/{filename}-{grid_id}-',
             scale=30,
             fileDimensions=[4096, 4096],
             region=geom,
             crs='EPSG:4326',
             maxPixels=1e13,
             skipEmptyTiles=True,
             formatOptions={
```

### Comparing `cnwigee-1.0.1/src/cnwi/trainingd.py` & `cnwigee-1.0.2/src/cnwi/trainingd.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/src/cnwigee.egg-info/PKG-INFO` & `cnwigee-1.0.2/src/cnwigee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnwigee
-Version: 1.0.1
+Version: 1.0.2
 Summary: Your description of the project
 Author: Ryan Hamilton
 Author-email: ryangilberthamilton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnwigee-1.0.1/src/cnwigee.egg-info/SOURCES.txt` & `cnwigee-1.0.2/src/cnwigee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.1/tests/test_eecnwi_helpers.py` & `cnwigee-1.0.2/tests/test_eecnwi_helpers.py`

 * *Files identical despite different names*

