# Comparing `tmp/dvp-common-4.0.5.tar.gz` & `tmp/dvp-common-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvp-common-4.0.5.tar", last modified: Tue Sep 13 07:36:00 2022, max compression
+gzip compressed data, was "dvp-common-4.1.0.tar", last modified: Thu Jun 22 07:57:21 2023, max compression
```

## Comparing `dvp-common-4.0.5.tar` & `dvp-common-4.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.879133 dvp-common-4.0.5/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    11358 2022-09-13 04:50:46.000000 dvp-common-4.0.5/LICENSE
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      134 2022-09-13 04:50:46.000000 dvp-common-4.0.5/MANIFEST.in
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1243 2022-09-13 07:36:00.879319 dvp-common-4.0.5/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      535 2022-09-13 04:50:46.000000 dvp-common-4.0.5/README.md
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      635 2022-09-13 07:36:00.881779 dvp-common-4.0.5/setup.cfg
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      596 2022-09-13 04:50:46.000000 dvp-common-4.0.5/setup.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.805034 dvp-common-4.0.5/src/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.805270 dvp-common-4.0.5/src/main/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.806633 dvp-common-4.0.5/src/main/python/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.818141 dvp-common-4.0.5/src/main/python/dlpx/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      124 2022-09-13 04:50:46.000000 dvp-common-4.0.5/src/main/python/dlpx/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.824071 dvp-common-4.0.5/src/main/python/dlpx/virtualization/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      124 2022-09-13 04:50:46.000000 dvp-common-4.0.5/src/main/python/dlpx/virtualization/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.865473 dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        6 2022-09-13 04:50:46.000000 dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/VERSION
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      196 2022-09-13 04:50:46.000000 dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/__init__.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    13515 2022-09-13 04:50:46.000000 dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/_common_classes.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     7528 2022-09-13 04:50:46.000000 dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/exceptions.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     3403 2022-09-13 04:50:46.000000 dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/util.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:36:00.878617 dvp-common-4.0.5/src/main/python/dvp_common.egg-info/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1243 2022-09-13 07:36:00.000000 dvp-common-4.0.5/src/main/python/dvp_common.egg-info/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      654 2022-09-13 07:36:00.000000 dvp-common-4.0.5/src/main/python/dvp_common.egg-info/SOURCES.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        1 2022-09-13 07:36:00.000000 dvp-common-4.0.5/src/main/python/dvp_common.egg-info/dependency_links.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)       15 2022-09-13 07:36:00.000000 dvp-common-4.0.5/src/main/python/dvp_common.egg-info/requires.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        5 2022-09-13 07:36:00.000000 dvp-common-4.0.5/src/main/python/dvp_common.egg-info/top_level.txt
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.598778 dvp-common-4.1.0/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    11358 2022-09-05 09:36:54.000000 dvp-common-4.1.0/LICENSE
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      134 2022-09-05 09:36:54.000000 dvp-common-4.1.0/MANIFEST.in
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1121 2023-06-22 07:57:21.599248 dvp-common-4.1.0/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      535 2022-09-05 09:36:54.000000 dvp-common-4.1.0/README.md
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      523 2023-06-22 07:57:21.603519 dvp-common-4.1.0/setup.cfg
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      570 2023-06-22 07:09:25.000000 dvp-common-4.1.0/setup.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.586405 dvp-common-4.1.0/src/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.586547 dvp-common-4.1.0/src/main/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.587373 dvp-common-4.1.0/src/main/python/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.590299 dvp-common-4.1.0/src/main/python/dlpx/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      124 2022-09-05 09:36:54.000000 dvp-common-4.1.0/src/main/python/dlpx/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.590994 dvp-common-4.1.0/src/main/python/dlpx/virtualization/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      124 2022-09-05 09:36:54.000000 dvp-common-4.1.0/src/main/python/dlpx/virtualization/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.594692 dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        6 2023-06-22 07:09:25.000000 dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/VERSION
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      196 2022-09-05 09:36:54.000000 dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/__init__.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    13515 2022-09-05 09:36:54.000000 dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/_common_classes.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     7528 2022-09-05 09:36:54.000000 dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/exceptions.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     3403 2022-09-05 09:36:54.000000 dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/util.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:57:21.597917 dvp-common-4.1.0/src/main/python/dvp_common.egg-info/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1121 2023-06-22 07:57:21.000000 dvp-common-4.1.0/src/main/python/dvp_common.egg-info/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      654 2023-06-22 07:57:21.000000 dvp-common-4.1.0/src/main/python/dvp_common.egg-info/SOURCES.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        1 2023-06-22 07:57:21.000000 dvp-common-4.1.0/src/main/python/dvp_common.egg-info/dependency_links.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)       31 2023-06-22 07:57:21.000000 dvp-common-4.1.0/src/main/python/dvp_common.egg-info/requires.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        5 2023-06-22 07:57:21.000000 dvp-common-4.1.0/src/main/python/dvp_common.egg-info/top_level.txt
```

### Comparing `dvp-common-4.0.5/LICENSE` & `dvp-common-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvp-common-4.0.5/PKG-INFO` & `dvp-common-4.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dvp-common
-Version: 4.0.5
+Version: 4.1.0
 Summary: UNKNOWN
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: **Standalone installation of this package is not supported.** Please install the [dvp](https://pypi.org/project/dvp/) package which will install this package.
         
         # Disclaimer
         
         The software is provided “as-is” without any warranties of any kind. To the maximum extent permitted by applicable law, Delphix Corp. and its affiliates disclaim any liability, implied warranties, including, without limitation, any implied warranties of merchantability, fitness for a particular purpose and non-infringement of intellectual property rights.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7, <3.9, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+Requires-Python: >=3.8, <3.9
 Description-Content-Type: text/markdown
```

### Comparing `dvp-common-4.0.5/README.md` & `dvp-common-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dvp-common-4.0.5/setup.cfg` & `dvp-common-4.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 author_email = virtualization-plugins@delphix.com
 home_page = https://developer.delphix.com
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3.8
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
-requires_python = >=2.7, <=3.8, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+requires_python = >=3.8, <3.9
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/_common_classes.py` & `dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/_common_classes.py`

 * *Files identical despite different names*

### Comparing `dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/exceptions.py` & `dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvp-common-4.0.5/src/main/python/dlpx/virtualization/common/util.py` & `dvp-common-4.1.0/src/main/python/dlpx/virtualization/common/util.py`

 * *Files identical despite different names*

### Comparing `dvp-common-4.0.5/src/main/python/dvp_common.egg-info/PKG-INFO` & `dvp-common-4.1.0/src/main/python/dvp_common.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dvp-common
-Version: 4.0.5
+Version: 4.1.0
 Summary: UNKNOWN
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: **Standalone installation of this package is not supported.** Please install the [dvp](https://pypi.org/project/dvp/) package which will install this package.
         
         # Disclaimer
         
         The software is provided “as-is” without any warranties of any kind. To the maximum extent permitted by applicable law, Delphix Corp. and its affiliates disclaim any liability, implied warranties, including, without limitation, any implied warranties of merchantability, fitness for a particular purpose and non-infringement of intellectual property rights.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7, <3.9, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+Requires-Python: >=3.8, <3.9
 Description-Content-Type: text/markdown
```

### Comparing `dvp-common-4.0.5/src/main/python/dvp_common.egg-info/SOURCES.txt` & `dvp-common-4.1.0/src/main/python/dvp_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

