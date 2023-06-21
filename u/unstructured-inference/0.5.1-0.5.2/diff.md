# Comparing `tmp/unstructured_inference-0.5.1.tar.gz` & `tmp/unstructured_inference-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.5.1.tar", last modified: Tue May 30 21:18:31 2023, max compression
+gzip compressed data, was "unstructured_inference-0.5.2.tar", last modified: Wed Jun 21 22:26:05 2023, max compression
```

## Comparing `unstructured_inference-0.5.1.tar` & `unstructured_inference-0.5.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.426563 unstructured_inference-0.5.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.430563 unstructured_inference-0.5.1/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.430563 unstructured_inference-0.5.1/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/inference/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/detectron2onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/models/yolox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.434563 unstructured_inference-0.5.1/unstructured_inference/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/patches/pdfminer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-30 21:16:30.000000 unstructured_inference-0.5.1/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:18:31.430563 unstructured_inference-0.5.1/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-30 21:18:31.000000 unstructured_inference-0.5.1/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.416619 unstructured_inference-0.5.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.416619 unstructured_inference-0.5.2/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.420619 unstructured_inference-0.5.2/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14401 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12571 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/inference/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/detectron2onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24059 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23929 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.428619 unstructured_inference-0.5.2/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-06-21 22:23:34.000000 unstructured_inference-0.5.2/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:26:05.420619 unstructured_inference-0.5.2/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-21 22:26:05.000000 unstructured_inference-0.5.2/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.5.1/PKG-INFO` & `unstructured_inference-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.5.1
+Version: 0.5.2
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.1/README.md` & `unstructured_inference-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.1/setup.py` & `unstructured_inference-0.5.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,37 +13,48 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-from setuptools import setup, find_packages
-from typing import List
+from typing import List, Optional, Union
+
+from setuptools import find_packages, setup
 
 from unstructured_inference.__version__ import __version__
 
 
-def load_requirements(file_list=None):
+def load_requirements(file_list: Optional[Union[str, List[str]]] = None):
+    """Loads the requirements from a .in file or list of .in files."""
     if file_list is None:
         file_list = ["requirements/base.in"]
     if isinstance(file_list, str):
         file_list = [file_list]
     requirements: List[str] = []
     for file in file_list:
         with open(file, encoding="utf-8") as f:
             requirements.extend(f.readlines())
-    requirements = [req for req in requirements if not req.startswith("#")]
+    requirements = [
+        req for req in requirements if not req.startswith("#") and not req.startswith("-")
+    ]
     return requirements
 
 
+def load_text_from_file(filename: str):
+    """Retrieves text from a file."""
+    with open(filename, encoding="utf-8") as fp:
+        description = fp.read()
+    return description
+
+
 setup(
     name="unstructured_inference",
     description="A library for performing inference using trained models.",
-    long_description=open("README.md", "r", encoding="utf-8").read(),
+    long_description=load_text_from_file("README.md"),
     long_description_content_type="text/markdown",
     keywords="NLP PDF HTML CV XML parsing preprocessing",
     url="https://github.com/Unstructured-IO/unstructured-inference",
     python_requires=">=3.7.0",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
@@ -74,10 +85,10 @@
             # If you cannot immediately regenerate your protos, some other possible workarounds are:
             #  1. Downgrade the protobuf package to 3.20.x or lower.
             #  2. Set PROTOCOL_BUFFERS_PYTHON_IMPLEMENTATION=python (but this will use pure-Python
             #     parsing and will be much slower).
             'protobuf<3.21 ; platform_machine=="x86_64"',
             # NOTE(alan): Pin to get around error: undefined symbol: _dl_sym, version GLIBC_PRIVATE
             'paddlepaddle>=2.4 ; platform_machine=="x86_64"',
-        ]
+        ],
     },
 )
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/inference/elements.py` & `unstructured_inference-0.5.2/unstructured_inference/inference/elements.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
-from copy import deepcopy
-from dataclasses import dataclass
+
 import re
-from typing import Optional, Union, Sequence, List
 import unicodedata
+from copy import deepcopy
+from dataclasses import dataclass
+from typing import Collection, List, Optional, Union
 
 import numpy as np
 from PIL import Image
 from scipy.sparse.csgraph import connected_components
 
 from unstructured_inference.logger import logger
 from unstructured_inference.models import tesseract
@@ -76,52 +77,84 @@
 
     def intersects(self, other: Rectangle) -> bool:
         """Checks whether this rectangle intersects another rectangle."""
         return intersections(self, other)[0, 1]
 
     def is_in(self, other: Rectangle, error_margin: Optional[Union[int, float]] = None) -> bool:
         """Checks whether this rectangle is contained within another rectangle."""
-        if error_margin is not None:
-            padded_other = other.pad(error_margin)
-        else:
-            padded_other = other
+        padded_other = other.pad(error_margin) if error_margin is not None else other
         return all(
             [
                 (self.x1 >= padded_other.x1),
                 (self.x2 <= padded_other.x2),
                 (self.y1 >= padded_other.y1),
                 (self.y2 <= padded_other.y2),
-            ]
+            ],
         )
 
     @property
     def coordinates(self):
         """Gets coordinates of the rectangle"""
         return ((self.x1, self.y1), (self.x1, self.y2), (self.x2, self.y2), (self.x2, self.y1))
 
