# Comparing `tmp/featurelayers-1.2.6.tar.gz` & `tmp/featurelayers-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.2.6.tar", last modified: Thu Jun 22 02:55:06 2023, max compression
+gzip compressed data, was "featurelayers-1.2.7.tar", last modified: Thu Jun 22 03:06:59 2023, max compression
```

## Comparing `featurelayers-1.2.6.tar` & `featurelayers-1.2.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:55:06.642799 featurelayers-1.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 02:54:46.000000 featurelayers-1.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:55:06.642799 featurelayers-1.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 02:54:46.000000 featurelayers-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:06:59.453309 featurelayers-1.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 03:06:59.453309 featurelayers-1.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 03:06:35.000000 featurelayers-1.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:06:59.453309 featurelayers-1.2.7/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 03:06:35.000000 featurelayers-1.2.7/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 03:06:35.000000 featurelayers-1.2.7/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 03:06:35.000000 featurelayers-1.2.7/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:06:59.453309 featurelayers-1.2.7/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-06-22 03:06:35.000000 featurelayers-1.2.7/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 03:06:35.000000 featurelayers-1.2.7/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:06:59.453309 featurelayers-1.2.7/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 03:06:59.000000 featurelayers-1.2.7/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 03:06:59.000000 featurelayers-1.2.7/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:06:59.000000 featurelayers-1.2.7/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 03:06:59.000000 featurelayers-1.2.7/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 03:06:59.000000 featurelayers-1.2.7/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:06:59.453309 featurelayers-1.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 03:06:35.000000 featurelayers-1.2.7/setup.py
```

### Comparing `featurelayers-1.2.6/PKG-INFO` & `featurelayers-1.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.6
+Version: 1.2.7
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
 
-__version__ = ""1.2.6""
+__version__ = ""1.2.7""
```

### Comparing `featurelayers-1.2.6/README.md` & `featurelayers-1.2.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.6""
+__version__ = ""1.2.7""
```

### Comparing `featurelayers-1.2.6/featurelayers/layers/LBC.py` & `featurelayers-1.2.7/featurelayers/layers/LBC.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,34 +37,37 @@
         # Fill those indexes with Bernoulli distribution
         # Method rvs = random variates
         weight[i] = bernoulli.rvs(0.5) * 2 - 1
     weights = weight.reshape(h_val, w_val, num_input_val, num_output_val)  # Reshape weights array for the matrix that we need
     return weights
 
 
+
+
+
 class LBC(Layer):
     def __init__(self, filters, kernel_size, stride=1, padding='same', activation='relu', dilation=1, sparsity=0.9,
-                 name="lbc_layer"):
+                 name="khengyun"):
         """
-       Local Binary Convolution (LBC) layer.
+              Local Binary Convolution (LBC) layer.
 
-        Args:
-            - filters: Number of filters (output channels) in the convolution.
-            - kernel_size: Size of the convolution kernel.
-            - stride: Stride of the convolution. Default is 1.
-            - padding: Padding mode for the convolution. Default is 'same'.
-            - activation: Activation function to use. Default is 'relu'.
-            - dilation: Dilation rate for the convolution. Default is 1.
-            - sparsity: Sparsity level of the non-trainable weights. Default is 0.9.
-            - name: Name of the layer. Default is 'lbc_layer'.
+               Args:
+                   - filters: Number of filters (output channels) in the convolution.
+                   - kernel_size: Size of the convolution kernel.
+                   - stride: Stride of the convolution. Default is 1.
+                   - padding: Padding mode for the convolution. Default is 'same'.
+                   - activation: Activation function to use. Default is 'relu'.
+                   - dilation: Dilation rate for the convolution. Default is 1.
+                   - sparsity: Sparsity level of the non-trainable weights. Default is 0.9.
+                   - name: Name of the layer. Default is 'lbc_layer'.
 
-        Returns:
-            The LBC layer.
+               Returns:
+                   The LBC layer.
 
-        """
+               """
         super(LBC, self).__init__()
         self.nOutputPlane = filters
         self.kW = kernel_size
         self.sparsity = sparsity
         self.LBC = Conv2D(filters, kernel_size=kernel_size, strides=stride, padding=padding,
                           dilation_rate=dilation, activation=activation, use_bias=False, name=name)
 
@@ -95,7 +98,8 @@
             'padding': self.LBC.padding,
             'activation': self.LBC.activation,
             'dilation': self.LBC.dilation_rate[0],
             'sparsity': self.sparsity,
             'name': self.LBC.name
         })
         return config
+
```

### Comparing `featurelayers-1.2.6/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.2.7/featurelayers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.6
+Version: 1.2.7
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
 
-__version__ = ""1.2.6""
+__version__ = ""1.2.7""
```

### Comparing `featurelayers-1.2.6/setup.py` & `featurelayers-1.2.7/setup.py`

 * *Files identical despite different names*

