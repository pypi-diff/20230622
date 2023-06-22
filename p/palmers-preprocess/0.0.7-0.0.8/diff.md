# Comparing `tmp/palmers_preprocess-0.0.7.tar.gz` & `tmp/palmers_preprocess-0.0.8.tar.gz`

## Comparing `palmers_preprocess-0.0.7.tar` & `palmers_preprocess-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/__init__.py
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/clearml_data_handler.py
--rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/config.py
--rw-r--r--   0        0        0    43620 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/events_handler.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/lags_feature_handler.py
--rw-r--r--   0        0        0     7475 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/preprocessor.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/regular_data_handler.py
--rw-r--r--   0        0        0     7669 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/config.py
--rw-r--r--   0        0        0     8923 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/cumulative_features.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/event_features.py
--rw-r--r--   0        0        0     8418 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/future_features.py
--rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/lags_features.py
--rw-r--r--   0        0        0     5404 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/features/weather_features.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/__init__.py
--rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/config_batch_dict.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/event_feature_test.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/features_test.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/lags_features_test.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/preprocessor_test.py
--rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/sanity_checks.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/test_todelete.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/weather_test.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/__init__.py
+-rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/clearml_data_handler.py
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/config.py
+-rw-r--r--   0        0        0    42984 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/events_handler.py
+-rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/lags_feature_handler.py
+-rw-r--r--   0        0        0    10060 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/preprocessor.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/regular_data_handler.py
+-rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/__init__.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/config.py
+-rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/cumulative_features.py
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/event_features.py
+-rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/future_features.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/lags_features.py
+-rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/weather_features.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/__init__.py
+-rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/config_batch_dict.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/event_feature_test.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/features_test.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/lags_features_test.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/preprocessor_test.py
+-rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/sanity_checks.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/test_todelete.py
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/weather_test.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/LICENSE
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/README.md
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/PKG-INFO
```

### Comparing `palmers_preprocess-0.0.7/requirements.txt` & `palmers_preprocess-0.0.8/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -55,7 +55,9 @@
 tomli==2.0.1
 twine==4.0.2
 typing_extensions==4.5.0
 tzdata==2023.3
 urllib3==1.26.15
 webencodings==0.5.1
 zipp==3.15.0
+catboost==1.1.1
+
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/clearml_data_handler.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/clearml_data_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/config.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-SKU_COLUMN_NAME = "sku"
+import datetime
+ITEM_COLUMN_NAME = "item"
 STORE_COLUMN_NAME = "store"
 SALES_COLUMN_NAME = "sales"
 DATE_COLUMN_NAME = "date"
-SKU_STORE_COLUMN_NAME = "sku, store"
+ITEM_STORE_COLUMN_NAME = "item, store"
+ITEM_STORE_COLUMN_NAME_LIST = ["item", "store"]
 ID_COLUMN_NAME = "id"
-
+SKU_COLUMN_NAME = "sku"
 LIST_FREQ = ["D", "W-Mon", "M", "Y"]
 START_DATE_CUMULATIVE_FEATURES = "2018-01-01"
+tomorrow_date = str(datetime.datetime.now(datetime.timezone.utc).date()+datetime.timedelta(days=1))
 
-# DEFAULT_MARKETING_PLAN_FEATURES = {'dataset_project': 'palmers/datasets',
-#                                    'dataset_name': 'marketing_plan',
-#                                    'dataset_file_name': 'marketing_plan.csv',
-#                                       'dataset_version': None,
-#                                         'dataset_tags': None,
-#
-#                                    }
 
 DEFAULT_MARKETING_PLAN_FEATURES = {'project_name': 'examples',
                                    'task_name': 'marketing_plan_feature',
                                    'task_id': '630578192a1f432bb58240782f47a0d6',
                                    'artifact_name': 'marketing_plan_feature',
                                    }
 
-DEFAULT_SKU_SALE_ENCODED_FEATURES = {'project_name': 'examples',
-                                     'task_name': 'mytest_sku_store_sales_encoders',
-                                     'task_id': 'eba5a050890b4e038a37b27d541d57a8',
-                                     'artifact_name': 'sku_encoders'}
+DEFAULT_ITEM_SALE_ENCODED_FEATURES = {'project_name': 'examples',
+                                     'task_name': 'mytest_item_store_sales_encoders_for_daily_preprocess',
+                                     'task_id': 'b8e7efbdb4cc4aedb4da34512eccc30c',
+                                     'artifact_name': 'item_encoders'}
 
 DEFAULT_STORE_SALE_ENCODED_FEATURES = {'project_name': 'examples',
-                                       'task_name': 'mytest_sku_store_sales_encoders',
-                                       'task_id': 'eba5a050890b4e038a37b27d541d57a8',
+                                       'task_name': 'mytest_item_store_sales_encoders_for_daily_preprocess',
+                                       'task_id': 'b8e7efbdb4cc4aedb4da34512eccc30c',
                                        'artifact_name': 'store_encoders'}
 
 DEFAULT_EVENT_DATASET = {'dataset_project': 'palmers/datasets',
                          'dataset_name': 'fix_events',
                          'dataset_file_name': 'events_new_fix.csv',
                          'dataset_version': None,
                          'dataset_tags': None}
@@ -42,15 +38,15 @@
 COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME='columns_interactions_encoder'
 APPLY_ENCODINGS_DICT_ARTIFACT_NAME='apply_encodings_dict'
 APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME='apply_encodings_at_once'
 
 
 DEFAULT_EVENT_ENCODING_FEATURES = {'project_name': 'examples',
                                    'task_name': 'event_feature_fit',
-                                   'task_id' : '0beb66fc16524ddb86ac68450167b329',
+                                   'task_id' : '8078f92691a54427b5123bc375efdd11',
                                    'artifacts_names': [APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME, APPLY_ENCODINGS_DICT_ARTIFACT_NAME,
                                                        COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME, PCA_ENCODER_ARTIFACT_NAME]
                                    }
 
 
 
 DEFAULT_HOLIDAYS_DATASET = {'dataset_project': 'palmers/datasets',
@@ -99,20 +95,15 @@
                           "duration_list_median_event",'is_tomorrow_event',"is_2_days_event"],
     'cols_days_for_ineraction' :['day_of_week', 'week_of_year', 'quarter', 'is_weekend', "ind_change_combo_event",
                             'is_sunday', "is_holday"],
     'type_encoder_list': ["MEstimateEncoder", "CatBoostEncoder"],
     'list_col_add': ["date"]
 }
 
