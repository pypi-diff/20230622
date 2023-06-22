# Comparing `tmp/comicon-0.3.1.tar.gz` & `tmp/comicon-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comicon-0.3.1.tar", max compression
+gzip compressed data, was "comicon-0.4.0a1.tar", max compression
```

## Comparing `comicon-0.3.1.tar` & `comicon-0.4.0a1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-0.3.1/LICENSE
--rw-r--r--   0        0        0     1605 2023-06-22 00:48:57.443731 comicon-0.3.1/README.md
--rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-0.3.1/comicon/__init__.py
--rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-0.3.1/comicon/api.py
--rw-r--r--   0        0        0     1764 2023-06-21 22:38:57.631788 comicon-0.3.1/comicon/base.py
--rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-0.3.1/comicon/cirtools.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/__init__.py
--rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/cbz.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/cir.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/epub.py
--rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.3.1/comicon/common/pdf.py
--rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-0.3.1/comicon/errors.py
--rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-0.3.1/comicon/inputs/__init__.py
--rw-r--r--   0        0        0     4807 2023-06-21 22:40:25.769680 comicon-0.3.1/comicon/inputs/cbz.py
--rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-0.3.1/comicon/inputs/cir.py
--rw-r--r--   0        0        0     6845 2023-06-21 22:57:31.844781 comicon-0.3.1/comicon/inputs/epub.py
--rw-r--r--   0        0        0     3034 2023-06-21 22:56:41.986407 comicon-0.3.1/comicon/inputs/pdf.py
--rw-r--r--   0        0        0     1905 2023-06-22 00:47:58.838468 comicon-0.3.1/comicon/outputs/__init__.py
--rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-0.3.1/comicon/outputs/cbz.py
--rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-0.3.1/comicon/outputs/cir.py
--rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-0.3.1/comicon/outputs/epub.py
--rw-r--r--   0        0        0     1759 2023-06-22 00:47:44.641646 comicon-0.3.1/comicon/outputs/mobi.py
--rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-0.3.1/comicon/outputs/pdf.py
--rw-r--r--   0        0        0      977 2023-06-22 00:50:27.589598 comicon-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 comicon-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34520 2023-04-28 17:41:58.054636 comicon-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     1752 2023-06-22 01:19:15.083880 comicon-0.4.0a1/README.md
+-rw-r--r--   0        0        0      348 2023-04-28 17:41:58.056636 comicon-0.4.0a1/comicon/__init__.py
+-rw-r--r--   0        0        0      585 2023-06-20 21:51:44.295564 comicon-0.4.0a1/comicon/api.py
+-rw-r--r--   0        0        0     1764 2023-06-21 22:38:57.631788 comicon-0.4.0a1/comicon/base.py
+-rw-r--r--   0        0        0     3391 2023-06-20 21:41:12.912362 comicon-0.4.0a1/comicon/cirtools.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.4.0a1/comicon/common/__init__.py
+-rw-r--r--   0        0        0      410 2023-04-28 17:41:58.063636 comicon-0.4.0a1/comicon/common/cbz.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.4.0a1/comicon/common/cir.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.4.0a1/comicon/common/epub.py
+-rw-r--r--   0        0        0        0 2023-04-28 17:41:58.063636 comicon-0.4.0a1/comicon/common/pdf.py
+-rw-r--r--   0        0        0      673 2023-06-20 21:37:55.976776 comicon-0.4.0a1/comicon/errors.py
+-rw-r--r--   0        0        0     1890 2023-04-28 17:41:58.058636 comicon-0.4.0a1/comicon/inputs/__init__.py
+-rw-r--r--   0        0        0     4807 2023-06-21 22:40:25.769680 comicon-0.4.0a1/comicon/inputs/cbz.py
+-rw-r--r--   0        0        0      631 2023-04-28 17:41:58.057636 comicon-0.4.0a1/comicon/inputs/cir.py
+-rw-r--r--   0        0        0     6845 2023-06-21 22:57:31.844781 comicon-0.4.0a1/comicon/inputs/epub.py
+-rw-r--r--   0        0        0     3034 2023-06-21 22:56:41.986407 comicon-0.4.0a1/comicon/inputs/pdf.py
+-rw-r--r--   0        0        0     1905 2023-06-22 00:47:58.838468 comicon-0.4.0a1/comicon/outputs/__init__.py
+-rw-r--r--   0        0        0     1845 2023-04-28 17:41:58.061636 comicon-0.4.0a1/comicon/outputs/cbz.py
+-rw-r--r--   0        0        0      657 2023-04-28 17:41:58.061636 comicon-0.4.0a1/comicon/outputs/cir.py
+-rw-r--r--   0        0        0     3117 2023-06-20 21:43:52.484820 comicon-0.4.0a1/comicon/outputs/epub.py
+-rw-r--r--   0        0        0     1971 2023-06-22 01:17:24.469271 comicon-0.4.0a1/comicon/outputs/mobi.py
+-rw-r--r--   0        0        0     1891 2023-04-28 17:41:58.062636 comicon-0.4.0a1/comicon/outputs/pdf.py
+-rw-r--r--   0        0        0      979 2023-06-22 01:20:59.819564 comicon-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2630 1970-01-01 00:00:00.000000 comicon-0.4.0a1/PKG-INFO
```

### Comparing `comicon-0.3.1/LICENSE` & `comicon-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/README.md` & `comicon-0.4.0a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import comicon
 
 comicon.convert("comic.cbz", "comic.epub")
 ```
 
 ## Installation
 
+Amazon's **Kindlegen** is required if you want to convert to MOBI. See [here](https://github.com/ciromattia/kcc/issues/371) for more information.
+
 Comicon is available from PyPI:
 
 ```
 pip install comicon
 ```
 
 ## Supported conversions
```

