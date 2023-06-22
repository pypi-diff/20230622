# Comparing `tmp/gingado-0.1.2.tar.gz` & `tmp/gingado-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gingado-0.1.2.tar", last modified: Mon Jan  9 21:08:47 2023, max compression
+gzip compressed data, was "gingado-0.1.3.tar", last modified: Thu Jun 22 11:43:46 2023, max compression
```

## Comparing `gingado-0.1.2.tar` & `gingado-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 douglasaraujo   (501) staff       (20)        0 2023-01-09 21:08:47.877517 gingado-0.1.2/
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     2330 2022-11-09 20:12:46.000000 gingado-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 douglasaraujo   (501) staff       (20)    11357 2022-05-11 22:37:56.000000 gingado-0.1.2/LICENSE
--rw-r--r--   0 douglasaraujo   (501) staff       (20)      153 2022-09-17 22:48:20.000000 gingado-0.1.2/MANIFEST.in
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     5074 2023-01-09 21:08:47.877217 gingado-0.1.2/PKG-INFO
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     4246 2022-11-10 13:37:47.000000 gingado-0.1.2/README.md
-drwxr-xr-x   0 douglasaraujo   (501) staff       (20)        0 2023-01-09 21:08:47.873966 gingado-0.1.2/gingado/
--rw-r--r--   0 douglasaraujo   (501) staff       (20)       22 2023-01-09 20:03:24.000000 gingado-0.1.2/gingado/__init__.py
--rw-r--r--   0 douglasaraujo   (501) staff       (20)    14360 2023-01-09 20:03:24.000000 gingado-0.1.2/gingado/_modidx.py
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     1084 2022-09-17 23:18:32.000000 gingado-0.1.2/gingado/_nbdev.py
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     5375 2023-01-09 20:03:24.000000 gingado-0.1.2/gingado/augmentation.py
--rw-r--r--   0 douglasaraujo   (501) staff       (20)    10747 2023-01-09 20:03:24.000000 gingado-0.1.2/gingado/benchmark.py
--rw-r--r--   0 douglasaraujo   (501) staff       (20)    44925 2023-01-09 20:03:25.000000 gingado-0.1.2/gingado/dataset_BarroLee_1994.csv
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     5803 2023-01-09 20:03:24.000000 gingado-0.1.2/gingado/datasets.py
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     9644 2023-01-09 20:03:24.000000 gingado-0.1.2/gingado/model_documentation.py
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     5468 2023-01-09 20:03:24.000000 gingado-0.1.2/gingado/utils.py
-drwxr-xr-x   0 douglasaraujo   (501) staff       (20)        0 2023-01-09 21:08:47.876774 gingado-0.1.2/gingado.egg-info/
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     5074 2023-01-09 21:08:47.000000 gingado-0.1.2/gingado.egg-info/PKG-INFO
--rw-r--r--   0 douglasaraujo   (501) staff       (20)      489 2023-01-09 21:08:47.000000 gingado-0.1.2/gingado.egg-info/SOURCES.txt
--rw-r--r--   0 douglasaraujo   (501) staff       (20)        1 2023-01-09 21:08:47.000000 gingado-0.1.2/gingado.egg-info/dependency_links.txt
--rw-r--r--   0 douglasaraujo   (501) staff       (20)       57 2023-01-09 21:08:47.000000 gingado-0.1.2/gingado.egg-info/entry_points.txt
--rw-r--r--   0 douglasaraujo   (501) staff       (20)        1 2022-05-27 20:07:24.000000 gingado-0.1.2/gingado.egg-info/not-zip-safe
--rw-r--r--   0 douglasaraujo   (501) staff       (20)      146 2023-01-09 21:08:47.000000 gingado-0.1.2/gingado.egg-info/requires.txt
--rw-r--r--   0 douglasaraujo   (501) staff       (20)        8 2023-01-09 21:08:47.000000 gingado-0.1.2/gingado.egg-info/top_level.txt
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     1330 2023-01-09 19:56:01.000000 gingado-0.1.2/settings.ini
--rw-r--r--   0 douglasaraujo   (501) staff       (20)       38 2023-01-09 21:08:47.877611 gingado-0.1.2/setup.cfg
--rw-r--r--   0 douglasaraujo   (501) staff       (20)     2541 2022-11-09 20:12:47.000000 gingado-0.1.2/setup.py
+drwxr-xr-x   0 douglasaraujo   (501) staff       (20)        0 2023-06-22 11:43:46.985129 gingado-0.1.3/
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     2330 2022-11-09 20:12:46.000000 gingado-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)    11357 2022-05-11 22:37:56.000000 gingado-0.1.3/LICENSE
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)      153 2022-09-17 22:48:20.000000 gingado-0.1.3/MANIFEST.in
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     5074 2023-06-22 11:43:46.984884 gingado-0.1.3/PKG-INFO
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     4246 2022-11-10 13:37:47.000000 gingado-0.1.3/README.md
+drwxr-xr-x   0 douglasaraujo   (501) staff       (20)        0 2023-06-22 11:43:46.982164 gingado-0.1.3/gingado/
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)       22 2023-06-22 09:46:04.000000 gingado-0.1.3/gingado/__init__.py
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)    15233 2023-06-22 09:46:04.000000 gingado-0.1.3/gingado/_modidx.py
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     1084 2022-09-17 23:18:32.000000 gingado-0.1.3/gingado/_nbdev.py
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     6739 2023-06-22 09:46:04.000000 gingado-0.1.3/gingado/augmentation.py
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)    11623 2023-06-22 09:46:04.000000 gingado-0.1.3/gingado/benchmark.py
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)    44925 2023-06-18 09:49:40.000000 gingado-0.1.3/gingado/dataset_BarroLee_1994.csv
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     5803 2023-06-22 09:46:04.000000 gingado-0.1.3/gingado/datasets.py
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)    15198 2023-06-22 09:46:04.000000 gingado-0.1.3/gingado/model_documentation.py
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     5468 2023-06-22 09:46:04.000000 gingado-0.1.3/gingado/utils.py
+drwxr-xr-x   0 douglasaraujo   (501) staff       (20)        0 2023-06-22 11:43:46.984515 gingado-0.1.3/gingado.egg-info/
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     5074 2023-06-22 11:43:46.000000 gingado-0.1.3/gingado.egg-info/PKG-INFO
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)      489 2023-06-22 11:43:46.000000 gingado-0.1.3/gingado.egg-info/SOURCES.txt
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)        1 2023-06-22 11:43:46.000000 gingado-0.1.3/gingado.egg-info/dependency_links.txt
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)       57 2023-06-22 11:43:46.000000 gingado-0.1.3/gingado.egg-info/entry_points.txt
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)        1 2022-05-27 20:07:24.000000 gingado-0.1.3/gingado.egg-info/not-zip-safe
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)      146 2023-06-22 11:43:46.000000 gingado-0.1.3/gingado.egg-info/requires.txt
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)        8 2023-06-22 11:43:46.000000 gingado-0.1.3/gingado.egg-info/top_level.txt
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     1330 2023-06-22 09:39:39.000000 gingado-0.1.3/settings.ini
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)       38 2023-06-22 11:43:46.985216 gingado-0.1.3/setup.cfg
+-rw-r--r--   0 douglasaraujo   (501) staff       (20)     2541 2022-11-09 20:12:47.000000 gingado-0.1.3/setup.py
```

### Comparing `gingado-0.1.2/CONTRIBUTING.md` & `gingado-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gingado-0.1.2/LICENSE` & `gingado-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gingado-0.1.2/PKG-INFO` & `gingado-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gingado
-Version: 0.1.2
+Version: 0.1.3
 Summary: A machine learning library for economics and finance
 Home-page: https://github.com/dkgaraujo/gingado
 Author: Douglas K. G. de Araujo
 Author-email: Douglas.Araujo@bis.org
 License: Apache Software License 2.0
 Keywords: AI Economics Finance
 Platform: UNKNOWN
