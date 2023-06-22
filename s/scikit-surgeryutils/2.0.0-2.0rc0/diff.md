# Comparing `tmp/scikit-surgeryutils-2.0.0.tar.gz` & `tmp/scikit-surgeryutils-2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-surgeryutils-2.0.0.tar", last modified: Thu Jun 22 19:55:19 2023, max compression
+gzip compressed data, was "scikit-surgeryutils-2.0rc0.tar", last modified: Thu Mar 23 16:27:26 2023, max compression
```

## Comparing `scikit-surgeryutils-2.0.0.tar` & `scikit-surgeryutils-2.0rc0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:55:19.921947 scikit-surgeryutils-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-22 19:55:19.921947 scikit-surgeryutils-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:55:19.917947 scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-06-22 19:55:19.000000 scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-22 19:55:19.000000 scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:55:19.000000 scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-22 19:55:19.000000 scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 19:55:19.000000 scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 19:55:19.000000 scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-22 19:55:19.921947 scikit-surgeryutils-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:55:19.921947 scikit-surgeryutils-2.0.0/sksurgeryutils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 19:55:19.921947 scikit-surgeryutils-2.0.0/sksurgeryutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/common_overlay_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:55:19.921947 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerycharucotest_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerycharucotest_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerymakecalibrationdots_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerymakecalibrationdots_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryreslice_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryreslice_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytextoverlay_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytextoverlay_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytransformpolydata_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytransformpolydata_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibration_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibration_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideolag_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideolag_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:55:19.921947 scikit-surgeryutils-2.0.0/sksurgeryutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/utils/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/utils/opencv_video_capture_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-22 19:55:10.000000 scikit-surgeryutils-2.0.0/sksurgeryutils/utils/screen_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-22 19:55:11.000000 scikit-surgeryutils-2.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:27:26.658490 scikit-surgeryutils-2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-03-23 16:27:26.658490 scikit-surgeryutils-2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:27:26.654490 scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-03-23 16:27:26.000000 scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-03-23 16:27:26.000000 scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 16:27:26.000000 scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-23 16:27:26.000000 scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-23 16:27:26.000000 scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-23 16:27:26.000000 scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-23 16:27:26.658490 scikit-surgeryutils-2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:27:26.658490 scikit-surgeryutils-2.0rc0/sksurgeryutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-03-23 16:27:26.658490 scikit-surgeryutils-2.0rc0/sksurgeryutils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/common_overlay_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:27:26.658490 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerycharucotest_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerycharucotest_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerymakecalibrationdots_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerymakecalibrationdots_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryreslice_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryreslice_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytextoverlay_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytextoverlay_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytransformpolydata_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytransformpolydata_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibration_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibration_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideolag_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideolag_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 16:27:26.658490 scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/opencv_video_capture_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/screen_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-03-23 16:27:17.000000 scikit-surgeryutils-2.0rc0/versioneer.py
```

### Comparing `scikit-surgeryutils-2.0.0/LICENSE` & `scikit-surgeryutils-2.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/PKG-INFO` & `scikit-surgeryutils-2.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgeryutils
-Version: 2.0.0
+Version: 2.0rc0
 Summary: scikit-surgeryutils - Tests/demos utilities, based around opencv-contrib-python-headless and PySide6
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryutils
 Author: Matt Clarkson
 Author-email: m.clarkson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryutils 
         ===============================
@@ -32,16 +32,16 @@
         .. image:: https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg
            :target: CODE_OF_CONDUCT.md
         
         .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
            :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
            :alt: Follow scikit_surgery on twitter
         
-        Author(s): Miguel Xochicale, Thomas Dowrick, Stephen Thompson and Matt Clarkson;
-        Contributor(s): Mian Ahmad.
+        Author(s): Stephen Thompson and Matt Clarkson;
+        Contributor(s): Miguel Xochicale, Thomas Dowrick, and Mian Ahmad.
         
         scikit-surgeryutils containing small demo apps and utilities.
         
         scikit-surgeryutils is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
         
         scikit-surgeryvtk is tested on Python 3.8. and may support other Python versions.
         
@@ -93,16 +93,14 @@
         
         You can run the unit tests by installing and running tox:
         
         ::
         
             pip install tox
             tox
-            tox -e docs
-            tox -e lint
         
         
         Encountering Problems?
         ^^^^^^^^^^^^^^^^^^^^^^
         Please get in touch or raise an `issue`_.
         
         Contributing
@@ -137,20 +135,21 @@
         .. _`SciKit-Surgery`: https://github.com/SciKit-Surgery/
         .. _`University College London (UCL)`: http://www.ucl.ac.uk/
         .. _`Wellcome`: https://wellcome.ac.uk/
         .. _`EPSRC`: https://www.epsrc.ac.uk/
         .. _`contributing guidelines`: https://github.com/SciKit-Surgery/scikit-surgeryutils/blob/master/CONTRIBUTING.rst
         .. _`license file`: https://github.com/SciKit-Surgery/scikit-surgeryutils/blob/master/LICENSE
         .. _`issue`: https://github.com/SciKit-Surgery/scikit-surgeryutils/issues/new
