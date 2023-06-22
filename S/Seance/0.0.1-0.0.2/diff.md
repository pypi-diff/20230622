# Comparing `tmp/Seance-0.0.1-py3-none-any.whl.zip` & `tmp/Seance-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15117 bytes, number of entries: 16
+Zip file size: 15260 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat     2360 b- defN 23-Jun-21 13:29 Seance/Explainer.py
--rw-rw-rw-  2.0 fat    11025 b- defN 23-Jun-22 14:34 Seance/Forecaster.py
--rw-rw-rw-  2.0 fat     9474 b- defN 23-Jun-21 22:41 Seance/Optimizer.py
+-rw-rw-rw-  2.0 fat    11262 b- defN 23-Jun-22 19:52 Seance/Forecaster.py
+-rw-rw-rw-  2.0 fat     9882 b- defN 23-Jun-22 19:52 Seance/Optimizer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:41 Seance/__init__.py
 -rw-rw-rw-  2.0 fat     3358 b- defN 23-May-18 13:18 Seance/Builder/PanelAxis.py
 -rw-rw-rw-  2.0 fat     3990 b- defN 23-May-18 13:16 Seance/Builder/PreProcess.py
 -rw-rw-rw-  2.0 fat     6595 b- defN 23-May-31 15:17 Seance/Builder/Transformations.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:40 Seance/Builder/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-Jun-03 01:07 Seance/basis_functions/__init__.py
 -rw-rw-rw-  2.0 fat      865 b- defN 23-May-27 00:20 Seance/basis_functions/fourier_basis.py
 -rw-rw-rw-  2.0 fat     2834 b- defN 23-May-31 21:10 Seance/basis_functions/linear_basis.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-22 14:38 Seance-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2676 b- defN 23-Jun-22 14:38 Seance-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 14:38 Seance-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-22 14:38 Seance-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1302 b- defN 23-Jun-22 14:38 Seance-0.0.1.dist-info/RECORD
-16 files, 45746 bytes uncompressed, 12969 bytes compressed:  71.6%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2684 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1302 b- defN 23-Jun-22 19:52 Seance-0.0.2.dist-info/RECORD
+16 files, 46399 bytes uncompressed, 13112 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: Seance/basis_functions/fourier_basis.py
 Comment: 
 
 Filename: Seance/basis_functions/linear_basis.py
 Comment: 
 
-Filename: Seance-0.0.1.dist-info/LICENSE
+Filename: Seance-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: Seance-0.0.1.dist-info/METADATA
+Filename: Seance-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Seance-0.0.1.dist-info/WHEEL
+Filename: Seance-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Seance-0.0.1.dist-info/top_level.txt
+Filename: Seance-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Seance-0.0.1.dist-info/RECORD
+Filename: Seance-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Seance/Forecaster.py

```diff
@@ -114,14 +114,15 @@
                                                    seasonal_period=i,
                                                    fourier_order=self.fourier_order)
                 column_names = [f'{i}_fourier_{j+1}' for j in range(2 * self.fourier_order)]
                 fourier_basis = pd.DataFrame(fourier_basis, columns=column_names)
                 seasonal_df.append(fourier_basis)
             seasonal_df = pd.concat(seasonal_df)
             seasonal_df[date_column] = self.time_periods.values
+            seasonal_df[date_column] = pd.to_datetime(seasonal_df[date_column]).dt.tz_localize(None)
             max_period = max(self.seasonal_period)
         else:
             max_period = None
 
         if differences is not None:
             if not isinstance(differences, list):
                 differences = [differences]
@@ -132,14 +133,15 @@
                                           linear_trend=linear_trend,
                                           linear_test_window=linear_test_window,
                                           seasonal_period=max_period,
                                           outlier_cap=outlier_cap,
                                           run_dict=self.run_dict)
         self.processed_df = self.processor.process(df)
         self.processed_df = self.processed_df.sort_values(['Seance ID', date_column])
+        self.processed_df[date_column] = self.processed_df[date_column].dt.tz_localize(None)
         if self.n_basis is not None and self.n_basis:
             self.basis_list = []
             basis = self.processed_df.groupby('Seance ID')[target_column].apply(self.linear_basis)
             self.processed_df = pd.concat([self.processed_df, basis], axis=1)
         if self.seasonal_period is not None:
             self.processed_df = self.processed_df.merge(seasonal_df, on=date_column)
         self.processed_df['cat_id_col'] = self.processed_df['Seance ID'].copy()
@@ -189,14 +191,15 @@
         return df
 
     def predict(self, forecast_horizon):
         self.forecast_horizon = forecast_horizon
         dates = pd.date_range(start=self.time_periods.iloc[-1],
                               freq=self.freq,
                               periods=forecast_horizon + 1)[1:]
+        dates = dates.tz_localize(None)
         future_dates = pd.DataFrame(dates,
                                     columns=[self.date_column])
         id_df = self.run_dict['global']['ID Mapping']
         pred_X = pd.merge(id_df, future_dates, how='cross')
         if self.seasonal_period is not None:
             seasonal_df = []
             for i in self.seasonal_period:
@@ -230,10 +233,8 @@
         return predicted
 
     def plot_importance(self, max_num_features=20):
         lgb.plot_importance(self.mlforecast.models_['LGBMRegressor'],
                             max_num_features=max_num_features)
         return
 
-
-
-
+
```

