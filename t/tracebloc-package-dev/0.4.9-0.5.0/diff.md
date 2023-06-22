# Comparing `tmp/tracebloc_package-dev-0.4.9.tar.gz` & `tmp/tracebloc_package-dev-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tracebloc_package-dev-0.4.9.tar", last modified: Fri Jun  9 11:52:41 2023, max compression
+gzip compressed data, was "tracebloc_package-dev-0.5.0.tar", last modified: Thu Jun 22 04:59:11 2023, max compression
```

## Comparing `tracebloc_package-dev-0.4.9.tar` & `tracebloc_package-dev-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:52:41.851592 tracebloc_package-dev-0.4.9/
--rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.9/LICENSE.txt
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-09 11:52:41.851713 tracebloc_package-dev-0.4.9/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.4.9/README.md
--rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-09 11:52:41.856260 tracebloc_package-dev-0.4.9/setup.cfg
--rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-09 11:51:30.000000 tracebloc_package-dev-0.4.9/setup.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:52:41.850265 tracebloc_package-dev-0.4.9/tracebloc_package/
--rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.9/tracebloc_package/__init__.py
--rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.9/tracebloc_package/check_parameters.py
--rw-r--r--   0 hasan      (501) staff       (20)    21521 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/functional_test.py
--rw-r--r--   0 hasan      (501) staff       (20)    61149 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/linkModelDataSet.py
--rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/messages.py
--rw-r--r--   0 hasan      (501) staff       (20)    10234 2023-06-09 11:45:18.000000 tracebloc_package-dev-0.4.9/tracebloc_package/upload.py
--rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/user.py
--rw-r--r--   0 hasan      (501) staff       (20)     5840 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.4.9/tracebloc_package/utils.py
--rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 11:24:43.000000 tracebloc_package-dev-0.4.9/tracebloc_package/weights.py
-drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-09 11:52:41.851398 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/
--rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/PKG-INFO
--rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/SOURCES.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/dependency_links.txt
--rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/not-zip-safe
--rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/requires.txt
--rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-09 11:52:41.000000 tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/top_level.txt
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-22 04:59:11.330904 tracebloc_package-dev-0.5.0/
+-rw-r--r--   0 hasan      (501) staff       (20)     1048 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.0/LICENSE.txt
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-22 04:59:11.330985 tracebloc_package-dev-0.5.0/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      188 2022-05-16 08:30:43.000000 tracebloc_package-dev-0.5.0/README.md
+-rw-r--r--   0 hasan      (501) staff       (20)       78 2023-06-22 04:59:11.331298 tracebloc_package-dev-0.5.0/setup.cfg
+-rw-r--r--   0 hasan      (501) staff       (20)      949 2023-06-22 04:56:54.000000 tracebloc_package-dev-0.5.0/setup.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-22 04:59:11.329692 tracebloc_package-dev-0.5.0/tracebloc_package/
+-rw-r--r--   0 hasan      (501) staff       (20)       67 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.0/tracebloc_package/__init__.py
+-rw-r--r--   0 hasan      (501) staff       (20)     5669 2023-06-07 12:41:07.000000 tracebloc_package-dev-0.5.0/tracebloc_package/check_parameters.py
+-rw-r--r--   0 hasan      (501) staff       (20)    24369 2023-06-21 10:23:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/functional_test.py
+-rw-r--r--   0 hasan      (501) staff       (20)    61149 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/linkModelDataSet.py
+-rw-r--r--   0 hasan      (501) staff       (20)     7100 2023-03-23 11:28:43.000000 tracebloc_package-dev-0.5.0/tracebloc_package/messages.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10936 2023-06-21 10:23:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/upload.py
+-rw-r--r--   0 hasan      (501) staff       (20)    10427 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/user.py
+-rw-r--r--   0 hasan      (501) staff       (20)     6712 2023-06-21 10:23:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/utils.py
+-rw-r--r--   0 hasan      (501) staff       (20)     3200 2023-06-09 12:24:04.000000 tracebloc_package-dev-0.5.0/tracebloc_package/weights.py
+drwxr-xr-x   0 hasan      (501) staff       (20)        0 2023-06-22 04:59:11.330748 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/
+-rw-r--r--   0 hasan      (501) staff       (20)      577 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/PKG-INFO
+-rw-r--r--   0 hasan      (501) staff       (20)      591 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 hasan      (501) staff       (20)        1 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/not-zip-safe
+-rw-r--r--   0 hasan      (501) staff       (20)      119 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/requires.txt
+-rw-r--r--   0 hasan      (501) staff       (20)       18 2023-06-22 04:59:11.000000 tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/top_level.txt
```

### Comparing `tracebloc_package-dev-0.4.9/LICENSE.txt` & `tracebloc_package-dev-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.9/PKG-INFO` & `tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tracebloc_package-dev
-Version: 0.4.9
+Name: tracebloc-package-dev
+Version: 0.5.0
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.9/setup.py` & `tracebloc_package-dev-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="tracebloc_package-dev",
-    version="0.4.9",
+    version="0.5.0",
     description="Package required to run Tracebloc jupyter notebook to create experiment",
     url="https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev",
     license="MIT",
     python_requires=">=3",
     packages=["tracebloc_package"],
     author="Tracebloc",
     author_email="info@tracebloc.io",
