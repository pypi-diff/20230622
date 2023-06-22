# Comparing `tmp/featurelayers-1.2.1.tar.gz` & `tmp/featurelayers-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.2.1.tar", last modified: Thu Jun 22 01:06:46 2023, max compression
+gzip compressed data, was "featurelayers-1.2.3.tar", last modified: Thu Jun 22 01:40:20 2023, max compression
```

## Comparing `featurelayers-1.2.1.tar` & `featurelayers-1.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.780841 featurelayers-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:06:46.780841 featurelayers-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 01:06:22.000000 featurelayers-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.776841 featurelayers-1.2.1/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.780841 featurelayers-1.2.1/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.776841 featurelayers-1.2.1/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:06:46.780841 featurelayers-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 01:06:22.000000 featurelayers-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:40:20.404117 featurelayers-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 01:39:57.000000 featurelayers-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:40:20.404117 featurelayers-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 01:39:57.000000 featurelayers-1.2.3/setup.py
```

### Comparing `featurelayers-1.2.1/PKG-INFO` & `featurelayers-1.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.1
+Version: 1.2.3
 Summary: FeatureLayers Package
 Author: khengyun
 Author-email: khaangnguyeen@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
@@ -46,8 +46,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.1""
+__version__ = ""1.2.3""
```

### Comparing `featurelayers-1.2.1/README.md` & `featurelayers-1.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.1""
+__version__ = ""1.2.3""
```

### Comparing `featurelayers-1.2.1/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.2.3/featurelayers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.1
+Version: 1.2.3
 Summary: FeatureLayers Package
 Author: khengyun
 Author-email: khaangnguyeen@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
@@ -46,8 +46,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.1""
+__version__ = ""1.2.3""
```

### Comparing `featurelayers-1.2.1/setup.py` & `featurelayers-1.2.3/setup.py`

 * *Files identical despite different names*

