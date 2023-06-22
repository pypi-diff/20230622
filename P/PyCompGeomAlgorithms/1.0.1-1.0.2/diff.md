# Comparing `tmp/PyCompGeomAlgorithms-1.0.1.tar.gz` & `tmp/PyCompGeomAlgorithms-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCompGeomAlgorithms-1.0.1.tar", last modified: Thu Jun 22 19:03:06 2023, max compression
+gzip compressed data, was "PyCompGeomAlgorithms-1.0.2.tar", last modified: Thu Jun 22 19:12:48 2023, max compression
```

## Comparing `PyCompGeomAlgorithms-1.0.1.tar` & `PyCompGeomAlgorithms-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 19:03:06.702077 PyCompGeomAlgorithms-1.0.1/
--rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      568 2023-06-22 19:03:06.704070 PyCompGeomAlgorithms-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 19:03:06.649252 PyCompGeomAlgorithms-1.0.1/PyCompGeomAlgorithms/
-drwxrwxrwx   0        0        0        0 2023-06-22 19:03:06.699087 PyCompGeomAlgorithms-1.0.1/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-22 19:03:06.000000 PyCompGeomAlgorithms-1.0.1/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-22 19:03:06.000000 PyCompGeomAlgorithms-1.0.1/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:03:06.000000 PyCompGeomAlgorithms-1.0.1/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:03:06.000000 PyCompGeomAlgorithms-1.0.1/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.1/README.md
--rw-rw-rw-   0        0        0       84 2023-06-22 11:43:03.000000 PyCompGeomAlgorithms-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      726 2023-06-22 19:03:06.724999 PyCompGeomAlgorithms-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 19:12:48.698697 PyCompGeomAlgorithms-1.0.2/
+-rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      568 2023-06-22 19:12:48.699955 PyCompGeomAlgorithms-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 19:12:48.644660 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/
+drwxrwxrwx   0        0        0        0 2023-06-22 19:12:48.696684 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/
+-rw-rw-rw-   0        0        0      568 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.2/README.md
+-rw-rw-rw-   0        0        0       88 2023-06-22 19:12:11.000000 PyCompGeomAlgorithms-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      726 2023-06-22 19:12:48.704933 PyCompGeomAlgorithms-1.0.2/setup.cfg
```

### Comparing `PyCompGeomAlgorithms-1.0.1/LICENSE` & `PyCompGeomAlgorithms-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.1/PKG-INFO` & `PyCompGeomAlgorithms-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCompGeomAlgorithms
-Version: 1.0.1
+Version: 1.0.2
 Summary: An implementation of computational geometry algorithms in Python3.
 Home-page: https://github.com/PyCompGeom/PyCompGeom-Algorithms
 Author: artandfi (Artem Fisunenko)
 Author-email: artyom.fisunenko@gmail.com
 Keywords: Python3,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PyCompGeomAlgorithms-1.0.1/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/PKG-INFO` & `PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyCompGeomAlgorithms
-Version: 1.0.1
+Version: 1.0.2
 Summary: An implementation of computational geometry algorithms in Python3.
 Home-page: https://github.com/PyCompGeom/PyCompGeom-Algorithms
 Author: artandfi (Artem Fisunenko)
 Author-email: artyom.fisunenko@gmail.com
 Keywords: Python3,computational geometry,convex hull,region search,geometric search,point location,proximity,closest pair,closest points
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `PyCompGeomAlgorithms-1.0.1/README.md` & `PyCompGeomAlgorithms-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.1/setup.cfg` & `PyCompGeomAlgorithms-1.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2050 7943 6f6d 7047 656f 6d41 6c67   = PyCompGeomAlg
 00000020: 6f72 6974 686d 730d 0a76 6572 7369 6f6e  orithms..version
-00000030: 203d 2031 2e30 2e31 0d0a 6175 7468 6f72   = 1.0.1..author
+00000030: 203d 2031 2e30 2e32 0d0a 6175 7468 6f72   = 1.0.2..author
 00000040: 203d 2061 7274 616e 6466 6920 2841 7274   = artandfi (Art
 00000050: 656d 2046 6973 756e 656e 6b6f 290d 0a61  em Fisunenko)..a
 00000060: 7574 686f 725f 656d 6169 6c20 3d20 6172  uthor_email = ar
 00000070: 7479 6f6d 2e66 6973 756e 656e 6b6f 4067  tyom.fisunenko@g
 00000080: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000090: 7074 696f 6e20 3d20 416e 2069 6d70 6c65  ption = An imple
 000000a0: 6d65 6e74 6174 696f 6e20 6f66 2063 6f6d  mentation of com
```

