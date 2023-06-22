# Comparing `tmp/featurelayers-1.2.3.tar.gz` & `tmp/featurelayers-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.2.3.tar", last modified: Thu Jun 22 01:40:20 2023, max compression
+gzip compressed data, was "featurelayers-1.2.4.tar", last modified: Thu Jun 22 02:01:34 2023, max compression
```

## Comparing `featurelayers-1.2.3.tar` & `featurelayers-1.2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:40:20.404117 featurelayers-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 01:39:57.000000 featurelayers-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 01:39:57.000000 featurelayers-1.2.3/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:40:20.404117 featurelayers-1.2.3/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 01:40:20.000000 featurelayers-1.2.3/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:40:20.404117 featurelayers-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 01:39:57.000000 featurelayers-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.283755 featurelayers-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:01:34.283755 featurelayers-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 02:01:17.000000 featurelayers-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.279755 featurelayers-1.2.4/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.283755 featurelayers-1.2.4/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.283755 featurelayers-1.2.4/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:01:34.283755 featurelayers-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 02:01:17.000000 featurelayers-1.2.4/setup.py
```

### Comparing `featurelayers-1.2.3/PKG-INFO` & `featurelayers-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.3
+Version: 1.2.4
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
 
-__version__ = ""1.2.3""
+__version__ = ""1.2.4""
```

### Comparing `featurelayers-1.2.3/README.md` & `featurelayers-1.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.3""
+__version__ = ""1.2.4""
```

### Comparing `featurelayers-1.2.3/featurelayers/layers/LBC.py` & `featurelayers-1.2.4/featurelayers/layers/LBC.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,73 +5,65 @@
 import tensorflow as tf
 import keras
 from keras.layers import Conv2D
 from keras import backend as K
 from keras.engine.base_layer import Layer
 
 
-# Non-trainable filters initialized with distribution
-# of Bernoulli as in article and then it's non-trainable
 def new_weights_non_trainable(h, w, num_input, num_output, sparsity=0.5):
     """
-       Create non-trainable weights with a Bernoulli distribution.
+    Create non-trainable weights with a Bernoulli distribution.
 
-       Args:
-           h: Height of the weight matrix.
-           w: Width of the weight matrix.
-           num_input: Number of input channels.
-           num_output: Number of output channels.
-           sparsity: Sparsity level of the weights.
+    Args:
+        h: Height of the weight matrix.
+        w: Width of the weight matrix.
+        num_input: Number of input channels.
+        num_output: Number of output channels.
+        sparsity: Sparsity level of the weights. Default is 0.5.
 
-       Returns:
-           The non-trainable weight matrix.
-
-       """
-
-    # Extract integer values from the tuples
-    h_val, w_val = h
+    Returns:
+        The non-trainable weight matrix.
+    """
+    h_val, w_val = h  # Extract integer values from the tuples
     num_input_val, num_output_val = num_input, num_output
 
-    # Number of elements
-    num_elements = h_val * w_val * num_input_val * num_output_val
-    # Create an array with n number of elements
-    array = np.arange(num_elements)
-    # Random shuffle it
-    np.random.shuffle(array)
-    # Fill with 0
-    weight = np.zeros([num_elements])
-    # Get the number of elements in the array that need to be non-zero
-    ind = int(sparsity * num_elements + 0.5)
-    # Get a piece of it as indexes for the weight matrix
-    index = array[:ind]
+    num_elements = h_val * w_val * num_input_val * num_output_val  # Number of elements
+    array = np.arange(num_elements)  # Create an array with n number of elements
+    np.random.shuffle(array)  # Random shuffle it
+    weight = np.zeros([num_elements])  # Fill with 0
+    ind = int(sparsity * num_elements + 0.5)  # Get the number of elements in the array that need to be non-zero
+    index = array[:ind]  # Get a piece of it as indexes for the weight matrix
 
     for i in index:
         # Fill those indexes with Bernoulli distribution
         # Method rvs = random variates
         weight[i] = bernoulli.rvs(0.5) * 2 - 1
-    # Reshape weights array for the matrix that we need
-    weights = weight.reshape(h_val, w_val, num_input_val, num_output_val)
+    weights = weight.reshape(h_val, w_val, num_input_val, num_output_val)  # Reshape weights array for the matrix that we need
     return weights
 
 
 class LBC(Layer):
     def __init__(self, filters, kernel_size, stride=1, padding='same', activation='relu', dilation=1, sparsity=0.9,
                  name="lbc_layer"):
         """
-        Local Binary Convolution (LBC) layer.
+       Local Binary Convolution (LBC) layer.
 
         Args:
-            filters: Number of filters (output channels) in the convolution.
-            kernel_size: Size of the convolution kernel.
-            stride: Stride of the convolution. Default is 1.
-            padding: Padding mode for the convolution. Default is 'same'.
-            activation: Activation function to use. Default is 'relu'.
-            dilation: Dilation rate for the convolution. Default is 1.
-            sparsity: Sparsity level of the non-trainable weights. Default is 0.9.
-            name: Name of the layer. Default is 'lbc_layer'.
+            - filters: Number of filters (output channels) in the convolution.
+            - kernel_size: Size of the convolution kernel.
+            - stride: Stride of the convolution. Default is 1.
+            - padding: Padding mode for the convolution. Default is 'same'.
+            - activation: Activation function to use. Default is 'relu'.
+            - dilation: Dilation rate for the convolution. Default is 1.
+            - sparsity: Sparsity level of the non-trainable weights. Default is 0.9.
+            - name: Name of the layer. Default is 'lbc_layer'.
+
+        Returns:
+            The LBC layer.
+
         """
         super(LBC, self).__init__()
         self.nOutputPlane = filters
         self.kW = kernel_size
         self.sparsity = sparsity
         self.LBC = Conv2D(filters, kernel_size=kernel_size, strides=stride, padding=padding,
                           dilation_rate=dilation, activation=activation, use_bias=False, name=name)
```

### Comparing `featurelayers-1.2.3/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.2.4/featurelayers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.3
+Version: 1.2.4
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
 
-__version__ = ""1.2.3""
+__version__ = ""1.2.4""
```

### Comparing `featurelayers-1.2.3/setup.py` & `featurelayers-1.2.4/setup.py`

 * *Files identical despite different names*

