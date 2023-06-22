# Comparing `tmp/sparrow-cvat-0.4.0.dev1687451336.tar.gz` & `tmp/sparrow-cvat-0.4.0.dev1687457857.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sparrow-cvat-0.4.0.dev1687451336.tar", last modified: Thu Jun 22 16:29:07 2023, max compression
+gzip compressed data, was "sparrow-cvat-0.4.0.dev1687457857.tar", last modified: Thu Jun 22 18:17:48 2023, max compression
```

## Comparing `sparrow-cvat-0.4.0.dev1687451336.tar` & `sparrow-cvat-0.4.0.dev1687457857.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:07.331173 sparrow-cvat-0.4.0.dev1687451336/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 16:29:07.331173 sparrow-cvat-0.4.0.dev1687451336/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 16:29:07.331173 sparrow-cvat-0.4.0.dev1687451336/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:07.327173 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:07.331173 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 16:28:22.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:29:07.331173 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 16:29:07.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-22 16:29:07.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:29:07.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 16:29:07.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 16:29:07.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 16:29:07.000000 sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:17:48.499881 sparrow-cvat-0.4.0.dev1687457857/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 18:17:48.499881 sparrow-cvat-0.4.0.dev1687457857/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 18:17:48.499881 sparrow-cvat-0.4.0.dev1687457857/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:17:48.495881 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:17:48.499881 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8276 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-22 18:17:00.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:17:48.495881 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-22 18:17:48.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-22 18:17:48.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:17:48.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-22 18:17:48.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 18:17:48.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 18:17:48.000000 sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/top_level.txt
```

### Comparing `sparrow-cvat-0.4.0.dev1687451336/LICENSE` & `sparrow-cvat-0.4.0.dev1687457857/LICENSE`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/setup.cfg` & `sparrow-cvat-0.4.0.dev1687457857/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sparrow-cvat
-version = 0.4.0.dev1687451336
+version = 0.4.0.dev1687457857
 author = Sparrow Computing
 author_email = ben@sparrow.dev
 
 [options]
 install_requires = 
 	cvat-sdk<2.4.0
 	fire
```

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/__main__.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/__main__.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/annotations.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/annotations.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/api.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """API class for CVAT."""
 from __future__ import annotations
 
 import os
+import time
 from getpass import getpass
 from typing import Any
 from urllib.parse import parse_qsl, urlencode, urlparse
 
 import requests
 from requests.auth import HTTPBasicAuth
 
@@ -67,14 +68,40 @@
         url = urlparse(route)
         query_params = dict(parse_qsl(url.query))
         query_params.update({"org": get_org()})
         query = urlencode(query_params)
         return f"{url.path}?{query}"
 
     @classmethod
+    def delete(cls, route: str) -> dict[str, Any]:
+        """Make a DELETE request to the CVAT API."""
+        route = cls._org_specific_route(route)
+        response = requests.delete(
+            os.path.join(cls.api_url, route), auth=cls.basic_auth
+        )
+        raise_for_status(response)
+        if response.status_code == 204:
+            return {}
+        return response.json()
+
+    @classmethod
+    def download(cls, route: str) -> bytes:
+        """Download a file from the CVAT API."""
+        route = cls._org_specific_route(route)
+        response = requests.get(os.path.join(cls.api_url, route), auth=cls.basic_auth)
+        raise_for_status(response)
+        while len(response.content) == 0:
+            time.sleep(0.25)
+            response = requests.get(
+                os.path.join(cls.api_url, route), auth=cls.basic_auth
+            )
+            raise_for_status(response)
+        return response.content
+
+    @classmethod
     def get(cls, route: str) -> dict[str, Any]:
         """Make a GET request to the CVAT API."""
         route = cls._org_specific_route(route)
         response = requests.get(os.path.join(cls.api_url, route), auth=cls.basic_auth)
         raise_for_status(response)
         if response.status_code == 204:
             return {}
```

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/auth.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/auth.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/core.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/core.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/create.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/create.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/dataset_manifest/utils.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/dataset_manifest/utils.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/jobs.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/jobs.py`

 * *Files identical despite different names*

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat/tasks.py` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,62 +12,58 @@
 from .api import CVAT
 from .auth import get_client
 from .utils import VALID_IMAGE_FORMATS, VALID_VIDEO_FORMATS
 
 
 def get_frames_info(task_id: int) -> list[dict[str, Any]]:
     """Get information about all frames in a task."""
-    with get_client() as client:
-        task = client.tasks.retrieve(task_id)
-        return task.get_frames_info()
+    task_meta = CVAT.get(f"tasks/{task_id}/data/meta")
+    return task_meta["frames"]
 
 
 def create_task(name: str, project_id: int, segment_size: int = 25) -> dict[str, Any]:
     """Create a new task (without attached images/videos)."""
     payload = {"name": name, "project_id": project_id, "segment_size": segment_size}
     return CVAT.post("tasks", payload)
 
 
 def delete_task(task_id: int) -> None:
     """Delete a task."""
-    with get_client() as client:
-        task = client.tasks.retrieve(task_id)
-        task.remove()
+    return CVAT.delete(f"tasks/{task_id}")
 
 
 def list_tasks(project_id: int) -> list[int]:
     """List all tasks in a project."""
-    with get_client() as client:
-        return client.projects.retrieve(project_id).tasks
+    project = CVAT.get(f"projects/{project_id}")
+    return project["tasks"]
 
 
 def download_annotations(
     task_id: int,
     output_path: Optional[Union[str, Path]] = None,
     media_type: str = "images",
 ) -> None:
     """Download CVAT XML annotations for a task."""
     if output_path is None:
         output_path = f"annotations_{task_id}.xml"
     assert media_type in ("images", "video"), "media_type must be 'images' or 'video'"
-    with get_client() as client, tempfile.TemporaryDirectory() as tmp_dir:
-        tmp_dir = Path(tmp_dir)
-        output_zip = tmp_dir / "download.zip"
-        task = client.tasks.retrieve(task_id)
-        task.export_dataset(
-            f"CVAT for {media_type} 1.1",
-            output_zip,
-            include_images=False,
-            pbar=TqdmProgressReporter(tqdm()),
-        )
-        with zipfile.ZipFile(output_zip, "r") as zip:
-            zip.extract("annotations.xml", tmp_dir)
-        xml_path = tmp_dir / "annotations.xml"
-        with open(xml_path, "r") as f1, open(output_path, "w") as f2:
-            f2.write(f1.read())
+    data_format = f"CVAT for {media_type} 1.1"
+    data = CVAT.download(
+        f"tasks/{task_id}/annotations?format={data_format}&action=download"
+    )
+    with tempfile.TemporaryDirectory() as tmpdir:
+        zip_file = f"{tmpdir}/annotations.zip"
+        with open(zip_file, "wb") as f:
+            f.write(data)
+        with zipfile.ZipFile(zip_file, "r") as f:
+            f.extract("annotations.xml", tmpdir)
+        with open(f"{tmpdir}/annotations.xml", "rb") as f:
+            data = f.read()
+    with open(output_path, "wb") as f:
+        f.write(data)
 
 
 def download_images(
     task_id: int, output_directory: Optional[Union[str, Path]] = None
 ) -> None:
     """Download CVAT images for a task."""
     if output_directory is None:
```

### Comparing `sparrow-cvat-0.4.0.dev1687451336/sparrow_cvat.egg-info/SOURCES.txt` & `sparrow-cvat-0.4.0.dev1687457857/sparrow_cvat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

