# Comparing `tmp/KMLPlus-3.0.0b3.tar.gz` & `tmp/KMLPlus-3.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KMLPlus-3.0.0b3.tar", last modified: Fri Jun 16 14:30:15 2023, max compression
+gzip compressed data, was "KMLPlus-3.0.0b4.tar", last modified: Thu Jun 22 14:35:11 2023, max compression
```

## Comparing `KMLPlus-3.0.0b3.tar` & `KMLPlus-3.0.0b4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/KMLPlus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-16 14:30:15.000000 KMLPlus-3.0.0b3/KMLPlus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/kmlplus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22594 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/kml.py
--rw-r--r--   0 runner    (1001) docker     (123)    21114 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/kmlplus/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:15.527131 KMLPlus-3.0.0b3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10426 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/test_geo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-16 14:30:07.000000 KMLPlus-3.0.0b3/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/KMLPlus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 14:35:11.000000 KMLPlus-3.0.0b4/KMLPlus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11208 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/kmlplus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22594 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10654 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/kml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21056 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/kmlplus/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:35:11.465559 KMLPlus-3.0.0b4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/test_geo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8784 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4744 2023-06-22 14:34:55.000000 KMLPlus-3.0.0b4/test/test_util.py
```

### Comparing `KMLPlus-3.0.0b3/KMLPlus.egg-info/PKG-INFO` & `KMLPlus-3.0.0b4/KMLPlus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,15 +58,15 @@
 Installing
 ----------
 
 ### Pip
 
 ```
 pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus==3.0.0b1 <--- Current v3.0.0-beta.1
+pip install kmlplus==3.0.0b3 <--- Current v3.0.0-beta.3
 ```
 
 ### Clone
 
 ```
 git clone https://github.com/MHenderson1988/kmlplus.git
```

### Comparing `KMLPlus-3.0.0b3/LICENSE` & `KMLPlus-3.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b3/PKG-INFO` & `KMLPlus-3.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KMLPlus
-Version: 3.0.0b3
+Version: 3.0.0b4
 Summary: A Python library for creating 3d floating polygons and circles in .kml for Google Earth.
 Home-page: https://github.com/MHenderson1988/kmlplus
 Author: Mark Henderson
 Author-email: mark.henderson1988@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,15 +58,15 @@
 Installing
 ----------
 
 ### Pip
 
 ```
 pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus==3.0.0b1 <--- Current v3.0.0-beta.1
+pip install kmlplus==3.0.0b3 <--- Current v3.0.0-beta.3
 ```
 
 ### Clone
 
 ```
 git clone https://github.com/MHenderson1988/kmlplus.git
```

### Comparing `KMLPlus-3.0.0b3/README.md` & `KMLPlus-3.0.0b4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 Installing
 ----------
 
 ### Pip
 
 ```
 pip install kmlplus==2.1.0  <--- last stable release
-pip install kmlplus==3.0.0b1 <--- Current v3.0.0-beta.1
+pip install kmlplus==3.0.0b3 <--- Current v3.0.0-beta.3
 ```
 
 ### Clone
 
 ```
 git clone https://github.com/MHenderson1988/kmlplus.git
```