+    def intersection(self, other: Rectangle) -> Optional[Rectangle]:
+        """Gives the rectangle that is the intersection of two rectangles, or None if the
+        rectangles are disjoint."""
+        x1 = max(self.x1, other.x1)
+        x2 = min(self.x2, other.x2)
+        y1 = max(self.y1, other.y1)
+        y2 = min(self.y2, other.y2)
+        if x1 > x2 or y1 > y2:
+            return None
+        return Rectangle(x1, y1, x2, y2)
+
+    def area(self) -> float:
+        """Gives the area of the rectangle."""
+        return self.width * self.height
+
+    def intersection_over_union(self, other: Rectangle) -> float:
+        """Gives the intersection-over-union of two rectangles. This tends to be a good metric of
+        how similar the regions are. Returns 0 for disjoint rectangles, 1 for two identical
+        rectangles -- area of intersection / area of union."""
+        intersection = self.intersection(other)
+        intersection_area = 0.0 if intersection is None else intersection.area()
+        union_area = self.area() + other.area() - intersection_area
+        return intersection_area / union_area
+
+    def intersection_over_minimum(self, other: Rectangle) -> float:
+        """Gives the area-of-intersection over the minimum of the areas of the rectangles. Useful
+        for identifying when one rectangle is almost-a-subset of the other. Returns 0 for disjoint
+        rectangles, 1 when either is a subset of the other."""
+        intersection = self.intersection(other)
+        intersection_area = 0.0 if intersection is None else intersection.area()
+        min_area = min(self.area(), other.area())
+        return intersection_area / min_area
+
+    def is_almost_subregion_of(self, other: Rectangle, subregion_threshold: float = 0.75) -> bool:
+        """Returns whether this region is almost a subregion of other. This is determined by
+        comparing the intersection area over self area to some threshold, and checking whether self
+        is the smaller rectangle."""
+        intersection = self.intersection(other)
+        intersection_area = 0.0 if intersection is None else intersection.area()
+        return (subregion_threshold < intersection_area / self.area()) and (
+            self.area() <= other.area()
+        )
+
 
 def minimal_containing_region(*regions: Rectangle) -> Rectangle:
     """Returns the smallest rectangular region that contains all regions passed"""
     x1 = min(region.x1 for region in regions)
     y1 = min(region.y1 for region in regions)
     x2 = max(region.x2 for region in regions)
     y2 = max(region.y2 for region in regions)
 
-    # Return most specialized class of which that every region is a subclass
-    def least_common_superclass(*instances):
-        mros = (type(ins).mro() for ins in instances)
-        mro = next(mros)
-        common = set(mro).intersection(*mros)
-        return next((x for x in mro if x in common), Rectangle)
+    return Rectangle(x1, y1, x2, y2)
 
-    cls = least_common_superclass(*regions)
-    return cls(x1, y1, x2, y2)
 
-
-def partition_groups_from_regions(regions: Sequence[Rectangle]) -> List[List[Rectangle]]:
+def partition_groups_from_regions(regions: Collection[Rectangle]) -> List[List[Rectangle]]:
     """Partitions regions into groups of regions based on proximity. Returns list of lists of
     regions, each list corresponding with a group"""
     padded_regions = [
         r.vpad(r.height * V_PADDING_COEF).hpad(r.height * H_PADDING_COEF) for r in regions
     ]
 
     intersection_mtx = intersections(*padded_regions)
@@ -134,14 +167,15 @@
     return groups
 
 
 def intersections(*rects: Rectangle):
     """Returns a square boolean matrix of intersections of an arbitrary number of rectangles, i.e.
     the ijth entry of the matrix is True if and only if the ith Rectangle and jth Rectangle
     intersect."""
+    # NOTE(alan): Rewrite using line scan
     coords = np.stack([[[r.x1, r.y1], [r.x2, r.y2]] for r in rects], axis=-1)
 
     (x1s, y1s), (x2s, y2s) = coords
 
     # Use broadcasting to get comparison matrices.
     # For Rectangles r1 and r2, any of the following conditions makes the rectangles disjoint:
     # r1.x1 > r2.x2
