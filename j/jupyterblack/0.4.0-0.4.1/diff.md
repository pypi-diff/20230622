# Comparing `tmp/jupyterblack-0.4.0.tar.gz` & `tmp/jupyterblack-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyterblack-0.4.0.tar", last modified: Tue Dec 27 21:17:36 2022, max compression
+gzip compressed data, was "jupyterblack-0.4.1.tar", last modified: Thu Jun 22 16:27:17 2023, max compression
```

## Comparing `jupyterblack-0.4.0.tar` & `jupyterblack-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2022-12-27 21:17:36.645089 jupyterblack-0.4.0/
--rw-r--r--   0 irahorecka   (501) staff       (20)     1068 2021-08-30 23:23:23.000000 jupyterblack-0.4.0/LICENSE
--rw-r--r--   0 irahorecka   (501) staff       (20)     3488 2022-12-27 21:17:36.644763 jupyterblack-0.4.0/PKG-INFO
--rw-r--r--   0 irahorecka   (501) staff       (20)     2591 2022-12-27 20:05:53.000000 jupyterblack-0.4.0/README.md
-drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2022-12-27 21:17:36.639542 jupyterblack-0.4.0/jupyterblack/
--rw-r--r--   0 irahorecka   (501) staff       (20)       60 2022-12-27 21:12:06.000000 jupyterblack-0.4.0/jupyterblack/__init__.py
--rw-r--r--   0 irahorecka   (501) staff       (20)     4118 2022-03-04 17:39:34.000000 jupyterblack-0.4.0/jupyterblack/__main__.py
--rw-r--r--   0 irahorecka   (501) staff       (20)     1446 2021-08-30 23:23:23.000000 jupyterblack-0.4.0/jupyterblack/arguments.py
--rw-r--r--   0 irahorecka   (501) staff       (20)     6925 2022-03-13 00:19:39.000000 jupyterblack-0.4.0/jupyterblack/parser.py
-drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2022-12-27 21:17:36.644126 jupyterblack-0.4.0/jupyterblack/util/
--rw-r--r--   0 irahorecka   (501) staff       (20)        0 2021-08-30 23:23:23.000000 jupyterblack-0.4.0/jupyterblack/util/__init__.py
--rw-r--r--   0 irahorecka   (501) staff       (20)      804 2022-12-27 20:30:35.000000 jupyterblack-0.4.0/jupyterblack/util/error_messages.py
--rw-r--r--   0 irahorecka   (501) staff       (20)     1921 2022-12-27 20:31:05.000000 jupyterblack-0.4.0/jupyterblack/util/files.py
--rw-r--r--   0 irahorecka   (501) staff       (20)       92 2021-08-30 23:23:23.000000 jupyterblack-0.4.0/jupyterblack/util/processing.py
--rw-r--r--   0 irahorecka   (501) staff       (20)      280 2021-08-30 23:23:23.000000 jupyterblack-0.4.0/jupyterblack/util/targets.py
-drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2022-12-27 21:17:36.641737 jupyterblack-0.4.0/jupyterblack.egg-info/
--rw-r--r--   0 irahorecka   (501) staff       (20)     3488 2022-12-27 21:17:36.000000 jupyterblack-0.4.0/jupyterblack.egg-info/PKG-INFO
--rw-r--r--   0 irahorecka   (501) staff       (20)      512 2022-12-27 21:17:36.000000 jupyterblack-0.4.0/jupyterblack.egg-info/SOURCES.txt
--rw-r--r--   0 irahorecka   (501) staff       (20)        1 2022-12-27 21:17:36.000000 jupyterblack-0.4.0/jupyterblack.egg-info/dependency_links.txt
--rw-r--r--   0 irahorecka   (501) staff       (20)       54 2022-12-27 21:17:36.000000 jupyterblack-0.4.0/jupyterblack.egg-info/entry_points.txt
--rw-r--r--   0 irahorecka   (501) staff       (20)       18 2022-12-27 21:17:36.000000 jupyterblack-0.4.0/jupyterblack.egg-info/requires.txt
--rw-r--r--   0 irahorecka   (501) staff       (20)       31 2022-12-27 21:17:36.000000 jupyterblack-0.4.0/jupyterblack.egg-info/top_level.txt
--rw-r--r--   0 irahorecka   (501) staff       (20)      164 2021-08-30 23:23:23.000000 jupyterblack-0.4.0/pyproject.toml
--rw-r--r--   0 irahorecka   (501) staff       (20)       38 2022-12-27 21:17:36.645196 jupyterblack-0.4.0/setup.cfg
--rw-r--r--   0 irahorecka   (501) staff       (20)     1481 2022-12-27 20:05:39.000000 jupyterblack-0.4.0/setup.py
+drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2023-06-22 16:27:17.508433 jupyterblack-0.4.1/
+-rw-r--r--   0 irahorecka   (501) staff       (20)     1068 2021-08-30 23:23:23.000000 jupyterblack-0.4.1/LICENSE
+-rw-r--r--   0 irahorecka   (501) staff       (20)     3500 2023-06-22 16:27:17.508162 jupyterblack-0.4.1/PKG-INFO
+-rw-r--r--   0 irahorecka   (501) staff       (20)     2583 2023-01-02 02:23:50.000000 jupyterblack-0.4.1/README.md
+drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2023-06-22 16:27:17.503277 jupyterblack-0.4.1/jupyterblack/
+-rw-r--r--   0 irahorecka   (501) staff       (20)       60 2023-06-22 16:24:26.000000 jupyterblack-0.4.1/jupyterblack/__init__.py
+-rw-r--r--   0 irahorecka   (501) staff       (20)     4118 2022-03-04 17:39:34.000000 jupyterblack-0.4.1/jupyterblack/__main__.py
+-rw-r--r--   0 irahorecka   (501) staff       (20)     1446 2021-08-30 23:23:23.000000 jupyterblack-0.4.1/jupyterblack/arguments.py
+-rw-r--r--   0 irahorecka   (501) staff       (20)     6925 2022-03-13 00:19:39.000000 jupyterblack-0.4.1/jupyterblack/parser.py
+drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2023-06-22 16:27:17.507739 jupyterblack-0.4.1/jupyterblack/util/
+-rw-r--r--   0 irahorecka   (501) staff       (20)        0 2021-08-30 23:23:23.000000 jupyterblack-0.4.1/jupyterblack/util/__init__.py
+-rw-r--r--   0 irahorecka   (501) staff       (20)      804 2022-12-27 20:30:35.000000 jupyterblack-0.4.1/jupyterblack/util/error_messages.py
+-rw-r--r--   0 irahorecka   (501) staff       (20)     1921 2022-12-27 20:31:05.000000 jupyterblack-0.4.1/jupyterblack/util/files.py
+-rw-r--r--   0 irahorecka   (501) staff       (20)       92 2021-08-30 23:23:23.000000 jupyterblack-0.4.1/jupyterblack/util/processing.py
+-rw-r--r--   0 irahorecka   (501) staff       (20)      280 2021-08-30 23:23:23.000000 jupyterblack-0.4.1/jupyterblack/util/targets.py
+drwxr-xr-x   0 irahorecka   (501) staff       (20)        0 2023-06-22 16:27:17.505991 jupyterblack-0.4.1/jupyterblack.egg-info/
+-rw-r--r--   0 irahorecka   (501) staff       (20)     3500 2023-06-22 16:27:17.000000 jupyterblack-0.4.1/jupyterblack.egg-info/PKG-INFO
+-rw-r--r--   0 irahorecka   (501) staff       (20)      512 2023-06-22 16:27:17.000000 jupyterblack-0.4.1/jupyterblack.egg-info/SOURCES.txt
+-rw-r--r--   0 irahorecka   (501) staff       (20)        1 2023-06-22 16:27:17.000000 jupyterblack-0.4.1/jupyterblack.egg-info/dependency_links.txt
+-rw-r--r--   0 irahorecka   (501) staff       (20)       55 2023-06-22 16:27:17.000000 jupyterblack-0.4.1/jupyterblack.egg-info/entry_points.txt
+-rw-r--r--   0 irahorecka   (501) staff       (20)       36 2023-06-22 16:27:17.000000 jupyterblack-0.4.1/jupyterblack.egg-info/requires.txt
+-rw-r--r--   0 irahorecka   (501) staff       (20)       31 2023-06-22 16:27:17.000000 jupyterblack-0.4.1/jupyterblack.egg-info/top_level.txt
+-rw-r--r--   0 irahorecka   (501) staff       (20)      164 2021-08-30 23:23:23.000000 jupyterblack-0.4.1/pyproject.toml
+-rw-r--r--   0 irahorecka   (501) staff       (20)       38 2023-06-22 16:27:17.508550 jupyterblack-0.4.1/setup.cfg
+-rw-r--r--   0 irahorecka   (501) staff       (20)     1502 2023-06-22 16:24:08.000000 jupyterblack-0.4.1/setup.py
```

### Comparing `jupyterblack-0.4.0/LICENSE` & `jupyterblack-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterblack-0.4.0/PKG-INFO` & `jupyterblack-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jupyterblack
-Version: 0.4.0
+Version: 0.4.1
 Summary: Format code cells in Jupyter Notebook and JupyterLab using black.
 Home-page: https://github.com/irahorecka/jupyterblack
 Author: Ira Horecka
 Author-email: ira89@icloud.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,15 +35,15 @@
 [comment]: <> ([![pyv]&#40;https://img.shields.io/pypi/pyversions/jupyterblack.svg&#41;]&#40;https://pypi.python.org/pypi/jupyterblack&#41;)
 [![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/irahorecka/jupyterblack/master/LICENSE)
 ![CodeSize](https://img.shields.io/github/languages/code-size/irahorecka/jupyterblack)
 
 Format code cells in Jupyter Notebook and JupyterLab using [Black](https://github.com/ambv/black).
 
 <p align="center">
-    <img src="documentation/jupyterblack_demo.gif">
+    <img src="docs/jupyterblack_demo.gif">
 </p>
 
 ## It's as simple as calling jblack
 
 ```bash
 jblack notebook.ipynb
 ```
@@ -88,17 +89,19 @@
                         number of worker processes
   --show-invalid-code
   -t {py27,py33,py34,py35,py36,py37,py38} [{py27,py33,py34,py35,py36,py37,py38} ...], --target-version {py27,py33,py34,py35,py36,py37,py38} [{py27,py33,py34,py35,py36,py37,py38} ...]
 ```
 
 ## Contribute
 
-- [Issue Tracker](https://github.com/irahorecka/jupyterblack/issues)
+- [Issues Tracker](https://github.com/irahorecka/jupyterblack/issues)
 - [Source Code](https://github.com/irahorecka/jupyterblack/tree/master/jupyterblack)
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/jupyterblack/issues).
 
 ## License
 
 The project is licensed under the MIT license.
+
+
```

### Comparing `jupyterblack-0.4.0/README.md` & `jupyterblack-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [comment]: <> ([![pyv]&#40;https://img.shields.io/pypi/pyversions/jupyterblack.svg&#41;]&#40;https://pypi.python.org/pypi/jupyterblack&#41;)
 [![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/irahorecka/jupyterblack/master/LICENSE)
 ![CodeSize](https://img.shields.io/github/languages/code-size/irahorecka/jupyterblack)
 
 Format code cells in Jupyter Notebook and JupyterLab using [Black](https://github.com/ambv/black).
 
 <p align="center">
-    <img src="documentation/jupyterblack_demo.gif">
+    <img src="docs/jupyterblack_demo.gif">
 </p>
 
 ## It's as simple as calling jblack
 
 ```bash
 jblack notebook.ipynb
 ```
@@ -65,15 +65,15 @@
                         number of worker processes
   --show-invalid-code
   -t {py27,py33,py34,py35,py36,py37,py38} [{py27,py33,py34,py35,py36,py37,py38} ...], --target-version {py27,py33,py34,py35,py36,py37,py38} [{py27,py33,py34,py35,py36,py37,py38} ...]
 ```
 
 ## Contribute
 
-- [Issue Tracker](https://github.com/irahorecka/jupyterblack/issues)
+- [Issues Tracker](https://github.com/irahorecka/jupyterblack/issues)
 - [Source Code](https://github.com/irahorecka/jupyterblack/tree/master/jupyterblack)
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/jupyterblack/issues).
 
 ## License
```

### Comparing `jupyterblack-0.4.0/jupyterblack/__main__.py` & `jupyterblack-0.4.1/jupyterblack/__main__.py`

 * *Files identical despite different names*

### Comparing `jupyterblack-0.4.0/jupyterblack/arguments.py` & `jupyterblack-0.4.1/jupyterblack/arguments.py`

 * *Files identical despite different names*

### Comparing `jupyterblack-0.4.0/jupyterblack/parser.py` & `jupyterblack-0.4.1/jupyterblack/parser.py`

 * *Files identical despite different names*

### Comparing `jupyterblack-0.4.0/jupyterblack/util/error_messages.py` & `jupyterblack-0.4.1/jupyterblack/util/error_messages.py`

 * *Files identical despite different names*

### Comparing `jupyterblack-0.4.0/jupyterblack/util/files.py` & `jupyterblack-0.4.1/jupyterblack/util/files.py`

 * *Files identical despite different names*

### Comparing `jupyterblack-0.4.0/jupyterblack.egg-info/PKG-INFO` & `jupyterblack-0.4.1/jupyterblack.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: jupyterblack
-Version: 0.4.0
+Version: 0.4.1
 Summary: Format code cells in Jupyter Notebook and JupyterLab using black.
 Home-page: https://github.com/irahorecka/jupyterblack
 Author: Ira Horecka
 Author-email: ira89@icloud.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -34,15 +35,15 @@
 [comment]: <> ([![pyv]&#40;https://img.shields.io/pypi/pyversions/jupyterblack.svg&#41;]&#40;https://pypi.python.org/pypi/jupyterblack&#41;)
 [![Licence](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/irahorecka/jupyterblack/master/LICENSE)
 ![CodeSize](https://img.shields.io/github/languages/code-size/irahorecka/jupyterblack)
 
 Format code cells in Jupyter Notebook and JupyterLab using [Black](https://github.com/ambv/black).
 
 <p align="center">
-    <img src="documentation/jupyterblack_demo.gif">
+    <img src="docs/jupyterblack_demo.gif">
 </p>
 
 ## It's as simple as calling jblack
 
 ```bash
 jblack notebook.ipynb
 ```
@@ -88,17 +89,19 @@
                         number of worker processes
   --show-invalid-code
   -t {py27,py33,py34,py35,py36,py37,py38} [{py27,py33,py34,py35,py36,py37,py38} ...], --target-version {py27,py33,py34,py35,py36,py37,py38} [{py27,py33,py34,py35,py36,py37,py38} ...]
 ```
 
 ## Contribute
 
-- [Issue Tracker](https://github.com/irahorecka/jupyterblack/issues)
+- [Issues Tracker](https://github.com/irahorecka/jupyterblack/issues)
 - [Source Code](https://github.com/irahorecka/jupyterblack/tree/master/jupyterblack)
 
 ## Support
 
 If you are having issues or would like to propose a new feature, please use the [issues tracker](https://github.com/irahorecka/jupyterblack/issues).
 
 ## License
 
 The project is licensed under the MIT license.
+
+
```

### Comparing `jupyterblack-0.4.0/jupyterblack.egg-info/SOURCES.txt` & `jupyterblack-0.4.1/jupyterblack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupyterblack-0.4.0/setup.py` & `jupyterblack-0.4.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,14 @@
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Intended Audience :: Developers",
     ],
     packages=["jupyterblack", "jupyterblack/util"],
     include_package_data=True,
-    install_requires=["attrs", "black", "safer"],
+    install_requires=["attrs", "black", "safer", "typing_extensions"],
     entry_points={
         "console_scripts": [
             "jblack=jupyterblack.__main__:main",
         ]
     },
 )
```

