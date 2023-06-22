# Comparing `tmp/halc-0.22.3.tar.gz` & `tmp/halc-0.22.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halc-0.22.3.tar", last modified: Sun Jun 18 05:38:33 2023, max compression
+gzip compressed data, was "halc-0.22.4.tar", last modified: Thu Jun 22 05:02:05 2023, max compression
```

## Comparing `halc-0.22.3.tar` & `halc-0.22.4.tar`

### file list

```diff
@@ -1,34 +1,42 @@
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.3/LICENSE
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-18 05:38:33.635181 halc-0.22.3/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.3/README.md
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.631181 halc-0.22.3/halc/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-18 05:38:27.000000 halc-0.22.3/halc/__about__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       95 2023-06-16 02:01:38.000000 halc-0.22.3/halc/__init__.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.631181 halc-0.22.3/halc/images/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       27 2023-06-16 03:45:31.000000 halc-0.22.3/halc/images/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      527 2023-06-18 05:34:51.000000 halc-0.22.3/halc/images/get.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5773 2023-06-18 03:52:20.000000 halc-0.22.3/halc/initialize.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/halc/projects/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      127 2023-06-18 04:01:46.000000 halc-0.22.3/halc/projects/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1388 2023-06-18 05:35:04.000000 halc-0.22.3/halc/projects/create.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      538 2023-06-18 05:11:14.000000 halc-0.22.3/halc/projects/delete.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1015 2023-06-18 04:06:48.000000 halc-0.22.3/halc/projects/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/halc/upload/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      101 2023-06-16 03:33:09.000000 halc-0.22.3/halc/upload/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     4762 2023-06-18 05:36:30.000000 halc-0.22.3/halc/upload/images.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6532 2023-06-18 05:32:04.000000 halc-0.22.3/halc/upload/labels.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      987 2023-06-16 04:34:06.000000 halc-0.22.3/halc/utils.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.635181 halc-0.22.3/halc/versions/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      157 2023-06-18 05:17:09.000000 halc-0.22.3/halc/versions/__init__.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1186 2023-06-18 05:37:02.000000 halc-0.22.3/halc/versions/create.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      707 2023-06-18 05:26:55.000000 halc-0.22.3/halc/versions/delete.py
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1596 2023-06-18 05:37:38.000000 halc-0.22.3/halc/versions/get.py
-drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-18 05:38:33.631181 halc-0.22.3/halc.egg-info/
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/PKG-INFO
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      544 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/SOURCES.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/dependency_links.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       88 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/requires.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-18 05:38:33.000000 halc-0.22.3/halc.egg-info/top_level.txt
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-18 05:38:33.635181 halc-0.22.3/setup.cfg
--rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1383 2023-06-16 03:56:22.000000 halc-0.22.3/setup.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.124743 halc-0.22.4/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1061 2023-06-14 16:42:42.000000 halc-0.22.4/LICENSE
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-22 05:02:05.124743 halc-0.22.4/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      328 2023-06-14 16:36:58.000000 halc-0.22.4/README.md
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.120743 halc-0.22.4/halc/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      227 2023-06-22 05:01:52.000000 halc-0.22.4/halc/__about__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      183 2023-06-22 04:12:24.000000 halc-0.22.4/halc/__init__.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.120743 halc-0.22.4/halc/coco/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       23 2023-06-22 04:12:24.000000 halc-0.22.4/halc/coco/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      343 2023-06-22 04:12:24.000000 halc-0.22.4/halc/coco/parse.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.120743 halc-0.22.4/halc/images/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       42 2023-06-21 23:09:44.000000 halc-0.22.4/halc/images/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1246 2023-06-21 23:19:20.000000 halc-0.22.4/halc/images/get.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     5773 2023-06-21 22:47:19.000000 halc-0.22.4/halc/initialize.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.124743 halc-0.22.4/halc/projects/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      127 2023-06-18 04:01:46.000000 halc-0.22.4/halc/projects/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1388 2023-06-18 05:35:04.000000 halc-0.22.4/halc/projects/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      538 2023-06-18 05:11:14.000000 halc-0.22.4/halc/projects/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1015 2023-06-18 04:06:48.000000 halc-0.22.4/halc/projects/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.124743 halc-0.22.4/halc/storage/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      164 2023-06-18 17:18:21.000000 halc-0.22.4/halc/storage/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     2494 2023-06-18 18:06:19.000000 halc-0.22.4/halc/storage/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      706 2023-06-18 17:21:10.000000 halc-0.22.4/halc/storage/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      617 2023-06-18 17:17:06.000000 halc-0.22.4/halc/storage/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.124743 halc-0.22.4/halc/upload/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      118 2023-06-22 00:14:50.000000 halc-0.22.4/halc/upload/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     6951 2023-06-22 02:52:05.000000 halc-0.22.4/halc/upload/images.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     7000 2023-06-22 04:12:24.000000 halc-0.22.4/halc/upload/labels.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1379 2023-06-22 04:12:24.000000 halc-0.22.4/halc/utils.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.124743 halc-0.22.4/halc/versions/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      157 2023-06-18 05:17:09.000000 halc-0.22.4/halc/versions/__init__.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1186 2023-06-18 05:37:02.000000 halc-0.22.4/halc/versions/create.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      707 2023-06-18 05:26:55.000000 halc-0.22.4/halc/versions/delete.py
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1596 2023-06-18 05:37:38.000000 halc-0.22.4/halc/versions/get.py
+drwxrwxr-x   0 lpaarup   (1001) lpaarup   (1001)        0 2023-06-22 05:02:05.120743 halc-0.22.4/halc.egg-info/
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      858 2023-06-22 05:02:05.000000 halc-0.22.4/halc.egg-info/PKG-INFO
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      676 2023-06-22 05:02:05.000000 halc-0.22.4/halc.egg-info/SOURCES.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        1 2023-06-22 05:02:05.000000 halc-0.22.4/halc.egg-info/dependency_links.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)      121 2023-06-22 05:02:05.000000 halc-0.22.4/halc.egg-info/requires.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)        5 2023-06-22 05:02:05.000000 halc-0.22.4/halc.egg-info/top_level.txt
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)       79 2023-06-22 05:02:05.124743 halc-0.22.4/setup.cfg
+-rw-rw-r--   0 lpaarup   (1001) lpaarup   (1001)     1437 2023-06-22 05:02:03.000000 halc-0.22.4/setup.py
```

### Comparing `halc-0.22.3/LICENSE` & `halc-0.22.4/LICENSE`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/PKG-INFO` & `halc-0.22.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.3
+Version: 0.22.4
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.3/halc/initialize.py` & `halc-0.22.4/halc/initialize.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/halc/projects/create.py` & `halc-0.22.4/halc/projects/create.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/halc/projects/delete.py` & `halc-0.22.4/halc/projects/delete.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/halc/projects/get.py` & `halc-0.22.4/halc/projects/get.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/halc/upload/images.py` & `halc-0.22.4/halc/upload/images.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import magic
 from PIL import Image
 import threading
 import queue
 
 from halc import Client, get_client
 from halc.projects import get_project
+from halc.storage import list_storages, StorageNotFound
 from halc.utils import get_random_color
 
 
 def _upload_image(
     path: str,
     project: dict,
     client: Client,
@@ -54,31 +55,25 @@
         headers={"Content-Type": content_type, "Content-Length": str(len(data))},
     )
     res.raise_for_status()
 
     return image
 
 
-def upload_images(
-    paths: List[str],
-    project_id: str,
-    tags: List[str] = [],
+def _parse_tags(
+    project: dict,
+    tags: list[str],
+    client: Client,
 ) -> dict:
-    """Upload a list of local images to the app
-    :param paths: list of paths to images
-    :param project_id: Id of the project
-    :param tags: list of tags to apply to the uploaded images
-    :return: status of the operation
+    """Parse tags for project
+    :param project: project spec
+    :param tags: tags to set
+    :param client: client to use
+    :return: attributes
     """
-
-    # Get project from backend
-    client = get_client()
-    project = get_project(project_id)
-
-    # If tags provided, merge them with existing tags and update the project
     tag_ids = []
     project_tags = project["attributes"][0]
     if len(tags) > 0:
         # Map tags to project tags
         project_options = project_tags["options"]
         project_option_names = [opt["name"] for opt in project_options]
         for tag in tags:
@@ -98,14 +93,35 @@
 
         # Save options to backend
         client.post(
             f"/attributes/options/{project['id']}/{project_tags['id']}",
             project_options,
         )
     attributes = {project_tags["id"]: tag_ids}
+    return attributes
+
+
+def upload_images(
+    paths: List[str],
+    project_id: str,
+    tags: List[str] = [],
+) -> dict:
+    """Upload a list of local images to the app
+    :param paths: list of paths to images
+    :param project_id: Id of the project
+    :param tags: list of tags to apply to the uploaded images
+    :return: status of the operation
+    """
+
+    # Get project from backend
+    client = get_client()
+    project = get_project(project_id)
+
+    # If tags provided, merge them with existing tags and update the project
+    attributes = _parse_tags(project, tags, client)
 
     # Upload images params
     session_id = str(uuid4())
     total = len(paths)
 
     # Create queues and progress bar
     read = queue.Queue()
@@ -170,7 +186,67 @@
         if ext.lower() not in valid_images:
             continue
         files.append(os.path.join(base_dir, f))
     print(f"Found {len(files)} images in {base_dir}")
 
     # Upload them to the app
     return upload_images(files, project_id, tags)
+
+
+class ImageRegistrationFailed(Exception):
+    pass
+
+
+def register_images(
+    image_names: list[str],
+    project_id: str,
+    storage_id: str,
+    tags: List[str] = [],
+    create_thumbnail: bool = False,
+) -> dict:
+    """Register images to existing storage
+    :param image_names: list of image names to register
+    :param project_id: Id of the project
+    :param storage_id: Id of the storage
+    :param tags: list of tags to apply to the registered images
+    :param create_thumbnail: Whether to create a thumbnail for every image
+    :return: status of the operation
+    """
+
+    # Check if storage id in project
+    if storage_id not in [storage["id"] for storage in list_storages(project_id)]:
+        raise StorageNotFound(f"storage with id '{storage_id}' not found")
+
+    # Get project from backend
+    client = get_client()
+    project = get_project(project_id)
+
+    # If tags provided, merge them with existing tags and update the project
+    attributes = _parse_tags(project, tags, client)
+
+    # Create image specs
+    images = [
+        {
+            "name": name,
+            "project_id": project_id,
+            "storage_id": storage_id,
+            "id": str(uuid4()),
+            "has_thumbnail": create_thumbnail,
+            "attributes": attributes,
+        }
+        for name in image_names
+    ]
+
+    # Register
+    try:
+        print(
+            f"Registering images. Check the status of the upload at https://app.happyrobot.ai/{project['organization_id']}/{project['id']}"
+        )
+        client.post(
+            f"/images/{project_id}",
+            images,
+            {"session_id": str(uuid4()), "total": len(images)},
+        )
+    except Exception:
+        raise ImageRegistrationFailed(
+            f"could not register images to storage with id '{storage_id}'"
+        )
```

