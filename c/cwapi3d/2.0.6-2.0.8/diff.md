# Comparing `tmp/cwapi3d-2.0.6.tar.gz` & `tmp/cwapi3d-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwapi3d-2.0.6.tar", last modified: Thu Jun  1 15:30:51 2023, max compression
+gzip compressed data, was "cwapi3d-2.0.8.tar", last modified: Mon Jun  5 14:57:11 2023, max compression
```

## Comparing `cwapi3d-2.0.6.tar` & `cwapi3d-2.0.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/attribute_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/attribute_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/bim_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/bim_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/cadwork/
--rw-r--r--   0 runner    (1001) docker     (123)    89894 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/cadwork/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.127132 cwapi3d-2.0.6/src/connector_axis_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/connector_axis_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/cwapi3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 15:30:51.000000 cwapi3d-2.0.6/src/cwapi3d.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/element_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    34859 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/element_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/endtype_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/endtype_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/file_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/file_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/geometry_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/geometry_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/list_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/list_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/machine_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/machine_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/material_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/material_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/menu_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/menu_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/roof_controller/
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/roof_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/scene_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/scene_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/shop_drawing_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/shop_drawing_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/utility_controller/
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/utility_controller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:30:51.131132 cwapi3d-2.0.6/src/visualization_controller/
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-01 15:30:40.000000 cwapi3d-2.0.6/src/visualization_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.291438 cwapi3d-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.291438 cwapi3d-2.0.8/src/attribute_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    23815 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/attribute_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.291438 cwapi3d-2.0.8/src/bim_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/bim_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.291438 cwapi3d-2.0.8/src/cadwork/
+-rw-r--r--   0 runner    (1001) docker     (123)    90064 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/cadwork/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.291438 cwapi3d-2.0.8/src/connector_axis_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/connector_axis_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.291438 cwapi3d-2.0.8/src/cwapi3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-05 14:57:11.000000 cwapi3d-2.0.8/src/cwapi3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-05 14:57:11.000000 cwapi3d-2.0.8/src/cwapi3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:57:11.000000 cwapi3d-2.0.8/src/cwapi3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-05 14:57:11.000000 cwapi3d-2.0.8/src/cwapi3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.291438 cwapi3d-2.0.8/src/element_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    34859 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/element_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/endtype_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/endtype_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/file_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/file_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/geometry_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/geometry_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/list_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/list_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/machine_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/machine_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/material_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/material_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/menu_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/menu_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/roof_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/roof_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/scene_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/scene_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/shop_drawing_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/shop_drawing_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/utility_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/utility_controller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:57:11.295438 cwapi3d-2.0.8/src/visualization_controller/
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-06-05 14:56:59.000000 cwapi3d-2.0.8/src/visualization_controller/__init__.pyi
```

### Comparing `cwapi3d-2.0.6/LICENSE` & `cwapi3d-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/PKG-INFO` & `cwapi3d-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 2.0.6
+Version: 2.0.8
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-2.0.6/README.md` & `cwapi3d-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/setup.py` & `cwapi3d-2.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='cwapi3d',
-    version='2.0.6',
+    version='2.0.8',
     author='Cadwork',
     author_email='it@cadwork.ca',
     description='Python bindings for CwAPI3D',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/cwapi3d/cwapi3dpython',
     classifiers=[
```

### Comparing `cwapi3d-2.0.6/src/attribute_controller/__init__.pyi` & `cwapi3d-2.0.8/src/attribute_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/bim_controller/__init__.pyi` & `cwapi3d-2.0.8/src/bim_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/cadwork/__init__.pyi` & `cwapi3d-2.0.8/src/cadwork/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 from platform import node
 from typing import List
-from enum import Enum, unique
+from enum import IntEnum, unique
 
 
 class layer_settings():
     def __init__(self) -> None:
         pass
 
 
@@ -2352,115 +2352,114 @@
     def set_none(self, element_ids: List[int], ifc_type) -> None:
         """_summary_
 
         Args:
             element_ids (List[int]): _description_
             ifc_type (_type_): _description_
         """
-# Node Symbols
 
 
 @unique
-class node_symbol(Enum):
+class node_symbol(IntEnum):
     """Change node symbol. 
 
     Examples:
         >>> point = cadwork.point_3d(0, 0, 0)
         >>> node = element_controller.create_node(point)
         >>> node.set_node_symbol(node, node_symbol.circle)
 
     Args:
-        small_circle (int): 1
-        square (int): 2
-        cross (int): 3
-        circle (int): 4
-        filled_circle (int): 5
-        chess_square (int): 6
-        half_filled_square (int): 7
-        cross_square (int): 8
-        filled_square (int): 9       
+        SmallCircle (int): 1
+        Square (int): 2
+        Cross (int): 3
+        Circle (int): 4
+        FilledCircle (int): 5
+        ChessSquare (int): 6
+        HalfFilledSquare (int): 7
+        CrossSquare (int): 8
+        FilledSquare (int): 9  
     """
-    small_circle = 1
-    square = 2
-    cross = 3
-    circle = 4
-    filled_circle = 5
-    chess_square = 6
-    half_filled_square = 7
-    cross_square = 8
-    filled_square = 9
+    SmallSquare = 1
+    Square = 2
+    Cross = 3
+    Circle = 4
+    FilledCircle = 5
+    ChessSquare = 6
+    HalfFilledSquare = 7
+    CrossSquare = 8
+    FilledSquare = 9
 
     def __int__(self) -> None:
         return self.value
 
 
 @unique
-class element_module_detail(Enum):
+class element_module_detail(IntEnum):
     """Add element situation to detail. 
 
     Examples:
         >>> element_controller.add_elements_to_detail(element_ids, element_module_detail.cross)
 
     Args:
-        none (int): 0
-        angle (int): 1
-        area (int): 2
-        cross (int): 3
-        edge (int): 4
-        end (int): 5
-        line (int): 6
-        open (int): 7
-        t_connection (int): 8
-        floor_area (int): 9
-        floor_end (int): 10
-        floor_line (int): 11
-        floor_open (int): 12
+        no_detail (int): 0
+        angle_detail (int): 1
+        area_detail (int): 2
+        cross_detail (int): 3
+        edge_detail (int): 4
+        end_detail (int): 5
+        line_detail (int): 6
+        open_detail (int): 7
+        t_detail (int): 8
+        floor_area_detail (int): 9
+        floor_end_detail (int): 10
+        floor_line_detail (int): 11
+        floor_open_detail (int): 12
 
     """
-    none_ = 0,
-    angle = 1,
-    area = 2,
-    cross = 3,
-    edge = 4,
-    end = 5,
-    line = 6,
-    open = 7,
-    t_connection = 8,
-    floor_area = 9,
-    floor_end = 10,
-    floor_line = 11,
-    floor_open = 12
+    no_detail = 0,
+    angle_detail = 1,
+    area_detail = 2,
+    cross_detail = 3,
+    edge_detail = 4,
+    end_detail = 5,
+    line_detail = 6,
+    open_detail = 7,
+    t_detail = 8,
+    floor_area_detail = 9,
+    floor_end_detail = 10,
+    floor_line_detail = 11,
+    floor_open_detail = 12
 
     def __int__(self) -> None:
         return self.value
 
 
 @unique
-class division_zone_direction(Enum):
+class division_zone_direction(IntEnum):
     """ Add division zone direction.
 
     Examples:
         >>> point = cadwork.point_3d(0, 0, 0)
         >>> geometry_controller.create_division_zone(123456, point, division_zone_direction.positive)
 
     Args:
         positive (int): 1
         negative (int): -1
         none (int): 0
     """
     positive = 1
     negative = -1
-    none = 0
+    no_direction = 0
 
     def __int__(self) -> None:
         return self.value
 
 
 @unique
-class shortcut_key(Enum):
+class shortcut_key(IntEnum):
     """Shortcut key.
 
     Examples:
         >>> utility_controller.execute_shortcut(shortcut_key.F1, shortcut_key_modifier.shift)
 
     Args:
         F1 (int): 1
@@ -2490,37 +2489,37 @@
     F12 = 12
 
     def __int__(self) -> None:
         return self.value
 
 
 @unique
-class shortcut_key_modifier(Enum):
+class shortcut_key_modifier(IntEnum):
     """Shortcut key.
 
     Examples:
         >>> utility_controller.execute_shortcut(shortcut_key.F1, shortcut_key_modifier.shift)
 
     Args:
-        none (int): 0
+        no_modifier (int): 0
         shift (int): 1
         ctrl (int): 2
         alt (int): 3
     """
-    none = 0
+    no_modifier = 0
     shift = 1
     ctrl = 2
     alt = 3
 
     def __int__(self) -> None:
         return self.value
 
 
 @unique
-class btl_version(Enum):
+class btl_version(IntEnum):
     """BTL version.
 
     Examples:
         >>> machine_controller.export_btl(btl_version.btl_1_6, "C:\\temp\\test.btl")
 
     Args:
         btl_1_0 (int): 110
@@ -2541,15 +2540,15 @@
     btl_1_6 = 116
 
     def __int__(self) -> None:
         return self.value
 
 
 @unique
-class hundegger_machine_type(Enum):
+class hundegger_machine_type(IntEnum):
     """Hundegger machine type.
 
     Examples:
         >>> machine_controller.export_hundegger(hundegger_machine_type.k2)
 
     Args:
         p8_10 (int): 1
@@ -2585,15 +2584,15 @@
     turbo_drive = 15
 
     def __int__(self) -> None:
         return self.value
 
 
 @unique
-class weinmann_mfb_version(Enum):
+class weinmann_mfb_version(IntEnum):
     """Weinmann MFB version.
 
     Examples:
         >>> machine_controller.export_weinmann_mfb(weinmann_mfb_version.wup_2_0)
 
     Args:
         wup_2_0 (int): 20
```

### Comparing `cwapi3d-2.0.6/src/connector_axis_controller/__init__.pyi` & `cwapi3d-2.0.8/src/connector_axis_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/cwapi3d.egg-info/PKG-INFO` & `cwapi3d-2.0.8/src/cwapi3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cwapi3d
-Version: 2.0.6
+Version: 2.0.8
 Summary: Python bindings for CwAPI3D
 Home-page: https://github.com/cwapi3d/cwapi3dpython
 Author: Cadwork
 Author-email: it@cadwork.ca
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `cwapi3d-2.0.6/src/cwapi3d.egg-info/SOURCES.txt` & `cwapi3d-2.0.8/src/cwapi3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/element_controller/__init__.pyi` & `cwapi3d-2.0.8/src/element_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/endtype_controller/__init__.pyi` & `cwapi3d-2.0.8/src/endtype_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/file_controller/__init__.pyi` & `cwapi3d-2.0.8/src/file_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/geometry_controller/__init__.pyi` & `cwapi3d-2.0.8/src/geometry_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/list_controller/__init__.pyi` & `cwapi3d-2.0.8/src/list_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/machine_controller/__init__.pyi` & `cwapi3d-2.0.8/src/machine_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/material_controller/__init__.pyi` & `cwapi3d-2.0.8/src/material_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/scene_controller/__init__.pyi` & `cwapi3d-2.0.8/src/scene_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/shop_drawing_controller/__init__.pyi` & `cwapi3d-2.0.8/src/shop_drawing_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/utility_controller/__init__.pyi` & `cwapi3d-2.0.8/src/utility_controller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `cwapi3d-2.0.6/src/visualization_controller/__init__.pyi` & `cwapi3d-2.0.8/src/visualization_controller/__init__.pyi`

 * *Files identical despite different names*