### Comparing `comicon-0.3.1/comicon/api.py` & `comicon-0.4.0a1/comicon/api.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/base.py` & `comicon-0.4.0a1/comicon/base.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/cirtools.py` & `comicon-0.4.0a1/comicon/cirtools.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/errors.py` & `comicon-0.4.0a1/comicon/errors.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/inputs/__init__.py` & `comicon-0.4.0a1/comicon/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/inputs/cbz.py` & `comicon-0.4.0a1/comicon/inputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/inputs/cir.py` & `comicon-0.4.0a1/comicon/inputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/inputs/epub.py` & `comicon-0.4.0a1/comicon/inputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/inputs/pdf.py` & `comicon-0.4.0a1/comicon/inputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/outputs/__init__.py` & `comicon-0.4.0a1/comicon/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/outputs/cbz.py` & `comicon-0.4.0a1/comicon/outputs/cbz.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/outputs/cir.py` & `comicon-0.4.0a1/comicon/outputs/cir.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/outputs/epub.py` & `comicon-0.4.0a1/comicon/outputs/epub.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/comicon/outputs/mobi.py` & `comicon-0.4.0a1/comicon/outputs/mobi.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,20 +5,25 @@
 from . import epub
 
 KINDLEGEN_BIN = "kindlegen"
 
 
 def check_kindlegen() -> None:
     # check if kindlegen is installed
-    kindlegen_return_code = subprocess.run(
-        [KINDLEGEN_BIN, "-locale", "en"],
-        stdout=subprocess.PIPE,
-        stdin=subprocess.PIPE,
-        stderr=subprocess.STDOUT,
-    ).returncode
+    try:
+        kindlegen_return_code = subprocess.run(
+            [KINDLEGEN_BIN, "-locale", "en"],
+            stdout=subprocess.PIPE,
+            stdin=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+        ).returncode
+    except FileNotFoundError as err:
+        raise RuntimeError(
+            "Kindlegen was not found in the current PATH and is required for MOBI conversion."
+        ) from err
 
     if kindlegen_return_code != 0:
         raise RuntimeError(
             f"Kindlegen failed with return code {kindlegen_return_code}. Is Kindlegen installed?"
         )
```

### Comparing `comicon-0.3.1/comicon/outputs/pdf.py` & `comicon-0.4.0a1/comicon/outputs/pdf.py`

 * *Files identical despite different names*

### Comparing `comicon-0.3.1/pyproject.toml` & `comicon-0.4.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "comicon"
-version = "0.3.1"
+version = "0.4.0a1"
 description = "A simple comic conversion library between CBZ/EPUB/MOBI/PDF"
 authors = ["Daniel Chen <danielchen04@hotmail.ca>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 repository = "https://github.com/potatoeggy/comicon"
 documentation = "https://github.com/potatoeggy/comicon"
 keywords = ["converter", "comic", "cbz", "epub", "pdf", "mobi"]
```

### Comparing `comicon-0.3.1/PKG-INFO` & `comicon-0.4.0a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comicon
-Version: 0.3.1
+Version: 0.4.0a1
 Summary: A simple comic conversion library between CBZ/EPUB/MOBI/PDF
 Home-page: https://github.com/potatoeggy/comicon
 License: AGPL-3.0-only
 Keywords: converter,comic,cbz,epub,pdf,mobi
 Author: Daniel Chen
 Author-email: danielchen04@hotmail.ca
 Requires-Python: >=3.10
@@ -32,14 +32,16 @@
 import comicon
 
 comicon.convert("comic.cbz", "comic.epub")
 ```
 
 ## Installation
 
+Amazon's **Kindlegen** is required if you want to convert to MOBI. See [here](https://github.com/ciromattia/kcc/issues/371) for more information.
+
 Comicon is available from PyPI:
 
 ```
 pip install comicon
 ```
 
 ## Supported conversions
```