+        
 Keywords: medical imaging
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Description-Content-Type: text/x-rst
```

### Comparing `scikit-surgeryutils-2.0.0/README.rst` & `scikit-surgeryutils-2.0rc0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 .. image:: https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg
    :target: CODE_OF_CONDUCT.md
 
 .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
    :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
    :alt: Follow scikit_surgery on twitter
 
-Author(s): Miguel Xochicale, Thomas Dowrick, Stephen Thompson and Matt Clarkson;
-Contributor(s): Mian Ahmad.
+Author(s): Stephen Thompson and Matt Clarkson;
+Contributor(s): Miguel Xochicale, Thomas Dowrick, and Mian Ahmad.
 
 scikit-surgeryutils containing small demo apps and utilities.
 
 scikit-surgeryutils is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
 
 scikit-surgeryvtk is tested on Python 3.8. and may support other Python versions.
 
@@ -85,16 +85,14 @@
 
 You can run the unit tests by installing and running tox:
 
 ::
 
     pip install tox
     tox
-    tox -e docs
-    tox -e lint
 
 
 Encountering Problems?
 ^^^^^^^^^^^^^^^^^^^^^^
 Please get in touch or raise an `issue`_.
 
 Contributing
@@ -128,8 +126,8 @@
 .. _`Documentation`: https://scikit-surgeryutils.readthedocs.io
 .. _`SciKit-Surgery`: https://github.com/SciKit-Surgery/
 .. _`University College London (UCL)`: http://www.ucl.ac.uk/
 .. _`Wellcome`: https://wellcome.ac.uk/
 .. _`EPSRC`: https://www.epsrc.ac.uk/
 .. _`contributing guidelines`: https://github.com/SciKit-Surgery/scikit-surgeryutils/blob/master/CONTRIBUTING.rst
 .. _`license file`: https://github.com/SciKit-Surgery/scikit-surgeryutils/blob/master/LICENSE
-.. _`issue`: https://github.com/SciKit-Surgery/scikit-surgeryutils/issues/new
+.. _`issue`: https://github.com/SciKit-Surgery/scikit-surgeryutils/issues/new
```

### Comparing `scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/PKG-INFO` & `scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-surgeryutils
-Version: 2.0.0
+Version: 2.0rc0
 Summary: scikit-surgeryutils - Tests/demos utilities, based around opencv-contrib-python-headless and PySide6
 Home-page: https://github.com/SciKit-Surgery/scikit-surgeryutils
 Author: Matt Clarkson
 Author-email: m.clarkson@ucl.ac.uk
 License: BSD-3 license
 Description: scikit-surgeryutils 
         ===============================
@@ -32,16 +32,16 @@
         .. image:: https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg
            :target: CODE_OF_CONDUCT.md
         
         .. image:: https://img.shields.io/twitter/follow/scikit_surgery?style=social
            :target: https://twitter.com/scikit_surgery?ref_src=twsrc%5Etfw
            :alt: Follow scikit_surgery on twitter
         
-        Author(s): Miguel Xochicale, Thomas Dowrick, Stephen Thompson and Matt Clarkson;
-        Contributor(s): Mian Ahmad.
+        Author(s): Stephen Thompson and Matt Clarkson;
+        Contributor(s): Miguel Xochicale, Thomas Dowrick, and Mian Ahmad.
         
         scikit-surgeryutils containing small demo apps and utilities.
         
         scikit-surgeryutils is part of the `SciKit-Surgery`_ software project, developed at the `Wellcome EPSRC Centre for Interventional and Surgical Sciences`_, part of `University College London (UCL)`_.
         
         scikit-surgeryvtk is tested on Python 3.8. and may support other Python versions.
         
@@ -93,16 +93,14 @@
         
         You can run the unit tests by installing and running tox:
         
         ::
         
             pip install tox
             tox
-            tox -e docs
-            tox -e lint
         
         
         Encountering Problems?
         ^^^^^^^^^^^^^^^^^^^^^^
         Please get in touch or raise an `issue`_.
         
         Contributing
@@ -137,20 +135,21 @@
         .. _`SciKit-Surgery`: https://github.com/SciKit-Surgery/
         .. _`University College London (UCL)`: http://www.ucl.ac.uk/
         .. _`Wellcome`: https://wellcome.ac.uk/
         .. _`EPSRC`: https://www.epsrc.ac.uk/
         .. _`contributing guidelines`: https://github.com/SciKit-Surgery/scikit-surgeryutils/blob/master/CONTRIBUTING.rst
         .. _`license file`: https://github.com/SciKit-Surgery/scikit-surgeryutils/blob/master/LICENSE
         .. _`issue`: https://github.com/SciKit-Surgery/scikit-surgeryutils/issues/new
