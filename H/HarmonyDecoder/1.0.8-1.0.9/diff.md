# Comparing `tmp/HarmonyDecoder-1.0.8.tar.gz` & `tmp/HarmonyDecoder-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HarmonyDecoder-1.0.8.tar", last modified: Sun Jun 18 20:26:51 2023, max compression
+gzip compressed data, was "HarmonyDecoder-1.0.9.tar", last modified: Thu Jun 22 18:51:22 2023, max compression
```

## Comparing `HarmonyDecoder-1.0.8.tar` & `HarmonyDecoder-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/
--rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.8/LICENSE
--rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0    42858 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.8/README.md
--rw-rw-rw-   0        0        0      722 2023-06-18 20:26:25.000000 HarmonyDecoder-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.141614 HarmonyDecoder-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.161736 HarmonyDecoder-1.0.8/src/HarmonyDecoder/
-drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/
--rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/BassCleff.png
--rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Flat.png
--rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Icon.png
--rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Sharp.png
--rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/TrebleCleff.png
--rw-rw-rw-   0        0        0      207 2023-06-18 20:02:32.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/__init__.py
--rw-rw-rw-   0        0        0    11022 2023-06-18 20:16:53.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/drawing.py
--rw-rw-rw-   0        0        0     4202 2023-06-18 20:05:58.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/function.py
--rw-rw-rw-   0        0        0       55 2023-06-18 20:24:39.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/harmony.py
--rw-rw-rw-   0        0        0     2585 2023-06-18 19:35:09.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/interval.py
--rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/logger.py
--rw-rw-rw-   0        0        0     3575 2023-06-16 07:11:26.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/note.py
--rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/possiblenotes.py
--rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/program.py
--rw-rw-rw-   0        0        0    15019 2023-06-18 19:42:46.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/rules.py
--rw-rw-rw-   0        0        0     4252 2023-06-18 19:42:56.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/scale.py
--rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/setup.py
--rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/strdecoder.py
--rw-rw-rw-   0        0        0    37529 2023-06-18 19:34:30.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder/ui.py
-drwxrwxrwx   0        0        0        0 2023-06-18 20:26:51.177361 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/
--rw-rw-rw-   0        0        0    42858 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      858 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-18 20:26:51.000000 HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 18:51:22.951839 HarmonyDecoder-1.0.9/
+-rw-rw-rw-   0        0        0    35801 2023-06-18 16:59:03.000000 HarmonyDecoder-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0       39 2023-06-18 18:13:19.000000 HarmonyDecoder-1.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    42858 2023-06-22 18:51:22.950836 HarmonyDecoder-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1095 2023-06-18 18:16:25.000000 HarmonyDecoder-1.0.9/README.md
+-rw-rw-rw-   0        0        0      722 2023-06-20 16:49:30.000000 HarmonyDecoder-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-22 18:51:22.953037 HarmonyDecoder-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 18:51:22.837654 HarmonyDecoder-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-06-22 18:51:22.899927 HarmonyDecoder-1.0.9/src/HarmonyDecoder/
+drwxrwxrwx   0        0        0        0 2023-06-22 18:51:22.944128 HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/
+-rw-rw-rw-   0        0        0    13455 2023-06-15 07:00:17.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/BassCleff.png
+-rw-rw-rw-   0        0        0     7610 2023-06-16 06:31:24.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/Flat.png
+-rw-rw-rw-   0        0        0   135161 2023-06-16 05:56:57.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/Icon.png
+-rw-rw-rw-   0        0        0     2165 2023-06-16 06:30:58.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/Sharp.png
+-rw-rw-rw-   0        0        0    17112 2023-06-15 06:58:41.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/TrebleCleff.png
+-rw-rw-rw-   0        0        0      274 2023-06-21 06:01:53.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/__init__.py
+-rw-rw-rw-   0        0        0    14085 2023-06-19 11:19:57.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/drawing.py
+-rw-rw-rw-   0        0        0     4202 2023-06-18 20:05:58.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/function.py
+-rw-rw-rw-   0        0        0       54 2023-06-20 20:45:16.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/harmony.py
+-rw-rw-rw-   0        0        0     3857 2023-06-22 18:49:04.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/interval.py
+-rw-rw-rw-   0        0        0      252 2023-06-14 16:55:50.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/logger.py
+-rw-rw-rw-   0        0        0     4244 2023-06-21 06:10:41.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/note.py
+-rw-rw-rw-   0        0        0     3196 2023-06-18 19:33:31.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/possiblenotes.py
+-rw-rw-rw-   0        0        0     7261 2023-06-18 19:35:04.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/program.py
+-rw-rw-rw-   0        0        0    15949 2023-06-20 20:45:42.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/rules.py
+-rw-rw-rw-   0        0        0     4252 2023-06-18 19:42:56.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/scale.py
+-rw-rw-rw-   0        0        0       62 2023-06-18 18:13:38.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/setup.py
+-rw-rw-rw-   0        0        0     9371 2023-06-16 06:08:37.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/strdecoder.py
+-rw-rw-rw-   0        0        0    39987 2023-06-20 21:25:28.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder/ui.py
+drwxrwxrwx   0        0        0        0 2023-06-22 18:51:22.920613 HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/
+-rw-rw-rw-   0        0        0    42858 2023-06-22 18:51:22.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      858 2023-06-22 18:51:22.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 18:51:22.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-22 18:51:22.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-22 18:51:22.000000 HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/top_level.txt
```

### Comparing `HarmonyDecoder-1.0.8/LICENSE` & `HarmonyDecoder-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/PKG-INFO` & `HarmonyDecoder-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.8
+Version: 1.0.9
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.8/README.md` & `HarmonyDecoder-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/pyproject.toml` & `HarmonyDecoder-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HarmonyDecoder"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" },
 ]
 maintainers = [
   { name="Przemysław Kojs", email="przemek.kojs@gmail.com" }
 ]
 dependencies = [
```

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/BassCleff.png` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/BassCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Flat.png` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/Flat.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Icon.png` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/Icon.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/Sharp.png` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/Sharp.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/Images/TrebleCleff.png` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/Images/TrebleCleff.png`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/drawing.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/drawing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from PIL import Image, ImageDraw
 from HarmonyDecoder.note import note
 from HarmonyDecoder.function import function
 from HarmonyDecoder.note import note
-from HarmonyDecoder.scale import scale
+from HarmonyDecoder.scale import scale, sharps_by_major_key, sharps_by_minor_key, flats_by_major_key, flats_by_minor_key
 import os
 
 
 class drawing:
     def __init__(self, tonation:scale = scale('C', 'major')) -> None:
         if tonation is None:
             raise TypeError("tonation cannot be none")
@@ -53,43 +53,22 @@
     def draw_measure_line(self, pos_x:int, pos_y:int) -> None:
         start_x:int = self.__margin_x + pos_x
         end_x:int = start_x
 
         start_y:int = self.__margin_y + pos_y
         end_y:int = self.__margin_y + pos_y + (4 * self.__staff_line_spacing) + self.__staff_spacing
 
-        self.__draw_line((start_x, start_y), (end_x, end_y), self.__staff_line_width, self.__staff_color)
-
-    def insert_image(self, pos_x:int, pos_y:int, source:str, scale:float=1.0) -> None:
-        if pos_x < 0 or pos_x > self.__size_x or pos_y < 0 or pos_y > self.__size_y:
-            raise ValueError("Cannot insert image oudside the canvas.")
-        
-        try:
-            to_insert:Image.Image = Image.open(source)
-        except FileNotFoundError:
-            print(f"File {source} not found.")
-            return
-        
-        size:tuple[int, int] = (to_insert.size[0], to_insert.size[1])
-        max_y:int = 10 * self.__staff_line_spacing
-        resize_value:int = (size[1] / max_y) / scale
-
-        to_insert = to_insert.resize(
-            (int(size[0] / resize_value),
-            int(size[1] / resize_value))
-        )
-        
-        self.__image.paste(to_insert, (pos_x, pos_y - int(to_insert.size[1] / 2)))
+        self.__draw_line((start_x, start_y), (end_x, end_y), self.__staff_line_width, self.__staff_color)    
 
     def draw_note(self, what:note, direction:str="up", cleff:str="Treble", staff_position:int=0, x:int=0) -> None:
         if direction not in ['up', 'down']:
             raise ValueError("Direction must be one of [up, down].")
         
         if cleff not in ['Treble', 'Bass']:
-            raise ValueError("Key must be one of [up, down]")
+            raise ValueError("Key must be one of [Treble, Bass]")
         
         if what is None:
             raise TypeError("Note cannot be none.")
         
         if cleff == 'Treble':
             C5_position:int = int(4.5 * self.__staff_line_spacing)
         else:
@@ -184,19 +163,19 @@
                         self.__staff_color
                     )
                     
                     add_line_start_y += self.__staff_line_spacing                
         
         sign_x:int = note_start_x - int(self.__staff_line_spacing * 1.5)        
 
-        if '#' in what.name: #and what.name not in self.__tonation.notes:
+        if '#' in what.name and what.name not in self.__tonation.notes:
             sign_y:int = note_start_y - int(self.__staff_line_spacing * 0.5)
             to_insert:Image.Image = self.__sharp
             self.__image.paste(to_insert, (sign_x, sign_y))
-        elif 'b' in what.name: #and what.name not in self.__tonation.notes:
+        elif 'b' in what.name and what.name not in self.__tonation.notes:
             sign_y:int = note_start_y - int(self.__staff_line_spacing * 0.8)
             to_insert:Image.Image = self.__flat
             self.__image.paste(to_insert, (sign_x, sign_y))        
 
     def draw_function(self, what:function, staff_position:int=0, x:int=0) -> None:
         self.draw_note(what.soprano, "up", "Treble", staff_position, x)
         self.draw_note(what.alto, "down", "Treble", staff_position, x)
@@ -206,34 +185,39 @@
     def save(self, name:str) -> None:
         self.__image.save(name)
 
 # private:
     def __draw_line(self, start:tuple[int, int], end:tuple[int, int], width:int, color:str) -> None:
         for coordinate in [start[0], end[0]]:
             if coordinate < 0 or coordinate > self.__size_x:
-                raise ValueError("Cannot draw line outside of the canvas.")
+                print("Cannot draw line outside of the canvas.")
+                return
             
         for coordinate in [start[1], end[1]]:
             if coordinate < 0 or coordinate > self.__size_y:
-                raise ValueError("Cannot draw line outside of the canvas.")
+                print("Cannot draw line outside of the canvas.")
+                return
 
         self.__drawing.line(
             [start, end],
             width=width,
             fill=color
         )
 
     def __draw_one_staff(self, pos_y:int, cleff:str) -> None:
         if pos_y < 0 or (pos_y + 6 * self.__staff_line_spacing) > self.__size_y:
-            raise ValueError("Cannot draw staff outside of the canvas.")
+            print("Cannot draw staff outside of the canvas.")
+            return
         
         scale:int = 0.5 if cleff == 'Bass' else 1
+        
+        self.__draw_tonation(pos_y, cleff)
 
-        self.insert_image(
-            self.__margin_x + self.__function_spacing,
+        self.__insert_image(
+            2 * self.__margin_x,
             self.__margin_y + 2 * self.__staff_line_spacing + pos_y,
             f'{os.path.dirname(os.path.realpath(__file__))}/Images/{cleff}Cleff.png',
             scale=scale
         )
 
         for index in range(5):
             start_x:int = self.__margin_x
@@ -253,14 +237,100 @@
         )
 
         resize_scalar = int((self.__flat.size[1] / self.__staff_line_spacing) / 2)
 
         self.__flat = self.__flat.resize(
             (int(self.__flat.size[0] / resize_scalar),
             int(self.__flat.size[1] / resize_scalar))
+        )   
+    
+    def __insert_image(self, pos_x:int, pos_y:int, source:(str | Image.Image), scale:float=1.0) -> None:
+        if pos_x < 0 or pos_x > self.__size_x or pos_y < 0 or pos_y > self.__size_y:
+            print("Cannot insert image oudside the canvas.")
+            return
+        
+        if isinstance(source, str):
+            try:
+                to_insert:Image.Image = Image.open(source)
+            except FileNotFoundError:
+                print(f"File {source} not found.")
+                return
+            
+            size:tuple[int, int] = (to_insert.size[0], to_insert.size[1])
+            max_y:int = 10 * self.__staff_line_spacing
+            resize_value:int = (size[1] / max_y) / scale
+
+            to_insert = to_insert.resize(
+                (int(size[0] / resize_value),
+                int(size[1] / resize_value))
+            )
+        else:
+            to_insert:Image.Image = source
+        
+        self.__image.paste(to_insert, (pos_x, pos_y - int(to_insert.size[1] / 2)))
+
+    def __draw_tonation(self, staff_position:int, cleff:str) -> None:
+        if cleff not in ['Treble', 'Bass']:
+            raise ValueError("Key must be one of [Treble, Bass]")
+
+        sharp_positions_y:tuple[tuple[str, int]] = (
+            ('F#', 0),
+            ('C#', int(self.__staff_line_spacing * 1.5)),
+            ('G#', int(self.__staff_line_spacing * (-0.5))),
+            ('D#', self.__staff_line_spacing),
+            ('A#', int(self.__staff_line_spacing * 2.5)),
+            ('E#', int(self.__staff_line_spacing * 0.5)),
+            ('B#', self.__staff_line_spacing * 2)
+        )
+
+        flat_positions_y:tuple[tuple[str, int]] = (
+            ('Bb', self.__staff_line_spacing * 2),
+            ('Eb', int(self.__staff_line_spacing * 0.5)),
+            ('Ab', int(self.__staff_line_spacing * 2.5)),
+            ('Db', self.__staff_line_spacing),
+            ('Gb', self.__staff_line_spacing * 3),
+            ('Cb', int(self.__staff_line_spacing * 1.5)),
+            ('Fb', int(self.__staff_line_spacing * 3.5))
         )
 
+        sign_start_x:int = self.__margin_x * 6
+
+        if cleff == 'Treble':
+            y_modifier:int = -int(self.__staff_line_spacing / 2)
+        else:
+            y_modifier:int = int(self.__staff_line_spacing / 2)
+
+        if self.__tonation.mode == 'minor':
+            if self.__tonation.name in list(sharps_by_minor_key.keys()):
+                tonation_signs:int = sharps_by_minor_key[self.__tonation.name]
+                sign:str = '#'
+            elif self.__tonation.name in list(flats_by_minor_key.keys()):
+                tonation_signs:int = flats_by_minor_key[self.__tonation.name]
+                sign:str = 'b'
+        else:
+            if self.__tonation.name in list(sharps_by_major_key.keys()):
+                tonation_signs:int = sharps_by_major_key[self.__tonation.name]
+                sign:str = '#'
+            elif self.__tonation.name in list(flats_by_major_key.keys()):
+                tonation_signs:int = flats_by_major_key[self.__tonation.name]
+                sign:str = 'b'
+
+        if sign == '#':
+            for index in range(tonation_signs):
+                self.__insert_image(
+                    sign_start_x + index * self.__staff_line_spacing + self.__margin_x,
+                    sharp_positions_y[index][1] + staff_position + y_modifier + self.__margin_y,
+                    self.__sharp
+                )
+        else:
+            for index in range(tonation_signs):
+                self.__insert_image(
+                    sign_start_x + index * self.__staff_line_spacing + self.__margin_x,
+                    flat_positions_y[index][1] + staff_position + y_modifier + self.__margin_y,
+                    self.__flat
+                )
+
     def __get_image(self) -> Image.Image:
         return self.__image
 
 # properties:
     image:Image.Image = property(__get_image)
```

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/function.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/function.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/note.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/note.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+'''Module containing everything referring to single musical note.
+
+Attributes
+----------
+all_notes : dict[str, int]
+    Dictionary of all note names mapped to their distance in semitones from the "C" note.
+
+ROOT_ROLE : str
+    Role describing note's role as root in function.
+
+THIRD_ROLE : str
+    Role describing note's role as third in function.
+
+FIFTH_ROLE : str
+    Role describing note's role as fifth in function.
+
+SIXTH_ROLE : str
+    Role describing note's role as sixth in function.
+
+SEVENTH_ROLE : str
+    Role describing note's role as seventh in function.
+
+NINTH_ROLE : str
+    Role describing note's role as ninth in function.
+'''
+
 all_notes:dict[str, int] = {        
         'C' : 0,    'Dbb' : 0,  'B#' : 0,
         'C#' : 1,   'Db' : 1,   'B##' : 1,
         'D' : 2,    'Ebb' : 2,  'C##' : 2,
         'D#' : 3,   'Eb' : 3,   'Fbb' : 3,
         'E' : 4,    'Fb' : 4,   'D##' : 4,
         'F' : 5,    'Gbb' : 5,  'E#' : 5,
@@ -9,20 +35,20 @@
         'G' : 7,   'Abb' : 7, 'F##' : 7,
         'G#': 8,   'Ab' : 8,
         'A' : 9,    'Bbb' : 9,  'G##' : 9,
         'A#' : 10,   'Bb' : 10,   'Cbb' : 10,
         'B' : 11,    'Cb': 11,    'A##' : 11,
     }
 
-ROOT_ROLE = "Root"
-THIRD_ROLE = "Third"
-FIFTH_ROLE = "Fifth"
-SIXTH_ROLE = "Sixth"
-SEVENTH_ROLE = "Seventh"
-NINTH_ROLE = "Ninth"
+ROOT_ROLE:str = "Root"
+THIRD_ROLE:str = "Third"
+FIFTH_ROLE:str = "Fifth"
+SIXTH_ROLE:str = "Sixth"
+SEVENTH_ROLE:str = "Seventh"
+NINTH_ROLE:str = "Ninth"
 
 class note:
     # Dictionary of all notes and their distance from note 'A' (in semitones)
     def __init__(self, name:str, octave:str, role:(str | None)=None):
         self.__name:str = name
         self.__octave:int = octave
         self.__role:(str | None) = role
```

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/possiblenotes.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/possiblenotes.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/program.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/program.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/rules.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from __future__ import annotations
 
 import abc
 
 from HarmonyDecoder.function import *
+from HarmonyDecoder.function import function
 from HarmonyDecoder.possiblenotes import possible_notes
 from HarmonyDecoder.scale import scale
 
 class rule_manager:
     def __init__(self):
         self._active_rules:list[rule] = [
             voice_crossing(),
             parallel_fifth(),
             parallel_octave(),
             one_direction(),
             seventh_down(),
             third_up(),
             ninth_down(),
             fifth_on_one(),
-            ninth_as_root()
+            ninth_as_root(),
+            voice_distance()
         ]
 
         self.__rules:list[rule] = self._active_rules.copy()
 
 # public:
     def activate_rule(self, name:str) -> None: self.__set_rule_state(name, True)
     def deactivate_rule(self, name:str) -> None: self.__set_rule_state(name, False)    
@@ -415,8 +417,31 @@
         if function2 is None:
             if function1.bass.is_ninth():
                 return False
               
         if function2.bass.is_ninth():
             return False
             
-        return True
+        return True
+    
+
+class voice_distance(rule):
+    def __init__(self, description:str="Some rule.", active:bool=True):
+        rule.__init__(self, description, active)
+
+    def check_if_fulfilled(self, function1: (function | None), function2: (function | None)) -> bool:
+        if function1 is None and function2 is None:
+            return True
+        
+        def check_function(function:(function | None)) -> bool:
+            if function is None:
+                return True
+            
+            if semitones_between(function.bass, function.tenore) > 24 or\
+                semitones_between(function.tenore, function.alto) > 12 or\
+                semitones_between(function.alto, function.soprano) > 12:
+                return False
+            
+            return True
+
+        return check_function(function1) and check_function(function2)
+
```

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/scale.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/scale.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/strdecoder.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/strdecoder.py`

 * *Files identical despite different names*

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder/ui.py` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder/ui.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 
 import sys
 
 arial_12:QFont = QFont('Arial', 12)
 arial_24:QFont = QFont('Arial', 24)
 
 class ui_solution(QWidget):
+    ''''''
+
     def __init__(self, parent:ui_program) -> None:
+        ''''''
+
         super().__init__()
 
         self.__parent:ui_program = parent        
         self.__drawing:drawing = drawing(self.__parent.program.tonation)
         self.__solutions:tuple[list[function]] = parent.program.solution
 
         self.setWindowTitle("Harmony decoder - solutions")
@@ -75,18 +79,23 @@
 
         self.__draw_solution_button.clicked.connect(self.__draw)
         self.__cancel_button.clicked.connect(self.closeEvent)
         self.__save_button.clicked.connect(self.__save)
 
 # public:
     def closeEvent(self, event: QCloseEvent) -> None:
+        ''''''
+
+        event.accept()
         self.__parent.close_solution()
 
 # private:
-    def __draw(self) -> None:        
+    def __draw(self) -> None:  
+        ''''''
+
         self.__drawing.clear()
 
         if self.__parent.program.task == []:
             self.__parent.program.program_logger.log("Cannot draw empty solution.")
             return
         
         if self.__parent.program.solution != ():
@@ -94,25 +103,24 @@
             index:int = 0
 
             for function in solution:
                 self.__drawing.draw_function(function, x=index)
                 index += 1
 
         self.__parent.program.program_logger.log("Drawing solution...")
-
         self.__drawing.draw_staff()
-
         self.__parent.program.program_logger.log("Solution drawn...")
-        self.__parent.program.program_logger.log("Showing  solution...")
 
+        self.__parent.program.program_logger.log("Showing  solution...")
         self.__drawing.show()
-
         self.__parent.program.program_logger.log("Solution shown.")
 
     def __save(self) -> None:
+        ''''''
+
         path:str = filedialog.askdirectory(
             initialdir=self.__parent.last_save_directory,
             mustexist=True,
             title="Choose save directory"
         )
 
         if len(path) >= 1:
@@ -121,15 +129,57 @@
             self.__parent.last_save_directory = path
             self.__parent.program.program_logger.log(f"File {filename} saved to {path}")
         else:
             self.__parent.program.program_logger.log("Saving canceled.")
 
 
 class ui_rules(QWidget):
+    '''Class used to manage rules, usually of other ui_program set to parent of this class.
+    '''
+
     def __init__(self, rules:rule_manager, parent:ui_program) -> None:
+        '''Class' constructor. Creates new ui_rules object with rules system and parent
+
+        Parameters
+        ----------
+        rules : rule_manager
+            Rules system to be used and (optionally) changed. It should be the same system as in parent form (usually), but it is not mandatory.
+        
+        parent : ui_program
+            Parent form.
+
+        Returns
+        -------
+        None
+            Constructor does not return anything.
+
+        Raises
+        ------
+        TypeError
+            If ``rules`` or ``program`` parameters are ``NoneType``.
+
+        See also
+        --------
+            rule_manager : Class for managing rules.
+            ui_program : Main workspace class.
+
+        Examples
+        --------
+        >>> rules:ui_rules = ui_rules(None, None)
+        TypeError: "Cannot initialize ui_rules class with no rules or parent."
+
+        >>> rules:rule_manager = rule_manager()
+        >>> program:ui_program = ui_program()
+        >>> rules_ui:ui_rules = ui_rules(rules, program)
+
+        '''
+
+        if rules is None or parent is None:
+            raise TypeError("Cannot initialize ui_rules class with no rules or parent.")
+
         super().__init__()
 
         self.__parent:ui_program = parent
         self.rules:rule_manager = rules
 
         self.setWindowTitle("Harmony decoder - rules")
         self.setGeometry(0, 0, 300, 400)
@@ -140,14 +190,15 @@
         self.__parallel_octave_checkbox:QCheckBox = QCheckBox("Parallel octaves checking")
         self.__one_direction_checkbox:QCheckBox = QCheckBox("One direction checking")
         self.__seventh_down_checkbox:QCheckBox = QCheckBox("Seventh down checking")
         self.__third_up_checkbox:QCheckBox = QCheckBox("Third up checking")
         self.__ninth_down_checkbox:QCheckBox = QCheckBox("Ninth down checking")
         self.__fifth_on_one_checkbox:QCheckBox = QCheckBox("Fifth on the first beat checking")
         self.__ninth_as_root_checkbox:QCheckBox = QCheckBox("Ninth as root checking")
+        self.__voice_distance_checkbox:QCheckBox = QCheckBox("Voice distance checking")
 
         self.__save_button:QPushButton = QPushButton("Save and quit")
         self.__cancel_button:QPushButton = QPushButton("Cancel")
 
         self.__save_button.setFont(arial_12)
         self.__cancel_button.setFont(arial_12)
 
@@ -157,74 +208,89 @@
         self.layout().addWidget(self.__parallel_octave_checkbox)
         self.layout().addWidget(self.__one_direction_checkbox)
         self.layout().addWidget(self.__seventh_down_checkbox)
         self.layout().addWidget(self.__third_up_checkbox)
         self.layout().addWidget(self.__ninth_down_checkbox)
         self.layout().addWidget(self.__fifth_on_one_checkbox)
         self.layout().addWidget(self.__ninth_as_root_checkbox)
+        self.layout().addWidget(self.__voice_distance_checkbox)
         self.layout().addWidget(self.__save_button)
         self.layout().addWidget(self.__cancel_button)
 
         self.__save_button.clicked.connect(self.__save_and_quit)
         self.__cancel_button.clicked.connect(self.__cancel)
 
         self.__get_state()
 
 # public:
-    def closeEvent(self, event: QCloseEvent) -> None:        
+    def closeEvent(self, event: QCloseEvent) -> None:  
+        ''''''
+
+        event.accept()      
         self.__parent.refresh_rules()
         self.__parent.show()
 
 # private:
     def __save_and_quit(self) -> None:
+        ''''''
+
         checkboxes:list[QCheckBox] = [
             self.__voice_crossing_checkbox,
             self.__parallel_fifth_checkbox,
             self.__parallel_octave_checkbox,
             self.__one_direction_checkbox,
             self.__seventh_down_checkbox,
             self.__third_up_checkbox,
             self.__ninth_down_checkbox,
             self.__fifth_on_one_checkbox,
-            self.__ninth_as_root_checkbox
+            self.__ninth_as_root_checkbox,
+            self.__voice_distance_checkbox
         ]
 
         for index in range(len(checkboxes)):
             if checkboxes[index].isChecked():
                 self.rules.active_rules[index].active = True
             else:
                 self.rules.active_rules[index].active = False
 
         self.close()
 
     def __cancel(self) -> None:
+        ''''''
+
         self.close()
 
     def __get_state(self) -> None:
+        ''''''
+
         checkboxes:list[QCheckBox] = [
             self.__voice_crossing_checkbox,
             self.__parallel_fifth_checkbox,
             self.__parallel_octave_checkbox,
             self.__one_direction_checkbox,
             self.__seventh_down_checkbox,
             self.__third_up_checkbox,
             self.__ninth_down_checkbox,
             self.__fifth_on_one_checkbox,
-            self.__ninth_as_root_checkbox
+            self.__ninth_as_root_checkbox,
+            self.__voice_distance_checkbox
         ]
 
         for index in range(len(checkboxes)):
             if self.rules.active_rules[index].active:
                 checkboxes[index].setChecked(True)
             else:
                 checkboxes[index].setChecked(False)
 
 
 class ui_function_creator(QWidget):
+    ''''''
+
     def __init__(self, parent:ui_program) -> None:
+        ''''''
         super().__init__()
 
         self.__parent:ui_program = parent
 
         self.__major_symbols:tuple[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str] = \
             ("T", "Sii", "mSii", "Tiii", "mDiii", "Diii", "S", "mS", "D", "mD", "Tvi", "Svi", "mSvi", "Dvii", "Svii", "mDvii", "mSvii")
         self.__minor_symbols:tuple[str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str, str] = \
@@ -459,86 +525,116 @@
         self.__set_deleted()
         self.__set_additional()
         self.__set_alterated_1()
         self.__set_alterated_2()
         self.__set_alterated_3()
         self.__set_alterated_4()
 
-# private:
+# private:    
     def __add_raw_symbol(self) -> None:
+        ''''''
+
         if len(self.__raw_text.text()) >= 11:
             symbol = self.__raw_text.text()
         else:
             return
 
         try:
             to_add:str_symbol = str_symbol(symbol)  
 
             self.__parent.program.add_to_task(to_add)
             self.__cancel_button.click()          
         except ValueError:
             self.__parent.program.program_logger.log("Parser error")
             return
-
+    
     def __add_symbol(self) -> None:
+        ''''''
+
         try:
             symbol:str = self.__get_current_state()
             to_add:str_symbol = str_symbol(symbol)
 
             self.__parent.program.add_to_task(to_add)
             self.__cancel_button.click()
         except ValueError:
             self.__parent.program.program_logger.log("Parse error")
             return
-
+    
     def __set_symbol(self) -> None:
+        ''''''
+
         self.__symbol = self.__symbols_combo.currentText()
         self.__refresh_current()
-
+    
     def __set_additional(self) -> None:
+        ''''''
+
         self.__added = self.__addable_combo.currentText()
         self.__refresh_current()
-
+    
     def __set_deleted(self) -> None:
+        ''''''
+
         self.__deleted = self.__deletable_combo.currentText()
         self.__refresh_current()
-
+    
     def __set_alterated_1(self) -> None:
+        ''''''
+
         self.__altered1 = f"{self.__alter_combo_1.currentText()}{self.__sign_combo_1.currentText()}"
         self.__refresh_current()
-
+    
     def __set_alterated_2(self) -> None:
+        ''''''
+
         self.__altered2 = f"{self.__alter_combo_2.currentText()}{self.__sign_combo_2.currentText()}"
         self.__refresh_current()
-
+    
     def __set_alterated_3(self) -> None:
+        ''''''
+
         self.__altered3 = f"{self.__alter_combo_3.currentText()}{self.__sign_combo_3.currentText()}"
         self.__refresh_current()
 
+    
     def __set_alterated_4(self) -> None:
+        ''''''
+
         self.__altered4 = f"{self.__alter_combo_4.currentText()}{self.__sign_combo_4.currentText()}"
         self.__refresh_current()
-
+    
     def __set_root(self) -> None:
+        ''''''
+
         self.__root = self.__root_combo.currentText()
         self.__refresh_current()
-
+    
     def __set_position(self) -> None:
+        ''''''
+
         self.__position = self.__position_combo.currentText()
         self.__refresh_current()
-
+    
     def __cancel(self) -> None:
+        ''''''
+
         self.__parent.show()
         self.__parent.refresh_functions()
         self.close()
 
+    
     def __refresh_current(self) -> None:
-        self.__current_text.setText(self.__get_current_state())
+        ''''''
 
+        self.__current_text.setText(self.__get_current_state())
+    
     def __get_current_state(self) -> str:
+        ''''''
+
         symbol:str = f"{self.__symbol}^{self.__position}/{self.__root}+{self.__added}+-{self.__deleted}-*"
 
         if self.__altered1 != "":
             symbol += self.__altered1 + ","
 
         if self.__altered2 != "":
             symbol += self.__altered2 + ","
@@ -554,15 +650,19 @@
 
         symbol += '*=='
 
         return symbol
 
 
 class ui_program(QWidget):
+    ''''''
+
     def __init__(self) -> None:
+        ''''''
+
         super().__init__()
         
         self.setWindowTitle("Harmony decoder")
         self.setGeometry(0, 0, 600, 400)       
         self.showMaximized()
         self.setWindowIcon(QtGui.QIcon('Images/Icon.png'))
 
@@ -692,26 +792,36 @@
         self.refresh_rules()
         self.refresh_functions()
         self.__change_measure_length()
         self.__change_scale()
 
 # public:
     def closeEvent(self, event:QCloseEvent) -> None:
+        ''''''
+
+        event.accept()
+        
         for window in QApplication.topLevelWidgets():
             window.close()
 
     def close_solution(self) -> None:
+        ''''''
+
         self.solutions = None
 
     def refresh_functions(self) -> None:
+        ''''''
+
         self.creator = None
         self.__input_text.clear()
         self.__input_text.append(self.program.input)
 
     def refresh_rules(self) -> None:
+        ''''''
+
         self.__rules_text.clear()
         self.rules = None
 
         for rule in self.program.rules.active_rules:
             if rule.active:
                 self.__rules_text.append(str(rule))
                 self.program.program_logger.log(f"Rule {str(rule)} activated.")
@@ -721,14 +831,16 @@
         self.program.solution = ()
         self.program.beginning = []
         self.program.input = self.__input_text.toPlainText()
         self.__rules_changed = True
 
 # private:
     def __solve(self) -> None:
+        ''''''
+
         start:datetime = datetime.now()
         self.program.program_logger.log(f"Started solving {str(self.program.input)}")
 
         self.__solve_button.setEnabled(False)
 
         if self.__last_input != self.program.input or self.__last_tonation is None or self.__last_tonation != self.program.tonation or self.__rules_changed:
             self.program.solve()
@@ -742,61 +854,77 @@
         end:datetime = datetime.now()
         self.program.program_logger.log(f"Finished solving {self.program.input}")
         self.program.program_logger.log(f"Total duration: {(end - start).total_seconds()}.\n")
 
         self.__show_solutions()
 
     def __clear_functions(self) -> None:
+        ''''''
+
         self.__input_text.clear()
         self.program.clear()
 
     def __add_function(self) -> None:
+        ''''''
+
         if self.creator is None:
             self.creator = ui_function_creator(self)
             self.creator.show()
             self.hide()
         else:
             self.creator = None
 
     def __show_rules(self) -> None:
+        ''''''
+
         if self.rules is None:
             self.rules = ui_rules(self.program.rules, self)
             self.rules.show()
         else:
             self.rules = None
 
     def __show_solutions(self) -> None:
+        ''''''
+
         if self.solutions is None:
             self.solutions = ui_solution(self)
             self.solutions.show()
         else:
             self.rules = None
 
     def __clear_logs(self) -> None:
+        ''''''
+
         self.__logs_text.clear()
 
     def __change_scale(self) -> None:
+        ''''''
+
         try:
             to_set:scale = scale(self.__tonation_combo.currentText(), self.__mode_combo.currentText())            
         except ValueError:
             self.program.program_logger.log(f"Tonation {self.__tonation_combo.currentText()} {self.__mode_combo.currentText()} not found.")
             return
         
         self.program.tonation = to_set
         self.program.solution = ()
         self.program.beginning = []
         self.program.input = self.__input_text.toPlainText()
 
         self.program.program_logger.log(f"Tonation set to {self.__tonation_combo.currentText()} {self.__mode_combo.currentText()}.")
 
     def __change_measure_length(self) -> None:
+        ''''''
+
         self.program.measure_length = int(self.__measure_length_combo.currentText())
         self.program.program_logger.log(f"Measure length set to {self.__measure_length_combo.currentText()}.")
 
     def __read_from_file(self) -> None:
+        ''''''
+
         filename:str = filedialog.askopenfilename(
             initialdir=self.last_load_directory,
             title="Select a file",
             filetypes=(("Harmony files", "*.harm"), ("Text files", "*.txt"))
         )
 
         self.last_load_directory = ""
@@ -830,15 +958,19 @@
                     self.program.add_to_task(str_symbol(item))
                 except ValueError:
                     self.program.program_logger.log("Invalud function syntax")
                     return
 
 
 class ui_about(QWidget):
+    ''''''
+
     def __init__(self, menu:ui_menu) -> None:
+        ''''''
+
         super().__init__()
         self.__menu:ui_menu = menu
 
         self.__title_label:QLabel = QLabel("About")
         self.__about_text:QTextEdit = QTextEdit("This program is essentialy a harmony task decoder.\
         It takes input as function symbols and gives output as notes drawn on staff.\n\nHappy using!")
 
@@ -855,19 +987,25 @@
         self.setWindowIcon(QtGui.QIcon('Images/Icon.png'))
 
         qr = self.frameGeometry()
         qr.moveCenter(QDesktopWidget().availableGeometry().center())
         self.move(qr.topLeft())
 
     def closeEvent(self, event: QCloseEvent) -> None:
+        ''''''
+
+        event.accept()
         self.__menu.close_about()
 
 
 class ui_menu(QWidget):
+    ''''''
+
     def __init__(self) -> None:
+        ''''''
         super().__init__()
 
         self.setWindowTitle("Harmony decoder - menu")
         self.setGeometry(0, 0, 300, 200)
         self.setWindowIcon(QtGui.QIcon('Images/Icon.png'))
         self.setWindowFlag(Qt.WindowCloseButtonHint, False)
         
@@ -907,39 +1045,52 @@
 
         self.__exit_button.clicked.connect(self.__exit)
         self.__start_button.clicked.connect(self.__run)
         self.__about_button.clicked.connect(self.__show_about)
 
 # public:
     def close_about(self) -> None:
+        ''''''
+
         self.__about = None
 
 # private:
     def __exit(self) -> None:
+        ''''''
+
         self.close()
 
     def __run(self) -> None:
+        ''''''
+
         if self.program is None:
             self.program = ui_program()
             self.program.show()
             self.hide()
         else:
             self.program.close()
             self.program = None
             self.show()
 
     def __show_about(self) -> None:
+        ''''''
+
         if self.__about is None:
             self.__about = ui_about(self)
             self.__about.show()
         else:
             self.__about.close()
             self.__about = None    
 
 
 class app:
+    ''''''
+
     def __init__(self) -> None:
+        ''''''
+
         self.__app:QApplication = QApplication(sys.argv)
         self.__menu:ui_menu = ui_menu()        
 
         self.__menu.show()
         sys.exit(self.__app.exec())
+
```

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/PKG-INFO` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HarmonyDecoder
-Version: 1.0.8
+Version: 1.0.9
 Summary: HarmonyDecoder package
 Author-email: Przemysław Kojs <przemek.kojs@gmail.com>
 Maintainer-email: Przemysław Kojs <przemek.kojs@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `HarmonyDecoder-1.0.8/src/HarmonyDecoder.egg-info/SOURCES.txt` & `HarmonyDecoder-1.0.9/src/HarmonyDecoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