### Comparing `halc-0.22.3/halc/upload/labels.py` & `halc-0.22.4/halc/upload/labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from uuid import uuid4
 from pathlib import Path
 import math
 
 from halc import get_client
-from halc.utils import get_random_color, clip_bbox, compressed_rle_to_list
+from halc.utils import get_random_color, clip_bbox, compressed_rle_to_list, polygons_to_rle
 from halc.projects import get_project
 from halc.images import get_images
 
 
 class PathNotFound(Exception):
     pass
 
@@ -65,15 +65,15 @@
 
     # Parse classes in project
     classes = {
         tokenize(cls["name"]): {"is_new": False, "count": 0, **cls}
         for cls in project["classes"]
     }
 
-    # Parse categories in datasource
+    # Parse categories in data source
     categories = ds.get("categories")
     if categories is None:
         raise CategoriesNotFound()
 
     # Map datasource category id to project class
     category_id_to_class = {}
     for category in categories:
@@ -154,16 +154,22 @@
             "color": get_random_color(),
         }
 
         # Process segmentation, if any
         if "segmentation" in ann:
             seg = ann["segmentation"]
             if isinstance(seg, list) and len(seg) > 0:
-                # TODO: Convert polygons to rle
-                continue
+                # Polygon is a list of lists
+                if len(seg[0]) < 2:
+                    # Discard polygons with less than 2 elements
+                    continue
+                rle = polygons_to_rle(polygons=seg, height=image["height"], width=image["width"])
+                assert not isinstance(rle["counts"], list), "RLE is a list of ints, should have been compressed string"
+                rle = compressed_rle_to_list(rle["counts"])
+                annotation["segmentation"] = {"rle": rle}            
             elif "counts" in seg:
                 if isinstance(seg["counts"], list):
                     # RLE is a list of ints
                     if len(seg["counts"]) < 2:
                         # Discard RLEs with less than 2 elements
                         continue
                     rle = seg["counts"]
