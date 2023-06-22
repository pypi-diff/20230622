# Comparing `tmp/Dakada-1.8.3.tar.gz` & `tmp/Dakada-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Dakada-1.8.3.tar", last modified: Wed Jun 21 13:36:55 2023, max compression
+gzip compressed data, was "dist\Dakada-1.8.4.tar", last modified: Thu Jun 22 10:43:53 2023, max compression
```

## Comparing `Dakada-1.8.3.tar` & `Dakada-1.8.4.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 13:36:55.000000 Dakada-1.8.3/
-drwxrwxrwx   0        0        0        0 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/
--rw-rw-rw-   0        0        0      666 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-06-21 13:36:55.000000 Dakada-1.8.3/Dakada.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      666 2023-06-21 13:36:55.000000 Dakada-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-06-21 13:15:08.000000 Dakada-1.8.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 13:36:55.000000 Dakada-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0     3734 2023-06-21 13:36:36.000000 Dakada-1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 10:43:53.000000 Dakada-1.8.4/
+drwxrwxrwx   0        0        0        0 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      678 2023-06-22 10:43:53.000000 Dakada-1.8.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 10:43:53.000000 Dakada-1.8.4/dakada/
+-rw-rw-rw-   0        0        0     8958 2023-06-22 10:43:34.000000 Dakada-1.8.4/dakada/Dakada.py
+-rw-rw-rw-   0        0        0     1194 2023-06-21 12:25:24.000000 Dakada-1.8.4/dakada/User.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 08:03:16.000000 Dakada-1.8.4/dakada/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-06-20 13:19:04.000000 Dakada-1.8.4/dakada/admin.py
+-rw-rw-rw-   0        0        0      547 2023-06-18 08:21:29.000000 Dakada-1.8.4/dakada/cookie.py
+-rw-rw-rw-   0        0        0      497 2023-06-20 12:22:16.000000 Dakada-1.8.4/dakada/render.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 10:43:53.000000 Dakada-1.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     3810 2023-06-22 10:42:48.000000 Dakada-1.8.4/setup.py
```

### Comparing `Dakada-1.8.3/Dakada.egg-info/PKG-INFO` & `Dakada-1.8.4/Dakada.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.8.3
+Version: 1.8.4
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
-Description: 
-        114514
+Description: A web framework by Dakada CN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `Dakada-1.8.3/PKG-INFO` & `Dakada-1.8.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.8.3
+Version: 1.8.4
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
-Description: 
-        114514
+Description: A web framework by Dakada CN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

### Comparing `Dakada-1.8.3/setup.py` & `Dakada-1.8.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import io
 import os
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
-
+print(find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]))
 # Package meta-data.
 NAME = 'Dakada'
 DESCRIPTION = 'A web framework by Dakada CN'
 URL = 'https://github.com/dakadayyds/dakadaWeb'
 EMAIL = 's75uy1e@dingtalk.com'
 AUTHOR = 'dakada'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.8.3'
+VERSION = '1.8.4'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'jinja2'
 ]
 
 # What packages are optional?
@@ -94,21 +94,21 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    py_modules=[
-        'Dakada'
-        'User'
-        'admin'
-        'cookie'
-        'render'
-    ],
+    # packages=[
+    #   'Dakada'
+    #   'User'
+    #   'admin'
+    #    'cookie'
+    #   'render'
+    #],
 
     # entry_points={
     #     'console_scripts': ['mycli=mymodule:cli'],
     # },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
```

