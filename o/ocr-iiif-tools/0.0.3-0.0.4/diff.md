# Comparing `tmp/ocr_iiif_tools-0.0.3.tar.gz` & `tmp/ocr_iiif_tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_iiif_tools-0.0.3.tar", last modified: Wed Jun 21 23:33:34 2023, max compression
+gzip compressed data, was "ocr_iiif_tools-0.0.4.tar", last modified: Thu Jun 22 03:09:34 2023, max compression
```

## Comparing `ocr_iiif_tools-0.0.3.tar` & `ocr_iiif_tools-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.572753 ocr_iiif_tools-0.0.3/
--rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/LICENSE
--rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 23:33:34.572542 ocr_iiif_tools-0.0.3/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      293 2023-06-21 22:45:36.000000 ocr_iiif_tools-0.0.3/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.569126 ocr_iiif_tools-0.0.3/iida/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/iida/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/iida/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/iida/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.569754 ocr_iiif_tools-0.0.3/ocr_iiif/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/ocr_iiif/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/ocr_iiif/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/ocr_iiif/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.570546 ocr_iiif_tools-0.0.3/ocr_iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/core.py
--rw-r--r--   0 nakamura   (501) staff       (20)    21348 2023-06-21 23:32:49.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools/pdf.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 23:33:34.572263 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-21 23:33:34.000000 ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-21 23:33:09.000000 ocr_iiif_tools-0.0.3/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-21 23:33:34.572813 ocr_iiif_tools-0.0.3/setup.cfg
--rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.3/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.124160 ocr_iiif_tools-0.0.4/
+-rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/LICENSE
+-rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 03:09:34.123989 ocr_iiif_tools-0.0.4/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      339 2023-06-21 23:57:18.000000 ocr_iiif_tools-0.0.4/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.120134 ocr_iiif_tools-0.0.4/iida/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/iida/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/iida/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/iida/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.121147 ocr_iiif_tools-0.0.4/ocr_iiif/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/ocr_iiif/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/ocr_iiif/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/ocr_iiif/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.122151 ocr_iiif_tools-0.0.4/ocr_iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)    21598 2023-06-22 03:08:47.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 03:09:34.123744 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-22 03:09:34.000000 ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-22 03:08:41.000000 ocr_iiif_tools-0.0.4/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-22 03:09:34.124214 ocr_iiif_tools-0.0.4/setup.cfg
+-rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.4/setup.py
```

### Comparing `ocr_iiif_tools-0.0.3/LICENSE` & `ocr_iiif_tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/PKG-INFO` & `ocr_iiif_tools-0.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr_iiif_tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -17,26 +17,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-iida
+IIIFとOCRを組み合わせたツール
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
 
 ``` sh
-pip install iida
+pip install ocr_iiif_tools
 ```
 
 ## How to use
 
 Fill me in please! Don’t forget code examples:
 
 ``` python
```

### Comparing `ocr_iiif_tools-0.0.3/iida/_modidx.py` & `ocr_iiif_tools-0.0.4/iida/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/iida/core.py` & `ocr_iiif_tools-0.0.4/iida/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/ocr_iiif/_modidx.py` & `ocr_iiif_tools-0.0.4/ocr_iiif/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/ocr_iiif/core.py` & `ocr_iiif_tools-0.0.4/ocr_iiif/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/ocr_iiif_tools/_modidx.py` & `ocr_iiif_tools-0.0.4/ocr_iiif_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/ocr_iiif_tools/core.py` & `ocr_iiif_tools-0.0.4/ocr_iiif_tools/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/ocr_iiif_tools/pdf.py` & `ocr_iiif_tools-0.0.4/ocr_iiif_tools/pdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,15 +171,15 @@
         self._draw_on_canvas(newPdfPage, annotations, image_size, page_size, font_page_limit,
                              default_color, default_alpha, default_main_color, default_main_alpha)
 
         newPdfPage.save()
         '''
         pass
 
-    def convert_iiif2pdf(self, output_path, iiif_manifest_url = None, iiif_manifest_path = None, post_text_size = 0, default_color = "red", default_alpha=0.0, default_main_color = "gray", default_main_alpha = 0.0, canvas_range=None, font_page_limit = 24, task_id = "base", compress_quality = 10):
+    def convert_iiif2pdf(self, output_path, iiif_manifest_url = None, iiif_manifest_path = None, post_text_size = 0, default_color = "red", default_alpha=0.0, default_main_color = "gray", default_main_alpha = 0.0, canvas_range=None, font_page_limit = 24, task_id = "base", compress_quality = 10, image_download_dir = None):
         """
         IIIFマニフェストをPDFに変換します。
 
         Parameters
         ----------
         output_path : str
             出力するPDFのパス
@@ -229,20 +229,25 @@
             raise Exception("Not supported context")
         
         canvases = manifest_json["items"]
 
         if canvas_range is not None:
             canvases = canvases[canvas_range[0]:canvas_range[1]]
 
-        for iiif_canvas in tqdm(canvases):
-            image_url = iiif_canvas["items"][0]["items"][0]["body"]["id"]
+        # for iiif_canvas in tqdm(canvases):
+        for i in range(len(canvases)):
+            iiif_canvas = canvases[i]
 
-            image_hash = hashlib.md5(image_url.encode()).hexdigest()
+            image_url = iiif_canvas["items"][0]["items"][0]["body"]["id"]
 
-            img_path = f"{self.tmp_dir}/{task_id}/images/{image_hash}.jpg"
+            if image_download_dir is None:
+                image_hash = hashlib.md5(image_url.encode()).hexdigest()
+                img_path = f"{self.tmp_dir}/{task_id}/images/{image_hash}.jpg"
+            else:
+                img_path = f"{image_download_dir}/{str(i+1).zfill(4)}.jpg"
 
             if not os.path.exists(img_path):
                 os.makedirs(os.path.dirname(img_path), exist_ok=True)
                 df = requests.get(image_url).content
                 open(img_path, "wb").write(df)
 
             # fliped_img_path = img_path + ".fliped.jpg"
```

### Comparing `ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/PKG-INFO` & `ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-iiif-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
@@ -17,26 +17,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-iida
+IIIFとOCRを組み合わせたツール
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
 
 ``` sh
-pip install iida
+pip install ocr_iiif_tools
 ```
 
 ## How to use
 
 Fill me in please! Don’t forget code examples:
 
 ``` python
```

### Comparing `ocr_iiif_tools-0.0.3/ocr_iiif_tools.egg-info/SOURCES.txt` & `ocr_iiif_tools-0.0.4/ocr_iiif_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.3/settings.ini` & `ocr_iiif_tools-0.0.4/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ocr_iiif_tools
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ocr_iiif_tools
```

### Comparing `ocr_iiif_tools-0.0.3/setup.py` & `ocr_iiif_tools-0.0.4/setup.py`

 * *Files identical despite different names*

