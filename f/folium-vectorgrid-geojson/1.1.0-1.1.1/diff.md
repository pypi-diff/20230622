# Comparing `tmp/folium_vectorgrid_geojson-1.1.0.tar.gz` & `tmp/folium_vectorgrid_geojson-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folium_vectorgrid_geojson-1.1.0.tar", max compression
+gzip compressed data, was "folium_vectorgrid_geojson-1.1.1.tar", max compression
```

## Comparing `folium_vectorgrid_geojson-1.1.0.tar` & `folium_vectorgrid_geojson-1.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1060 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.0/LICENSE
--rw-r--r--   0        0        0      146 2023-06-21 14:54:04.178169 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/__init__.py
--rw-r--r--   0        0        0     3936 2023-06-21 14:47:04.377711 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/heat_map.py
--rw-r--r--   0        0        0     5596 2023-06-21 14:38:37.225122 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/template/leaflet_heat.min.js
--rw-r--r--   0        0        0     4337 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid.py
--rw-r--r--   0        0        0     4360 2023-06-20 13:06:27.363853 folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid_geojson.py
--rw-r--r--   0        0        0     2027 2023-06-21 14:53:49.186153 folium_vectorgrid_geojson-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3699 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.0/readme.md
--rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 folium_vectorgrid_geojson-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.1/LICENSE
+-rw-r--r--   0        0        0      146 2023-06-22 14:51:56.128437 folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/__init__.py
+-rw-r--r--   0        0        0     4031 2023-06-22 14:50:57.792416 folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/heat_map.py
+-rw-r--r--   0        0        0     5596 2023-06-21 14:38:37.225122 folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/template/leaflet_heat.min.js
+-rw-r--r--   0        0        0     4337 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/vectorgrid.py
+-rw-r--r--   0        0        0     4360 2023-06-20 13:06:27.363853 folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/vectorgrid_geojson.py
+-rw-r--r--   0        0        0     2027 2023-06-22 14:51:29.040431 folium_vectorgrid_geojson-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3699 2023-06-05 11:02:56.625854 folium_vectorgrid_geojson-1.1.1/readme.md
+-rw-r--r--   0        0        0     4369 1970-01-01 00:00:00.000000 folium_vectorgrid_geojson-1.1.1/PKG-INFO
```

### Comparing `folium_vectorgrid_geojson-1.1.0/LICENSE` & `folium_vectorgrid_geojson-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/heat_map.py` & `folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/heat_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,18 @@
     name : string, default None
         The name of the Layer, as it will appear in LayerControls.
     min_opacity  : default 1.
         The minimum opacity the heat will start at.
     max_zoom : default 18
         Zoom level where the points reach maximum intensity (as intensity
         scales with zoom), equals maxZoom of the map by default
+    max_zoom_v: int, default None (the max zoom level of the base layer)
+        The maximum zoom level up to which this layer will be displayed (inclusive).
+    min__zoom_v: int, default 0
+        The minimum zoom level down to which this layer will be displayed (inclusive).
     radius : int, default 25
         Radius of each "point" of the heatmap
     blur : int, default 15
         Amount of blur
     gradient : dict, default None
         Color gradient config. e.g. {0.4: 'blue', 0.65: 'lime', 1: 'red'}
     overlay : bool, default True
@@ -54,16 +58,15 @@
         {% endmacro %}
         """
     )
 
     default_js = [
         (
             "leaflet-heat.js",
-            # Note is is an actual link to the templete files in github. It would be better to refeer to some other link for instance to https://cdn.jsdelivr.net.
-            "https://raw.githubusercontent.com/zarandras/folium-vectorgrid/vectorgrid-geojson/folium_vectorgrid_geojson/template/leaflet_heat.min.js",
+            "https://cdn.jsdelivr.net/gh/zarandras/folium-vectorgrid@latest/folium_vectorgrid_geojson/template/leaflet_heat.min.js",
         ),
     ]
 
     def __init__(
         self,
         data,
         name=None,
```

### Comparing `folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/template/leaflet_heat.min.js` & `folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/template/leaflet_heat.min.js`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid.py` & `folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/vectorgrid.py`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.1.0/folium_vectorgrid_geojson/vectorgrid_geojson.py` & `folium_vectorgrid_geojson-1.1.1/folium_vectorgrid_geojson/vectorgrid_geojson.py`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.1.0/pyproject.toml` & `folium_vectorgrid_geojson-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "folium-vectorgrid-geojson"
 #name = "folium-vectorgrid"
-version = "1.1.0"
+version = "1.1.1"
 description = "VectorGrid plugin for folium"
 repository = "https://github.com/zarandras/folium-vectorgrid"
 authors = ["Lukács Gábor <lukacs.hod@gmail.com>", "Molnár András <molnar.andras.jozsef@gmail.com>", "Benjamin Ramser <ahoi@ipwnd.pw>"]
 license = "MIT"
 readme = "readme.md"
 
 [tool.poetry.dependencies]
```

### Comparing `folium_vectorgrid_geojson-1.1.0/readme.md` & `folium_vectorgrid_geojson-1.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `folium_vectorgrid_geojson-1.1.0/PKG-INFO` & `folium_vectorgrid_geojson-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: folium-vectorgrid-geojson
-Version: 1.1.0
+Version: 1.1.1
 Summary: VectorGrid plugin for folium
 Home-page: https://github.com/zarandras/folium-vectorgrid
 License: MIT
 Author: Lukács Gábor
 Author-email: lukacs.hod@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: folium-vectorgrid-geojson Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: folium-vectorgrid-geojson Version: 1.1.1 Summary:
 VectorGrid plugin for folium Home-page: https://github.com/zarandras/folium-
 vectorgrid License: MIT Author: LukÃ¡cs GÃ¡bor Author-email:
 lukacs.hod@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: folium (>=0.14.0,<0.15.0) Project-URL: Repository, https://
```

