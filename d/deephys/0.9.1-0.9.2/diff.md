# Comparing `tmp/deephys-0.9.1.tar.gz` & `tmp/deephys-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephys-0.9.1.tar", last modified: Fri Jan 27 19:06:24 2023, max compression
+gzip compressed data, was "deephys-0.9.2.tar", last modified: Fri Jan 27 19:12:56 2023, max compression
```

## Comparing `deephys-0.9.1.tar` & `deephys-0.9.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-01-27 19:06:24.781249 deephys-0.9.1/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      299 2023-01-27 19:06:24.781077 deephys-0.9.1/PKG-INFO
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-01-27 19:06:24.779914 deephys-0.9.1/deephys/
--r--r--r--   0 matthewgroth   (501) staff       (20)      307 2023-01-05 20:12:06.000000 deephys-0.9.1/deephys/__init__.py
--r--r--r--   0 matthewgroth   (501) staff       (20)     9022 2023-01-27 19:06:01.000000 deephys-0.9.1/deephys/deephys.py
-drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-01-27 19:06:24.780908 deephys-0.9.1/deephys.egg-info/
--rw-r--r--   0 matthewgroth   (501) staff       (20)      299 2023-01-27 19:06:24.000000 deephys-0.9.1/deephys.egg-info/PKG-INFO
--rw-r--r--   0 matthewgroth   (501) staff       (20)      207 2023-01-27 19:06:24.000000 deephys-0.9.1/deephys.egg-info/SOURCES.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-01-27 19:06:24.000000 deephys-0.9.1/deephys.egg-info/dependency_links.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)       18 2023-01-27 19:06:24.000000 deephys-0.9.1/deephys.egg-info/requires.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)        8 2023-01-27 19:06:24.000000 deephys-0.9.1/deephys.egg-info/top_level.txt
--rw-r--r--   0 matthewgroth   (501) staff       (20)      367 2023-01-27 19:05:05.000000 deephys-0.9.1/pyproject.toml
--rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-01-27 19:06:24.781291 deephys-0.9.1/setup.cfg
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-01-27 19:12:56.440220 deephys-0.9.2/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      299 2023-01-27 19:12:56.440049 deephys-0.9.2/PKG-INFO
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-01-27 19:12:56.438791 deephys-0.9.2/deephys/
+-r--r--r--   0 matthewgroth   (501) staff       (20)      307 2023-01-05 20:12:06.000000 deephys-0.9.2/deephys/__init__.py
+-r--r--r--   0 matthewgroth   (501) staff       (20)     9237 2023-01-27 19:11:32.000000 deephys-0.9.2/deephys/deephys.py
+drwxr-xr-x   0 matthewgroth   (501) staff       (20)        0 2023-01-27 19:12:56.439859 deephys-0.9.2/deephys.egg-info/
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      299 2023-01-27 19:12:56.000000 deephys-0.9.2/deephys.egg-info/PKG-INFO
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      207 2023-01-27 19:12:56.000000 deephys-0.9.2/deephys.egg-info/SOURCES.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        1 2023-01-27 19:12:56.000000 deephys-0.9.2/deephys.egg-info/dependency_links.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       18 2023-01-27 19:12:56.000000 deephys-0.9.2/deephys.egg-info/requires.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)        8 2023-01-27 19:12:56.000000 deephys-0.9.2/deephys.egg-info/top_level.txt
+-rw-r--r--   0 matthewgroth   (501) staff       (20)      367 2023-01-27 19:11:07.000000 deephys-0.9.2/pyproject.toml
+-rw-r--r--   0 matthewgroth   (501) staff       (20)       38 2023-01-27 19:12:56.440268 deephys-0.9.2/setup.cfg
```

### Comparing `deephys-0.9.1/deephys/deephys.py` & `deephys-0.9.2/deephys/deephys.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,32 +48,38 @@
     """
 
     layers: List[Layer]
 
     def __post_init__(self):
         self.extension = f"model"
 
-    def state(self, activations):
+    def state(self, activations, dtype):
         if len(activations) != len(self.layers):
             raise Exception(
                 f"expected activations data with length of {len(self.layers)} (number of layers) but got {len(activations)}"
             )
+        if dtype == "float32":
+            b = 4
+        elif dtype == "float64":
+            b = 8
+        else:
+            raise Exception(f"invalid dtype: {dtype}")
         for index, sub in enumerate(activations):
-            subLen = len(sub) / 4
+            subLen = len(sub) / b
             neuronsLen = len(self.layers[index].neurons)
             if subLen != neuronsLen:
                 raise Exception(
-                    f"expected activations data with length of {neuronsLen} (number of neurons in layer {index}) but got {subLen / 4}"
+                    f"expected activations data with length of {neuronsLen} (number of neurons in layer {index}) but got {subLen / b}"
                 )
         ms = self.ModelState(activations)
         return ms
 
     @dataclass
     class ModelState:
-        activations: List[bytearray]  # float32
+        activations: List[bytearray]  # float32 or float64
 
 
 def import_torch_dataset(
     name: str,
     dataset: torch.utils.data.DataLoader,
     classes: list,
     state: Union[list, np.ndarray, torch.FloatTensor],
@@ -212,15 +218,16 @@
                     list(
                         map(
                             lambda layer: bytearray(
                                 [b for a in layer for b in float_fun(a)]
                             ),
                             im_activations,
                         )
-                    )
+                    ),
+                    dtype,
                 ),
                 features=None,
             )
         )
     test = Test(name=name, suffix=None, dtype=dtype, images=imageList)
     return test
```

