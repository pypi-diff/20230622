# Comparing `tmp/sdypy-0.1.0.tar.gz` & `tmp/sdypy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdypy-0.1.0.tar", last modified: Tue Jan 31 10:43:32 2023, max compression
+gzip compressed data, was "sdypy-0.2.0.tar", last modified: Thu Jun 22 07:52:28 2023, max compression
```

## Comparing `sdypy-0.1.0.tar` & `sdypy-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 10:43:32.452417 sdypy-0.1.0/
--rw-rw-rw-   0        0        0     1104 2020-11-16 15:09:15.000000 sdypy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3188 2023-01-31 10:43:32.451424 sdypy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2629 2022-07-13 06:23:47.000000 sdypy-0.1.0/README.rst
--rw-rw-rw-   0        0        0      108 2021-04-16 06:36:51.000000 sdypy-0.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-31 10:43:32.427009 sdypy-0.1.0/sdypy/
--rw-rw-rw-   0        0        0       89 2021-04-16 06:36:51.000000 sdypy-0.1.0/sdypy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 10:43:32.449438 sdypy-0.1.0/sdypy/core/
--rw-rw-rw-   0        0        0       21 2023-01-31 10:41:38.000000 sdypy-0.1.0/sdypy/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-31 10:43:32.448433 sdypy-0.1.0/sdypy.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-01-31 10:43:32.000000 sdypy-0.1.0/sdypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-01-31 10:43:32.000000 sdypy-0.1.0/sdypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 10:43:32.000000 sdypy-0.1.0/sdypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-01-31 10:43:32.000000 sdypy-0.1.0/sdypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-31 10:43:32.000000 sdypy-0.1.0/sdypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 10:43:32.453416 sdypy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1877 2023-01-31 10:40:57.000000 sdypy-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:52:28.740501 sdypy-0.2.0/
+-rw-rw-rw-   0        0        0     1104 2020-11-16 15:09:15.000000 sdypy-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     3396 2023-06-22 07:52:28.740501 sdypy-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2799 2023-06-22 07:52:24.000000 sdypy-0.2.0/README.rst
+-rw-rw-rw-   0        0        0      108 2021-04-16 06:36:51.000000 sdypy-0.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-22 07:52:28.728782 sdypy-0.2.0/sdypy/
+-rw-rw-rw-   0        0        0      111 2023-06-22 07:52:24.000000 sdypy-0.2.0/sdypy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:52:28.740501 sdypy-0.2.0/sdypy/core/
+-rw-rw-rw-   0        0        0       21 2023-06-22 07:52:24.000000 sdypy-0.2.0/sdypy/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:52:28.740501 sdypy-0.2.0/sdypy.egg-info/
+-rw-rw-rw-   0        0        0     3396 2023-06-22 07:52:28.000000 sdypy-0.2.0/sdypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-06-22 07:52:28.000000 sdypy-0.2.0/sdypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:52:28.000000 sdypy-0.2.0/sdypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-22 07:52:28.000000 sdypy-0.2.0/sdypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 07:52:28.000000 sdypy-0.2.0/sdypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:52:28.740501 sdypy-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1930 2023-06-22 07:52:24.000000 sdypy-0.2.0/setup.py
```

### Comparing `sdypy-0.1.0/LICENSE` & `sdypy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdypy-0.1.0/PKG-INFO` & `sdypy-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sdypy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Structural Dynamics Python.
 Home-page: https://github.com/sdypy/sdypy
 Author: Janko Slavič, Domen Gorjup, Klemen Zaletelj
 Author-email: janko.slavic@fs.uni-lj.si
 Maintainer: Janko Slavič, Domen Gorjup, Klemen Zaletelj
 Maintainer-email: janko.slavic@fs.uni-lj.si
 License: MIT license
 Keywords: sdypy
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 SDyPy - Structural Dynamics Python
 ----------------------------------
 
 This package has the goal to defragment the open source effort in the scientific field 
 of structural dynamics. Our goal is to speed-up the development and implementation of scientific
@@ -46,18 +47,19 @@
 Package integration in SDyPy
 ----------------------------
 
 The existing efforts in the field of structural dynamics are included in SDyPy according to
 the level of integration (see `SEP 1 <https://github.com/sdypy/sdypy/blob/main/docs/seps/sep-0001.rst>`_).
 
 - **1st level** (part of SDyPy repository or organization):
-    - *No packages are currently at 1st level*
+    - `sdypy-EMA <https://github.com/sdypy/sdypy-EMA>`_ (Experimental Modal Analysis in Python)
+    - `sdypy-io <https://github.com/sdypy/sdypy-io>`_ (Input/Output for Structural Dynamics)
 
 - **2nd level** (namespace package in independent repository):
