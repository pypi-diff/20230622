# Comparing `tmp/getpaper-0.1.1.tar.gz` & `tmp/getpaper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpaper-0.1.1.tar", last modified: Wed Jun 21 21:32:18 2023, max compression
+gzip compressed data, was "getpaper-0.1.2.tar", last modified: Wed Jun 21 22:08:49 2023, max compression
```

## Comparing `getpaper-0.1.1.tar` & `getpaper-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 21:32:18.718173 getpaper-0.1.1/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.1/LICENSE
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 21:32:18.718173 getpaper-0.1.1/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1976 2023-06-21 14:08:28.000000 getpaper-0.1.1/README.md
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 21:32:18.718173 getpaper-0.1.1/getpaper/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.1/getpaper/__init__.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3997 2023-06-21 14:18:41.000000 getpaper-0.1.1/getpaper/download.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.1/getpaper/index.py
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5473 2023-06-21 21:31:41.000000 getpaper-0.1.1/getpaper/parse.py
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.1/getpaper/splitter.py
-drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 21:32:18.718173 getpaper-0.1.1/getpaper.egg-info/
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 21:32:18.000000 getpaper-0.1.1/getpaper.egg-info/PKG-INFO
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 21:32:18.000000 getpaper-0.1.1/getpaper.egg-info/SOURCES.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 21:32:18.000000 getpaper-0.1.1/getpaper.egg-info/dependency_links.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-21 21:32:18.000000 getpaper-0.1.1/getpaper.egg-info/entry_points.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 21:32:18.000000 getpaper-0.1.1/getpaper.egg-info/requires.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 21:32:18.000000 getpaper-0.1.1/getpaper.egg-info/top_level.txt
--rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 21:32:18.718173 getpaper-0.1.1/setup.cfg
--rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-21 21:31:59.000000 getpaper-0.1.1/setup.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 22:08:49.405064 getpaper-0.1.2/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1072 2023-06-20 19:48:29.000000 getpaper-0.1.2/LICENSE
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 22:08:49.405064 getpaper-0.1.2/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1976 2023-06-21 14:08:28.000000 getpaper-0.1.2/README.md
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 22:08:49.405064 getpaper-0.1.2/getpaper/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-20 20:08:46.000000 getpaper-0.1.2/getpaper/__init__.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     3997 2023-06-21 14:18:41.000000 getpaper-0.1.2/getpaper/download.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     4452 2023-06-21 21:08:34.000000 getpaper-0.1.2/getpaper/index.py
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     5455 2023-06-21 21:39:55.000000 getpaper-0.1.2/getpaper/parse.py
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     1069 2023-06-21 21:08:34.000000 getpaper-0.1.2/getpaper/splitter.py
+drwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)        0 2023-06-21 22:08:49.405064 getpaper-0.1.2/getpaper.egg-info/
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)     2591 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/PKG-INFO
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      319 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/SOURCES.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        1 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/dependency_links.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      105 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/entry_points.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)      190 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/requires.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)        9 2023-06-21 22:08:49.000000 getpaper-0.1.2/getpaper.egg-info/top_level.txt
+-rw-rw-r--   0 antonkulaga  (1000) antonkulaga  (1000)       38 2023-06-21 22:08:49.405064 getpaper-0.1.2/setup.cfg
+-rwxrwxr-x   0 antonkulaga  (1000) antonkulaga  (1000)     1572 2023-06-21 22:08:35.000000 getpaper-0.1.2/setup.py
```

### Comparing `getpaper-0.1.1/LICENSE` & `getpaper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.1/PKG-INFO` & `getpaper-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.1
+Version: 0.1.2
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.1.1/README.md` & `getpaper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.1/getpaper/download.py` & `getpaper-0.1.2/getpaper/download.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.1/getpaper/index.py` & `getpaper-0.1.2/getpaper/index.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.1/getpaper/parse.py` & `getpaper-0.1.2/getpaper/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     """
     Parses the paper using Unstructured paper parser
     :param paper:
     :param folder:
     :param mode: can be single or paged
     :return:
     """
-    bin_file = open(str(paper), "rb", encoding="utf-8")
+    bin_file = open(str(paper), "rb")
     loader = UnstructuredPDFLoader(file_path=None, file = bin_file,  mode=mode,
                                    pdf_infer_table_structure=pdf_infer_table_structure,
                                    strategy = strategy,
                                     include_page_breaks = include_page_breaks)
     where = paper.parent if folder is None else folder
     docs: list[Document] = loader.load()
     if len(docs) ==1:
```

### Comparing `getpaper-0.1.1/getpaper/splitter.py` & `getpaper-0.1.2/getpaper/splitter.py`

 * *Files identical despite different names*

### Comparing `getpaper-0.1.1/getpaper.egg-info/PKG-INFO` & `getpaper-0.1.2/getpaper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getpaper
-Version: 0.1.1
+Version: 0.1.2
 Summary: getpaper - papers download made easy!
 Author: antonkulaga (Anton Kulaga)
 Author-email: <antonkulaga@gmail.com>
 Keywords: python,utils,files,papers,download
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `getpaper-0.1.1/setup.py` & `getpaper-0.1.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'getpaper - papers download made easy!'
 LONG_DESCRIPTION = 'A package with python functions for downloading papers'
 
 # Setting up
 setup(
     name="getpaper",
     version=VERSION,
```