-OUTLETS_SDATTA = [3, 18, 22, 28, 44, 50, 55, 57, 68, 73, 74, 76, 79, 82, 88, 91, 96, 99, 100, 119, 123, 130, 133, 141,
-                  144, 149, 152, 162, 164, 166, 167, 168, 171, 173, 175, 180, 181, 184, 185, 186, 188, 189, 202, 203,
-                  214, 216, 218, 221, 226, 3005, 3202, 3205, 3208, 3290, 4104, 4123, 4129, 4132, 4133, 4134, 4803, 4805,
-                  4904, 4906]
-OUTLETS_PALMERS = [4, 5, 7, 8, 10, 11, 15, 21, 26, 27, 29, 35, 36, 37, 42, 43, 45, 46, 47, 51, 52, 56, 61, 63, 64, 67,
-                   69, 81, 84, 85, 89, 90, 95, 104, 105, 106, 109, 114, 117, 121, 122, 135, 136, 143, 147, 150, 156,
-                   159, 160, 163, 170, 172, 174, 179, 182, 183, 201, 213, 215, 217, 219, 220, 225, 3245]
+OUTLETS_SDATTA = [3, 18, 22, 28, 29, 44, 51, 57, 63, 73, 74, 76, 79, 88, 89, 91, 96, 100, 117, 119, 123, 130, 133, 135, 136, 141, 143, 144, 149, 150, 152, 162, 164, 166, 167, 168, 171, 172, 175, 179, 181, 184, 185, 186, 188, 189, 202, 214, 216, 217, 226, 3005, 3202, 3205, 3208, 4104, 4123, 4129, 4134, 4803, 4805,4904,4906]
+
 OUTLETS_ALL = [3, 18, 22, 28, 44, 50, 55, 57, 68, 73, 74, 76, 79, 82, 88, 91, 96, 99, 100, 119, 123, 130, 133, 141, 144,
                149, 152, 162, 164, 166, 167, 168, 171, 173, 175, 180, 181, 184, 185, 186, 188, 189, 202, 203, 214, 216,
                218, 221, 226, 3005, 3202, 3205, 3208, 3290, 4104, 4123, 4129, 4132, 4133, 4134, 4803, 4805, 4904, 4906,
                4, 5, 7, 8, 10, 11, 15, 21, 26, 27, 29, 35, 36, 37, 42, 43, 45, 46, 47, 51, 52, 56, 61, 63, 64, 67, 69,
                81, 84, 85, 89, 90, 95, 104, 105, 106, 109, 114, 117, 121, 122, 135, 136, 143, 147, 150, 156, 159, 160,
                163, 170, 172, 174, 179, 182, 183, 201, 213, 215, 217, 219, 220, 225, 3245]
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/events_handler.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/events_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,45 +4,58 @@
 from scipy.fftpack import fft
 from scipy.signal import argrelextrema
 from sklearn.decomposition import PCA
 from category_encoders import GLMMEncoder, MEstimateEncoder, CatBoostEncoder
 from . import config
 
 
-#TODO: speak to yotam
-def run_pipline_event(data_event, data_sales, data_hol, date_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['date_col'], start_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['start_date'], target_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['target_col'],
+# TODO: speak to yotam
+def run_pipline_event(data_event, data_sales, data_hol, date_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['date_col'],
+                      start_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['start_date'],
+                      target_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['target_col'],
                       max_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['max_date'],
-                      min_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['min_date'], duration_list_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['duration_list_col'],
-                      column_list_map_id=config.DEFAULT_EVENT_HANDLER_VARIABLES['column_list_map_id'], event_num=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_num'],
-                      event_col_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_col_list'], event_col_even=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_col_even'],
-                      date_min_col_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['date_min_col_list'], holiday_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['holiday_col'],
-                      holiday_col_type=config.DEFAULT_EVENT_HANDLER_VARIABLES['holiday_col_type'], weekend_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['weekend_col'],
-                      year_forecast=config.DEFAULT_EVENT_HANDLER_VARIABLES['year_forecast'], pca_num=config.DEFAULT_EVENT_HANDLER_VARIABLES['pca_num'],
-                      type_encoder_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['type_encoder_list'], cols_to_encode=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode'],
+                      min_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['min_date'],
+                      duration_list_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['duration_list_col'],
+                      column_list_map_id=config.DEFAULT_EVENT_HANDLER_VARIABLES['column_list_map_id'],
+                      event_num=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_num'],
+                      event_col_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_col_list'],
+                      event_col_even=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_col_even'],
+                      date_min_col_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['date_min_col_list'],
+                      holiday_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['holiday_col'],
+                      holiday_col_type=config.DEFAULT_EVENT_HANDLER_VARIABLES['holiday_col_type'],
+                      weekend_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['weekend_col'],
+                      year_forecast=config.DEFAULT_EVENT_HANDLER_VARIABLES['year_forecast'],
+                      pca_num=config.DEFAULT_EVENT_HANDLER_VARIABLES['pca_num'],
+                      type_encoder_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['type_encoder_list'],
+                      cols_to_encode=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode'],
                       cols_to_encode_at_once=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode_at_once'],
                       cols_days_for_interaction=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_days_for_ineraction'],
                       list_col_add=config.DEFAULT_EVENT_HANDLER_VARIABLES['list_col_add']):
-        
     event_preprocess = EventFeatureGenerator()
     # event_preprocess.change_columns_names_in_dataframe_by_dict(data_sales, column_dict)
     data_sales0 = event_preprocess.filter_data_by_date(data_sales, date_col, start_date)
     data_sales_process = event_preprocess.aggregate_data(data_sales0, target_col)
     data_sales_process1 = event_preprocess.process_date_column(data_sales_process, date_col)
     data_event_process = event_preprocess.calculate_duration(data_event, max_date, min_date)
-    data_sales_process2 = event_preprocess.identify_event(data_event_process, data_sales_process1, date_col, min_date, max_date)
-    data_sales_process3 = event_preprocess.map_event_to_list(data_sales_process2, data_event_process, max_date, min_date, column_list_map_id, date_col)
+    data_sales_process2 = event_preprocess.identify_event(data_event_process, data_sales_process1, date_col, min_date,
+                                                          max_date)
+    data_sales_process3 = event_preprocess.map_event_to_list(data_sales_process2, data_event_process, max_date,
+                                                             min_date, column_list_map_id, date_col)
     data_sales_process4 = event_preprocess.add_stat_duartions(data_sales_process3, duration_list_col)
     data_sales_process5 = event_preprocess.length_list_event(data_sales_process4, event_col_list)
     data_sales_process6 = event_preprocess.diff_col(data_sales_process5, target_col, date_col)
     data_sales_process7 = event_preprocess.event_frequency(data_sales_process6, date_col, event_num)
     data_sales_process8 = event_preprocess.indicate_event_combination_change(data_sales_process7, event_col_even)
     # data_sales_process9 = event_preprocess.std_on_list(data_sales_process8, event_col_discount_type)
     data_sales_process10 = event_preprocess.log_col(data_sales_process8, target_col)
