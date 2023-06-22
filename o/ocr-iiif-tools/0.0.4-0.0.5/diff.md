# Comparing `tmp/ocr_iiif_tools-0.0.4.tar.gz` & `tmp/ocr_iiif_tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_iiif_tools-0.0.4.tar", last modified: Thu Jun 22 03:09:34 2023, max compression
+gzip compressed data, was "ocr_iiif_tools-0.0.5.tar", last modified: Thu Jun 22 03:53:24 2023, max compression
```

## Comparing `ocr_iiif_tools-0.0.4.tar` & `ocr_iiif_tools-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.124160 ocr_iiif_tools-0.0.4/
--rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/LICENSE
--rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 03:09:34.123989 ocr_iiif_tools-0.0.4/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      339 2023-06-21 23:57:18.000000 ocr_iiif_tools-0.0.4/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.120134 ocr_iiif_tools-0.0.4/iida/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/iida/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/iida/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/iida/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.121147 ocr_iiif_tools-0.0.4/ocr_iiif/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/ocr_iiif/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/ocr_iiif/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/ocr_iiif/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.122151 ocr_iiif_tools-0.0.4/ocr_iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/core.py
--rw-r--r--   0 nakamura   (501) staff       (20)    21598 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/pdf.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.123744 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-22 03:08:41.000000 ocr_iiif_tools-0.0.4/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-22 03:09:34.124214 ocr_iiif_tools-0.0.4/setup.cfg
--rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:53:24.272733 ocr_iiif_tools-0.0.5/
+-rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/LICENSE
+-rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 03:53:24.272555 ocr_iiif_tools-0.0.5/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      339 2023-06-21 23:57:18.000000 ocr_iiif_tools-0.0.5/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:53:24.268233 ocr_iiif_tools-0.0.5/iida/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/iida/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/iida/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/iida/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:53:24.269084 ocr_iiif_tools-0.0.5/ocr_iiif/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/ocr_iiif/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/ocr_iiif/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/ocr_iiif/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:53:24.270244 ocr_iiif_tools-0.0.5/ocr_iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-22 03:52:33.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-22 03:52:33.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-22 03:52:33.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)    22336 2023-06-22 03:52:33.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:53:24.272286 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 03:53:24.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-22 03:53:24.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-22 03:53:24.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-22 03:53:24.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-22 03:53:24.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-22 03:53:24.000000 ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-22 03:53:19.000000 ocr_iiif_tools-0.0.5/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-22 03:53:24.272794 ocr_iiif_tools-0.0.5/setup.cfg
+-rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.5/setup.py
```

### Comparing `ocr_iiif_tools-0.0.4/LICENSE` & `ocr_iiif_tools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/PKG-INFO` & `ocr_iiif_tools-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr_iiif_tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.4/iida/_modidx.py` & `ocr_iiif_tools-0.0.5/iida/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/iida/core.py` & `ocr_iiif_tools-0.0.5/iida/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/ocr_iiif/_modidx.py` & `ocr_iiif_tools-0.0.5/ocr_iiif/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/ocr_iiif/core.py` & `ocr_iiif_tools-0.0.5/ocr_iiif/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/ocr_iiif_tools/_modidx.py` & `ocr_iiif_tools-0.0.5/ocr_iiif_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/ocr_iiif_tools/core.py` & `ocr_iiif_tools-0.0.5/ocr_iiif_tools/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/ocr_iiif_tools/pdf.py` & `ocr_iiif_tools-0.0.5/ocr_iiif_tools/pdf.py`

 * *Files 3% similar despite different names*

```diff
@@ -248,15 +248,34 @@
             if not os.path.exists(img_path):
                 os.makedirs(os.path.dirname(img_path), exist_ok=True)
                 df = requests.get(image_url).content
                 open(img_path, "wb").write(df)
 
             # fliped_img_path = img_path + ".fliped.jpg"
             im = Image.open(img_path)
-            image_width, image_height = im.size
+            image_original_width, image_original_height = im.size
+            image_width = image_original_width
+            image_height = image_original_height
+
+            canvas_width = iiif_canvas["width"]
+            canvas_height = iiif_canvas["height"]
+
+            '''
+            print("image_width", image_width)
+            print("image_height", image_height)
+
+            print("canvas_width", canvas_width)
+            print("canvas_height", canvas_height)
+
+            print("----")
+            '''
+
+            # 
+            image_width = canvas_width
+            image_height = canvas_height
 
             # ページサイズ
             page_size = {}
 
             ratio = image_width / image_height
 
 
@@ -274,14 +293,15 @@
 
             p_height = page_size['height'] / image_height
             p_width = page_size['width'] / image_width
 
             '''
             print("p_height", p_height)
             print("p_width", p_width)
+            
             '''
             
             # 小さい方のスケールを維持する
             scale = min(p_height, p_width)
 
             '''
             image_page_height = image_height * scale
@@ -302,17 +322,20 @@
             im_resized.save(im_resized_path)
 
             im_webp_path = img_path + ".webp"
 
             im.save(im_webp_path, optimize=True, quality=comp_q)
             '''
 
-            im_jpg_path = img_path + ".comp.jpg"
-
-            im.save(im_jpg_path, optimize=True, quality=compress_quality)
+            # 画像が大きい場合は圧縮する
+            if image_original_height > 1024:
+                im_jpg_path = img_path + "_comp.jpg"
+                im.save(im_jpg_path, optimize=True, quality=compress_quality)
+            else:
+                im_jpg_path = img_path
 
             # newPdfPage.drawImage(im_resized_path,0,0,width=page_size['width'], height=page_size['height'], preserveAspectRatio=True)
             # newPdfPage.drawImage(im_webp_path,0,0,width=page_size['width'], height=page_size['height'], preserveAspectRatio=True)
             newPdfPage.drawImage(im_jpg_path,0,0,width=page_size['width'], height=page_size['height'], preserveAspectRatio=True)
 
             offset_page_x = (page_size['width'] - image_width * scale) / 2
             offset_page_y = (page_size['height'] - image_height * scale) / 2
```

### Comparing `ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/PKG-INFO` & `ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-iiif-tools
-Version: 0.0.4
+Version: 0.0.5
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/SOURCES.txt` & `ocr_iiif_tools-0.0.5/ocr_iiif_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.4/settings.ini` & `ocr_iiif_tools-0.0.5/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ocr_iiif_tools
 lib_name = %(repo)s
-version = 0.0.4
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ocr_iiif_tools
```

### Comparing `ocr_iiif_tools-0.0.4/setup.py` & `ocr_iiif_tools-0.0.5/setup.py`

 * *Files identical despite different names*

