# Comparing `tmp/ocr_iiif_tools-0.0.2.tar.gz` & `tmp/ocr_iiif_tools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_iiif_tools-0.0.2.tar", last modified: Wed Jun 21 22:50:34 2023, max compression
+gzip compressed data, was "ocr_iiif_tools-0.0.3.tar", last modified: Wed Jun 21 23:33:34 2023, max compression
```

## Comparing `ocr_iiif_tools-0.0.2.tar` & `ocr_iiif_tools-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.035881 ocr_iiif_tools-0.0.2/
--rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/LICENSE
--rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 22:50:34.035696 ocr_iiif_tools-0.0.2/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      293 2023-06-21 22:45:36.000000 ocr_iiif_tools-0.0.2/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.032069 ocr_iiif_tools-0.0.2/iida/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/iida/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/iida/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/iida/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.032841 ocr_iiif_tools-0.0.2/ocr_iiif/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/ocr_iiif/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/ocr_iiif/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/ocr_iiif/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.033954 ocr_iiif_tools-0.0.2/ocr_iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/core.py
--rw-r--r--   0 nakamura   (501) staff       (20)    19958 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/pdf.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.035456 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-21 22:50:19.000000 ocr_iiif_tools-0.0.2/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-21 22:50:34.035940 ocr_iiif_tools-0.0.2/setup.cfg
--rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.572753 ocr_iiif_tools-0.0.3/
+-rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/LICENSE
+-rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 23:33:34.572542 ocr_iiif_tools-0.0.3/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      293 2023-06-21 22:45:36.000000 ocr_iiif_tools-0.0.3/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.569126 ocr_iiif_tools-0.0.3/iida/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/iida/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/iida/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/iida/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.569754 ocr_iiif_tools-0.0.3/ocr_iiif/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/ocr_iiif/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/ocr_iiif/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/ocr_iiif/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.570546 ocr_iiif_tools-0.0.3/ocr_iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)    21348 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.572263 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-21 23:33:09.000000 ocr_iiif_tools-0.0.3/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-21 23:33:34.572813 ocr_iiif_tools-0.0.3/setup.cfg
+-rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/setup.py
```

### Comparing `ocr_iiif_tools-0.0.2/LICENSE` & `ocr_iiif_tools-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/PKG-INFO` & `ocr_iiif_tools-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr_iiif_tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.2/iida/_modidx.py` & `ocr_iiif_tools-0.0.3/iida/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/iida/core.py` & `ocr_iiif_tools-0.0.3/iida/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/ocr_iiif/_modidx.py` & `ocr_iiif_tools-0.0.3/ocr_iiif/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/ocr_iiif/core.py` & `ocr_iiif_tools-0.0.3/ocr_iiif/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/ocr_iiif_tools/_modidx.py` & `ocr_iiif_tools-0.0.3/ocr_iiif_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/ocr_iiif_tools/core.py` & `ocr_iiif_tools-0.0.3/ocr_iiif_tools/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/ocr_iiif_tools/pdf.py` & `ocr_iiif_tools-0.0.3/ocr_iiif_tools/pdf.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,14 +154,16 @@
             メインテキストのデフォルトの透明度
         canvas_range : list, optional
             キャンバスの範囲 [start, end]
         font_page_limit : int, optional
             フォントサイズの上限
         task_id : str, optional
             タスクID
+        compress_quality : int, optional
+            圧縮率
         """
         # ... method content ...
 
         '''
         newPdfPage = canvas.Canvas(output_path)
         image_size = (image_width, image_height)
 
@@ -169,15 +171,15 @@
         self._draw_on_canvas(newPdfPage, annotations, image_size, page_size, font_page_limit,
                              default_color, default_alpha, default_main_color, default_main_alpha)
 
         newPdfPage.save()
         '''
         pass
 
-    def convert_iiif2pdf(self, output_path, iiif_manifest_url = None, iiif_manifest_path = None, post_text_size = 5, default_color = "red", default_alpha=0.5, default_main_color = "gray", default_main_alpha = 0.5, canvas_range=None, font_page_limit = 24, task_id = "base"):
+    def convert_iiif2pdf(self, output_path, iiif_manifest_url = None, iiif_manifest_path = None, post_text_size = 0, default_color = "red", default_alpha=0.0, default_main_color = "gray", default_main_alpha = 0.0, canvas_range=None, font_page_limit = 24, task_id = "base", compress_quality = 10):
         """
         IIIFマニフェストをPDFに変換します。
 
         Parameters
         ----------
         output_path : str
             出力するPDFのパス