-    data_sales_process11 = event_preprocess.caculate_amount_days_pass_from_start_of_event(data_sales_process10, date_col, date_min_col_list)
-    data_sales_process12 = event_preprocess.caculate_amount_days_pass_from_start_of_event_most_new(data_sales_process11, date_min_col_list, date_col)
+    data_sales_process11 = event_preprocess.caculate_amount_days_pass_from_start_of_event(data_sales_process10,
+                                                                                          date_col, date_min_col_list)
+    data_sales_process12 = event_preprocess.caculate_amount_days_pass_from_start_of_event_most_new(data_sales_process11,
+                                                                                                   date_min_col_list,
+                                                                                                   date_col)
     data_sales_process13 = event_preprocess.merge_df(data_sales_process12, data_hol, date_col)
     data_sales_process14 = event_preprocess.identify_date_occasion(data_sales_process13, holiday_col, date_col)
     data_sales_process15 = event_preprocess.feature_combine_str(data_sales_process14, holiday_col_type, holiday_col)
     data_sales_process16 = event_preprocess.add_cumulative_sum_column_for_targe(data_sales_process15, target_col)
     data_sales_process17 = event_preprocess.fft_features(data_sales_process16, target_col)
     data_sales_process18 = event_preprocess.time_series_shape_features(data_sales_process17, target_col)
     data_sales_process21 = event_preprocess.convert_str_indicator(data_sales_process18, weekend_col)
@@ -50,31 +63,25 @@
     # data_sales_process22 = event_preprocess.extract_features_pca(data_sales_process21, date_col, year_forecast, pca_num,
     #                                                              target_col, task=task)
     #
     data_sales_process23 = event_preprocess.process_next_days_events(data_sales_process21, target_col)
 
     return data_sales_process23
 
-def finalize_data(df):
-    event_preprocess = EventFeatureGenerator()
 
-    # data_sales_process24 = event_preprocess.apply_encodings(data_sales_process23, type_encoder_list, cols_to_encode,
-    #                                                         target_col, year_forecast, sigma=1,
-    #                                                         random_state=12, task=task)
-    # data_sales_process25 = event_preprocess.apply_encodings_at_once(data_sales_process24, type_encoder_list,
-    #                                                                 cols_to_encode, target_col,
-    #                                                                 year_forecast=2022, sigma=1, random_state=12,
-    #                                                                 task=task)
-    # data_sales_process26 = event_preprocess.columns_interactions_encoder(data_sales_process25, cols_to_encode_at_once,
-    #                                                                      cols_days_for_ineraction, target_col,
-    #                                                                      type_encoder_list, year_forecast, task=task)
-    # selected_col_by_corr = event_preprocess.filter_columns_by_correlation(data_sales_process25, year_forecast, target_col,
-    #                                                                       date_col)
-    # data_sales_final1 = event_preprocess.add_back_feature(data_sales_process25, list_col_add, selected_col_by_corr)
-    # data_sales_final2 = event_preprocess.process_date_column(data_sales_process26, date_col)
+def finalize_data(df: pd.DataFrame) -> pd.DataFrame:
+    """
+    Finalize data for model removing unnecessary columns
+    Args:
+        df: data event features
+
+    Returns:
+        df
+    """
+    event_preprocess = EventFeatureGenerator()
     data_sales_process27 = event_preprocess.remove_expand_dates(df)
     data_final_event = data_sales_process27.copy()
     return data_final_event
 
 
 class EventFeatureGenerator:
     @classmethod
@@ -280,16 +287,17 @@
             date_col (str): The name of the column representing the dates.
             event_num (str): The name of the column representing the event counts ->'num_event_id_list'
 
         Returns:
             pd.DataFrame: DataFrame with a new column called 'event_frequency'.
             This column represents the average number of events per week, based on the event count and number of weeks in the date column.
         """
+
         df_sales['event_frequency'] = (
-                    df_sales[event_num] / pd.to_datetime(df_sales[date_col]).dt.week.nunique()).shift(1).fillna(0)
+                df_sales[event_num] / df_sales[date_col].dt.isocalendar().week.nunique()).shift(1).fillna(0)
         return df_sales
 
     @classmethod
     def indicate_event_combination_change(cls, df_sales: pd.DataFrame, event_col_even: str) -> pd.DataFrame:
         """
         Indicates whether the combination of events has changed from the previous row in a pandas DataFrame.
 
@@ -363,15 +371,14 @@
             pd.DataFrame: DataFrame with a new column called 'amount_of_days_pass_from_start_of_event'.
             This column represents the number of days that have passed since the start of the event, for each row in the DataFrame.
         """
         df_sales["amount_of_days_pass_from_start_of_event"] = df_sales.apply(
             lambda x: np.abs(pd.to_datetime(x[date_col]) - pd.to_datetime(x[date_min_col_list])), axis=1)
         return df_sales
 
-
     @classmethod
     def caculate_amount_days_pass_from_start_of_event_most_new(cls, df_sales: pd.DataFrame, event_col: str,
                                                                date_col: str) -> pd.DataFrame:
         """
         Calculates the number of days that have passed since the start of an event, for the most recent event in a pandas DataFrame.
 
         Args:
@@ -404,15 +411,15 @@
 
         Returns:
             df_merge    pd.DataFrame: A new DataFrame that contains all columns from both input DataFrames, merged
             on the specified key. The merge type is left join (i.e., all rows from df1 are retained, and
             matching rows from df2 are included where available).
         """
         df_sales[key] = pd.to_datetime(df_sales[key])
-        df_holiday[key] = pd.to_datetime(df_holiday[key])
+        df_holiday[key] = pd.to_datetime(df_holiday[key], format="%d/%m/%Y")
         df_sales = df_sales.merge(df_holiday, on=key, how="left")
         return df_sales
 
     @classmethod
     def identify_date_occasion(cls, df_sales: pd.DataFrame, holiday_col: str, date_col: str) -> pd.DataFrame:
         """
         Identifies holidays in a pandas DataFrame based on a specified column.
@@ -579,15 +586,15 @@
         """
 
         df_sales[weekend_col] = np.where(df_sales[weekend_col] is True, 1, 0)
         return df_sales
 
     @classmethod
     def extract_features_pca(cls, df_sales: pd.DataFrame, date_col: str,
-                             pca_num: int, year_forecast: int=None) -> pd.DataFrame:
+                             pca_num: int, year_forecast: int = None) -> pd.DataFrame:
         """
         Perform Principal Component Analysis (PCA) on a subset of numerical columns in a DataFrame, and append the resulting
         principal components to the original DataFrame.
 
         Args:
             df (pd.DataFrame): The input DataFrame.
             year_forecast (int): The year after which to exclude data from PCA analysis.
@@ -727,16 +734,16 @@
         interactions_columns = []
         for col1 in cols_to_encode_at_once:
             for col2 in cols_days_for_interaction:
                 df_sales[f"{col1}_interactions_{col2}"] = df_sales[f"{col1}"] * df_sales[f"{col2}"]
                 interactions_columns.append(f"{col1}_interactions_{col2}")
 
         df_sales = cls.apply_encodings_at_once(df_sales=df_sales, type_encoder_list=type_encoder_list,
-                                                cols_to_encode=interactions_columns,
-                                                target_col=target_col, year_forecast=year_forecast)
+                                               cols_to_encode=interactions_columns,
+                                               target_col=target_col, year_forecast=year_forecast)
         return df_sales
 
     @classmethod
     def remove_expand_dates(cls, df_sales: pd.DataFrame):
         columns_to_check = ['year', 'month', 'day', 'day_of_week', 'week_of_year', 'quarter', 'is_weekend']
         if all(column in df_sales.columns for column in columns_to_check):
             df_sales = df_sales.drop(columns=columns_to_check)
