# Comparing `tmp/krakatoa-0.0.5.post6.tar.gz` & `tmp/krakatoa-0.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakatoa-0.0.5.post6.tar", last modified: Thu Jun 22 19:50:02 2023, max compression
+gzip compressed data, was "krakatoa-0.0.5a1.tar", last modified: Tue Dec 27 19:54:13 2022, max compression
```

## Comparing `krakatoa-0.0.5.post6.tar` & `krakatoa-0.0.5a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 19:50:02.666823 krakatoa-0.0.5.post6/
--rw-rw-rw-   0        0        0     1084 2022-12-27 18:23:30.000000 krakatoa-0.0.5.post6/LICENSE
--rw-rw-rw-   0        0        0      888 2023-06-22 19:50:02.667817 krakatoa-0.0.5.post6/PKG-INFO
--rw-rw-rw-   0        0        0      448 2022-12-27 18:23:30.000000 krakatoa-0.0.5.post6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 19:50:02.623817 krakatoa-0.0.5.post6/krakatoa/
--rw-rw-rw-   0        0        0      363 2022-12-27 18:23:30.000000 krakatoa-0.0.5.post6/krakatoa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:50:02.646819 krakatoa-0.0.5.post6/krakatoa/future/
--rw-rw-rw-   0        0        0      420 2022-12-27 19:22:04.000000 krakatoa-0.0.5.post6/krakatoa/future/__init__.py
--rw-rw-rw-   0        0        0     5018 2023-06-22 18:04:27.000000 krakatoa-0.0.5.post6/krakatoa/future/analysis.py
--rw-rw-rw-   0        0        0      966 2022-12-27 19:21:04.000000 krakatoa-0.0.5.post6/krakatoa/future/evaluate.py
--rw-rw-rw-   0        0        0     1584 2022-12-27 19:21:04.000000 krakatoa-0.0.5.post6/krakatoa/future/experiment.py
--rw-rw-rw-   0        0        0     8196 2022-12-28 14:07:17.000000 krakatoa-0.0.5.post6/krakatoa/future/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:50:02.660820 krakatoa-0.0.5.post6/krakatoa/models/
--rw-rw-rw-   0        0        0      360 2022-12-27 18:23:30.000000 krakatoa-0.0.5.post6/krakatoa/models/__init__.py
--rw-rw-rw-   0        0        0    29218 2022-12-27 19:21:04.000000 krakatoa-0.0.5.post6/krakatoa/models/_config.py
--rw-rw-rw-   0        0        0     1208 2022-12-27 19:21:04.000000 krakatoa-0.0.5.post6/krakatoa/models/_getmodels.py
--rw-rw-rw-   0        0        0     2370 2022-12-27 19:21:04.000000 krakatoa-0.0.5.post6/krakatoa/models/_metrics.py
--rw-rw-rw-   0        0        0    21564 2022-12-27 19:21:04.000000 krakatoa-0.0.5.post6/krakatoa/models/autotune.py
--rw-rw-rw-   0        0        0     8537 2022-12-27 19:21:04.000000 krakatoa-0.0.5.post6/krakatoa/models/quick.py
-drwxrwxrwx   0        0        0        0 2023-06-22 19:50:02.632818 krakatoa-0.0.5.post6/krakatoa.egg-info/
--rw-rw-rw-   0        0        0      888 2023-06-22 19:50:02.000000 krakatoa-0.0.5.post6/krakatoa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-06-22 19:50:02.000000 krakatoa-0.0.5.post6/krakatoa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:50:02.000000 krakatoa-0.0.5.post6/krakatoa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-06-22 19:50:02.000000 krakatoa-0.0.5.post6/krakatoa.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2023-06-22 19:50:02.000000 krakatoa-0.0.5.post6/krakatoa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-22 19:50:02.668815 krakatoa-0.0.5.post6/setup.cfg
--rw-rw-rw-   0        0        0     1184 2023-06-22 19:40:58.000000 krakatoa-0.0.5.post6/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.265231 krakatoa-0.0.5a1/
+-rw-rw-rw-   0        0        0     1084 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/LICENSE
+-rw-rw-rw-   0        0        0      728 2022-12-27 19:54:13.265231 krakatoa-0.0.5a1/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/README.md
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.250219 krakatoa-0.0.5a1/krakatoa/
+-rw-rw-rw-   0        0        0      363 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/krakatoa/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.257219 krakatoa-0.0.5a1/krakatoa/future/
+-rw-rw-rw-   0        0        0      420 2022-12-27 19:22:04.000000 krakatoa-0.0.5a1/krakatoa/future/__init__.py
+-rw-rw-rw-   0        0        0     4992 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/analysis.py
+-rw-rw-rw-   0        0        0      966 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/evaluate.py
+-rw-rw-rw-   0        0        0     1584 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/experiment.py
+-rw-rw-rw-   0        0        0     8192 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/future/preprocess.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.262219 krakatoa-0.0.5a1/krakatoa/models/
+-rw-rw-rw-   0        0        0      360 2022-12-27 18:23:30.000000 krakatoa-0.0.5a1/krakatoa/models/__init__.py
+-rw-rw-rw-   0        0        0    29218 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/_config.py
+-rw-rw-rw-   0        0        0     1208 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/_getmodels.py
+-rw-rw-rw-   0        0        0     2370 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/_metrics.py
+-rw-rw-rw-   0        0        0    21564 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/autotune.py
+-rw-rw-rw-   0        0        0     8537 2022-12-27 19:21:04.000000 krakatoa-0.0.5a1/krakatoa/models/quick.py
+drwxrwxrwx   0        0        0        0 2022-12-27 19:54:13.254219 krakatoa-0.0.5a1/krakatoa.egg-info/
+-rw-rw-rw-   0        0        0      728 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       41 2022-12-27 19:54:13.000000 krakatoa-0.0.5a1/krakatoa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2022-12-27 19:54:13.266229 krakatoa-0.0.5a1/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2022-12-27 19:53:57.000000 krakatoa-0.0.5a1/setup.py
```

### Comparing `krakatoa-0.0.5.post6/LICENSE` & `krakatoa-0.0.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa/future/analysis.py` & `krakatoa-0.0.5a1/krakatoa/future/analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import pandas as pd
 import numpy as np
 from .preprocess import DataClean
 
 #============================================================
 class Analytics(DataClean):
 
