# Comparing `tmp/featurelayers-1.2.0.tar.gz` & `tmp/featurelayers-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.2.0.tar", last modified: Thu Jun 22 01:04:14 2023, max compression
+gzip compressed data, was "featurelayers-1.2.1.tar", last modified: Thu Jun 22 01:06:46 2023, max compression
```

## Comparing `featurelayers-1.2.0.tar` & `featurelayers-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:04:14.949221 featurelayers-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-22 01:04:14.945221 featurelayers-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-22 01:03:55.000000 featurelayers-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:04:14.945221 featurelayers-1.2.0/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:03:55.000000 featurelayers-1.2.0/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 01:03:55.000000 featurelayers-1.2.0/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 01:03:55.000000 featurelayers-1.2.0/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:04:14.945221 featurelayers-1.2.0/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-22 01:03:55.000000 featurelayers-1.2.0/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 01:03:55.000000 featurelayers-1.2.0/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:04:14.945221 featurelayers-1.2.0/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-22 01:04:14.000000 featurelayers-1.2.0/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 01:04:14.000000 featurelayers-1.2.0/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:04:14.000000 featurelayers-1.2.0/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 01:04:14.000000 featurelayers-1.2.0/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 01:04:14.000000 featurelayers-1.2.0/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:04:14.949221 featurelayers-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 01:03:55.000000 featurelayers-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.780841 featurelayers-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:06:46.780841 featurelayers-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 01:06:22.000000 featurelayers-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.776841 featurelayers-1.2.1/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.780841 featurelayers-1.2.1/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 01:06:22.000000 featurelayers-1.2.1/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:06:46.776841 featurelayers-1.2.1/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 01:06:46.000000 featurelayers-1.2.1/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:06:46.780841 featurelayers-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 01:06:22.000000 featurelayers-1.2.1/setup.py
```

### Comparing `featurelayers-1.2.0/PKG-INFO` & `featurelayers-1.2.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.0
+Version: 1.2.1
 Summary: FeatureLayers Package
 Author: khengyun
 Author-email: khaangnguyeen@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
@@ -20,15 +20,15 @@
 
 
 ## Usage
 ```python
 import numpy as np
 from keras.models import Sequential
 from keras.layers import Dense, Flatten
-from your_module import LBC
+from featurelayers.layers.LBC import LBC
 
 # Create a simple Keras model
 model = Sequential()
 # Add the LBC layer as the first layer in the model
 model.add(LBC(filters=32, kernel_size=3, stride=1, padding='same', activation='relu', sparsity=0.9, name='lbc_layer'))
 # Add a Flatten layer to convert the output to 1D
 model.add(Flatten())
@@ -46,8 +46,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.0""
+__version__ = ""1.2.1""
```

### Comparing `featurelayers-1.2.0/README.md` & `featurelayers-1.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 ## Usage
 ```python
 import numpy as np
 from keras.models import Sequential
 from keras.layers import Dense, Flatten
-from your_module import LBC
+from featurelayers.layers.LBC import LBC
 
 # Create a simple Keras model
 model = Sequential()
 # Add the LBC layer as the first layer in the model
 model.add(LBC(filters=32, kernel_size=3, stride=1, padding='same', activation='relu', sparsity=0.9, name='lbc_layer'))
 # Add a Flatten layer to convert the output to 1D
 model.add(Flatten())
@@ -33,8 +33,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.0""
+__version__ = ""1.2.1""
```

### Comparing `featurelayers-1.2.0/featurelayers/layers/LBC.py` & `featurelayers-1.2.1/featurelayers/layers/LBC.py`

 * *Files identical despite different names*

### Comparing `featurelayers-1.2.0/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.2.1/featurelayers.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.0
+Version: 1.2.1
 Summary: FeatureLayers Package
 Author: khengyun
 Author-email: khaangnguyeen@email.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
@@ -20,15 +20,15 @@
 
 
 ## Usage
 ```python
 import numpy as np
 from keras.models import Sequential
 from keras.layers import Dense, Flatten
-from your_module import LBC
+from featurelayers.layers.LBC import LBC
 
 # Create a simple Keras model
 model = Sequential()
 # Add the LBC layer as the first layer in the model
 model.add(LBC(filters=32, kernel_size=3, stride=1, padding='same', activation='relu', sparsity=0.9, name='lbc_layer'))
 # Add a Flatten layer to convert the output to 1D
 model.add(Flatten())
@@ -46,8 +46,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.0""
+__version__ = ""1.2.1""
```

### Comparing `featurelayers-1.2.0/setup.py` & `featurelayers-1.2.1/setup.py`

 * *Files identical despite different names*