@@ -164,44 +198,41 @@
     text: Optional[str] = None
 
     def __str__(self) -> str:
         return str(self.text)
 
     def extract_text(
         self,
-        objects: Optional[List[TextRegion]],
+        objects: Optional[Collection[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
     ) -> str:
         """Extracts text contained in region."""
         if self.text is not None:
             # If block text is already populated, we'll assume it's correct
             text = self.text
         elif objects is not None:
             text = aggregate_by_block(self, image, objects, ocr_strategy)
         elif image is not None:
-            if ocr_strategy != "never":
-                # We don't have anything to go on but the image itself, so we use OCR
-                text = ocr(self, image, languages=ocr_languages)
-            else:
-                text = ""
+            # We don't have anything to go on but the image itself, so we use OCR
+            text = ocr(self, image, languages=ocr_languages) if ocr_strategy != "never" else ""
         else:
             raise ValueError(
                 "Got arguments image and layout as None, at least one must be populated to use for "
-                "text extraction."
+                "text extraction.",
             )
         return text
 
 
 class EmbeddedTextRegion(TextRegion):
     def extract_text(
         self,
-        objects: Optional[List[TextRegion]],
+        objects: Optional[Collection[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
     ) -> str:
         """Extracts text contained in region."""
         if self.text is None:
@@ -209,15 +240,15 @@
         else:
             return self.text
 
 
 class ImageTextRegion(TextRegion):
     def extract_text(
         self,
-        objects: Optional[List[TextRegion]],
+        objects: Optional[Collection[TextRegion]],
         image: Optional[Image.Image] = None,
         extract_tables: bool = False,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
     ) -> str:
         """Extracts text contained in region."""
         if self.text is None:
@@ -239,15 +270,15 @@
     if agent is None:
         raise RuntimeError("OCR agent is not loaded for {languages}.")
     return agent.detect(cropped_image)
 
 
 def needs_ocr(
     region: TextRegion,
-    pdf_objects: List[TextRegion],
+    pdf_objects: Collection[TextRegion],
     ocr_strategy: str,
 ) -> bool:
     """Logic to determine whether ocr is needed to extract text from given region."""
     if ocr_strategy == "force":
         return True
     elif ocr_strategy == "auto":
         image_objects = [obj for obj in pdf_objects if isinstance(obj, ImageTextRegion)]
@@ -260,28 +291,26 @@
             # If the region has no text check if any images overlap with the region that might
             # contain text.
             if any(obj.is_in(region) and obj.text is not None for obj in word_objects):
                 # If there are word objects in the region, we defer to that rather than OCR
                 return False
             else:
                 return image_intersects
-        elif cid_ratio(region.text) > 0.5:
+        else:
             # If the region has text, we should only have to OCR if too much of the text is
             # uninterpretable.
-            return True
-        else:
-            return False
+            return cid_ratio(region.text) > 0.5
     else:
         return False
 
 
 def aggregate_by_block(
     text_region: TextRegion,
     image: Optional[Image.Image],
-    pdf_objects: List[TextRegion],
+    pdf_objects: Collection[TextRegion],
     ocr_strategy: str = "auto",
     ocr_languages: str = "eng",
 ) -> str:
     """Extracts the text aggregated from the elements of the given layout that lie within the given
     block."""
     if image is not None and needs_ocr(text_region, pdf_objects, ocr_strategy):
         text = ocr(text_region, image, languages=ocr_languages)
@@ -312,7 +341,31 @@
     return text.find("(cid:") != -1
 
 
 def remove_control_characters(text: str) -> str:
     """Removes control characters from text."""
     out_text = "".join(c for c in text if unicodedata.category(c)[0] != "C")
     return out_text
+
+
+def region_bounding_boxes_are_almost_the_same(
+    region1: Rectangle,
+    region2: Rectangle,
+    same_region_threshold: float = 0.75,
+) -> bool:
+    """Returns whether bounding boxes are almost the same. This is determined by checking if the
+    intersection over union is above some threshold."""
+    return region1.intersection_over_union(region2) > same_region_threshold
+
+
+def grow_region_to_match_region(region_to_grow: Rectangle, region_to_match: Rectangle):
+    """Grows a region to the minimum size necessary to contain both regions."""
+    (new_x1, new_y1), _, (new_x2, new_y2), _ = minimal_containing_region(
+        region_to_grow,
+        region_to_match,
+    ).coordinates
+    region_to_grow.x1, region_to_grow.y1, region_to_grow.x2, region_to_grow.y2 = (
+        new_x1,
+        new_y1,
+        new_x2,
+        new_y2,
+    )
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/inference/layout.py` & `unstructured_inference-0.5.2/unstructured_inference/inference/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 from __future__ import annotations
+
 import os
 import tempfile
-from typing import List, Optional, Tuple, Union, BinaryIO
+from typing import BinaryIO, List, Optional, Tuple, Union
 
 import numpy as np
 import pdf2image
 from pdfminer import psparser
+from pdfminer.high_level import extract_pages
 from PIL import Image
 
 from unstructured_inference.inference.elements import (
-    TextRegion,
     EmbeddedTextRegion,
     ImageTextRegion,
+    TextRegion,
+)
+from unstructured_inference.inference.layoutelement import (
+    LayoutElement,
+    merge_inferred_layout_with_extracted_layout,
 )
-from unstructured_inference.inference.layoutelement import LayoutElement
 from unstructured_inference.inference.ordering import order_layout
 from unstructured_inference.logger import logger
 from unstructured_inference.models.base import get_model
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.patches.pdfminer import parse_keyword
 from unstructured_inference.visualize import draw_bbox
 
@@ -68,17 +73,17 @@
         extract_tables: bool = False,
     ) -> DocumentLayout:
         """Creates a DocumentLayout from a pdf file."""
         logger.info(f"Reading PDF for file: {filename} ...")
         layouts, images = load_pdf(filename)
         if len(layouts) > len(images):
             raise RuntimeError(
-                "Some images were not loaded. Check that poppler is installed and in your $PATH."
+                "Some images were not loaded. Check that poppler is installed and in your $PATH.",
             )
-        pages: List[PageLayout] = list()
+        pages: List[PageLayout] = []
         if fixed_layouts is None:
             fixed_layouts = [None for _ in layouts]
         for i, (image, layout, fixed_layout) in enumerate(zip(images, layouts, fixed_layouts)):
             # NOTE(robinson) - In the future, maybe we detect the page number and default
             # to the index if it is not detected
             page = PageLayout.from_image(
                 image,
@@ -141,15 +146,15 @@
         extract_tables: bool = False,
     ):
         self.image = image
         self.image_array: Union[np.ndarray, None] = None
         self.layout = layout
         self.number = number
         self.model = model
-        self.elements: List[LayoutElement] = list()
+        self.elements: List[LayoutElement] = []
         if ocr_strategy not in VALID_OCR_STRATEGIES:
             raise ValueError(f"ocr_strategy must be one of {VALID_OCR_STRATEGIES}.")
         self.ocr_strategy = ocr_strategy
         self.ocr_languages = ocr_languages
         self.extract_tables = extract_tables
 
     def __str__(self) -> str:
@@ -160,14 +165,19 @@
         logger.info("Detecting page elements ...")
         if self.model is None:
             self.model = get_model()
 
         # NOTE(mrobinson) - We'll want make this model inference step some kind of
         # remote call in the future.
         inferred_layout = self.model(self.image)
+        if self.layout is not None:
+            inferred_layout = merge_inferred_layout_with_extracted_layout(
+                inferred_layout=inferred_layout,
+                extracted_layout=self.layout,
+            )
         elements = self.get_elements_from_layout(inferred_layout)
         if inplace:
             self.elements = elements
             return None
         return elements
 
     def get_elements_from_layout(self, layout: List[TextRegion]) -> List[LayoutElement]:
@@ -207,16 +217,16 @@
         for el, color in zip(self.elements, colors):
             img = draw_bbox(img, el, color=color)
         return img
 
     @classmethod
     def from_image(
         cls,
-        image,
-        number=1,
+        image: Image.Image,
+        number: int = 1,
         model: Optional[UnstructuredModel] = None,
         layout: Optional[List[TextRegion]] = None,
         ocr_strategy: str = "auto",
         ocr_languages: str = "eng",
         extract_tables: bool = False,
         fixed_layout: Optional[List[TextRegion]] = None,
     ):
@@ -302,73 +312,47 @@
     pdf_objects: Optional[List[TextRegion]] = None,
     ocr_strategy: str = "auto",
     ocr_languages: str = "eng",
     extract_tables: bool = False,
 ) -> LayoutElement:
     """Creates a LayoutElement from a given layout or image by finding all the text that lies within
     a given block."""
-    if isinstance(block, LayoutElement):
-        element = block
-    else:
-        element = LayoutElement.from_region(block)
+    element = block if isinstance(block, LayoutElement) else LayoutElement.from_region(block)
     element.text = element.extract_text(
         objects=pdf_objects,
         image=image,
         extract_tables=extract_tables,
         ocr_strategy=ocr_strategy,
         ocr_languages=ocr_languages,
     )
     return element
 
 
 def load_pdf(
     filename: str,
-    x_tolerance: Union[int, float] = 1.5,
-    y_tolerance: Union[int, float] = 2,
-    keep_blank_chars: bool = False,
-    use_text_flow: bool = False,
-    horizontal_ltr: bool = True,  # Should words be read left-to-right?
-    vertical_ttb: bool = True,  # Should vertical words be read top-to-bottom?
-    extra_attrs: Optional[List[str]] = None,
-    split_at_punctuation: Union[bool, str] = False,
     dpi: int = 200,
 ) -> Tuple[List[List[TextRegion]], List[Image.Image]]:
     """Loads the image and word objects from a pdf using pdfplumber and the image renderings of the
     pdf pages using pdf2image"""
-    pdf_object = pdfplumber.open(filename)
     layouts = []
-    images = []
-    for page in pdf_object.pages:
-        plumber_words = page.extract_words(
-            x_tolerance=x_tolerance,
-            y_tolerance=y_tolerance,
-            keep_blank_chars=keep_blank_chars,
-            use_text_flow=use_text_flow,
-            horizontal_ltr=horizontal_ltr,
-            vertical_ttb=vertical_ttb,
-            extra_attrs=extra_attrs,
-            split_at_punctuation=split_at_punctuation,
-        )
-        word_objs: List[TextRegion] = [
-            EmbeddedTextRegion(
-                x1=word["x0"] * dpi / 72,
-                y1=word["top"] * dpi / 72,
-                x2=word["x1"] * dpi / 72,
-                y2=word["bottom"] * dpi / 72,
-                text=word["text"],
-            )
-            for word in plumber_words
-        ]
-        image_objs: List[TextRegion] = [
-            ImageTextRegion(
-                x1=image["x0"] * dpi / 72,
-                y1=image["top"] * dpi / 72,
-                x2=image["x1"] * dpi / 72,
-                y2=image["bottom"] * dpi / 72,
+    for page in extract_pages(filename):
+        layout = []
+        height = page.height
+        for element in page:
+            x1, y2, x2, y1 = element.bbox
+            y1 = height - y1
+            y2 = height - y2
+            # Coefficient to rescale bounding box to be compatible with images
+            coef = dpi / 72
+            _text, element_class = (
+                (element.get_text(), EmbeddedTextRegion)
+                if hasattr(element, "get_text")
+                else (None, ImageTextRegion)
             )
-            for image in page.images
-        ]
-        layout = word_objs + image_objs
+            text_region = element_class(x1 * coef, y1 * coef, x2 * coef, y2 * coef, text=_text)
+
+            if text_region.area() > 0:
+                layout.append(text_region)
         layouts.append(layout)
 
     images = pdf2image.convert_from_path(filename, dpi=dpi)
     return layouts, images
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/inference/ordering.py` & `unstructured_inference-0.5.2/unstructured_inference/inference/ordering.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/base.py` & `unstructured_inference-0.5.2/unstructured_inference/models/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from typing import Optional
-from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 
 from unstructured_inference.models.detectron2 import (
     MODEL_TYPES as DETECTRON2_MODEL_TYPES,
+)
+from unstructured_inference.models.detectron2 import (
     UnstructuredDetectronModel,
 )
 from unstructured_inference.models.detectron2onnx import (
     MODEL_TYPES as DETECTRON2_ONNX_MODEL_TYPES,
+)
+from unstructured_inference.models.detectron2onnx import (
     UnstructuredDetectronONNXModel,
 )
+from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 from unstructured_inference.models.yolox import (
     MODEL_TYPES as YOLOX_MODEL_TYPES,
+)
+from unstructured_inference.models.yolox import (
     UnstructuredYoloXModel,
 )
 
 DEFAULT_MODEL = "detectron2_onnx"
 
 
 def get_model(model_name: Optional[str] = None) -> UnstructuredModel:
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.5.2/unstructured_inference/models/detectron2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from typing import Final, Optional, Union, List, Dict, Any
 from pathlib import Path
+from typing import Any, Dict, Final, List, Optional, Union
 
+from huggingface_hub import hf_hub_download
 from layoutparser.models.detectron2.layoutmodel import (
-    is_detectron2_available,
     Detectron2LayoutModel,
+    is_detectron2_available,
 )
 from layoutparser.models.model_config import LayoutModelConfig
 from PIL import Image
-from huggingface_hub import hf_hub_download
 
-from unstructured_inference.logger import logger
 from unstructured_inference.inference.layoutelement import LayoutElement
-from unstructured_inference.models.unstructuredmodel import UnstructuredObjectDetectionModel
+from unstructured_inference.logger import logger
+from unstructured_inference.models.unstructuredmodel import (
+    UnstructuredObjectDetectionModel,
+)
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
 
-
 DETECTRON_CONFIG: Final = "lp://PubLayNet/faster_rcnn_R_50_FPN_3x/config"
 DEFAULT_LABEL_MAP: Final[Dict[int, str]] = {
     0: "Text",
     1: "Title",
     2: "List",
     3: "Table",
     4: "Figure",
@@ -41,18 +42,22 @@
             "PubLayNet/faster_rcnn_R_50_FPN_3x/config.yml",
         ),
         label_map=DEFAULT_LABEL_MAP,
         extra_config=DEFAULT_EXTRA_CONFIG,
     ),
     "checkbox": LazyDict(
         model_path=LazyEvaluateInfo(
-            hf_hub_download, "unstructuredio/oer-checkbox", "detectron2_finetuned_oer_checkbox.pth"
+            hf_hub_download,
+            "unstructuredio/oer-checkbox",
+            "detectron2_finetuned_oer_checkbox.pth",
         ),
         config_path=LazyEvaluateInfo(
-            hf_hub_download, "unstructuredio/oer-checkbox", "detectron2_oer_checkbox.json"
+            hf_hub_download,
+            "unstructuredio/oer-checkbox",
+            "detectron2_oer_checkbox.json",
         ),
         label_map={0: "Unchecked", 1: "Checked"},
         extra_config=None,
     ),
 }
 
 
@@ -74,15 +79,15 @@
         device: Optional[str] = None,
     ):
         """Loads the detectron2 model using the specified parameters"""
 
         if not is_detectron2_available():
             raise ImportError(
                 "Failed to load the Detectron2 model. Ensure that the Detectron2 "
-                "module is correctly installed."
+                "module is correctly installed.",
             )
 
         config_path_str = str(config_path)
         model_path_str: Optional[str] = None if model_path is None else str(model_path)
         logger.info("Loading the Detectron2 layout model ...")
         self.model = Detectron2LayoutModel(
             config_path_str,
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/detectron2onnx.py` & `unstructured_inference-0.5.2/unstructured_inference/models/detectron2onnx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from typing import Final, Optional, Union, Dict, List
 from pathlib import Path
+from typing import Dict, Final, List, Optional, Union
 
-from PIL import Image
+import cv2
+import numpy as np
+import onnxruntime
 from huggingface_hub import hf_hub_download
+from PIL import Image
 
-from unstructured_inference.logger import logger
 from unstructured_inference.inference.layoutelement import LayoutElement
-from unstructured_inference.models.unstructuredmodel import UnstructuredObjectDetectionModel
+from unstructured_inference.logger import logger
+from unstructured_inference.models.unstructuredmodel import (
+    UnstructuredObjectDetectionModel,
+)
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
-import onnxruntime
-import numpy as np
-import cv2
-
 
 DEFAULT_LABEL_MAP: Final[Dict[int, str]] = {
     0: "Text",
     1: "Title",
     2: "List",
     3: "Table",
     4: "Figure",
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/donut.py` & `unstructured_inference-0.5.2/unstructured_inference/models/donut.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,20 @@
-import torch
 import logging
+from pathlib import Path
+from typing import Optional, Union
 
-from unstructured_inference.models.unstructuredmodel import UnstructuredModel
-from transformers import DonutProcessor, VisionEncoderDecoderModel, VisionEncoderDecoderConfig
+import torch
 from PIL import Image
-from typing import Union, Optional
-from pathlib import Path
+from transformers import (
+    DonutProcessor,
+    VisionEncoderDecoderConfig,
+    VisionEncoderDecoderModel,
+)
+
+from unstructured_inference.models.unstructuredmodel import UnstructuredModel
 
 
 class UnstructuredDonutModel(UnstructuredModel):
     """Unstructured model wrapper for Donut image transformer."""
 
     def predict(self, x: Image):
         """Make prediction using donut model"""
@@ -36,24 +41,26 @@
             logging.info("Loading the Donut model and processor...")
             self.processor = DonutProcessor.from_pretrained(processor)
             self.model = VisionEncoderDecoderModel.from_pretrained(model, config=config)
 
         except EnvironmentError:
             logging.critical("Failed to initialize the model.")
             logging.critical(
-                "Ensure that the Donut parameters config, model and processor are correct"
+                "Ensure that the Donut parameters config, model and processor are correct",
             )
             raise ImportError("Review the parameters to initialize a UnstructuredDonutModel obj")
         self.model.to(device)
 
     def run_prediction(self, x: Image):
         """Internal prediction method."""
         pixel_values = self.processor(x, return_tensors="pt").pixel_values
         decoder_input_ids = self.processor.tokenizer(
-            self.task_prompt, add_special_tokens=False, return_tensors="pt"
+            self.task_prompt,
+            add_special_tokens=False,
+            return_tensors="pt",
         ).input_ids
         outputs = self.model.generate(
             pixel_values.to(self.device),
             decoder_input_ids=decoder_input_ids.to(self.device),
             max_length=self.model.decoder.config.max_position_embeddings,
             early_stopping=True,
             pad_token_id=self.processor.tokenizer.pad_token_id,
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.5.2/unstructured_inference/models/table_postprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,18 @@
     """
 
     if len(tokens) > 0:
         columns = nms_by_containment(columns, tokens, overlap_threshold=0.5)
         remove_objects_without_content(tokens, columns)
     else:
         columns = nms(
-            columns, match_criteria="object2_overlap", match_threshold=0.25, keep_higher=True
+            columns,
+            match_criteria="object2_overlap",
+            match_threshold=0.25,
+            keep_higher=True,
         )
     if len(columns) > 1:
         columns = sort_objects_left_to_right(columns)
 
     return columns
 
 
@@ -188,15 +191,15 @@
         package_area = package_rect.get_area()
         for container_num, container in enumerate(container_objects):
             container_rect = Rect(container["bbox"])
             intersect_area = container_rect.intersect(Rect(package["bbox"])).get_area()
             overlap_fraction = intersect_area / package_area
 
             match_scores.append(
-                {"container": container, "container_num": container_num, "score": overlap_fraction}
+                {"container": container, "container_num": container_num, "score": overlap_fraction},
             )
 
         sorted_match_scores = sort_objects_by_score(match_scores)
 
         best_match_score = sorted_match_scores[0]
         best_match_scores.append(best_match_score["score"])
         if forced_assignment or best_match_score["score"] >= overlap_threshold:
@@ -285,26 +288,23 @@
     spans_copy.sort(key=lambda span: span["block_num"])
 
     # Force the span at the end of every line within a block to have exactly one space
     # unless the line ends with a space or ends with a non-space followed by a hyphen
     line_texts = []
     line_span_texts = [spans_copy[0]["text"]]
     for span1, span2 in zip(spans_copy[:-1], spans_copy[1:]):
-        if (
-            not span1["block_num"] == span2["block_num"]
-            or not span1["line_num"] == span2["line_num"]
-        ):
+        if span1["block_num"] != span2["block_num"] or span1["line_num"] != span2["line_num"]:
             line_text = join_char.join(line_span_texts).strip()
             if (
                 len(line_text) > 0
-                and not line_text[-1] == " "
-                and not (len(line_text) > 1 and line_text[-1] == "-" and not line_text[-2] == " ")
+                and line_text[-1] != " "
+                and not (len(line_text) > 1 and line_text[-1] == "-" and line_text[-2] != " ")
+                and not join_with_space
             ):
-                if not join_with_space:
-                    line_text += " "
+                line_text += " "
             line_texts.append(line_text)
             line_span_texts = [span2["text"]]
         else:
             line_span_texts.append(span2["text"])
     line_text = join_char.join(line_span_texts)
     line_texts.append(line_text)
 
@@ -331,15 +331,15 @@
     table bounding box.
     """
     try:
         for column in columns:
             column["bbox"][1] = bbox[1]
             column["bbox"][3] = bbox[3]
     except Exception as err:
-        print("Could not align columns: {}".format(err))
+        print(f"Could not align columns: {err}")
         pass
 
     return columns
 
 
 def align_rows(rows, bbox):
     """
@@ -347,15 +347,15 @@
     table bounding box.
     """
     try:
         for row in rows:
             row["bbox"][0] = bbox[0]
             row["bbox"][2] = bbox[2]
     except Exception as err:
-        print("Could not align rows: {}".format(err))
+        print(f"Could not align rows: {err}")
         pass
 
     return rows
 
 
 def nms(objects, match_criteria="object2_overlap", match_threshold=0.05, keep_higher=True):
     """
@@ -420,15 +420,16 @@
             row_height = row["bbox"][3] - row["bbox"][1]
             supercell_height = supercell["bbox"][3] - supercell["bbox"][1]
             min_row_overlap = max(row["bbox"][1], supercell["bbox"][1])
             max_row_overlap = min(row["bbox"][3], supercell["bbox"][3])
             overlap_height = max_row_overlap - min_row_overlap
             if "span" in supercell:
                 overlap_fraction = max(
-                    overlap_height / row_height, overlap_height / supercell_height
+                    overlap_height / row_height,
+                    overlap_height / supercell_height,
                 )
             else:
                 overlap_fraction = overlap_height / row_height
             if overlap_fraction >= 0.5:
                 if "header" in row and row["header"]:
                     intersecting_header_rows.add(row_num)
                 else:
@@ -555,22 +556,21 @@
     header_supercells = sort_objects_by_score(header_supercells)
 
     for header_supercell in header_supercells[:]:
         ancestors_by_row = defaultdict(int)
         min_row = min(header_supercell["row_numbers"])
         for header_supercell2 in header_supercells:
             max_row2 = max(header_supercell2["row_numbers"])
-            if max_row2 < min_row:
-                if set(header_supercell["column_numbers"]).issubset(
-                    set(header_supercell2["column_numbers"])
-                ):
-                    for row2 in header_supercell2["row_numbers"]:
-                        ancestors_by_row[row2] += 1
+            if max_row2 < min_row and set(header_supercell["column_numbers"]).issubset(
+                set(header_supercell2["column_numbers"]),
+            ):
+                for row2 in header_supercell2["row_numbers"]:
+                    ancestors_by_row[row2] += 1
         for row in range(0, min_row):
-            if not ancestors_by_row[row] == 1:
+            if ancestors_by_row[row] != 1:
                 supercells.remove(header_supercell)
                 break
 
 
 def remove_supercell_overlap(supercell1, supercell2):
     """
     This function resolves overlap between supercells (supercells must be
@@ -583,15 +583,15 @@
     versus the number of rows in column C. If the number of columns in row R
     is less than the number of rows in column C, we eliminate row R from
     supercell #1. This resolves the overlap by removing fewer grid cells from
     supercell #1 than if we eliminated column C from it.
     """
     common_rows = set(supercell1["row_numbers"]).intersection(set(supercell2["row_numbers"]))
     common_columns = set(supercell1["column_numbers"]).intersection(
-        set(supercell2["column_numbers"])
+        set(supercell2["column_numbers"]),
     )
 
     # While the supercells have overlapping grid cells, continue shrinking the less-confident
     # supercell one row or one column at a time
     while len(common_rows) > 0 and len(common_columns) > 0:
         # Try to shrink the supercell as little as possible to remove the overlap;
         # if the supercell has fewer rows than columns, remove an overlapping column,
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/tables.py` & `unstructured_inference-0.5.2/unstructured_inference/models/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 # https://github.com/microsoft/table-transformer/blob/main/src/inference.py
 # https://github.com/NielsRogge/Transformers-Tutorials/blob/master/Table%20Transformer/Using_Table_Transformer_for_table_detection_and_table_structure_recognition.ipynb
-import torch
 import logging
-
-from unstructured_inference.models.unstructuredmodel import UnstructuredModel
-from unstructured_inference.logger import logger
-
-from collections import defaultdict
+import platform
 import xml.etree.ElementTree as ET
+from collections import defaultdict
+from pathlib import Path
+from typing import Optional, Union
 
 import cv2
 import numpy as np
 import pandas as pd
-
 import pytesseract
-
-from transformers import TableTransformerForObjectDetection
-from transformers import DetrImageProcessor
+import torch
 from PIL import Image
-from typing import Union, Optional
-from pathlib import Path
-import platform
+from transformers import DetrImageProcessor, TableTransformerForObjectDetection
 
-from . import table_postprocess as postprocess
+from unstructured_inference.logger import logger
 from unstructured_inference.models.table_postprocess import Rect
+from unstructured_inference.models.unstructuredmodel import UnstructuredModel
+
+from . import table_postprocess as postprocess
 
 
 class UnstructuredTableTransformerModel(UnstructuredModel):
     """Unstructured model wrapper for table-transformer."""
 
     def __init__(self):
         pass
@@ -51,15 +47,15 @@
             self.model = TableTransformerForObjectDetection.from_pretrained(model)
             self.model.eval()
 
         except EnvironmentError:
             logging.critical("Failed to initialize the model.")
             logging.critical("Ensure that the model is correct")
             raise ImportError(
-                "Review the parameters to initialize a UnstructuredTableTransformerModel obj"
+                "Review the parameters to initialize a UnstructuredTableTransformerModel obj",
             )
         self.model.to(device)
 
     def run_prediction(self, x: Image):
         """Predict table structure"""
         with torch.no_grad():
             encoding = self.feature_extractor(x, return_tensors="pt").to(self.device)
@@ -90,15 +86,16 @@
             )
 
             kernel = np.ones((1, 1), np.uint8)
             img = cv2.dilate(img, kernel, iterations=1)
             img = cv2.erode(img, kernel, iterations=1)
 
             ocr_df: pd.DataFrame = pytesseract.image_to_data(
-                Image.fromarray(img), output_type="data.frame"
+                Image.fromarray(img),
+                output_type="data.frame",
             )
 
             ocr_df = ocr_df.dropna()
 
             tokens = []
             for idtx in ocr_df.itertuples():
                 tokens.append(
@@ -106,15 +103,15 @@
                         "bbox": [
                             idtx.left / zoom,
                             idtx.top / zoom,
                             (idtx.left + idtx.width) / zoom,
                             (idtx.top + idtx.height) / zoom,
                         ],
                         "text": idtx.text,
-                    }
+                    },
                 )
 
         sorted(tokens, key=lambda x: x["bbox"][1] * 10000 + x["bbox"][0])
 
         # 'tokens' is a list of tokens
         # Need to be in a relative reading order
         # If no order is provided, use current order
@@ -204,21 +201,21 @@
     pred_scores = list(m.values.detach().cpu().numpy())[0]
     pred_bboxes = outputs["pred_boxes"].detach().cpu()[0]
     pred_bboxes = [elem.tolist() for elem in rescale_bboxes(pred_bboxes, img_size)]
 
     objects = []
     for label, score, bbox in zip(pred_labels, pred_scores, pred_bboxes):
         class_label = class_idx2name[int(label)]
-        if not class_label == "no object":
+        if class_label != "no object":
             objects.append(
                 {
                     "label": class_label,
                     "score": float(score),
                     "bbox": [float(elem) for elem in bbox],
-                }
+                },
             )
 
     return objects
 
 
 # for output bounding box post-processing
 def box_cxcywh_to_xyxy(x):
@@ -284,15 +281,17 @@
             for header_obj in column_headers:
                 if iob(obj["bbox"], header_obj["bbox"]) >= 0.5:
                     obj["column header"] = True
 
         # Refine table structures
         rows = postprocess.refine_rows(rows, table_tokens, class_thresholds["table row"])
         columns = postprocess.refine_columns(
-            columns, table_tokens, class_thresholds["table column"]
+            columns,
+            table_tokens,
+            class_thresholds["table column"],
         )
 
         # Shrink table bbox to just the total height of the rows
         # and the total width of the columns
         row_rect = Rect()
         for obj in rows:
             row_rect.include_rect(obj["bbox"])
@@ -331,31 +330,34 @@
     """
     rows = table_structure["rows"]
     columns = table_structure["columns"]
 
     # Process the headers
     column_headers = table_structure["column headers"]
     column_headers = postprocess.apply_threshold(
-        column_headers, class_thresholds["table column header"]
+        column_headers,
+        class_thresholds["table column header"],
     )
     column_headers = postprocess.nms(column_headers)
     column_headers = align_headers(column_headers, rows)
 
     # Process spanning cells
     spanning_cells = [
         elem for elem in table_structure["spanning cells"] if not elem["projected row header"]
     ]
     projected_row_headers = [
         elem for elem in table_structure["spanning cells"] if elem["projected row header"]
     ]
     spanning_cells = postprocess.apply_threshold(
-        spanning_cells, class_thresholds["table spanning cell"]
+        spanning_cells,
+        class_thresholds["table spanning cell"],
     )
     projected_row_headers = postprocess.apply_threshold(
-        projected_row_headers, class_thresholds["table projected row header"]
+        projected_row_headers,
+        class_thresholds["table projected row header"],
     )
     spanning_cells += projected_row_headers
     # Align before NMS for spanning cells because alignment brings them into agreement
     # with rows and columns first; if spanning cells still overlap after this operation,
     # the threshold for NMS can basically be lowered to just above 0
     spanning_cells = postprocess.align_supercells(spanning_cells, rows, columns)
     spanning_cells = postprocess.nms_supercells(spanning_cells)
@@ -517,23 +519,27 @@
         row_rect = Rect()
         for row_num in cell["row_nums"]:
             row_rect.include_rect(list(dilated_rows[row_num]["bbox"]))
         cell_rect = column_rect.intersect(row_rect)
         cell["bbox"] = cell_rect.get_bbox()
 
     span_nums_by_cell, _, _ = postprocess.slot_into_containers(
-        cells, tokens, overlap_threshold=0.001, forced_assignment=False
+        cells,
+        tokens,
+        overlap_threshold=0.001,
+        forced_assignment=False,
     )
 
     for cell, cell_span_nums in zip(cells, span_nums_by_cell):
         cell_spans = [tokens[num] for num in cell_span_nums]
         # TODO: Refine how text is extracted; should be character-based, not span-based;
         # but need to associate
         cell["cell text"] = postprocess.extract_text_from_spans(
-            cell_spans, remove_integer_superscripts=False
+            cell_spans,
+            remove_integer_superscripts=False,
         )
         cell["spans"] = cell_spans
 
     # Adjust the row, column, and cell bounding boxes to reflect the extracted text
     num_rows = len(rows)
     rows = postprocess.sort_objects_top_to_bottom(rows)
     num_columns = len(columns)
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.5.2/unstructured_inference/models/tesseract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from layoutparser.ocr.tesseract_agent import is_pytesseract_available, TesseractAgent
+from layoutparser.ocr.tesseract_agent import TesseractAgent, is_pytesseract_available
 
 from unstructured_inference.logger import logger
 
 ocr_agents: Dict[str, TesseractAgent] = {}
 
 
 def load_agent(languages: str = "eng"):
@@ -17,13 +17,13 @@
         to isntall the appropriate Tesseract language pack.
     """
     global ocr_agents
 
     if not is_pytesseract_available():
         raise ImportError(
             "Failed to load Tesseract. Ensure that Tesseract is installed. Example command: \n"
-            "    >>> sudo apt install -y tesseract-ocr"
+            "    >>> sudo apt install -y tesseract-ocr",
         )
 
     if languages not in ocr_agents:
         logger.info(f"Loading the Tesseract OCR agent for {languages} ...")
         ocr_agents[languages] = TesseractAgent(languages=languages)
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.5.2/unstructured_inference/models/unstructuredmodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from typing import TYPE_CHECKING, Any, List
 
 from PIL.Image import Image
 
 if TYPE_CHECKING:
     from unstructured_inference.inference.layoutelement import LayoutElement
@@ -20,15 +21,15 @@
 
     @abstractmethod
     def predict(self, x: Any) -> Any:
         """Do inference using the wrapped model."""
         if self.model is None:
             raise ModelNotInitializedError(
                 "Model has not been initialized. Please call the initialize method with the "
-                "appropriate arguments for loading the model."
+                "appropriate arguments for loading the model.",
             )
         pass  # pragma: no cover
 
     def __call__(self, x: Any) -> Any:
         """Inference using function call interface."""
         return self.predict(x)
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/models/yolox.py` & `unstructured_inference-0.5.2/unstructured_inference/models/yolox.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # Copyright (c) Megvii, Inc. and its affiliates.
 # Unstructured modified the original source code found at:
 # https://github.com/Megvii-BaseDetection/YOLOX/blob/237e943ac64aa32eb32f875faa93ebb18512d41d/yolox/data/data_augment.py
 # https://github.com/Megvii-BaseDetection/YOLOX/blob/ac379df3c97d1835ebd319afad0c031c36d03f36/yolox/utils/demo_utils.py
 
-from PIL import Image
+from typing import List
+
 import cv2
-from huggingface_hub import hf_hub_download
 import numpy as np
 import onnxruntime
-from typing import List
+from huggingface_hub import hf_hub_download
+from PIL import Image
 
 from unstructured_inference.inference.layoutelement import LayoutElement
 from unstructured_inference.models.unstructuredmodel import UnstructuredModel
-from unstructured_inference.visualize import draw_yolox_bounding_boxes
 from unstructured_inference.utils import LazyDict, LazyEvaluateInfo
+from unstructured_inference.visualize import draw_yolox_bounding_boxes
 
 YOLOX_LABEL_MAP = {
     0: "Caption",
     1: "Footnote",
     2: "Formula",
     3: "List-item",
     4: "Page-footer",
@@ -28,21 +29,25 @@
     9: "Text",
     10: "Title",
 }
 
 MODEL_TYPES = {
     "yolox": LazyDict(
         model_path=LazyEvaluateInfo(
-            hf_hub_download, "unstructuredio/yolo_x_layout", "yolox_l0.05.onnx"
+            hf_hub_download,
+            "unstructuredio/yolo_x_layout",
+            "yolox_l0.05.onnx",
         ),
         label_map=YOLOX_LABEL_MAP,
     ),
     "yolox_tiny": LazyDict(
         model_path=LazyEvaluateInfo(
-            hf_hub_download, "unstructuredio/yolo_x_layout", "yolox_tiny.onnx"
+            hf_hub_download,
+            "unstructuredio/yolo_x_layout",
+            "yolox_tiny.onnx",
         ),
         label_map=YOLOX_LABEL_MAP,
     ),
 }
 
 
 class UnstructuredYoloXModel(UnstructuredModel):
@@ -153,18 +158,15 @@
 
 
 def demo_postprocess(outputs, img_size, p6=False):
     """Postprocessing for YoloX model."""
     grids = []
     expanded_strides = []
 
-    if not p6:
-        strides = [8, 16, 32]
-    else:
-        strides = [8, 16, 32, 64]
+    strides = [8, 16, 32] if not p6 else [8, 16, 32, 64]
 
     hsizes = [img_size[0] // stride for stride in strides]
     wsizes = [img_size[1] // stride for stride in strides]
 
     for hsize, wsize, stride in zip(hsizes, wsizes, strides):
         xv, yv = np.meshgrid(np.arange(wsize), np.arange(hsize))
         grid = np.stack((xv, yv), 2).reshape(1, -1, 2)
@@ -197,15 +199,16 @@
 
     valid_score_mask = cls_scores > score_thr
     valid_scores = cls_scores[valid_score_mask]
     valid_boxes = boxes[valid_score_mask]
     valid_cls_inds = cls_inds[valid_score_mask]
     keep = nms(valid_boxes, valid_scores, nms_thr)
     dets = np.concatenate(
-        [valid_boxes[keep], valid_scores[keep, None], valid_cls_inds[keep, None]], 1
+        [valid_boxes[keep], valid_scores[keep, None], valid_cls_inds[keep, None]],
+        1,
     )
     return dets
 
 
 def nms(boxes, scores, nms_thr):
     """Single class NMS implemented in Numpy."""
     x1 = boxes[:, 0]
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/patches/pdfminer.py` & `unstructured_inference-0.5.2/unstructured_inference/patches/pdfminer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Union
 
-from pdfminer.psparser import END_KEYWORD, PSKeyword, KWD, PSBaseParser
+from pdfminer.psparser import END_KEYWORD, KWD, PSBaseParser, PSKeyword
 
 
 def parse_keyword(self: PSBaseParser, s: bytes, i: int) -> int:
     """Patch for pdfminer method _parse_keyword of PSBaseParser. Changes are identical to the PR
     https://github.com/pdfminer/pdfminer.six/pull/885."""
     m = END_KEYWORD.search(s, i)
     if not m:
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/utils.py` & `unstructured_inference-0.5.2/unstructured_inference/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from collections.abc import Mapping
-from typing import Any, Hashable, Union, Iterator, Callable
+from typing import Any, Callable, Hashable, Iterator, Union
 
 
 class LazyEvaluateInfo:
     """Class that stores the information needed to lazily evaluate a function with given arguments.
     The object stores the information needed for evaluation as a function and its arguments.
     """
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference/visualize.py` & `unstructured_inference-0.5.2/unstructured_inference/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,19 @@
         font = cv2.FONT_HERSHEY_SIMPLEX
 
         txt_size = cv2.getTextSize(text, font, 0.4, 1)[0]
         cv2.rectangle(img, (x0, y0), (x1, y1), color, 2)
 
         txt_bk_color = (_COLORS[cls_id] * 255 * 0.7).astype(np.uint8).tolist()
         cv2.rectangle(
-            img, (x0, y0 + 1), (x0 + txt_size[0] + 1, y0 + int(1.5 * txt_size[1])), txt_bk_color, -1
+            img,
+            (x0, y0 + 1),
+            (x0 + txt_size[0] + 1, y0 + int(1.5 * txt_size[1])),
+            txt_bk_color,
+            -1,
         )
         cv2.putText(img, text, (x0, y0 + txt_size[1]), font, 0.4, txt_color, thickness=1)
 
     return img
 
 
 _COLORS = np.array(
@@ -138,9 +142,9 @@
         [0.429, 0.429, 0.429],
         [0.571, 0.571, 0.571],
         [0.714, 0.714, 0.714],
         [0.857, 0.857, 0.857],
         [0.000, 0.447, 0.741],
         [0.314, 0.717, 0.741],
         [0.50, 0.5, 0],
-    ]
+    ],
 ).astype(np.float32)
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.5.2/unstructured_inference.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.5.1
+Version: 0.5.2
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.5.1/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.5.2/unstructured_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