@@ -803,14 +810,11 @@
 
 
 def create_interactions_columns(processed_event_features_df):
     cols_to_encode_at_once = config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode_at_once']
     cols_days_for_interaction = config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_days_for_ineraction']
     for col1 in cols_to_encode_at_once:
         for col2 in cols_days_for_interaction:
-            processed_event_features_df[f"{col1}_interactions_{col2}"] = processed_event_features_df[f"{col1}"] * processed_event_features_df[f"{col2}"]
-
-
+            processed_event_features_df[f"{col1}_interactions_{col2}"] = processed_event_features_df[f"{col1}"] * \
+                                                                         processed_event_features_df[f"{col2}"]
 
     return processed_event_features_df
-
-
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/regular_data_handler.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/regular_data_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,17 +9,17 @@
        return cls.load_specific()
 
     @classmethod
     def load_specific(cls):
         # Load data
 
 
-        file_name = "regular_data_after_cleaning.csv"
+        file_name = "not_sparse_data_gap_until_2023_05_22.csv"
         dataset_df_files = cdh.DatasetLoader().load_dfs_from_dataset(dataset_project='palmers/datasets',
-                                                                     dataset_name="regular_dataset_include_04_2023"
+                                                                     dataset_name="gap_filling_for_models_until_2023_05_22"
                                               , dataset_file_names=[file_name])
         regular_data_df = dataset_df_files[file_name]#.drop('Unnamed: 0', axis=1)
         return regular_data_df
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/utils.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from datetime import timedelta, datetime
 
 import numpy as np
 import pandas as pd
 from . import config
 
-def process_date_column(df_sales: pd.DataFrame, date_col: str, expanded:bool = False) -> pd.DataFrame:
+
+def process_date_column(df_sales: pd.DataFrame, date_col: str, expanded: bool = False) -> pd.DataFrame:
     """
     Process date column
     Args:
         df_sales: pandas DataFrame
         date_col: name of date column
     Returns: pandas DataFrame
     """
@@ -24,20 +25,19 @@
 
     if expanded:
         df_sales['day_of_year'] = df_sales[date_col].dt.dayofyear
         df_sales['day_of_the_month'] = df_sales[date_col].dt.days_in_month
         df_sales['is_weekend_c'] = df_sales['day_of_week'].apply(lambda x: 1 if x in [5, 6] else 0)
         df_sales['is_weekend_j'] = df_sales['day_of_week'].apply(lambda x: 1 if x in [4, 5] else 0)
 