```

### Comparing `gingado-0.1.2/README.md` & `gingado-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gingado-0.1.2/gingado/_modidx.py` & `gingado-0.1.3/gingado/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,26 @@
                                    'gingado.benchmark.ggdBenchmark.score': ('benchmark.html#ggdbenchmark.score', 'gingado/benchmark.py'),
                                    'gingado.benchmark.ggdBenchmark.score_samples': ( 'benchmark.html#ggdbenchmark.score_samples',
                                                                                      'gingado/benchmark.py'),
                                    'gingado.benchmark.ggdBenchmark.set_benchmark': ( 'benchmark.html#ggdbenchmark.set_benchmark',
                                                                                      'gingado/benchmark.py')},
             'gingado.datasets': { 'gingado.datasets.load_BarroLee_1994': ('datasets.html#load_barrolee_1994', 'gingado/datasets.py'),
                                   'gingado.datasets.make_causal_effect': ('datasets.html#make_causal_effect', 'gingado/datasets.py')},
-            'gingado.model_documentation': { 'gingado.model_documentation.ModelCard': ( 'documentation.html#modelcard',
+            'gingado.model_documentation': { 'gingado.model_documentation.ForecastCard': ( 'documentation.html#forecastcard',
+                                                                                           'gingado/model_documentation.py'),
+                                             'gingado.model_documentation.ForecastCard.__init__': ( 'documentation.html#forecastcard.__init__',
+                                                                                                    'gingado/model_documentation.py'),
+                                             'gingado.model_documentation.ForecastCard.autofill_template': ( 'documentation.html#forecastcard.autofill_template',
+                                                                                                             'gingado/model_documentation.py'),
+                                             'gingado.model_documentation.ModelCard': ( 'documentation.html#modelcard',
                                                                                         'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ModelCard.__init__': ( 'documentation.html#modelcard.__init__',
                                                                                                  'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ModelCard.autofill_template': ( 'documentation.html#modelcard.autofill_template',
                                                                                                           'gingado/model_documentation.py'),
-                                             'gingado.model_documentation.ModelCard.fill_model_info': ( 'documentation.html#modelcard.fill_model_info',
-                                                                                                        'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation': ( 'documentation.html#ggdmodeldocumentation',
                                                                                                     'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.__getitem__': ( 'documentation.html#ggdmodeldocumentation.__getitem__',
                                                                                                                 'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.__repr__': ( 'documentation.html#ggdmodeldocumentation.__repr__',
                                                                                                              'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.__setitem__': ( 'documentation.html#ggdmodeldocumentation.__setitem__',
@@ -85,14 +89,16 @@
                                                                                                             'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation._read_attr': ( 'documentation.html#ggdmodeldocumentation._read_attr',
                                                                                                                'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.documentation_path': ( 'documentation.html#ggdmodeldocumentation.documentation_path',
                                                                                                                        'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.fill_info': ( 'documentation.html#ggdmodeldocumentation.fill_info',
                                                                                                               'gingado/model_documentation.py'),
+                                             'gingado.model_documentation.ggdModelDocumentation.fill_model_info': ( 'documentation.html#ggdmodeldocumentation.fill_model_info',
+                                                                                                                    'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.open_questions': ( 'documentation.html#ggdmodeldocumentation.open_questions',
                                                                                                                    'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.read_json': ( 'documentation.html#ggdmodeldocumentation.read_json',
                                                                                                               'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.read_model': ( 'documentation.html#ggdmodeldocumentation.read_model',
                                                                                                                'gingado/model_documentation.py'),
                                              'gingado.model_documentation.ggdModelDocumentation.save_json': ( 'documentation.html#ggdmodeldocumentation.save_json',
```

### Comparing `gingado-0.1.2/gingado/_nbdev.py` & `gingado-0.1.3/gingado/_nbdev.py`

 * *Files identical despite different names*

### Comparing `gingado-0.1.2/gingado/augmentation.py` & `gingado-0.1.3/gingado/augmentation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../00_augmentation.ipynb.
 
+# %% ../00_augmentation.ipynb 2
+#| include: false
+#| echo: false
+from __future__ import annotations # allows multiple typing of arguments in Python versions prior to 3.10
+
 # %% auto 0
 __all__ = ['AugmentSDMX']
 
-# %% ../00_augmentation.ipynb 6
+# %% ../00_augmentation.ipynb 7
 #| include: false
-from .utils import load_SDMX_data
 import numpy as np
 import pandas as pd
 import pandasdmx as sdmx
+
+from .utils import load_SDMX_data
 from sklearn.base import BaseEstimator, TransformerMixin
 from sklearn.utils.validation import check_is_fitted
 from sklearn.feature_selection import VarianceThreshold
 
+# %% ../00_augmentation.ipynb 8
+#| include: false
 class AugmentSDMX(BaseEstimator, TransformerMixin):
     "A transformer that augments a dataset using SDMX"
     
     InputIndexMessage = "The dataset to be augmented must have a row index with the date/time information"
     def _format_string(self):
         return "%Y-%m-%d" if self.data_freq_ == 'D' else "%Y-%m" if self.data_freq_ == 'M' else "%Y"
     
@@ -33,56 +41,73 @@
             return X
 
         if training:
             # test that the dataset `X` has the same dimension as the one
             # used during training, which is an evidence they are the same
             n_samples_in_transform, n_features_in_transform = X.shape
             if n_samples_in_transform != self.n_samples_in_ or n_features_in_transform != self.n_features_in_:
-                raise ValueError("The X passed to the transform() method must be compatible with the X used by the fit() method.")
+                raise ValueError("The `X` passed to the transform() method must be compatible with the `X` used by the fit() method.")
             # during testing, we don't want the possibility of a different
             # set of columns being retained by virtue of different dynamics
             # in both datasets. For example, if a feature is included in the
             # training but during the test dates the variable didn't move, it
             # should not be subject to the test below so that it is still
             # included in the fitted data.
-            feat_sel = VarianceThreshold() if self.variance_threshold is None else VarianceThreshold(threshold=self.variance_threshold)
-            feat_sel.fit(df)
-            self.features_stay_ = df.columns[feat_sel.get_support()]
-            self.features_removed_ = df.columns[~feat_sel.get_support()]
-            
-            df = df.iloc[:, feat_sel.get_support()]
-            df.columns = feat_sel.get_feature_names_out()
-
+            self.features_stay_ = df.columns
+            self.features_removed_ = None
+            merge_df = True
+            if self.variance_threshold:
+                df_temp = df.dropna(axis=0, how='any')
+                feat_sel = VarianceThreshold(threshold=self.variance_threshold)
+                try:
+                    feat_sel.fit(df)
+                    self.features_stay_ = df.columns[feat_sel.get_support()]
+                    self.features_removed_ = df.columns[~feat_sel.get_support()]
+                    df = df.iloc[:, feat_sel.get_support()]
+                    df.columns = feat_sel.get_feature_names_out()
+                except ValueError as e:
+                    print("No columns added to original data because " + str(e).lower())
+                    merge_df = False
             df.dropna(axis=0, how='all', inplace=True)
-            df.dropna(axis=1, how='all', inplace=True)        
+            df.dropna(axis=1, how='all', inplace=True)  
+            if merge_df:
+                X = pd.merge(left=X, right=df, how='left', left_index=True, right_on='TIME_PERIOD')      
         
-        X = pd.merge(left=X, right=df, how='left', left_index=True, right_on='TIME_PERIOD')
+        if training is False: # if True, `X` would already have merged with `df` (or not if no added column)
+            X = pd.merge(left=X, right=df, how='left', left_index=True, right_on='TIME_PERIOD')
         if 'TIME_PERIOD' in X.columns:
             X.drop(columns='TIME_PERIOD', inplace=True)
         if self.propagate_last_known_value:
             X.fillna(method="ffill", inplace=True)
         if self.fillna is not None:
             X.fillna(self.fillna)
         if training:
             X.index = self.index_
         return X
 
-    def __init__(self, sources={'BIS': 'WS_CBPOL_D'}, variance_threshold=None, propagate_last_known_value=True, fillna = 0, verbose=True):
+    def __init__(
+        self,
+        sources:dict={'BIS': 'WS_CBPOL_D'}, # A dictionary with sources as keys and dataflows as values
+        variance_threshold:float|None=None, # If None (default), all variables are kept. Otherwise, variables that have a lower variance through time are removed
+        propagate_last_known_value:bool=True, # Whether the last value that is not NA should be propagated to the following dates
+        fillna:float|int = 0, # Value to use to fill missing data
+        verbose:bool=True # Whether to inform the user as the process progresses
+        ):
         self.sources = sources
         self.variance_threshold = variance_threshold
         self.propagate_last_known_value = propagate_last_known_value
         self.fillna = fillna
         self.verbose = verbose
 
     def fit(
             self,
-            X, # a pandas Series or DataFrame with an index of datetime type
+            X:pd.Series|pd.DataFrame, # Data having an index of `datetime` type
             y:None=None # `y` is kept as argument for API consistency only
         ): # A fitted version of the same AugmentSDMX instance
-        # Fits instance of AugmentSDMX to `X`, learning its time series frequency
+        "Fits instance of AugmentSDMX to `X`, learning its time series frequency"
         
         try:
             self.data_freq_ = X.index.to_series().diff().min().resolution_string
         except AttributeError:
             print(self.InputIndexMessage)
             raise
         self.index_ = X.index
@@ -93,29 +118,29 @@
         # if `fit` and `transform` are called separately with the same `X`
         self.n_samples_in_ = X.shape[0]
 
         return self
 
     def transform(
             self,
-            X, # a pandas Series or DataFrame with an index of datetime type
+            X:pd.Series|pd.DataFrame, # Data having an index of `datetime` type
             y:None=None, # `y` is kept as argument for API consistency only
-            training=False # `True` is `transform` is called during training; `False` if called during testing
-        ): # `X` augmented with data from SDMX
-        # Transforms input dataset `X` by adding the requested data using SDMX
+            training:bool=False # `True` if `transform` is called during training, `False` (default) if called during testing
+        ) -> np.ndarray: # `X` augmented with data from SDMX with the same number of samples but more columns
+        "Transforms input dataset `X` by adding the requested data using SDMX"
         check_is_fitted(self)
         self.params_ = self._get_dates()
         idx = X.index
         transf_X = self._transform(X, training=training)
         transf_X.index = idx
         return transf_X
 
     def fit_transform(
             self, 
-            X, # # a pandas Series or DataFrame with an index of datetime type
+            X:pd.Series|pd.DataFrame, # Data having an index of `datetime` type
             y:None=None # `y` is kept as argument for API consistency only
             ) -> np.ndarray: # `X` augmented with data from SDMX with the same number of samples but more columns
-        # Fit to data, then transform it.
+        "Fit to data, then transform it."
         
         self.fit(X)
         self.params_ = self._get_dates()
         return self.transform(X, training=True)
```

### Comparing `gingado-0.1.2/gingado/benchmark.py` & `gingado-0.1.3/gingado/benchmark.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../00_benchmark.ipynb.
 
+# %% ../00_benchmark.ipynb 2
+#| include: false
+#| echo: false
+from __future__ import annotations # allows multiple typing of arguments in Python versions prior to 3.10
+
 # %% auto 0
 __all__ = ['ggdBenchmark', 'ClassificationBenchmark', 'RegressionBenchmark']
 
-# %% ../00_benchmark.ipynb 7
+# %% ../00_benchmark.ipynb 9
 #| include: false
 import numpy as np
 import pandas as pd
 from sklearn.base import BaseEstimator
 from sklearn.model_selection import TimeSeriesSplit, GridSearchCV
 from sklearn.pipeline import Pipeline
 from sklearn.utils.metaestimators import available_if
 from sklearn.utils.validation import check_is_fitted
 from .model_documentation import ggdModelDocumentation, ModelCard
 
+# %% ../00_benchmark.ipynb 10
+#| include: false
 def _benchmark_has(attr):
     # Check if the benchmark has certain attributes
     def check(self):
         getattr(self.benchmark, attr)
         return True
     return check
         
@@ -150,60 +157,69 @@
                     model_attr = self.benchmark.__getattribute__(a)
                     yield {a: model_attr}
                 except:
                     pass
 
     def document(
         self, 
-        documenter=None # A gingado Documenter or the documenter set in `auto_document` if None.
+        documenter:ggdModelDocumentation|None=None # A gingado Documenter or the documenter set in `auto_document` if None.
         ):
         "Document the benchmark model using the template in `documenter`"
         documenter = self.auto_document if documenter is None else documenter
         self.model_documentation = documenter()
         model_info = list(self._read_attr())
         model_info = {k:v for i in model_info for k, v in i.items()}
         #self.model_documentation.read_model(self.benchmark)
         self.model_documentation.fill_model_info(model_info)
 
     @available_if(_benchmark_has("predict"))
     def predict(self, X, **predict_params):
+        "Note: only available if the benchmark implements this method."
         return self.benchmark.predict(X, **predict_params)
 
     @available_if(_benchmark_has("fit_predict"))
     def fit_predict(self, X, y=None, **predict_params):
+        "Note: only available if the benchmark implements this method."
         return self.benchmark.fit_predict(X, y, **predict_params)
 
     @available_if(_benchmark_has("predict_proba"))
     def predict_proba(self, X, **predict_proba_params):
+        "Note: only available if the benchmark implements this method."
         return self.benchmark.predict_proba(X, **predict_proba_params)
 
     @available_if(_benchmark_has("decision_function"))
     def decision_function(self, X):
+        "Note: only available if the benchmark implements this method."
         return self.benchmark.decision_function(X)
 
     @available_if(_benchmark_has("score"))
     def score(self, X):
+        "Note: only available if the benchmark implements this method."
         return self.benchmark.score(X)
 
     @available_if(_benchmark_has("score_samples"))
     def score_samples(self, X):
+        "Note: only available if the benchmark implements this method."
         return self.benchmark.score_samples(X)
 
     @available_if(_benchmark_has("predict_log_proba"))
     def predict_log_proba(self, X, **predict_log_proba_params):
+        "Note: only available if the benchmark implements this method."
         return self.benchmark.predict_log_proba(X, **predict_log_proba_params)
 
-# %% ../00_benchmark.ipynb 12
+# %% ../00_benchmark.ipynb 23
 #| include: false
 import numpy as np
 from .model_documentation import ModelCard
 from sklearn.base import ClassifierMixin
 from sklearn.model_selection import StratifiedShuffleSplit, GridSearchCV
 from sklearn.ensemble import RandomForestClassifier, VotingClassifier
 
+# %% ../00_benchmark.ipynb 24
+#| include: false
 class ClassificationBenchmark(ggdBenchmark, ClassifierMixin):
     "A gingado Benchmark object used for classification tasks"
     def __init__(self, 
     cv=None, 
     default_cv = StratifiedShuffleSplit(),
     estimator=RandomForestClassifier(oob_score=True), 
     param_grid={'n_estimators': [100, 250], 'max_features': ['sqrt', 'log2', None]}, 
@@ -223,28 +239,30 @@
         self.random_state = random_state
         self.verbose_grid = verbose_grid
         self.ensemble_method = ensemble_method
         
     def fit(
         self, 
         X:np.ndarray, # Array-like data of shape (n_samples, n_features)
-        y=None # Array-like data of shape (n_samples,) or (n_samples, n_targets) or None
+        y:np.ndarray|None=None # Array-like data of shape (n_samples,) or (n_samples, n_targets) or None
         ):
         "Fit the `ClassificationBenchmark` model"
         self._fit(X, y)
         return self
 
-# %% ../00_benchmark.ipynb 23
+# %% ../00_benchmark.ipynb 35
 #| include: false
 import numpy as np
 from .model_documentation import ModelCard
 from sklearn.base import RegressorMixin
 from sklearn.ensemble import RandomForestRegressor, VotingRegressor
 from sklearn.model_selection import ShuffleSplit, GridSearchCV
 
+# %% ../00_benchmark.ipynb 36
+#| include: false
 class RegressionBenchmark(ggdBenchmark, RegressorMixin):
     "A gingado Benchmark object used for regression tasks"
     def __init__(self, 
     cv=None, 
     default_cv=ShuffleSplit(),
     estimator=RandomForestRegressor(oob_score=True), 
     param_grid={'n_estimators': [100, 250], 'max_features': ['sqrt', 'log2', None]}, 
@@ -264,12 +282,12 @@
         self.random_state = random_state
         self.verbose_grid = verbose_grid
         self.ensemble_method = ensemble_method
 
     def fit(
         self, 
         X:np.ndarray, # Array-like data of shape (n_samples, n_features)
-        y=None # Array-like data of shape (n_samples,) or (n_samples, n_targets) or None
+        y:np.ndarray|None=None # Array-like data of shape (n_samples,) or (n_samples, n_targets) or None
         ):
         "Fit the `RegressionBenchmark` model"
         self._fit(X, y)
         return self
```

### Comparing `gingado-0.1.2/gingado/dataset_BarroLee_1994.csv` & `gingado-0.1.3/gingado/dataset_BarroLee_1994.csv`

 * *Files identical despite different names*

### Comparing `gingado-0.1.2/gingado/datasets.py` & `gingado-0.1.3/gingado/datasets.py`

 * *Files identical despite different names*

### Comparing `gingado-0.1.2/gingado/utils.py` & `gingado-0.1.3/gingado/utils.py`

 * *Files identical despite different names*

### Comparing `gingado-0.1.2/gingado.egg-info/PKG-INFO` & `gingado-0.1.3/gingado.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gingado
-Version: 0.1.2
+Version: 0.1.3
 Summary: A machine learning library for economics and finance
 Home-page: https://github.com/dkgaraujo/gingado
 Author: Douglas K. G. de Araujo
 Author-email: Douglas.Araujo@bis.org
 License: Apache Software License 2.0
 Keywords: AI Economics Finance
 Platform: UNKNOWN
```

### Comparing `gingado-0.1.2/settings.ini` & `gingado-0.1.3/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 user = dkgaraujo
 description = A machine learning library for economics and finance
 keywords = AI Economics Finance
 author = Douglas K. G. de Araujo
 author_email = Douglas.Araujo@bis.org
 copyright = Douglas K. G. de Araujo
 branch = main
-version = 0.1.2
+version = 0.1.3
 min_python = 3.7
 audience = Developers
 language = English
 custom_sidebar = True
 custom_quarto_yml = True
 license = apache2
 # From 1-7: Planning Pre-Alpha Alpha Beta Production Mature Inactive
```

### Comparing `gingado-0.1.2/setup.py` & `gingado-0.1.3/setup.py`

 * *Files identical despite different names*

