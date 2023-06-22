# Comparing `tmp/dvp-4.0.5.tar.gz` & `tmp/dvp-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvp-4.0.5.tar", last modified: Tue Sep 13 07:41:52 2022, max compression
+gzip compressed data, was "dvp-4.1.0.tar", last modified: Thu Jun 22 07:58:17 2023, max compression
```

## Comparing `dvp-4.0.5.tar` & `dvp-4.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:41:52.724501 dvp-4.0.5/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    11358 2022-09-13 04:50:46.000000 dvp-4.0.5/LICENSE
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      126 2022-09-13 04:50:46.000000 dvp-4.0.5/MANIFEST.in
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1396 2022-09-13 07:41:52.724661 dvp-4.0.5/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      725 2022-09-13 04:50:46.000000 dvp-4.0.5/README.md
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      594 2022-09-13 07:41:52.743625 dvp-4.0.5/setup.cfg
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      638 2022-09-13 04:50:46.000000 dvp-4.0.5/setup.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:41:52.685301 dvp-4.0.5/src/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:41:52.685586 dvp-4.0.5/src/main/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:41:52.686558 dvp-4.0.5/src/main/python/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:41:52.704997 dvp-4.0.5/src/main/python/dlpx/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      123 2022-09-13 04:50:46.000000 dvp-4.0.5/src/main/python/dlpx/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:41:52.712902 dvp-4.0.5/src/main/python/dlpx/virtualization/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        6 2022-09-13 04:50:46.000000 dvp-4.0.5/src/main/python/dlpx/virtualization/VERSION
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      123 2022-09-13 04:50:46.000000 dvp-4.0.5/src/main/python/dlpx/virtualization/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:41:52.724090 dvp-4.0.5/src/main/python/dvp.egg-info/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1396 2022-09-13 07:41:52.000000 dvp-4.0.5/src/main/python/dvp.egg-info/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      387 2022-09-13 07:41:52.000000 dvp-4.0.5/src/main/python/dvp.egg-info/SOURCES.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        1 2022-09-13 07:41:52.000000 dvp-4.0.5/src/main/python/dvp.egg-info/dependency_links.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)       71 2022-09-13 07:41:52.000000 dvp-4.0.5/src/main/python/dvp.egg-info/requires.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        5 2022-09-13 07:41:52.000000 dvp-4.0.5/src/main/python/dvp.egg-info/top_level.txt
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:17.633733 dvp-4.1.0/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    11358 2022-09-05 09:36:54.000000 dvp-4.1.0/LICENSE
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      126 2022-09-05 09:36:54.000000 dvp-4.1.0/MANIFEST.in
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1396 2023-06-22 07:58:17.634003 dvp-4.1.0/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      725 2022-09-05 09:36:54.000000 dvp-4.1.0/README.md
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      594 2023-06-22 07:58:17.634894 dvp-4.1.0/setup.cfg
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      663 2023-06-22 07:09:25.000000 dvp-4.1.0/setup.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:17.616584 dvp-4.1.0/src/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:17.616797 dvp-4.1.0/src/main/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:17.617611 dvp-4.1.0/src/main/python/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:17.626159 dvp-4.1.0/src/main/python/dlpx/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      123 2022-09-05 09:36:54.000000 dvp-4.1.0/src/main/python/dlpx/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:17.628667 dvp-4.1.0/src/main/python/dlpx/virtualization/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        6 2023-06-22 07:09:25.000000 dvp-4.1.0/src/main/python/dlpx/virtualization/VERSION
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      123 2022-09-05 09:36:54.000000 dvp-4.1.0/src/main/python/dlpx/virtualization/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:17.632839 dvp-4.1.0/src/main/python/dvp.egg-info/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1396 2023-06-22 07:58:17.000000 dvp-4.1.0/src/main/python/dvp.egg-info/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      387 2023-06-22 07:58:17.000000 dvp-4.1.0/src/main/python/dvp.egg-info/SOURCES.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        1 2023-06-22 07:58:17.000000 dvp-4.1.0/src/main/python/dvp.egg-info/dependency_links.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)       71 2023-06-22 07:58:17.000000 dvp-4.1.0/src/main/python/dvp.egg-info/requires.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        5 2023-06-22 07:58:17.000000 dvp-4.1.0/src/main/python/dvp.egg-info/top_level.txt
```

### Comparing `dvp-4.0.5/LICENSE` & `dvp-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvp-4.0.5/PKG-INFO` & `dvp-4.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvp
-Version: 4.0.5
+Version: 4.1.0
 Summary: Delphix Virtualization Platform SDK
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: The Delphix Virtualization SDK helps developers build plugins to ingest and provision data on top of the Delphix platform. For more information please refer to the [documentation](https://developer.delphix.com/).
```

### Comparing `dvp-4.0.5/README.md` & `dvp-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dvp-4.0.5/setup.cfg` & `dvp-4.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvp-4.0.5/setup.py` & `dvp-4.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 PYTHON_SRC = 'src/main/python'
 
 with open(os.path.join(PYTHON_SRC, 'dlpx/virtualization/VERSION')) as version_file:
     version = version_file.read().strip()
 
 install_requires = [
-  "dvp-common == {}".format(version),
-  "dvp-libs == {}".format(version),
-  "dvp-platform == {}".format(version),
-  "dvp-tools == {}".format(version)
+    "dvp-common == {}".format(version),
+    "dvp-libs == {}".format(version),
+    "dvp-platform == {}".format(version),
+    "dvp-tools == {}".format(version)
 ]
 
 setuptools.setup(name='dvp',
                  version=version,
                  install_requires=install_requires,
                  package_dir={'': PYTHON_SRC},
                  packages=setuptools.find_packages(PYTHON_SRC),
                  python_requires='>=3.8, <3.9',
-)
+                 )
```

### Comparing `dvp-4.0.5/src/main/python/dvp.egg-info/PKG-INFO` & `dvp-4.1.0/src/main/python/dvp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvp
-Version: 4.0.5
+Version: 4.1.0
 Summary: Delphix Virtualization Platform SDK
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: The Delphix Virtualization SDK helps developers build plugins to ingest and provision data on top of the Delphix platform. For more information please refer to the [documentation](https://developer.delphix.com/).
```

