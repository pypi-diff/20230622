# Comparing `tmp/ocr_iiif_tools-0.0.1.tar.gz` & `tmp/ocr_iiif_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_iiif_tools-0.0.1.tar", last modified: Tue Jun 20 20:10:38 2023, max compression
+gzip compressed data, was "ocr_iiif_tools-0.0.2.tar", last modified: Wed Jun 21 22:50:34 2023, max compression
```

## Comparing `ocr_iiif_tools-0.0.1.tar` & `ocr_iiif_tools-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 20:10:38.302786 ocr_iiif_tools-0.0.1/
--rw-rw-r--   0 nakamura   (501) staff       (20)    11337 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.1/LICENSE
--rw-rw-r--   0 nakamura   (501) staff       (20)      111 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.1/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-20 20:10:38.302633 ocr_iiif_tools-0.0.1/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      293 2023-06-20 19:40:44.000000 ocr_iiif_tools-0.0.1/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 20:10:38.300214 ocr_iiif_tools-0.0.1/iida/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 20:02:06.000000 ocr_iiif_tools-0.0.1/iida/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-20 20:02:06.000000 ocr_iiif_tools-0.0.1/iida/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-20 20:02:06.000000 ocr_iiif_tools-0.0.1/iida/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 20:10:38.300642 ocr_iiif_tools-0.0.1/ocr_iiif/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 20:09:43.000000 ocr_iiif_tools-0.0.1/ocr_iiif/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-20 20:09:43.000000 ocr_iiif_tools-0.0.1/ocr_iiif/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-20 20:09:43.000000 ocr_iiif_tools-0.0.1/ocr_iiif/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 20:10:38.301092 ocr_iiif_tools-0.0.1/ocr_iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-20 20:10:35.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1301 2023-06-20 20:10:35.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-20 20:10:35.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-20 20:10:38.302406 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-20 20:10:38.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      498 2023-06-20 20:10:38.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 20:10:38.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-20 20:10:38.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-20 20:10:31.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)        7 2023-06-20 20:10:38.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-20 20:10:38.000000 ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      925 2023-06-20 20:10:25.000000 ocr_iiif_tools-0.0.1/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-20 20:10:38.302839 ocr_iiif_tools-0.0.1/setup.cfg
--rw-rw-r--   0 nakamura   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 ocr_iiif_tools-0.0.1/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.035881 ocr_iiif_tools-0.0.2/
+-rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/LICENSE
+-rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 22:50:34.035696 ocr_iiif_tools-0.0.2/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      293 2023-06-21 22:45:36.000000 ocr_iiif_tools-0.0.2/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.032069 ocr_iiif_tools-0.0.2/iida/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/iida/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/iida/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/iida/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.032841 ocr_iiif_tools-0.0.2/ocr_iiif/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/ocr_iiif/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/ocr_iiif/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/ocr_iiif/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.033954 ocr_iiif_tools-0.0.2/ocr_iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)    19958 2023-06-21 22:48:58.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-21 22:50:34.035456 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1064 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-21 22:50:33.000000 ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-21 22:50:19.000000 ocr_iiif_tools-0.0.2/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-21 22:50:34.035940 ocr_iiif_tools-0.0.2/setup.cfg
+-rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.2/setup.py
```

### Comparing `ocr_iiif_tools-0.0.1/LICENSE` & `ocr_iiif_tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.1/PKG-INFO` & `ocr_iiif_tools-0.0.2/ocr_iiif_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocr_iiif_tools
-Version: 0.0.1
+Name: ocr-iiif-tools
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.1/iida/_modidx.py` & `ocr_iiif_tools-0.0.2/iida/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.1/iida/core.py` & `ocr_iiif_tools-0.0.2/iida/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.1/ocr_iiif/_modidx.py` & `ocr_iiif_tools-0.0.2/ocr_iiif/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.1/ocr_iiif/core.py` & `ocr_iiif_tools-0.0.2/ocr_iiif/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.1/ocr_iiif_tools/_modidx.py` & `ocr_iiif_tools-0.0.2/ocr_iiif_tools/_modidx.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,8 +8,25 @@
   'syms': { 'ocr_iiif_tools.core': { 'ocr_iiif_tools.core.Client': ('core.html#client', 'ocr_iiif_tools/core.py'),
                                      'ocr_iiif_tools.core.Client.__init__': ('core.html#client.__init__', 'ocr_iiif_tools/core.py'),
                                      'ocr_iiif_tools.core.Client.create_annotation_list': ( 'core.html#client.create_annotation_list',
                                                                                             'ocr_iiif_tools/core.py'),
                                      'ocr_iiif_tools.core.Client.create_manifest': ( 'core.html#client.create_manifest',
                                                                                      'ocr_iiif_tools/core.py'),
                                      'ocr_iiif_tools.core.Client.get_size': ('core.html#client.get_size', 'ocr_iiif_tools/core.py'),
-                                     'ocr_iiif_tools.core.Client.get_xywh': ('core.html#client.get_xywh', 'ocr_iiif_tools/core.py')}}}
+                                     'ocr_iiif_tools.core.Client.get_xywh': ('core.html#client.get_xywh', 'ocr_iiif_tools/core.py')},
+            'ocr_iiif_tools.pdf': { 'ocr_iiif_tools.pdf.PdfClient': ('pdf.html#pdfclient', 'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.__init__': ('pdf.html#pdfclient.__init__', 'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient._draw_on_canvas': ( 'pdf.html#pdfclient._draw_on_canvas',
+                                                                                      'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient._initialize_canvas': ( 'pdf.html#pdfclient._initialize_canvas',
+                                                                                         'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.convert_iiif2pdf': ( 'pdf.html#pdfclient.convert_iiif2pdf',
+                                                                                       'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.divideByY': ('pdf.html#pdfclient.dividebyy', 'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.getPostText': ('pdf.html#pdfclient.getposttext', 'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.get_color': ('pdf.html#pdfclient.get_color', 'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.get_manifest_json_from_path': ( 'pdf.html#pdfclient.get_manifest_json_from_path',
+                                                                                                  'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.get_manifest_json_from_url': ( 'pdf.html#pdfclient.get_manifest_json_from_url',
+                                                                                                 'ocr_iiif_tools/pdf.py'),
+                                    'ocr_iiif_tools.pdf.PdfClient.sort_annotation': ( 'pdf.html#pdfclient.sort_annotation',
+                                                                                      'ocr_iiif_tools/pdf.py')}}}
```

### Comparing `ocr_iiif_tools-0.0.1/ocr_iiif_tools/core.py` & `ocr_iiif_tools-0.0.2/ocr_iiif_tools/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.1/ocr_iiif_tools.egg-info/PKG-INFO` & `ocr_iiif_tools-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ocr-iiif-tools
-Version: 0.0.1
+Name: ocr_iiif_tools
+Version: 0.0.2
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.1/settings.ini` & `ocr_iiif_tools-0.0.2/settings.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ocr_iiif_tools
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ocr_iiif_tools
@@ -34,10 +34,10 @@
 description = 
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = nakamura196
 
 ### Optional ###
-# requirements = fastcore pandas
+requirements = reportlab requests tqdm
 # dev_requirements = 
 # console_scripts =
```

### Comparing `ocr_iiif_tools-0.0.1/setup.py` & `ocr_iiif_tools-0.0.2/setup.py`

 * *Files identical despite different names*

