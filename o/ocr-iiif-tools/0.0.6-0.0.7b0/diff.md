# Comparing `tmp/ocr_iiif_tools-0.0.6.tar.gz` & `tmp/ocr_iiif_tools-0.0.7b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocr_iiif_tools-0.0.6.tar", last modified: Thu Jun 22 04:03:56 2023, max compression
+gzip compressed data, was "ocr_iiif_tools-0.0.7b0.tar", last modified: Thu Jun 22 21:33:03 2023, max compression
```

## Comparing `ocr_iiif_tools-0.0.6.tar` & `ocr_iiif_tools-0.0.7b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 04:03:56.088724 ocr_iiif_tools-0.0.6/
--rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/LICENSE
--rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/MANIFEST.in
--rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 04:03:56.088380 ocr_iiif_tools-0.0.6/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      339 2023-06-21 23:57:18.000000 ocr_iiif_tools-0.0.6/README.md
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 04:03:56.081826 ocr_iiif_tools-0.0.6/iida/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/iida/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/iida/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/iida/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 04:03:56.083127 ocr_iiif_tools-0.0.6/ocr_iiif/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/ocr_iiif/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/ocr_iiif/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/ocr_iiif/core.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 04:03:56.084035 ocr_iiif_tools-0.0.6/ocr_iiif_tools/
--rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools/__init__.py
--rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools/_modidx.py
--rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools/core.py
--rw-r--r--   0 nakamura   (501) staff       (20)    22342 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools/pdf.py
-drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 04:03:56.086620 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/
--rw-r--r--   0 nakamura   (501) staff       (20)     1110 2023-06-22 04:03:56.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/PKG-INFO
--rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-22 04:03:56.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/SOURCES.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-22 04:03:56.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/dependency_links.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-22 04:03:56.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/entry_points.txt
--rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/not-zip-safe
--rw-r--r--   0 nakamura   (501) staff       (20)       31 2023-06-22 04:03:56.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/requires.txt
--rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-22 04:03:56.000000 ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/top_level.txt
--rw-r--r--   0 nakamura   (501) staff       (20)      931 2023-06-22 04:03:34.000000 ocr_iiif_tools-0.0.6/settings.ini
--rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-22 04:03:56.088825 ocr_iiif_tools-0.0.6/setup.cfg
--rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.6/setup.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 21:33:03.095660 ocr_iiif_tools-0.0.7b0/
+-rw-r--r--   0 nakamura   (501) staff       (20)    11337 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/LICENSE
+-rw-r--r--   0 nakamura   (501) staff       (20)      111 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/MANIFEST.in
+-rw-r--r--   0 nakamura   (501) staff       (20)     1112 2023-06-22 21:33:03.095484 ocr_iiif_tools-0.0.7b0/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      339 2023-06-21 23:57:18.000000 ocr_iiif_tools-0.0.7b0/README.md
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 21:33:03.091236 ocr_iiif_tools-0.0.7b0/iida/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/iida/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)      912 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/iida/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/iida/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 21:33:03.092274 ocr_iiif_tools-0.0.7b0/ocr_iiif/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     1077 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif/core.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 21:33:03.093723 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/
+-rw-r--r--   0 nakamura   (501) staff       (20)       22 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/__init__.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     3466 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/_modidx.py
+-rw-r--r--   0 nakamura   (501) staff       (20)     5202 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/core.py
+-rw-r--r--   0 nakamura   (501) staff       (20)    22342 2023-06-22 04:03:40.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/pdf.py
+drwxr-xr-x   0 nakamura   (501) staff       (20)        0 2023-06-22 21:33:03.095248 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/
+-rw-r--r--   0 nakamura   (501) staff       (20)     1112 2023-06-22 21:33:03.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/PKG-INFO
+-rw-r--r--   0 nakamura   (501) staff       (20)      520 2023-06-22 21:33:03.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-22 21:33:03.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       71 2023-06-22 21:33:03.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/entry_points.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)        1 2023-06-21 11:50:57.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/not-zip-safe
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-22 21:33:03.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/requires.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)       29 2023-06-22 21:33:03.000000 ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/top_level.txt
+-rw-r--r--   0 nakamura   (501) staff       (20)      943 2023-06-22 21:32:55.000000 ocr_iiif_tools-0.0.7b0/settings.ini
+-rw-r--r--   0 nakamura   (501) staff       (20)       38 2023-06-22 21:33:03.095720 ocr_iiif_tools-0.0.7b0/setup.cfg
+-rw-r--r--   0 nakamura   (501) staff       (20)     2596 2023-06-21 11:48:10.000000 ocr_iiif_tools-0.0.7b0/setup.py
```

### Comparing `ocr_iiif_tools-0.0.6/LICENSE` & `ocr_iiif_tools-0.0.7b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/PKG-INFO` & `ocr_iiif_tools-0.0.7b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr_iiif_tools
-Version: 0.0.6
+Version: 0.0.7b0
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.6/iida/_modidx.py` & `ocr_iiif_tools-0.0.7b0/iida/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/iida/core.py` & `ocr_iiif_tools-0.0.7b0/iida/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/ocr_iiif/_modidx.py` & `ocr_iiif_tools-0.0.7b0/ocr_iiif/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/ocr_iiif/core.py` & `ocr_iiif_tools-0.0.7b0/ocr_iiif/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/ocr_iiif_tools/_modidx.py` & `ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/_modidx.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/ocr_iiif_tools/core.py` & `ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/core.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/ocr_iiif_tools/pdf.py` & `ocr_iiif_tools-0.0.7b0/ocr_iiif_tools/pdf.py`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/PKG-INFO` & `ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocr-iiif-tools
-Version: 0.0.6
+Version: 0.0.7b0
 Summary: UNKNOWN
 Home-page: https://github.com/nakamura196/ocr_iiif_tools
 Author: Satoru
 Author-email: you@example.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `ocr_iiif_tools-0.0.6/ocr_iiif_tools.egg-info/SOURCES.txt` & `ocr_iiif_tools-0.0.7b0/ocr_iiif_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocr_iiif_tools-0.0.6/settings.ini` & `ocr_iiif_tools-0.0.7b0/settings.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ocr_iiif_tools
 lib_name = %(repo)s
-version = 0.0.6
+version = 0.0.7.beta
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
-requirements = reportlab requests tqdm
+requirements = reportlab==3.6.9 requests tqdm
 # dev_requirements = 
 # console_scripts =
```

### Comparing `ocr_iiif_tools-0.0.6/setup.py` & `ocr_iiif_tools-0.0.7b0/setup.py`

 * *Files identical despite different names*

