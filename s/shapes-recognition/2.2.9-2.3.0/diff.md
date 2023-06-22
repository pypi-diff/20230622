# Comparing `tmp/shapes_recognition-2.2.9.tar.gz` & `tmp/shapes_recognition-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapes_recognition-2.2.9.tar", last modified: Thu Jun 22 10:26:56 2023, max compression
+gzip compressed data, was "shapes_recognition-2.3.0.tar", last modified: Thu Jun 22 11:00:55 2023, max compression
```

## Comparing `shapes_recognition-2.2.9.tar` & `shapes_recognition-2.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 10:26:56.220794 shapes_recognition-2.2.9/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-22 10:26:56.220540 shapes_recognition-2.2.9/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.2.9/README.md
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-22 10:26:56.220878 shapes_recognition-2.2.9/setup.cfg
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-22 10:22:43.000000 shapes_recognition-2.2.9/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 10:26:56.218394 shapes_recognition-2.2.9/shapes_recognition/
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 10:26:56.220165 shapes_recognition-2.2.9/shapes_recognition/pure_cython/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      301 2022-12-10 15:57:51.000000 shapes_recognition-2.2.9/shapes_recognition/pure_cython/setup.py
-drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 10:26:56.219888 shapes_recognition-2.2.9/shapes_recognition.egg-info/
--rw-r--r--   0 boriskravtsov   (501) staff       (20)     1155 2023-06-22 10:26:56.000000 shapes_recognition-2.2.9/shapes_recognition.egg-info/PKG-INFO
--rw-r--r--   0 boriskravtsov   (501) staff       (20)      226 2023-06-22 10:26:56.000000 shapes_recognition-2.2.9/shapes_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-22 10:26:56.000000 shapes_recognition-2.2.9/shapes_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-22 10:26:56.000000 shapes_recognition-2.2.9/shapes_recognition.egg-info/top_level.txt
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 11:00:55.586699 shapes_recognition-2.3.0/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1175 2023-06-22 11:00:55.586460 shapes_recognition-2.3.0/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      606 2023-02-16 10:59:45.000000 shapes_recognition-2.3.0/README.md
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       38 2023-06-22 11:00:55.586777 shapes_recognition-2.3.0/setup.cfg
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1198 2023-06-22 10:58:58.000000 shapes_recognition-2.3.0/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 11:00:55.584414 shapes_recognition-2.3.0/shapes_recognition/
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 11:00:55.586102 shapes_recognition-2.3.0/shapes_recognition/pure_cython/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      301 2022-12-10 15:57:51.000000 shapes_recognition-2.3.0/shapes_recognition/pure_cython/setup.py
+drwxr-xr-x   0 boriskravtsov   (501) staff       (20)        0 2023-06-22 11:00:55.585842 shapes_recognition-2.3.0/shapes_recognition.egg-info/
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)     1175 2023-06-22 11:00:55.000000 shapes_recognition-2.3.0/shapes_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)      226 2023-06-22 11:00:55.000000 shapes_recognition-2.3.0/shapes_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)        1 2023-06-22 11:00:55.000000 shapes_recognition-2.3.0/shapes_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 boriskravtsov   (501) staff       (20)       19 2023-06-22 11:00:55.000000 shapes_recognition-2.3.0/shapes_recognition.egg-info/top_level.txt
```

### Comparing `shapes_recognition-2.2.9/PKG-INFO` & `shapes_recognition-2.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: shapes_recognition
-Version: 2.2.9
+Version: 2.3.0
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
@@ -26,7 +27,9 @@
 
 <p align="center"><img src="https://boriskravtsov.com/pypi/shapes.png"/>
 
 To simulate such recognition capability, we introduce the **shapes_recognition** library.
 
 [Here](https://kravtsov-development.medium.com/amazing-ai-tables-44af52c993a2) 
 we show how to use it. 
+
+
```

### Comparing `shapes_recognition-2.2.9/README.md` & `shapes_recognition-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shapes_recognition-2.2.9/setup.py` & `shapes_recognition-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="shapes_recognition",
-    version="2.2.9",
+    version="2.3.0",
     description="New Shape Matching Technology",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://boriskravtsov.com/",
     author="Boris Kravtsov",
     author_email="boriskravtsov.contacts@gmail.com",
     license="MIT",
```

### Comparing `shapes_recognition-2.2.9/shapes_recognition.egg-info/PKG-INFO` & `shapes_recognition-2.3.0/shapes_recognition.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: shapes-recognition
-Version: 2.2.9
+Version: 2.3.0
 Summary: New Shape Matching Technology
 Home-page: https://boriskravtsov.com/
 Author: Boris Kravtsov
 Author-email: boriskravtsov.contacts@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: MacOS :: MacOS X
 Description-Content-Type: text/markdown
@@ -26,7 +27,9 @@
 
 <p align="center"><img src="https://boriskravtsov.com/pypi/shapes.png"/>
 
 To simulate such recognition capability, we introduce the **shapes_recognition** library.
 
 [Here](https://kravtsov-development.medium.com/amazing-ai-tables-44af52c993a2) 
 we show how to use it. 
+
+
```

