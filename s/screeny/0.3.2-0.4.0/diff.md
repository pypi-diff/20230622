# Comparing `tmp/screeny-0.3.2.tar.gz` & `tmp/screeny-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screeny-0.3.2.tar", last modified: Fri May 12 19:15:53 2023, max compression
+gzip compressed data, was "screeny-0.4.0.tar", last modified: Thu Jun 22 19:52:37 2023, max compression
```

## Comparing `screeny-0.3.2.tar` & `screeny-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 19:15:53.796268 screeny-0.3.2/
--rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.3.2/LICENSE
--rw-r--r--   0 paulpol    (501) staff       (20)    25695 2023-05-12 15:40:17.000000 screeny-0.3.2/LICENSE-3RD-Party.txt
--rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 19:15:53.796400 screeny-0.3.2/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)     2544 2023-05-12 15:40:04.000000 screeny-0.3.2/README.md
--rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.3.2/pyproject.toml
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 19:15:53.794083 screeny-0.3.2/screeny/
--rw-r--r--   0 paulpol    (501) staff       (20)      195 2023-05-12 15:40:04.000000 screeny-0.3.2/screeny/__init__.py
--rw-r--r--   0 paulpol    (501) staff       (20)     4530 2023-05-12 19:11:06.000000 screeny-0.3.2/screeny/image.py
--rw-r--r--   0 paulpol    (501) staff       (20)      445 2023-05-12 15:40:04.000000 screeny-0.3.2/screeny/mouse.py
--rw-r--r--   0 paulpol    (501) staff       (20)     2294 2023-05-12 18:59:44.000000 screeny-0.3.2/screeny/screeny.py
-drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-05-12 19:15:53.795963 screeny-0.3.2/screeny.egg-info/
--rw-r--r--   0 paulpol    (501) staff       (20)     2925 2023-05-12 19:15:53.000000 screeny-0.3.2/screeny.egg-info/PKG-INFO
--rw-r--r--   0 paulpol    (501) staff       (20)      291 2023-05-12 19:15:53.000000 screeny-0.3.2/screeny.egg-info/SOURCES.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-05-12 19:15:53.000000 screeny-0.3.2/screeny.egg-info/dependency_links.txt
--rw-r--r--   0 paulpol    (501) staff       (20)       55 2023-05-12 19:15:53.000000 screeny-0.3.2/screeny.egg-info/requires.txt
--rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-05-12 19:15:53.000000 screeny-0.3.2/screeny.egg-info/top_level.txt
--rw-r--r--   0 paulpol    (501) staff       (20)      528 2023-05-12 19:15:53.797014 screeny-0.3.2/setup.cfg
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-22 19:52:37.276400 screeny-0.4.0/
+-rw-r--r--   0 paulpol    (501) staff       (20)     1065 2023-04-28 17:23:56.000000 screeny-0.4.0/LICENSE
+-rw-r--r--   0 paulpol    (501) staff       (20)    25695 2023-05-12 15:40:17.000000 screeny-0.4.0/LICENSE-3RD-Party.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)     3557 2023-06-22 19:52:37.276584 screeny-0.4.0/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)     3176 2023-06-22 19:43:27.000000 screeny-0.4.0/README.md
+-rw-r--r--   0 paulpol    (501) staff       (20)       80 2023-05-09 15:01:19.000000 screeny-0.4.0/pyproject.toml
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-22 19:52:37.273563 screeny-0.4.0/screeny/
+-rw-r--r--   0 paulpol    (501) staff       (20)      239 2023-06-22 19:28:07.000000 screeny-0.4.0/screeny/__init__.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     7260 2023-06-22 19:43:27.000000 screeny-0.4.0/screeny/image.py
+-rw-r--r--   0 paulpol    (501) staff       (20)      445 2023-05-12 15:40:04.000000 screeny-0.4.0/screeny/mouse.py
+-rw-r--r--   0 paulpol    (501) staff       (20)     2294 2023-05-12 18:59:44.000000 screeny-0.4.0/screeny/screeny.py
+drwxr-xr-x   0 paulpol    (501) staff       (20)        0 2023-06-22 19:52:37.275978 screeny-0.4.0/screeny.egg-info/
+-rw-r--r--   0 paulpol    (501) staff       (20)     3557 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/PKG-INFO
+-rw-r--r--   0 paulpol    (501) staff       (20)      291 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/SOURCES.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        1 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/dependency_links.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)       55 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/requires.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)        8 2023-06-22 19:52:37.000000 screeny-0.4.0/screeny.egg-info/top_level.txt
+-rw-r--r--   0 paulpol    (501) staff       (20)      528 2023-06-22 19:52:37.277384 screeny-0.4.0/setup.cfg
```

### Comparing `screeny-0.3.2/LICENSE` & `screeny-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screeny-0.3.2/LICENSE-3RD-Party.txt` & `screeny-0.4.0/LICENSE-3RD-Party.txt`

 * *Files identical despite different names*

### Comparing `screeny-0.3.2/PKG-INFO` & `screeny-0.4.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: screeny
-Version: 0.3.2
-Summary: A simple python library for working with screens and images.
-Author: Paul Pol
-Author-email: mail@paul-pol.de
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: LICENSE-3RD-Party.txt
-
 # Screeny
 A simple python library for working with screens and images.
 
 ## Installation
 
 ```sh
 pip install screeny
@@ -34,21 +21,26 @@
 * [Screeny.get_mouse_pos](#screenyget_mouse_pos)
 * [Screeny.locate_image](#screenylocate_imageimage-str--npndarray--image--rect-rect-confidence-float)
 * [Screeny.read_text](#screenyread_textrect-rect)
 * [Screeny.take_screenshot](#screenytake_screenshotrect-rect)
 ####
 * [Image.__init__](#imageinitimage-str--npndarray--image)
 * [Image.binarize](#imagebinarizemethod-str-threshold-int)
+* Image.compute_descriptors
 * [Image.denoise](#imagedenoise)
+* Image.detect_features
+* Image.detect_keypoints
 * [Image.get_data](#imageget_data)
 * [Image.invert](#imageinvert)
 * [Image.locate_image](#imagelocate_imageimage_to_find-str--npndarray--image-confidence-float)
+* Image.match_features
 * [Image.read_text](#imageread_textresize_factor-int-whitelist-str)
 * [Image.resize](#imageresizefactor-int)
 * [Image.show](#imageshowtitle-str)
+* Image.show_matches
 * [Image.to_grayscale](#imageto_grayscale)
 * [Image.to_hsv](#imageto_hsv)
 
 ### Screeny-class
 
 #### Screeny.get_mouse_pos()
         
@@ -78,19 +70,34 @@
 
 ---
 #### Image.binarize(method: str[, threshold: int])
 
 Binarize the image.
 
 ---
+#### Image.compute_descriptors()
+
+Computes the descriptors of the image.
+
+---
 #### Image.denoise()
 
 Denoise the image.
 
 ---
+#### Image.detect_features()
+
+Finds features (keypoints and descriptors) in the image.
+
+---
+#### Image.detect_keypoints()
+
+Finds the keypoints of the image.
+
+---
 #### Image.get_data()
 
 Returns the pixels as numpy-array.
 
 ---
 #### Image.invert()
 
@@ -98,14 +105,19 @@
 
 ---
 #### Image.locate_image(image_to_find: str | np.ndarray | Image[, confidence: float])
 
 Locates an second image in the image and returns the position of the founded image or False if no image was found.
 
 ---
+#### Image.match_features(image_to_find: str | np.ndarray | Image)
+
+Matches the features of the image with another image.
+
+---
 #### Image.read_text([resize_factor: int, whitelist: str])
 
 Reads the text from the image.
 
 ---
 #### Image.resize(factor: int)
 
@@ -113,15 +125,20 @@
 
 ---
 #### Image.show([title: str])
 
 Displays the image.
 
 ---
+#### Image.show_matches(image_to_find: str | np.ndarray | Image, matches: list)
+
+Show the two images with matches as lines connect points.
+
+---
 #### Image.to_grayscale()
 
 Converts the image to grayscale.
 
 ---
 #### Image.to_hsv()
 
-Converts the image to HSV.
+Converts the image to HSV.
```

