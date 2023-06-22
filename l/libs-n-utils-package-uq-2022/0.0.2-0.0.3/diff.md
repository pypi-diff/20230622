# Comparing `tmp/libs_n_utils_package_uq_2022-0.0.2.tar.gz` & `tmp/libs_n_utils_package_uq_2022-0.0.3.tar.gz`

## Comparing `libs_n_utils_package_uq_2022-0.0.2.tar` & `libs_n_utils_package_uq_2022-0.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/__init__.py
--rwxr-xr-x   0        0        0     2747 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_NN_functional.py
--rwxr-xr-x   0        0        0     6968 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_NN_models.py
--rwxr-xr-x   0        0        0     1984 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_binary_classification.py
--rwxr-xr-x   0        0        0     7534 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_data_preprocessing.py
--rwxr-xr-x   0        0        0     3982 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_dataframe_manipulation.py
--rwxr-xr-x   0        0        0     9038 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_embedding.py
--rwxr-xr-x   0        0        0    12691 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_feature_calculation.py
--rwxr-xr-x   0        0        0    10595 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_file_manipulation.py
--rwxr-xr-x   0        0        0     3294 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_flow.py
--rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_helpers.py
--rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_imbalance.py
--rwxr-xr-x   0        0        0     5253 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_pandas_extensions.py
--rwxr-xr-x   0        0        0    37598 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_plotters.py
--rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_small_utils.py
--rwxr-xr-x   0        0        0     8975 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/lib_stat_distribution.py
--rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/lib/my_easy_logger.py
--rwxr-xr-x   0        0        0     2909 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/3class_ds_select_save.py
--rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/MI_feature_importance.py
--rwxr-xr-x   0        0        0     7432 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/RF_feature_importance.py
--rwxr-xr-x   0        0        0     3367 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/RF_feimp_weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0     2090 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/UNSW_NB15_data_preparation.py
--rwxr-xr-x   0        0        0     5956 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/alternate_feature_wasserstein.py
--rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/attack_types.py
--rwxr-xr-x   0        0        0     1947 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/average_wasserstein.py
--rwxr-xr-x   0        0        0     7705 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/boruta_feature_selection.py
--rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/boruta_visualisation.py
--rwxr-xr-x   0        0        0     1878 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/combine_2feather.py
--rwxr-xr-x   0        0        0     3105 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/combine_2pickles.py
--rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/combine_3pickles.py
--rwxr-xr-x   0        0        0     3851 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/combine_folder_csv.py
--rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/compare_pickle_files_in_folder.py
--rwxr-xr-x   0        0        0      767 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/csv_folder_to_feather_folder.py
--rwxr-xr-x   0        0        0      893 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/csv_folder_to_pickle_folder.py
--rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/datasets_information.py
--rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/dict_manipulation.py
--rwxr-xr-x   0        0        0     3281 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/edit_CIC.py
--rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/edit_CIC_ton.py
--rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/feather_2m_sel_cols.py
--rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/feather_fldr_2_pickle_fldr.py
--rwxr-xr-x   0        0        0    12322 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/inter_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     3215 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/intra_dataset_feature_wasserstein.py
--rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/make_cics_compatible.py
--rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/make_unity_fi_pickle.py
--rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/netflow_preprocessing.py
--rwxr-xr-x   0        0        0     2332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/pickle_fldr_2_feather_fldr.py
--rwxr-xr-x   0        0        0     1402 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/plot_MI_feature_importances.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/plot_RF_feature_importance_differences.py
--rwxr-xr-x   0        0        0     1829 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/print_feature_selction_results.py
--rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/reading_txt_files.py
--rwxr-xr-x   0        0        0     4726 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/sample_save_fldr_datasets.py
--rwxr-xr-x   0        0        0     4879 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/weighted_average_alternate_wasserstein.py
--rwxr-xr-x   0        0        0     3332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/utilities/weighted_average_wasserstein.py
--rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/LICENSE
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/README.md
--rwxr-xr-x   0        0        0      594 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/__init__.py
+-rwxr-xr-x   0        0        0     2751 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_NN_functional.py
+-rwxr-xr-x   0        0        0     6972 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_NN_models.py
+-rwxr-xr-x   0        0        0     1992 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_binary_classification.py
+-rwxr-xr-x   0        0        0     7538 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_data_preprocessing.py
+-rwxr-xr-x   0        0        0     3986 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_dataframe_manipulation.py
+-rwxr-xr-x   0        0        0     9122 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_embedding.py
+-rwxr-xr-x   0        0        0    12695 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_feature_calculation.py
+-rwxr-xr-x   0        0        0    10603 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_file_manipulation.py
+-rwxr-xr-x   0        0        0     3298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_flow.py
+-rwxr-xr-x   0        0        0     1287 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_helpers.py
+-rwxr-xr-x   0        0        0     3285 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_imbalance.py
+-rwxr-xr-x   0        0        0     5253 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_pandas_extensions.py
+-rwxr-xr-x   0        0        0    37603 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_plotters.py
+-rwxr-xr-x   0        0        0      395 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_small_utils.py
+-rwxr-xr-x   0        0        0     8979 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/lib_stat_distribution.py
+-rwxr-xr-x   0        0        0     4390 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/lib/my_easy_logger.py
+-rwxr-xr-x   0        0        0     2913 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/3class_ds_select_save.py
+-rwxr-xr-x   0        0        0     4168 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/MI_feature_importance.py
+-rwxr-xr-x   0        0        0     7436 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/RF_feature_importance.py
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/RF_feimp_weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0     2090 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/UNSW_NB15_data_preparation.py
+-rwxr-xr-x   0        0        0     5964 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/alternate_feature_wasserstein.py
+-rwxr-xr-x   0        0        0      346 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/attack_types.py
+-rwxr-xr-x   0        0        0     1955 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/average_wasserstein.py
+-rwxr-xr-x   0        0        0     7709 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/boruta_feature_selection.py
+-rwxr-xr-x   0        0        0      613 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/boruta_visualisation.py
+-rwxr-xr-x   0        0        0     1882 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_2feather.py
+-rwxr-xr-x   0        0        0     3109 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_2pickles.py
+-rwxr-xr-x   0        0        0     3278 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_3pickles.py
+-rwxr-xr-x   0        0        0     3859 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/combine_folder_csv.py
+-rwxr-xr-x   0        0        0     1051 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/compare_pickle_files_in_folder.py
+-rwxr-xr-x   0        0        0      771 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/csv_folder_to_feather_folder.py
+-rwxr-xr-x   0        0        0      893 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/csv_folder_to_pickle_folder.py
+-rwxr-xr-x   0        0        0      494 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/datasets_information.py
+-rwxr-xr-x   0        0        0     1239 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/dict_manipulation.py
+-rwxr-xr-x   0        0        0     3289 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/edit_CIC.py
+-rwxr-xr-x   0        0        0     1443 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/edit_CIC_ton.py
+-rwxr-xr-x   0        0        0     1112 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/feather_2m_sel_cols.py
+-rwxr-xr-x   0        0        0     1298 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/feather_fldr_2_pickle_fldr.py
+-rwxr-xr-x   0        0        0    12334 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/inter_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     3231 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/intra_dataset_feature_wasserstein.py
+-rwxr-xr-x   0        0        0     5404 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/make_cics_compatible.py
+-rwxr-xr-x   0        0        0     2082 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/make_unity_fi_pickle.py
+-rwxr-xr-x   0        0        0    14129 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/netflow_preprocessing.py
+-rwxr-xr-x   0        0        0     2332 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/pickle_fldr_2_feather_fldr.py
+-rwxr-xr-x   0        0        0     1406 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/plot_MI_feature_importances.py
+-rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/plot_RF_feature_importance_differences.py
+-rwxr-xr-x   0        0        0     1833 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/print_feature_selction_results.py
+-rwxr-xr-x   0        0        0     1293 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/reading_txt_files.py
+-rwxr-xr-x   0        0        0     4730 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/sample_save_fldr_datasets.py
+-rwxr-xr-x   0        0        0     4883 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/weighted_average_alternate_wasserstein.py
+-rwxr-xr-x   0        0        0     3340 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/utilities/weighted_average_wasserstein.py
+-rwxr-xr-x   0        0        0     1073 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/README.md
+-rwxr-xr-x   0        0        0      594 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 libs_n_utils_package_uq_2022-0.0.3/PKG-INFO
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_NN_functional.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_NN_functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import inspect
 import tensorflow as tf
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_purple,bg_white'
 
 METRICS = [
     tf.keras.metrics.TruePositives(name='tp'),
     tf.keras.metrics.FalsePositives(name='fp'),
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_NN_models.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_NN_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import inspect
 import os
 import tensorflow as tf
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_purple,bg_white'
 # TODO: BatchNormalization 
 
 # metrics for evaluation (not loss function) --------
 METRICS = [
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_binary_classification.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_binary_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 # import psutil
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 from config_template import NetFlow_v2, NN
 import inspect
 
 seed_ = NN.seeds
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
@@ -28,15 +28,15 @@
 
 
 
 # *--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*--*
 def get_AK_model(x_train_, y_train_, x_test_, y_test_, dataset_name, dest_fldr=None, epochs_=None):
     import tensorflow as tf
     import autokeras as ak
-    from lib_NN_models import METRICS
+    from lib.lib_NN_models import METRICS
     tf.random.set_seed(seed_)
     func_name = inspect.stack()[0][3]
     logger_ = my_logger(
         reporter_file_name=script_name,
         info_c='fg_blue,bg_black',
         reporter_func_name=func_name,
         log_level='debug'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_data_preprocessing.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_data_preprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import _pickle as pickle
 import feather
 import numpy as np
 import pandas as pd
 from sklearn import preprocessing
 from sklearn.model_selection import train_test_split
 from lib_binary_classification import netflow_identifiers, seed_, netflow_columns
-from my_easy_logger import logger_cleaner
+from lib.my_easy_logger import logger_cleaner
 
 
 
 
 
 # ---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**
 @logger_cleaner
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_dataframe_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_dataframe_manipulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import numpy as np
 import os
 
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_purple,bg_white'
 
 
 # ######################################################################################################################
 def nunique_groups(dataframe, field_list, value_field=None, log_msg=None):
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_embedding.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import os
 import feather
 import umap
 import pandas as pd
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE, LocallyLinearEmbedding, MDS, SpectralEmbedding
-from sklearn.preprocessing import MinMaxScaler
+from sklearn.preprocessing import StandardScaler, MinMaxScaler
 from sklearn.discriminant_analysis import LinearDiscriminantAnalysis
+from sklearn.impute import SimpleImputer
+import numpy as np
 import config_template
-from lib_feature_calculation import features_calculation
-from my_easy_logger import logger_cleaner
+from lib.lib_feature_calculation import features_calculation
+from lib.my_easy_logger import logger_cleaner
 import matplotlib.pyplot as plt
 
 script_name = os.path.split(__file__)[1]
 groupby_features = config_template.features.groupby_features
 features_class = config_template.features()
 ds_colors = config_template.plot_parameters.dataset_edgecolors
 ds_short_names = config_template.plot_parameters.dataset_shorts
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_feature_calculation.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_feature_calculation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import _pickle as pickle
 import feather
 import pandas as pd
 import config_template
 import os
 from datetime import datetime
-from my_easy_logger import logger_cleaner
+from lib.my_easy_logger import logger_cleaner
 from config_template import NetFlow_fields
 from lib_file_manipulation import create_ReadMe
 
 param_dic = config_template.plot_parameters.CDFplot_params_dic
 groupby_features = config_template.features.groupby_features
 features_class = config_template.features()
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_file_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_file_manipulation.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 import re
 import time
 import feather
 import _pickle as pickle
 import gc
 import pandas as pd
 
-from lib_pandas_extensions import rapid_csv_read
-from my_easy_logger import my_logger, logger_cleaner
+from lib.lib_pandas_extensions import rapid_csv_read
+from lib.my_easy_logger import my_logger, logger_cleaner
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'fg_bold_black,bg_white'
 
 
 # ######################################################################################################################
 @logger_cleaner
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_flow.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_flow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import pandas as pd
 import os
 
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'blue,bg_white'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_helpers.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_helpers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import inspect
 
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'black,bg_white'
 
 
 
 # ######################################################################################################################
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_imbalance.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_imbalance.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_pandas_extensions.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_pandas_extensions.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_plotters.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_plotters.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 import seaborn as sns
 import numpy as np
 import os
 import config_template
 import matplotlib.transforms
 from matplotlib import pyplot as plt
 from plotly import express as px
+from lib.my_easy_logger import logger_cleaner
 from lib_small_utils import random_hex_color
-from my_easy_logger import logger_cleaner
+
 
 param_dic = config_template.plot_parameters.CDFplot_params_dic
 dataset_colors = config_template.plot_parameters.dataset_colors
 
 filename = os.path.split(__file__)[1]
 info_log_color = 'purple,bg_yellow'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/lib_stat_distribution.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/lib_stat_distribution.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 
 import numpy as np
 from scipy.stats import wasserstein_distance
 from config_template import NN
 from lib_data_preprocessing import get_binary_prepared
 from lib_plotters import plot_hist_list
-from my_easy_logger import logger_cleaner
+from lib.my_easy_logger import logger_cleaner
 
 seed_ = NN.seeds
 
 
 # ----------------------------------------------------------------------------------------------------------------------
 @logger_cleaner
 def compute_CDF(_values_df, column=0, **kwargs):
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/lib/my_easy_logger.py` & `libs_n_utils_package_uq_2022-0.0.3/lib/my_easy_logger.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/3class_ds_select_save.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/3class_ds_select_save.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 
 import os
 import pickle
 import gc
 import inspect
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 import time
 
 filename = os.path.split(__file__)[1]
 
 
 def select_dos_rows(_src_fldr, _dst_fldr, new_name_ext='3class_'):
     func_name = inspect.stack()[0][3]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/MI_feature_importance.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/MI_feature_importance.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/RF_feature_importance.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/RF_feature_importance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import os
 import warnings
 import pandas as pd
 import _pickle as pickle
 from sklearn.ensemble import RandomForestClassifier
-from my_easy_logger import my_logger, logger_cleaner
+from lib.my_easy_logger import my_logger, logger_cleaner
 from intra_dataset_feature_wasserstein import get_dataset_prepared
 
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
     info_c='bold_blue',
     reporter_func_name=__name__,
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/RF_feimp_weighted_average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/RF_feimp_weighted_average_wasserstein.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import _pickle as pickle
 from intra_dataset_feature_wasserstein import plot_wasserstein_table
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger
+from lib.lib_plotters import draw_bar_chart
+from lib.my_easy_logger import my_logger
 
 script_name = os.path.split(__file__)[1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/UNSW_NB15_data_preparation.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/UNSW_NB15_data_preparation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/alternate_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/alternate_feature_wasserstein.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 import inspect
 import os
 import _pickle as pickle
 import pandas as pd
 from scipy.stats import wasserstein_distance
 
 from intra_dataset_feature_wasserstein import get_dataset_prepared
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger, logger_cleaner
+from lib.lib_plotters import draw_bar_chart
+from lib.my_easy_logger import my_logger, logger_cleaner
 
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
     info_c='bold_blue',
     reporter_func_name=__name__,
     log_level='debug'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/average_wasserstein.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import _pickle as pickle
 from intra_dataset_feature_wasserstein import plot_wasserstein_table
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger
+from lib.lib_plotters import draw_bar_chart
+from lib.my_easy_logger import my_logger
 
 script_name = os.path.split(__file__)[1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/boruta_feature_selection.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/boruta_feature_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 import os
 import warnings
 import pandas as pd
 import _pickle as pickle
 from sklearn.ensemble import RandomForestClassifier
 from boruta import BorutaPy
-from my_easy_logger import my_logger, logger_cleaner
+from lib.my_easy_logger import my_logger, logger_cleaner
 from intra_dataset_feature_wasserstein import get_dataset_prepared
 
 script_name = os.path.split(__file__)[1][:-3]
 logger = my_logger(
     reporter_file_name=script_name,
     info_c='bold_blue',
     reporter_func_name=__name__,
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/boruta_visualisation.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/boruta_visualisation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/combine_2feather.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/combine_2feather.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import pandas as pd
 import feather
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 
 filename = os.path.split(__file__)[1]
 
 
 def combine_2feather(feather_file1, feather_file2):
     logger_ = my_logger(reporter_file_name=filename,
                         reporter_func_name=__name__,
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/combine_2pickles.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/combine_2pickles.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import itertools
 import os
 import pandas as pd
 import pickle
 import gc
 from functools import lru_cache
 from datetime import datetime
-from my_easy_logger import my_logger, logger_cleaner
+from lib.my_easy_logger import my_logger, logger_cleaner
 
 scriptname = os.path.split(__file__)[1]
 
 @logger_cleaner
 @lru_cache()
 def combine_2pickle(pickle_file1, pickle_file2, **kwargs):
     func_name = inspect.stack()[0][3]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/combine_3pickles.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/combine_3pickles.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import pandas as pd
 import pickle
 import gc
 import itertools
 from datetime import datetime
 from functools import lru_cache
-from my_easy_logger import my_logger, logger_cleaner
+from lib.my_easy_logger import my_logger, logger_cleaner
 
 scriptname = os.path.split(__file__)[1]
 
 
 # ~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X~~~X
 @logger_cleaner
 @lru_cache()
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/combine_folder_csv.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/combine_folder_csv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import pandas as pd
 import gc
 import _pickle as pickle
 import datetime
 
-from my_easy_logger import my_logger
-from lib_pandas_extensions import rapid_csv_read
+from lib.my_easy_logger import my_logger
+from lib.lib_pandas_extensions import rapid_csv_read
 
 filename = os.path.split(__file__)[1]
 
 
 
 if __name__ == '__main__':
     log_file = f'../../outputs/logs/{filename[:-3]}-' \
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/compare_pickle_files_in_folder.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/compare_pickle_files_in_folder.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/csv_folder_to_feather_folder.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/csv_folder_to_feather_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from lib_file_manipulation import csvfile_2_featherfile
+from lib.lib_file_manipulation import csvfile_2_featherfile
 from config_template import FlowMeter
 
 cols = FlowMeter.columns
 
 csv_folder = '/storage/datasets/Comscentre2017/Elasticsearch_CSV_full_headers/'
 feather_folder = '/storage/datasets/Comscentre2017/feather/'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/csv_folder_to_pickle_folder.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/csv_folder_to_pickle_folder.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/dict_manipulation.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/dict_manipulation.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/edit_CIC.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/edit_CIC.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import pandas as pd
 import numpy as np
 from config_template import FlowMeter
 import gc
 import os
 
-from lib_pandas_extensions import rapid_csv_read
-from my_easy_logger import my_logger
+from lib.lib_pandas_extensions import rapid_csv_read
+from lib.my_easy_logger import my_logger
 
 cols = FlowMeter.columns
 cols.remove('Attack')
 script_name = os.path.split(__file__)[1][:-3]
 ds_names = ['BoT_IoT', 'IDS_2018', 'ToN_IoT']
 ds_names = ['ToN_IoT']
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/edit_CIC_ton.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/edit_CIC_ton.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/feather_2m_sel_cols.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/feather_2m_sel_cols.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/feather_fldr_2_pickle_fldr.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/feather_fldr_2_pickle_fldr.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/inter_dataset_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/inter_dataset_feature_wasserstein.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import os
 import pickle
 import re
 
 import numpy as np
 
 from config_template import NetFlow_v2, FlowMeter
-from lib_plotters import plot_wasserstein_table
-from lib_stat_distribution import inter_dataset_wasserstein_table
-from my_easy_logger import my_logger, logger_cleaner
+from lib.lib_plotters import plot_wasserstein_table
+from lib.lib_stat_distribution import inter_dataset_wasserstein_table
+from lib.my_easy_logger import my_logger, logger_cleaner
 
 script_name = os.path.split(__file__)[1][:-3]
 
 
 
 
 @logger_cleaner
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/intra_dataset_feature_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/intra_dataset_feature_wasserstein.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 This scripts computes the wasserstein distances between attack classes
 and plots them using heat-maps
 """
 
 import os
 
-from lib_data_preprocessing import get_dataset_prepared
-from lib_plotters import plot_wasserstein_table
-from lib_stat_distribution import intra_dataset_wasserstein_table
-from my_easy_logger import my_logger, logger_cleaner
+from lib.lib_data_preprocessing import get_dataset_prepared
+from lib.lib_plotters import plot_wasserstein_table
+from lib.lib_stat_distribution import intra_dataset_wasserstein_table
+from lib.my_easy_logger import my_logger, logger_cleaner
 
 script_name = os.path.split(__file__)[1][:-3]
 
 
 
 
 # ---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**---**
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/make_cics_compatible.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/make_cics_compatible.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/make_unity_fi_pickle.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/make_unity_fi_pickle.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/netflow_preprocessing.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/netflow_preprocessing.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/pickle_fldr_2_feather_fldr.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/pickle_fldr_2_feather_fldr.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/plot_MI_feature_importances.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/plot_MI_feature_importances.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import _pickle as pickle
 import os
 import matplotlib.pyplot as plt
-from lib_plotters import draw_bar_chart
+from lib.lib_plotters import draw_bar_chart
 
 fn = 'feature_importance_using_mi_39_features_NF-UNSW-NB15-v2_whole_rows.pickle'
 fldr = '/home/nids1/Desktop/ZSL_visualizations'
 addr = os.path.join(fldr, fn)
 mi_dict = pickle.load(open(addr, 'rb'))
 keys = list(mi_dict.keys())
 attacks = keys[:-1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/plot_RF_feature_importance_differences.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/plot_RF_feature_importance_differences.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/print_feature_selction_results.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/print_feature_selction_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import os
 import _pickle as pickle
 import math
 from scipy.stats import binom
 from datetime import datetime
-from my_easy_logger import my_logger
+from lib.my_easy_logger import my_logger
 
 
 filename = os.path.split(__file__)[1]
 
 
 def boruta_result_interpret(n_trial, rank_value_list, probability=0.5):
     # pmf = [binom.pmf(x, n_trial, probability) for x in range(n_trial + 1)]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/reading_txt_files.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/reading_txt_files.py`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/sample_save_fldr_datasets.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/sample_save_fldr_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import _pickle as pickle
 import gc
 from datetime import datetime
 
 import pandas as pd
 
-from my_easy_logger import my_logger, logger_cleaner
+from lib.my_easy_logger import my_logger, logger_cleaner
 from config_template import NN
 from pickle_fldr_2_feather_fldr import get_df_dtypes
 
 script_name = os.path.split(__file__)[1][:-3]
 
 
 # ---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*---*
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/weighted_average_alternate_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/weighted_average_alternate_wasserstein.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 to go without weights
 """
 
 
 import os
 import pickle
-from lib_plotters import draw_bar_chart
+from lib.lib_plotters import draw_bar_chart
 import pandas as pd
 
 
 # src_fldr = '/home/nids1/Desktop/ZSL_visualizations/NetFlow/'
 # save_fldr = '/home/nids1/Desktop/ZSL_visualizations/alternate_feature_wasserstein/'
 src_fldr = '/home/nids1/Desktop/ZSL_visualizations/original_ds/src/'
 save_fldr = '/home/nids1/Desktop/ZSL_visualizations/original_ds'
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/utilities/weighted_average_wasserstein.py` & `libs_n_utils_package_uq_2022-0.0.3/utilities/weighted_average_wasserstein.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import numpy as np
 import _pickle as pickle
 from intra_dataset_feature_wasserstein import plot_wasserstein_table
-from lib_plotters import draw_bar_chart
-from my_easy_logger import my_logger
+from lib.lib_plotters import draw_bar_chart
+from lib.my_easy_logger import my_logger
 
 script_name = os.path.split(__file__)[1]
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/LICENSE` & `libs_n_utils_package_uq_2022-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libs_n_utils_package_uq_2022-0.0.2/pyproject.toml` & `libs_n_utils_package_uq_2022-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "libs_n_utils_package_uq_2022"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="siamak layeghy", email="siamak.layeghy@uq.net.au" },
 ]
 description = "A small library of utilities"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `libs_n_utils_package_uq_2022-0.0.2/PKG-INFO` & `libs_n_utils_package_uq_2022-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libs_n_utils_package_uq_2022
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small library of utilities
 Project-URL: Homepage, https://github.com/layeghy/libs_n_utils
 Project-URL: Bug Tracker, https://github.com/layeghy/libs_n_utils/issues
 Author-email: siamak layeghy <siamak.layeghy@uq.net.au>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

