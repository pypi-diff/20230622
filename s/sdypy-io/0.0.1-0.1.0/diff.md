# Comparing `tmp/sdypy-io-0.0.1.tar.gz` & `tmp/sdypy-io-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdypy-io-0.0.1.tar", last modified: Thu Jun 22 04:37:03 2023, max compression
+gzip compressed data, was "sdypy-io-0.1.0.tar", last modified: Thu Jun 22 07:50:13 2023, max compression
```

## Comparing `sdypy-io-0.0.1.tar` & `sdypy-io-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 04:37:03.148315 sdypy-io-0.0.1/
--rw-rw-rw-   0        0        0     1100 2023-06-22 04:34:38.000000 sdypy-io-0.0.1/License
--rw-rw-rw-   0        0        0     1368 2023-06-22 04:37:03.148315 sdypy-io-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      950 2023-06-22 04:34:38.000000 sdypy-io-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-22 04:37:03.132640 sdypy-io-0.0.1/sdypy/
-drwxrwxrwx   0        0        0        0 2023-06-22 04:37:03.132640 sdypy-io-0.0.1/sdypy/io/
--rw-rw-rw-   0        0        0      113 2023-06-22 04:34:38.000000 sdypy-io-0.0.1/sdypy/io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 04:37:03.148315 sdypy-io-0.0.1/sdypy_io.egg-info/
--rw-rw-rw-   0        0        0     1368 2023-06-22 04:37:03.000000 sdypy-io-0.0.1/sdypy_io.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-06-22 04:37:03.000000 sdypy-io-0.0.1/sdypy_io.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 04:37:03.000000 sdypy-io-0.0.1/sdypy_io.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-22 04:37:03.000000 sdypy-io-0.0.1/sdypy_io.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-22 04:37:03.000000 sdypy-io-0.0.1/sdypy_io.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 04:37:03.148315 sdypy-io-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1488 2023-06-22 04:34:38.000000 sdypy-io-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:50:13.667378 sdypy-io-0.1.0/
+-rw-rw-rw-   0        0        0     1100 2023-06-22 04:34:38.000000 sdypy-io-0.1.0/License
+-rw-rw-rw-   0        0        0     1368 2023-06-22 07:50:13.667378 sdypy-io-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      950 2023-06-22 04:34:38.000000 sdypy-io-0.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-22 07:50:13.627626 sdypy-io-0.1.0/sdypy/
+drwxrwxrwx   0        0        0        0 2023-06-22 07:50:13.633330 sdypy-io-0.1.0/sdypy/io/
+-rw-rw-rw-   0        0        0      122 2023-06-22 07:50:08.000000 sdypy-io-0.1.0/sdypy/io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:50:13.664870 sdypy-io-0.1.0/sdypy_io.egg-info/
+-rw-rw-rw-   0        0        0     1368 2023-06-22 07:50:13.000000 sdypy-io-0.1.0/sdypy_io.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-06-22 07:50:13.000000 sdypy-io-0.1.0/sdypy_io.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:50:13.000000 sdypy-io-0.1.0/sdypy_io.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-22 07:50:13.000000 sdypy-io-0.1.0/sdypy_io.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 07:50:13.000000 sdypy-io-0.1.0/sdypy_io.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:50:13.667378 sdypy-io-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1488 2023-06-22 04:34:38.000000 sdypy-io-0.1.0/setup.py
```

### Comparing `sdypy-io-0.0.1/License` & `sdypy-io-0.1.0/License`

 * *Files identical despite different names*

### Comparing `sdypy-io-0.0.1/PKG-INFO` & `sdypy-io-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdypy-io
-Version: 0.0.1
+Version: 0.1.0
 Summary: Reading and writing of data in structural dynamics.
 Home-page: https://github.com/sdypy/sdypy-io
 Author: Janko Slavič, et al.
 Author-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Keywords: read/write,io,structural dynamics,UFF,UNV,Universal File Format,LVM
 Platform: UNKNOWN
```

### Comparing `sdypy-io-0.0.1/README.rst` & `sdypy-io-0.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `sdypy-io-0.0.1/sdypy_io.egg-info/PKG-INFO` & `sdypy-io-0.1.0/sdypy_io.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdypy-io
-Version: 0.0.1
+Version: 0.1.0
 Summary: Reading and writing of data in structural dynamics.
 Home-page: https://github.com/sdypy/sdypy-io
 Author: Janko Slavič, et al.
 Author-email: janko.slavic@fs.uni-lj.si
 License: UNKNOWN
 Keywords: read/write,io,structural dynamics,UFF,UNV,Universal File Format,LVM
 Platform: UNKNOWN
```

### Comparing `sdypy-io-0.0.1/setup.py` & `sdypy-io-0.1.0/setup.py`

 * *Files identical despite different names*

