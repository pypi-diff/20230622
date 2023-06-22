# Comparing `tmp/PyPDFMerge-0.0.1.tar.gz` & `tmp/PyPDFMerge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyPDFMerge-0.0.1.tar", last modified: Thu Jun 22 14:51:00 2023, max compression
+gzip compressed data, was "PyPDFMerge-0.0.2.tar", last modified: Thu Jun 22 14:55:55 2023, max compression
```

## Comparing `PyPDFMerge-0.0.1.tar` & `PyPDFMerge-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 14:51:00.083743 PyPDFMerge-0.0.1/
--rw-rw-rw-   0        0        0     1083 2023-06-22 14:19:56.000000 PyPDFMerge-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2615 2023-06-22 14:51:00.081746 PyPDFMerge-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 14:51:00.075752 PyPDFMerge-0.0.1/PyPDFMerge.egg-info/
--rw-rw-rw-   0        0        0     2615 2023-06-22 14:50:59.000000 PyPDFMerge-0.0.1/PyPDFMerge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-06-22 14:50:59.000000 PyPDFMerge-0.0.1/PyPDFMerge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 14:50:59.000000 PyPDFMerge-0.0.1/PyPDFMerge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-22 14:50:59.000000 PyPDFMerge-0.0.1/PyPDFMerge.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-06-22 14:50:59.000000 PyPDFMerge-0.0.1/PyPDFMerge.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 14:50:59.000000 PyPDFMerge-0.0.1/PyPDFMerge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1398 2023-06-22 14:48:52.000000 PyPDFMerge-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 14:51:00.079744 PyPDFMerge-0.0.1/pdfmerger/
--rw-rw-rw-   0        0        0       26 2023-06-22 06:26:36.000000 PyPDFMerge-0.0.1/pdfmerger/__init__.py
--rw-rw-rw-   0        0        0     8910 2023-06-22 13:59:03.000000 PyPDFMerge-0.0.1/pdfmerger/main.py
--rw-rw-rw-   0        0        0       42 2023-06-22 14:51:00.083743 PyPDFMerge-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1802 2023-06-22 14:47:32.000000 PyPDFMerge-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 14:55:55.211761 PyPDFMerge-0.0.2/
+-rw-rw-rw-   0        0        0     1083 2023-06-22 14:19:56.000000 PyPDFMerge-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2724 2023-06-22 14:55:55.209771 PyPDFMerge-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 14:55:55.203765 PyPDFMerge-0.0.2/PyPDFMerge.egg-info/
+-rw-rw-rw-   0        0        0     2724 2023-06-22 14:55:54.000000 PyPDFMerge-0.0.2/PyPDFMerge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-22 14:55:54.000000 PyPDFMerge-0.0.2/PyPDFMerge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 14:55:54.000000 PyPDFMerge-0.0.2/PyPDFMerge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-06-22 14:55:54.000000 PyPDFMerge-0.0.2/PyPDFMerge.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-06-22 14:55:54.000000 PyPDFMerge-0.0.2/PyPDFMerge.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 14:55:54.000000 PyPDFMerge-0.0.2/PyPDFMerge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1507 2023-06-22 14:54:11.000000 PyPDFMerge-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 14:55:55.207768 PyPDFMerge-0.0.2/pdfmerger/
+-rw-rw-rw-   0        0        0       26 2023-06-22 06:26:36.000000 PyPDFMerge-0.0.2/pdfmerger/__init__.py
+-rw-rw-rw-   0        0        0     8910 2023-06-22 13:59:03.000000 PyPDFMerge-0.0.2/pdfmerger/main.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 14:55:55.211761 PyPDFMerge-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1814 2023-06-22 14:55:05.000000 PyPDFMerge-0.0.2/setup.py
```

### Comparing `PyPDFMerge-0.0.1/LICENSE` & `PyPDFMerge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyPDFMerge-0.0.1/PKG-INFO` & `PyPDFMerge-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFMerge
-Version: 0.0.1
+Version: 0.0.2
 Summary: Merge individual pages of PDF file into one page
 Home-page: https://github.com/shhossain/pdf-merger
 Author: sifat (shhossain)
 Author-email: <hossain@gmail.com>
 Project-URL: Documentation, https://github.com/shhossain/pdf-merger/blob/main/README.md
 Project-URL: Source, https://github.com/shhossain/pdf-merger
 Project-URL: Bug Report, https://github.com/shhossain/pdf-merger/issues
