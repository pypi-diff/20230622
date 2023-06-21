# Comparing `tmp/BroadSword-0.1.tar.gz` & `tmp/BroadSword-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BroadSword-0.1.tar", last modified: Tue Jun  6 17:57:37 2023, max compression
+gzip compressed data, was "BroadSword-0.1.1.tar", last modified: Wed Jun 21 22:49:16 2023, max compression
```

## Comparing `BroadSword-0.1.tar` & `BroadSword-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-06 17:57:16.000000 BroadSword-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 17:57:37.360304 BroadSword-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-06 17:57:16.000000 BroadSword-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-06 17:57:16.000000 BroadSword-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-06 17:57:37.360304 BroadSword-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/BroadSword/
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-06 17:57:16.000000 BroadSword-0.1/src/BroadSword/BroadSword.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:57:16.000000 BroadSword-0.1/src/BroadSword/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 17:57:37.360304 BroadSword-0.1/src/BroadSword.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-06 17:57:37.000000 BroadSword-0.1/src/BroadSword.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.628856 BroadSword-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 22:49:05.000000 BroadSword-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-21 22:49:16.628856 BroadSword-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4914 2023-06-21 22:49:05.000000 BroadSword-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-21 22:49:05.000000 BroadSword-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-21 22:49:16.628856 BroadSword-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.624856 BroadSword-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.624856 BroadSword-0.1.1/src/BroadSword/
+-rw-r--r--   0 runner    (1001) docker     (123)    29345 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/BroadSword.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20584 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/libmatrices.so
+-rw-r--r--   0 runner    (1001) docker     (123)    33748 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/libmatrices_ARM64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)    33320 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/libmatrices_x86_64.dylib
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-21 22:49:05.000000 BroadSword-0.1.1/src/BroadSword/matrices.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:49:16.628856 BroadSword-0.1.1/src/BroadSword.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:49:16.000000 BroadSword-0.1.1/src/BroadSword.egg-info/zip-safe
```

### Comparing `BroadSword-0.1/LICENSE` & `BroadSword-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `BroadSword-0.1/setup.cfg` & `BroadSword-0.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 [metadata]
 name = BroadSword
-version = 0.1
+version = 0.1.1
 author = Cody Somers
 author_email = cas003@usask.ca
 description = Python script to broaden calculated spectra from Wien2k and compare to experimental data at the REIXS Beamline at the Canadian Light Source, Saskatoon, Canada.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Cody-Somers/BroadSword
 project_urls = 
 	Beamline Information = https://reixs.lightsource.ca
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
+zip_safe = True
+include_package_data = True
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 install_requires = 
-	ctypes
 	numpy
 	pandas
 	bokeh>=2.3.3,<3
 
 [options.packages.find]
 where = src
 
+[options.package_data]
+BroadSword = *.so, *.dylib, *.c
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

