# Comparing `tmp/dvp-libs-4.0.5.tar.gz` & `tmp/dvp-libs-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvp-libs-4.0.5.tar", last modified: Tue Sep 13 07:38:45 2022, max compression
+gzip compressed data, was "dvp-libs-4.1.0.tar", last modified: Thu Jun 22 07:58:42 2023, max compression
```

## Comparing `dvp-libs-4.0.5.tar` & `dvp-libs-4.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.164723 dvp-libs-4.0.5/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    11358 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/LICENSE
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      132 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/MANIFEST.in
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1275 2022-09-13 07:38:45.164899 dvp-libs-4.0.5/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      535 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/README.md
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      687 2022-09-13 07:38:45.167374 dvp-libs-4.0.5/setup.cfg
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      629 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/setup.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.083630 dvp-libs-4.0.5/src/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.083906 dvp-libs-4.0.5/src/main/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.085368 dvp-libs-4.0.5/src/main/python/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.109265 dvp-libs-4.0.5/src/main/python/dlpx/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      124 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/src/main/python/dlpx/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.115619 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      124 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.154095 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        6 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/VERSION
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      239 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/__init__.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      475 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/_logging.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     2673 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/exceptions.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    21280 2022-09-13 04:50:46.000000 dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/libs.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:38:45.164287 dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1275 2022-09-13 07:38:45.000000 dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      627 2022-09-13 07:38:45.000000 dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/SOURCES.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        1 2022-09-13 07:38:45.000000 dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/dependency_links.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)       33 2022-09-13 07:38:45.000000 dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/requires.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        5 2022-09-13 07:38:45.000000 dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/top_level.txt
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.317137 dvp-libs-4.1.0/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    11358 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/LICENSE
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      132 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/MANIFEST.in
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1153 2023-06-22 07:58:42.317366 dvp-libs-4.1.0/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      535 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/README.md
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      575 2023-06-22 07:58:42.318265 dvp-libs-4.1.0/setup.cfg
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      606 2023-06-22 07:09:25.000000 dvp-libs-4.1.0/setup.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.297454 dvp-libs-4.1.0/src/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.297634 dvp-libs-4.1.0/src/main/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.298593 dvp-libs-4.1.0/src/main/python/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.303074 dvp-libs-4.1.0/src/main/python/dlpx/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      124 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/src/main/python/dlpx/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.304251 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      124 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.312133 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        6 2023-06-22 07:09:25.000000 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/VERSION
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      239 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/__init__.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      475 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/_logging.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     2673 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/exceptions.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    21280 2022-09-05 09:36:54.000000 dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/libs.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:58:42.316625 dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1153 2023-06-22 07:58:42.000000 dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      627 2023-06-22 07:58:42.000000 dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        1 2023-06-22 07:58:42.000000 dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)       49 2023-06-22 07:58:42.000000 dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/requires.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        5 2023-06-22 07:58:42.000000 dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/top_level.txt
```

### Comparing `dvp-libs-4.0.5/LICENSE` & `dvp-libs-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvp-libs-4.0.5/PKG-INFO` & `dvp-libs-4.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dvp-libs
-Version: 4.0.5
+Version: 4.1.0
 Summary: Delphix Virtualization Platform Libraries
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

### Comparing `dvp-libs-4.0.5/README.md` & `dvp-libs-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dvp-libs-4.0.5/setup.cfg` & `dvp-libs-4.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 home_page = https://developer.delphix.com
 summary = Delphix Virtualization Platform Libraries
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

### Comparing `dvp-libs-4.0.5/setup.py` & `dvp-libs-4.1.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 
 PYTHON_SRC = 'src/main/python'
 
 with open(os.path.join(PYTHON_SRC, 'dlpx/virtualization/libs/VERSION')) as version_file:
     version = version_file.read().strip()
 
 install_requires = [
-  "dvp-api == 1.7.0",
-  "dvp-common == {}".format(version)
+    "dvp-api == 1.8.0",
+    "dvp-common == {}".format(version),
+    "six >= 1.16, < 1.17",
 ]
 
 setuptools.setup(name='dvp-libs',
                  version=version,
                  install_requires=install_requires,
                  package_dir={'': PYTHON_SRC},
                  packages=setuptools.find_packages(PYTHON_SRC),
-                 python_requires='>=2.7, <3.9, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*',
-)
+                 python_requires='>=3.8, <3.9',
+                 )
```

### Comparing `dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/exceptions.py` & `dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvp-libs-4.0.5/src/main/python/dlpx/virtualization/libs/libs.py` & `dvp-libs-4.1.0/src/main/python/dlpx/virtualization/libs/libs.py`

 * *Files identical despite different names*

### Comparing `dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/PKG-INFO` & `dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dvp-libs
-Version: 4.0.5
+Version: 4.1.0
 Summary: Delphix Virtualization Platform Libraries
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

### Comparing `dvp-libs-4.0.5/src/main/python/dvp_libs.egg-info/SOURCES.txt` & `dvp-libs-4.1.0/src/main/python/dvp_libs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