-    def __init__(self, target, mode):
-        super().__init__(target, mode)
+    def __init__(self):
+        super().__init__()
         pass
 
     def loadDataset(self, dataset, load_from="dataframe"):
         if load_from == "dataframe":
             self.dataset = dataset
             self.originalDataset = dataset
         elif load_from == "dict":
```

### Comparing `krakatoa-0.0.5.post6/krakatoa/future/evaluate.py` & `krakatoa-0.0.5a1/krakatoa/future/evaluate.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa/future/experiment.py` & `krakatoa-0.0.5a1/krakatoa/future/experiment.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa/future/preprocess.py` & `krakatoa-0.0.5a1/krakatoa/future/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         # Instancia e fit one hot encoder
         hot = OneHotEncoder(handle_unknown='ignore', sparse=False)
         hot.fit(self.dataset[cat_cols])
 
         hot_ds = hot.transform(self.dataset[cat_cols])
 
         # Cria dataframe transformada
-        hot_df = pd.DataFrame(hot_ds, columns = hot.get_feature_names_out(input_features=cat_cols))
+        hot_df = pd.DataFrame(hot_ds, columns = hot.get_feature_names(input_features=cat_cols))
 
         # Concatena o dataframe do one hot com o original
         concat_df = pd.concat([self.dataset, hot_df], axis=1).drop(columns=cat_cols, axis=1)
         self.oneHotEncoding = hot
         self.dataset = concat_df
 
         return self.dataset
```

### Comparing `krakatoa-0.0.5.post6/krakatoa/models/_config.py` & `krakatoa-0.0.5a1/krakatoa/models/_config.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa/models/_getmodels.py` & `krakatoa-0.0.5a1/krakatoa/models/_getmodels.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa/models/_metrics.py` & `krakatoa-0.0.5a1/krakatoa/models/_metrics.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa/models/autotune.py` & `krakatoa-0.0.5a1/krakatoa/models/autotune.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa/models/quick.py` & `krakatoa-0.0.5a1/krakatoa/models/quick.py`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/krakatoa.egg-info/SOURCES.txt` & `krakatoa-0.0.5a1/krakatoa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krakatoa-0.0.5.post6/setup.py` & `krakatoa-0.0.5a1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from setuptools import setup
 
 setup(
   name = 'krakatoa',       
   packages = ['krakatoa', 'krakatoa/models', 'krakatoa/future'],  
-  version = '0.0.5post6',      
+  version = '0.0.5a1',      
   license='MIT',        
   description = 'Machine Learning high level package.',  
-  long_description='Machine Learning high level package.',  
   author = 'Matheus de Prá Andrade',              
   author_email = 'mpandrade@ucs.br',    
   url = 'https://github.com/aitec-mp/krakatoa',  
-  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.5post6.tar.gz',    
+  download_url = 'https://github.com/aitec-mp/krakatoa/archive/refs/tags/0.0.5.tar.gz',    
   keywords = ['krakatoa', 'machine learning'],  
   install_requires=[    
-          'scikit-learn',
+          'sklearn',
           'numpy',
           'pandas',
           'xgboost'
       ],
   classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Developers',  
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
-    'Programming Language :: Python :: 3.10',
-    'Programming Language :: Python :: 3.11',
   ],
 )
```

