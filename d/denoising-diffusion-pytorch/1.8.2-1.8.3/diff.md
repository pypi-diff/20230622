# Comparing `tmp/denoising-diffusion-pytorch-1.8.2.tar.gz` & `tmp/denoising-diffusion-pytorch-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.8.2.tar", last modified: Wed Jun 21 14:03:43 2023, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.8.3.tar", last modified: Thu Jun 22 15:50:42 2023, max compression
```

## Comparing `denoising-diffusion-pytorch-1.8.2.tar` & `denoising-diffusion-pytorch-1.8.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    36175 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    29665 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 14:03:43.000000 denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 14:03:43.802075 denoising-diffusion-pytorch-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-21 14:03:32.000000 denoising-diffusion-pytorch-1.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10547 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27823 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8811 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36175 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29929 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9203 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35629 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21236 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5780 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 15:50:42.000000 denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 15:50:42.405177 denoising-diffusion-pytorch-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-22 15:50:31.000000 denoising-diffusion-pytorch-1.8.3/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.8.2/LICENSE` & `denoising-diffusion-pytorch-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/PKG-INFO` & `denoising-diffusion-pytorch-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.2
+Version: 1.8.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.2/README.md` & `denoising-diffusion-pytorch-1.8.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     image_size = 128,
     timesteps = 1000    # number of steps
 )
 
 training_images = torch.rand(8, 3, 128, 128) # images are normalized from 0 to 1
 loss = diffusion(training_images)
 loss.backward()
+
 # after a lot of training
 
 sampled_images = diffusion.sample(batch_size = 4)
 sampled_images.shape # (4, 3, 128, 128)
 ```
 
 Or, if you simply want to pass in a folder name and the desired image dimensions, you can use the `Trainer` class to easily train a model.
```

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,9 +2,8 @@
 
 from denoising_diffusion_pytorch.learned_gaussian_diffusion import LearnedGaussianDiffusion
 from denoising_diffusion_pytorch.continuous_time_gaussian_diffusion import ContinuousTimeGaussianDiffusion
 from denoising_diffusion_pytorch.weighted_objective_gaussian_diffusion import WeightedObjectiveGaussianDiffusion
 from denoising_diffusion_pytorch.elucidated_diffusion import ElucidatedDiffusion
 from denoising_diffusion_pytorch.v_param_continuous_time_gaussian_diffusion import VParamContinuousTimeGaussianDiffusion
 
-from denoising_diffusion_pytorch.denoising_diffusion_pytorch_1d import GaussianDiffusion1D, Unet1D, Trainer1D
-
+from denoising_diffusion_pytorch.denoising_diffusion_pytorch_1d import GaussianDiffusion1D, Unet1D, Trainer1D, Dataset1D
```

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import math
-from multiprocessing import cpu_count
 from pathlib import Path
 from random import random
 from functools import partial
 from collections import namedtuple
+from multiprocessing import cpu_count
 
 import torch
-from accelerate import Accelerator
-from ema_pytorch import EMA
-from torch import nn, einsum
+from torch import nn, einsum, Tensor
 import torch.nn.functional as F
 from torch.cuda.amp import autocast
+from torch.optim import Adam
+from torch.utils.data import Dataset, DataLoader
 
 from einops import rearrange, reduce
 from einops.layers.torch import Rearrange
-from torch.optim import Adam
-from torch.utils.data import Dataset, DataLoader
+
+from accelerate import Accelerator
+from ema_pytorch import EMA
 
 from tqdm.auto import tqdm
 
 from denoising_diffusion_pytorch.version import __version__
 
 # constants
 
@@ -63,14 +64,27 @@
 
 def normalize_to_neg_one_to_one(img):
     return img * 2 - 1
 
 def unnormalize_to_zero_to_one(t):
     return (t + 1) * 0.5
 
+# data
+
+class Dataset1D(Dataset):
+    def __init__(self, tensor: Tensor):
+        super().__init__()
+        self.tensor = tensor.clone()
+
+    def __len__(self):
+        return len(self.tensor)
+
+    def __getitem__(self, idx):
+        return self.tensor[idx].clone()
+
 # small helper modules
 
 class Residual(nn.Module):
     def __init__(self, fn):
         super().__init__()
         self.fn = fn
 
@@ -710,28 +724,26 @@
         ema_update_every = 10,
         ema_decay = 0.995,
         adam_betas = (0.9, 0.99),
         save_and_sample_every = 1000,
         num_samples = 25,
         results_folder = './results',
         amp = False,
-        fp16 = False,
+        mixed_precision_type = 'fp16',
         split_batches = True,
     ):
         super().__init__()
 
         # accelerator
 
         self.accelerator = Accelerator(
             split_batches = split_batches,
-            mixed_precision = 'fp16' if fp16 else 'no'
+            mixed_precision = mixed_precision_type if amp else 'no'
         )
 
-        self.accelerator.native_amp = amp
-
         # model
 
         self.model = diffusion_model
         self.channels = diffusion_model.channels
 
         # sampling and training hyperparameters
```

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.8.2
+Version: 1.8.3
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.8.2/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.8.3/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.8.2/setup.py` & `denoising-diffusion-pytorch-1.8.3/setup.py`

 * *Files identical despite different names*