-
     return df_sales
 
 
 def add_values_to_dict_mapper(dict_mapper: dict, df_encoders: pd.DataFrame, column_name: str, encoders_name: list,
-                             dict_of_time_interval: dict) -> dict:
+                              dict_of_time_interval: dict) -> dict:
     """
     Adds the values of the encoders in the df_encoders dataframe to the dict_maper dictionary.
 
     Args:
         dict_mapper:     The dictionary that holds the encoded values.
         df_encoders:        The dataframe that holds the encoded values.
         column_name:    The name of the column in the df_encoders dataframe.
@@ -60,89 +60,152 @@
                             item_encoders_with_item_index.loc[item][encoder + "_all_time:all_time"]
                     else:
                         dict_mapper[column_name][encoder][time][(item, date)] = \
                             item_encoders_with_item_index.loc[item][encoder + "_" + str(time) + ":" + str(date)]
     return dict_mapper
 
 
-def map_encoders_columns_to_base_df( data: pd.DataFrame, dict_map: dict, encoders_name: list) -> pd.DataFrame:
+def map_encoders_columns_to_base_df(data: pd.DataFrame, dict_map: dict, encoders_name: list) -> pd.DataFrame:
     """
     Adds the encoded values to the data dataframe.
     Args:
         data:   The dataframe to add the encoded values to.
         dict_map:   The dictionary that holds the encoded values.
         encoders_name:  The names of the encoders in the df_encoders dataframe.
 
     Returns:    The updated data dataframe.
 
     """
     for encoder_name in encoders_name:
         data[encoder_name + "_day_store"] = data.apply(
-            lambda x: dict_map["store"][encoder_name]["name_of_day"][x["store"], x["name_of_day"]], axis=1)
-        data[encoder_name + "_day_sku"] = data.apply(
-            lambda x: dict_map["sku"][encoder_name]["name_of_day"][x["sku"], x["name_of_day"]], axis=1)
+            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["name_of_day"][
+                x[config.STORE_COLUMN_NAME], x["name_of_day"]], axis=1)
+        data[encoder_name + "_day_item"] = data.apply(
+            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["name_of_day"][
+                x[config.ITEM_COLUMN_NAME], x["name_of_day"]], axis=1)
         data[encoder_name + "_month_store"] = data.apply(
-            lambda x: dict_map["store"][encoder_name]["month"][x["store"], x["month"]], axis=1)
-        data[encoder_name + "_month_sku"] = data.apply(
-            lambda x: dict_map["sku"][encoder_name]["month"][x["sku"], x["month"]], axis=1)
+            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["month"][
+                x[config.STORE_COLUMN_NAME], x["month"]], axis=1)
+        data[encoder_name + "_month_item"] = data.apply(
+            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["month"][x[config.ITEM_COLUMN_NAME], x["month"]],
+            axis=1)
         data[encoder_name + "_quarter_store"] = data.apply(
-            lambda x: dict_map["store"][encoder_name]["quarter"][x["store"], x["quarter"]], axis=1)
-        data[encoder_name + "_quarter_sku"] = data.apply(
-            lambda x: dict_map["sku"][encoder_name]["quarter"][x["sku"], x["quarter"]], axis=1)
-        data[encoder_name + "_months_5_6_7_store"] = data.apply(
-            lambda x: dict_map["store"][encoder_name]["months_5_6_7"][x["store"], 0], axis=1)
-        data[encoder_name + "_months_5_6_7_sku"] = data.apply(
-            lambda x: dict_map["sku"][encoder_name]["months_5_6_7"][x["sku"], 0], axis=1)
-        data[encoder_name + "_all_time_store"] = data.apply(
-            lambda x: dict_map["store"][encoder_name]["all"][x["store"], 0], axis=1)
-        data[encoder_name + "_all_time_sku"] = data.apply(
-            lambda x: dict_map["sku"][encoder_name]["all"][x["sku"], 0], axis=1)
+            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["quarter"][
+                x[config.STORE_COLUMN_NAME], x["quarter"]], axis=1)
+        data[encoder_name + "_quarter_item"] = data.apply(
+            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["quarter"][
+                x[config.ITEM_COLUMN_NAME], x["quarter"]], axis=1)
 
         data[encoder_name + "_day_store"] = data[encoder_name + "_day_store"].astype("float")
-        data[encoder_name + "_day_sku"] = data[encoder_name + "_day_sku"].astype("float")
+        data[encoder_name + "_day_item"] = data[encoder_name + "_day_item"].astype("float")
         data[encoder_name + "_month_store"] = data[encoder_name + "_month_store"].astype("float")
-        data[encoder_name + "_month_sku"] = data[encoder_name + "_month_sku"].astype("float")
+        data[encoder_name + "_month_item"] = data[encoder_name + "_month_item"].astype("float")
         data[encoder_name + "_quarter_store"] = data[encoder_name + "_quarter_store"].astype("float")
-        data[encoder_name + "_quarter_sku"] = data[encoder_name + "_quarter_sku"].astype("float")
-        data[encoder_name + "_months_5_6_7_store"] = data[encoder_name + "_months_5_6_7_store"].astype("float")
-        data[encoder_name + "_months_5_6_7_sku"] = data[encoder_name + "_months_5_6_7_sku"].astype("float")
-        data[encoder_name + "_all_time_store"] = data[encoder_name + "_all_time_store"].astype("float")
-        data[encoder_name + "_all_time_sku"] = data[encoder_name + "_all_time_sku"].astype("float")
+        data[encoder_name + "_quarter_item"] = data[encoder_name + "_quarter_item"].astype("float")
 
         return data
 
-def parse_regular_data_columns(data: pd.DataFrame, sku_col_str = config.SKU_COLUMN_NAME, store_col_str=config.STORE_COLUMN_NAME,
-                                   sales_col_str=config.SALES_COLUMN_NAME, date_col_str=config.DATE_COLUMN_NAME,
-                               sku_store_col_str=config.SKU_STORE_COLUMN_NAME):
-    if sku_col_str in data.columns:
-        data[sku_col_str] = data[sku_col_str].astype(np.int64)
+
+def parse_regular_data_columns(data: pd.DataFrame, item_col_str: str = config.ITEM_COLUMN_NAME,
+                               store_col_str: str = config.STORE_COLUMN_NAME,
+                               sales_col_str: str = config.SALES_COLUMN_NAME,
+                               date_col_str: str = config.DATE_COLUMN_NAME,
+                               item_store_col_str: str = config.ITEM_STORE_COLUMN_NAME) -> pd.DataFrame:
+    """
+    Parses the columns of the data dataframe to the correct data type.
+
+    Args:
+        data: The dataframe to parse.
+        item_col_str: The name of the item column.
+        store_col_str: The name of the store column.
+        sales_col_str: The name of the sales column.
+        date_col_str: The name of the date column.
+        item_store_col_str: The name of the item_store column.
+
+    Returns:
+        The updated data dataframe.
+
+    Notes:
+    1) item_col_str -> np.int64
+    2) store_col_str -> np.int32
+    3) sales_col_str -> np.float32
+    4) date_col_str -> pd.to_datetime
+    5) item_store_col_str -> str
+    """
+    if item_col_str in data.columns:
+        data[item_col_str] = data[item_col_str].astype(np.int64)
     if store_col_str in data.columns:
         data[store_col_str] = data[store_col_str].astype(np.int32)
     if sales_col_str in data.columns:
         data[sales_col_str] = data[sales_col_str].astype(np.float32)
     if date_col_str in data.columns:
         data[date_col_str] = pd.to_datetime(data[date_col_str])
-    if sku_store_col_str in data.columns:
-        data[sku_store_col_str] = data[sku_store_col_str].astype(str)
+    if item_store_col_str in data.columns:
+        data[item_store_col_str] = data[item_store_col_str].astype(str)
     return data
 
-def next_two_days_skip_sunday(start_date):
-    # Create a list to store the dates
+
+def next_two_days_skip_sunday(start_date:str):
+    """
+    This function returns the next two days after the start date, skipping Sunday.
+
+    Args:
+        start_date: The start date
+
+    Returns:
+        A list of the next two days after the start date, skipping Sunday.
+
+    """
     dates = []
-    # parse start_date to datetime
     start_date = datetime.strptime(start_date, '%Y-%m-%d')
-
-    # Loop through the next two days
     for i in range(2):
-        # Add a day to the date
         start_date += timedelta(days=1)
-        # Check if the new date is a Sunday
         if start_date.weekday() == 6:
-            # If it's a Sunday, add another day to skip it
             start_date += timedelta(days=1)
-        # Add the date to the list
         dates.append(start_date)
 
+    return dates
 
 
-    # Return the dataframe
-    return dates
+def convert_df_with_sku_to_df_with_item(df: pd.DataFrame) -> pd.DataFrame:
+    """
+    Converts a dataframe with sku to a dataframe with item and group by date, item, store and sales.
+    Args:
+        df:     The dataframe to convert.
+
+    Returns:
+        The converted dataframe.
+
+    """
+    df[config.ITEM_COLUMN_NAME] = df[config.SKU_COLUMN_NAME].str[:-3]
+    df[config.SALES_COLUMN_NAME] = df[config.SALES_COLUMN_NAME].astype(float)
+    df[config.ITEM_STORE_COLUMN_NAME] = df[config.ITEM_COLUMN_NAME] + ", " + df[config.STORE_COLUMN_NAME]
+    df = df[[config.DATE_COLUMN_NAME, config.ITEM_STORE_COLUMN_NAME, config.ITEM_COLUMN_NAME, config.STORE_COLUMN_NAME,
+             config.SALES_COLUMN_NAME]]
+    df = df.groupby(
+        [config.DATE_COLUMN_NAME, config.ITEM_STORE_COLUMN_NAME, config.ITEM_COLUMN_NAME, config.STORE_COLUMN_NAME])[
+        config.SALES_COLUMN_NAME].sum().reset_index()
+    return df
+
+
+def daily_sales_to_weekly_mean_sales(df: pd.DataFrame) -> pd.DataFrame:
+    """
+    This function converts the daily sales to weekly mean sales.
+    with groupby on item_store and rolling mean of 6 days - excluding the sunday.
+    Args:
+        df:     The dataframe to convert.
+
+    Returns:
+        The converted dataframe.
+    """
+    df_with_window_6_rolling = pd.DataFrame()
+    grouped = df.groupby([config.ITEM_STORE_COLUMN_NAME])
+    for name, group in grouped:
+        group_rolling = group.groupby(config.DATE_COLUMN_NAME)[config.SALES_COLUMN_NAME].sum().rolling(6,
+                                                                                                       min_periods=6).mean().reset_index()
+        group_rolling[config.ITEM_STORE_COLUMN_NAME] = name
+        group_rolling[config.ITEM_COLUMN_NAME] = name.split(", ")[0]
+        group_rolling[config.STORE_COLUMN_NAME] = name.split(", ")[1]
+        df_with_window_6_rolling = pd.concat([df_with_window_6_rolling, group_rolling])
+    df_with_window_6_rolling.reset_index(drop=True, inplace=True)
+    df_with_window_6_rolling = df_with_window_6_rolling.dropna(subset=[config.SALES_COLUMN_NAME])
+    return df_with_window_6_rolling
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/future_features.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/features/future_features.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,155 +1,191 @@
-# from clearml_architecture.feature_process.WeatherFeatures.global_config import *
-from clearml import Dataset, Task
 import pandas as pd
-
 from .. import config as global_config
 from . import config
-
-from ..clearml_data_handler import DatasetLoader, ArtifactLoader
 from ..utils import process_date_column, add_values_to_dict_mapper, map_encoders_columns_to_base_df
 
-class MarketingPlanFeatures:
-    @classmethod
-    def load(cls, project_name=global_config.DEFAULT_MARKETING_PLAN_FEATURES['project_name'],
-             task_name=global_config.DEFAULT_MARKETING_PLAN_FEATURES['task_name'],
-             task_id=global_config.DEFAULT_MARKETING_PLAN_FEATURES['task_id'],
-             artifact_name=global_config.DEFAULT_MARKETING_PLAN_FEATURES['artifact_name'],
-             ):
-
-        marketing_plan_df = ArtifactLoader().load_artifact_as_df(project_name=project_name,
-                                                                   task_name=task_name,
-                                                                   task_id=task_id,
-                                                                   artifact_name=artifact_name,
-                                                                   )
-        marketing_plan_df = marketing_plan_df.loc[:,
-                                   ~marketing_plan_df.columns.str.contains('Unnamed')]
-        marketing_plan_df = marketing_plan_df.dropna()
-
-        cols_to_convert = marketing_plan_df.columns.difference(['date'])
-        marketing_plan_df[cols_to_convert] = marketing_plan_df[cols_to_convert].astype('int32')
-
-        return marketing_plan_df
-
-
-class SkuSaleEncodedFeatures:
-    @classmethod
-    def load(cls, task_id=global_config.DEFAULT_SKU_SALE_ENCODED_FEATURES['task_id'],
-             project_name=global_config.DEFAULT_SKU_SALE_ENCODED_FEATURES['project_name'],
-             task_name=global_config.DEFAULT_SKU_SALE_ENCODED_FEATURES['task_name'],
-             artifact_name=global_config.DEFAULT_SKU_SALE_ENCODED_FEATURES['artifact_name']):
-        sku_encoders = ArtifactLoader().load_artifact_as_df(project_name=project_name,
-                                                            task_name=task_name,
-                                                            task_id=task_id,
-                                                            artifact_name=artifact_name)
-        sku_encoders = sku_encoders.drop('Unnamed: 0', axis=1)
-        sku_encoders[global_config.SKU_COLUMN_NAME] = sku_encoders[global_config.SKU_COLUMN_NAME].astype('int64')
-        sku_encoders = sku_encoders.set_index(global_config.SKU_COLUMN_NAME)
-        sku_encoders = sku_encoders.astype('float')
-
-        return sku_encoders
-
-
-class StoreSaleEncodedFeatures:
-    @classmethod
-    def load(cls, task_id=global_config.DEFAULT_STORE_SALE_ENCODED_FEATURES['task_id'],
-             project_name=global_config.DEFAULT_STORE_SALE_ENCODED_FEATURES['project_name'],
-             task_name=global_config.DEFAULT_STORE_SALE_ENCODED_FEATURES['task_name'],
-             artifact_name=global_config.DEFAULT_STORE_SALE_ENCODED_FEATURES['artifact_name']):
-        store_encoders =  ArtifactLoader().load_artifact_as_df(project_name=project_name,
-                                                            task_name=task_name,
-                                                            task_id=task_id,
-                                                            artifact_name=artifact_name)
-        store_encoders = store_encoders.drop('Unnamed: 0', axis=1)
-        store_encoders[global_config.STORE_COLUMN_NAME] = store_encoders[global_config.STORE_COLUMN_NAME].astype('int32')
-        store_encoders = store_encoders.set_index(global_config.STORE_COLUMN_NAME)
-        store_encoders=store_encoders.astype('float')
-
-        return store_encoders
-
+def clean_marketing(marketing_plan_df: pd.DataFrame) -> pd.DataFrame:
+    """
+    Clean marketing plan df from unnecessary columns and convert columns to int32
+    Args:
+        marketing_plan_df:
+
+    Returns:
+
+    """
+    marketing_plan_df = marketing_plan_df.loc[:,
+                        ~marketing_plan_df.columns.str.contains('Unnamed')]
+    marketing_plan_df = marketing_plan_df.dropna()
+
+    cols_to_convert = marketing_plan_df.columns.difference(['date'])
+    marketing_plan_df[cols_to_convert] = marketing_plan_df[cols_to_convert].astype('int32')
+
+    return marketing_plan_df
+
+
+def clean_item_encoder(item_encoders):
+    """
+    Clean item encoder df from unnecessary columns and convert columns to int64
+    Args:
+        item_encoders:  item encoder df
+
+    Returns:
+        item_encoders
+    """
+    item_encoders = item_encoders.drop('Unnamed: 0', axis=1)
+    item_encoders[global_config.ITEM_COLUMN_NAME] = item_encoders[global_config.ITEM_COLUMN_NAME].astype('int64')
+    item_encoders = item_encoders.set_index(global_config.ITEM_COLUMN_NAME)
+    item_encoders = item_encoders.astype('float')
+    return item_encoders
+
+
+def clean_store_encoder(store_encoders):
+    """
+    Clean store encoder df from unnecessary columns and convert columns to int32
+    Args:
+        store_encoders:     store encoder df
+
+    Returns:
+        store_encoders
+    """
+    store_encoders = store_encoders.drop('Unnamed: 0', axis=1)
+    store_encoders[global_config.STORE_COLUMN_NAME] = store_encoders[global_config.STORE_COLUMN_NAME].astype(
+        'int32')
+    store_encoders = store_encoders.set_index(global_config.STORE_COLUMN_NAME)
+    store_encoders = store_encoders.astype('float')
+    return store_encoders
 
 
 class FarFutureFeaturesGenerator:
 
     @classmethod
-    def far_future_features_preprocess_of_store(cls, store_batch, begin_predict_dates):
-        marketing_plan = MarketingPlanFeatures.load()
-        sku_encoders =  SkuSaleEncodedFeatures.load()#.reset_index().rename(columns={'index': global_config.SKU_COLUMN_NAME})
-        store_encoders =  StoreSaleEncodedFeatures.load()#.reset_index().rename(columns={'index': global_config.STORE_COLUMN_NAME})
-
-
-        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, sku_encoders, global_config.SKU_COLUMN_NAME, config.ENCODERS_NAME,
-                                              config.DICT_OF_TIME_INTERVAL)
-
-        dict_mapper = add_values_to_dict_mapper(dict_mapper, store_encoders, global_config.STORE_COLUMN_NAME, config.ENCODERS_NAME,
-                                              config.DICT_OF_TIME_INTERVAL)
+    def far_future_features_preprocess_of_store(cls, marketing_plan: pd.DataFrame, item_encoders , store_encoders, store_batch,
+                                                begin_predict_dates: str) -> pd.DataFrame:
+        """
+        Preprocess of store for far future features generation
+        following the steps:
+        1) clean marketing plan df
+        2) clean item encoder df
+        3) clean store encoder df
+        4) add values to dict mapper
+        5) create future date range
+        6) create future features df
+        7) create future features df with store batch
+        8) create future features df with store batch and begin predict dates
+        9) create future features df with store batch and begin predict dates and marketing plan
+        10) create future features df with store batch and begin predict dates and marketing plan and item encoders
+        Args:
+            marketing_plan:     marketing plan df
+            item_encoders:    item encoder df
+            store_encoders:     store encoder df
+            store_batch:    store batch
+            begin_predict_dates:    begin predict dates
+
+        Returns:
+            output_df : future features df with store batch and begin predict dates and marketing plan and item encoders
+        """
+        marketing_plan = clean_marketing(marketing_plan)
+        item_encoders = clean_item_encoder(item_encoders)
+        store_encoders = clean_store_encoder(store_encoders)
 
+        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, item_encoders, global_config.ITEM_COLUMN_NAME,
+                                                config.ENCODERS_NAME,
+                                                config.DICT_OF_TIME_INTERVAL)
 
+        dict_mapper = add_values_to_dict_mapper(dict_mapper, store_encoders, global_config.STORE_COLUMN_NAME,
+                                                config.ENCODERS_NAME,
+                                                config.DICT_OF_TIME_INTERVAL)
 
         future_date_range = pd.date_range(start=begin_predict_dates, end=begin_predict_dates, freq='D')
 
         output_df = pd.DataFrame()
         for _id in store_batch:
-            sku_store_id = _id
-            sku = int(sku_store_id.split(',')[0])
-            store = int(sku_store_id.split(',')[1])
+            item_store_id = _id
+            item = int(item_store_id.split(',')[0])
+            store = int(item_store_id.split(',')[1])
             id_data_future = pd.DataFrame({'date': future_date_range,
-                                           'sku, store': sku_store_id,
-                                           'sku': sku,
+                                           'item, store': item_store_id,
+                                           'item': item,
                                            'store': store})
 
             id_data_future = process_date_column(id_data_future, global_config.DATE_COLUMN_NAME, expanded=True)
 
             # Exclude Sunday
-            #id_data_future = id_data_future[id_data_future['day_of_week'] != 6]
+            # id_data_future = id_data_future[id_data_future['day_of_week'] != 6]
 
-            marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(marketing_plan[global_config.DATE_COLUMN_NAME])
+            marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
+                marketing_plan[global_config.DATE_COLUMN_NAME])
 
             id_data_future = pd.merge(id_data_future, marketing_plan, on=[global_config.DATE_COLUMN_NAME], how='left')
 
             id_data_future = map_encoders_columns_to_base_df(id_data_future, dict_mapper, config.ENCODERS_NAME)
             output_df = pd.concat([output_df, id_data_future])
 
-        #output_df.drop('name_of_day', axis=1, inplace=True)
+        # output_df.drop('name_of_day', axis=1, inplace=True)
         return output_df
 
     @classmethod
-    def far_future_features_preprocess_of_several_stores(cls, store_batch_dict, begin_predict_dates):
-        marketing_plan = MarketingPlanFeatures.load()
-        sku_encoders = SkuSaleEncodedFeatures.load()
-        store_encoders = StoreSaleEncodedFeatures.load()
+    def far_future_features_preprocess_of_several_stores(cls, marketing_plan: pd.DataFrame, item_encoders, store_encoders, store_batch_dict, begin_predict_dates: str) -> pd.DataFrame:
+        """
+        Preprocess of store for far future features generation
+        following the steps:
+        1) clean marketing plan df
+        2) clean item encoder df
+        3) clean store encoder df
+        4) add values to dict mapper
+        5) create future date range
+        6) create future features df
+        7) create future features df with store batch
+        8) create future features df with store batch and begin predict dates
+        9) create future features df with store batch and begin predict dates and marketing plan
+        10) create future features df with store batch and begin predict dates and marketing plan and item encoders
+        Args:
+            marketing_plan:     marketing plan df
+            item_encoders:    item encoder df
+            store_encoders:     store encoder df
+            store_batch:    store batch
+            begin_predict_dates:    begin predict dates
+
+        Returns:
+            output_df : future features df with store batch and begin predict dates and marketing plan and item encoders
+        """
+
+        marketing_plan = clean_marketing(marketing_plan)
+        item_encoders = clean_item_encoder(item_encoders)
+        store_encoders = clean_store_encoder(store_encoders)
 
-        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, sku_encoders, global_config.SKU_COLUMN_NAME,
+        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, item_encoders, global_config.ITEM_COLUMN_NAME,
                                                 config.ENCODERS_NAME,
                                                 config.DICT_OF_TIME_INTERVAL)
 
         dict_mapper = add_values_to_dict_mapper(dict_mapper, store_encoders, global_config.STORE_COLUMN_NAME,
                                                 config.ENCODERS_NAME,
                                                 config.DICT_OF_TIME_INTERVAL)
 
         future_date_range = pd.date_range(start=begin_predict_dates, end=begin_predict_dates, freq='D')
 
         output_dfs = {}
         for store_id in list(store_batch_dict.keys()):
             output_df = pd.DataFrame()
             for _id in store_batch_dict[store_id]:
-                sku_store_id = _id
-                sku = int(sku_store_id.split(',')[0])
-                store = int(sku_store_id.split(',')[1])
+                item_store_id = _id
+                item = int(item_store_id.split(',')[0])
+                store = int(item_store_id.split(',')[1])
                 id_data_future = pd.DataFrame({'date': future_date_range,
-                                               'sku, store': sku_store_id,
-                                               'sku': sku,
+                                               'item, store': item_store_id,
+                                               'item': item,
                                                'store': store})
                 id_data_future = process_date_column(id_data_future, global_config.DATE_COLUMN_NAME, expanded=True)
 
                 # Exclude Sunday
                 # id_data_future = id_data_future[id_data_future['day_of_week'] != 6]
 
-                marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(marketing_plan[global_config.DATE_COLUMN_NAME])
-                id_data_future = pd.merge(id_data_future, marketing_plan, on=[global_config.DATE_COLUMN_NAME], how='left')
+                marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
+                    marketing_plan[global_config.DATE_COLUMN_NAME])
+                id_data_future = pd.merge(id_data_future, marketing_plan, on=[global_config.DATE_COLUMN_NAME],
+                                          how='left')
                 id_data_future = map_encoders_columns_to_base_df(id_data_future, dict_mapper, config.ENCODERS_NAME)
                 output_df = pd.concat([output_df, id_data_future])
 
-            #output_df.drop('name_of_day', axis=1, inplace=True)
+            # output_df.drop('name_of_day', axis=1, inplace=True)
             output_dfs[store_id] = output_df
-
-        return output_dfs
+        return output_dfs
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/features/weather_features.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/features/weather_features.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,47 +4,70 @@
 from . import config as config
 
 import pandas as pd
 from meteostat import Point, Daily
 from datetime import datetime
 
 
-class StoreLocationLoader:
-
-    @classmethod
-    def load(cls, dataset_project=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_project'],
-             dataset_name=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_name'],
-             dataset_version=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_version'],
-             dataset_tags=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_tags'],
-             dataset_file_name=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_file_name']
-             ):
-        store_location_dfs = DatasetLoader().load_dfs_from_dataset(dataset_project=dataset_project,
-                                                                   dataset_name=dataset_name,
-                                                                   dataset_version=dataset_version,
-                                                                   dataset_tags=dataset_tags,
-                                                                   dataset_file_names=[dataset_file_name])
-        store_location_df = store_location_dfs[dataset_file_name]
-        store_location_df = store_location_df.drop('Unnamed: 0', axis=1)
-
-        return store_location_df
+# class StoreLocationLoader:
+#
+#     @classmethod
+#     def load(cls, dataset_project=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_project'],
+#              dataset_name=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_name'],
+#              dataset_version=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_version'],
+#              dataset_tags=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_tags'],
+#              dataset_file_name=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_file_name']
+#              ):
+#         store_location_dfs = DatasetLoader().load_dfs_from_dataset(dataset_project=dataset_project,
+#                                                                    dataset_name=dataset_name,
+#                                                                    dataset_version=dataset_version,
+#                                                                    dataset_tags=dataset_tags,
+#                                                                    dataset_file_names=[dataset_file_name])
+#         store_location_df = store_location_dfs[dataset_file_name]
+#         store_location_df = store_location_df.drop('Unnamed: 0', axis=1)
+#
+#         return store_location_df
 
 
 class WeatherFeatureGenerator:
     @classmethod
     def load(cls, store_location_df, store_id, start_date, end_date, weather_columns=config.WEATHER_COLUMNS):
+        """
+        Load weather data for specific store
+        Args:
+            store_location_df:  store location dataframe
+            store_id:         store id
+            start_date:     start date
+            end_date:    end date
+            weather_columns:    weather columns
+
+        Returns:
+            dataframe: dataframe with weather data for specific store
+        """
         store_weather_df = cls.return_df_of_stores_weather(stores_location_df=store_location_df,
                                                           store_id=store_id,
                                                           start_date_str=start_date,
                                                           end_date_str=end_date,
                                                           weather_columns=weather_columns)
 
         return store_weather_df
 
     @classmethod
     def return_weather_daily_data_for_specific_location(cls, start_date, end_date, latitude, longitude):
+        """
+        Return weather data for specific location and time period
+        Args:
+            start_date:     start date
+            end_date:   end date
+            latitude:   latitude
+            longitude:  longitude
+
+        Returns:
+            dataframe: dataframe with weather data for specific location and time period
+        """
         start = datetime.strptime(start_date, '%Y-%m-%d')
         end = datetime.strptime(end_date, '%Y-%m-%d')
         vienna = Point(float(latitude), float(longitude))
         data = Daily(vienna, start, end)
         data = data.fetch()
         if "tavg" in data.columns:
             data['tavg'].interpolate(method='linear', limit_area='outside', inplace=True)
@@ -65,14 +88,28 @@
         data.interpolate('linear', inplace=True)
         return data
 
     @classmethod
     def return_df_of_stores_weather(cls, stores_location_df, store_id, start_date_str, end_date_str, weather_columns,
                                     lat_vienna=48.2082,
                                     lon_vienna=16.3738):
+        """
+        Return weather data for specific store and time period and if not available for vienna
+        Args:
+            stores_location_df:     store location dataframe
+            store_id:   store id
+            start_date_str:     start date
+            end_date_str:   end date
+            weather_columns:    weather columns
+            lat_vienna:     latitude_vienna
+            lon_vienna:     longitude_vienna
+
+        Returns:
+            dataframe: dataframe with weather data for specific store and time period and if not available for vienna
+        """
 
         start_date = datetime.strptime(start_date_str, "%Y-%m-%d").date()
         end_date = datetime.strptime(end_date_str, "%Y-%m-%d").date()
         delta = end_date - start_date
 
         stores_location_df['store_id'] = stores_location_df['store_id'].astype(int)
 
@@ -92,13 +129,25 @@
         df_weather_of_store['store'] = store_id
         df_weather_of_store['store'] = df_weather_of_store['store'].astype(int)
 
 
         return df_weather_of_store.reset_index().rename(columns={"index": "date", "time": "date"})
 
     @classmethod
-    def generate(cls, store_id, start_predict_date, end_predict_date, weather_columns=config.WEATHER_COLUMNS):
-        store_location_df = StoreLocationLoader.load()
+    def generate(cls, store_location_df, store_id, start_predict_date, end_predict_date, weather_columns=config.WEATHER_COLUMNS):
+        """
+        Generate weather data for specific store and time period
+        Args:
+            store_location_df:      store location dataframe
+            store_id:     store id
+            start_predict_date:     start date
+            end_predict_date:   end date
+            weather_columns:    weather columns
+
+        Returns:
+            dataframe: dataframe with weather data for specific store and time period
+        """
+        # store_location_df = StoreLocationLoader.load()
         store_weather_df = cls.load(store_location_df=store_location_df, store_id=store_id, start_date=start_predict_date, end_date=end_predict_date, weather_columns=weather_columns)
         return store_weather_df
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/config_batch_dict.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/config_batch_dict.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/event_feature_test.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/event_feature_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 def test_event_features_generate():
     generator = EventFeaturesGenerator()
     preprocessor = Preprocessor()
     stores = ['4906', '3']
     df = RegularDataLoader().load()
     df = df[df['store'].isin(stores)]
-    skus_1 = df[df['store'] == '4906']['sku'].unique()[0:5]
-    skus_2 = df[df['store'] == '3']['sku'].unique()[0:5]
-    df = df[df['sku'].isin(skus_1) | df['sku'].isin(skus_2)]
+    skus_1 = df[df['store'] == '4906']['item'].unique()[0:5]
+    skus_2 = df[df['store'] == '3']['item'].unique()[0:5]
+    df = df[df['item'].isin(skus_1) | df['item'].isin(skus_2)]
 
     df = generator.generate(regular_data_df = df)
     print(df)
     print(df.info())
 
 
 def test_event_encoding_features_loader():
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/features_test.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/features_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import sys
 sys.path.append('../..')
-from src.palmers_preprocessing.features.future_features import MarketingPlanFeatures, SkuSaleEncodedFeatures, \
+from src.palmers_preprocessing.features.future_features import MarketingPlanFeatures, ItemSaleEncodedFeatures, \
     StoreSaleEncodedFeatures, FarFutureFeaturesGenerator
 from src.palmers_preprocessing.clearml_data_handler import TaskLoader, ArtifactLoader
 
 
 def test_marketing_plan_features():
     mpf = MarketingPlanFeatures()
     df = mpf.load()
     print(df)
     print(df.info())
 
 def test_sku_sale_encoded_features():
-    ssef = SkuSaleEncodedFeatures()
+    ssef = ItemSaleEncodedFeatures()
     df = ssef.load()
     print(df)
     print(df.info())
 
 
 def test_store_sale_encoded_features():
     ssef = StoreSaleEncodedFeatures()
```

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/lags_features_test.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/lags_features_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/sanity_checks.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.7/src/palmers_preprocessing/tests/weather_test.py` & `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/weather_test.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.7/LICENSE` & `palmers_preprocess-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.7/pyproject.toml` & `palmers_preprocess-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_preprocess"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_preprocess-0.0.7/PKG-INFO` & `palmers_preprocess-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_preprocess
-Version: 0.0.7
+Version: 0.0.8
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Roy  <roy@sdatta.ai>, Assaf <assafm@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

