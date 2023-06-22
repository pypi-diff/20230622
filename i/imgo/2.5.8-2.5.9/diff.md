# Comparing `tmp/imgo-2.5.8.tar.gz` & `tmp/imgo-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgo-2.5.8.tar", last modified: Wed Jun 21 07:19:34 2023, max compression
+gzip compressed data, was "dist/imgo-2.5.9.tar", last modified: Thu Jun 22 14:56:50 2023, max compression
```

## Comparing `imgo-2.5.8.tar` & `imgo-2.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-21 07:19:34.459475 imgo-2.5.8/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1066 2020-10-24 16:50:48.000000 imgo-2.5.8/LICENSE.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)     2998 2023-06-21 07:19:34.458897 imgo-2.5.8/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)     2550 2023-06-20 16:09:32.000000 imgo-2.5.8/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-21 07:19:34.453230 imgo-2.5.8/imgo/
--rw-r--r--   0 lucbatty   (501) staff       (20)        0 2020-09-26 14:01:11.000000 imgo-2.5.8/imgo/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    49895 2023-06-20 09:27:56.000000 imgo-2.5.8/imgo/augtools.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    87279 2023-06-20 09:27:57.000000 imgo-2.5.8/imgo/uptools.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-21 07:19:34.457899 imgo-2.5.8/imgo.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)     2998 2023-06-21 07:19:34.000000 imgo-2.5.8/imgo.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      207 2023-06-21 07:19:34.000000 imgo-2.5.8/imgo.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-21 07:19:34.000000 imgo-2.5.8/imgo.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        5 2023-06-21 07:19:34.000000 imgo-2.5.8/imgo.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      226 2020-10-23 14:05:03.000000 imgo-2.5.8/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-21 07:19:34.459710 imgo-2.5.8/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      652 2023-06-21 07:17:56.000000 imgo-2.5.8/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 14:56:50.000000 imgo-2.5.9/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1066 2020-10-24 16:50:48.000000 imgo-2.5.9/LICENSE.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2948 2023-06-22 14:56:50.000000 imgo-2.5.9/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2550 2023-06-20 16:09:32.000000 imgo-2.5.9/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 14:56:50.000000 imgo-2.5.9/imgo/
+-rw-r--r--   0 lucbatty   (501) staff       (20)        0 2020-09-26 14:01:11.000000 imgo-2.5.9/imgo/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    49895 2023-06-20 09:27:56.000000 imgo-2.5.9/imgo/augtools.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    87279 2023-06-20 09:27:57.000000 imgo-2.5.9/imgo/uptools.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 14:56:50.000000 imgo-2.5.9/imgo.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     2948 2023-06-22 14:56:50.000000 imgo-2.5.9/imgo.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      207 2023-06-22 14:56:50.000000 imgo-2.5.9/imgo.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-22 14:56:50.000000 imgo-2.5.9/imgo.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        5 2023-06-22 14:56:50.000000 imgo-2.5.9/imgo.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      226 2020-10-23 14:05:03.000000 imgo-2.5.9/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-22 14:56:50.000000 imgo-2.5.9/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      603 2023-06-22 14:56:27.000000 imgo-2.5.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `imgo-2.5.8/LICENSE.txt` & `imgo-2.5.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `imgo-2.5.8/PKG-INFO` & `imgo-2.5.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: imgo
-Version: 2.5.8
+Version: 2.5.9
 Summary: Image Dataset Management Toolkit
 Home-page: https://github.com/celerygemini/imgo
 Author: celerygemini
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # imgo
 
 ## Process, Augment, and Balance Image Data
```

### Comparing `imgo-2.5.8/README.md` & `imgo-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `imgo-2.5.8/imgo/augtools.py` & `imgo-2.5.9/imgo/augtools.py`

 * *Files identical despite different names*

### Comparing `imgo-2.5.8/imgo/uptools.py` & `imgo-2.5.9/imgo/uptools.py`

 * *Files identical despite different names*

### Comparing `imgo-2.5.8/imgo.egg-info/PKG-INFO` & `imgo-2.5.9/imgo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: imgo
-Version: 2.5.8
+Version: 2.5.9
 Summary: Image Dataset Management Toolkit
 Home-page: https://github.com/celerygemini/imgo
 Author: celerygemini
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # imgo
 
 ## Process, Augment, and Balance Image Data
```

### Comparing `imgo-2.5.8/setup.py` & `imgo-2.5.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="imgo",
-    version="2.5.8",
+    version="2.5.9",
     author="celerygemini",
     description="Image Dataset Management Toolkit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/celerygemini/imgo",
     packages=setuptools.find_packages(),
     classifiers=[
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