### Comparing `KMLPlus-3.0.0b3/kmlplus/geo.py` & `KMLPlus-3.0.0b4/kmlplus/geo.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b3/kmlplus/interface.py` & `KMLPlus-3.0.0b4/kmlplus/interface.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b3/kmlplus/kml.py` & `KMLPlus-3.0.0b4/kmlplus/kml.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,16 @@
         self.save_name = kwargs.get('file_name', 'KmlPlus.kml')
         self.kml = simplekml.Kml()
 
     def point(self, coordinate_list: list, **kwargs: str) -> None:
         """
 
         Args:
-            coordinate_list (list): A list containing a single coordinate
+            coordinate_list (list): A list containing a single coordinate. Z values are to be given
+            in metres (M).
 
         Keyword Args:
             fol (str): A string to name the folder in which the point is stored.
             point_name (str): String to name the point object
             colour_hex (str): String representing a colour hex
             extrude (int): 1 or 0, Whether to extrude the point
             altitude_mode (str): Accepts simplekml Altitude mode options
```

### Comparing `KMLPlus-3.0.0b3/kmlplus/shapes.py` & `KMLPlus-3.0.0b4/kmlplus/shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
     __slots__ = (
     'uom', 'sample', 'radius_uom', '_lower_radius', '_upper_radius', '_upper_layer', '_lower_layer', '_sides')
 
     def __init__(self, lower_coordinates: list, upper_coordinates: list, **kwargs):
         self.uom = kwargs.get('uom', 'FT')
         self.sample = kwargs.get('sample', 100)
         self.radius_uom = kwargs.get('radius_uom', 'M')
-        self.lower_radius = convert_to_metres(lower_coordinates[1], self.uom)
-        self.upper_radius = convert_to_metres(upper_coordinates[1], self.uom)
+        self.lower_radius = lower_coordinates[1]
+        self.upper_radius = upper_coordinates[1]
         self.lower_layer = self.create_layer(
             (lower_coordinates[0], self.lower_radius),
             kwargs.get('lower_layer', None)
         )
         self._upper_layer = self.create_layer(
             (upper_coordinates[0], self.upper_radius),
             kwargs.get('upper_layer', None)
```

### Comparing `KMLPlus-3.0.0b3/kmlplus/util.py` & `KMLPlus-3.0.0b4/kmlplus/util.py`

 * *Files identical despite different names*

### Comparing `KMLPlus-3.0.0b3/setup.py` & `KMLPlus-3.0.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="KMLPlus",  # Replace with your own username
-    version="3.0.0-beta.3",
+    version="3.0.0-beta.4",
     author="Mark Henderson",
     author_email="mark.henderson1988@gmail.com",
     description="A Python library for creating 3d floating polygons and circles in .kml for Google Earth.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MHenderson1988/kmlplus",
     packages=setuptools.find_packages(),
```

### Comparing `KMLPlus-3.0.0b3/test/test_geo.py` & `KMLPlus-3.0.0b4/test/test_geo.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,25 +77,33 @@
 
 
 class TestPointFactory(TestCase):
     def setUp(self):
         self.pf = PointFactory(['22.323232 -4.287282', '23.323232 -5.328723', '22.112333 -6.23789238923'])
 
     def test_process_coordinates(self):
+        # Test that decimal degrees coordinates are correctly returned as decimal degrees.
+
         test_dd = self.pf.process_coordinates()
         for i in range(len(test_dd)):
             self.assertTrue(isinstance(test_dd[i], Point))
 
+        self.assertEqual(3, len(test_dd))
+        self.assertEqual(test_dd[0].y, 22.323232)
+        self.assertTrue(isinstance(test_dd[0].y, float))
+
         # Test that dms coordinates are correctly returned as decimal degrees.
         test_dms = self.pf.process_coordinates()
         type_result = util.detect_coordinate_type(f'{test_dms[0].y} {test_dms[0].x}')
         self.assertEqual(type_result, 'dd')
 
     def test_populate_point_list(self):
         test_point_list = self.pf.populate_point_list()
+        self.assertNotEqual(test_point_list, None)
+        self.assertAlmostEqual(test_point_list[0].y, 22.323232, delta=0.0000001)
         self.assertTrue(isinstance(test_point_list, list))
         self.assertEqual(3, len(test_point_list))
 
     def test_create_curved_segment(self):
         test_segment = self.pf.create_curved_segment('start=553322N 0043322W, centre=502211N 0043222W, end=510000N '
                                                      '0040010W, direction=clockwise')
```

### Comparing `KMLPlus-3.0.0b3/test/test_util.py` & `KMLPlus-3.0.0b4/test/test_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,17 @@
         result = detect_coordinate_type('0045645.21W 0045645.21W')
         self.assertEqual('dms', result)
 
     def test_point_or_segment(self):
         # point, no height
         coordinate_string = '521244N, 0056555W'
         result = point_or_segment(coordinate_string)
-        pass
+        self.assertEqual(result, 'point')
+        self.assertNotEqual(result, 'segment')
+        self.assertTrue(isinstance(result, str))
 
     def test_split_segment_string(self):
         string = 'start=522423N 0042354W, end=522428N 0042254W, direction=clockwise,' \
                  ' centre=502211N 0043212W, sample=50'
         d = split_segment_string(string)
 
         self.assertTrue(isinstance(d, dict))
@@ -110,9 +112,12 @@
 
         result = convert_to_metres(1, 'm')
         self.assertEqual(1, result)
 
         result = convert_to_metres(1, 'Ft')
         self.assertEqual(0.3048, result)
 
+        result = convert_to_metres(1, 'ft')
+        self.assertEqual(0.3048, result)
+
         with self.assertRaises(TypeError):
             convert_to_metres(20, 'fdskl;jfdasjkl;adf')
```