## Seance/Optimizer.py

```diff
@@ -2,14 +2,15 @@
 from sklearn.model_selection import TimeSeriesSplit
 from sklearn.metrics import mean_squared_error
 import time
 import numpy as np
 import optuna
 from numba import njit
 import numpy as np
+import pandas as pd
 from Seance.Forecaster import Forecaster
 # optuna.logging.set_verbosity(optuna.logging.WARNING)
 
 
 @njit
 def smape(A, F):
     return 100/len(A) * np.sum(2 * np.abs(F - A) / (0.0001 + (np.abs(A) + np.abs(F))))
@@ -60,14 +61,15 @@
     #         self.seasonal_period = 0
 
     def get_splits(self, df, id_column):
         df['test_split'] = df.groupby(id_column).cumcount()+1
         df['len'] = df.groupby(id_column)[self.date_column].transform('size')
         df['test_split'] = ((df['test_split'] - self.test_size > self.test_size) & (df['test_split'] > df['len'] - self.test_size))
         self.train_df = df[df['test_split'] == False]
+        # self.train_df[self.date_column] = pd.to_datetime(self.train_df[self.date_column]).dt.
         self.test_df = df[df['test_split'] == True]
 
     def scorer(self, params, metric):
         scores = []
         # for train_index, test_index in cv_splits:
         try:
             model_obj = Forecaster()
@@ -75,26 +77,30 @@
                           target_column=self.target_column,
                           date_column=self.date_column,
                           id_column=self.id_column,
                           freq=self.freq,
                           **params)
             predicted = model_obj.predict(self.test_size)
             self.predicted = predicted
-            assert len(predicted) == len(self.test_df), 'Predicted not the same size as test set'
+            if len(predicted) != len(self.test_df):
+                print('Predicted not the same size as test set')
     
             if any(np.isnan(predicted['LGBMRegressor'])):
                 scores.append(np.inf)
             else:
+                # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
+                self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
                 self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
                 if metric == 'mse':
                     scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df['LGBMRegressor'].values))
                 elif metric == 'smape':
                     scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column))
-        except:
-            scores.append(np.inf)
+        except Exception as e:
+                scores.append(np.inf)
+                print(f'ERROR WHILE TUNING: {e}')
         return np.mean(scores)
 
 
     def objective(self, trial):
         params = {
             "n_estimators": trial.suggest_int(name="n_estimators", low=50, high=self.max_n_estimators),
             'lambda_l1': trial.suggest_float('lambda_l1', 1e-8, 10.0),
```

## Comparing `Seance-0.0.1.dist-info/LICENSE` & `Seance-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Seance-0.0.1.dist-info/METADATA` & `Seance-0.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Seance
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Wrapper around MLForecast.
 Home-page: https://github.com/tblume1992/Seance
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,lightgbm,mlforecast
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: optuna
 Requires-Dist: mlforecast
 