```

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/check_parameters.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/check_parameters.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/functional_test.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/functional_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 silence_tensorflow()
 import os
 import dis
 import re
 import shutil
 from torch.utils.data import DataLoader
+from collections import OrderedDict
 import torch.optim as optim
 import torch.nn as nn
 import torchvision.datasets as datasets
 from inspect import getmembers, isfunction
 from .utils import *
 
 
@@ -346,32 +347,40 @@
     def model_func_checks(self):
         # check if model is eligible
         try:
             self.load_model_file()
             self.message = "all check passed"
             eligible = True
         except Exception as e:  # pragma: no cover
-            if self.message == "":
-                self.message = f"Model checks failed with error as {e}"
+            self.message = f"Model checks failed with error as {e}"
             eligible = False
         if not eligible:
             return eligible, self.message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
 class TensorflowChecks:
-    def __init__(
-        self, model, model_name, message, progress_bar, image_size, batch_size
-    ):
-        self.message = message
-        self.model = model
-        self.model_name = model_name
-        self.progress_bar = progress_bar
-        self.image_size = image_size
-        self.batch_size = batch_size
+    def __init__(self, **kwargs):
+        validate_kwargs(
+            kwargs,
+            {
+                "model",
+                "model_name",
+                "message",
+                "progress_bar",
+                "image_size",
+                "batch_size",
+            },
+        )
+        self.message = kwargs["message"]
+        self.model = kwargs["model"]
+        self.model_name = kwargs["model_name"]
+        self.progress_bar = kwargs["progress_bar"]
+        self.image_size = kwargs["image_size"]
+        self.batch_size = kwargs["batch_size"]
 
     def progress_bar_update(self):
         if self.progress_bar is not None:
             self.progress_bar.update(1)
 
     def is_model_supported(self):
         """
@@ -452,23 +461,35 @@
         eligible, message = self.is_model_eligible()
         if not eligible:
             return eligible, message, None, self.progress_bar  # pragma: no cover
         return True, self.message, self.model_name, self.progress_bar
 
 
 class TorchChecks:
-    def __init__(
-        self, model, model_name, message, progress_bar, image_size, batch_size
-    ):
-        self.message = message
-        self.model = model
-        self.model_name = model_name
-        self.progress_bar = progress_bar
-        self.image_size = image_size
-        self.batch_size = batch_size
+    def __init__(self, **kwargs):
+        validate_kwargs(
+            kwargs,
+            {
+                "model",
+                "model_name",
+                "message",
+                "progress_bar",
+                "image_size",
+                "batch_size",
+                "tmp_path",
+            },
+        )
+        self.message = kwargs["message"]
+        self.model = kwargs["model"]
+        self.model_name = kwargs["model_name"]
+        self.progress_bar = kwargs["progress_bar"]
+        self.image_size = kwargs["image_size"]
+        self.batch_size = kwargs["batch_size"]
+        self.tmp_path = kwargs["tmp_path"]
+        self.average_weights_file_path = None
 
     def is_model_supported(self):
         """
         Check if model contains:
             - forward function
         """
         model = self.model
@@ -511,27 +532,89 @@
                     outputs = self.model(inputs)
                     loss = criterion(outputs, labels)
                     loss.backward()
                     optimizer.step()
 
                     # print statistics
                     running_loss += loss.item()
+            # dump weights from trained model will be used in averaging check
+            get_model_parameters(
+                model=self.model,
+                weight_file_path=self.tmp_path,
+                weights_file_name=TRAINED_WEIGHTS_FILENAME,
+            )
             self.progress_bar.update(1)
         except Exception as e:  # pragma: no cover
             self.message = f"\nModel not support training on image classification dataset as there is error {e} "
             raise
 
+    def average_weights(self):
+        weights = []
+        new_weights = []
+        no_images_array = [20, 20]
+        weights_file_path_1 = os.path.join(
+            self.tmp_path, f"{UNTRAINED_WEIGHTS_FILENAME}.pkl"
+        )
+        weights_file_path_2 = os.path.join(
+            self.tmp_path, f"{TRAINED_WEIGHTS_FILENAME}.pkl"
+        )
+        self.average_weights_file_path = os.path.join(
+            self.tmp_path, f"{AVERAGED_WEIGHTS_PATH}.pkl"
+        )
+        try:
+            with open(weights_file_path_1, "rb") as pkl_file, open(
+                weights_file_path_2, "rb"
+            ) as pkl_file2:
+                weights.append(pickle.load(pkl_file))
+                weights.append(pickle.load(pkl_file2))
+        except Exception as e:
+            raise
+        try:
+            new_weights = [
+                np.array(
+                    [
+                        np.average(np.array(w), weights=no_images_array, axis=0)
+                        for w in zip(*weights_list_tuple)
+                    ]
+                )
+                for weights_list_tuple in zip(*weights)
+            ]
+            del weights
+            del no_images_array
+        except Exception as e:
+            raise
+        try:
+            with open(self.average_weights_file_path, "wb") as f:
+                pickle.dump(new_weights, f)
+            del new_weights
+        except Exception as e:
+            raise
+
+    def load_averaged_weights(self):
+        try:
+            with open(self.average_weights_file_path, "rb") as f:
+                parameters = pickle.load(f)
+            params_dict = zip(self.model.state_dict().keys(), parameters)
+            state_dict = OrderedDict({k: torch.tensor(v) for k, v in params_dict})
+            self.model.load_state_dict(state_dict, strict=True)
+            del params_dict
+            del state_dict
+            del parameters
+        except Exception as e:
+            raise
+
     def model_func_checks(self):
         # check if model is eligible
         try:
             self.is_model_supported()
             self.progress_bar.update(2)
             self.small_training_loop()
+            self.average_weights()
+            self.load_averaged_weights()
             self.message = "all check passed"
             eligible = True
         except Exception as e:  # pragma: no cover
-            if self.message == "":
-                self.message = f"Model checks failed with error as {e}"
+            self.message = f"Model checks failed with error as {e}"
             eligible = False
         if not eligible:
             return eligible, self.message, None, self.progress_bar  # pragma: no cover
         return eligible, self.message, self.model_name, self.progress_bar
```

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/linkModelDataSet.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/linkModelDataSet.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/messages.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/messages.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/upload.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/upload.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     Parameters: modelname
 
     modelname: model file name eg: vggnet, if file name is vggnet.py
 
     """
 
     def __init__(self, modelname, token, weights=False, url=""):
+        self.model_check_class = None
+        self.progress_bar = None
         self.__modelname = ""
         self.__model_path = ""
         self.__weights_path = ""
         self.__framework = TENSORFLOW_FRAMEWORK
         self.__image_size = 224
         self.__batch_size = 16
         self.__ext = ".py"
@@ -117,33 +119,45 @@
                 print(text, "\n")
                 self.progress_bar.close()
                 return None
             loaded_model = model_checks_generic.model
             self.__framework = model_checks_generic.framework
             self.__image_size = int(model_checks_generic.image_size)
             self.__batch_size = int(model_checks_generic.batch_size)
-            model_check_class = TensorflowChecks
             if self.__framework == PYTORCH_FRAMEWORK:
-                model_check_class = TorchChecks
+                # dump weights from non-trained model will be used in averaging check
+                get_model_parameters(
+                    model=loaded_model,
+                    weight_file_path=model_checks_generic.tmp_file_path,
+                    weights_file_name=UNTRAINED_WEIGHTS_FILENAME,
+                )
+                self.model_check_class = TorchChecks(
+                    model=loaded_model,
+                    model_name=model_name,
+                    message=message,
+                    progress_bar=self.progress_bar,
+                    image_size=self.__image_size,
+                    batch_size=self.__batch_size,
+                    tmp_path=model_checks_generic.tmp_file_path,
+                )
             elif self.__framework == TENSORFLOW_FRAMEWORK:
-                model_check_class = TensorflowChecks
-            model_checks = model_check_class(
-                model=loaded_model,
-                model_name=model_name,
-                message=message,
-                progress_bar=self.progress_bar,
-                image_size=self.__image_size,
-                batch_size=self.__batch_size,
-            )
+                self.model_check_class = TensorflowChecks(
+                    model=loaded_model,
+                    model_name=model_name,
+                    message=message,
+                    progress_bar=self.progress_bar,
+                    image_size=self.__image_size,
+                    batch_size=self.__batch_size,
+                )
             (
                 status,
                 message,
                 model_name,
                 progress_bar,
-            ) = model_checks.model_func_checks()
+            ) = self.model_check_class.model_func_checks()
             if not status:
                 model_checks_generic.remove_tmp_file()
                 text = colored(
                     message,
                     "red",
                 )
                 print(text, "\n")
```

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/user.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/user.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/utils.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,31 @@
 import torch
 import torchvision
 import torchvision.transforms as transforms
 import numpy as np
 from tensorflow_datasets.testing import mock_data
 from importlib.machinery import SourceFileLoader
 import base64
+import os
 import ast
-
+import pickle
+import pickletools
 
 TENSORFLOW_FRAMEWORK = "tensorflow"
 PYTORCH_FRAMEWORK = "pytorch"
 CONSTANT = "constant"
 STANDARD = "standard"
 ADAPTIVE = "adaptive"
 CUSTOM = "custom"
 TYPE = "type"
 FUNCTION = "function"
 VALUE = "value"
+UNTRAINED_WEIGHTS_FILENAME = "untrained_weights"
+TRAINED_WEIGHTS_FILENAME = "trained_weights"
+AVERAGED_WEIGHTS_PATH = "averaged"
 
 
 def check_MyModel(filename, path):
     try:
         # check if file contains the MyModel function
         model = SourceFileLoader(filename, f"{path}").load_module()
         model.MyModel(input_shape=(500, 500, 3), classes=10)
@@ -188,7 +193,25 @@
         )
         multi_disease_model = Sequential()
         multi_disease_model.add(base_mobilenet_model)
         multi_disease_model.add(GlobalAveragePooling2D())
         multi_disease_model.add(Dropout(0.5))
         multi_disease_model.add(Dense(output_classes, activation="sigmoid"))
         return multi_disease_model
+
+
+def get_model_parameters(model, weight_file_path: str, weights_file_name: str) -> None:
+    parameters = [val.cpu().numpy() for _, val in model.state_dict().items()]
+    with open(os.path.join(weight_file_path, f"{weights_file_name}.pkl"), "wb") as f:
+        pickled = pickle.dumps(parameters)
+        optimized_pickle = pickletools.optimize(pickled)
+        f.write(optimized_pickle)
+    del parameters
+
+
+def validate_kwargs(
+    kwargs, allowed_kwargs, error_message="Keyword argument not understood:"
+):
+    """Checks that all keyword arguments are in the set of allowed keys."""
+    for kwarg in kwargs:
+        if kwarg not in allowed_kwargs:
+            raise TypeError(error_message, kwarg)
```

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package/weights.py` & `tracebloc_package-dev-0.5.0/tracebloc_package/weights.py`

 * *Files identical despite different names*

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/PKG-INFO` & `tracebloc_package-dev-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: tracebloc-package-dev
-Version: 0.4.9
+Name: tracebloc_package-dev
+Version: 0.5.0
 Summary: Package required to run Tracebloc jupyter notebook to create experiment
 Home-page: https://gitlab.com/tracebloc/tracebloc-py-package/-/tree/dev
 Author: Tracebloc
 Author-email: info@tracebloc.io
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3
```

### Comparing `tracebloc_package-dev-0.4.9/tracebloc_package_dev.egg-info/SOURCES.txt` & `tracebloc_package-dev-0.5.0/tracebloc_package_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