### Comparing `screeny-0.3.2/screeny/screeny.py` & `screeny-0.4.0/screeny/screeny.py`

 * *Files identical despite different names*

### Comparing `screeny-0.3.2/screeny.egg-info/PKG-INFO` & `screeny-0.4.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: screeny
-Version: 0.3.2
+Version: 0.4.0
 Summary: A simple python library for working with screens and images.
 Author: Paul Pol
 Author-email: mail@paul-pol.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
@@ -34,21 +34,26 @@
 * [Screeny.get_mouse_pos](#screenyget_mouse_pos)
 * [Screeny.locate_image](#screenylocate_imageimage-str--npndarray--image--rect-rect-confidence-float)
 * [Screeny.read_text](#screenyread_textrect-rect)
 * [Screeny.take_screenshot](#screenytake_screenshotrect-rect)
 ####
 * [Image.__init__](#imageinitimage-str--npndarray--image)
 * [Image.binarize](#imagebinarizemethod-str-threshold-int)
+* Image.compute_descriptors
 * [Image.denoise](#imagedenoise)
+* Image.detect_features
+* Image.detect_keypoints
 * [Image.get_data](#imageget_data)
 * [Image.invert](#imageinvert)
 * [Image.locate_image](#imagelocate_imageimage_to_find-str--npndarray--image-confidence-float)
+* Image.match_features
 * [Image.read_text](#imageread_textresize_factor-int-whitelist-str)
 * [Image.resize](#imageresizefactor-int)
 * [Image.show](#imageshowtitle-str)
+* Image.show_matches
 * [Image.to_grayscale](#imageto_grayscale)
 * [Image.to_hsv](#imageto_hsv)
 
 ### Screeny-class
 
 #### Screeny.get_mouse_pos()
         
@@ -78,19 +83,34 @@
 
 ---
 #### Image.binarize(method: str[, threshold: int])
 
 Binarize the image.
 
 ---
+#### Image.compute_descriptors()
+
+Computes the descriptors of the image.
+
+---
 #### Image.denoise()
 
 Denoise the image.
 
 ---
+#### Image.detect_features()
+
+Finds features (keypoints and descriptors) in the image.
+
+---
+#### Image.detect_keypoints()
+
+Finds the keypoints of the image.
+
+---
 #### Image.get_data()
 
 Returns the pixels as numpy-array.
 
 ---
 #### Image.invert()
 
@@ -98,14 +118,19 @@
 
 ---
 #### Image.locate_image(image_to_find: str | np.ndarray | Image[, confidence: float])
 
 Locates an second image in the image and returns the position of the founded image or False if no image was found.
 
 ---
+#### Image.match_features(image_to_find: str | np.ndarray | Image)
+
+Matches the features of the image with another image.
+
+---
 #### Image.read_text([resize_factor: int, whitelist: str])
 
 Reads the text from the image.
 
 ---
 #### Image.resize(factor: int)
 
@@ -113,14 +138,19 @@
 
 ---
 #### Image.show([title: str])
 
 Displays the image.
 
 ---
+#### Image.show_matches(image_to_find: str | np.ndarray | Image, matches: list)
+
+Show the two images with matches as lines connect points.
+
+---
 #### Image.to_grayscale()
 
 Converts the image to grayscale.
 
 ---
 #### Image.to_hsv()
```

### Comparing `screeny-0.3.2/setup.cfg` & `screeny-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = screeny
-version = 0.3.2
+version = 0.4.0
 author = Paul Pol
 author_email = mail@paul-pol.de
 description = A simple python library for working with screens and images.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 classifiers =
```

