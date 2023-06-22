# Comparing `tmp/featurelayers-1.2.4.tar.gz` & `tmp/featurelayers-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featurelayers-1.2.4.tar", last modified: Thu Jun 22 02:01:34 2023, max compression
+gzip compressed data, was "featurelayers-1.2.6.tar", last modified: Thu Jun 22 02:55:06 2023, max compression
```

## Comparing `featurelayers-1.2.4.tar` & `featurelayers-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.283755 featurelayers-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:01:34.283755 featurelayers-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 02:01:17.000000 featurelayers-1.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.279755 featurelayers-1.2.4/featurelayers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.283755 featurelayers-1.2.4/featurelayers/layers/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/layers/LBC.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 02:01:17.000000 featurelayers-1.2.4/featurelayers/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:01:34.283755 featurelayers-1.2.4/featurelayers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 02:01:34.000000 featurelayers-1.2.4/featurelayers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:01:34.283755 featurelayers-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 02:01:17.000000 featurelayers-1.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:55:06.642799 featurelayers-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-22 02:54:46.000000 featurelayers-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/featurelayers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/featurelayers/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/layers/LBC.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 02:54:46.000000 featurelayers-1.2.6/featurelayers/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 02:55:06.642799 featurelayers-1.2.6/featurelayers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 02:55:06.000000 featurelayers-1.2.6/featurelayers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 02:55:06.642799 featurelayers-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-22 02:54:46.000000 featurelayers-1.2.6/setup.py
```

### Comparing `featurelayers-1.2.4/PKG-INFO` & `featurelayers-1.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.4
+Version: 1.2.6
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
 
-__version__ = ""1.2.4""
+__version__ = ""1.2.6""
```

### Comparing `featurelayers-1.2.4/README.md` & `featurelayers-1.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
 y_train = keras.utils.to_categorical(y_train, num_classes=10)
 
 # Train the model
 model.fit(x_train, y_train, epochs=10, batch_size=32)
 
 ```
 
-__version__ = ""1.2.4""
+__version__ = ""1.2.6""
```

### Comparing `featurelayers-1.2.4/featurelayers/layers/LBC.py` & `featurelayers-1.2.6/featurelayers/layers/LBC.py`

 * *Files 9% similar despite different names*

```diff
@@ -65,62 +65,32 @@
         self.nOutputPlane = filters
         self.kW = kernel_size
         self.sparsity = sparsity
         self.LBC = Conv2D(filters, kernel_size=kernel_size, strides=stride, padding=padding,
                           dilation_rate=dilation, activation=activation, use_bias=False, name=name)
 
     def build(self, input_shape):
-        """
-        Build the layer.
-
-        Args:
-            input_shape: Shape of the input tensor.
-        """
         nInputPlane = input_shape[-1]
 
         with K.name_scope(self.LBC.name):
             self.LBC.build(input_shape)
         anchor_weights = tf.Variable(new_weights_non_trainable(h=self.kW, w=self.kW, num_input=nInputPlane,
                                                                num_output=self.nOutputPlane,
                                                                sparsity=self.sparsity).astype(np.float32),
                                      trainable=False)
         self.LBC.kernel = anchor_weights
         super(LBC, self).build(input_shape)
 
     def call(self, x):
-        """
-        Perform the forward pass of the layer.
-
-        Args:
-            x: Input tensor.
-
-        Returns:
-            Output tensor.
-        """
         return self.LBC(x)
 
     def compute_output_shape(self, input_shape):
-        """
-        Compute the output shape of the layer.
-
-        Args:
-            input_shape: Shape of the input tensor.
-
-        Returns:
-            Output shape.
-        """
         return self.LBC.compute_output_shape(input_shape)
 
     def get_config(self):
-        """
-        Get the configuration of the layer.
-
-        Returns:
-            Configuration dictionary.
-        """
         config = super(LBC, self).get_config()
         config.update({
             'filters': self.nOutputPlane,
             'kernel_size': self.kW,
             'stride': self.LBC.strides[0],
             'padding': self.LBC.padding,
             'activation': self.LBC.activation,
```

### Comparing `featurelayers-1.2.4/featurelayers.egg-info/PKG-INFO` & `featurelayers-1.2.6/featurelayers.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurelayers
-Version: 1.2.4
+Version: 1.2.6
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
 
-__version__ = ""1.2.4""
+__version__ = ""1.2.6""
```

### Comparing `featurelayers-1.2.4/setup.py` & `featurelayers-1.2.6/setup.py`

 * *Files identical despite different names*