@@ -32,15 +32,15 @@
 
 ## Demo
 
 ### Merging 2 pages into 1
 
 | Before | After |
 |---------|---------|
-| ![Image 1](image.png) | ![Image 2](image-1.png) |
+| ![Image 1](https://raw.githubusercontent.com/shhossain/PyPDFMerge/main/image.png) | ![Image 2](https://github.com/shhossain/PyPDFMerge/raw/main/image-1.png) |
 
 
 ## Installation
 
 ```bash
 pip install PyPDFMerge
 ```
```

### Comparing `PyPDFMerge-0.0.1/PyPDFMerge.egg-info/PKG-INFO` & `PyPDFMerge-0.0.2/PyPDFMerge.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyPDFMerge
-Version: 0.0.1
+Version: 0.0.2
 Summary: Merge individual pages of PDF file into one page
 Home-page: https://github.com/shhossain/pdf-merger
 Author: sifat (shhossain)
 Author-email: <hossain@gmail.com>
 Project-URL: Documentation, https://github.com/shhossain/pdf-merger/blob/main/README.md
 Project-URL: Source, https://github.com/shhossain/pdf-merger
 Project-URL: Bug Report, https://github.com/shhossain/pdf-merger/issues
@@ -32,15 +32,15 @@
 
 ## Demo
 
 ### Merging 2 pages into 1
 
 | Before | After |
 |---------|---------|
-| ![Image 1](image.png) | ![Image 2](image-1.png) |
+| ![Image 1](https://raw.githubusercontent.com/shhossain/PyPDFMerge/main/image.png) | ![Image 2](https://github.com/shhossain/PyPDFMerge/raw/main/image-1.png) |
 
 
 ## Installation
 
 ```bash
 pip install PyPDFMerge
 ```
```

### Comparing `PyPDFMerge-0.0.1/README.md` & `PyPDFMerge-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Demo
 
 ### Merging 2 pages into 1
 
 | Before | After |
 |---------|---------|
-| ![Image 1](image.png) | ![Image 2](image-1.png) |
+| ![Image 1](https://raw.githubusercontent.com/shhossain/PyPDFMerge/main/image.png) | ![Image 2](https://github.com/shhossain/PyPDFMerge/raw/main/image-1.png) |
 
 
 ## Installation
 
 ```bash
 pip install PyPDFMerge
 ```
```

### Comparing `PyPDFMerge-0.0.1/pdfmerger/main.py` & `PyPDFMerge-0.0.2/pdfmerger/main.py`

 * *Files identical despite different names*

### Comparing `PyPDFMerge-0.0.1/setup.py` & `PyPDFMerge-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import find_packages, setup
 
-version = '0.0.1'
-description = 'Merge individual pages of PDF file into one page'
+name = 'PyPDFMerge'
+version = '0.0.2'
+author = 'sifat (shhossain)'
+email = '<hossain@gmail.com>'
+short_description = 'Merge individual pages of PDF file into one page'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
-name = 'PyPDFMerge'
-author = 'sifat (shhossain)'
-email = '<hossain@gmail.com>'
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 keywords = ['pdf-merger', 'pdf']
 
 classifiers = [
@@ -36,15 +36,15 @@
     "Source": "https://github.com/shhossain/pdf-merger",
     "Bug Report": "https://github.com/shhossain/pdf-merger/issues",
 }
 
 setup(
     name=name,
     version=version,
-    description=description,
+    description=short_description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=author,
     author_email=email,
     url=projects_links["Source"],
     project_urls=projects_links,
     packages=find_packages(),
```