+        
 Keywords: medical imaging
 Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Description-Content-Type: text/x-rst
```

### Comparing `scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/SOURCES.txt` & `scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/scikit_surgeryutils.egg-info/entry_points.txt` & `scikit-surgeryutils-2.0rc0/scikit_surgeryutils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/setup.py` & `scikit-surgeryutils-2.0rc0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,27 +18,27 @@
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/SciKit-Surgery/scikit-surgeryutils',
     author='Matt Clarkson',
     author_email='m.clarkson@ucl.ac.uk',
     license='BSD-3 license',
     classifiers=[
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 4 - Beta',
 
         'Intended Audience :: Developers',
         'Intended Audience :: Healthcare Industry',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Science/Research',
 
 
         'License :: OSI Approved :: BSD License',
 
 
         'Programming Language :: Python',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3',
 
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Scientific/Engineering :: Medical Science Apps.',
     ],
 
     keywords='medical imaging',
 
@@ -48,20 +48,20 @@
             'tests',
         ]
     ),
 
     install_requires=[
         'six>=1.10',
         'numpy>=1.11',
-        'PySide6>=6.5.1.1',
         'opencv-contrib-python-headless>=4.2.0.32',
+        'pyside6>=6.4.2',
         'scikit-surgerycore>=0.1.7',
         'scikit-surgeryimage>=0.10.1',
-        'scikit-surgeryvtk>=2.0.1',
-        'scikit-surgeryarucotracker',
+        'scikit-surgeryvtk==2.0rc0',
+        'scikit-surgeryarucotracker>=0.2.7',
         'scikit-surgerycalibration>=0.2.1'
     ],
 
     entry_points={
         'console_scripts': [
             'sksurgeryvideolag=sksurgeryutils.ui.sksurgeryvideolag_command_line:main',
             'sksurgerycharucotest=sksurgeryutils.ui.sksurgerycharucotest_command_line:main',
```

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/common_overlay_apps.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/common_overlay_apps.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         self.layout.setSpacing(0)
 
         if platform.system() == 'Linux':
             init_vtk_widget = False
         else:
             init_vtk_widget = True
 
-        self.vtk_overlay_window = VTKOverlayWindow(offscreen=False,
-                                                   init_widget=init_vtk_widget)
+        self.vtk_overlay_window = VTKOverlayWindow(init_widget=init_vtk_widget)
         self.layout.addWidget(self.vtk_overlay_window)
 
         self.video_source = TimestampedVideoSource(video_source, dims)
 
         self.timer = QTimer()
         self.timer.timeout.connect(self.update_view)
 
@@ -97,16 +96,16 @@
         Get the next frame of input and display it.
         """
         _bool_retrieve, self.img = self.video_source.read()
         self.vtk_overlay_window.set_video_image(self.img)
         self.vtk_overlay_window.Render()
 
         if platform.system() == 'Linux':
-            self.vtk_overlay_window.Initialize() #Allows the interactor to initialize itself. # pylint: disable=line-too-long
-            self.vtk_overlay_window.Start() #Start the event loop. # pylint: disable=line-too-long
+            self.vtk_overlay_window.Initialize()
+
 
 class OverlayOnVideoFeedCropRecord(OverlayBaseWidget):
     """ Add cropping of the incoming video feed, and the ability to
         record the vtk_overlay_window.
 
        :param video_source: OpenCV compatible video source (int or filename)
        :param output_filename: Location of output video file when recording.
```

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerycharucotest_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerycharucotest_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerycharucotest_demo.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerycharucotest_demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerymakecalibrationdots_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerymakecalibrationdots_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerymakecalibrationdots_demo.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerymakecalibrationdots_demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_demo.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryrendermodelslikecamera_demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryreslice_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryreslice_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryreslice_demo.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryreslice_demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytextoverlay_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytextoverlay_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytextoverlay_demo.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytextoverlay_demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytransformpolydata_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytransformpolydata_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgerytransformpolydata_demo.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgerytransformpolydata_demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibration_app.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibration_app.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibration_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibration_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_app.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_app.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideocalibrationchecker_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideolag_command_line.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideolag_command_line.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/ui/sksurgeryvideolag_demo.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/ui/sksurgeryvideolag_demo.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/utils/image_utils.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/utils/opencv_video_capture_utils.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/opencv_video_capture_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/sksurgeryutils/utils/screen_utils.py` & `scikit-surgeryutils-2.0rc0/sksurgeryutils/utils/screen_utils.py`

 * *Files identical despite different names*

### Comparing `scikit-surgeryutils-2.0.0/versioneer.py` & `scikit-surgeryutils-2.0rc0/versioneer.py`

 * *Files identical despite different names*