-   - `pyEMA <https://github.com/ladisk/pyEMA>`_ (Experimental Modal Analysis in Python)
+   - `pyEMA <https://github.com/ladisk/pyEMA>`_ (Experimental Modal Analysis in Python) - **No longer developed.**
    
 - **3rd level** (packages that correspond to the SDyPy template):
    - `pyExSi <https://github.com/ladisk/pyExSi>`_ (Excitation signal generator)
    - `FLife <https://github.com/ladisk/FLife>`_ (Vibration fatigue life in the spectral domain)
    - `pyIDI <https://github.com/ladisk/pyidi>`_ (Image-Based Displacement Identification)
    
 - **4th level** (these packages are developed completely independently but might be useful for 3rd, 2nd and 1st level packages):
```

### Comparing `sdypy-0.1.0/README.rst` & `sdypy-0.2.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -29,18 +29,19 @@
 Package integration in SDyPy
 ----------------------------
 
 The existing efforts in the field of structural dynamics are included in SDyPy according to
 the level of integration (see `SEP 1 <https://github.com/sdypy/sdypy/blob/main/docs/seps/sep-0001.rst>`_).
 
 - **1st level** (part of SDyPy repository or organization):
-    - *No packages are currently at 1st level*
+    - `sdypy-EMA <https://github.com/sdypy/sdypy-EMA>`_ (Experimental Modal Analysis in Python)
+    - `sdypy-io <https://github.com/sdypy/sdypy-io>`_ (Input/Output for Structural Dynamics)
 
 - **2nd level** (namespace package in independent repository):
-   - `pyEMA <https://github.com/ladisk/pyEMA>`_ (Experimental Modal Analysis in Python)
+   - `pyEMA <https://github.com/ladisk/pyEMA>`_ (Experimental Modal Analysis in Python) - **No longer developed.**
    
 - **3rd level** (packages that correspond to the SDyPy template):
    - `pyExSi <https://github.com/ladisk/pyExSi>`_ (Excitation signal generator)
    - `FLife <https://github.com/ladisk/FLife>`_ (Vibration fatigue life in the spectral domain)
    - `pyIDI <https://github.com/ladisk/pyidi>`_ (Image-Based Displacement Identification)
    
 - **4th level** (these packages are developed completely independently but might be useful for 3rd, 2nd and 1st level packages):
```

### Comparing `sdypy-0.1.0/sdypy.egg-info/PKG-INFO` & `sdypy-0.2.0/sdypy.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: sdypy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Structural Dynamics Python.
 Home-page: https://github.com/sdypy/sdypy
 Author: Janko Slavič, Domen Gorjup, Klemen Zaletelj
 Author-email: janko.slavic@fs.uni-lj.si
 Maintainer: Janko Slavič, Domen Gorjup, Klemen Zaletelj
 Maintainer-email: janko.slavic@fs.uni-lj.si
 License: MIT license
 Keywords: sdypy
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 SDyPy - Structural Dynamics Python
 ----------------------------------
 
 This package has the goal to defragment the open source effort in the scientific field 
 of structural dynamics. Our goal is to speed-up the development and implementation of scientific
@@ -46,18 +47,19 @@
 Package integration in SDyPy
 ----------------------------
 
 The existing efforts in the field of structural dynamics are included in SDyPy according to
 the level of integration (see `SEP 1 <https://github.com/sdypy/sdypy/blob/main/docs/seps/sep-0001.rst>`_).
 
 - **1st level** (part of SDyPy repository or organization):
-    - *No packages are currently at 1st level*
+    - `sdypy-EMA <https://github.com/sdypy/sdypy-EMA>`_ (Experimental Modal Analysis in Python)
+    - `sdypy-io <https://github.com/sdypy/sdypy-io>`_ (Input/Output for Structural Dynamics)
 
 - **2nd level** (namespace package in independent repository):
-   - `pyEMA <https://github.com/ladisk/pyEMA>`_ (Experimental Modal Analysis in Python)
+   - `pyEMA <https://github.com/ladisk/pyEMA>`_ (Experimental Modal Analysis in Python) - **No longer developed.**
    
 - **3rd level** (packages that correspond to the SDyPy template):
    - `pyExSi <https://github.com/ladisk/pyExSi>`_ (Excitation signal generator)
    - `FLife <https://github.com/ladisk/FLife>`_ (Vibration fatigue life in the spectral domain)
    - `pyIDI <https://github.com/ladisk/pyidi>`_ (Image-Based Displacement Identification)
    
 - **4th level** (these packages are developed completely independently but might be useful for 3rd, 2nd and 1st level packages):
```

### Comparing `sdypy-0.1.0/setup.py` & `sdypy-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 requirements = parse_requirements('requirements.txt')
 
 if __name__ == '__main__':
     setup(
         name='sdypy',
         description='Structural Dynamics Python.',
         long_description=readme,
+        long_description_content_type='text/x-rst',
         license='MIT license',
         url='https://github.com/sdypy/sdypy',
         version=version,
         author='Janko Slavič, Domen Gorjup, Klemen Zaletelj',
         author_email='janko.slavic@fs.uni-lj.si',
         maintainer='Janko Slavič, Domen Gorjup, Klemen Zaletelj',
         maintainer_email='janko.slavic@fs.uni-lj.si',
```