-#SeÃ¡nce v0.0.1
+## SeÃ¡nce v0.0.1
 
 A simple wrapper around Nixtla's MLForecast aimed at streamlining plug-and-play forecasting.
 
 A general pattern is to optimize then forecast such as:
 
 ```
 from mlforecast.utils import generate_daily_series
@@ -42,37 +42,37 @@
             test_size=10,
             # ar_lags=[list(range(1, 8))], #by default this will be done based on seasonal period
             metric='smape',
             n_trials=100)
 #returns an optuna study obj
 best_params, study = opt.fit(seed=1)
 ```
-#optuna plotting
+## optuna plotting
 ```
 import optuna
 optuna.visualization.matplotlib.plot_param_importances(study)
 ```
 ![alt text](https://github.com/tblume1992/Seance/blob/main/static/seance_param_imp.png?raw=true "Param Importance")
 Here we can see the most important parameter is (unsurprisingly) the number of lags. Followd by decay which controls the 'forgetfulness' of the basis functions.
 ```
 optuna.visualization.matplotlib.plot_optimization_history(study)
 ```
 ![alt text](https://github.com/tblume1992/Seance/blob/main/static/seance_study.png?raw=true "Study")
-#passing off best params for forecasts
+## passing off best params for forecasts
 ```
 seance = Forecaster()
 output = seance.fit(series,
                     target_column='y',
                     date_column='ds',
                     id_column='unique_id',
                     freq='D',
                     **best_params)
 predicted = seance.predict(24)
 ```
-#quick plot of the forecasts
+## quick plot of the forecasts
 ```
 import matplotlib.pyplot as plt
 plot_ser = np.append(series[series['unique_id'] == 'id_00']['y'].values,
                      predicted[predicted['unique_id'] == 'id_00']['LGBMRegressor'].values)
 plt.plot(plot_ser)
 plt.vlines(x=len(plot_ser) - 24, ymin=0, ymax=max(plot_ser), linestyle='dashed', color='red')
 plt.show()
```

## Comparing `Seance-0.0.1.dist-info/RECORD` & `Seance-0.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Seance/Explainer.py,sha256=ViUQvXZhsyrKjAscA88NOmBZEXwBl6pldjKe8IJ_fT0,2360
-Seance/Forecaster.py,sha256=kCblcH3FxayeyHin-YY0f9gTVChjYA4Qgq6LZKKOXNs,11025
-Seance/Optimizer.py,sha256=wc9VELNy4T3r0VOeH3QKCN6Qw2QhrQ3C5yFtNcSeyrk,9474
+Seance/Forecaster.py,sha256=csW12Sytquao5R2InOa5q8DASG-bCGiZjOsftVrO2uQ,11262
+Seance/Optimizer.py,sha256=McIC6ZUCAJlSFTk0LRxQ_RneOLg2VFiflr67wBXqyqs,9882
 Seance/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/Builder/PanelAxis.py,sha256=w5YYnDXgprHWUzCWcqqBEkV1xJ_6qLabzW_PIbQF9ZQ,3358
 Seance/Builder/PreProcess.py,sha256=i4IWwm12welXyK1b90CbHJyQi02vjtTHcaEacjLsm-A,3990
 Seance/Builder/Transformations.py,sha256=JY27tWWvxha2JXhVgOALQFJUhV-N2Hcmg2u9hhBSeaA,6595
 Seance/Builder/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/fourier_basis.py,sha256=SNOuujoYtcofte1z9BoBDR7kCBdvWaCONrjeSWvesow,865
 Seance/basis_functions/linear_basis.py,sha256=1RHj--VkbA4heV8QwzNE7a9O0-aPu3Br3EqLlcuUHWU,2834
-Seance-0.0.1.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
-Seance-0.0.1.dist-info/METADATA,sha256=W8H-k4KihKssbIANWizYe6lbAtdHn2lrDm8BXyMUc24,2676
-Seance-0.0.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Seance-0.0.1.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
-Seance-0.0.1.dist-info/RECORD,,
+Seance-0.0.2.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
+Seance-0.0.2.dist-info/METADATA,sha256=ZiE_6C29mUulcd1vyFYneyQmRLt2b2iKs7R-BJeH7Ls,2684
+Seance-0.0.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Seance-0.0.2.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
+Seance-0.0.2.dist-info/RECORD,,
```