```

### Comparing `halc-0.22.3/halc/utils.py` & `halc-0.22.4/halc/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import random
 from typing import List
+import numpy as np
+from pycocotools import mask as coco_mask_utils
 
 
 def get_random_color() -> str:
     r = lambda: random.randint(0, 255)
     return "#%02X%02X%02X" % (r(), r(), r())
 
 
@@ -32,7 +34,16 @@
                 x |= -1 << (5 * k)
 
         if len(listCounts) > 2:
             x += listCounts[len(listCounts) - 2]
         listCounts.append(x)
 
     return listCounts
+
+
+def polygons_to_rle(polygons: np.ndarray, height: int, width: int) -> dict:
+    if len(polygons) == 0:
+        # COCOAPI does not support empty polygons
+        return np.zeros((height, width)).astype(bool)
+    rles = coco_mask_utils.frPyObjects(polygons, height, width)
+    rle = coco_mask_utils.merge(rles)
+    return rle
```

### Comparing `halc-0.22.3/halc/versions/create.py` & `halc-0.22.4/halc/versions/create.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/halc/versions/delete.py` & `halc-0.22.4/halc/versions/delete.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/halc/versions/get.py` & `halc-0.22.4/halc/versions/get.py`

 * *Files identical despite different names*

### Comparing `halc-0.22.3/halc.egg-info/PKG-INFO` & `halc-0.22.4/halc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halc
-Version: 0.22.3
+Version: 0.22.4
 Summary: Python SDK for Happyrobot's HALC
 Home-page: https://happyrobot.ai
 Author: Happyrobot
 Author-email: luis.paarup@happyrobot.ai
 License: MIT
 Keywords: happyrobot computer vision artificial intelligence foundation models large vision
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `halc-0.22.3/setup.py` & `halc-0.22.4/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     install_requires=[
         "pyyaml==6.0",
         "requests==2.22.0",
         "tqdm==4.65.0",
         "pillow==9.5.0",
         "python-magic==0.4.27",
         "uuid==1.30",
+        "numpy==1.23.5",
+        "pycocotools==2.0.6"
     ],
     packages=find_packages(),
     python_requires=">=3.5",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