@@ -197,14 +199,16 @@
             メインテキストのデフォルトの透明度
         canvas_range : list, optional
             キャンバスの範囲 [start, end]
         font_page_limit : int, optional
             フォントサイズの上限
         task_id : str, optional
             タスクID
+        compress_quality : int, optional
+            圧縮率
         """
 
         if iiif_manifest_url is None and iiif_manifest_path is None:
             raise Exception('iiif_manifest_url or iiif_manifest_path must be specified.')
 
         # pass
         newPdfPage = canvas.Canvas(output_path)
@@ -259,29 +263,58 @@
                 page_size['width'], page_size['height'] = landscape(A4)
             else:
                 newPdfPage.setPageSize(A4)
                 page_size['width'], page_size['height'] = A4
 
             # 画像のほうが横に長い
 
-
-
-            newPdfPage.drawImage(img_path,0,0,width=page_size['width'], height=page_size['height'], preserveAspectRatio=True)
-
             p_height = page_size['height'] / image_height
             p_width = page_size['width'] / image_width
 
+            '''
+            print("p_height", p_height)
+            print("p_width", p_width)
+            '''
             
             # 小さい方のスケールを維持する
             scale = min(p_height, p_width)
 
-            offset_page_x = (page_size['width'] - image_width * scale) / 2
-            offset_page_y = (page_size['height'] - image_height * scale) / 2
+            '''
+            image_page_height = image_height * scale
+            image_page_width = image_width * scale
+            
+            print("image_original_height", image_height)
+            print("image_original_width", image_width)
 
+            print("image_page_height", image_page_height)
+            print("image_page_width", image_page_width)
+            '''
+
+            '''
+            im_resized = im.resize((int(image_page_width), int(image_page_height))) # , Image.LANCZOS
+            
+            im_resized_path = img_path + ".resized.jpg"
             
+            im_resized.save(im_resized_path)
+
+            im_webp_path = img_path + ".webp"
+
+            im.save(im_webp_path, optimize=True, quality=comp_q)
+            '''
+
+            im_jpg_path = img_path + ".comp.jpg"
+
+            im.save(im_jpg_path, optimize=True, quality=compress_quality)
+
+            # newPdfPage.drawImage(im_resized_path,0,0,width=page_size['width'], height=page_size['height'], preserveAspectRatio=True)
+            # newPdfPage.drawImage(im_webp_path,0,0,width=page_size['width'], height=page_size['height'], preserveAspectRatio=True)
+            newPdfPage.drawImage(im_jpg_path,0,0,width=page_size['width'], height=page_size['height'], preserveAspectRatio=True)
+
+            offset_page_x = (page_size['width'] - image_width * scale) / 2
+            offset_page_y = (page_size['height'] - image_height * scale) / 2
 
             annotations = iiif_canvas["annotations"][0]["items"]
 
             sorted_annotations = self.sort_annotation(annotations)
 
             prev_group = None
```

### Comparing `ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/PKG-INFO` & `ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-iiif-tools
-Version: 0.0.2
+Version: 0.0.3
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/SOURCES.txt` & `ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.2/settings.ini` & `ocr_iiif_tools-0.0.3/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ocr_iiif_tools
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ocr_iiif_tools
```

### Comparing `ocr_iiif_tools-0.0.2/setup.py` & `ocr_iiif_tools-0.0.3/setup.py`

 * *Files identical despite different names*

