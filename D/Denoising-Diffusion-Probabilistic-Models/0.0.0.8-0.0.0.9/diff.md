# Comparing `tmp/Denoising_Diffusion_Probabilistic_Models-0.0.0.8-py3-none-any.whl.zip` & `tmp/Denoising_Diffusion_Probabilistic_Models-0.0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,13 @@
-Zip file size: 1913 bytes, number of entries: 6
--rw-r--r--  2.0 unx      137 b- defN 23-Jun-20 11:32 diffusion/Test.py
--rw-r--r--  2.0 unx       61 b- defN 23-Jun-20 11:32 diffusion/__init__.py
--rw-r--r--  2.0 unx      432 b- defN 23-Jun-20 11:32 Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-20 11:32 Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-20 11:32 Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      586 b- defN 23-Jun-20 11:32 Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/RECORD
-6 files, 1318 bytes uncompressed, 823 bytes compressed:  37.6%
+Zip file size: 9550 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     6478 b- defN 23-Jun-22 12:34 diffusion/DMFunctions.py
+-rw-r--r--  2.0 unx    10044 b- defN 23-Jun-22 12:34 diffusion/Network.py
+-rw-r--r--  2.0 unx     1115 b- defN 23-Jun-22 12:34 diffusion/Scheduler.py
+-rw-r--r--  2.0 unx      148 b- defN 23-Jun-22 12:34 diffusion/Test.py
+-rw-r--r--  2.0 unx     3459 b- defN 23-Jun-22 12:34 diffusion/Train.py
+-rw-r--r--  2.0 unx      187 b- defN 23-Jun-22 12:34 diffusion/__init__.py
+-rw-r--r--  2.0 unx      355 b- defN 23-Jun-22 12:34 diffusion/diffusion_process.py
+-rw-r--r--  2.0 unx      432 b- defN 23-Jun-22 12:34 Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 12:34 Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-22 12:34 Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      986 b- defN 23-Jun-22 12:34 Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/RECORD
+11 files, 23306 bytes uncompressed, 7852 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -1,19 +1,34 @@
+Filename: diffusion/DMFunctions.py
+Comment: 
+
+Filename: diffusion/Network.py
+Comment: 
+
+Filename: diffusion/Scheduler.py
+Comment: 
+
 Filename: diffusion/Test.py
 Comment: 
 
+Filename: diffusion/Train.py
+Comment: 
+
 Filename: diffusion/__init__.py
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/METADATA
+Filename: diffusion/diffusion_process.py
+Comment: 
+
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/WHEEL
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/top_level.txt
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.8.dist-info/RECORD
+Filename: Denoising_Diffusion_Probabilistic_Models-0.0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## diffusion/Test.py

```diff
@@ -1,10 +1,10 @@
 print('Test')
 class Test():
   def __init__(self):
-    print('Test1')
+    pass
 
   def test(self):
-    print('Test2')
+    print('Hello world!')
 
-def f1():
-  print('test f1')
+def function():
+  print('Function is ok.')
```

## diffusion/__init__.py

```diff
@@ -1,3 +1,7 @@
 import sys
-sys.path.append('../')
-from .Test import Test, f1
+sys.path.append('./')
+from .Test import Test, function
+from .DMFunctions import DMFunctions
+from .Network import Unet
+from .Scheduler import Scheduler
+from .Train import Train
```

