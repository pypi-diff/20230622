# Comparing `tmp/palmers_preprocess-0.0.8.tar.gz` & `tmp/palmers_preprocess-0.0.9.tar.gz`

## Comparing `palmers_preprocess-0.0.8.tar` & `palmers_preprocess-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/__init__.py
--rw-r--r--   0        0        0     5181 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/clearml_data_handler.py
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/config.py
--rw-r--r--   0        0        0    42984 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/events_handler.py
--rw-r--r--   0        0        0     5254 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/lags_feature_handler.py
--rw-r--r--   0        0        0    10060 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/preprocessor.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/regular_data_handler.py
--rw-r--r--   0        0        0     9835 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/__init__.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/config.py
--rw-r--r--   0        0        0     8120 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/cumulative_features.py
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/event_features.py
--rw-r--r--   0        0        0     8989 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/future_features.py
--rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/lags_features.py
--rw-r--r--   0        0        0     7265 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/features/weather_features.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/__init__.py
--rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/config_batch_dict.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/event_feature_test.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/features_test.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/lags_features_test.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/preprocessor_test.py
--rw-r--r--   0        0        0    50890 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/sanity_checks.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/test_todelete.py
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/weather_test.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/LICENSE
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/README.md
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/__init__.py
+-rw-r--r--   0        0        0     5073 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/clearml_data_handler.py
+-rw-r--r--   0        0        0     6103 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/config.py
+-rw-r--r--   0        0        0    42164 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/events_handler.py
+-rw-r--r--   0        0        0     5144 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/lags_feature_handler.py
+-rw-r--r--   0        0        0     9869 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/preprocessor.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/regular_data_handler.py
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/features/__init__.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/features/config.py
+-rw-r--r--   0        0        0     7964 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/features/cumulative_features.py
+-rw-r--r--   0        0        0     7527 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/features/event_features.py
+-rw-r--r--   0        0        0     8798 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/features/future_features.py
+-rw-r--r--   0        0        0     5563 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/features/lags_features.py
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/features/weather_features.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/__init__.py
+-rw-r--r--   0        0        0   719548 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/config_batch_dict.py
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/event_feature_test.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/features_test.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/lags_features_test.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/preprocessor_test.py
+-rw-r--r--   0        0        0    50876 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/sanity_checks.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/test_todelete.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/weather_test.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/LICENSE
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/README.md
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 palmers_preprocess-0.0.9/PKG-INFO
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/clearml_data_handler.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/clearml_data_handler.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,108 +1,108 @@
-import pickle
-
-import pandas as pd
-from clearml import Dataset, Task
-
-
-class DatasetLoader:
-    def __init__(self, dataset_path=None):
-        self.dataset_path = dataset_path
-
-    @classmethod
-    def _validate_dataset_identifier(cls, dataset_id, dataset_name, dataset_project):
-        if dataset_id is None and (dataset_name is None or dataset_project is None):
-            raise ValueError('dataset id cannot be None')
-
-    def download(self, dataset_id=None, dataset_name=None, dataset_project=None, dataset_version=None, tags=None, cache=False):
-        self._validate_dataset_identifier(dataset_id, dataset_name, dataset_project)
-        if (not cache) or self.dataset_path is None:
-            self.dataset_path = Dataset.get(dataset_id=dataset_id,
-                                         dataset_name=dataset_name,
-                                         dataset_project=dataset_project,
-                                         dataset_version=dataset_version,
-                                         dataset_tags=tags
-
-                                         ).get_local_copy()
-        return self.dataset_path
-
-
-    def load_dfs_from_dataset(self, dataset_id=None, dataset_name=None, dataset_project=None, dataset_path=None,
-                              dataset_file_names=None, dataset_version=None, dataset_tags=None, cache=False):
-        if dataset_path is not None:
-            self.dataset_path = dataset_path
-
-        if self.dataset_path is None or (not cache):
-            self.dataset_path = self.download(dataset_id=dataset_id,
-                                                  dataset_project=dataset_project,
-                                                  dataset_name=dataset_name,
-                                                  dataset_version=dataset_version,
-                                                  tags=dataset_tags, cache=cache)
-
-        dfs = {}
-        for file_name in dataset_file_names:
-            if file_name:
-                dataset_file_path = self.dataset_path + '/' + file_name
-                df = pd.read_csv(dataset_file_path, dtype=str)
-                dfs[file_name] = df
-        return dfs
-
-
-class TaskLoader:
-    @classmethod
-    def _validate_task_identifier(cls, task_id, project_name, task_name):
-        if task_id is None and (project_name is None or task_name is None):
-            raise ValueError('task_id cannot be None')
-
-    @classmethod
-    def get_task(cls, task_id=None, project_name=None, task_name=None, tags=None):
-        cls._validate_task_identifier(task_id=task_id, project_name=project_name, task_name=task_name)
-        task = Task.get_task(task_id=task_id, project_name=project_name, task_name=task_name,
-                             tags=tags)
-        return task
-
-
-class ArtifactLoader:
-    def __init__(self):
-        self.artifact_local_path = None
-
-    @classmethod
-    def load_artifacts(cls, project_name=None, task_name=None, task_id=None, tags=None):
-        task = TaskLoader().get_task(task_id=task_id, project_name=project_name, task_name=task_name, tags=tags)
-        return task.artifacts
-
-
-    def download(self, artifact_name, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
-        if self.artifact_local_path is None or (not cache):
-            artifacts = self.load_artifacts(project_name=project_name, task_name=task_name, task_id=task_id, tags=tags)
-            if artifact_name in artifacts:
-                self.artifact_local_path = artifacts[artifact_name].get_local_copy()
-            else:
-                raise ValueError(f"Artifact {artifact_name} not found in task {task_id} {project_name}/{task_name}")
-
-        return self.artifact_local_path
-
-    def download_artifacts(self, artifacts_names, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
-        artifact_paths = {}
-        artifacts = self.load_artifacts(project_name=project_name, task_name=task_name, task_id=task_id, tags=tags)
-        for artifact_name in artifacts_names:
-            if artifact_name in artifacts:
-                artifact_paths[artifact_name] = artifacts[artifact_name].get_local_copy()
-
-        return artifact_paths
-
-
-    def load_artifact_as_df(self, artifact_name, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
-        local_path = self.download(artifact_name=artifact_name, task_id=task_id, project_name=project_name, task_name=task_name, tags=tags, cache=cache)
-        artifact = pd.read_csv(local_path, dtype=str)
-        return artifact
-
-    def load_pickle_artifacts(self, artifacts_names, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
-        local_paths = self.download_artifacts(artifacts_names=artifacts_names, task_id=task_id, project_name=project_name, task_name=task_name, tags=tags, cache=cache)
-        files = {}
-        for artifact_name, local_path in local_paths.items():
-            # read pickle from local_path
-            with open(local_path, 'rb') as f:
-                files[artifact_name] = pickle.load(f)
-
-        return files
-
+import pickle
+
+import pandas as pd
+from clearml import Dataset, Task
+
+
+class DatasetLoader:
+    def __init__(self, dataset_path=None):
+        self.dataset_path = dataset_path
+
+    @classmethod
+    def _validate_dataset_identifier(cls, dataset_id, dataset_name, dataset_project):
+        if dataset_id is None and (dataset_name is None or dataset_project is None):
+            raise ValueError('dataset id cannot be None')
+
+    def download(self, dataset_id=None, dataset_name=None, dataset_project=None, dataset_version=None, tags=None, cache=False):
+        self._validate_dataset_identifier(dataset_id, dataset_name, dataset_project)
+        if (not cache) or self.dataset_path is None:
+            self.dataset_path = Dataset.get(dataset_id=dataset_id,
+                                         dataset_name=dataset_name,
+                                         dataset_project=dataset_project,
+                                         dataset_version=dataset_version,
+                                         dataset_tags=tags
+
+                                         ).get_local_copy()
+        return self.dataset_path
+
+
+    def load_dfs_from_dataset(self, dataset_id=None, dataset_name=None, dataset_project=None, dataset_path=None,
+                              dataset_file_names=None, dataset_version=None, dataset_tags=None, cache=False):
+        if dataset_path is not None:
+            self.dataset_path = dataset_path
+
+        if self.dataset_path is None or (not cache):
+            self.dataset_path = self.download(dataset_id=dataset_id,
+                                                  dataset_project=dataset_project,
+                                                  dataset_name=dataset_name,
+                                                  dataset_version=dataset_version,
+                                                  tags=dataset_tags, cache=cache)
+
+        dfs = {}
+        for file_name in dataset_file_names:
+            if file_name:
+                dataset_file_path = self.dataset_path + '/' + file_name
+                df = pd.read_csv(dataset_file_path, dtype=str)
+                dfs[file_name] = df
+        return dfs
+
+
+class TaskLoader:
+    @classmethod
+    def _validate_task_identifier(cls, task_id, project_name, task_name):
+        if task_id is None and (project_name is None or task_name is None):
+            raise ValueError('task_id cannot be None')
+
+    @classmethod
+    def get_task(cls, task_id=None, project_name=None, task_name=None, tags=None):
+        cls._validate_task_identifier(task_id=task_id, project_name=project_name, task_name=task_name)
+        task = Task.get_task(task_id=task_id, project_name=project_name, task_name=task_name,
+                             tags=tags)
+        return task
+
+
+class ArtifactLoader:
+    def __init__(self):
+        self.artifact_local_path = None
+
+    @classmethod
+    def load_artifacts(cls, project_name=None, task_name=None, task_id=None, tags=None):
+        task = TaskLoader().get_task(task_id=task_id, project_name=project_name, task_name=task_name, tags=tags)
+        return task.artifacts
+
+
+    def download(self, artifact_name, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
+        if self.artifact_local_path is None or (not cache):
+            artifacts = self.load_artifacts(project_name=project_name, task_name=task_name, task_id=task_id, tags=tags)
+            if artifact_name in artifacts:
+                self.artifact_local_path = artifacts[artifact_name].get_local_copy()
+            else:
+                raise ValueError(f"Artifact {artifact_name} not found in task {task_id} {project_name}/{task_name}")
+
+        return self.artifact_local_path
+
+    def download_artifacts(self, artifacts_names, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
+        artifact_paths = {}
+        artifacts = self.load_artifacts(project_name=project_name, task_name=task_name, task_id=task_id, tags=tags)
+        for artifact_name in artifacts_names:
+            if artifact_name in artifacts:
+                artifact_paths[artifact_name] = artifacts[artifact_name].get_local_copy()
+
+        return artifact_paths
+
+
+    def load_artifact_as_df(self, artifact_name, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
+        local_path = self.download(artifact_name=artifact_name, task_id=task_id, project_name=project_name, task_name=task_name, tags=tags, cache=cache)
+        artifact = pd.read_csv(local_path, dtype=str)
+        return artifact
+
+    def load_pickle_artifacts(self, artifacts_names, task_id=None, project_name=None, task_name=None, tags=None, cache=False):
+        local_paths = self.download_artifacts(artifacts_names=artifacts_names, task_id=task_id, project_name=project_name, task_name=task_name, tags=tags, cache=cache)
+        files = {}
+        for artifact_name, local_path in local_paths.items():
+            # read pickle from local_path
+            with open(local_path, 'rb') as f:
+                files[artifact_name] = pickle.load(f)
+
+        return files
+
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/config.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-import datetime
-ITEM_COLUMN_NAME = "item"
-STORE_COLUMN_NAME = "store"
-SALES_COLUMN_NAME = "sales"
-DATE_COLUMN_NAME = "date"
-ITEM_STORE_COLUMN_NAME = "item, store"
-ITEM_STORE_COLUMN_NAME_LIST = ["item", "store"]
-ID_COLUMN_NAME = "id"
-SKU_COLUMN_NAME = "sku"
-LIST_FREQ = ["D", "W-Mon", "M", "Y"]
-START_DATE_CUMULATIVE_FEATURES = "2018-01-01"
-tomorrow_date = str(datetime.datetime.now(datetime.timezone.utc).date()+datetime.timedelta(days=1))
-
-
-DEFAULT_MARKETING_PLAN_FEATURES = {'project_name': 'examples',
-                                   'task_name': 'marketing_plan_feature',
-                                   'task_id': '630578192a1f432bb58240782f47a0d6',
-                                   'artifact_name': 'marketing_plan_feature',
-                                   }
-
-DEFAULT_ITEM_SALE_ENCODED_FEATURES = {'project_name': 'examples',
-                                     'task_name': 'mytest_item_store_sales_encoders_for_daily_preprocess',
-                                     'task_id': 'b8e7efbdb4cc4aedb4da34512eccc30c',
-                                     'artifact_name': 'item_encoders'}
-
-DEFAULT_STORE_SALE_ENCODED_FEATURES = {'project_name': 'examples',
-                                       'task_name': 'mytest_item_store_sales_encoders_for_daily_preprocess',
-                                       'task_id': 'b8e7efbdb4cc4aedb4da34512eccc30c',
-                                       'artifact_name': 'store_encoders'}
-
-DEFAULT_EVENT_DATASET = {'dataset_project': 'palmers/datasets',
-                         'dataset_name': 'fix_events',
-                         'dataset_file_name': 'events_new_fix.csv',
-                         'dataset_version': None,
-                         'dataset_tags': None}
-
-PCA_ENCODER_ARTIFACT_NAME='pca_dict'
-COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME='columns_interactions_encoder'
-APPLY_ENCODINGS_DICT_ARTIFACT_NAME='apply_encodings_dict'
-APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME='apply_encodings_at_once'
-
-
-DEFAULT_EVENT_ENCODING_FEATURES = {'project_name': 'examples',
-                                   'task_name': 'event_feature_fit',
-                                   'task_id' : '8078f92691a54427b5123bc375efdd11',
-                                   'artifacts_names': [APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME, APPLY_ENCODINGS_DICT_ARTIFACT_NAME,
-                                                       COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME, PCA_ENCODER_ARTIFACT_NAME]
-                                   }
-
-
-
-DEFAULT_HOLIDAYS_DATASET = {'dataset_project': 'palmers/datasets',
-                            'dataset_name': 'events_holidays_raw',
-                            'dataset_file_name': 'Holidays - holidays.csv',
-                            'dataset_version': None,
-                            'dataset_tags': None}
-
-DEFAULT_STORE_LOCATION_DATASET = {'dataset_project': 'palmers/datasets',
-                                  'dataset_name': 'stores_location',
-                                  'dataset_file_name': 'store_location_df.csv',
-                                  'dataset_version': None,
-                                  'dataset_tags': None}
-
-DEFAULT_EVENT_HANDLER_VARIABLES = {
-    'max_date': 'max_date',
-    'min_date': 'min_date',
-    'date_min_col_list': "min_date_list",
-    'target_col': 'sales',
-    'date_col': 'date',
-    'start_date': "2018-01-01",
-    'holiday_col': "holiday_name",
-    'holiday_col_type': "type",
-    'duration_list_col': "duration_list",
-    'event_num': 'num_event_id_list',
-    'event_col_even': "event_id_list",
-    'trend_col': 'rolling_7_mean',
-    'window_size_list': list(range(1, 31)),
-    'lags_list': list(range(1, 31)),
-    'event_col_list': ["event_id_list", "sub_event_id_list"],
-    'type_functions': ["mean", "std", "median"],
-    'duration_list_cols': ['duration_list_mean_event', 'duration_list_median_event'],
-    'weekend_col': "is_weekend",
-    'year_forecast': None,  # 2022, not relevant to daily inference
-    'pca_num': 2,
-    'column_list_map_id': ['event_id', 'duration', 'min_date', 'sub_event_id', 'is_old', "max_date"],
-    'cols_to_encode': ["type_holiday_name", "num_sub_event_id_list", "cumulative_sum_sales", "PC1", "PC2", "comments",
-                  "fft_real", "fft_imag", "num_event_id_list", "duration_list_mean_event",
-                  "duration_list_median_event",
-                  "duration_list_std_event", 'is_weekend',
-                  "ind_change_combo_event", 'is_sunday','is_tomorrow_event',"is_2_days_event"],
-
-    'cols_to_encode_at_once':  ["num_sub_event_id_list", "num_event_id_list", "PC1",
-                          "PC2", "fft_real", "fft_imag", "cumulative_sum_sales", "duration_list_mean_event",
-                          "duration_list_std_event",
-                          "duration_list_median_event",'is_tomorrow_event',"is_2_days_event"],
-    'cols_days_for_ineraction' :['day_of_week', 'week_of_year', 'quarter', 'is_weekend', "ind_change_combo_event",
-                            'is_sunday', "is_holday"],
-    'type_encoder_list': ["MEstimateEncoder", "CatBoostEncoder"],
-    'list_col_add': ["date"]
-}
-
-OUTLETS_SDATTA = [3, 18, 22, 28, 29, 44, 51, 57, 63, 73, 74, 76, 79, 88, 89, 91, 96, 100, 117, 119, 123, 130, 133, 135, 136, 141, 143, 144, 149, 150, 152, 162, 164, 166, 167, 168, 171, 172, 175, 179, 181, 184, 185, 186, 188, 189, 202, 214, 216, 217, 226, 3005, 3202, 3205, 3208, 4104, 4123, 4129, 4134, 4803, 4805,4904,4906]
-
-OUTLETS_ALL = [3, 18, 22, 28, 44, 50, 55, 57, 68, 73, 74, 76, 79, 82, 88, 91, 96, 99, 100, 119, 123, 130, 133, 141, 144,
-               149, 152, 162, 164, 166, 167, 168, 171, 173, 175, 180, 181, 184, 185, 186, 188, 189, 202, 203, 214, 216,
-               218, 221, 226, 3005, 3202, 3205, 3208, 3290, 4104, 4123, 4129, 4132, 4133, 4134, 4803, 4805, 4904, 4906,
-               4, 5, 7, 8, 10, 11, 15, 21, 26, 27, 29, 35, 36, 37, 42, 43, 45, 46, 47, 51, 52, 56, 61, 63, 64, 67, 69,
-               81, 84, 85, 89, 90, 95, 104, 105, 106, 109, 114, 117, 121, 122, 135, 136, 143, 147, 150, 156, 159, 160,
-               163, 170, 172, 174, 179, 182, 183, 201, 213, 215, 217, 219, 220, 225, 3245]
+import datetime
+ITEM_COLUMN_NAME = "item"
+STORE_COLUMN_NAME = "store"
+SALES_COLUMN_NAME = "sales"
+DATE_COLUMN_NAME = "date"
+ITEM_STORE_COLUMN_NAME = "item, store"
+ITEM_STORE_COLUMN_NAME_LIST = ["item", "store"]
+ID_COLUMN_NAME = "id"
+SKU_COLUMN_NAME = "sku"
+LIST_FREQ = ["D", "W-Mon", "M", "Y"]
+START_DATE_CUMULATIVE_FEATURES = "2018-01-01"
+tomorrow_date = str(datetime.datetime.now(datetime.timezone.utc).date()+datetime.timedelta(days=1))
+
+
+DEFAULT_MARKETING_PLAN_FEATURES = {'project_name': 'examples',
+                                   'task_name': 'marketing_plan_feature',
+                                   'task_id': '630578192a1f432bb58240782f47a0d6',
+                                   'artifact_name': 'marketing_plan_feature',
+                                   }
+
+DEFAULT_ITEM_SALE_ENCODED_FEATURES = {'project_name': 'examples',
+                                     'task_name': 'mytest_item_store_sales_encoders_for_daily_preprocess',
+                                     'task_id': 'b8e7efbdb4cc4aedb4da34512eccc30c',
+                                     'artifact_name': 'item_encoders'}
+
+DEFAULT_STORE_SALE_ENCODED_FEATURES = {'project_name': 'examples',
+                                       'task_name': 'mytest_item_store_sales_encoders_for_daily_preprocess',
+                                       'task_id': 'b8e7efbdb4cc4aedb4da34512eccc30c',
+                                       'artifact_name': 'store_encoders'}
+
+DEFAULT_EVENT_DATASET = {'dataset_project': 'palmers/datasets',
+                         'dataset_name': 'fix_events',
+                         'dataset_file_name': 'events_new_fix.csv',
+                         'dataset_version': None,
+                         'dataset_tags': None}
+
+PCA_ENCODER_ARTIFACT_NAME='pca_dict'
+COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME='columns_interactions_encoder'
+APPLY_ENCODINGS_DICT_ARTIFACT_NAME='apply_encodings_dict'
+APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME='apply_encodings_at_once'
+
+
+DEFAULT_EVENT_ENCODING_FEATURES = {'project_name': 'examples',
+                                   'task_name': 'event_feature_fit',
+                                   'task_id' : '8078f92691a54427b5123bc375efdd11',
+                                   'artifacts_names': [APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME, APPLY_ENCODINGS_DICT_ARTIFACT_NAME,
+                                                       COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME, PCA_ENCODER_ARTIFACT_NAME]
+                                   }
+
+
+
+DEFAULT_HOLIDAYS_DATASET = {'dataset_project': 'palmers/datasets',
+                            'dataset_name': 'events_holidays_raw',
+                            'dataset_file_name': 'Holidays - holidays.csv',
+                            'dataset_version': None,
+                            'dataset_tags': None}
+
+DEFAULT_STORE_LOCATION_DATASET = {'dataset_project': 'palmers/datasets',
+                                  'dataset_name': 'stores_location',
+                                  'dataset_file_name': 'store_location_df.csv',
+                                  'dataset_version': None,
+                                  'dataset_tags': None}
+
+DEFAULT_EVENT_HANDLER_VARIABLES = {
+    'max_date': 'max_date',
+    'min_date': 'min_date',
+    'date_min_col_list': "min_date_list",
+    'target_col': 'sales',
+    'date_col': 'date',
+    'start_date': "2018-01-01",
+    'holiday_col': "holiday_name",
+    'holiday_col_type': "type",
+    'duration_list_col': "duration_list",
+    'event_num': 'num_event_id_list',
+    'event_col_even': "event_id_list",
+    'trend_col': 'rolling_7_mean',
+    'window_size_list': list(range(1, 31)),
+    'lags_list': list(range(1, 31)),
+    'event_col_list': ["event_id_list", "sub_event_id_list"],
+    'type_functions': ["mean", "std", "median"],
+    'duration_list_cols': ['duration_list_mean_event', 'duration_list_median_event'],
+    'weekend_col': "is_weekend",
+    'year_forecast': None,  # 2022, not relevant to daily inference
+    'pca_num': 2,
+    'column_list_map_id': ['event_id', 'duration', 'min_date', 'sub_event_id', 'is_old', "max_date"],
+    'cols_to_encode': ["type_holiday_name", "num_sub_event_id_list", "cumulative_sum_sales", "PC1", "PC2", "comments",
+                  "fft_real", "fft_imag", "num_event_id_list", "duration_list_mean_event",
+                  "duration_list_median_event",
+                  "duration_list_std_event", 'is_weekend',
+                  "ind_change_combo_event", 'is_sunday','is_tomorrow_event',"is_2_days_event"],
+
+    'cols_to_encode_at_once':  ["num_sub_event_id_list", "num_event_id_list", "PC1",
+                          "PC2", "fft_real", "fft_imag", "cumulative_sum_sales", "duration_list_mean_event",
+                          "duration_list_std_event",
+                          "duration_list_median_event",'is_tomorrow_event',"is_2_days_event"],
+    'cols_days_for_ineraction' :['day_of_week', 'week_of_year', 'quarter', 'is_weekend', "ind_change_combo_event",
+                            'is_sunday', "is_holday"],
+    'type_encoder_list': ["MEstimateEncoder", "CatBoostEncoder"],
+    'list_col_add': ["date"]
+}
+
+OUTLETS_SDATTA = [3, 18, 22, 28, 29, 44, 51, 57, 63, 73, 74, 76, 79, 88, 89, 91, 96, 100, 117, 119, 123, 130, 133, 135, 136, 141, 143, 144, 149, 150, 152, 162, 164, 166, 167, 168, 171, 172, 175, 179, 181, 184, 185, 186, 188, 189, 202, 214, 216, 217, 226, 3005, 3202, 3205, 3208, 4104, 4123, 4129, 4134, 4803, 4805,4904,4906]
+
+OUTLETS_ALL = [3, 18, 22, 28, 44, 50, 55, 57, 68, 73, 74, 76, 79, 82, 88, 91, 96, 99, 100, 119, 123, 130, 133, 141, 144,
+               149, 152, 162, 164, 166, 167, 168, 171, 173, 175, 180, 181, 184, 185, 186, 188, 189, 202, 203, 214, 216,
+               218, 221, 226, 3005, 3202, 3205, 3208, 3290, 4104, 4123, 4129, 4132, 4133, 4134, 4803, 4805, 4904, 4906,
+               4, 5, 7, 8, 10, 11, 15, 21, 26, 27, 29, 35, 36, 37, 42, 43, 45, 46, 47, 51, 52, 56, 61, 63, 64, 67, 69,
+               81, 84, 85, 89, 90, 95, 104, 105, 106, 109, 114, 117, 121, 122, 135, 136, 143, 147, 150, 156, 159, 160,
+               163, 170, 172, 174, 179, 182, 183, 201, 213, 215, 217, 219, 220, 225, 3245]
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/events_handler.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/events_handler.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,820 +1,820 @@
-from typing import List
-import pandas as pd
-import numpy as np
-from scipy.fftpack import fft
-from scipy.signal import argrelextrema
-from sklearn.decomposition import PCA
-from category_encoders import GLMMEncoder, MEstimateEncoder, CatBoostEncoder
-from . import config
-
-
-# TODO: speak to yotam
-def run_pipline_event(data_event, data_sales, data_hol, date_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['date_col'],
-                      start_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['start_date'],
-                      target_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['target_col'],
-                      max_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['max_date'],
-                      min_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['min_date'],
-                      duration_list_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['duration_list_col'],
-                      column_list_map_id=config.DEFAULT_EVENT_HANDLER_VARIABLES['column_list_map_id'],
-                      event_num=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_num'],
-                      event_col_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_col_list'],
-                      event_col_even=config.DEFAULT_EVENT_HANDLER_VARIABLES['event_col_even'],
-                      date_min_col_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['date_min_col_list'],
-                      holiday_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['holiday_col'],
-                      holiday_col_type=config.DEFAULT_EVENT_HANDLER_VARIABLES['holiday_col_type'],
-                      weekend_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['weekend_col'],
-                      year_forecast=config.DEFAULT_EVENT_HANDLER_VARIABLES['year_forecast'],
-                      pca_num=config.DEFAULT_EVENT_HANDLER_VARIABLES['pca_num'],
-                      type_encoder_list=config.DEFAULT_EVENT_HANDLER_VARIABLES['type_encoder_list'],
-                      cols_to_encode=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode'],
-                      cols_to_encode_at_once=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode_at_once'],
-                      cols_days_for_interaction=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_days_for_ineraction'],
-                      list_col_add=config.DEFAULT_EVENT_HANDLER_VARIABLES['list_col_add']):
-    event_preprocess = EventFeatureGenerator()
-    # event_preprocess.change_columns_names_in_dataframe_by_dict(data_sales, column_dict)
-    data_sales0 = event_preprocess.filter_data_by_date(data_sales, date_col, start_date)
-    data_sales_process = event_preprocess.aggregate_data(data_sales0, target_col)
-    data_sales_process1 = event_preprocess.process_date_column(data_sales_process, date_col)
-    data_event_process = event_preprocess.calculate_duration(data_event, max_date, min_date)
-    data_sales_process2 = event_preprocess.identify_event(data_event_process, data_sales_process1, date_col, min_date,
-                                                          max_date)
-    data_sales_process3 = event_preprocess.map_event_to_list(data_sales_process2, data_event_process, max_date,
-                                                             min_date, column_list_map_id, date_col)
-    data_sales_process4 = event_preprocess.add_stat_duartions(data_sales_process3, duration_list_col)
-    data_sales_process5 = event_preprocess.length_list_event(data_sales_process4, event_col_list)
-    data_sales_process6 = event_preprocess.diff_col(data_sales_process5, target_col, date_col)
-    data_sales_process7 = event_preprocess.event_frequency(data_sales_process6, date_col, event_num)
-    data_sales_process8 = event_preprocess.indicate_event_combination_change(data_sales_process7, event_col_even)
-    # data_sales_process9 = event_preprocess.std_on_list(data_sales_process8, event_col_discount_type)
-    data_sales_process10 = event_preprocess.log_col(data_sales_process8, target_col)
-    data_sales_process11 = event_preprocess.caculate_amount_days_pass_from_start_of_event(data_sales_process10,
-                                                                                          date_col, date_min_col_list)
-    data_sales_process12 = event_preprocess.caculate_amount_days_pass_from_start_of_event_most_new(data_sales_process11,
-                                                                                                   date_min_col_list,
-                                                                                                   date_col)
-    data_sales_process13 = event_preprocess.merge_df(data_sales_process12, data_hol, date_col)
-    data_sales_process14 = event_preprocess.identify_date_occasion(data_sales_process13, holiday_col, date_col)
-    data_sales_process15 = event_preprocess.feature_combine_str(data_sales_process14, holiday_col_type, holiday_col)
-    data_sales_process16 = event_preprocess.add_cumulative_sum_column_for_targe(data_sales_process15, target_col)
-    data_sales_process17 = event_preprocess.fft_features(data_sales_process16, target_col)
-    data_sales_process18 = event_preprocess.time_series_shape_features(data_sales_process17, target_col)
-    data_sales_process21 = event_preprocess.convert_str_indicator(data_sales_process18, weekend_col)
-
-    # data_sales_process22 = event_preprocess.extract_features_pca(data_sales_process21, date_col, year_forecast, pca_num,
-    #                                                              target_col, task=task)
-    #
-    data_sales_process23 = event_preprocess.process_next_days_events(data_sales_process21, target_col)
-
-    return data_sales_process23
-
-
-def finalize_data(df: pd.DataFrame) -> pd.DataFrame:
-    """
-    Finalize data for model removing unnecessary columns
-    Args:
-        df: data event features
-
-    Returns:
-        df
-    """
-    event_preprocess = EventFeatureGenerator()
-    data_sales_process27 = event_preprocess.remove_expand_dates(df)
-    data_final_event = data_sales_process27.copy()
-    return data_final_event
-
-
-class EventFeatureGenerator:
-    @classmethod
-    def aggregate_data(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
-        """
-        Aggregate data by date
-        Args:
-            target_col:     name of target column
-            df_sales:      pandas DataFrame
-
-        Returns:   aggregate by target_col pandas DataFrame
-
-        """
-        df_sales[target_col] = df_sales[target_col].astype(np.float64)
-        return df_sales.groupby(['date'])[target_col].sum(numeric_only=True).reset_index()
-
-    @classmethod
-    def filter_data_by_date(cls, df_sales: pd.DataFrame, date_col: str, start_date: str) -> pd.DataFrame:
-        """
-        Filter data by date
-        Args:
-            df_sales:      pandas DataFrame
-            start_date:    start date
-            end_date:      end date
-
-        Returns:   filtered pandas DataFrame
-
-        """
-        df_sales = df_sales[df_sales[date_col] >= start_date]
-        return df_sales
-
-    @classmethod
-    def process_date_column(cls, df_sales: pd.DataFrame, date_col: str) -> pd.DataFrame:
-        """
-        Process date column
-        Args:
-            df_sales: pandas DataFrame
-            date_col: name of date column
-        Returns: pandas DataFrame
-        """
-        df_sales[date_col] = pd.to_datetime(df_sales[date_col])
-        df_sales['year'] = df_sales[date_col].dt.year
-        df_sales['month'] = df_sales[date_col].dt.month
-        df_sales['day'] = df_sales[date_col].dt.day
-        df_sales['day_of_week'] = df_sales[date_col].dt.dayofweek
-        df_sales['week_of_year'] = df_sales[date_col].apply(lambda x: x.isocalendar()[1])
-        df_sales['quarter'] = df_sales[date_col].dt.quarter
-        df_sales['is_weekend'] = df_sales[date_col].dt.dayofweek.isin([5, 6]).astype(int)
-        return df_sales
-
-    @classmethod
-    def calculate_duration(cls, df_event: pd.DataFrame, max_date: str, min_date: str) -> pd.DataFrame:
-        """
-        Calculate the duration between two dates in a DataFrame of events.
-        Args:
-            df_event: A pandas DataFrame containing the event dates.
-            max_date (str): The name of the column containing the latest date.
-            min_date (str): The name of the column containing the earliest date.
-
-        Returns:
-            A pandas DataFrame with a new 'duration' column containing the duration between the two dates.
-        """
-        df_event = df_event[(df_event['event_id'] != -1)]
-        df_event[max_date], df_event[min_date] = pd.to_datetime(df_event[max_date]), pd.to_datetime(df_event[min_date])
-        df_event['duration'] = df_event[max_date] - df_event[min_date]
-        return df_event
-
-    @classmethod
-    def identify_event(cls, df_event: pd.DataFrame, df_sales: pd.DataFrame, date_col: str, min_date: str,
-                       max_date: str) -> pd.DataFrame:
-        """
-        Identify event dates in sales data and create an is_event column in sales DataFrame.
-
-        Args:
-        df_event (pd.DataFrame): DataFrame containing the event dates.
-        df_sales (pd.DataFrame): DataFrame containing the sales data.
-        date_col (str): Column name for date in df_sales.
-        min_date (str): Column name for start event date in df_event.
-        end_event_date (str): Column name for end event date in df_event.
-
-        Returns:
-        A pandas DataFrame containing the sales data with an is_event column added.
-        """
-        df_sales['is_event'] = 0
-        for index, event in df_event.iterrows():
-            mask = df_sales[date_col].isin(pd.date_range(start=event[min_date], end=event[max_date]))
-            df_sales.loc[mask, 'is_event'] = 1
-        return df_sales
-
-    @staticmethod
-    def get_event_id_list(df_temp: pd.DataFrame, row: pd.Series, col: str, date_col: str) -> List[str]:
-        """
-        Get list of event ids for a given date and event type.
-        Args:
-            df_temp:
-            row:
-            col:
-
-        Returns:
-
-        """
-        df_event_row = df_temp[df_temp[date_col] == row[date_col]][f"{col}_list"].tolist()
-        return df_event_row
-
-    @classmethod
-    def map_event_to_list(cls, df_sales: pd.DataFrame, df_event: pd.DataFrame, max_date: str, min_date: str,
-                          column_list_map_id: List[str], date_col: str) -> pd.DataFrame:
-        """
-        Map event to list of event ids for a given date and event type.
-        Args:
-            df_sales:   DataFrame containing the sales data.
-            df_event:   DataFrame containing the event dates.
-            max_date:   Column name for end event date in df_event.
-            min_date:   Column name for start event date in df_event.
-            column_list_map_id: List of columns to map to list.
-
-        Returns:
-
-        """
-        for col in column_list_map_id:
-            temp_list = []
-            for index, event in df_event.iterrows():
-                dates = pd.date_range(start=event[min_date], end=event[max_date])
-                for date in dates:
-                    temp_list.append({date_col: date, f"{col}_list": event[col]})
-            df_temp = pd.DataFrame(temp_list)
-            df_sales[f"{col}_list"] = df_sales.apply(
-                lambda row: EventFeatureGenerator.get_event_id_list(df_temp, row, col, date_col), axis=1)
-            del temp_list
-        return df_sales
-
-    @classmethod
-    def add_stat_duartions(cls, df_sales: pd.DataFrame, duration_list_col: str) -> pd.DataFrame:
-        """
-        Adds statistical measures of the durations of events in a column of a pandas DataFrame.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the event column.
-            duration_list_col (str): The name of the column representing the events -> "duration_list"
-
-        Returns:
-            pd.DataFrame: DataFrame with three new columns:
-                - '{event_col}_mean_event': the mean duration of events in the event column, for each row in the DataFrame.
-                - '{event_col}_median_event': the median duration of events in the event column, for each row in the DataFrame.
-                - '{event_col}_std_event': the standard deviation of the duration of events in the event column, for each row in the DataFrame.
-        """
-        df_sales[f"{duration_list_col}_mean_event"] = df_sales.apply(lambda x: np.mean(x[duration_list_col]), axis=1)
-        df_sales[f"{duration_list_col}_mean_event"] = df_sales[f"{duration_list_col}_mean_event"].dt.days
-        df_sales[f"{duration_list_col}_median_event"] = df_sales.apply(lambda x: np.median(x[duration_list_col]),
-                                                                       axis=1)
-        df_sales[f"{duration_list_col}_median_event"] = df_sales[f"{duration_list_col}_median_event"].dt.days
-        df_sales[f"{duration_list_col}_std_event"] = df_sales.apply(
-            lambda x: np.std([d.total_seconds() for d in x[duration_list_col]]), axis=1)
-        return df_sales
-
-    @classmethod
-    def length_list_event(cls, df_sales: pd.DataFrame, event_col_list: List[str]) -> pd.DataFrame:
-        """
-        Calculates the length of each list in a column of a pandas DataFrame, for a specified list of columns.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the event columns.
-            event_col_list (List[str]): The list of names of columns representing the events -> ["event_id_list","sub_event_id_list"]
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'num_{col}' for each column in event_col_list.
-            These columns represent the length of each list in the corresponding event column, for each row in the DataFrame.
-        """
-        for col in event_col_list:
-            df_sales[f"num_{col}"] = df_sales.apply(lambda x: len(x[col]), axis=1)
-        return df_sales
-
-    @classmethod
-    def diff_col(cls, df_sales: pd.DataFrame, target_col: str, date_col: str) -> pd.DataFrame:
-        """
-        Calculates the rate of change in a column of a pandas DataFrame over time, based on a date column.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the target and date columns.
-            target_col (str): The name of the column representing the target variable.
-            date_col (str): The name of the column representing the dates.
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called '{target_col}_diff'.
-            This column represents the rate of change in the target column over time, based on the day-to-day difference
-            in the target variable and the number of days between each row in the date column.
-            :param df_sales:
-        """
-        diff = df_sales[target_col].astype(np.int64).diff().dropna()
-        days_diff = pd.to_datetime(df_sales[date_col]).dt.day.diff().dropna()
-        rate_of_change = diff / days_diff
-        df_sales[f"{target_col}_diff"] = rate_of_change.shift()
-        df_sales[f"{target_col}_diff"] = df_sales[f"{target_col}_diff"].replace([np.inf, -np.inf], 0)
-        return df_sales
-
-    @classmethod
-    def event_frequency(cls, df_sales: pd.DataFrame, date_col: str, event_num: str) -> pd.DataFrame:
-        """
-        Calculates the frequency of events in a pandas DataFrame, based on a specified date column and event count column.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the date and event count columns.
-            date_col (str): The name of the column representing the dates.
-            event_num (str): The name of the column representing the event counts ->'num_event_id_list'
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'event_frequency'.
-            This column represents the average number of events per week, based on the event count and number of weeks in the date column.
-        """
-
-        df_sales['event_frequency'] = (
-                df_sales[event_num] / df_sales[date_col].dt.isocalendar().week.nunique()).shift(1).fillna(0)
-        return df_sales
-
-    @classmethod
-    def indicate_event_combination_change(cls, df_sales: pd.DataFrame, event_col_even: str) -> pd.DataFrame:
-        """
-        Indicates whether the combination of events has changed from the previous row in a pandas DataFrame.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the event column.
-            event_col_even (str): The name of the column representing the events.
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'ind_change_combo_event'.
-            This column represents whether the combination of events in the current row is different from the previous row (1),
-            or not (0).
-        """
-        df_sales["ind_change_combo_event"] = np.where(df_sales[event_col_even].shift() != df_sales[event_col_even], 1,
-                                                      0)
-        df_sales.loc[0, "ind_change_combo_event"] = 0
-        return df_sales
-
-    # def std_on_list(self, df_sales: pd.DataFrame, event_col_discount_type: str) -> pd.DataFrame:
-    #     """
-    #     Calculates the standard deviation of a list of values in a column of a pandas DataFrame.
-    #
-    #     Args:
-    #         df (pd.DataFrame): The pandas DataFrame containing the column of lists.
-    #         event_col_discount_type (str): The name of the column containing the lists -> "discount_type_list"
-    #
-    #     Returns:
-    #         pd.DataFrame: DataFrame with a new column called '{event_col}_std'.
-    #         This column represents the standard deviation of the values in the list in the specified event column,
-    #         for each row in the DataFrame.
-    #         [0.0,1.0,1.0]
-    #     """
-    #
-    #     df_sales[event_col_discount_type] = df_sales[event_col_discount_type].apply(lambda x: [int(i) for i in x] if isinstance(x, (list, tuple)) else x)
-    #     df_sales[f"{event_col_discount_type}_std"] = df_sales.apply(
-    #         lambda x: np.std([d for d in x[event_col_discount_type]]) if isinstance(x[event_col_discount_type],
-    #                                                                                 (list, tuple)) else np.nan,
-    #         axis=1)
-    #     return df_sales
-
-    @classmethod
-    def log_col(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
-        """
-        Applies the natural logarithm to a specified column in a pandas DataFrame.
-        but skips the operation for any zero values.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the target column.
-            target_col (str): The name of the column to apply the logarithm to.
-
-        Returns:
-            pd.DataFrame:DataFrame with a new column called '{target_col}_log'.
-            This column represents the natural logarithm of the specified target column,
-            except for any zero values which are left unchanged.
-        """
-        df_sales[f"{target_col}_log"] = np.where(df_sales[target_col] == 0, 0, np.log(df_sales[target_col]))
-        df_sales[f"{target_col}_log"] = df_sales[f"{target_col}_log"].shift(1).fillna(0)
-        return df_sales
-
-    @classmethod
-    def caculate_amount_days_pass_from_start_of_event(cls, df_sales: pd.DataFrame, date_col: str,
-                                                      date_min_col_list: str) -> pd.DataFrame:
-        """
-        Calculates the number of days that have passed since the start of an event in a pandas DataFrame.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the event and date columns.
-            date_min_col_list (str): The name of the column representing the start of the event     -> "date_min_list"
-            date_col (str): The name of the column representing the dates.
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'amount_of_days_pass_from_start_of_event'.
-            This column represents the number of days that have passed since the start of the event, for each row in the DataFrame.
-        """
-        df_sales["amount_of_days_pass_from_start_of_event"] = df_sales.apply(
-            lambda x: np.abs(pd.to_datetime(x[date_col]) - pd.to_datetime(x[date_min_col_list])), axis=1)
-        return df_sales
-
-    @classmethod
-    def caculate_amount_days_pass_from_start_of_event_most_new(cls, df_sales: pd.DataFrame, event_col: str,
-                                                               date_col: str) -> pd.DataFrame:
-        """
-        Calculates the number of days that have passed since the start of an event, for the most recent event in a pandas DataFrame.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the event and date columns.
-            event_col (str): The name of the column representing the events -> "min_date_list"
-            date_col (str): The name of the column representing the dates.
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'amount_of_days_pass_from_start_of_event_most_new'.
-            This column represents the number of days that have passed since the start of the most recent event, for each row in the DataFrame.
-        """
-        df_sales["amount_of_days_pass_from_start_of_event_most_new"] = df_sales.apply(
-            lambda x: np.min(pd.to_datetime(x[date_col]) - pd.to_datetime(x[event_col])), axis=1)
-        df_sales["amount_of_days_pass_from_start_of_event_most_new"] = pd.to_timedelta(
-            df_sales["amount_of_days_pass_from_start_of_event_most_new"]).dt.days
-        return df_sales
-
-    @classmethod
-    def merge_df(cls, df_sales: pd.DataFrame, df_holiday: pd.DataFrame, key: str) -> pd.DataFrame:
-        """
-        Merges two pandas DataFrames based on a common key.
-        1: df1 = df_sales
-        2: df2 = df_holidays
-        key: 'date'
-
-        Args:
-            df1 (pd.DataFrame): The first pandas DataFrame to merge.
-            df2 (pd.DataFrame): The second pandas DataFrame to merge.
-            key (str): The name of the key column to merge on.
-
-        Returns:
-            df_merge    pd.DataFrame: A new DataFrame that contains all columns from both input DataFrames, merged
-            on the specified key. The merge type is left join (i.e., all rows from df1 are retained, and
-            matching rows from df2 are included where available).
-        """
-        df_sales[key] = pd.to_datetime(df_sales[key])
-        df_holiday[key] = pd.to_datetime(df_holiday[key], format="%d/%m/%Y")
-        df_sales = df_sales.merge(df_holiday, on=key, how="left")
-        return df_sales
-
-    @classmethod
-    def identify_date_occasion(cls, df_sales: pd.DataFrame, holiday_col: str, date_col: str) -> pd.DataFrame:
-        """
-        Identifies holidays in a pandas DataFrame based on a specified column.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the holiday column.
-            holiday_col (str): The name of the column representing the holidays -> "holiday_name"
-            date_col (str): The name of the column representing the dates -> "date"
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'is_holiday'. This column
-            represents whether each row is a holiday (1) or not (0), based on whether the holiday column
-            is null or not.
-        """
-        df_sales["is_holday"] = np.where(df_sales[holiday_col].isnull(), 0, 1)
-        df_sales["is_sunday"] = np.where(df_sales[date_col].dt.day_name() == "Sunday", 1, 0)
-        return df_sales
-
-    @classmethod
-    def feature_combine_str(cls, df_sales: pd.DataFrame, holiday_col_type: str, holiday_col: str) -> pd.DataFrame:
-        """
-        Combines the values of two columns in a pandas DataFrame into a new column as a string.
-        col1='type',col2='holiday_name' -> 'type_holiday_name'
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the two columns to combine.
-            holiday_col_type (str): The name of the first column to combine -> "holiday_type"
-            holiday_col (str): The name of the second column to combine -> "holiday_name"
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called '{col1}_{col2}'. This column
-            represents the concatenation of the values of col1 and col2 as strings, separated by an underscore.
-        """
-        df_sales[f"{holiday_col_type}_{holiday_col}"] = df_sales[holiday_col_type].map(str) + "_" + df_sales[
-            holiday_col].map(str)
-        return df_sales
-
-    @classmethod
-    def calculate_rolling_functions(cls, df_sales: pd.DataFrame, target_col: str, window_size_list: List[int],
-                                    type_functions: List[str]) -> pd.DataFrame:
-        """
-        Calculates the moving average trend for a specified column in a pandas DataFrame.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the target column.
-            target_col (str): The name of the column for which to calculate the trend.
-            window_size_list (int): list size of the rolling window to use when calculating the trend.
-            type_functions (List[str]): The type of trend to calculate. This can be any function
-                from the numpy library that can be applied to a rolling window.
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'trend'. This column represents
-            the moving average trend of the specified target column over the rolling window.
-        """
-        for type_function in type_functions:
-            for window_size in window_size_list:
-                df_sales[f'rolling_{window_size}_{type_functions}'] = df_sales[target_col].rolling(
-                    window=window_size).apply(
-                    getattr(np, type_function)).shift(1).fillna(0)
-        return df_sales
-
-    @classmethod
-    def add_cumulative_sum_column_for_targe(cls, df_sales: pd.DataFrame, col: str) -> pd.DataFrame:
-        """
-        Adds a cumulative sum column to a pandas DataFrame.
-        Args:
-            df (pd.DataFrame): The pandas DataFrame to add the cumulative sum column to.
-            col (str): The name of the column to calculate the cumulative sum for.
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'cumulative_sum'. This column
-            represents the cumulative sum of the specified column.
-        """
-        df_sales[f'cumulative_sum_{col}'] = df_sales[col].cumsum()
-        df_sales[f'cumulative_sum_{col}'] = df_sales[f'cumulative_sum_{col}'].shift(1).fillna(0)
-        return df_sales
-
-    @classmethod
-    def fft_features(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
-        """
-        Extracts spectral analysis features using Fast Fourier Transform (FFT).
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the target column.
-            target_col (str): The name of the column representing the target variable.
-
-        Returns:
-            pd.DataFrame: DataFrame with two new columns: 'fft_real' and 'fft_imag'.
-            These columns represent the real and imaginary parts of the FFT output, respectively.
-        """
-        df_temp = fft(df_sales[target_col].shift(1).fillna(0).values)
-        df_sales['fft_real'] = np.real(df_temp)
-        df_sales['fft_imag'] = np.imag(df_temp)
-        return df_sales
-
-    @classmethod
-    def extract_trend_change(cls, df_sales: pd.DataFrame, trend_col: str) -> pd.DataFrame:
-        """
-        Extracts trend changes in a pandas DataFrame based on peaks in a specified trend column.
-
-        Args:
-            df (pd.DataFrame): The pandas DataFrame containing the trend column.
-            trend_col (str): The name of the column representing the trend -> 'rolling_7_mean'
-
-        Returns:
-            pd.DataFrame: DataFrame with a new column called 'trend_change' indicating
-            trend changes. If the value in the trend column is a local maximum (peak), the value in the
-            'trend_change' column will be set to 1. Otherwise, it will be set to 0.
-        """
-        peaks_extract = argrelextrema(np.array(df_sales[trend_col].shift(1).fillna(0).values), np.greater)
-        df_sales['trend_change'] = 0
-        df_sales.loc[peaks_extract[0], 'trend_change'] = 1
-        return df_sales
-
-    @classmethod
-    def time_series_shape_features(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
-        """
-        Calculates shape-based features of a time series and adds them as columns to the input dataframe.
-
-        Args:
-            df (pd.DataFrame): The input time series data as a pandas dataframe.
-            target_col (str): The name of the column in the input dataframe that contains the target variable.
-
-        Returns:
-            pd.DataFrame: A pandas dataframe with the same columns as the input dataframe, but with additional columns for the calculated shape-based features.
-        """
-        df_sales['skewness'] = df_sales[target_col].shift(1).fillna(0).skew()
-        df_sales['kurtosis'] = df_sales[target_col].shift(1).fillna(0).kurt()
-        df_sales['slope'] = np.polyfit(df_sales.index, df_sales[target_col].shift(1).fillna(0).values, 1)[0]
-        return df_sales
-
-    @classmethod
-    def add_lagged_feature_to_time_series_of_column(cls, df_sales: pd.DataFrame, cols: list[str],
-                                                    lags_list: List[int]) -> pd.DataFrame:
-        """
-        Add a lagged feature to a time series dataframe.
-
-        Args:
-            df: The dataframe to add the lagged feature to.
-                assumed to be in time series format
-            col: The column to add the lagged feature to.
-            lag: The lag to add to the dataframe.
-
-        Returns:
-            The dataframe with the lagged feature added.
-
-
-        """
-
-        for col in cols:
-            for lag in lags_list:
-                df_sales[f'{col}_lag_{lag}'] = df_sales[col].shift(lag)
-        return df_sales
-
-    @classmethod
-    def convert_str_indicator(cls, df_sales: pd.DataFrame, weekend_col: list[str]) -> pd.DataFrame:
-        """
-        Converts boolean columns in a pandas DataFrame to binary integer columns (0 or 1).
-        Args:
-            df: The input DataFrame.
-            weekend_cols: A list of column names to be converted.
-
-        Returns:
-            The input DataFrame with the specified columns converted to binary integer format.
-        """
-
-        df_sales[weekend_col] = np.where(df_sales[weekend_col] is True, 1, 0)
-        return df_sales
-
-    @classmethod
-    def extract_features_pca(cls, df_sales: pd.DataFrame, date_col: str,
-                             pca_num: int, year_forecast: int = None) -> pd.DataFrame:
-        """
-        Perform Principal Component Analysis (PCA) on a subset of numerical columns in a DataFrame, and append the resulting
-        principal components to the original DataFrame.
-
-        Args:
-            df (pd.DataFrame): The input DataFrame.
-            year_forecast (int): The year after which to exclude data from PCA analysis.
-            pca_num (int): The number of principal components to retain.
-
-        Returns:
-            pd.DataFrame: The input DataFrame with additional columns corresponding to the retained principal components.
-        """
-
-        ##### NOT FOR INFERENCE
-        if year_forecast is None:
-            df_pca = df_sales
-        else:
-            df_pca = df_sales[df_sales[date_col].dt.year < year_forecast].copy()
-
-        df_numeric = df_pca.select_dtypes(include=[np.number])
-        df_numeric = df_numeric.drop(columns=df_numeric.select_dtypes(include='timedelta64').columns.tolist())
-        df_numeric_imputed = df_numeric.fillna(0)
-        pca = PCA(n_components=pca_num)
-        pca.fit(df_numeric_imputed)
-        df_setup_process = df_sales.copy()
-        pca_components = pca.transform(df_setup_process[df_numeric_imputed.columns].fillna(0))
-        columns_pca = [f"PC{i}" for i in range(1, pca_num + 1)]
-        pca_df = pd.DataFrame(pca_components, columns=columns_pca)
-        df_sales[columns_pca] = pca_df
-        return df_sales
-
-    @classmethod
-    def apply_encodings(cls, df_sales: pd.DataFrame, type_encoder_list: List[str], cols_to_encode: List[str],
-                        target_col: str,
-                        year_forecast: int, sigma=1, random_state=12) -> pd.DataFrame:
-        """
-        Applies a set of target encoders to specified columns in a pandas DataFrame.
-
-        Args:
-            target_col:
-            df (pd.DataFrame): The input DataFrame.
-            type_encoder_list (List[str]): A list of target encoders to apply to the specified columns. The encoder names should be strings and correspond to the name of the encoder class from the category_encoders package.
-            ->["GLMMEncoder","MEstimateEncoder","CatBoostEncoder"]
-            cols_to_encode (List[str]): A list of column names to encode.
-            target (str): The name of the target column.
-            year_forecast (int): The year until which to include data.
-            sigma (float): The noise level added to the encoding.
-            random_state (int): The random seed used for the encoding.
-
-        Returns:
-            pd.DataFrame: The encoded DataFrame.
-        """
-        ##### NOT FOR INFERENCE
-        encoder_class_dict = {
-            # "GLMMEncoder": GLMMEncoder,
-            "MEstimateEncoder": MEstimateEncoder,
-            "CatBoostEncoder": CatBoostEncoder
-        }
-        if year_forecast is None:
-            df_filtered = df_sales
-        else:
-            df_filtered = df_sales[df_sales.date.dt.year < year_forecast].copy()
-
-        for encoder_type in type_encoder_list:
-            encoder_class = encoder_class_dict[encoder_type]
-            for col in cols_to_encode:
-                encoder = encoder_class(cols=[col], sigma=sigma, random_state=random_state)
-                if encoder_type == "CatBoostEncoder":
-                    encoder.fit(df_filtered[col].astype(str), df_filtered[target_col])
-                    df_sales[f'{encoder_type}_of_{col}'] = encoder.transform(df_sales[col], df_sales[target_col])
-                else:
-                    encoder.fit(df_filtered[col], df_filtered[target_col])
-                    df_sales[f'{encoder_type}_of_{col}'] = encoder.transform(df_sales[col], df_sales[target_col])
-        return df_sales
-
-    @classmethod
-    def apply_encodings_at_once(cls, df_sales: pd.DataFrame, type_encoder_list: List[str], cols_to_encode: List[str],
-                                target_col: str,
-                                year_forecast: int, sigma=1, random_state: int = 12) -> pd.DataFrame:
-        """
-        Apply multiple category encoders to the same set of columns at once.
-
-        Args:
-            df (pd.DataFrame): The input dataframe to be encoded.
-            type_encoder_list (List[str]): A list of category encoder types to be applied ->["GLMMEncoder","MEstimateEncoder","CatBoostEncoder"]
-            cols (List[str]): A list of column names to be encoded.
-            target (str): The name of the target column to encode against.
-            year_forecast (int): The year forecast limit to use for training data.
-            sigma (float): The regularization parameter for encoders that support it. Default is 1.
-            random_state (int): The random seed to use. Default is 12.
-
-        Returns:
-            pd.DataFrame: A new dataframe with the encoded columns added.
-        """
-        ##### NOT FOR INFERENCE
-        encoder_class_dict = {
-            # "GLMMEncoder": GLMMEncoder,
-            "MEstimateEncoder": MEstimateEncoder,
-            "CatBoostEncoder": CatBoostEncoder
-        }
-        if year_forecast is None:
-            df_filtered = df_sales
-        else:
-            df_filtered = df_sales[df_sales.date.dt.year < year_forecast].copy()
-
-        for encoder_type in type_encoder_list:
-            encoder_class = encoder_class_dict[encoder_type]
-            encoder = encoder_class(cols=cols_to_encode, sigma=sigma, random_state=random_state)
-            if encoder_type == "CatBoostEncoder":
-                encoder.fit(df_filtered[cols_to_encode].astype(str), df_filtered[target_col])
-                encoded_df = encoder.transform(df_sales[cols_to_encode], df_sales[target_col])
-                for col in encoded_df.columns:
-                    df_sales[f'{encoder_type}_of_all_{col}'] = encoded_df[col]
-            else:
-                encoder.fit(df_filtered[cols_to_encode], df_filtered[target_col])
-                encoded_df = encoder.transform(df_sales[cols_to_encode], df_sales[target_col])
-                for col in encoded_df.columns:
-                    df_sales[f'{encoder_type}_of_all_{col}'] = encoded_df[col]
-        return df_sales
-
-    @classmethod
-    def columns_interactions_encoder(cls, df_sales: pd.DataFrame, cols_to_encode_at_once: List[str],
-                                     cols_days_for_interaction: List[str], target_col: str,
-                                     type_encoder_list: List[str], year_forecast: int) -> pd.DataFrame:
-        """
-        Apply feature interaction encoding on specified columns and then encode the new columns using a list of categorical encoders.
-
-        Args:
-            df_sales (pd.DataFrame): The input dataframe to be encoded.
-            cols_to_encode_at_once (List[str]): A list of columns to be encoded at once.
-            cols_days_for_interaction (List[str]): A list of columns to be used for feature interaction.
-            target_col (str): The name of the target column to encode against.
-            type_encoder_list (List[str]): A list of category encoder types to be applied ->["GLMMEncoder","MEstimateEncoder","CatBoostEncoder"]
-            year_forecast (int): The year forecast limit to use for training data.
-
-
-        Returns:
-            pd.DataFrame: A new DataFrame with feature interaction columns and encoded columns using specified categorical encoders.
-
-        """
-        interactions_columns = []
-        for col1 in cols_to_encode_at_once:
-            for col2 in cols_days_for_interaction:
-                df_sales[f"{col1}_interactions_{col2}"] = df_sales[f"{col1}"] * df_sales[f"{col2}"]
-                interactions_columns.append(f"{col1}_interactions_{col2}")
-
-        df_sales = cls.apply_encodings_at_once(df_sales=df_sales, type_encoder_list=type_encoder_list,
-                                               cols_to_encode=interactions_columns,
-                                               target_col=target_col, year_forecast=year_forecast)
-        return df_sales
-
-    @classmethod
-    def remove_expand_dates(cls, df_sales: pd.DataFrame):
-        columns_to_check = ['year', 'month', 'day', 'day_of_week', 'week_of_year', 'quarter', 'is_weekend']
-        if all(column in df_sales.columns for column in columns_to_check):
-            df_sales = df_sales.drop(columns=columns_to_check)
-            print("All specified columns have been dropped.")
-        else:
-            print("Not all specified columns are present in the DataFrame.")
-        return df_sales
-
-    @classmethod
-    def filter_columns_by_correlation(cls, df_sales: pd.DataFrame, year_forecast: int, target_col: str,
-                                      date_col: str) -> List[
-        str]:
-        """
-        Filters the columns in the input dataframe based on their correlation with the target column.
-        Args:
-            df (pd.DataFrame): The input dataframe to be filtered.
-            year_forecast (int): The year forecast limit to use for training data.
-            target_col (str): The name of the target column to be used for correlation analysis.
-            date_col (str): The name of the date column to be used for filtering based on the year forecast.
-
-        Returns:
-            List[str]: A list of column names that are highly correlated with the target column.
-        """
-
-        if year_forecast is None:
-            corr = df_sales.corr()
-        else:
-            corr = df_sales[df_sales[date_col].dt.year < year_forecast].corr()
-
-        corr_target = abs(corr[target_col])
-        relevant_features = corr_target[(corr_target > 0.4) & (corr_target < 1)]
-        selected_col_by_corr = relevant_features.index.tolist()
-        return selected_col_by_corr
-
-    @classmethod
-    def add_back_feature(cls, df_sales: pd.DataFrame, list_col_add: List[str],
-                         selected_col_by_corr: List[str]) -> pd.DataFrame:
-        """
-        Add a list of columns back to the dataframe.
-
-        Args:
-            df_sales:
-            df (pd.DataFrame): The input dataframe.
-            list_col_add (List[str]): A list of column names to add to the dataframe -> ["date",'target']
-            selected_col_by_corr (List[str]): A list of column names to add to the dataframe selected by correlation.
-
-        Returns:
-            pd.DataFrame: A new dataframe with the added columns.
-        """
-        union_list = list_col_add + selected_col_by_corr
-        df_union = df_sales[union_list]
-        return df_union
-
-    @classmethod
-    def process_next_days_events(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
-        df_sales['is_tomorrow_event'] = df_sales['is_event'].shift(-1)
-        df_sales['is_2_days_event'] = df_sales['is_event'].shift(-2)
-
-        # this is only in inferring
-        df_sales[target_col] = df_sales[target_col].shift(-1) + df_sales[target_col].shift(-2)
-        y_prcoess = df_sales["is_2_days_event"].dropna()
-        df_sales_next = df_sales.loc[y_prcoess.index]
-        return df_sales_next
-
-
-def create_interactions_columns(processed_event_features_df):
-    cols_to_encode_at_once = config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode_at_once']
-    cols_days_for_interaction = config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_days_for_ineraction']
-    for col1 in cols_to_encode_at_once:
-        for col2 in cols_days_for_interaction:
-            processed_event_features_df[f"{col1}_interactions_{col2}"] = processed_event_features_df[f"{col1}"] * \
-                                                                         processed_event_features_df[f"{col2}"]
-
-    return processed_event_features_df
+from typing import List
+import pandas as pd
+import numpy as np
+from scipy.fftpack import fft
+from scipy.signal import argrelextrema
+from sklearn.decomposition import PCA
+from category_encoders import GLMMEncoder, MEstimateEncoder, CatBoostEncoder
+from . import config
+
+
+# TODO: speak to yotam
+def run_pipline_event(data_event, data_sales, data_hol, date_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['date_col'],
+                      start_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['start_date'],
+                      target_col=config.DEFAULT_EVENT_HANDLER_VARIABLES['target_col'],
+                      max_date=config.DEFAULT_EVENT_HANDLER_VARIABLES['max_date'],
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
+                      cols_to_encode_at_once=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode_at_once'],
+                      cols_days_for_interaction=config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_days_for_ineraction'],
+                      list_col_add=config.DEFAULT_EVENT_HANDLER_VARIABLES['list_col_add']):
+    event_preprocess = EventFeatureGenerator()
+    # event_preprocess.change_columns_names_in_dataframe_by_dict(data_sales, column_dict)
+    data_sales0 = event_preprocess.filter_data_by_date(data_sales, date_col, start_date)
+    data_sales_process = event_preprocess.aggregate_data(data_sales0, target_col)
+    data_sales_process1 = event_preprocess.process_date_column(data_sales_process, date_col)
+    data_event_process = event_preprocess.calculate_duration(data_event, max_date, min_date)
+    data_sales_process2 = event_preprocess.identify_event(data_event_process, data_sales_process1, date_col, min_date,
+                                                          max_date)
+    data_sales_process3 = event_preprocess.map_event_to_list(data_sales_process2, data_event_process, max_date,
+                                                             min_date, column_list_map_id, date_col)
+    data_sales_process4 = event_preprocess.add_stat_duartions(data_sales_process3, duration_list_col)
+    data_sales_process5 = event_preprocess.length_list_event(data_sales_process4, event_col_list)
+    data_sales_process6 = event_preprocess.diff_col(data_sales_process5, target_col, date_col)
+    data_sales_process7 = event_preprocess.event_frequency(data_sales_process6, date_col, event_num)
+    data_sales_process8 = event_preprocess.indicate_event_combination_change(data_sales_process7, event_col_even)
+    # data_sales_process9 = event_preprocess.std_on_list(data_sales_process8, event_col_discount_type)
+    data_sales_process10 = event_preprocess.log_col(data_sales_process8, target_col)
+    data_sales_process11 = event_preprocess.caculate_amount_days_pass_from_start_of_event(data_sales_process10,
+                                                                                          date_col, date_min_col_list)
+    data_sales_process12 = event_preprocess.caculate_amount_days_pass_from_start_of_event_most_new(data_sales_process11,
+                                                                                                   date_min_col_list,
+                                                                                                   date_col)
+    data_sales_process13 = event_preprocess.merge_df(data_sales_process12, data_hol, date_col)
+    data_sales_process14 = event_preprocess.identify_date_occasion(data_sales_process13, holiday_col, date_col)
+    data_sales_process15 = event_preprocess.feature_combine_str(data_sales_process14, holiday_col_type, holiday_col)
+    data_sales_process16 = event_preprocess.add_cumulative_sum_column_for_targe(data_sales_process15, target_col)
+    data_sales_process17 = event_preprocess.fft_features(data_sales_process16, target_col)
+    data_sales_process18 = event_preprocess.time_series_shape_features(data_sales_process17, target_col)
+    data_sales_process21 = event_preprocess.convert_str_indicator(data_sales_process18, weekend_col)
+
+    # data_sales_process22 = event_preprocess.extract_features_pca(data_sales_process21, date_col, year_forecast, pca_num,
+    #                                                              target_col, task=task)
+    #
+    data_sales_process23 = event_preprocess.process_next_days_events(data_sales_process21, target_col)
+
+    return data_sales_process23
+
+
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
+    data_sales_process27 = event_preprocess.remove_expand_dates(df)
+    data_final_event = data_sales_process27.copy()
+    return data_final_event
+
+
+class EventFeatureGenerator:
+    @classmethod
+    def aggregate_data(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """
+        Aggregate data by date
+        Args:
+            target_col:     name of target column
+            df_sales:      pandas DataFrame
+
+        Returns:   aggregate by target_col pandas DataFrame
+
+        """
+        df_sales[target_col] = df_sales[target_col].astype(np.float64)
+        return df_sales.groupby(['date'])[target_col].sum(numeric_only=True).reset_index()
+
+    @classmethod
+    def filter_data_by_date(cls, df_sales: pd.DataFrame, date_col: str, start_date: str) -> pd.DataFrame:
+        """
+        Filter data by date
+        Args:
+            df_sales:      pandas DataFrame
+            start_date:    start date
+            end_date:      end date
+
+        Returns:   filtered pandas DataFrame
+
+        """
+        df_sales = df_sales[df_sales[date_col] >= start_date]
+        return df_sales
+
+    @classmethod
+    def process_date_column(cls, df_sales: pd.DataFrame, date_col: str) -> pd.DataFrame:
+        """
+        Process date column
+        Args:
+            df_sales: pandas DataFrame
+            date_col: name of date column
+        Returns: pandas DataFrame
+        """
+        df_sales[date_col] = pd.to_datetime(df_sales[date_col])
+        df_sales['year'] = df_sales[date_col].dt.year
+        df_sales['month'] = df_sales[date_col].dt.month
+        df_sales['day'] = df_sales[date_col].dt.day
+        df_sales['day_of_week'] = df_sales[date_col].dt.dayofweek
+        df_sales['week_of_year'] = df_sales[date_col].apply(lambda x: x.isocalendar()[1])
+        df_sales['quarter'] = df_sales[date_col].dt.quarter
+        df_sales['is_weekend'] = df_sales[date_col].dt.dayofweek.isin([5, 6]).astype(int)
+        return df_sales
+
+    @classmethod
+    def calculate_duration(cls, df_event: pd.DataFrame, max_date: str, min_date: str) -> pd.DataFrame:
+        """
+        Calculate the duration between two dates in a DataFrame of events.
+        Args:
+            df_event: A pandas DataFrame containing the event dates.
+            max_date (str): The name of the column containing the latest date.
+            min_date (str): The name of the column containing the earliest date.
+
+        Returns:
+            A pandas DataFrame with a new 'duration' column containing the duration between the two dates.
+        """
+        df_event = df_event[(df_event['event_id'] != -1)]
+        df_event[max_date], df_event[min_date] = pd.to_datetime(df_event[max_date]), pd.to_datetime(df_event[min_date])
+        df_event['duration'] = df_event[max_date] - df_event[min_date]
+        return df_event
+
+    @classmethod
+    def identify_event(cls, df_event: pd.DataFrame, df_sales: pd.DataFrame, date_col: str, min_date: str,
+                       max_date: str) -> pd.DataFrame:
+        """
+        Identify event dates in sales data and create an is_event column in sales DataFrame.
+
+        Args:
+        df_event (pd.DataFrame): DataFrame containing the event dates.
+        df_sales (pd.DataFrame): DataFrame containing the sales data.
+        date_col (str): Column name for date in df_sales.
+        min_date (str): Column name for start event date in df_event.
+        end_event_date (str): Column name for end event date in df_event.
+
+        Returns:
+        A pandas DataFrame containing the sales data with an is_event column added.
+        """
+        df_sales['is_event'] = 0
+        for index, event in df_event.iterrows():
+            mask = df_sales[date_col].isin(pd.date_range(start=event[min_date], end=event[max_date]))
+            df_sales.loc[mask, 'is_event'] = 1
+        return df_sales
+
+    @staticmethod
+    def get_event_id_list(df_temp: pd.DataFrame, row: pd.Series, col: str, date_col: str) -> List[str]:
+        """
+        Get list of event ids for a given date and event type.
+        Args:
+            df_temp:
+            row:
+            col:
+
+        Returns:
+
+        """
+        df_event_row = df_temp[df_temp[date_col] == row[date_col]][f"{col}_list"].tolist()
+        return df_event_row
+
+    @classmethod
+    def map_event_to_list(cls, df_sales: pd.DataFrame, df_event: pd.DataFrame, max_date: str, min_date: str,
+                          column_list_map_id: List[str], date_col: str) -> pd.DataFrame:
+        """
+        Map event to list of event ids for a given date and event type.
+        Args:
+            df_sales:   DataFrame containing the sales data.
+            df_event:   DataFrame containing the event dates.
+            max_date:   Column name for end event date in df_event.
+            min_date:   Column name for start event date in df_event.
+            column_list_map_id: List of columns to map to list.
+
+        Returns:
+
+        """
+        for col in column_list_map_id:
+            temp_list = []
+            for index, event in df_event.iterrows():
+                dates = pd.date_range(start=event[min_date], end=event[max_date])
+                for date in dates:
+                    temp_list.append({date_col: date, f"{col}_list": event[col]})
+            df_temp = pd.DataFrame(temp_list)
+            df_sales[f"{col}_list"] = df_sales.apply(
+                lambda row: EventFeatureGenerator.get_event_id_list(df_temp, row, col, date_col), axis=1)
+            del temp_list
+        return df_sales
+
+    @classmethod
+    def add_stat_duartions(cls, df_sales: pd.DataFrame, duration_list_col: str) -> pd.DataFrame:
+        """
+        Adds statistical measures of the durations of events in a column of a pandas DataFrame.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the event column.
+            duration_list_col (str): The name of the column representing the events -> "duration_list"
+
+        Returns:
+            pd.DataFrame: DataFrame with three new columns:
+                - '{event_col}_mean_event': the mean duration of events in the event column, for each row in the DataFrame.
+                - '{event_col}_median_event': the median duration of events in the event column, for each row in the DataFrame.
+                - '{event_col}_std_event': the standard deviation of the duration of events in the event column, for each row in the DataFrame.
+        """
+        df_sales[f"{duration_list_col}_mean_event"] = df_sales.apply(lambda x: np.mean(x[duration_list_col]), axis=1)
+        df_sales[f"{duration_list_col}_mean_event"] = df_sales[f"{duration_list_col}_mean_event"].dt.days
+        df_sales[f"{duration_list_col}_median_event"] = df_sales.apply(lambda x: np.median(x[duration_list_col]),
+                                                                       axis=1)
+        df_sales[f"{duration_list_col}_median_event"] = df_sales[f"{duration_list_col}_median_event"].dt.days
+        df_sales[f"{duration_list_col}_std_event"] = df_sales.apply(
+            lambda x: np.std([d.total_seconds() for d in x[duration_list_col]]), axis=1)
+        return df_sales
+
+    @classmethod
+    def length_list_event(cls, df_sales: pd.DataFrame, event_col_list: List[str]) -> pd.DataFrame:
+        """
+        Calculates the length of each list in a column of a pandas DataFrame, for a specified list of columns.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the event columns.
+            event_col_list (List[str]): The list of names of columns representing the events -> ["event_id_list","sub_event_id_list"]
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'num_{col}' for each column in event_col_list.
+            These columns represent the length of each list in the corresponding event column, for each row in the DataFrame.
+        """
+        for col in event_col_list:
+            df_sales[f"num_{col}"] = df_sales.apply(lambda x: len(x[col]), axis=1)
+        return df_sales
+
+    @classmethod
+    def diff_col(cls, df_sales: pd.DataFrame, target_col: str, date_col: str) -> pd.DataFrame:
+        """
+        Calculates the rate of change in a column of a pandas DataFrame over time, based on a date column.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the target and date columns.
+            target_col (str): The name of the column representing the target variable.
+            date_col (str): The name of the column representing the dates.
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called '{target_col}_diff'.
+            This column represents the rate of change in the target column over time, based on the day-to-day difference
+            in the target variable and the number of days between each row in the date column.
+            :param df_sales:
+        """
+        diff = df_sales[target_col].astype(np.int64).diff().dropna()
+        days_diff = pd.to_datetime(df_sales[date_col]).dt.day.diff().dropna()
+        rate_of_change = diff / days_diff
+        df_sales[f"{target_col}_diff"] = rate_of_change.shift()
+        df_sales[f"{target_col}_diff"] = df_sales[f"{target_col}_diff"].replace([np.inf, -np.inf], 0)
+        return df_sales
+
+    @classmethod
+    def event_frequency(cls, df_sales: pd.DataFrame, date_col: str, event_num: str) -> pd.DataFrame:
+        """
+        Calculates the frequency of events in a pandas DataFrame, based on a specified date column and event count column.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the date and event count columns.
+            date_col (str): The name of the column representing the dates.
+            event_num (str): The name of the column representing the event counts ->'num_event_id_list'
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'event_frequency'.
+            This column represents the average number of events per week, based on the event count and number of weeks in the date column.
+        """
+
+        df_sales['event_frequency'] = (
+                df_sales[event_num] / df_sales[date_col].dt.isocalendar().week.nunique()).shift(1).fillna(0)
+        return df_sales
+
+    @classmethod
+    def indicate_event_combination_change(cls, df_sales: pd.DataFrame, event_col_even: str) -> pd.DataFrame:
+        """
+        Indicates whether the combination of events has changed from the previous row in a pandas DataFrame.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the event column.
+            event_col_even (str): The name of the column representing the events.
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'ind_change_combo_event'.
+            This column represents whether the combination of events in the current row is different from the previous row (1),
+            or not (0).
+        """
+        df_sales["ind_change_combo_event"] = np.where(df_sales[event_col_even].shift() != df_sales[event_col_even], 1,
+                                                      0)
+        df_sales.loc[0, "ind_change_combo_event"] = 0
+        return df_sales
+
+    # def std_on_list(self, df_sales: pd.DataFrame, event_col_discount_type: str) -> pd.DataFrame:
+    #     """
+    #     Calculates the standard deviation of a list of values in a column of a pandas DataFrame.
+    #
+    #     Args:
+    #         df (pd.DataFrame): The pandas DataFrame containing the column of lists.
+    #         event_col_discount_type (str): The name of the column containing the lists -> "discount_type_list"
+    #
+    #     Returns:
+    #         pd.DataFrame: DataFrame with a new column called '{event_col}_std'.
+    #         This column represents the standard deviation of the values in the list in the specified event column,
+    #         for each row in the DataFrame.
+    #         [0.0,1.0,1.0]
+    #     """
+    #
+    #     df_sales[event_col_discount_type] = df_sales[event_col_discount_type].apply(lambda x: [int(i) for i in x] if isinstance(x, (list, tuple)) else x)
+    #     df_sales[f"{event_col_discount_type}_std"] = df_sales.apply(
+    #         lambda x: np.std([d for d in x[event_col_discount_type]]) if isinstance(x[event_col_discount_type],
+    #                                                                                 (list, tuple)) else np.nan,
+    #         axis=1)
+    #     return df_sales
+
+    @classmethod
+    def log_col(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """
+        Applies the natural logarithm to a specified column in a pandas DataFrame.
+        but skips the operation for any zero values.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the target column.
+            target_col (str): The name of the column to apply the logarithm to.
+
+        Returns:
+            pd.DataFrame:DataFrame with a new column called '{target_col}_log'.
+            This column represents the natural logarithm of the specified target column,
+            except for any zero values which are left unchanged.
+        """
+        df_sales[f"{target_col}_log"] = np.where(df_sales[target_col] == 0, 0, np.log(df_sales[target_col]))
+        df_sales[f"{target_col}_log"] = df_sales[f"{target_col}_log"].shift(1).fillna(0)
+        return df_sales
+
+    @classmethod
+    def caculate_amount_days_pass_from_start_of_event(cls, df_sales: pd.DataFrame, date_col: str,
+                                                      date_min_col_list: str) -> pd.DataFrame:
+        """
+        Calculates the number of days that have passed since the start of an event in a pandas DataFrame.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the event and date columns.
+            date_min_col_list (str): The name of the column representing the start of the event     -> "date_min_list"
+            date_col (str): The name of the column representing the dates.
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'amount_of_days_pass_from_start_of_event'.
+            This column represents the number of days that have passed since the start of the event, for each row in the DataFrame.
+        """
+        df_sales["amount_of_days_pass_from_start_of_event"] = df_sales.apply(
+            lambda x: np.abs(pd.to_datetime(x[date_col]) - pd.to_datetime(x[date_min_col_list])), axis=1)
+        return df_sales
+
+    @classmethod
+    def caculate_amount_days_pass_from_start_of_event_most_new(cls, df_sales: pd.DataFrame, event_col: str,
+                                                               date_col: str) -> pd.DataFrame:
+        """
+        Calculates the number of days that have passed since the start of an event, for the most recent event in a pandas DataFrame.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the event and date columns.
+            event_col (str): The name of the column representing the events -> "min_date_list"
+            date_col (str): The name of the column representing the dates.
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'amount_of_days_pass_from_start_of_event_most_new'.
+            This column represents the number of days that have passed since the start of the most recent event, for each row in the DataFrame.
+        """
+        df_sales["amount_of_days_pass_from_start_of_event_most_new"] = df_sales.apply(
+            lambda x: np.min(pd.to_datetime(x[date_col]) - pd.to_datetime(x[event_col])), axis=1)
+        df_sales["amount_of_days_pass_from_start_of_event_most_new"] = pd.to_timedelta(
+            df_sales["amount_of_days_pass_from_start_of_event_most_new"]).dt.days
+        return df_sales
+
+    @classmethod
+    def merge_df(cls, df_sales: pd.DataFrame, df_holiday: pd.DataFrame, key: str) -> pd.DataFrame:
+        """
+        Merges two pandas DataFrames based on a common key.
+        1: df1 = df_sales
+        2: df2 = df_holidays
+        key: 'date'
+
+        Args:
+            df1 (pd.DataFrame): The first pandas DataFrame to merge.
+            df2 (pd.DataFrame): The second pandas DataFrame to merge.
+            key (str): The name of the key column to merge on.
+
+        Returns:
+            df_merge    pd.DataFrame: A new DataFrame that contains all columns from both input DataFrames, merged
+            on the specified key. The merge type is left join (i.e., all rows from df1 are retained, and
+            matching rows from df2 are included where available).
+        """
+        df_sales[key] = pd.to_datetime(df_sales[key])
+        df_holiday[key] = pd.to_datetime(df_holiday[key], format="%d/%m/%Y")
+        df_sales = df_sales.merge(df_holiday, on=key, how="left")
+        return df_sales
+
+    @classmethod
+    def identify_date_occasion(cls, df_sales: pd.DataFrame, holiday_col: str, date_col: str) -> pd.DataFrame:
+        """
+        Identifies holidays in a pandas DataFrame based on a specified column.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the holiday column.
+            holiday_col (str): The name of the column representing the holidays -> "holiday_name"
+            date_col (str): The name of the column representing the dates -> "date"
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'is_holiday'. This column
+            represents whether each row is a holiday (1) or not (0), based on whether the holiday column
+            is null or not.
+        """
+        df_sales["is_holday"] = np.where(df_sales[holiday_col].isnull(), 0, 1)
+        df_sales["is_sunday"] = np.where(df_sales[date_col].dt.day_name() == "Sunday", 1, 0)
+        return df_sales
+
+    @classmethod
+    def feature_combine_str(cls, df_sales: pd.DataFrame, holiday_col_type: str, holiday_col: str) -> pd.DataFrame:
+        """
+        Combines the values of two columns in a pandas DataFrame into a new column as a string.
+        col1='type',col2='holiday_name' -> 'type_holiday_name'
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the two columns to combine.
+            holiday_col_type (str): The name of the first column to combine -> "holiday_type"
+            holiday_col (str): The name of the second column to combine -> "holiday_name"
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called '{col1}_{col2}'. This column
+            represents the concatenation of the values of col1 and col2 as strings, separated by an underscore.
+        """
+        df_sales[f"{holiday_col_type}_{holiday_col}"] = df_sales[holiday_col_type].map(str) + "_" + df_sales[
+            holiday_col].map(str)
+        return df_sales
+
+    @classmethod
+    def calculate_rolling_functions(cls, df_sales: pd.DataFrame, target_col: str, window_size_list: List[int],
+                                    type_functions: List[str]) -> pd.DataFrame:
+        """
+        Calculates the moving average trend for a specified column in a pandas DataFrame.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the target column.
+            target_col (str): The name of the column for which to calculate the trend.
+            window_size_list (int): list size of the rolling window to use when calculating the trend.
+            type_functions (List[str]): The type of trend to calculate. This can be any function
+                from the numpy library that can be applied to a rolling window.
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'trend'. This column represents
+            the moving average trend of the specified target column over the rolling window.
+        """
+        for type_function in type_functions:
+            for window_size in window_size_list:
+                df_sales[f'rolling_{window_size}_{type_functions}'] = df_sales[target_col].rolling(
+                    window=window_size).apply(
+                    getattr(np, type_function)).shift(1).fillna(0)
+        return df_sales
+
+    @classmethod
+    def add_cumulative_sum_column_for_targe(cls, df_sales: pd.DataFrame, col: str) -> pd.DataFrame:
+        """
+        Adds a cumulative sum column to a pandas DataFrame.
+        Args:
+            df (pd.DataFrame): The pandas DataFrame to add the cumulative sum column to.
+            col (str): The name of the column to calculate the cumulative sum for.
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'cumulative_sum'. This column
+            represents the cumulative sum of the specified column.
+        """
+        df_sales[f'cumulative_sum_{col}'] = df_sales[col].cumsum()
+        df_sales[f'cumulative_sum_{col}'] = df_sales[f'cumulative_sum_{col}'].shift(1).fillna(0)
+        return df_sales
+
+    @classmethod
+    def fft_features(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """
+        Extracts spectral analysis features using Fast Fourier Transform (FFT).
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the target column.
+            target_col (str): The name of the column representing the target variable.
+
+        Returns:
+            pd.DataFrame: DataFrame with two new columns: 'fft_real' and 'fft_imag'.
+            These columns represent the real and imaginary parts of the FFT output, respectively.
+        """
+        df_temp = fft(df_sales[target_col].shift(1).fillna(0).values)
+        df_sales['fft_real'] = np.real(df_temp)
+        df_sales['fft_imag'] = np.imag(df_temp)
+        return df_sales
+
+    @classmethod
+    def extract_trend_change(cls, df_sales: pd.DataFrame, trend_col: str) -> pd.DataFrame:
+        """
+        Extracts trend changes in a pandas DataFrame based on peaks in a specified trend column.
+
+        Args:
+            df (pd.DataFrame): The pandas DataFrame containing the trend column.
+            trend_col (str): The name of the column representing the trend -> 'rolling_7_mean'
+
+        Returns:
+            pd.DataFrame: DataFrame with a new column called 'trend_change' indicating
+            trend changes. If the value in the trend column is a local maximum (peak), the value in the
+            'trend_change' column will be set to 1. Otherwise, it will be set to 0.
+        """
+        peaks_extract = argrelextrema(np.array(df_sales[trend_col].shift(1).fillna(0).values), np.greater)
+        df_sales['trend_change'] = 0
+        df_sales.loc[peaks_extract[0], 'trend_change'] = 1
+        return df_sales
+
+    @classmethod
+    def time_series_shape_features(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        """
+        Calculates shape-based features of a time series and adds them as columns to the input dataframe.
+
+        Args:
+            df (pd.DataFrame): The input time series data as a pandas dataframe.
+            target_col (str): The name of the column in the input dataframe that contains the target variable.
+
+        Returns:
+            pd.DataFrame: A pandas dataframe with the same columns as the input dataframe, but with additional columns for the calculated shape-based features.
+        """
+        df_sales['skewness'] = df_sales[target_col].shift(1).fillna(0).skew()
+        df_sales['kurtosis'] = df_sales[target_col].shift(1).fillna(0).kurt()
+        df_sales['slope'] = np.polyfit(df_sales.index, df_sales[target_col].shift(1).fillna(0).values, 1)[0]
+        return df_sales
+
+    @classmethod
+    def add_lagged_feature_to_time_series_of_column(cls, df_sales: pd.DataFrame, cols: list[str],
+                                                    lags_list: List[int]) -> pd.DataFrame:
+        """
+        Add a lagged feature to a time series dataframe.
+
+        Args:
+            df: The dataframe to add the lagged feature to.
+                assumed to be in time series format
+            col: The column to add the lagged feature to.
+            lag: The lag to add to the dataframe.
+
+        Returns:
+            The dataframe with the lagged feature added.
+
+
+        """
+
+        for col in cols:
+            for lag in lags_list:
+                df_sales[f'{col}_lag_{lag}'] = df_sales[col].shift(lag)
+        return df_sales
+
+    @classmethod
+    def convert_str_indicator(cls, df_sales: pd.DataFrame, weekend_col: list[str]) -> pd.DataFrame:
+        """
+        Converts boolean columns in a pandas DataFrame to binary integer columns (0 or 1).
+        Args:
+            df: The input DataFrame.
+            weekend_cols: A list of column names to be converted.
+
+        Returns:
+            The input DataFrame with the specified columns converted to binary integer format.
+        """
+
+        df_sales[weekend_col] = np.where(df_sales[weekend_col] is True, 1, 0)
+        return df_sales
+
+    @classmethod
+    def extract_features_pca(cls, df_sales: pd.DataFrame, date_col: str,
+                             pca_num: int, year_forecast: int = None) -> pd.DataFrame:
+        """
+        Perform Principal Component Analysis (PCA) on a subset of numerical columns in a DataFrame, and append the resulting
+        principal components to the original DataFrame.
+
+        Args:
+            df (pd.DataFrame): The input DataFrame.
+            year_forecast (int): The year after which to exclude data from PCA analysis.
+            pca_num (int): The number of principal components to retain.
+
+        Returns:
+            pd.DataFrame: The input DataFrame with additional columns corresponding to the retained principal components.
+        """
+
+        ##### NOT FOR INFERENCE
+        if year_forecast is None:
+            df_pca = df_sales
+        else:
+            df_pca = df_sales[df_sales[date_col].dt.year < year_forecast].copy()
+
+        df_numeric = df_pca.select_dtypes(include=[np.number])
+        df_numeric = df_numeric.drop(columns=df_numeric.select_dtypes(include='timedelta64').columns.tolist())
+        df_numeric_imputed = df_numeric.fillna(0)
+        pca = PCA(n_components=pca_num)
+        pca.fit(df_numeric_imputed)
+        df_setup_process = df_sales.copy()
+        pca_components = pca.transform(df_setup_process[df_numeric_imputed.columns].fillna(0))
+        columns_pca = [f"PC{i}" for i in range(1, pca_num + 1)]
+        pca_df = pd.DataFrame(pca_components, columns=columns_pca)
+        df_sales[columns_pca] = pca_df
+        return df_sales
+
+    @classmethod
+    def apply_encodings(cls, df_sales: pd.DataFrame, type_encoder_list: List[str], cols_to_encode: List[str],
+                        target_col: str,
+                        year_forecast: int, sigma=1, random_state=12) -> pd.DataFrame:
+        """
+        Applies a set of target encoders to specified columns in a pandas DataFrame.
+
+        Args:
+            target_col:
+            df (pd.DataFrame): The input DataFrame.
+            type_encoder_list (List[str]): A list of target encoders to apply to the specified columns. The encoder names should be strings and correspond to the name of the encoder class from the category_encoders package.
+            ->["GLMMEncoder","MEstimateEncoder","CatBoostEncoder"]
+            cols_to_encode (List[str]): A list of column names to encode.
+            target (str): The name of the target column.
+            year_forecast (int): The year until which to include data.
+            sigma (float): The noise level added to the encoding.
+            random_state (int): The random seed used for the encoding.
+
+        Returns:
+            pd.DataFrame: The encoded DataFrame.
+        """
+        ##### NOT FOR INFERENCE
+        encoder_class_dict = {
+            # "GLMMEncoder": GLMMEncoder,
+            "MEstimateEncoder": MEstimateEncoder,
+            "CatBoostEncoder": CatBoostEncoder
+        }
+        if year_forecast is None:
+            df_filtered = df_sales
+        else:
+            df_filtered = df_sales[df_sales.date.dt.year < year_forecast].copy()
+
+        for encoder_type in type_encoder_list:
+            encoder_class = encoder_class_dict[encoder_type]
+            for col in cols_to_encode:
+                encoder = encoder_class(cols=[col], sigma=sigma, random_state=random_state)
+                if encoder_type == "CatBoostEncoder":
+                    encoder.fit(df_filtered[col].astype(str), df_filtered[target_col])
+                    df_sales[f'{encoder_type}_of_{col}'] = encoder.transform(df_sales[col], df_sales[target_col])
+                else:
+                    encoder.fit(df_filtered[col], df_filtered[target_col])
+                    df_sales[f'{encoder_type}_of_{col}'] = encoder.transform(df_sales[col], df_sales[target_col])
+        return df_sales
+
+    @classmethod
+    def apply_encodings_at_once(cls, df_sales: pd.DataFrame, type_encoder_list: List[str], cols_to_encode: List[str],
+                                target_col: str,
+                                year_forecast: int, sigma=1, random_state: int = 12) -> pd.DataFrame:
+        """
+        Apply multiple category encoders to the same set of columns at once.
+
+        Args:
+            df (pd.DataFrame): The input dataframe to be encoded.
+            type_encoder_list (List[str]): A list of category encoder types to be applied ->["GLMMEncoder","MEstimateEncoder","CatBoostEncoder"]
+            cols (List[str]): A list of column names to be encoded.
+            target (str): The name of the target column to encode against.
+            year_forecast (int): The year forecast limit to use for training data.
+            sigma (float): The regularization parameter for encoders that support it. Default is 1.
+            random_state (int): The random seed to use. Default is 12.
+
+        Returns:
+            pd.DataFrame: A new dataframe with the encoded columns added.
+        """
+        ##### NOT FOR INFERENCE
+        encoder_class_dict = {
+            # "GLMMEncoder": GLMMEncoder,
+            "MEstimateEncoder": MEstimateEncoder,
+            "CatBoostEncoder": CatBoostEncoder
+        }
+        if year_forecast is None:
+            df_filtered = df_sales
+        else:
+            df_filtered = df_sales[df_sales.date.dt.year < year_forecast].copy()
+
+        for encoder_type in type_encoder_list:
+            encoder_class = encoder_class_dict[encoder_type]
+            encoder = encoder_class(cols=cols_to_encode, sigma=sigma, random_state=random_state)
+            if encoder_type == "CatBoostEncoder":
+                encoder.fit(df_filtered[cols_to_encode].astype(str), df_filtered[target_col])
+                encoded_df = encoder.transform(df_sales[cols_to_encode], df_sales[target_col])
+                for col in encoded_df.columns:
+                    df_sales[f'{encoder_type}_of_all_{col}'] = encoded_df[col]
+            else:
+                encoder.fit(df_filtered[cols_to_encode], df_filtered[target_col])
+                encoded_df = encoder.transform(df_sales[cols_to_encode], df_sales[target_col])
+                for col in encoded_df.columns:
+                    df_sales[f'{encoder_type}_of_all_{col}'] = encoded_df[col]
+        return df_sales
+
+    @classmethod
+    def columns_interactions_encoder(cls, df_sales: pd.DataFrame, cols_to_encode_at_once: List[str],
+                                     cols_days_for_interaction: List[str], target_col: str,
+                                     type_encoder_list: List[str], year_forecast: int) -> pd.DataFrame:
+        """
+        Apply feature interaction encoding on specified columns and then encode the new columns using a list of categorical encoders.
+
+        Args:
+            df_sales (pd.DataFrame): The input dataframe to be encoded.
+            cols_to_encode_at_once (List[str]): A list of columns to be encoded at once.
+            cols_days_for_interaction (List[str]): A list of columns to be used for feature interaction.
+            target_col (str): The name of the target column to encode against.
+            type_encoder_list (List[str]): A list of category encoder types to be applied ->["GLMMEncoder","MEstimateEncoder","CatBoostEncoder"]
+            year_forecast (int): The year forecast limit to use for training data.
+
+
+        Returns:
+            pd.DataFrame: A new DataFrame with feature interaction columns and encoded columns using specified categorical encoders.
+
+        """
+        interactions_columns = []
+        for col1 in cols_to_encode_at_once:
+            for col2 in cols_days_for_interaction:
+                df_sales[f"{col1}_interactions_{col2}"] = df_sales[f"{col1}"] * df_sales[f"{col2}"]
+                interactions_columns.append(f"{col1}_interactions_{col2}")
+
+        df_sales = cls.apply_encodings_at_once(df_sales=df_sales, type_encoder_list=type_encoder_list,
+                                               cols_to_encode=interactions_columns,
+                                               target_col=target_col, year_forecast=year_forecast)
+        return df_sales
+
+    @classmethod
+    def remove_expand_dates(cls, df_sales: pd.DataFrame):
+        columns_to_check = ['year', 'month', 'day', 'day_of_week', 'week_of_year', 'quarter', 'is_weekend']
+        if all(column in df_sales.columns for column in columns_to_check):
+            df_sales = df_sales.drop(columns=columns_to_check)
+            print("All specified columns have been dropped.")
+        else:
+            print("Not all specified columns are present in the DataFrame.")
+        return df_sales
+
+    @classmethod
+    def filter_columns_by_correlation(cls, df_sales: pd.DataFrame, year_forecast: int, target_col: str,
+                                      date_col: str) -> List[
+        str]:
+        """
+        Filters the columns in the input dataframe based on their correlation with the target column.
+        Args:
+            df (pd.DataFrame): The input dataframe to be filtered.
+            year_forecast (int): The year forecast limit to use for training data.
+            target_col (str): The name of the target column to be used for correlation analysis.
+            date_col (str): The name of the date column to be used for filtering based on the year forecast.
+
+        Returns:
+            List[str]: A list of column names that are highly correlated with the target column.
+        """
+
+        if year_forecast is None:
+            corr = df_sales.corr()
+        else:
+            corr = df_sales[df_sales[date_col].dt.year < year_forecast].corr()
+
+        corr_target = abs(corr[target_col])
+        relevant_features = corr_target[(corr_target > 0.4) & (corr_target < 1)]
+        selected_col_by_corr = relevant_features.index.tolist()
+        return selected_col_by_corr
+
+    @classmethod
+    def add_back_feature(cls, df_sales: pd.DataFrame, list_col_add: List[str],
+                         selected_col_by_corr: List[str]) -> pd.DataFrame:
+        """
+        Add a list of columns back to the dataframe.
+
+        Args:
+            df_sales:
+            df (pd.DataFrame): The input dataframe.
+            list_col_add (List[str]): A list of column names to add to the dataframe -> ["date",'target']
+            selected_col_by_corr (List[str]): A list of column names to add to the dataframe selected by correlation.
+
+        Returns:
+            pd.DataFrame: A new dataframe with the added columns.
+        """
+        union_list = list_col_add + selected_col_by_corr
+        df_union = df_sales[union_list]
+        return df_union
+
+    @classmethod
+    def process_next_days_events(cls, df_sales: pd.DataFrame, target_col: str) -> pd.DataFrame:
+        df_sales['is_tomorrow_event'] = df_sales['is_event'].shift(-1)
+        df_sales['is_2_days_event'] = df_sales['is_event'].shift(-2)
+
+        # this is only in inferring
+        df_sales[target_col] = df_sales[target_col].shift(-1) + df_sales[target_col].shift(-2)
+        y_prcoess = df_sales["is_2_days_event"].dropna()
+        df_sales_next = df_sales.loc[y_prcoess.index]
+        return df_sales_next
+
+
+def create_interactions_columns(processed_event_features_df):
+    cols_to_encode_at_once = config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_to_encode_at_once']
+    cols_days_for_interaction = config.DEFAULT_EVENT_HANDLER_VARIABLES['cols_days_for_ineraction']
+    for col1 in cols_to_encode_at_once:
+        for col2 in cols_days_for_interaction:
+            processed_event_features_df[f"{col1}_interactions_{col2}"] = processed_event_features_df[f"{col1}"] * \
+                                                                         processed_event_features_df[f"{col2}"]
+
+    return processed_event_features_df
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/lags_feature_handler.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/lags_feature_handler.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-
-import pandas as pd
-
-
-class LagsRollingAverageDiffsEWMsFeaturesGenerator:
-    def __init__(self, df_sales: pd.DataFrame, store_name: str, item_name: str, sales_name: str, date_name: str, end_date: str,
-                 start_date_of_test: str, lags_back: list, windows: list, diff_lags: list, ewms: list):
-        self.df_sales = df_sales
-        self.store_name = store_name
-        self.item_name = item_name
-        self.sales_name = sales_name
-        self.date_name = date_name
-        self.end_date = end_date
-        self.start_date_of_test = start_date_of_test
-        self.lags_back = lags_back
-        self.windows = windows
-        self.diff_lags = diff_lags
-        self.ewms = ewms
-
-
-    def sum_agg_per_item_date_store(self, data):
-        data = data.groupby([self.date_name, self.store_name, self.item_name]).sum(numeric_only=True)[self.sales_name].reset_index()
-        data[self.item_name] = data[self.item_name].astype('category')
-        data[self.store_name] = data[self.store_name].astype('category')
-        return data
-
-    def add_item_store_id_col(self, df):
-        ''' Add a column with the item and store id.
-
-            Args:
-                    df: The dataframe to add the column to.
-                    DEFAULT_item_NAME: The default name of the item column.
-                    DEFAULT_STORE_NAME: The default name of the store column.
-
-            Returns:
-                    The dataframe with the new column.
-
-            '''
-        df['item, store'] = list(zip(df[self.item_name], df[self.store_name]))
-        return df
-
-    def take_more_then_0_sales_and_set_index_to_date(self, data):
-        ''' Take only the rows with more then 0 sales and set the index to the date.
-
-            Args:
-                    data: The dataframe to take the rows from.
-                    DEFAULT_DATE_NAME: The default name of the date column.
-                    DEFAULT_SALES_NAME: The default name of the sales column.
-
-            Returns:
-                    The dataframe with the new index.
-
-            '''
-        data = data[data[self.sales_name] > 0]
-        data = data.set_index(self.date_name)
-        data.index = pd.to_datetime(data.index)
-        return data
-
-    def add_lags_and_rolling_averages_and_diffs_and_ewms(self, df1, item):
-        for lag in self.lags_back:
-            df1[f'{item}_sales_lag_{lag}'] = df1['sales'].shift(lag)
-        for window in self.windows:
-            df1[f'{item}_sales_rolling_{window}'] = df1['sales'].shift(1).rolling(window).mean()
-        for diff_lag in self.diff_lags:
-            df1[f'{item}_sales_diff_{diff_lag}'] = df1['sales'].shift(1) - df1['sales'].shift(diff_lag)
-        for ewm in self.ewms:
-            df1[f'{item}_sales_ewm_{ewm}'] = df1['sales'].shift(1).ewm(alpha=ewm).mean()
-        return df1
-
-    def fill_0_in_gaps_item_store_dates_until_end_date_df(self, df_of_item_store_sales):
-        df_of_item_store_sales = df_of_item_store_sales.reindex(pd.date_range(min(df_of_item_store_sales.index), self.end_date))
-
-        return df_of_item_store_sales
-
-    def return_df_of_item_store_sales_with_lags_rolling_diff_ewm(self, data):
-        df_of_item_store_sales = pd.DataFrame()
-        i = 0
-        for item_store in data["item, store"].unique():
-            i += 1
-            item_store_data = data[data["item, store"] == item_store]
-            item_store_data['item, store'] = [item_store] * len(item_store_data)
-            item_store_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, item_store_data[['sales']], 'id')
-            item_store_data['item, store'] = [item_store] * len(item_store_data)
-            df_of_item_store_sales = pd.concat([item_store_data.reset_index().rename(columns={"index": "date"})])
-        return df_of_item_store_sales
-
-
-    def return_df_of_store_sales_with_lags_rolling_diff_ewm(self, data):
-        df_of_store_sales = pd.DataFrame()
-        i = 0
-        for store in data["store"].unique():
-            i += 1
-            store_data = data[data["store"] == store].groupby("date").sum(numeric_only=True)
-            store_data['store'] = store
-            store_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, store_data[['sales']], self.store_name)
-            store_data['store'] = store
-            df_of_store_sales = pd.concat([store_data.reset_index().rename(columns={"index": "date"})])
-        return df_of_store_sales
-
-    def return_df_of_item_sales_with_lags_rolling_diff_ewm(self, data):
-        df_of_item_sales = pd.DataFrame()
-        i = 0
-        for item in data["item"].unique():
-            i += 1
-            item_data = data[data["item"] == item].groupby("date").sum(numeric_only=True)
-            item_data['item'] = item
-            item_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, item_data[['sales']], self.item_name)
-            item_data['item'] = item
-            df_of_item_sales = pd.concat([item_data.reset_index().rename(columns={"index": "date"})])
-
+
+import pandas as pd
+
+
+class LagsRollingAverageDiffsEWMsFeaturesGenerator:
+    def __init__(self, df_sales: pd.DataFrame, store_name: str, item_name: str, sales_name: str, date_name: str, end_date: str,
+                 start_date_of_test: str, lags_back: list, windows: list, diff_lags: list, ewms: list):
+        self.df_sales = df_sales
+        self.store_name = store_name
+        self.item_name = item_name
+        self.sales_name = sales_name
+        self.date_name = date_name
+        self.end_date = end_date
+        self.start_date_of_test = start_date_of_test
+        self.lags_back = lags_back
+        self.windows = windows
+        self.diff_lags = diff_lags
+        self.ewms = ewms
+
+
+    def sum_agg_per_item_date_store(self, data):
+        data = data.groupby([self.date_name, self.store_name, self.item_name]).sum(numeric_only=True)[self.sales_name].reset_index()
+        data[self.item_name] = data[self.item_name].astype('category')
+        data[self.store_name] = data[self.store_name].astype('category')
+        return data
+
+    def add_item_store_id_col(self, df):
+        ''' Add a column with the item and store id.
+
+            Args:
+                    df: The dataframe to add the column to.
+                    DEFAULT_item_NAME: The default name of the item column.
+                    DEFAULT_STORE_NAME: The default name of the store column.
+
+            Returns:
+                    The dataframe with the new column.
+
+            '''
+        df['item, store'] = list(zip(df[self.item_name], df[self.store_name]))
+        return df
+
+    def take_more_then_0_sales_and_set_index_to_date(self, data):
+        ''' Take only the rows with more then 0 sales and set the index to the date.
+
+            Args:
+                    data: The dataframe to take the rows from.
+                    DEFAULT_DATE_NAME: The default name of the date column.
+                    DEFAULT_SALES_NAME: The default name of the sales column.
+
+            Returns:
+                    The dataframe with the new index.
+
+            '''
+        data = data[data[self.sales_name] > 0]
+        data = data.set_index(self.date_name)
+        data.index = pd.to_datetime(data.index)
+        return data
+
+    def add_lags_and_rolling_averages_and_diffs_and_ewms(self, df1, item):
+        for lag in self.lags_back:
+            df1[f'{item}_sales_lag_{lag}'] = df1['sales'].shift(lag)
+        for window in self.windows:
+            df1[f'{item}_sales_rolling_{window}'] = df1['sales'].shift(1).rolling(window).mean()
+        for diff_lag in self.diff_lags:
+            df1[f'{item}_sales_diff_{diff_lag}'] = df1['sales'].shift(1) - df1['sales'].shift(diff_lag)
+        for ewm in self.ewms:
+            df1[f'{item}_sales_ewm_{ewm}'] = df1['sales'].shift(1).ewm(alpha=ewm).mean()
+        return df1
+
+    def fill_0_in_gaps_item_store_dates_until_end_date_df(self, df_of_item_store_sales):
+        df_of_item_store_sales = df_of_item_store_sales.reindex(pd.date_range(min(df_of_item_store_sales.index), self.end_date))
+
+        return df_of_item_store_sales
+
+    def return_df_of_item_store_sales_with_lags_rolling_diff_ewm(self, data):
+        df_of_item_store_sales = pd.DataFrame()
+        i = 0
+        for item_store in data["item, store"].unique():
+            i += 1
+            item_store_data = data[data["item, store"] == item_store]
+            item_store_data['item, store'] = [item_store] * len(item_store_data)
+            item_store_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, item_store_data[['sales']], 'id')
+            item_store_data['item, store'] = [item_store] * len(item_store_data)
+            df_of_item_store_sales = pd.concat([item_store_data.reset_index().rename(columns={"index": "date"})])
+        return df_of_item_store_sales
+
+
+    def return_df_of_store_sales_with_lags_rolling_diff_ewm(self, data):
+        df_of_store_sales = pd.DataFrame()
+        i = 0
+        for store in data["store"].unique():
+            i += 1
+            store_data = data[data["store"] == store].groupby("date").sum(numeric_only=True)
+            store_data['store'] = store
+            store_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, store_data[['sales']], self.store_name)
+            store_data['store'] = store
+            df_of_store_sales = pd.concat([store_data.reset_index().rename(columns={"index": "date"})])
+        return df_of_store_sales
+
+    def return_df_of_item_sales_with_lags_rolling_diff_ewm(self, data):
+        df_of_item_sales = pd.DataFrame()
+        i = 0
+        for item in data["item"].unique():
+            i += 1
+            item_data = data[data["item"] == item].groupby("date").sum(numeric_only=True)
+            item_data['item'] = item
+            item_data = LagsRollingAverageDiffsEWMsFeaturesGenerator.add_lags_and_rolling_averages_and_diffs_and_ewms(self, item_data[['sales']], self.item_name)
+            item_data['item'] = item
+            df_of_item_sales = pd.concat([item_data.reset_index().rename(columns={"index": "date"})])
+
         return df_of_item_sales
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/preprocessor.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/preprocessor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,171 +1,170 @@
-import pandas as pd
-from . import config as global_config
-from .features.event_features import EventFeaturesGenerator
-from .features.future_features import FarFutureFeaturesGenerator
-from .features.lags_features import ItemLagFeatureGenerator, StoreLagFeatureGenerator, IDLagFeatureGenerator
-from .features.weather_features import WeatherFeatureGenerator
-# from .regular_data_handler import RegularDataLoader
-from .utils import parse_regular_data_columns,daily_sales_to_weekly_mean_sales
-from .features.cumulative_features import CumulativeFeatureGenerator
-
-
-class Preprocessor:
-    def __init__(self):
-        pass
-
-    @classmethod
-    def get_future_rows(cls, regular_data_df: pd.DataFrame, begin_date: str, end_date: str):
-        """
-        Creates the future rows for prediction as a dataframe
-        Args:
-            regular_data_df: regular data dataframe
-            begin_date: begin date of prediction
-            end_date: end date of prediction
-
-        Returns:
-            dataframe with future rows
-        notes:
-        1) The names of the input columns must be the same as the global_config
-        2) for now the begin_date and end_date must be the same as the prediction date but for future it can be an iterative process
-        """
-        unique_ids = regular_data_df[global_config.ITEM_STORE_COLUMN_NAME].unique()
-
-        dfs = []
-        for date in pd.date_range(begin_date, end_date):
-            df = pd.DataFrame(
-                {global_config.ITEM_STORE_COLUMN_NAME: unique_ids, global_config.DATE_COLUMN_NAME: date})
-            df[[global_config.ITEM_COLUMN_NAME, global_config.STORE_COLUMN_NAME]] = df[
-                global_config.ITEM_STORE_COLUMN_NAME].str.split(", ", expand=True)
-            dfs.append(df)
-
-        # future_df = pd.DataFrame(
-        #     {global_config.ITEM_STORE_COLUMN_NAME: unique_ids, global_config.DATE_COLUMN_NAME: begin_date})
-        # future_df[[global_config.ITEM_COLUMN_NAME, global_config.STORE_COLUMN_NAME]] = future_df[
-        #     global_config.ITEM_STORE_COLUMN_NAME].str.split(", ", expand=True)
-
-        return pd.concat(dfs)
-
-    @classmethod
-    def create_store_id_dict(cls, regular_data_df: pd.DataFrame):
-        """
-        Create a dictionary with store as key and list of items as value
-        Args:
-            regular_data_df:    regular data dataframe
-
-        Returns:
-            dictionary with store as key and list of items as value
-
-        """
-        item_store_dict = regular_data_df.groupby(global_config.STORE_COLUMN_NAME)[
-            global_config.ITEM_STORE_COLUMN_NAME].unique().apply(list).to_dict()
-        return item_store_dict
-
-    @classmethod
-    def preprocess(cls, stores_list: list[int] = global_config.OUTLETS_SDATTA, marketing_plan: pd.DataFrame = None,
-                   item_encoders = None, store_encoders = None, store_location_df: pd.DataFrame = None,
-                   begin_predict_dates: str = global_config.tomorrow_date, event_encoders: dict = None,
-                   regular_data_df: pd.DataFrame = None, event_df: pd.DataFrame = None,
-                   holiday_df: pd.DataFrame = None):
-        """
-        Preprocess data for prediction and return a dataframe with all features:
-        1) event features
-        2) weather features
-        3) lag features
-        4) cumulative features
-
-        Args:
-            stores_list: list of stores to predict
-            begin_predict_dates: date to predict
-            regular_data_df: regular data dataframe
-            event_df: event dataframe
-            holiday_df: holiday dataframe
-
-        :return:
-            dataframe with all features
-
-        Notes:
-        dataframe must have the following columns:
-        1) date
-        2) item
-        3) store
-        4) item_store
-        """
-        if pd.to_datetime(begin_predict_dates).strftime("%A") == "Sunday":
-            print("predict_date is Sunday, no need to predict")
-            return
-
-        # if need to load regular data
-        # if regular_data_df is None:
-        #     regular_data_df = RegularDataLoader().load()
-
-        # TODO: seperate the two days being added for events
-        future_df = cls.get_future_rows(regular_data_df, begin_predict_dates, begin_predict_dates)
-        regular_data_df = parse_regular_data_columns(pd.concat([regular_data_df, future_df], ignore_index=True))
-        regular_data_df = daily_sales_to_weekly_mean_sales(regular_data_df)
-        final_event_features_df = EventFeaturesGenerator().generate(regular_data_df, event_df, holiday_df,
-                                                                    event_encoders,
-                                                                    begin_predict_dates=begin_predict_dates)
-        # TODO: first load store_location_here, then call weather prediction someplace else.
-        # store_location_df = StoreLocationLoader().load() # on all stores
-        cumulative_features_df = CumulativeFeatureGenerator().run_pipline_cumulative(regular_data_df)
-        item_lags_features_df = ItemLagFeatureGenerator().create_all_item_lags(regular_data_df, begin_predict_dates)
-        # TODO: after the sku_lags, we can filter the regular data (Check this!!!!!)
-        regular_data_df = regular_data_df[regular_data_df[global_config.STORE_COLUMN_NAME].isin(stores_list)]
-        store_id_dict = cls.create_store_id_dict(regular_data_df)
-        far_future_features_df = FarFutureFeaturesGenerator().far_future_features_preprocess_of_several_stores(
-            marketing_plan=marketing_plan, item_encoders=item_encoders, store_encoders=store_encoders,
-            store_batch_dict=store_id_dict, begin_predict_dates=begin_predict_dates)
-        all_ids_data_for_predict_date = pd.DataFrame()
-
-        for store in stores_list:
-            all_id_data_in_store = pd.DataFrame()
-            store_data_df = regular_data_df[regular_data_df[global_config.STORE_COLUMN_NAME] == store]
-            store_future_features = far_future_features_df[store]  # feature
-            store_lags_df = StoreLagFeatureGenerator().create_all_stores_lags(store_data_df,
-                                                                              predict_date=begin_predict_dates)  # feature
-            stores_weather_df = WeatherFeatureGenerator().generate(store_location_df=store_location_df, store_id=store,
-                                                                   start_predict_date=begin_predict_dates,
-                                                                   end_predict_date=begin_predict_dates)
-
-            for item in store_data_df[global_config.ITEM_COLUMN_NAME].unique():
-                _id = str(item) + ", " + str(store)
-                id_data_df = store_data_df[store_data_df[global_config.ITEM_STORE_COLUMN_NAME] == _id]
-
-                id_data_df = IDLagFeatureGenerator().create_id_lags(id_data_df=id_data_df, item=item, store=store,
-                                                                    predict_date=begin_predict_dates)  # feature
-                # id_data_df[global_config.ITEM_STORE_COLUMN_NAME] = _id
-                all_id_data_in_store = pd.concat([all_id_data_in_store, id_data_df])
-
-            all_id_data_in_store = all_id_data_in_store.merge(store_future_features,
-                                                              on=[global_config.DATE_COLUMN_NAME,
-                                                                  global_config.ITEM_COLUMN_NAME,
-                                                                  global_config.STORE_COLUMN_NAME],
-                                                              how="left")
-
-            all_id_data_in_store = all_id_data_in_store.merge(store_lags_df,
-                                                              on=[global_config.DATE_COLUMN_NAME],
-                                                              how="left")
-            all_id_data_in_store = all_id_data_in_store.merge(stores_weather_df, on=[global_config.DATE_COLUMN_NAME,
-                                                                                     global_config.STORE_COLUMN_NAME],
-                                                              how="left")
-
-            all_id_data_in_store = all_id_data_in_store.merge(cumulative_features_df,
-                                                              on=[global_config.DATE_COLUMN_NAME,
-                                                                  global_config.ITEM_COLUMN_NAME,
-                                                                  global_config.STORE_COLUMN_NAME], how="left")
-
-            all_ids_data_for_predict_date = pd.concat([all_ids_data_for_predict_date, all_id_data_in_store])
-
-        all_ids_data_for_predict_date = all_ids_data_for_predict_date.merge(item_lags_features_df,
-                                                                            on=[global_config.DATE_COLUMN_NAME,
-                                                                                global_config.ITEM_COLUMN_NAME,
-                                                                                ],
-                                                                            how="left")
-        all_ids_data_for_predict_date = all_ids_data_for_predict_date.merge(final_event_features_df,
-                                                                            on=[global_config.DATE_COLUMN_NAME],
-                                                                            how="left")
-        all_ids_data_for_predict_date.columns = all_ids_data_for_predict_date.columns.str.replace(':', '')
-        cols_to_drop = [col for col in all_ids_data_for_predict_date.columns if 'MEST_all_time' in col
-                        or 'months_5_6_7' in col or col == 'index']
-        all_ids_data_for_predict_date.drop(cols_to_drop, axis=1, inplace=True)
-        return all_ids_data_for_predict_date
+import pandas as pd
+from . import config as global_config
+from .features.event_features import EventFeaturesGenerator
+from .features.future_features import FarFutureFeaturesGenerator
+from .features.lags_features import ItemLagFeatureGenerator, StoreLagFeatureGenerator, IDLagFeatureGenerator
+from .features.weather_features import WeatherFeatureGenerator
+# from .regular_data_handler import RegularDataLoader
+from .utils import parse_regular_data_columns,daily_sales_to_weekly_mean_sales,convert_df_with_sku_to_df_with_item
+from .features.cumulative_features import CumulativeFeatureGenerator
+
+
+class Preprocessor:
+    def __init__(self):
+        pass
+
+
+    @classmethod
+    def get_future_rows(cls, regular_data_df: pd.DataFrame, begin_date: str, end_date: str):
+        """
+        Creates the future rows for prediction as a dataframe
+        Args:
+            regular_data_df: regular data dataframe
+            begin_date: begin date of prediction
+            end_date: end date of prediction
+
+        Returns:
+            dataframe with future rows
+        notes:
+        1) The names of the input columns must be the same as the global_config
+        2) for now the begin_date and end_date must be the same as the prediction date but for future it can be an iterative process
+        """
+        unique_ids = regular_data_df[global_config.ITEM_STORE_COLUMN_NAME].unique()
+
+        dfs = []
+        for date in pd.date_range(begin_date, end_date):
+            df = pd.DataFrame(
+                {global_config.ITEM_STORE_COLUMN_NAME: unique_ids, global_config.DATE_COLUMN_NAME: date})
+            df[[global_config.ITEM_COLUMN_NAME, global_config.STORE_COLUMN_NAME]] = df[
+                global_config.ITEM_STORE_COLUMN_NAME].str.split(", ", expand=True)
+            dfs.append(df)
+
+        # future_df = pd.DataFrame(
+        #     {global_config.ITEM_STORE_COLUMN_NAME: unique_ids, global_config.DATE_COLUMN_NAME: begin_date})
+        # future_df[[global_config.ITEM_COLUMN_NAME, global_config.STORE_COLUMN_NAME]] = future_df[
+        #     global_config.ITEM_STORE_COLUMN_NAME].str.split(", ", expand=True)
+
+        return pd.concat(dfs)
+
+    @classmethod
+    def create_store_id_dict(cls, regular_data_df: pd.DataFrame):
+        """
+        Create a dictionary with store as key and list of items as value
+        Args:
+            regular_data_df:    regular data dataframe
+
+        Returns:
+            dictionary with store as key and list of items as value
+
+        """
+        item_store_dict = regular_data_df.groupby(global_config.STORE_COLUMN_NAME)[
+            global_config.ITEM_STORE_COLUMN_NAME].unique().apply(list).to_dict()
+        return item_store_dict
+
+    @classmethod
+    def preprocess(cls, stores_list: list[int] = global_config.OUTLETS_SDATTA, marketing_plan: pd.DataFrame = None,
+                   item_encoders = None, store_encoders = None, store_location_df: pd.DataFrame = None,
+                   begin_predict_dates: str = global_config.tomorrow_date, event_encoders: dict = None,
+                   regular_data_df: pd.DataFrame = None, event_df: pd.DataFrame = None,
+                   holiday_df: pd.DataFrame = None):
+        """
+        Preprocess data for prediction and return a dataframe with all features:
+        1) event features
+        2) weather features
+        3) lag features
+        4) cumulative features
+
+        Args:
+            stores_list: list of stores to predict
+            begin_predict_dates: date to predict
+            regular_data_df: regular data dataframe
+            event_df: event dataframe
+            holiday_df: holiday dataframe
+
+        :return:
+            dataframe with all features
+
+        Notes:
+        dataframe must have the following columns:
+        1) date
+        2) item
+        3) store
+        4) item_store
+        """
+        if pd.to_datetime(begin_predict_dates).strftime("%A") == "Sunday":
+            print("predict_date is Sunday, no need to predict")
+            return
+
+        # TODO: seperate the two days being added for events
+        regular_data_df = convert_df_with_sku_to_df_with_item(regular_data_df)
+        regular_data_df = daily_sales_to_weekly_mean_sales(regular_data_df)
+        future_df = cls.get_future_rows(regular_data_df, begin_predict_dates, begin_predict_dates)
+        regular_data_df = parse_regular_data_columns(pd.concat([regular_data_df, future_df], ignore_index=True))
+        final_event_features_df = EventFeaturesGenerator().generate(regular_data_df, event_df, holiday_df,
+                                                                    event_encoders,
+                                                                    begin_predict_dates=begin_predict_dates)
+        # TODO: first load store_location_here, then call weather prediction someplace else.
+        # store_location_df = StoreLocationLoader().load() # on all stores
+        cumulative_features_df = CumulativeFeatureGenerator().run_pipline_cumulative(regular_data_df)
+        item_lags_features_df = ItemLagFeatureGenerator().create_all_item_lags(regular_data_df, begin_predict_dates)
+        # TODO: after the sku_lags, we can filter the regular data (Check this!!!!!)
+        regular_data_df = regular_data_df[regular_data_df[global_config.STORE_COLUMN_NAME].isin(stores_list)]
+        store_id_dict = cls.create_store_id_dict(regular_data_df)
+        far_future_features_df = FarFutureFeaturesGenerator().far_future_features_preprocess_of_several_stores(
+            marketing_plan=marketing_plan, item_encoders=item_encoders, store_encoders=store_encoders,
+            store_batch_dict=store_id_dict, begin_predict_dates=begin_predict_dates)
+        all_ids_data_for_predict_date = pd.DataFrame()
+
+        for store in stores_list:
+            all_id_data_in_store = pd.DataFrame()
+            store_data_df = regular_data_df[regular_data_df[global_config.STORE_COLUMN_NAME] == store]
+            store_future_features = far_future_features_df[store]  # feature
+            store_lags_df = StoreLagFeatureGenerator().create_all_stores_lags(store_data_df,
+                                                                              predict_date=begin_predict_dates)  # feature
+            stores_weather_df = WeatherFeatureGenerator().generate(store_location_df=store_location_df, store_id=store,
+                                                                   start_predict_date=begin_predict_dates,
+                                                                   end_predict_date=begin_predict_dates)
+
+            for item in store_data_df[global_config.ITEM_COLUMN_NAME].unique():
+                _id = str(item) + ", " + str(store)
+                id_data_df = store_data_df[store_data_df[global_config.ITEM_STORE_COLUMN_NAME] == _id]
+
+                id_data_df = IDLagFeatureGenerator().create_id_lags(id_data_df=id_data_df, item=item, store=store,
+                                                                    predict_date=begin_predict_dates)  # feature
+                # id_data_df[global_config.ITEM_STORE_COLUMN_NAME] = _id
+                all_id_data_in_store = pd.concat([all_id_data_in_store, id_data_df])
+
+            all_id_data_in_store = all_id_data_in_store.merge(store_future_features,
+                                                              on=[global_config.DATE_COLUMN_NAME,
+                                                                  global_config.ITEM_COLUMN_NAME,
+                                                                  global_config.STORE_COLUMN_NAME],
+                                                              how="left")
+
+            all_id_data_in_store = all_id_data_in_store.merge(store_lags_df,
+                                                              on=[global_config.DATE_COLUMN_NAME],
+                                                              how="left")
+            all_id_data_in_store = all_id_data_in_store.merge(stores_weather_df, on=[global_config.DATE_COLUMN_NAME,
+                                                                                     global_config.STORE_COLUMN_NAME],
+                                                              how="left")
+
+            all_id_data_in_store = all_id_data_in_store.merge(cumulative_features_df,
+                                                              on=[global_config.DATE_COLUMN_NAME,
+                                                                  global_config.ITEM_COLUMN_NAME,
+                                                                  global_config.STORE_COLUMN_NAME], how="left")
+
+            all_ids_data_for_predict_date = pd.concat([all_ids_data_for_predict_date, all_id_data_in_store])
+
+        all_ids_data_for_predict_date = all_ids_data_for_predict_date.merge(item_lags_features_df,
+                                                                            on=[global_config.DATE_COLUMN_NAME,
+                                                                                global_config.ITEM_COLUMN_NAME,
+                                                                                ],
+                                                                            how="left")
+        all_ids_data_for_predict_date = all_ids_data_for_predict_date.merge(final_event_features_df,
+                                                                            on=[global_config.DATE_COLUMN_NAME],
+                                                                            how="left")
+        all_ids_data_for_predict_date.columns = all_ids_data_for_predict_date.columns.str.replace(':', '')
+        cols_to_drop = [col for col in all_ids_data_for_predict_date.columns if 'MEST_all_time' in col
+                        or 'months_5_6_7' in col or col == 'index']
+        all_ids_data_for_predict_date.drop(cols_to_drop, axis=1, inplace=True)
+        return all_ids_data_for_predict_date
+
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/utils.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-from datetime import timedelta, datetime
-
-import numpy as np
-import pandas as pd
-from . import config
-
-
-def process_date_column(df_sales: pd.DataFrame, date_col: str, expanded: bool = False) -> pd.DataFrame:
-    """
-    Process date column
-    Args:
-        df_sales: pandas DataFrame
-        date_col: name of date column
-    Returns: pandas DataFrame
-    """
-    df_sales[date_col] = pd.to_datetime(df_sales[date_col])
-    df_sales['year'] = df_sales[date_col].dt.year
-    df_sales['month'] = df_sales[date_col].dt.month
-    df_sales['day'] = df_sales[date_col].dt.day
-    df_sales['day_of_week'] = df_sales[date_col].dt.dayofweek
-    df_sales['week_of_year'] = df_sales[date_col].apply(lambda x: x.isocalendar()[1])
-    df_sales['quarter'] = df_sales[date_col].dt.quarter
-    df_sales['is_weekend'] = df_sales[date_col].dt.dayofweek.isin([5, 6]).astype(int)
-    df_sales['name_of_day'] = df_sales[date_col].dt.strftime("%A")
-
-    if expanded:
-        df_sales['day_of_year'] = df_sales[date_col].dt.dayofyear
-        df_sales['day_of_the_month'] = df_sales[date_col].dt.days_in_month
-        df_sales['is_weekend_c'] = df_sales['day_of_week'].apply(lambda x: 1 if x in [5, 6] else 0)
-        df_sales['is_weekend_j'] = df_sales['day_of_week'].apply(lambda x: 1 if x in [4, 5] else 0)
-
-    return df_sales
-
-
-def add_values_to_dict_mapper(dict_mapper: dict, df_encoders: pd.DataFrame, column_name: str, encoders_name: list,
-                              dict_of_time_interval: dict) -> dict:
-    """
-    Adds the values of the encoders in the df_encoders dataframe to the dict_maper dictionary.
-
-    Args:
-        dict_mapper:     The dictionary that holds the encoded values.
-        df_encoders:        The dataframe that holds the encoded values.
-        column_name:    The name of the column in the df_encoders dataframe.
-        encoders_name:  The names of the encoders in the df_encoders dataframe.
-        dict_of_time_interval:  The dictionary that holds the time intervals.
-
-    Returns:    The updated dict_maper dictionary.
-
-    """
-    item_encoders_with_item_index = df_encoders.rename_axis(column_name)
-    for item in df_encoders.index:
-        for time in dict_of_time_interval:
-            for date in dict_of_time_interval[time]:
-                for encoder in encoders_name:
-                    if time == "months_5_6_7":
-                        dict_mapper[column_name][encoder]["months_5_6_7"][(item, date)] = \
-                            item_encoders_with_item_index.loc[item][encoder + "_months:5_6_7"]
-                    elif time == "all":
-                        dict_mapper[column_name][encoder]["all"][(item, date)] = \
-                            item_encoders_with_item_index.loc[item][encoder + "_all_time:all_time"]
-                    else:
-                        dict_mapper[column_name][encoder][time][(item, date)] = \
-                            item_encoders_with_item_index.loc[item][encoder + "_" + str(time) + ":" + str(date)]
-    return dict_mapper
-
-
-def map_encoders_columns_to_base_df(data: pd.DataFrame, dict_map: dict, encoders_name: list) -> pd.DataFrame:
-    """
-    Adds the encoded values to the data dataframe.
-    Args:
-        data:   The dataframe to add the encoded values to.
-        dict_map:   The dictionary that holds the encoded values.
-        encoders_name:  The names of the encoders in the df_encoders dataframe.
-
-    Returns:    The updated data dataframe.
-
-    """
-    for encoder_name in encoders_name:
-        data[encoder_name + "_day_store"] = data.apply(
-            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["name_of_day"][
-                x[config.STORE_COLUMN_NAME], x["name_of_day"]], axis=1)
-        data[encoder_name + "_day_item"] = data.apply(
-            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["name_of_day"][
-                x[config.ITEM_COLUMN_NAME], x["name_of_day"]], axis=1)
-        data[encoder_name + "_month_store"] = data.apply(
-            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["month"][
-                x[config.STORE_COLUMN_NAME], x["month"]], axis=1)
-        data[encoder_name + "_month_item"] = data.apply(
-            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["month"][x[config.ITEM_COLUMN_NAME], x["month"]],
-            axis=1)
-        data[encoder_name + "_quarter_store"] = data.apply(
-            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["quarter"][
-                x[config.STORE_COLUMN_NAME], x["quarter"]], axis=1)
-        data[encoder_name + "_quarter_item"] = data.apply(
-            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["quarter"][
-                x[config.ITEM_COLUMN_NAME], x["quarter"]], axis=1)
-
-        data[encoder_name + "_day_store"] = data[encoder_name + "_day_store"].astype("float")
-        data[encoder_name + "_day_item"] = data[encoder_name + "_day_item"].astype("float")
-        data[encoder_name + "_month_store"] = data[encoder_name + "_month_store"].astype("float")
-        data[encoder_name + "_month_item"] = data[encoder_name + "_month_item"].astype("float")
-        data[encoder_name + "_quarter_store"] = data[encoder_name + "_quarter_store"].astype("float")
-        data[encoder_name + "_quarter_item"] = data[encoder_name + "_quarter_item"].astype("float")
-
-        return data
-
-
-def parse_regular_data_columns(data: pd.DataFrame, item_col_str: str = config.ITEM_COLUMN_NAME,
-                               store_col_str: str = config.STORE_COLUMN_NAME,
-                               sales_col_str: str = config.SALES_COLUMN_NAME,
-                               date_col_str: str = config.DATE_COLUMN_NAME,
-                               item_store_col_str: str = config.ITEM_STORE_COLUMN_NAME) -> pd.DataFrame:
-    """
-    Parses the columns of the data dataframe to the correct data type.
-
-    Args:
-        data: The dataframe to parse.
-        item_col_str: The name of the item column.
-        store_col_str: The name of the store column.
-        sales_col_str: The name of the sales column.
-        date_col_str: The name of the date column.
-        item_store_col_str: The name of the item_store column.
-
-    Returns:
-        The updated data dataframe.
-
-    Notes:
-    1) item_col_str -> np.int64
-    2) store_col_str -> np.int32
-    3) sales_col_str -> np.float32
-    4) date_col_str -> pd.to_datetime
-    5) item_store_col_str -> str
-    """
-    if item_col_str in data.columns:
-        data[item_col_str] = data[item_col_str].astype(np.int64)
-    if store_col_str in data.columns:
-        data[store_col_str] = data[store_col_str].astype(np.int32)
-    if sales_col_str in data.columns:
-        data[sales_col_str] = data[sales_col_str].astype(np.float32)
-    if date_col_str in data.columns:
-        data[date_col_str] = pd.to_datetime(data[date_col_str])
-    if item_store_col_str in data.columns:
-        data[item_store_col_str] = data[item_store_col_str].astype(str)
-    return data
-
-
-def next_two_days_skip_sunday(start_date:str):
-    """
-    This function returns the next two days after the start date, skipping Sunday.
-
-    Args:
-        start_date: The start date
-
-    Returns:
-        A list of the next two days after the start date, skipping Sunday.
-
-    """
-    dates = []
-    start_date = datetime.strptime(start_date, '%Y-%m-%d')
-    for i in range(2):
-        start_date += timedelta(days=1)
-        if start_date.weekday() == 6:
-            start_date += timedelta(days=1)
-        dates.append(start_date)
-
-    return dates
-
-
-def convert_df_with_sku_to_df_with_item(df: pd.DataFrame) -> pd.DataFrame:
-    """
-    Converts a dataframe with sku to a dataframe with item and group by date, item, store and sales.
-    Args:
-        df:     The dataframe to convert.
-
-    Returns:
-        The converted dataframe.
-
-    """
-    df[config.ITEM_COLUMN_NAME] = df[config.SKU_COLUMN_NAME].str[:-3]
-    df[config.SALES_COLUMN_NAME] = df[config.SALES_COLUMN_NAME].astype(float)
-    df[config.ITEM_STORE_COLUMN_NAME] = df[config.ITEM_COLUMN_NAME] + ", " + df[config.STORE_COLUMN_NAME]
-    df = df[[config.DATE_COLUMN_NAME, config.ITEM_STORE_COLUMN_NAME, config.ITEM_COLUMN_NAME, config.STORE_COLUMN_NAME,
-             config.SALES_COLUMN_NAME]]
-    df = df.groupby(
-        [config.DATE_COLUMN_NAME, config.ITEM_STORE_COLUMN_NAME, config.ITEM_COLUMN_NAME, config.STORE_COLUMN_NAME])[
-        config.SALES_COLUMN_NAME].sum().reset_index()
-    return df
-
-
-def daily_sales_to_weekly_mean_sales(df: pd.DataFrame) -> pd.DataFrame:
-    """
-    This function converts the daily sales to weekly mean sales.
-    with groupby on item_store and rolling mean of 6 days - excluding the sunday.
-    Args:
-        df:     The dataframe to convert.
-
-    Returns:
-        The converted dataframe.
-    """
-    df_with_window_6_rolling = pd.DataFrame()
-    grouped = df.groupby([config.ITEM_STORE_COLUMN_NAME])
-    for name, group in grouped:
-        group_rolling = group.groupby(config.DATE_COLUMN_NAME)[config.SALES_COLUMN_NAME].sum().rolling(6,
-                                                                                                       min_periods=6).mean().reset_index()
-        group_rolling[config.ITEM_STORE_COLUMN_NAME] = name
-        group_rolling[config.ITEM_COLUMN_NAME] = name.split(", ")[0]
-        group_rolling[config.STORE_COLUMN_NAME] = name.split(", ")[1]
-        df_with_window_6_rolling = pd.concat([df_with_window_6_rolling, group_rolling])
-    df_with_window_6_rolling.reset_index(drop=True, inplace=True)
-    df_with_window_6_rolling = df_with_window_6_rolling.dropna(subset=[config.SALES_COLUMN_NAME])
-    return df_with_window_6_rolling
+from datetime import timedelta, datetime
+
+import numpy as np
+import pandas as pd
+from . import config
+
+
+def process_date_column(df_sales: pd.DataFrame, date_col: str, expanded: bool = False) -> pd.DataFrame:
+    """
+    Process date column
+    Args:
+        df_sales: pandas DataFrame
+        date_col: name of date column
+    Returns: pandas DataFrame
+    """
+    df_sales[date_col] = pd.to_datetime(df_sales[date_col])
+    df_sales['year'] = df_sales[date_col].dt.year
+    df_sales['month'] = df_sales[date_col].dt.month
+    df_sales['day'] = df_sales[date_col].dt.day
+    df_sales['day_of_week'] = df_sales[date_col].dt.dayofweek
+    df_sales['week_of_year'] = df_sales[date_col].apply(lambda x: x.isocalendar()[1])
+    df_sales['quarter'] = df_sales[date_col].dt.quarter
+    df_sales['is_weekend'] = df_sales[date_col].dt.dayofweek.isin([5, 6]).astype(int)
+    df_sales['name_of_day'] = df_sales[date_col].dt.strftime("%A")
+
+    if expanded:
+        df_sales['day_of_year'] = df_sales[date_col].dt.dayofyear
+        df_sales['day_of_the_month'] = df_sales[date_col].dt.days_in_month
+        df_sales['is_weekend_c'] = df_sales['day_of_week'].apply(lambda x: 1 if x in [5, 6] else 0)
+        df_sales['is_weekend_j'] = df_sales['day_of_week'].apply(lambda x: 1 if x in [4, 5] else 0)
+
+    return df_sales
+
+
+def add_values_to_dict_mapper(dict_mapper: dict, df_encoders: pd.DataFrame, column_name: str, encoders_name: list,
+                              dict_of_time_interval: dict) -> dict:
+    """
+    Adds the values of the encoders in the df_encoders dataframe to the dict_maper dictionary.
+
+    Args:
+        dict_mapper:     The dictionary that holds the encoded values.
+        df_encoders:        The dataframe that holds the encoded values.
+        column_name:    The name of the column in the df_encoders dataframe.
+        encoders_name:  The names of the encoders in the df_encoders dataframe.
+        dict_of_time_interval:  The dictionary that holds the time intervals.
+
+    Returns:    The updated dict_maper dictionary.
+
+    """
+    item_encoders_with_item_index = df_encoders.rename_axis(column_name)
+    for item in df_encoders.index:
+        for time in dict_of_time_interval:
+            for date in dict_of_time_interval[time]:
+                for encoder in encoders_name:
+                    if time == "months_5_6_7":
+                        dict_mapper[column_name][encoder]["months_5_6_7"][(item, date)] = \
+                            item_encoders_with_item_index.loc[item][encoder + "_months:5_6_7"]
+                    elif time == "all":
+                        dict_mapper[column_name][encoder]["all"][(item, date)] = \
+                            item_encoders_with_item_index.loc[item][encoder + "_all_time:all_time"]
+                    else:
+                        dict_mapper[column_name][encoder][time][(item, date)] = \
+                            item_encoders_with_item_index.loc[item][encoder + "_" + str(time) + ":" + str(date)]
+    return dict_mapper
+
+
+def map_encoders_columns_to_base_df(data: pd.DataFrame, dict_map: dict, encoders_name: list) -> pd.DataFrame:
+    """
+    Adds the encoded values to the data dataframe.
+    Args:
+        data:   The dataframe to add the encoded values to.
+        dict_map:   The dictionary that holds the encoded values.
+        encoders_name:  The names of the encoders in the df_encoders dataframe.
+
+    Returns:    The updated data dataframe.
+
+    """
+    for encoder_name in encoders_name:
+        data[encoder_name + "_day_store"] = data.apply(
+            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["name_of_day"][
+                x[config.STORE_COLUMN_NAME], x["name_of_day"]], axis=1)
+        data[encoder_name + "_day_item"] = data.apply(
+            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["name_of_day"][
+                x[config.ITEM_COLUMN_NAME], x["name_of_day"]], axis=1)
+        data[encoder_name + "_month_store"] = data.apply(
+            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["month"][
+                x[config.STORE_COLUMN_NAME], x["month"]], axis=1)
+        data[encoder_name + "_month_item"] = data.apply(
+            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["month"][x[config.ITEM_COLUMN_NAME], x["month"]],
+            axis=1)
+        data[encoder_name + "_quarter_store"] = data.apply(
+            lambda x: dict_map[config.STORE_COLUMN_NAME][encoder_name]["quarter"][
+                x[config.STORE_COLUMN_NAME], x["quarter"]], axis=1)
+        data[encoder_name + "_quarter_item"] = data.apply(
+            lambda x: dict_map[config.ITEM_COLUMN_NAME][encoder_name]["quarter"][
+                x[config.ITEM_COLUMN_NAME], x["quarter"]], axis=1)
+
+        data[encoder_name + "_day_store"] = data[encoder_name + "_day_store"].astype("float")
+        data[encoder_name + "_day_item"] = data[encoder_name + "_day_item"].astype("float")
+        data[encoder_name + "_month_store"] = data[encoder_name + "_month_store"].astype("float")
+        data[encoder_name + "_month_item"] = data[encoder_name + "_month_item"].astype("float")
+        data[encoder_name + "_quarter_store"] = data[encoder_name + "_quarter_store"].astype("float")
+        data[encoder_name + "_quarter_item"] = data[encoder_name + "_quarter_item"].astype("float")
+
+        return data
+
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
+    if store_col_str in data.columns:
+        data[store_col_str] = data[store_col_str].astype(np.int32)
+    if sales_col_str in data.columns:
+        data[sales_col_str] = data[sales_col_str].astype(np.float32)
+    if date_col_str in data.columns:
+        data[date_col_str] = pd.to_datetime(data[date_col_str])
+    if item_store_col_str in data.columns:
+        data[item_store_col_str] = data[item_store_col_str].astype(str)
+    return data
+
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
+    dates = []
+    start_date = datetime.strptime(start_date, '%Y-%m-%d')
+    for i in range(2):
+        start_date += timedelta(days=1)
+        if start_date.weekday() == 6:
+            start_date += timedelta(days=1)
+        dates.append(start_date)
+
+    return dates
+
+
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

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/features/cumulative_features.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/features/cumulative_features.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-import numpy as np
-from typing import List
-import pandas as pd
-from ..utils import parse_regular_data_columns
-from .. import config
-
-
-class CumulativeFeatureGenerator:
-    @classmethod
-    def filter_data_by_date(cls, df: pd.DataFrame, date_col: str, start_date: str) -> pd.DataFrame:
-        """
-        Filters the data by the start date.
-        Args:
-            df:     The dataframe to filter.
-            date_col:   The name of the date column.
-            start_date:     The start date.
-
-        Returns:
-            The filtered dataframe.
-        """
-        df = df[df[date_col] >= start_date]
-        return df
-
-    @classmethod
-    def groupby_sum_item_store(cls, df: pd.DataFrame, target_col: str, item_store_col: List[str],
-                               date_col: str) -> pd.DataFrame:
-        """
-        Groups the dataframe by item_store and date and sums the target column.
-        Args:
-            df:     The dataframe to group.
-            target_col:     The name of the target column -> sales.
-            item_store_col:     The name of the item_store column -> item_store.
-            date_col:   The name of the date column.
-
-        Returns:
-            The grouped dataframe.
-        """
-        df[target_col] = df[target_col].astype(np.float64)
-        return df.groupby(item_store_col + [date_col])[target_col].sum().reset_index()
-
-    @classmethod
-    def add_cumulative_sum_column_respect_time(cls, df: pd.DataFrame, target_col: str, item_store_col: List[str],
-                                               list_freq: List[str], date_col: str) -> pd.DataFrame:
-        """
-        This function adds cumulative sum columns to the dataframe respect to the time.
-        describe the following steps:
-        1) Group the dataframe by item_store and date and sum the target column.
-        2) Add cumulative sum columns to the dataframe respect to the time.
-        3) Merge the dataframe with the cumulative sum columns to the original dataframe.
-        4) Fill the cumulative sum columns with the previous values.
-        Args:
-            df:    The dataframe to group.
-            target_col:    The name of the target column -> sales.
-            item_store_col:   The name of the item_store column -> item_store.
-            list_freq:  The list of frequencies to calculate the cumulative sum -> ["D", "W-Mon", "M", "Y"]
-            date_col:   The name of the date column.
-
-        Returns:
-            The dataframe with the cumulative sum columns.
-
-        """
-        df[date_col] = pd.to_datetime(df[date_col])
-        item_store_col_name = '_'.join(item_store_col)
-        for freq in list_freq:
-            df_grouped = df.groupby(item_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum(
-                numeric_only=True).reset_index()
-
-            df_grouped[f"sales_cumulative_{item_store_col_name}_{freq}"] = df_grouped.groupby(item_store_col)[
-                target_col].apply(lambda x: np.cumsum(x.shift(1).fillna(0)))
-
-            df = df.merge(df_grouped.drop(columns=[target_col]), on=item_store_col + [date_col], how='left').fillna(0)
-            df = df.drop_duplicates(subset=item_store_col + [date_col], keep='last')
-        return df
-
-    @classmethod
-    def add_expected_value_column_respect_time(cls, df: pd.DataFrame, target_col: str, item_store_col: List[str],
-                                               list_freq: List[str], date_col: str) -> pd.DataFrame:
-        """
-        This function adds expected value columns to the dataframe respect to the time.
-        describe the following steps:
-        1) Group the dataframe by item_store and date and sum the target column.
-        2) Add expected value columns to the dataframe respect to the time.
-        3) Merge the dataframe with the expected value columns to the original dataframe.
-        4) Fill the expected value columns with the previous values.
-        Args:
-            df:     The dataframe to group.
-            target_col:     The name of the target column -> sales.
-            item_store_col:     The name of the item_store column -> item_store.
-            list_freq:  The list of frequencies to calculate the expected value -> ["D", "W-Mon", "M", "Y"]
-            date_col:   The name of the date column.
-
-        Returns:
-            The dataframe with the expected value columns.
-
-        """
-        item_store_col_name = '_'.join(item_store_col)
-        df_expected = pd.DataFrame()
-        df[target_col] = df[target_col].astype(np.float32)
-        for freq in list_freq:
-            df_temp = df.groupby(item_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum(
-                numeric_only=True).reset_index()
-            df_temp[f"sales_expected_{item_store_col_name}_{freq}"] = df_temp.groupby(item_store_col)[
-                target_col].transform(
-                lambda x: x.mean()).shift(1).fillna(0)
-            df_temp[f"sales_expected_{item_store_col_name}_{freq}"] = df_temp[
-                f"sales_expected_{item_store_col_name}_{freq}"].replace(
-                [np.inf, -np.inf], 0)
-            df_expected = pd.concat(
-                [df_expected, df_temp[[date_col] + item_store_col + [f"sales_expected_{item_store_col_name}_{freq}"]]])
-
-        df = pd.merge(df, df_expected, on=[date_col] + item_store_col, how='left').fillna(0)
-        df = df.drop_duplicates(subset=item_store_col + [date_col], keep='last')
-        return df
-
-    # TODO: fix item_store_col value to be unified across all project
-    @classmethod
-    def run_pipline_cumulative(cls, data_sales: pd.DataFrame, target_col: str = config.SALES_COLUMN_NAME,
-                               item_store_col: list[str, str] = config.ITEM_STORE_COLUMN_NAME_LIST,
-                               date_col: str = config.DATE_COLUMN_NAME,
-                               list_freq: list[str, str, str, str] = config.LIST_FREQ,
-                               start_date: str = config.START_DATE_CUMULATIVE_FEATURES):
-        """
-        This function runs the pipeline to create the cumulative features.
-        following steps:
-        1) Filter the data by date.
-        2) Group the data by item_store and date and sum the target column.
-        3) Add cumulative sum columns to the dataframe respect to the time.
-        4) Add expected value columns to the dataframe respect to the time.
-        5) Drop the target column.
-        6) parse the data columns
-        Args:
-            data_sales:     The dataframe to group.
-            target_col:     The name of the target column -> sales.
-            item_store_col:     The name of the item_store column -> item_store.
-            date_col:   The name of the date column.
-            list_freq:  The list of frequencies to calculate the cumulative sum and expected value -> ["D", "W-Mon", "M", "Y"]
-            start_date:     The start date to filter the data.
-
-        Returns:
-            The dataframe with the cumulative sum and expected value columns.
-        """
-
-        data_sales2 = cls.filter_data_by_date(data_sales, date_col, start_date)
-        data_sales2 = cls.groupby_sum_item_store(data_sales2, target_col, item_store_col,
-                                                 date_col)
-        data_sales2 = cls.add_cumulative_sum_column_respect_time(data_sales2,
-                                                                 target_col, item_store_col,
-                                                                 list_freq,
-                                                                 date_col)
-        data_sales2 = cls.add_expected_value_column_respect_time(data_sales2, target_col,
-                                                                 item_store_col,
-                                                                 list_freq, date_col)
-
-        data_sales2.drop(columns=[target_col], inplace=True)
-        cumulative_features = parse_regular_data_columns(data_sales2)
-        return cumulative_features
+import numpy as np
+from typing import List
+import pandas as pd
+from ..utils import parse_regular_data_columns
+from .. import config
+
+
+class CumulativeFeatureGenerator:
+    @classmethod
+    def filter_data_by_date(cls, df: pd.DataFrame, date_col: str, start_date: str) -> pd.DataFrame:
+        """
+        Filters the data by the start date.
+        Args:
+            df:     The dataframe to filter.
+            date_col:   The name of the date column.
+            start_date:     The start date.
+
+        Returns:
+            The filtered dataframe.
+        """
+        df = df[df[date_col] >= start_date]
+        return df
+
+    @classmethod
+    def groupby_sum_item_store(cls, df: pd.DataFrame, target_col: str, item_store_col: List[str],
+                               date_col: str) -> pd.DataFrame:
+        """
+        Groups the dataframe by item_store and date and sums the target column.
+        Args:
+            df:     The dataframe to group.
+            target_col:     The name of the target column -> sales.
+            item_store_col:     The name of the item_store column -> item_store.
+            date_col:   The name of the date column.
+
+        Returns:
+            The grouped dataframe.
+        """
+        df[target_col] = df[target_col].astype(np.float64)
+        return df.groupby(item_store_col + [date_col])[target_col].sum().reset_index()
+
+    @classmethod
+    def add_cumulative_sum_column_respect_time(cls, df: pd.DataFrame, target_col: str, item_store_col: List[str],
+                                               list_freq: List[str], date_col: str) -> pd.DataFrame:
+        """
+        This function adds cumulative sum columns to the dataframe respect to the time.
+        describe the following steps:
+        1) Group the dataframe by item_store and date and sum the target column.
+        2) Add cumulative sum columns to the dataframe respect to the time.
+        3) Merge the dataframe with the cumulative sum columns to the original dataframe.
+        4) Fill the cumulative sum columns with the previous values.
+        Args:
+            df:    The dataframe to group.
+            target_col:    The name of the target column -> sales.
+            item_store_col:   The name of the item_store column -> item_store.
+            list_freq:  The list of frequencies to calculate the cumulative sum -> ["D", "W-Mon", "M", "Y"]
+            date_col:   The name of the date column.
+
+        Returns:
+            The dataframe with the cumulative sum columns.
+
+        """
+        df[date_col] = pd.to_datetime(df[date_col])
+        item_store_col_name = '_'.join(item_store_col)
+        for freq in list_freq:
+            df_grouped = df.groupby(item_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum(
+                numeric_only=True).reset_index()
+
+            df_grouped[f"sales_cumulative_{item_store_col_name}_{freq}"] = df_grouped.groupby(item_store_col)[
+                target_col].apply(lambda x: np.cumsum(x.shift(1).fillna(0)))
+
+            df = df.merge(df_grouped.drop(columns=[target_col]), on=item_store_col + [date_col], how='left').fillna(0)
+            df = df.drop_duplicates(subset=item_store_col + [date_col], keep='last')
+        return df
+
+    @classmethod
+    def add_expected_value_column_respect_time(cls, df: pd.DataFrame, target_col: str, item_store_col: List[str],
+                                               list_freq: List[str], date_col: str) -> pd.DataFrame:
+        """
+        This function adds expected value columns to the dataframe respect to the time.
+        describe the following steps:
+        1) Group the dataframe by item_store and date and sum the target column.
+        2) Add expected value columns to the dataframe respect to the time.
+        3) Merge the dataframe with the expected value columns to the original dataframe.
+        4) Fill the expected value columns with the previous values.
+        Args:
+            df:     The dataframe to group.
+            target_col:     The name of the target column -> sales.
+            item_store_col:     The name of the item_store column -> item_store.
+            list_freq:  The list of frequencies to calculate the expected value -> ["D", "W-Mon", "M", "Y"]
+            date_col:   The name of the date column.
+
+        Returns:
+            The dataframe with the expected value columns.
+
+        """
+        item_store_col_name = '_'.join(item_store_col)
+        df_expected = pd.DataFrame()
+        df[target_col] = df[target_col].astype(np.float32)
+        for freq in list_freq:
+            df_temp = df.groupby(item_store_col + [pd.Grouper(key=date_col, freq=freq)])[target_col].sum(
+                numeric_only=True).reset_index()
+            df_temp[f"sales_expected_{item_store_col_name}_{freq}"] = df_temp.groupby(item_store_col)[
+                target_col].transform(
+                lambda x: x.mean()).shift(1).fillna(0)
+            df_temp[f"sales_expected_{item_store_col_name}_{freq}"] = df_temp[
+                f"sales_expected_{item_store_col_name}_{freq}"].replace(
+                [np.inf, -np.inf], 0)
+            df_expected = pd.concat(
+                [df_expected, df_temp[[date_col] + item_store_col + [f"sales_expected_{item_store_col_name}_{freq}"]]])
+
+        df = pd.merge(df, df_expected, on=[date_col] + item_store_col, how='left').fillna(0)
+        df = df.drop_duplicates(subset=item_store_col + [date_col], keep='last')
+        return df
+
+    # TODO: fix item_store_col value to be unified across all project
+    @classmethod
+    def run_pipline_cumulative(cls, data_sales: pd.DataFrame, target_col: str = config.SALES_COLUMN_NAME,
+                               item_store_col: list[str, str] = config.ITEM_STORE_COLUMN_NAME_LIST,
+                               date_col: str = config.DATE_COLUMN_NAME,
+                               list_freq: list[str, str, str, str] = config.LIST_FREQ,
+                               start_date: str = config.START_DATE_CUMULATIVE_FEATURES):
+        """
+        This function runs the pipeline to create the cumulative features.
+        following steps:
+        1) Filter the data by date.
+        2) Group the data by item_store and date and sum the target column.
+        3) Add cumulative sum columns to the dataframe respect to the time.
+        4) Add expected value columns to the dataframe respect to the time.
+        5) Drop the target column.
+        6) parse the data columns
+        Args:
+            data_sales:     The dataframe to group.
+            target_col:     The name of the target column -> sales.
+            item_store_col:     The name of the item_store column -> item_store.
+            date_col:   The name of the date column.
+            list_freq:  The list of frequencies to calculate the cumulative sum and expected value -> ["D", "W-Mon", "M", "Y"]
+            start_date:     The start date to filter the data.
+
+        Returns:
+            The dataframe with the cumulative sum and expected value columns.
+        """
+
+        data_sales2 = cls.filter_data_by_date(data_sales, date_col, start_date)
+        data_sales2 = cls.groupby_sum_item_store(data_sales2, target_col, item_store_col,
+                                                 date_col)
+        data_sales2 = cls.add_cumulative_sum_column_respect_time(data_sales2,
+                                                                 target_col, item_store_col,
+                                                                 list_freq,
+                                                                 date_col)
+        data_sales2 = cls.add_expected_value_column_respect_time(data_sales2, target_col,
+                                                                 item_store_col,
+                                                                 list_freq, date_col)
+
+        data_sales2.drop(columns=[target_col], inplace=True)
+        cumulative_features = parse_regular_data_columns(data_sales2)
+        return cumulative_features
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/features/event_features.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/features/event_features.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,152 +1,152 @@
-import pandas as pd
-
-from .. import config as global_config
-from .. import events_handler as eh
-from ..utils import next_two_days_skip_sunday, parse_regular_data_columns
-
-
-
-class EventFeaturesGenerator:
-    @classmethod
-    def apply_encoder(cls, df, encoder, columns, columns_after_apply, fillna=False):
-        if fillna:
-            df[columns_after_apply] = encoder.transform(df[columns].fillna(0))
-        else:
-            df[columns_after_apply] = encoder.transform(df[columns])
-
-        return df
-
-    @classmethod
-    def perform_encoders(cls, processed_event_features_df, event_encoders):
-        pca_dict = event_encoders[global_config.PCA_ENCODER_ARTIFACT_NAME]['pca_weights']
-        cls.apply_encoder(df=processed_event_features_df,
-                          encoder=pca_dict['pca'],
-                          columns=pca_dict['columns'],
-                          columns_after_apply=pca_dict['columns_after_apply'],
-                          fillna=True)
-
-        apply_encoding_dict = event_encoders[global_config.APPLY_ENCODINGS_DICT_ARTIFACT_NAME]
-        for key in apply_encoding_dict.keys():
-            encoder_dict = apply_encoding_dict[key]
-            cls.apply_encoder(df=processed_event_features_df,
-                              encoder=encoder_dict['encoder'],
-                              columns=encoder_dict['columns'],
-                              columns_after_apply=key)
-
-        for encoder_name in ['MEstimateEncoder', 'CatBoostEncoder']:
-            encoder_model = event_encoders[global_config.APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME][encoder_name]
-            cls.apply_encoder(df=processed_event_features_df,
-                              encoder=encoder_model['encoder'],
-                              columns=encoder_model['columns'],
-                              columns_after_apply=encoder_model['columns_after_apply']
-                              )
-
-        processed_event_features_df = eh.create_interactions_columns(processed_event_features_df)
-        for encoder_name in ['MEstimateEncoder', 'CatBoostEncoder']:
-            encoder_model = event_encoders[global_config.COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME][encoder_name]
-            cls.apply_encoder(df=processed_event_features_df,
-                              encoder=encoder_model['encoder'],
-                              columns=encoder_model['columns'],
-                              columns_after_apply=encoder_model['columns_after_apply']
-                              )
-        return processed_event_features_df
-
-    @classmethod
-    def get_future_rows(cls, regular_data_df: pd.DataFrame, begin_date: str, end_date: str):
-        """
-        Creates the future rows for prediction as a dataframe
-        Args:
-            regular_data_df: regular data dataframe
-            begin_date: begin date of prediction
-            end_date: end date of prediction
-
-        Returns:
-            dataframe with future rows
-        notes:
-        1) The names of the input columns must be the same as the global_config
-        2) for now the begin_date and end_date must be the same as the prediction date but for future it can be an iterative process
-        """
-        unique_ids = regular_data_df[global_config.ITEM_STORE_COLUMN_NAME].unique()
-
-        dfs = []
-        for date in pd.date_range(begin_date, end_date):
-            df = pd.DataFrame(
-                {global_config.ITEM_STORE_COLUMN_NAME: unique_ids, global_config.DATE_COLUMN_NAME: date})
-            df[[global_config.ITEM_COLUMN_NAME, global_config.STORE_COLUMN_NAME]] = df[
-                global_config.ITEM_STORE_COLUMN_NAME].str.split(", ", expand=True)
-            dfs.append(df)
-
-        return pd.concat(dfs)
-
-    @classmethod
-    def generate_event_features(cls, regular_data_df, event_df, holiday_df,event_encoders, begin_predict_dates):
-        """
-        Generates the event features for the future rows by the following steps:
-        1) start_date,end_date from next_two_days_skip_sunday
-        2) get_future_rows: creates the future rows for prediction as a dataframe
-        3) parse_regular_data_columns: parses the regular data columns
-        4) run_pipline_event: runs the event pipeline from the event handler
-        5) perform_encoders: performs the encoders on the event features
-        6) finalize and remove columns: finalizes the event features and removes the columns that are not needed
-        7) return the event features dataframe
-        Args:
-            regular_data_df:    regular data dataframe
-            event_df:        event dataframe
-            holiday_df:       holiday dataframe
-            event_encoders:  event encoders
-            begin_predict_dates:    begin predict dates
-
-        Returns:
-           processed_event_features_df : dataframe
-        """
-
-        start_date,end_date = next_two_days_skip_sunday(begin_predict_dates)[0]
-        end_date = next_two_days_skip_sunday(begin_predict_dates)[-1]
-        future_df = cls.get_future_rows(regular_data_df, start_date, end_date)
-        df_with2days = pd.concat([regular_data_df, future_df], ignore_index=True)
-        df_with2days = parse_regular_data_columns(df_with2days)
-        processed_event_features_df = eh.run_pipline_event(data_event=event_df, data_sales=df_with2days,
-                                                           data_hol=holiday_df)
-
-        processed_event_features_df = cls.perform_encoders(processed_event_features_df, event_encoders)
-
-        processed_event_features_df = eh.finalize_data(processed_event_features_df)
-
-        df_final_event_features = processed_event_features_df.loc[:,
-                                  ~processed_event_features_df.columns.str.contains('Unnamed')]
-
-        df_final_event_features[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
-            df_final_event_features[global_config.DATE_COLUMN_NAME])
-        df_final_event_features.set_index(global_config.DATE_COLUMN_NAME, inplace=True)
-
-        df_final_event_features.fillna(0, inplace=True)
-        df_final_event_features.reset_index(inplace=True)
-
-        processed_event_features_df = processed_event_features_df[
-            processed_event_features_df[global_config.DATE_COLUMN_NAME] == begin_predict_dates]
-        return processed_event_features_df
-
-    @classmethod
-    def generate(cls, regular_data_df, event_df, holiday_df,event_encoders, begin_predict_dates):
-        """
-        Generates the event features for the future rows by the following steps:
-        1) generate_event_features: generates the event features for the future rows
-        2) filter date and columns: filters the date and columns
-        Args:
-            regular_data_df:    regular data dataframe
-            event_df:     event dataframe
-            holiday_df:   holiday dataframe
-            event_encoders: event encoders
-            begin_predict_dates:        begin predict dates
-
-        Returns:
-            processed_event_features_df: processed event features dataframe
-
-        """
-
-        processed_event_features_df = cls.generate_event_features(regular_data_df, event_df, holiday_df,event_encoders,
-                                                                  begin_predict_dates=begin_predict_dates)
-        processed_event_features_df = processed_event_features_df[
-            processed_event_features_df[global_config.DATE_COLUMN_NAME] == begin_predict_dates]
-        processed_event_features_df.drop(columns=[global_config.SALES_COLUMN_NAME], inplace=True)
-        return processed_event_features_df
+import pandas as pd
+
+from .. import config as global_config
+from .. import events_handler as eh
+from ..utils import next_two_days_skip_sunday, parse_regular_data_columns
+
+
+
+class EventFeaturesGenerator:
+    @classmethod
+    def apply_encoder(cls, df, encoder, columns, columns_after_apply, fillna=False):
+        if fillna:
+            df[columns_after_apply] = encoder.transform(df[columns].fillna(0))
+        else:
+            df[columns_after_apply] = encoder.transform(df[columns])
+
+        return df
+
+    @classmethod
+    def perform_encoders(cls, processed_event_features_df, event_encoders):
+        pca_dict = event_encoders[global_config.PCA_ENCODER_ARTIFACT_NAME]['pca_weights']
+        cls.apply_encoder(df=processed_event_features_df,
+                          encoder=pca_dict['pca'],
+                          columns=pca_dict['columns'],
+                          columns_after_apply=pca_dict['columns_after_apply'],
+                          fillna=True)
+
+        apply_encoding_dict = event_encoders[global_config.APPLY_ENCODINGS_DICT_ARTIFACT_NAME]
+        for key in apply_encoding_dict.keys():
+            encoder_dict = apply_encoding_dict[key]
+            cls.apply_encoder(df=processed_event_features_df,
+                              encoder=encoder_dict['encoder'],
+                              columns=encoder_dict['columns'],
+                              columns_after_apply=key)
+
+        for encoder_name in ['MEstimateEncoder', 'CatBoostEncoder']:
+            encoder_model = event_encoders[global_config.APPLY_ENCODINGS_AT_ONCE_ARTIFACT_NAME][encoder_name]
+            cls.apply_encoder(df=processed_event_features_df,
+                              encoder=encoder_model['encoder'],
+                              columns=encoder_model['columns'],
+                              columns_after_apply=encoder_model['columns_after_apply']
+                              )
+
+        processed_event_features_df = eh.create_interactions_columns(processed_event_features_df)
+        for encoder_name in ['MEstimateEncoder', 'CatBoostEncoder']:
+            encoder_model = event_encoders[global_config.COLUMNS_INTERACTIONS_ENCODER_ARTIFACT_NAME][encoder_name]
+            cls.apply_encoder(df=processed_event_features_df,
+                              encoder=encoder_model['encoder'],
+                              columns=encoder_model['columns'],
+                              columns_after_apply=encoder_model['columns_after_apply']
+                              )
+        return processed_event_features_df
+
+    @classmethod
+    def get_future_rows(cls, regular_data_df: pd.DataFrame, begin_date: str, end_date: str):
+        """
+        Creates the future rows for prediction as a dataframe
+        Args:
+            regular_data_df: regular data dataframe
+            begin_date: begin date of prediction
+            end_date: end date of prediction
+
+        Returns:
+            dataframe with future rows
+        notes:
+        1) The names of the input columns must be the same as the global_config
+        2) for now the begin_date and end_date must be the same as the prediction date but for future it can be an iterative process
+        """
+        unique_ids = regular_data_df[global_config.ITEM_STORE_COLUMN_NAME].unique()
+
+        dfs = []
+        for date in pd.date_range(begin_date, end_date):
+            df = pd.DataFrame(
+                {global_config.ITEM_STORE_COLUMN_NAME: unique_ids, global_config.DATE_COLUMN_NAME: date})
+            df[[global_config.ITEM_COLUMN_NAME, global_config.STORE_COLUMN_NAME]] = df[
+                global_config.ITEM_STORE_COLUMN_NAME].str.split(", ", expand=True)
+            dfs.append(df)
+
+        return pd.concat(dfs)
+
+    @classmethod
+    def generate_event_features(cls, regular_data_df, event_df, holiday_df,event_encoders, begin_predict_dates):
+        """
+        Generates the event features for the future rows by the following steps:
+        1) start_date,end_date from next_two_days_skip_sunday
+        2) get_future_rows: creates the future rows for prediction as a dataframe
+        3) parse_regular_data_columns: parses the regular data columns
+        4) run_pipline_event: runs the event pipeline from the event handler
+        5) perform_encoders: performs the encoders on the event features
+        6) finalize and remove columns: finalizes the event features and removes the columns that are not needed
+        7) return the event features dataframe
+        Args:
+            regular_data_df:    regular data dataframe
+            event_df:        event dataframe
+            holiday_df:       holiday dataframe
+            event_encoders:  event encoders
+            begin_predict_dates:    begin predict dates
+
+        Returns:
+           processed_event_features_df : dataframe
+        """
+
+        start_date,end_date = next_two_days_skip_sunday(begin_predict_dates)[0]
+        end_date = next_two_days_skip_sunday(begin_predict_dates)[-1]
+        future_df = cls.get_future_rows(regular_data_df, start_date, end_date)
+        df_with2days = pd.concat([regular_data_df, future_df], ignore_index=True)
+        df_with2days = parse_regular_data_columns(df_with2days)
+        processed_event_features_df = eh.run_pipline_event(data_event=event_df, data_sales=df_with2days,
+                                                           data_hol=holiday_df)
+
+        processed_event_features_df = cls.perform_encoders(processed_event_features_df, event_encoders)
+
+        processed_event_features_df = eh.finalize_data(processed_event_features_df)
+
+        df_final_event_features = processed_event_features_df.loc[:,
+                                  ~processed_event_features_df.columns.str.contains('Unnamed')]
+
+        df_final_event_features[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
+            df_final_event_features[global_config.DATE_COLUMN_NAME])
+        df_final_event_features.set_index(global_config.DATE_COLUMN_NAME, inplace=True)
+
+        df_final_event_features.fillna(0, inplace=True)
+        df_final_event_features.reset_index(inplace=True)
+
+        processed_event_features_df = processed_event_features_df[
+            processed_event_features_df[global_config.DATE_COLUMN_NAME] == begin_predict_dates]
+        return processed_event_features_df
+
+    @classmethod
+    def generate(cls, regular_data_df, event_df, holiday_df,event_encoders, begin_predict_dates):
+        """
+        Generates the event features for the future rows by the following steps:
+        1) generate_event_features: generates the event features for the future rows
+        2) filter date and columns: filters the date and columns
+        Args:
+            regular_data_df:    regular data dataframe
+            event_df:     event dataframe
+            holiday_df:   holiday dataframe
+            event_encoders: event encoders
+            begin_predict_dates:        begin predict dates
+
+        Returns:
+            processed_event_features_df: processed event features dataframe
+
+        """
+
+        processed_event_features_df = cls.generate_event_features(regular_data_df, event_df, holiday_df,event_encoders,
+                                                                  begin_predict_dates=begin_predict_dates)
+        processed_event_features_df = processed_event_features_df[
+            processed_event_features_df[global_config.DATE_COLUMN_NAME] == begin_predict_dates]
+        processed_event_features_df.drop(columns=[global_config.SALES_COLUMN_NAME], inplace=True)
+        return processed_event_features_df
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/features/future_features.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/features/future_features.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-import pandas as pd
-from .. import config as global_config
-from . import config
-from ..utils import process_date_column, add_values_to_dict_mapper, map_encoders_columns_to_base_df
-
-def clean_marketing(marketing_plan_df: pd.DataFrame) -> pd.DataFrame:
-    """
-    Clean marketing plan df from unnecessary columns and convert columns to int32
-    Args:
-        marketing_plan_df:
-
-    Returns:
-
-    """
-    marketing_plan_df = marketing_plan_df.loc[:,
-                        ~marketing_plan_df.columns.str.contains('Unnamed')]
-    marketing_plan_df = marketing_plan_df.dropna()
-
-    cols_to_convert = marketing_plan_df.columns.difference(['date'])
-    marketing_plan_df[cols_to_convert] = marketing_plan_df[cols_to_convert].astype('int32')
-
-    return marketing_plan_df
-
-
-def clean_item_encoder(item_encoders):
-    """
-    Clean item encoder df from unnecessary columns and convert columns to int64
-    Args:
-        item_encoders:  item encoder df
-
-    Returns:
-        item_encoders
-    """
-    item_encoders = item_encoders.drop('Unnamed: 0', axis=1)
-    item_encoders[global_config.ITEM_COLUMN_NAME] = item_encoders[global_config.ITEM_COLUMN_NAME].astype('int64')
-    item_encoders = item_encoders.set_index(global_config.ITEM_COLUMN_NAME)
-    item_encoders = item_encoders.astype('float')
-    return item_encoders
-
-
-def clean_store_encoder(store_encoders):
-    """
-    Clean store encoder df from unnecessary columns and convert columns to int32
-    Args:
-        store_encoders:     store encoder df
-
-    Returns:
-        store_encoders
-    """
-    store_encoders = store_encoders.drop('Unnamed: 0', axis=1)
-    store_encoders[global_config.STORE_COLUMN_NAME] = store_encoders[global_config.STORE_COLUMN_NAME].astype(
-        'int32')
-    store_encoders = store_encoders.set_index(global_config.STORE_COLUMN_NAME)
-    store_encoders = store_encoders.astype('float')
-    return store_encoders
-
-
-class FarFutureFeaturesGenerator:
-
-    @classmethod
-    def far_future_features_preprocess_of_store(cls, marketing_plan: pd.DataFrame, item_encoders , store_encoders, store_batch,
-                                                begin_predict_dates: str) -> pd.DataFrame:
-        """
-        Preprocess of store for far future features generation
-        following the steps:
-        1) clean marketing plan df
-        2) clean item encoder df
-        3) clean store encoder df
-        4) add values to dict mapper
-        5) create future date range
-        6) create future features df
-        7) create future features df with store batch
-        8) create future features df with store batch and begin predict dates
-        9) create future features df with store batch and begin predict dates and marketing plan
-        10) create future features df with store batch and begin predict dates and marketing plan and item encoders
-        Args:
-            marketing_plan:     marketing plan df
-            item_encoders:    item encoder df
-            store_encoders:     store encoder df
-            store_batch:    store batch
-            begin_predict_dates:    begin predict dates
-
-        Returns:
-            output_df : future features df with store batch and begin predict dates and marketing plan and item encoders
-        """
-        marketing_plan = clean_marketing(marketing_plan)
-        item_encoders = clean_item_encoder(item_encoders)
-        store_encoders = clean_store_encoder(store_encoders)
-
-        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, item_encoders, global_config.ITEM_COLUMN_NAME,
-                                                config.ENCODERS_NAME,
-                                                config.DICT_OF_TIME_INTERVAL)
-
-        dict_mapper = add_values_to_dict_mapper(dict_mapper, store_encoders, global_config.STORE_COLUMN_NAME,
-                                                config.ENCODERS_NAME,
-                                                config.DICT_OF_TIME_INTERVAL)
-
-        future_date_range = pd.date_range(start=begin_predict_dates, end=begin_predict_dates, freq='D')
-
-        output_df = pd.DataFrame()
-        for _id in store_batch:
-            item_store_id = _id
-            item = int(item_store_id.split(',')[0])
-            store = int(item_store_id.split(',')[1])
-            id_data_future = pd.DataFrame({'date': future_date_range,
-                                           'item, store': item_store_id,
-                                           'item': item,
-                                           'store': store})
-
-            id_data_future = process_date_column(id_data_future, global_config.DATE_COLUMN_NAME, expanded=True)
-
-            # Exclude Sunday
-            # id_data_future = id_data_future[id_data_future['day_of_week'] != 6]
-
-            marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
-                marketing_plan[global_config.DATE_COLUMN_NAME])
-
-            id_data_future = pd.merge(id_data_future, marketing_plan, on=[global_config.DATE_COLUMN_NAME], how='left')
-
-            id_data_future = map_encoders_columns_to_base_df(id_data_future, dict_mapper, config.ENCODERS_NAME)
-            output_df = pd.concat([output_df, id_data_future])
-
-        # output_df.drop('name_of_day', axis=1, inplace=True)
-        return output_df
-
-    @classmethod
-    def far_future_features_preprocess_of_several_stores(cls, marketing_plan: pd.DataFrame, item_encoders, store_encoders, store_batch_dict, begin_predict_dates: str) -> pd.DataFrame:
-        """
-        Preprocess of store for far future features generation
-        following the steps:
-        1) clean marketing plan df
-        2) clean item encoder df
-        3) clean store encoder df
-        4) add values to dict mapper
-        5) create future date range
-        6) create future features df
-        7) create future features df with store batch
-        8) create future features df with store batch and begin predict dates
-        9) create future features df with store batch and begin predict dates and marketing plan
-        10) create future features df with store batch and begin predict dates and marketing plan and item encoders
-        Args:
-            marketing_plan:     marketing plan df
-            item_encoders:    item encoder df
-            store_encoders:     store encoder df
-            store_batch:    store batch
-            begin_predict_dates:    begin predict dates
-
-        Returns:
-            output_df : future features df with store batch and begin predict dates and marketing plan and item encoders
-        """
-
-        marketing_plan = clean_marketing(marketing_plan)
-        item_encoders = clean_item_encoder(item_encoders)
-        store_encoders = clean_store_encoder(store_encoders)
-
-        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, item_encoders, global_config.ITEM_COLUMN_NAME,
-                                                config.ENCODERS_NAME,
-                                                config.DICT_OF_TIME_INTERVAL)
-
-        dict_mapper = add_values_to_dict_mapper(dict_mapper, store_encoders, global_config.STORE_COLUMN_NAME,
-                                                config.ENCODERS_NAME,
-                                                config.DICT_OF_TIME_INTERVAL)
-
-        future_date_range = pd.date_range(start=begin_predict_dates, end=begin_predict_dates, freq='D')
-
-        output_dfs = {}
-        for store_id in list(store_batch_dict.keys()):
-            output_df = pd.DataFrame()
-            for _id in store_batch_dict[store_id]:
-                item_store_id = _id
-                item = int(item_store_id.split(',')[0])
-                store = int(item_store_id.split(',')[1])
-                id_data_future = pd.DataFrame({'date': future_date_range,
-                                               'item, store': item_store_id,
-                                               'item': item,
-                                               'store': store})
-                id_data_future = process_date_column(id_data_future, global_config.DATE_COLUMN_NAME, expanded=True)
-
-                # Exclude Sunday
-                # id_data_future = id_data_future[id_data_future['day_of_week'] != 6]
-
-                marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
-                    marketing_plan[global_config.DATE_COLUMN_NAME])
-                id_data_future = pd.merge(id_data_future, marketing_plan, on=[global_config.DATE_COLUMN_NAME],
-                                          how='left')
-                id_data_future = map_encoders_columns_to_base_df(id_data_future, dict_mapper, config.ENCODERS_NAME)
-                output_df = pd.concat([output_df, id_data_future])
-
-            # output_df.drop('name_of_day', axis=1, inplace=True)
-            output_dfs[store_id] = output_df
-        return output_dfs
+import pandas as pd
+from .. import config as global_config
+from . import config
+from ..utils import process_date_column, add_values_to_dict_mapper, map_encoders_columns_to_base_df
+
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
+
+
+class FarFutureFeaturesGenerator:
+
+    @classmethod
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
+
+        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, item_encoders, global_config.ITEM_COLUMN_NAME,
+                                                config.ENCODERS_NAME,
+                                                config.DICT_OF_TIME_INTERVAL)
+
+        dict_mapper = add_values_to_dict_mapper(dict_mapper, store_encoders, global_config.STORE_COLUMN_NAME,
+                                                config.ENCODERS_NAME,
+                                                config.DICT_OF_TIME_INTERVAL)
+
+        future_date_range = pd.date_range(start=begin_predict_dates, end=begin_predict_dates, freq='D')
+
+        output_df = pd.DataFrame()
+        for _id in store_batch:
+            item_store_id = _id
+            item = int(item_store_id.split(',')[0])
+            store = int(item_store_id.split(',')[1])
+            id_data_future = pd.DataFrame({'date': future_date_range,
+                                           'item, store': item_store_id,
+                                           'item': item,
+                                           'store': store})
+
+            id_data_future = process_date_column(id_data_future, global_config.DATE_COLUMN_NAME, expanded=True)
+
+            # Exclude Sunday
+            # id_data_future = id_data_future[id_data_future['day_of_week'] != 6]
+
+            marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
+                marketing_plan[global_config.DATE_COLUMN_NAME])
+
+            id_data_future = pd.merge(id_data_future, marketing_plan, on=[global_config.DATE_COLUMN_NAME], how='left')
+
+            id_data_future = map_encoders_columns_to_base_df(id_data_future, dict_mapper, config.ENCODERS_NAME)
+            output_df = pd.concat([output_df, id_data_future])
+
+        # output_df.drop('name_of_day', axis=1, inplace=True)
+        return output_df
+
+    @classmethod
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
+
+        dict_mapper = add_values_to_dict_mapper(config.DICT_MAPPER, item_encoders, global_config.ITEM_COLUMN_NAME,
+                                                config.ENCODERS_NAME,
+                                                config.DICT_OF_TIME_INTERVAL)
+
+        dict_mapper = add_values_to_dict_mapper(dict_mapper, store_encoders, global_config.STORE_COLUMN_NAME,
+                                                config.ENCODERS_NAME,
+                                                config.DICT_OF_TIME_INTERVAL)
+
+        future_date_range = pd.date_range(start=begin_predict_dates, end=begin_predict_dates, freq='D')
+
+        output_dfs = {}
+        for store_id in list(store_batch_dict.keys()):
+            output_df = pd.DataFrame()
+            for _id in store_batch_dict[store_id]:
+                item_store_id = _id
+                item = int(item_store_id.split(',')[0])
+                store = int(item_store_id.split(',')[1])
+                id_data_future = pd.DataFrame({'date': future_date_range,
+                                               'item, store': item_store_id,
+                                               'item': item,
+                                               'store': store})
+                id_data_future = process_date_column(id_data_future, global_config.DATE_COLUMN_NAME, expanded=True)
+
+                # Exclude Sunday
+                # id_data_future = id_data_future[id_data_future['day_of_week'] != 6]
+
+                marketing_plan[global_config.DATE_COLUMN_NAME] = pd.to_datetime(
+                    marketing_plan[global_config.DATE_COLUMN_NAME])
+                id_data_future = pd.merge(id_data_future, marketing_plan, on=[global_config.DATE_COLUMN_NAME],
+                                          how='left')
+                id_data_future = map_encoders_columns_to_base_df(id_data_future, dict_mapper, config.ENCODERS_NAME)
+                output_df = pd.concat([output_df, id_data_future])
+
+            # output_df.drop('name_of_day', axis=1, inplace=True)
+            output_dfs[store_id] = output_df
+        return output_dfs
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/features/lags_features.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/features/lags_features.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,124 +1,124 @@
-import numpy as np
-import pandas as pd
-
-from .. import config as global_config
-from . import config as config
-
-store_col_str = global_config.STORE_COLUMN_NAME
-item_col_str = global_config.ITEM_COLUMN_NAME
-date_col_str = global_config.DATE_COLUMN_NAME
-sales_col_str = global_config.SALES_COLUMN_NAME
-id_col_str = global_config.ID_COLUMN_NAME
-item_store_col_str = global_config.ITEM_STORE_COLUMN_NAME
-
-
-class LagFeatureGenerator:
-    def __init__(self, daily_lags_back=config.DAILY_LAGS_BACK,
-                 daily_windows=config.DAILY_WINDOWS,
-                 daily_diff_lags=config.DAILY_DIFF_LAGS,
-                 daily_ewms=config.DAILY_EWMS):
-        self.daily_lags_back = daily_lags_back
-        self.daily_windows = daily_windows
-        self.daily_diff_lags = daily_diff_lags
-        self.daily_ewms = daily_ewms
-
-    def add_lags_and_rolling_averages_and_diffs_and_ewms(self, df: pd.DataFrame, base_column_name: str):
-        """
-        This function creates lags, rolling averages, diffs and ewms for a given column
-        Args:
-            df: dataframe
-            base_column_name: column name to create lags, rolling averages, diffs and ewms for
-
-        Returns:
-            dataframe with lags, rolling averages, diffs and ewms for a given column
-        """
-        for lag in self.daily_lags_back:
-            df[f'{base_column_name}_sales_lag_{lag}'] = df[sales_col_str].shift(lag)
-        for window in self.daily_windows:
-            df[f'{base_column_name}_sales_rolling_{window}'] = df[sales_col_str].shift(1).rolling(window).mean()
-        for diff_lag in self.daily_diff_lags:
-            df[f'{base_column_name}_sales_diff_{diff_lag}'] = df[sales_col_str].shift(1) - df[sales_col_str].shift(
-                diff_lag)
-        for ewm in self.daily_ewms:
-            df[f'{base_column_name}_sales_ewm_{ewm}'] = df[sales_col_str].shift(1).ewm(alpha=ewm).mean()
-        return df
-
-
-class StoreLagFeatureGenerator(LagFeatureGenerator):
-    def __init__(self):
-        super().__init__()
-
-    def create_all_stores_lags(self, store_data_df: pd.DataFrame, predict_date: str):
-        """
-        This function creates groupby by date and sum of sales for all stores
-        and then creates lags, rolling averages, diffs and ewms for the sum of sales
-        Args:
-            store_data_df: dataframe with store data
-            predict_date: date to filter the dataframe
-
-        Returns:
-            dataframe with lags, rolling averages, diffs and ewms for the sum of sales
-        """
-        store_df = store_data_df.groupby(date_col_str).sum(numeric_only=True).reset_index()[
-            [date_col_str, sales_col_str]]
-        store_df = store_df.set_index(date_col_str)
-        store_df = self.add_lags_and_rolling_averages_and_diffs_and_ewms(df=store_df[[sales_col_str]],
-                                                                         base_column_name=store_col_str)
-        store_df = store_df.drop(columns=[sales_col_str]).reset_index()
-        store_df = store_df[store_df[date_col_str] == pd.to_datetime(predict_date)]
-
-        return store_df
-
-
-class ItemLagFeatureGenerator(LagFeatureGenerator):
-    def __init__(self):
-        super().__init__()
-
-    def create_all_item_lags(self, regular_data_df: str, predict_date: str):
-        """
-        This function creates groupby by date and sum of sales for all items and then creates lags, rolling averages,
-        diffs and ewms for the sum of sales for each item
-        Args:
-            regular_data_df: dataframe with regular data
-            predict_date: date to filter the dataframe
-
-        Returns:
-            dataframe with lags, rolling averages, diffs and ewms for the sum of sales for each item
-        """
-        all_item_lags = pd.DataFrame()
-        for item in regular_data_df[item_col_str].unique():
-            item_data = regular_data_df[regular_data_df[item_col_str] == item].groupby(date_col_str).sum(
-                numeric_only=True).reset_index()[
-                [date_col_str, sales_col_str]]
-            item_data = item_data.set_index(date_col_str)
-            item_data = self.add_lags_and_rolling_averages_and_diffs_and_ewms(item_data[[sales_col_str]], item_col_str)
-            item_data = item_data.drop(columns=[sales_col_str]).reset_index()
-            item_data[item_col_str] = np.int64(item)
-            all_item_lags = pd.concat([all_item_lags, item_data], ignore_index=True)
-        all_item_lags = all_item_lags[all_item_lags[date_col_str] == pd.to_datetime(predict_date)]
-        return all_item_lags
-
-
-class IDLagFeatureGenerator(LagFeatureGenerator):
-    def __init__(self):
-        super().__init__()
-
-    def create_id_lags(self, id_data_df: pd.DataFrame, item, store, predict_date: str):
-        """
-        This function creates lags, rolling averages, diffs and ewms for a given item and store
-        Args:
-            id_data_df:     dataframe with data for a given item and store
-            item:        item id
-            store:     store id
-            predict_date:   date to filter the dataframe
-
-        Returns:
-            dataframe with lags, rolling averages, diffs and ewms for a given item and store
-
-        """
-        id_data_df = self.add_lags_and_rolling_averages_and_diffs_and_ewms(
-            id_data_df.set_index(date_col_str)[[sales_col_str]], id_col_str).reset_index()
-        id_data_df[item_col_str] = np.int64(item)
-        id_data_df[store_col_str] = np.int32(store)
-        id_data_df = id_data_df[id_data_df[date_col_str] == pd.to_datetime(predict_date)]
-        return id_data_df
+import numpy as np
+import pandas as pd
+
+from .. import config as global_config
+from . import config as config
+
+store_col_str = global_config.STORE_COLUMN_NAME
+item_col_str = global_config.ITEM_COLUMN_NAME
+date_col_str = global_config.DATE_COLUMN_NAME
+sales_col_str = global_config.SALES_COLUMN_NAME
+id_col_str = global_config.ID_COLUMN_NAME
+item_store_col_str = global_config.ITEM_STORE_COLUMN_NAME
+
+
+class LagFeatureGenerator:
+    def __init__(self, daily_lags_back=config.DAILY_LAGS_BACK,
+                 daily_windows=config.DAILY_WINDOWS,
+                 daily_diff_lags=config.DAILY_DIFF_LAGS,
+                 daily_ewms=config.DAILY_EWMS):
+        self.daily_lags_back = daily_lags_back
+        self.daily_windows = daily_windows
+        self.daily_diff_lags = daily_diff_lags
+        self.daily_ewms = daily_ewms
+
+    def add_lags_and_rolling_averages_and_diffs_and_ewms(self, df: pd.DataFrame, base_column_name: str):
+        """
+        This function creates lags, rolling averages, diffs and ewms for a given column
+        Args:
+            df: dataframe
+            base_column_name: column name to create lags, rolling averages, diffs and ewms for
+
+        Returns:
+            dataframe with lags, rolling averages, diffs and ewms for a given column
+        """
+        for lag in self.daily_lags_back:
+            df[f'{base_column_name}_sales_lag_{lag}'] = df[sales_col_str].shift(lag)
+        for window in self.daily_windows:
+            df[f'{base_column_name}_sales_rolling_{window}'] = df[sales_col_str].shift(1).rolling(window).mean()
+        for diff_lag in self.daily_diff_lags:
+            df[f'{base_column_name}_sales_diff_{diff_lag}'] = df[sales_col_str].shift(1) - df[sales_col_str].shift(
+                diff_lag)
+        for ewm in self.daily_ewms:
+            df[f'{base_column_name}_sales_ewm_{ewm}'] = df[sales_col_str].shift(1).ewm(alpha=ewm).mean()
+        return df
+
+
+class StoreLagFeatureGenerator(LagFeatureGenerator):
+    def __init__(self):
+        super().__init__()
+
+    def create_all_stores_lags(self, store_data_df: pd.DataFrame, predict_date: str):
+        """
+        This function creates groupby by date and sum of sales for all stores
+        and then creates lags, rolling averages, diffs and ewms for the sum of sales
+        Args:
+            store_data_df: dataframe with store data
+            predict_date: date to filter the dataframe
+
+        Returns:
+            dataframe with lags, rolling averages, diffs and ewms for the sum of sales
+        """
+        store_df = store_data_df.groupby(date_col_str).sum(numeric_only=True).reset_index()[
+            [date_col_str, sales_col_str]]
+        store_df = store_df.set_index(date_col_str)
+        store_df = self.add_lags_and_rolling_averages_and_diffs_and_ewms(df=store_df[[sales_col_str]],
+                                                                         base_column_name=store_col_str)
+        store_df = store_df.drop(columns=[sales_col_str]).reset_index()
+        store_df = store_df[store_df[date_col_str] == pd.to_datetime(predict_date)]
+
+        return store_df
+
+
+class ItemLagFeatureGenerator(LagFeatureGenerator):
+    def __init__(self):
+        super().__init__()
+
+    def create_all_item_lags(self, regular_data_df: str, predict_date: str):
+        """
+        This function creates groupby by date and sum of sales for all items and then creates lags, rolling averages,
+        diffs and ewms for the sum of sales for each item
+        Args:
+            regular_data_df: dataframe with regular data
+            predict_date: date to filter the dataframe
+
+        Returns:
+            dataframe with lags, rolling averages, diffs and ewms for the sum of sales for each item
+        """
+        all_item_lags = pd.DataFrame()
+        for item in regular_data_df[item_col_str].unique():
+            item_data = regular_data_df[regular_data_df[item_col_str] == item].groupby(date_col_str).sum(
+                numeric_only=True).reset_index()[
+                [date_col_str, sales_col_str]]
+            item_data = item_data.set_index(date_col_str)
+            item_data = self.add_lags_and_rolling_averages_and_diffs_and_ewms(item_data[[sales_col_str]], item_col_str)
+            item_data = item_data.drop(columns=[sales_col_str]).reset_index()
+            item_data[item_col_str] = np.int64(item)
+            all_item_lags = pd.concat([all_item_lags, item_data], ignore_index=True)
+        all_item_lags = all_item_lags[all_item_lags[date_col_str] == pd.to_datetime(predict_date)]
+        return all_item_lags
+
+
+class IDLagFeatureGenerator(LagFeatureGenerator):
+    def __init__(self):
+        super().__init__()
+
+    def create_id_lags(self, id_data_df: pd.DataFrame, item, store, predict_date: str):
+        """
+        This function creates lags, rolling averages, diffs and ewms for a given item and store
+        Args:
+            id_data_df:     dataframe with data for a given item and store
+            item:        item id
+            store:     store id
+            predict_date:   date to filter the dataframe
+
+        Returns:
+            dataframe with lags, rolling averages, diffs and ewms for a given item and store
+
+        """
+        id_data_df = self.add_lags_and_rolling_averages_and_diffs_and_ewms(
+            id_data_df.set_index(date_col_str)[[sales_col_str]], id_col_str).reset_index()
+        id_data_df[item_col_str] = np.int64(item)
+        id_data_df[store_col_str] = np.int32(store)
+        id_data_df = id_data_df[id_data_df[date_col_str] == pd.to_datetime(predict_date)]
+        return id_data_df
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/features/weather_features.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/features/weather_features.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,153 +1,153 @@
-import pandas as pd
-from ..clearml_data_handler import DatasetLoader
-from .. import config as global_config
-from . import config as config
-
-import pandas as pd
-from meteostat import Point, Daily
-from datetime import datetime
-
-
-# class StoreLocationLoader:
-#
-#     @classmethod
-#     def load(cls, dataset_project=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_project'],
-#              dataset_name=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_name'],
-#              dataset_version=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_version'],
-#              dataset_tags=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_tags'],
-#              dataset_file_name=global_config.DEFAULT_STORE_LOCATION_DATASET['dataset_file_name']
-#              ):
-#         store_location_dfs = DatasetLoader().load_dfs_from_dataset(dataset_project=dataset_project,
-#                                                                    dataset_name=dataset_name,
-#                                                                    dataset_version=dataset_version,
-#                                                                    dataset_tags=dataset_tags,
-#                                                                    dataset_file_names=[dataset_file_name])
-#         store_location_df = store_location_dfs[dataset_file_name]
-#         store_location_df = store_location_df.drop('Unnamed: 0', axis=1)
-#
-#         return store_location_df
-
-
-class WeatherFeatureGenerator:
-    @classmethod
-    def load(cls, store_location_df, store_id, start_date, end_date, weather_columns=config.WEATHER_COLUMNS):
-        """
-        Load weather data for specific store
-        Args:
-            store_location_df:  store location dataframe
-            store_id:         store id
-            start_date:     start date
-            end_date:    end date
-            weather_columns:    weather columns
-
-        Returns:
-            dataframe: dataframe with weather data for specific store
-        """
-        store_weather_df = cls.return_df_of_stores_weather(stores_location_df=store_location_df,
-                                                          store_id=store_id,
-                                                          start_date_str=start_date,
-                                                          end_date_str=end_date,
-                                                          weather_columns=weather_columns)
-
-        return store_weather_df
-
-    @classmethod
-    def return_weather_daily_data_for_specific_location(cls, start_date, end_date, latitude, longitude):
-        """
-        Return weather data for specific location and time period
-        Args:
-            start_date:     start date
-            end_date:   end date
-            latitude:   latitude
-            longitude:  longitude
-
-        Returns:
-            dataframe: dataframe with weather data for specific location and time period
-        """
-        start = datetime.strptime(start_date, '%Y-%m-%d')
-        end = datetime.strptime(end_date, '%Y-%m-%d')
-        vienna = Point(float(latitude), float(longitude))
-        data = Daily(vienna, start, end)
-        data = data.fetch()
-        if "tavg" in data.columns:
-            data['tavg'].interpolate(method='linear', limit_area='outside', inplace=True)
-        if "tmin" in data.columns:
-            data['tmin'].interpolate(method='linear', limit_area='outside', inplace=True)
-        if "tmax" in data.columns:
-            data['tmax'].interpolate(method='linear', limit_area='outside', inplace=True)
-        if 'pres' in data.columns:
-            data['pres'].interpolate(method='linear', limit_area='outside', inplace=True)
-        if 'prcp' in data.columns:
-            data['prcp'].fillna(0, inplace=True)
-        if 'snow' in data.columns:
-            data['snow'].fillna(0, inplace=True)
-        if 'wspd' in data.columns:
-            data['wspd'].fillna(0, inplace=True)
-        if data['pres'].isnull().values.any():
-            data["pres"] = 0
-        data.interpolate('linear', inplace=True)
-        return data
-
-    @classmethod
-    def return_df_of_stores_weather(cls, stores_location_df, store_id, start_date_str, end_date_str, weather_columns,
-                                    lat_vienna=48.2082,
-                                    lon_vienna=16.3738):
-        """
-        Return weather data for specific store and time period and if not available for vienna
-        Args:
-            stores_location_df:     store location dataframe
-            store_id:   store id
-            start_date_str:     start date
-            end_date_str:   end date
-            weather_columns:    weather columns
-            lat_vienna:     latitude_vienna
-            lon_vienna:     longitude_vienna
-
-        Returns:
-            dataframe: dataframe with weather data for specific store and time period and if not available for vienna
-        """
-
-        start_date = datetime.strptime(start_date_str, "%Y-%m-%d").date()
-        end_date = datetime.strptime(end_date_str, "%Y-%m-%d").date()
-        delta = end_date - start_date
-
-        stores_location_df['store_id'] = stores_location_df['store_id'].astype(int)
-
-        store_location = stores_location_df[stores_location_df['store_id'] == store_id]
-        latitude = store_location['latitude'].values[0]
-        longitude = store_location['longitude'].values[0]
-        df_weather_of_store = \
-            cls.return_weather_daily_data_for_specific_location(start_date_str,end_date_str, latitude,longitude)[weather_columns]
-        if (len(df_weather_of_store) < delta.days) or (df_weather_of_store.isna().sum().sum() > 0) or len(
-                df_weather_of_store) == 0:
-            df_weather_of_store = \
-                cls.return_weather_daily_data_for_specific_location(start_date_str,
-                                                                    end_date_str, lat_vienna,
-                                                                    lon_vienna)[
-                    weather_columns]
-
-        df_weather_of_store['store'] = store_id
-        df_weather_of_store['store'] = df_weather_of_store['store'].astype(int)
-
-
-        return df_weather_of_store.reset_index().rename(columns={"index": "date", "time": "date"})
-
-    @classmethod
-    def generate(cls, store_location_df, store_id, start_predict_date, end_predict_date, weather_columns=config.WEATHER_COLUMNS):
-        """
-        Generate weather data for specific store and time period
-        Args:
-            store_location_df:      store location dataframe
-            store_id:     store id
-            start_predict_date:     start date
-            end_predict_date:   end date
-            weather_columns:    weather columns
-
-        Returns:
-            dataframe: dataframe with weather data for specific store and time period
-        """
-        # store_location_df = StoreLocationLoader.load()
-        store_weather_df = cls.load(store_location_df=store_location_df, store_id=store_id, start_date=start_predict_date, end_date=end_predict_date, weather_columns=weather_columns)
-        return store_weather_df
-
-
+import pandas as pd
+from ..clearml_data_handler import DatasetLoader
+from .. import config as global_config
+from . import config as config
+
+import pandas as pd
+from meteostat import Point, Daily
+from datetime import datetime
+
+
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
+
+
+class WeatherFeatureGenerator:
+    @classmethod
+    def load(cls, store_location_df, store_id, start_date, end_date, weather_columns=config.WEATHER_COLUMNS):
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
+        store_weather_df = cls.return_df_of_stores_weather(stores_location_df=store_location_df,
+                                                          store_id=store_id,
+                                                          start_date_str=start_date,
+                                                          end_date_str=end_date,
+                                                          weather_columns=weather_columns)
+
+        return store_weather_df
+
+    @classmethod
+    def return_weather_daily_data_for_specific_location(cls, start_date, end_date, latitude, longitude):
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
+        start = datetime.strptime(start_date, '%Y-%m-%d')
+        end = datetime.strptime(end_date, '%Y-%m-%d')
+        vienna = Point(float(latitude), float(longitude))
+        data = Daily(vienna, start, end)
+        data = data.fetch()
+        if "tavg" in data.columns:
+            data['tavg'].interpolate(method='linear', limit_area='outside', inplace=True)
+        if "tmin" in data.columns:
+            data['tmin'].interpolate(method='linear', limit_area='outside', inplace=True)
+        if "tmax" in data.columns:
+            data['tmax'].interpolate(method='linear', limit_area='outside', inplace=True)
+        if 'pres' in data.columns:
+            data['pres'].interpolate(method='linear', limit_area='outside', inplace=True)
+        if 'prcp' in data.columns:
+            data['prcp'].fillna(0, inplace=True)
+        if 'snow' in data.columns:
+            data['snow'].fillna(0, inplace=True)
+        if 'wspd' in data.columns:
+            data['wspd'].fillna(0, inplace=True)
+        if data['pres'].isnull().values.any():
+            data["pres"] = 0
+        data.interpolate('linear', inplace=True)
+        return data
+
+    @classmethod
+    def return_df_of_stores_weather(cls, stores_location_df, store_id, start_date_str, end_date_str, weather_columns,
+                                    lat_vienna=48.2082,
+                                    lon_vienna=16.3738):
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
+
+        start_date = datetime.strptime(start_date_str, "%Y-%m-%d").date()
+        end_date = datetime.strptime(end_date_str, "%Y-%m-%d").date()
+        delta = end_date - start_date
+
+        stores_location_df['store_id'] = stores_location_df['store_id'].astype(int)
+
+        store_location = stores_location_df[stores_location_df['store_id'] == store_id]
+        latitude = store_location['latitude'].values[0]
+        longitude = store_location['longitude'].values[0]
+        df_weather_of_store = \
+            cls.return_weather_daily_data_for_specific_location(start_date_str,end_date_str, latitude,longitude)[weather_columns]
+        if (len(df_weather_of_store) < delta.days) or (df_weather_of_store.isna().sum().sum() > 0) or len(
+                df_weather_of_store) == 0:
+            df_weather_of_store = \
+                cls.return_weather_daily_data_for_specific_location(start_date_str,
+                                                                    end_date_str, lat_vienna,
+                                                                    lon_vienna)[
+                    weather_columns]
+
+        df_weather_of_store['store'] = store_id
+        df_weather_of_store['store'] = df_weather_of_store['store'].astype(int)
+
+
+        return df_weather_of_store.reset_index().rename(columns={"index": "date", "time": "date"})
+
+    @classmethod
+    def generate(cls, store_location_df,store_id, start_predict_date, end_predict_date, weather_columns=config.WEATHER_COLUMNS):
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
+        store_weather_df = cls.load(store_location_df=store_location_df, store_id=store_id, start_date=start_predict_date, end_date=end_predict_date, weather_columns=weather_columns)
+        return store_weather_df
+
+
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/config_batch_dict.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/config_batch_dict.py`

 * *Files identical despite different names*

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/event_feature_test.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/event_feature_test.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-import sys
-
-from ..preprocessor import Preprocessor
-from ..regular_data_handler import RegularDataLoader
-
-
-from ..features.event_features import EventHistoryFeatureLoader, EventFeaturesGenerator, \
-    EventEncodingFeaturesLoader
-from .. import config as global_config
-
-
-def test_event_features_load():
-    event_feature_df = EventHistoryFeatureLoader.load(project_name=global_config.DEFAULT_EVENT_FEATURES['project_name'],
-                                                      task_name=global_config.DEFAULT_EVENT_FEATURES['task_name'],
-                                                      task_id=global_config.DEFAULT_EVENT_FEATURES['task_id'],
-                                                      artifact_name=global_config.DEFAULT_EVENT_FEATURES['artifact_name'])
-
-    print(event_feature_df)
-    print(event_feature_df.columns)
-
-
-def test_event_features_generate():
-    generator = EventFeaturesGenerator()
-    preprocessor = Preprocessor()
-    stores = ['4906', '3']
-    df = RegularDataLoader().load()
-    df = df[df['store'].isin(stores)]
-    skus_1 = df[df['store'] == '4906']['item'].unique()[0:5]
-    skus_2 = df[df['store'] == '3']['item'].unique()[0:5]
-    df = df[df['item'].isin(skus_1) | df['item'].isin(skus_2)]
-
-    df = generator.generate(regular_data_df = df)
-    print(df)
-    print(df.info())
-
-
-def test_event_encoding_features_loader():
-    artifacts = EventEncodingFeaturesLoader().load()
-
-    model3 = artifacts['apply_encodings_dict']
-    print(model3)
-
-    # print(artifacts.keys())
-    # model1 = artifacts['apply_encodings_at_once']
-    # print(model1)
-    # model2 = artifacts['apply_encodings_dict']
-    # print(model2)
-    #
-    # model4 = artifacts['pca_dict']
-    # print(model4)
-
-test_event_features_generate()
-#test_event_features_load()
-#test_event_encoding_features_loader()
-
-
+import sys
+
+from ..preprocessor import Preprocessor
+from ..regular_data_handler import RegularDataLoader
+
+
+from ..features.event_features import EventHistoryFeatureLoader, EventFeaturesGenerator, \
+    EventEncodingFeaturesLoader
+from .. import config as global_config
+
+
+def test_event_features_load():
+    event_feature_df = EventHistoryFeatureLoader.load(project_name=global_config.DEFAULT_EVENT_FEATURES['project_name'],
+                                                      task_name=global_config.DEFAULT_EVENT_FEATURES['task_name'],
+                                                      task_id=global_config.DEFAULT_EVENT_FEATURES['task_id'],
+                                                      artifact_name=global_config.DEFAULT_EVENT_FEATURES['artifact_name'])
+
+    print(event_feature_df)
+    print(event_feature_df.columns)
+
+
+def test_event_features_generate():
+    generator = EventFeaturesGenerator()
+    preprocessor = Preprocessor()
+    stores = ['4906', '3']
+    df = RegularDataLoader().load()
+    df = df[df['store'].isin(stores)]
+    skus_1 = df[df['store'] == '4906']['item'].unique()[0:5]
+    skus_2 = df[df['store'] == '3']['item'].unique()[0:5]
+    df = df[df['item'].isin(skus_1) | df['item'].isin(skus_2)]
+
+    df = generator.generate(regular_data_df = df)
+    print(df)
+    print(df.info())
+
+
+def test_event_encoding_features_loader():
+    artifacts = EventEncodingFeaturesLoader().load()
+
+    model3 = artifacts['apply_encodings_dict']
+    print(model3)
+
+    # print(artifacts.keys())
+    # model1 = artifacts['apply_encodings_at_once']
+    # print(model1)
+    # model2 = artifacts['apply_encodings_dict']
+    # print(model2)
+    #
+    # model4 = artifacts['pca_dict']
+    # print(model4)
+
+test_event_features_generate()
+#test_event_features_load()
+#test_event_encoding_features_loader()
+
+
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/features_test.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/features_test.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import sys
-sys.path.append('../..')
-from src.palmers_preprocessing.features.future_features import MarketingPlanFeatures, ItemSaleEncodedFeatures, \
-    StoreSaleEncodedFeatures, FarFutureFeaturesGenerator
-from src.palmers_preprocessing.clearml_data_handler import TaskLoader, ArtifactLoader
-
-
-def test_marketing_plan_features():
-    mpf = MarketingPlanFeatures()
-    df = mpf.load()
-    print(df)
-    print(df.info())
-
-def test_sku_sale_encoded_features():
-    ssef = ItemSaleEncodedFeatures()
-    df = ssef.load()
-    print(df)
-    print(df.info())
-
-
-def test_store_sale_encoded_features():
-    ssef = StoreSaleEncodedFeatures()
-    df = ssef.load()
-    print(df)
-    print(df.info())
-
-
-def test_task_loader():
-    tl = ArtifactLoader()
-    tt = tl.load_artifact_as_df(artifact_name='sku_sales_encoders',  project_name="examples",
-                            task_name="sku_store_sales_encoders",
-                            task_id="a313d610ce5a43f6936f50a103984096", tags=None
-                        )
-    print(tt)
-
-
-def test_far_future_feature_generator():
-    fffg = FarFutureFeaturesGenerator()
-    import config_batch_dict as cbd
-    d = fffg.far_future_features_preprocess_of_store(cbd.ids_batches['3'])
-    print(d)
-    print(d.info())
-
-
-
-def test_far_future_feature_generator_2():
-    fffg = FarFutureFeaturesGenerator()
-    import config_batch_dict as cbd
-    subdict = {k: v for k, v in cbd.ids_batches.items() if k in ['4906', '3']}
-
-    a = fffg.far_future_features_preprocess_of_several_stores(subdict, begin_predict_dates='2023-05-01')
-    print(a)
-    print(a['4906'].columns.tolist())
-    print(a['4906'].info())
-
-
-
-#test_marketing_plan_features()
-#test_sku_sale_encoded_features()
-#test_store_sale_encoded_features()
-#test_far_future_feature_generator()
+import sys
+sys.path.append('../..')
+from src.palmers_preprocessing.features.future_features import MarketingPlanFeatures, ItemSaleEncodedFeatures, \
+    StoreSaleEncodedFeatures, FarFutureFeaturesGenerator
+from src.palmers_preprocessing.clearml_data_handler import TaskLoader, ArtifactLoader
+
+
+def test_marketing_plan_features():
+    mpf = MarketingPlanFeatures()
+    df = mpf.load()
+    print(df)
+    print(df.info())
+
+def test_sku_sale_encoded_features():
+    ssef = ItemSaleEncodedFeatures()
+    df = ssef.load()
+    print(df)
+    print(df.info())
+
+
+def test_store_sale_encoded_features():
+    ssef = StoreSaleEncodedFeatures()
+    df = ssef.load()
+    print(df)
+    print(df.info())
+
+
+def test_task_loader():
+    tl = ArtifactLoader()
+    tt = tl.load_artifact_as_df(artifact_name='sku_sales_encoders',  project_name="examples",
+                            task_name="sku_store_sales_encoders",
+                            task_id="a313d610ce5a43f6936f50a103984096", tags=None
+                        )
+    print(tt)
+
+
+def test_far_future_feature_generator():
+    fffg = FarFutureFeaturesGenerator()
+    import config_batch_dict as cbd
+    d = fffg.far_future_features_preprocess_of_store(cbd.ids_batches['3'])
+    print(d)
+    print(d.info())
+
+
+
+def test_far_future_feature_generator_2():
+    fffg = FarFutureFeaturesGenerator()
+    import config_batch_dict as cbd
+    subdict = {k: v for k, v in cbd.ids_batches.items() if k in ['4906', '3']}
+
+    a = fffg.far_future_features_preprocess_of_several_stores(subdict, begin_predict_dates='2023-05-01')
+    print(a)
+    print(a['4906'].columns.tolist())
+    print(a['4906'].info())
+
+
+
+#test_marketing_plan_features()
+#test_sku_sale_encoded_features()
+#test_store_sale_encoded_features()
+#test_far_future_feature_generator()
 test_far_future_feature_generator_2()
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/preprocessor_test.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/preprocessor_test.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import sys
-import catboost
-
-from src.palmers_preprocessing.regular_data_handler import RegularDataLoader
-import pandas as pd
-sys.path.append('../..')
-from src.palmers_preprocessing.preprocessor import Preprocessor
-from src.palmers_preprocessing.utils import convert_df_with_sku_to_df_with_item, daily_sales_to_weekly_mean_sales
-from clearml import Model, InputModel, Task
-import pickle
-
-def test_prepreocessor():
-    preprocessor = Preprocessor()
-    stores = ['3']
-    print("Loading data...")
-    df = RegularDataLoader().load()
-    print(df['store'].unique().tolist())
-    print("Data loaded")
-    df = df[df['store'].isin(stores)]
-    print("Data filtered")
-    print(df.head())
-    print("Convert df with sku to df with item")
-    df = convert_df_with_sku_to_df_with_item(df)
-    print(df.info())
-
-  #  items_1 = df[df['store'] == '100']['item'].unique()
-  #  items_2 = df[df['store'] == '3']['item'].unique()
-  #  df = df[df['item'].isin(items_1) | df['item'].isin(items_2)]
-    print(df["item, store"].unique())
-    print("Daily Sales to weekly mean sales")
-    df = daily_sales_to_weekly_mean_sales(df)
-    df = preprocessor.preprocess(stores_list=[3], begin_predict_dates='2023-05-23', regular_data_df=df)
-    pd.set_option('display.max_rows', None)
-    print(df.isnull().sum())
-    print(df)
-    print(df.columns.tolist())
-    return df
-# def test_cumulative_features():
-#     preprocessor = Preprocessor()
-#     df = preprocessor.get_regular_data_of_store(store_id='109', predict_date='2023-05-23')
-#     cum_feat = preprocessor.get_cumulative_features(df)
-#     print(cum_feat)
-
-
-task = Task.init(project_name='test_predict_store_3', task_name='test_predict_store_3')
-model_id = '3e2ac457fc644f39b4eb6d5a68e84dfb'  # Replace with your actual model ID
-print("111")
-models_store_3_path = Model(model_id).get_local_copy()
-print("222")
-with open(models_store_3_path, 'rb') as f:
-     model_3 = pickle.load(f)['3']
-print(model_3)
-print("333")
-df = test_prepreocessor()
-for item_store in model_3.keys():
-    model = model_3[item_store]['model']
-    prediction = model.predict(df[df["item, store"] == item_store][model.feature_names_])[0]
-    print("Item store: ", item_store, "prediction: ", prediction)
-
-
+import sys
+import catboost
+
+from src.palmers_preprocessing.regular_data_handler import RegularDataLoader
+import pandas as pd
+sys.path.append('../..')
+from src.palmers_preprocessing.preprocessor import Preprocessor
+from src.palmers_preprocessing.utils import convert_df_with_sku_to_df_with_item, daily_sales_to_weekly_mean_sales
+from clearml import Model, InputModel, Task
+import pickle
+
+def test_prepreocessor():
+    preprocessor = Preprocessor()
+    stores = ['3']
+    print("Loading data...")
+    df = RegularDataLoader().load()
+    print(df['store'].unique().tolist())
+    print("Data loaded")
+    df = df[df['store'].isin(stores)]
+    print("Data filtered")
+    print(df.head())
+    print("Convert df with sku to df with item")
+    df = convert_df_with_sku_to_df_with_item(df)
+    print(df.info())
+
+  #  items_1 = df[df['store'] == '100']['item'].unique()
+  #  items_2 = df[df['store'] == '3']['item'].unique()
+  #  df = df[df['item'].isin(items_1) | df['item'].isin(items_2)]
+    print(df["item, store"].unique())
+    print("Daily Sales to weekly mean sales")
+    df = daily_sales_to_weekly_mean_sales(df)
+    df = preprocessor.preprocess(stores_list=[3], begin_predict_dates='2023-05-23', regular_data_df=df)
+    pd.set_option('display.max_rows', None)
+    print(df.isnull().sum())
+    print(df)
+    print(df.columns.tolist())
+    return df
+# def test_cumulative_features():
+#     preprocessor = Preprocessor()
+#     df = preprocessor.get_regular_data_of_store(store_id='109', predict_date='2023-05-23')
+#     cum_feat = preprocessor.get_cumulative_features(df)
+#     print(cum_feat)
+
+
+task = Task.init(project_name='test_predict_store_3', task_name='test_predict_store_3')
+model_id = '3e2ac457fc644f39b4eb6d5a68e84dfb'  # Replace with your actual model ID
+print("111")
+models_store_3_path = Model(model_id).get_local_copy()
+print("222")
+with open(models_store_3_path, 'rb') as f:
+     model_3 = pickle.load(f)['3']
+print(model_3)
+print("333")
+df = test_prepreocessor()
+for item_store in model_3.keys():
+    model = model_3[item_store]['model']
+    prediction = model.predict(df[df["item, store"] == item_store][model.feature_names_])[0]
+    print("Item store: ", item_store, "prediction: ", prediction)
+
+
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/sanity_checks.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/sanity_checks.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-all_columns =  ['date', 'sku, store', 'sales', 'sku', 'store', 'id_sales_lag_1', 'id_sales_lag_2', 'id_sales_lag_3', 'id_sales_lag_4', 'id_sales_lag_5', 'id_sales_lag_6', 'id_sales_lag_7', 'id_sales_lag_12', 'id_sales_lag_14', 'id_sales_lag_18', 'id_sales_lag_21', 'id_sales_lag_24', 'id_sales_lag_312', 'id_sales_lag_313', 'id_sales_lag_364', 'id_sales_lag_365', 'id_sales_rolling_1', 'id_sales_rolling_2', 'id_sales_rolling_3', 'id_sales_rolling_4', 'id_sales_rolling_5', 'id_sales_rolling_6', 'id_sales_rolling_7', 'id_sales_rolling_12', 'id_sales_rolling_14', 'id_sales_rolling_18', 'id_sales_rolling_21', 'id_sales_rolling_24', 'id_sales_rolling_312', 'id_sales_rolling_313', 'id_sales_rolling_364', 'id_sales_rolling_365', 'id_sales_diff_1', 'id_sales_diff_2', 'id_sales_diff_3', 'id_sales_diff_4', 'id_sales_diff_5', 'id_sales_diff_6', 'id_sales_diff_7', 'id_sales_diff_12', 'id_sales_diff_14', 'id_sales_diff_18', 'id_sales_diff_21', 'id_sales_diff_24', 'id_sales_diff_312', 'id_sales_diff_313', 'id_sales_diff_364', 'id_sales_diff_365', 'id_sales_ewm_0.99', 'id_sales_ewm_0.95', 'id_sales_ewm_0.7', 'id_sales_ewm_0.1', 'sku_sales_lag_1', 'sku_sales_lag_2', 'sku_sales_lag_3', 'sku_sales_lag_4', 'sku_sales_lag_5', 'sku_sales_lag_6', 'sku_sales_lag_7', 'sku_sales_lag_12', 'sku_sales_lag_14', 'sku_sales_lag_18', 'sku_sales_lag_21', 'sku_sales_lag_24', 'sku_sales_lag_312', 'sku_sales_lag_313', 'sku_sales_lag_364', 'sku_sales_lag_365', 'sku_sales_rolling_1', 'sku_sales_rolling_2', 'sku_sales_rolling_3', 'sku_sales_rolling_4', 'sku_sales_rolling_5', 'sku_sales_rolling_6', 'sku_sales_rolling_7', 'sku_sales_rolling_12', 'sku_sales_rolling_14', 'sku_sales_rolling_18', 'sku_sales_rolling_21', 'sku_sales_rolling_24', 'sku_sales_rolling_312', 'sku_sales_rolling_313', 'sku_sales_rolling_364', 'sku_sales_rolling_365', 'sku_sales_diff_1', 'sku_sales_diff_2', 'sku_sales_diff_3', 'sku_sales_diff_4', 'sku_sales_diff_5', 'sku_sales_diff_6', 'sku_sales_diff_7', 'sku_sales_diff_12', 'sku_sales_diff_14', 'sku_sales_diff_18', 'sku_sales_diff_21', 'sku_sales_diff_24', 'sku_sales_diff_312', 'sku_sales_diff_313', 'sku_sales_diff_364', 'sku_sales_diff_365', 'sku_sales_ewm_0.99', 'sku_sales_ewm_0.95', 'sku_sales_ewm_0.7', 'sku_sales_ewm_0.1', 'store_sales_lag_1', 'store_sales_lag_2', 'store_sales_lag_3', 'store_sales_lag_4', 'store_sales_lag_5', 'store_sales_lag_6', 'store_sales_lag_7', 'store_sales_lag_12', 'store_sales_lag_14', 'store_sales_lag_18', 'store_sales_lag_21', 'store_sales_lag_24', 'store_sales_lag_312', 'store_sales_lag_313', 'store_sales_lag_364', 'store_sales_lag_365', 'store_sales_rolling_1', 'store_sales_rolling_2', 'store_sales_rolling_3', 'store_sales_rolling_4', 'store_sales_rolling_5', 'store_sales_rolling_6', 'store_sales_rolling_7', 'store_sales_rolling_12', 'store_sales_rolling_14', 'store_sales_rolling_18', 'store_sales_rolling_21', 'store_sales_rolling_24', 'store_sales_rolling_312', 'store_sales_rolling_313', 'store_sales_rolling_364', 'store_sales_rolling_365', 'store_sales_diff_1', 'store_sales_diff_2', 'store_sales_diff_3', 'store_sales_diff_4', 'store_sales_diff_5', 'store_sales_diff_6', 'store_sales_diff_7', 'store_sales_diff_12', 'store_sales_diff_14', 'store_sales_diff_18', 'store_sales_diff_21', 'store_sales_diff_24', 'store_sales_diff_312', 'store_sales_diff_313', 'store_sales_diff_364', 'store_sales_diff_365', 'store_sales_ewm_0.99', 'store_sales_ewm_0.95', 'store_sales_ewm_0.7', 'store_sales_ewm_0.1', 'day', 'month', 'year', 'day_of_week', 'day_of_year', 'name_of_day', 'week_of_year', 'quarter', 'day_of_the_month', 'is_weekend_c', 'is_weekend_j', 'MEST_day_store', 'MEST_day_sku', 'MEST_month_store', 'MEST_month_sku', 'MEST_quarter_store', 'MEST_quarter_sku', 'tavg', 'tmin', 'tmax', 'prcp', 'snow', 'wspd', 'pres', 'is_weekend', 'is_event', 'event_id_list', 'duration_list', 'min_date_list', 'sub_event_id_list', 'is_old_list', 'max_date_list', 'duration_list_mean_event', 'duration_list_median_event', 'duration_list_std_event', 'num_event_id_list', 'num_sub_event_id_list', 'sales_diff', 'event_frequency', 'ind_change_combo_event', 'sales_log', 'amount_of_days_pass_from_start_of_event', 'amount_of_days_pass_from_start_of_event_most_new', 'holiday_name', 'type', 'comments', 'is_holday', 'is_sunday', 'type_holiday_name', 'cumulative_sum_sales', 'fft_real', 'fft_imag', 'skewness', 'kurtosis', 'slope', 'PC1', 'PC2', 'is_tomorrow_event', 'is_2_days_event', 'MEstimateEncoder_of_type_holiday_name', 'MEstimateEncoder_of_num_sub_event_id_list', 'MEstimateEncoder_of_cumulative_sum_sales', 'MEstimateEncoder_of_PC1', 'MEstimateEncoder_of_PC2', 'MEstimateEncoder_of_comments', 'MEstimateEncoder_of_fft_real', 'MEstimateEncoder_of_fft_imag', 'MEstimateEncoder_of_num_event_id_list', 'MEstimateEncoder_of_duration_list_mean_event', 'MEstimateEncoder_of_duration_list_median_event', 'MEstimateEncoder_of_duration_list_std_event', 'MEstimateEncoder_of_is_weekend', 'MEstimateEncoder_of_ind_change_combo_event', 'MEstimateEncoder_of_is_sunday', 'MEstimateEncoder_of_is_tomorrow_event', 'MEstimateEncoder_of_is_2_days_event', 'CatBoostEncoder_of_type_holiday_name', 'CatBoostEncoder_of_num_sub_event_id_list', 'CatBoostEncoder_of_cumulative_sum_sales', 'CatBoostEncoder_of_PC1', 'CatBoostEncoder_of_PC2', 'CatBoostEncoder_of_comments', 'CatBoostEncoder_of_fft_real', 'CatBoostEncoder_of_fft_imag', 'CatBoostEncoder_of_num_event_id_list', 'CatBoostEncoder_of_duration_list_mean_event', 'CatBoostEncoder_of_duration_list_median_event', 'CatBoostEncoder_of_duration_list_std_event', 'CatBoostEncoder_of_is_weekend', 'CatBoostEncoder_of_ind_change_combo_event', 'CatBoostEncoder_of_is_sunday', 'CatBoostEncoder_of_is_tomorrow_event', 'CatBoostEncoder_of_is_2_days_event', 'MEstimateEncoder_of_all_type_holiday_name', 'MEstimateEncoder_of_all_num_sub_event_id_list', 'MEstimateEncoder_of_all_cumulative_sum_sales', 'MEstimateEncoder_of_all_PC1', 'MEstimateEncoder_of_all_PC2', 'MEstimateEncoder_of_all_comments', 'MEstimateEncoder_of_all_fft_real', 'MEstimateEncoder_of_all_fft_imag', 'MEstimateEncoder_of_all_num_event_id_list', 'MEstimateEncoder_of_all_duration_list_mean_event', 'MEstimateEncoder_of_all_duration_list_median_event', 'MEstimateEncoder_of_all_duration_list_std_event', 'MEstimateEncoder_of_all_is_weekend', 'MEstimateEncoder_of_all_ind_change_combo_event', 'MEstimateEncoder_of_all_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event', 'MEstimateEncoder_of_all_is_2_days_event', 'CatBoostEncoder_of_all_type_holiday_name', 'CatBoostEncoder_of_all_num_sub_event_id_list', 'CatBoostEncoder_of_all_cumulative_sum_sales', 'CatBoostEncoder_of_all_PC1', 'CatBoostEncoder_of_all_PC2', 'CatBoostEncoder_of_all_comments', 'CatBoostEncoder_of_all_fft_real', 'CatBoostEncoder_of_all_fft_imag', 'CatBoostEncoder_of_all_num_event_id_list', 'CatBoostEncoder_of_all_duration_list_mean_event', 'CatBoostEncoder_of_all_duration_list_median_event', 'CatBoostEncoder_of_all_duration_list_std_event', 'CatBoostEncoder_of_all_is_weekend', 'CatBoostEncoder_of_all_ind_change_combo_event', 'CatBoostEncoder_of_all_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event', 'CatBoostEncoder_of_all_is_2_days_event', 'num_sub_event_id_list_interactions_day_of_week', 'num_sub_event_id_list_interactions_week_of_year', 'num_sub_event_id_list_interactions_quarter', 'num_sub_event_id_list_interactions_is_weekend', 'num_sub_event_id_list_interactions_ind_change_combo_event', 'num_sub_event_id_list_interactions_is_sunday', 'num_sub_event_id_list_interactions_is_holday', 'num_event_id_list_interactions_day_of_week', 'num_event_id_list_interactions_week_of_year', 'num_event_id_list_interactions_quarter', 'num_event_id_list_interactions_is_weekend', 'num_event_id_list_interactions_ind_change_combo_event', 'num_event_id_list_interactions_is_sunday', 'num_event_id_list_interactions_is_holday', 'PC1_interactions_day_of_week', 'PC1_interactions_week_of_year', 'PC1_interactions_quarter', 'PC1_interactions_is_weekend', 'PC1_interactions_ind_change_combo_event', 'PC1_interactions_is_sunday', 'PC1_interactions_is_holday', 'PC2_interactions_day_of_week', 'PC2_interactions_week_of_year', 'PC2_interactions_quarter', 'PC2_interactions_is_weekend', 'PC2_interactions_ind_change_combo_event', 'PC2_interactions_is_sunday', 'PC2_interactions_is_holday', 'fft_real_interactions_day_of_week', 'fft_real_interactions_week_of_year', 'fft_real_interactions_quarter', 'fft_real_interactions_is_weekend', 'fft_real_interactions_ind_change_combo_event', 'fft_real_interactions_is_sunday', 'fft_real_interactions_is_holday', 'fft_imag_interactions_day_of_week', 'fft_imag_interactions_week_of_year', 'fft_imag_interactions_quarter', 'fft_imag_interactions_is_weekend', 'fft_imag_interactions_ind_change_combo_event', 'fft_imag_interactions_is_sunday', 'fft_imag_interactions_is_holday', 'cumulative_sum_sales_interactions_day_of_week', 'cumulative_sum_sales_interactions_week_of_year', 'cumulative_sum_sales_interactions_quarter', 'cumulative_sum_sales_interactions_is_weekend', 'cumulative_sum_sales_interactions_ind_change_combo_event', 'cumulative_sum_sales_interactions_is_sunday', 'cumulative_sum_sales_interactions_is_holday', 'duration_list_mean_event_interactions_day_of_week', 'duration_list_mean_event_interactions_week_of_year', 'duration_list_mean_event_interactions_quarter', 'duration_list_mean_event_interactions_is_weekend', 'duration_list_mean_event_interactions_ind_change_combo_event', 'duration_list_mean_event_interactions_is_sunday', 'duration_list_mean_event_interactions_is_holday', 'duration_list_std_event_interactions_day_of_week', 'duration_list_std_event_interactions_week_of_year', 'duration_list_std_event_interactions_quarter', 'duration_list_std_event_interactions_is_weekend', 'duration_list_std_event_interactions_ind_change_combo_event', 'duration_list_std_event_interactions_is_sunday', 'duration_list_std_event_interactions_is_holday', 'duration_list_median_event_interactions_day_of_week', 'duration_list_median_event_interactions_week_of_year', 'duration_list_median_event_interactions_quarter', 'duration_list_median_event_interactions_is_weekend', 'duration_list_median_event_interactions_ind_change_combo_event', 'duration_list_median_event_interactions_is_sunday', 'duration_list_median_event_interactions_is_holday', 'is_tomorrow_event_interactions_day_of_week', 'is_tomorrow_event_interactions_week_of_year', 'is_tomorrow_event_interactions_quarter', 'is_tomorrow_event_interactions_is_weekend', 'is_tomorrow_event_interactions_ind_change_combo_event', 'is_tomorrow_event_interactions_is_sunday', 'is_tomorrow_event_interactions_is_holday', 'is_2_days_event_interactions_day_of_week', 'is_2_days_event_interactions_week_of_year', 'is_2_days_event_interactions_quarter', 'is_2_days_event_interactions_is_weekend', 'is_2_days_event_interactions_ind_change_combo_event', 'is_2_days_event_interactions_is_sunday', 'is_2_days_event_interactions_is_holday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_PC1_interactions_day_of_week', 'MEstimateEncoder_of_all_PC1_interactions_week_of_year', 'MEstimateEncoder_of_all_PC1_interactions_quarter', 'MEstimateEncoder_of_all_PC1_interactions_is_weekend', 'MEstimateEncoder_of_all_PC1_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC1_interactions_is_sunday', 'MEstimateEncoder_of_all_PC1_interactions_is_holday', 'MEstimateEncoder_of_all_PC2_interactions_day_of_week', 'MEstimateEncoder_of_all_PC2_interactions_week_of_year', 'MEstimateEncoder_of_all_PC2_interactions_quarter', 'MEstimateEncoder_of_all_PC2_interactions_is_weekend', 'MEstimateEncoder_of_all_PC2_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC2_interactions_is_sunday', 'MEstimateEncoder_of_all_PC2_interactions_is_holday', 'MEstimateEncoder_of_all_fft_real_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_real_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_real_interactions_quarter', 'MEstimateEncoder_of_all_fft_real_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_real_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_real_interactions_is_holday', 'MEstimateEncoder_of_all_fft_imag_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_imag_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_imag_interactions_quarter', 'MEstimateEncoder_of_all_fft_imag_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_imag_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_imag_interactions_is_holday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_quarter', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_2_days_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_2_days_event_interactions_quarter', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_holday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_PC1_interactions_day_of_week', 'CatBoostEncoder_of_all_PC1_interactions_week_of_year', 'CatBoostEncoder_of_all_PC1_interactions_quarter', 'CatBoostEncoder_of_all_PC1_interactions_is_weekend', 'CatBoostEncoder_of_all_PC1_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC1_interactions_is_sunday', 'CatBoostEncoder_of_all_PC1_interactions_is_holday', 'CatBoostEncoder_of_all_PC2_interactions_day_of_week', 'CatBoostEncoder_of_all_PC2_interactions_week_of_year', 'CatBoostEncoder_of_all_PC2_interactions_quarter', 'CatBoostEncoder_of_all_PC2_interactions_is_weekend', 'CatBoostEncoder_of_all_PC2_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC2_interactions_is_sunday', 'CatBoostEncoder_of_all_PC2_interactions_is_holday', 'CatBoostEncoder_of_all_fft_real_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_real_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_real_interactions_quarter', 'CatBoostEncoder_of_all_fft_real_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_real_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_real_interactions_is_holday', 'CatBoostEncoder_of_all_fft_imag_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_imag_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_imag_interactions_quarter', 'CatBoostEncoder_of_all_fft_imag_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_imag_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_imag_interactions_is_holday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_quarter', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_2_days_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_2_days_event_interactions_quarter', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_holday', 'Palmers Week', 'Maria Galland', 'Black Weekend', 'Cyber Monday', 'Valentine', 'Bride', 'Frühling', 'Ostern', 'Muttertag', 'Vatertag', 'Glamour Week', 'Palmers x Marina Hoermanseder', 'Palmers x Lenzing', 'Black  Week', 'Osterpromotion PALMERS Münz-Ei', 'Woman’s Day', '20% auf alle Herrenartikel', 'WOMAN SOMMER SHOPPING', 'Palmers Münze 50+10', '- 20% auf Strümpfe Shade', 'ab 80€ Einkauf', 'Palmers Münze 100+10', 'Kampagne Bademode', '20€ geschenkt', 'SHADE Promotion', '10€ Palmers Münze geschenkt', 'CLUB PROMO', 'WELTFRAUENTAG', '2+1 STRUMPFKATION', 'Muttertag Münze 100+10', '20€ geschenkt Palmers Club', 'FINAL SALE WITH NUM', 'FINAL SALE', 'MID SEASON SALE', 'PALMERS CLUB SALE', 'lag_-1_Palmers Week', 'lag_-1_Maria Galland', 'lag_-1_Black Weekend', 'lag_-1_Cyber Monday', 'lag_-1_Valentine', 'lag_-1_Bride', 'lag_-1_Frühling', 'lag_-1_Ostern', 'lag_-1_Muttertag', 'lag_-1_Vatertag', 'lag_-1_Glamour Week', 'lag_-1_Palmers x Marina Hoermanseder', 'lag_-1_Palmers x Lenzing', 'lag_-1_Black  Week', 'lag_-1_Osterpromotion PALMERS Münz-Ei', 'lag_-1_Woman’s Day', 'lag_-1_20% auf alle Herrenartikel', 'lag_-1_WOMAN SOMMER SHOPPING', 'lag_-1_Palmers Münze 50+10', 'lag_-1_- 20% auf Strümpfe Shade', 'lag_-1_ab 80€ Einkauf', 'lag_-1_Palmers Münze 100+10', 'lag_-1_Kampagne Bademode', 'lag_-1_20€ geschenkt', 'lag_-1_SHADE Promotion', 'lag_-1_10€ Palmers Münze geschenkt', 'lag_-1_CLUB PROMO', 'lag_-1_WELTFRAUENTAG', 'lag_-1_2+1 STRUMPFKATION', 'lag_-1_Muttertag Münze 100+10', 'lag_-1_20€ geschenkt Palmers Club', 'lag_-1_FINAL SALE WITH NUM', 'lag_-1_FINAL SALE', 'lag_-1_MID SEASON SALE', 'lag_-1_PALMERS CLUB SALE', 'lag_-2_Palmers Week', 'lag_-2_Maria Galland', 'lag_-2_Black Weekend', 'lag_-2_Cyber Monday', 'lag_-2_Valentine', 'lag_-2_Bride', 'lag_-2_Frühling', 'lag_-2_Ostern', 'lag_-2_Muttertag', 'lag_-2_Vatertag', 'lag_-2_Glamour Week', 'lag_-2_Palmers x Marina Hoermanseder', 'lag_-2_Palmers x Lenzing', 'lag_-2_Black  Week', 'lag_-2_Osterpromotion PALMERS Münz-Ei', 'lag_-2_Woman’s Day', 'lag_-2_20% auf alle Herrenartikel', 'lag_-2_WOMAN SOMMER SHOPPING', 'lag_-2_Palmers Münze 50+10', 'lag_-2_- 20% auf Strümpfe Shade', 'lag_-2_ab 80€ Einkauf', 'lag_-2_Palmers Münze 100+10', 'lag_-2_Kampagne Bademode', 'lag_-2_20€ geschenkt', 'lag_-2_SHADE Promotion', 'lag_-2_10€ Palmers Münze geschenkt', 'lag_-2_CLUB PROMO', 'lag_-2_WELTFRAUENTAG', 'lag_-2_2+1 STRUMPFKATION', 'lag_-2_Muttertag Münze 100+10', 'lag_-2_20€ geschenkt Palmers Club', 'lag_-2_FINAL SALE WITH NUM', 'lag_-2_FINAL SALE', 'lag_-2_MID SEASON SALE', 'lag_-2_PALMERS CLUB SALE', 'sales_cumulative_store_sku_D', 'sales_cumulative_store_sku_W-Mon', 'sales_cumulative_store_sku_M', 'sales_cumulative_store_sku_Y', 'sales_expected_store_sku_D', 'sales_expected_store_sku_W-Mon', 'sales_expected_store_sku_M', 'sales_expected_store_sku_Y']
-some_columns = ['date', 'sales', 'id_sales_lag_1', 'id_sales_lag_2', 'id_sales_lag_3', 'id_sales_lag_4', 'id_sales_lag_5', 'id_sales_lag_6', 'id_sales_lag_7', 'id_sales_lag_12', 'id_sales_lag_14', 'id_sales_lag_18', 'id_sales_lag_21', 'id_sales_lag_24', 'id_sales_lag_312', 'id_sales_lag_313', 'id_sales_lag_364', 'id_sales_lag_365', 'id_sales_rolling_1', 'id_sales_rolling_2', 'id_sales_rolling_3', 'id_sales_rolling_4', 'id_sales_rolling_5', 'id_sales_rolling_6', 'id_sales_rolling_7', 'id_sales_rolling_12', 'id_sales_rolling_14', 'id_sales_rolling_18', 'id_sales_rolling_21', 'id_sales_rolling_24', 'id_sales_rolling_312', 'id_sales_rolling_313', 'id_sales_rolling_364', 'id_sales_rolling_365', 'id_sales_diff_1', 'id_sales_diff_2', 'id_sales_diff_3', 'id_sales_diff_4', 'id_sales_diff_5', 'id_sales_diff_6', 'id_sales_diff_7', 'id_sales_diff_12', 'id_sales_diff_14', 'id_sales_diff_18', 'id_sales_diff_21', 'id_sales_diff_24', 'id_sales_diff_312', 'id_sales_diff_313', 'id_sales_diff_364', 'id_sales_diff_365', 'id_sales_ewm_0.99', 'id_sales_ewm_0.95', 'id_sales_ewm_0.7', 'id_sales_ewm_0.1', 'sku', 'store', 'sku, store', 'year', 'month', 'day', 'day_of_week', 'week_of_year', 'quarter', 'is_weekend', 'day_of_year', 'day_of_the_month', 'is_weekend_c', 'is_weekend_j', 'Palmers Week', 'Maria Galland', 'Black Weekend', 'Cyber Monday', 'Valentine', 'Bride', 'Frühling', 'Ostern', 'Muttertag', 'Vatertag', 'Glamour Week', 'Palmers x Marina Hoermanseder', 'Palmers x Lenzing', 'Black  Week', 'Osterpromotion PALMERS Münz-Ei', 'Woman’s Day', '20% auf alle Herrenartikel', 'WOMAN SOMMER SHOPPING', 'Palmers Münze 50+10', '- 20% auf Strümpfe Shade', 'ab 80€ Einkauf', 'Palmers Münze 100+10', 'Kampagne Bademode', '20€ geschenkt', 'SHADE Promotion', '10€ Palmers Münze geschenkt', 'CLUB PROMO', 'WELTFRAUENTAG', '2+1 STRUMPFKATION', 'Muttertag Münze 100+10', '20€ geschenkt Palmers Club', 'FINAL SALE WITH NUM', 'FINAL SALE', 'MID SEASON SALE', 'PALMERS CLUB SALE', 'lag_-1_Palmers Week', 'lag_-1_Maria Galland', 'lag_-1_Black Weekend', 'lag_-1_Cyber Monday', 'lag_-1_Valentine', 'lag_-1_Bride', 'lag_-1_Frühling', 'lag_-1_Ostern', 'lag_-1_Muttertag', 'lag_-1_Vatertag', 'lag_-1_Glamour Week', 'lag_-1_Palmers x Marina Hoermanseder', 'lag_-1_Palmers x Lenzing', 'lag_-1_Black  Week', 'lag_-1_Osterpromotion PALMERS Münz-Ei', 'lag_-1_Woman’s Day', 'lag_-1_20% auf alle Herrenartikel', 'lag_-1_WOMAN SOMMER SHOPPING', 'lag_-1_Palmers Münze 50+10', 'lag_-1_- 20% auf Strümpfe Shade', 'lag_-1_ab 80€ Einkauf', 'lag_-1_Palmers Münze 100+10', 'lag_-1_Kampagne Bademode', 'lag_-1_20€ geschenkt', 'lag_-1_SHADE Promotion', 'lag_-1_10€ Palmers Münze geschenkt', 'lag_-1_CLUB PROMO', 'lag_-1_WELTFRAUENTAG', 'lag_-1_2+1 STRUMPFKATION', 'lag_-1_Muttertag Münze 100+10', 'lag_-1_20€ geschenkt Palmers Club', 'lag_-1_FINAL SALE WITH NUM', 'lag_-1_FINAL SALE', 'lag_-1_MID SEASON SALE', 'lag_-1_PALMERS CLUB SALE', 'lag_-2_Palmers Week', 'lag_-2_Maria Galland', 'lag_-2_Black Weekend', 'lag_-2_Cyber Monday', 'lag_-2_Valentine', 'lag_-2_Bride', 'lag_-2_Frühling', 'lag_-2_Ostern', 'lag_-2_Muttertag', 'lag_-2_Vatertag', 'lag_-2_Glamour Week', 'lag_-2_Palmers x Marina Hoermanseder', 'lag_-2_Palmers x Lenzing', 'lag_-2_Black  Week', 'lag_-2_Osterpromotion PALMERS Münz-Ei', 'lag_-2_Woman’s Day', 'lag_-2_20% auf alle Herrenartikel', 'lag_-2_WOMAN SOMMER SHOPPING', 'lag_-2_Palmers Münze 50+10', 'lag_-2_- 20% auf Strümpfe Shade', 'lag_-2_ab 80€ Einkauf', 'lag_-2_Palmers Münze 100+10', 'lag_-2_Kampagne Bademode', 'lag_-2_20€ geschenkt', 'lag_-2_SHADE Promotion', 'lag_-2_10€ Palmers Münze geschenkt', 'lag_-2_CLUB PROMO', 'lag_-2_WELTFRAUENTAG', 'lag_-2_2+1 STRUMPFKATION', 'lag_-2_Muttertag Münze 100+10', 'lag_-2_20€ geschenkt Palmers Club', 'lag_-2_FINAL SALE WITH NUM', 'lag_-2_FINAL SALE', 'lag_-2_MID SEASON SALE', 'lag_-2_PALMERS CLUB SALE', 'MEST_day_store', 'MEST_day_sku', 'MEST_month_store', 'MEST_month_sku', 'MEST_quarter_store', 'MEST_quarter_sku', 'store_sales_lag_1', 'store_sales_lag_2', 'store_sales_lag_3', 'store_sales_lag_4', 'store_sales_lag_5', 'store_sales_lag_6', 'store_sales_lag_7', 'store_sales_lag_12', 'store_sales_lag_14', 'store_sales_lag_18', 'store_sales_lag_21', 'store_sales_lag_24', 'store_sales_lag_312', 'store_sales_lag_313', 'store_sales_lag_364', 'store_sales_lag_365', 'store_sales_rolling_1', 'store_sales_rolling_2', 'store_sales_rolling_3', 'store_sales_rolling_4', 'store_sales_rolling_5', 'store_sales_rolling_6', 'store_sales_rolling_7', 'store_sales_rolling_12', 'store_sales_rolling_14', 'store_sales_rolling_18', 'store_sales_rolling_21', 'store_sales_rolling_24', 'store_sales_rolling_312', 'store_sales_rolling_313', 'store_sales_rolling_364', 'store_sales_rolling_365', 'store_sales_diff_1', 'store_sales_diff_2', 'store_sales_diff_3', 'store_sales_diff_4', 'store_sales_diff_5', 'store_sales_diff_6', 'store_sales_diff_7', 'store_sales_diff_12', 'store_sales_diff_14', 'store_sales_diff_18', 'store_sales_diff_21', 'store_sales_diff_24', 'store_sales_diff_312', 'store_sales_diff_313', 'store_sales_diff_364', 'store_sales_diff_365', 'store_sales_ewm_0.99', 'store_sales_ewm_0.95', 'store_sales_ewm_0.7', 'store_sales_ewm_0.1', 'tavg', 'tmin', 'tmax', 'prcp', 'snow', 'wspd', 'pres', 'sales_cumulative_store_sku_D', 'sales_cumulative_store_sku_W-Mon', 'sales_cumulative_store_sku_M', 'sales_cumulative_store_sku_Y', 'sales_expected_store_sku_D', 'sales_expected_store_sku_W-Mon', 'sales_expected_store_sku_M', 'sales_expected_store_sku_Y', 'sku_sales_lag_1', 'sku_sales_lag_2', 'sku_sales_lag_3', 'sku_sales_lag_4', 'sku_sales_lag_5', 'sku_sales_lag_6', 'sku_sales_lag_7', 'sku_sales_lag_12', 'sku_sales_lag_14', 'sku_sales_lag_18', 'sku_sales_lag_21', 'sku_sales_lag_24', 'sku_sales_lag_312', 'sku_sales_lag_313', 'sku_sales_lag_364', 'sku_sales_lag_365', 'sku_sales_rolling_1', 'sku_sales_rolling_2', 'sku_sales_rolling_3', 'sku_sales_rolling_4', 'sku_sales_rolling_5', 'sku_sales_rolling_6', 'sku_sales_rolling_7', 'sku_sales_rolling_12', 'sku_sales_rolling_14', 'sku_sales_rolling_18', 'sku_sales_rolling_21', 'sku_sales_rolling_24', 'sku_sales_rolling_312', 'sku_sales_rolling_313', 'sku_sales_rolling_364', 'sku_sales_rolling_365', 'sku_sales_diff_1', 'sku_sales_diff_2', 'sku_sales_diff_3', 'sku_sales_diff_4', 'sku_sales_diff_5', 'sku_sales_diff_6', 'sku_sales_diff_7', 'sku_sales_diff_12', 'sku_sales_diff_14', 'sku_sales_diff_18', 'sku_sales_diff_21', 'sku_sales_diff_24', 'sku_sales_diff_312', 'sku_sales_diff_313', 'sku_sales_diff_364', 'sku_sales_diff_365', 'sku_sales_ewm_0.99', 'sku_sales_ewm_0.95', 'sku_sales_ewm_0.7', 'sku_sales_ewm_0.1', 'is_event', 'event_id_list', 'duration_list', 'min_date_list', 'sub_event_id_list', 'is_old_list', 'max_date_list', 'duration_list_mean_event', 'duration_list_median_event', 'duration_list_std_event', 'num_event_id_list', 'num_sub_event_id_list', 'sales_diff', 'event_frequency', 'ind_change_combo_event', 'sales_log', 'amount_of_days_pass_from_start_of_event', 'amount_of_days_pass_from_start_of_event_most_new', 'holiday_name', 'type', 'comments', 'is_holday', 'is_sunday', 'type_holiday_name', 'cumulative_sum_sales', 'fft_real', 'fft_imag', 'skewness', 'kurtosis', 'slope', 'is_tomorrow_event', 'is_2_days_event', 'PC1', 'PC2', 'MEstimateEncoder_of_type_holiday_name', 'MEstimateEncoder_of_num_sub_event_id_list', 'MEstimateEncoder_of_cumulative_sum_sales', 'MEstimateEncoder_of_PC1', 'MEstimateEncoder_of_PC2', 'MEstimateEncoder_of_comments', 'MEstimateEncoder_of_fft_real', 'MEstimateEncoder_of_fft_imag', 'MEstimateEncoder_of_num_event_id_list', 'MEstimateEncoder_of_duration_list_mean_event', 'MEstimateEncoder_of_duration_list_median_event', 'MEstimateEncoder_of_duration_list_std_event', 'MEstimateEncoder_of_is_weekend', 'MEstimateEncoder_of_ind_change_combo_event', 'MEstimateEncoder_of_is_sunday', 'MEstimateEncoder_of_is_tomorrow_event', 'MEstimateEncoder_of_is_2_days_event', 'CatBoostEncoder_of_type_holiday_name', 'CatBoostEncoder_of_num_sub_event_id_list', 'CatBoostEncoder_of_cumulative_sum_sales', 'CatBoostEncoder_of_PC1', 'CatBoostEncoder_of_PC2', 'CatBoostEncoder_of_comments', 'CatBoostEncoder_of_fft_real', 'CatBoostEncoder_of_fft_imag', 'CatBoostEncoder_of_num_event_id_list', 'CatBoostEncoder_of_duration_list_mean_event', 'CatBoostEncoder_of_duration_list_median_event', 'CatBoostEncoder_of_duration_list_std_event', 'CatBoostEncoder_of_is_weekend', 'CatBoostEncoder_of_ind_change_combo_event', 'CatBoostEncoder_of_is_sunday', 'CatBoostEncoder_of_is_tomorrow_event', 'CatBoostEncoder_of_is_2_days_event', 'MEstimateEncoder_of_all_type_holiday_name', 'MEstimateEncoder_of_all_num_sub_event_id_list', 'MEstimateEncoder_of_all_cumulative_sum_sales', 'MEstimateEncoder_of_all_PC1', 'MEstimateEncoder_of_all_PC2', 'MEstimateEncoder_of_all_comments', 'MEstimateEncoder_of_all_fft_real', 'MEstimateEncoder_of_all_fft_imag', 'MEstimateEncoder_of_all_num_event_id_list', 'MEstimateEncoder_of_all_duration_list_mean_event', 'MEstimateEncoder_of_all_duration_list_median_event', 'MEstimateEncoder_of_all_duration_list_std_event', 'MEstimateEncoder_of_all_is_weekend', 'MEstimateEncoder_of_all_ind_change_combo_event', 'MEstimateEncoder_of_all_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event', 'MEstimateEncoder_of_all_is_2_days_event', 'CatBoostEncoder_of_all_type_holiday_name', 'CatBoostEncoder_of_all_num_sub_event_id_list', 'CatBoostEncoder_of_all_cumulative_sum_sales', 'CatBoostEncoder_of_all_PC1', 'CatBoostEncoder_of_all_PC2', 'CatBoostEncoder_of_all_comments', 'CatBoostEncoder_of_all_fft_real', 'CatBoostEncoder_of_all_fft_imag', 'CatBoostEncoder_of_all_num_event_id_list', 'CatBoostEncoder_of_all_duration_list_mean_event', 'CatBoostEncoder_of_all_duration_list_median_event', 'CatBoostEncoder_of_all_duration_list_std_event', 'CatBoostEncoder_of_all_is_weekend', 'CatBoostEncoder_of_all_ind_change_combo_event', 'CatBoostEncoder_of_all_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event', 'CatBoostEncoder_of_all_is_2_days_event', 'num_sub_event_id_list_interactions_day_of_week', 'num_sub_event_id_list_interactions_week_of_year', 'num_sub_event_id_list_interactions_quarter', 'num_sub_event_id_list_interactions_is_weekend', 'num_sub_event_id_list_interactions_ind_change_combo_event', 'num_sub_event_id_list_interactions_is_sunday', 'num_sub_event_id_list_interactions_is_holday', 'num_event_id_list_interactions_day_of_week', 'num_event_id_list_interactions_week_of_year', 'num_event_id_list_interactions_quarter', 'num_event_id_list_interactions_is_weekend', 'num_event_id_list_interactions_ind_change_combo_event', 'num_event_id_list_interactions_is_sunday', 'num_event_id_list_interactions_is_holday', 'PC1_interactions_day_of_week', 'PC1_interactions_week_of_year', 'PC1_interactions_quarter', 'PC1_interactions_is_weekend', 'PC1_interactions_ind_change_combo_event', 'PC1_interactions_is_sunday', 'PC1_interactions_is_holday', 'PC2_interactions_day_of_week', 'PC2_interactions_week_of_year', 'PC2_interactions_quarter', 'PC2_interactions_is_weekend', 'PC2_interactions_ind_change_combo_event', 'PC2_interactions_is_sunday', 'PC2_interactions_is_holday', 'fft_real_interactions_day_of_week', 'fft_real_interactions_week_of_year', 'fft_real_interactions_quarter', 'fft_real_interactions_is_weekend', 'fft_real_interactions_ind_change_combo_event', 'fft_real_interactions_is_sunday', 'fft_real_interactions_is_holday', 'fft_imag_interactions_day_of_week', 'fft_imag_interactions_week_of_year', 'fft_imag_interactions_quarter', 'fft_imag_interactions_is_weekend', 'fft_imag_interactions_ind_change_combo_event', 'fft_imag_interactions_is_sunday', 'fft_imag_interactions_is_holday', 'cumulative_sum_sales_interactions_day_of_week', 'cumulative_sum_sales_interactions_week_of_year', 'cumulative_sum_sales_interactions_quarter', 'cumulative_sum_sales_interactions_is_weekend', 'cumulative_sum_sales_interactions_ind_change_combo_event', 'cumulative_sum_sales_interactions_is_sunday', 'cumulative_sum_sales_interactions_is_holday', 'duration_list_mean_event_interactions_day_of_week', 'duration_list_mean_event_interactions_week_of_year', 'duration_list_mean_event_interactions_quarter', 'duration_list_mean_event_interactions_is_weekend', 'duration_list_mean_event_interactions_ind_change_combo_event', 'duration_list_mean_event_interactions_is_sunday', 'duration_list_mean_event_interactions_is_holday', 'duration_list_std_event_interactions_day_of_week', 'duration_list_std_event_interactions_week_of_year', 'duration_list_std_event_interactions_quarter', 'duration_list_std_event_interactions_is_weekend', 'duration_list_std_event_interactions_ind_change_combo_event', 'duration_list_std_event_interactions_is_sunday', 'duration_list_std_event_interactions_is_holday', 'duration_list_median_event_interactions_day_of_week', 'duration_list_median_event_interactions_week_of_year', 'duration_list_median_event_interactions_quarter', 'duration_list_median_event_interactions_is_weekend', 'duration_list_median_event_interactions_ind_change_combo_event', 'duration_list_median_event_interactions_is_sunday', 'duration_list_median_event_interactions_is_holday', 'is_tomorrow_event_interactions_day_of_week', 'is_tomorrow_event_interactions_week_of_year', 'is_tomorrow_event_interactions_quarter', 'is_tomorrow_event_interactions_is_weekend', 'is_tomorrow_event_interactions_ind_change_combo_event', 'is_tomorrow_event_interactions_is_sunday', 'is_tomorrow_event_interactions_is_holday', 'is_2_days_event_interactions_day_of_week', 'is_2_days_event_interactions_week_of_year', 'is_2_days_event_interactions_quarter', 'is_2_days_event_interactions_is_weekend', 'is_2_days_event_interactions_ind_change_combo_event', 'is_2_days_event_interactions_is_sunday', 'is_2_days_event_interactions_is_holday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_PC1_interactions_day_of_week', 'MEstimateEncoder_of_all_PC1_interactions_week_of_year', 'MEstimateEncoder_of_all_PC1_interactions_quarter', 'MEstimateEncoder_of_all_PC1_interactions_is_weekend', 'MEstimateEncoder_of_all_PC1_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC1_interactions_is_sunday', 'MEstimateEncoder_of_all_PC1_interactions_is_holday', 'MEstimateEncoder_of_all_PC2_interactions_day_of_week', 'MEstimateEncoder_of_all_PC2_interactions_week_of_year', 'MEstimateEncoder_of_all_PC2_interactions_quarter', 'MEstimateEncoder_of_all_PC2_interactions_is_weekend', 'MEstimateEncoder_of_all_PC2_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC2_interactions_is_sunday', 'MEstimateEncoder_of_all_PC2_interactions_is_holday', 'MEstimateEncoder_of_all_fft_real_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_real_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_real_interactions_quarter', 'MEstimateEncoder_of_all_fft_real_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_real_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_real_interactions_is_holday', 'MEstimateEncoder_of_all_fft_imag_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_imag_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_imag_interactions_quarter', 'MEstimateEncoder_of_all_fft_imag_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_imag_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_imag_interactions_is_holday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_quarter', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_2_days_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_2_days_event_interactions_quarter', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_holday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_PC1_interactions_day_of_week', 'CatBoostEncoder_of_all_PC1_interactions_week_of_year', 'CatBoostEncoder_of_all_PC1_interactions_quarter', 'CatBoostEncoder_of_all_PC1_interactions_is_weekend', 'CatBoostEncoder_of_all_PC1_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC1_interactions_is_sunday', 'CatBoostEncoder_of_all_PC1_interactions_is_holday', 'CatBoostEncoder_of_all_PC2_interactions_day_of_week', 'CatBoostEncoder_of_all_PC2_interactions_week_of_year', 'CatBoostEncoder_of_all_PC2_interactions_quarter', 'CatBoostEncoder_of_all_PC2_interactions_is_weekend', 'CatBoostEncoder_of_all_PC2_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC2_interactions_is_sunday', 'CatBoostEncoder_of_all_PC2_interactions_is_holday', 'CatBoostEncoder_of_all_fft_real_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_real_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_real_interactions_quarter', 'CatBoostEncoder_of_all_fft_real_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_real_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_real_interactions_is_holday', 'CatBoostEncoder_of_all_fft_imag_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_imag_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_imag_interactions_quarter', 'CatBoostEncoder_of_all_fft_imag_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_imag_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_imag_interactions_is_holday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_quarter', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_2_days_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_2_days_event_interactions_quarter', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_holday']
-
-
-
-
-def func(list1, list2):
-    not_in_list1 = set(list2).difference(list1)
-    print("Values not in list1 but in list2:", not_in_list1)
-    # find values not in list2 but in list1
-    not_in_list2 = set(list1).difference(list2)
-    print("Values not in list2 but in list1:", not_in_list2)
-
-
+all_columns =  ['date', 'sku, store', 'sales', 'sku', 'store', 'id_sales_lag_1', 'id_sales_lag_2', 'id_sales_lag_3', 'id_sales_lag_4', 'id_sales_lag_5', 'id_sales_lag_6', 'id_sales_lag_7', 'id_sales_lag_12', 'id_sales_lag_14', 'id_sales_lag_18', 'id_sales_lag_21', 'id_sales_lag_24', 'id_sales_lag_312', 'id_sales_lag_313', 'id_sales_lag_364', 'id_sales_lag_365', 'id_sales_rolling_1', 'id_sales_rolling_2', 'id_sales_rolling_3', 'id_sales_rolling_4', 'id_sales_rolling_5', 'id_sales_rolling_6', 'id_sales_rolling_7', 'id_sales_rolling_12', 'id_sales_rolling_14', 'id_sales_rolling_18', 'id_sales_rolling_21', 'id_sales_rolling_24', 'id_sales_rolling_312', 'id_sales_rolling_313', 'id_sales_rolling_364', 'id_sales_rolling_365', 'id_sales_diff_1', 'id_sales_diff_2', 'id_sales_diff_3', 'id_sales_diff_4', 'id_sales_diff_5', 'id_sales_diff_6', 'id_sales_diff_7', 'id_sales_diff_12', 'id_sales_diff_14', 'id_sales_diff_18', 'id_sales_diff_21', 'id_sales_diff_24', 'id_sales_diff_312', 'id_sales_diff_313', 'id_sales_diff_364', 'id_sales_diff_365', 'id_sales_ewm_0.99', 'id_sales_ewm_0.95', 'id_sales_ewm_0.7', 'id_sales_ewm_0.1', 'sku_sales_lag_1', 'sku_sales_lag_2', 'sku_sales_lag_3', 'sku_sales_lag_4', 'sku_sales_lag_5', 'sku_sales_lag_6', 'sku_sales_lag_7', 'sku_sales_lag_12', 'sku_sales_lag_14', 'sku_sales_lag_18', 'sku_sales_lag_21', 'sku_sales_lag_24', 'sku_sales_lag_312', 'sku_sales_lag_313', 'sku_sales_lag_364', 'sku_sales_lag_365', 'sku_sales_rolling_1', 'sku_sales_rolling_2', 'sku_sales_rolling_3', 'sku_sales_rolling_4', 'sku_sales_rolling_5', 'sku_sales_rolling_6', 'sku_sales_rolling_7', 'sku_sales_rolling_12', 'sku_sales_rolling_14', 'sku_sales_rolling_18', 'sku_sales_rolling_21', 'sku_sales_rolling_24', 'sku_sales_rolling_312', 'sku_sales_rolling_313', 'sku_sales_rolling_364', 'sku_sales_rolling_365', 'sku_sales_diff_1', 'sku_sales_diff_2', 'sku_sales_diff_3', 'sku_sales_diff_4', 'sku_sales_diff_5', 'sku_sales_diff_6', 'sku_sales_diff_7', 'sku_sales_diff_12', 'sku_sales_diff_14', 'sku_sales_diff_18', 'sku_sales_diff_21', 'sku_sales_diff_24', 'sku_sales_diff_312', 'sku_sales_diff_313', 'sku_sales_diff_364', 'sku_sales_diff_365', 'sku_sales_ewm_0.99', 'sku_sales_ewm_0.95', 'sku_sales_ewm_0.7', 'sku_sales_ewm_0.1', 'store_sales_lag_1', 'store_sales_lag_2', 'store_sales_lag_3', 'store_sales_lag_4', 'store_sales_lag_5', 'store_sales_lag_6', 'store_sales_lag_7', 'store_sales_lag_12', 'store_sales_lag_14', 'store_sales_lag_18', 'store_sales_lag_21', 'store_sales_lag_24', 'store_sales_lag_312', 'store_sales_lag_313', 'store_sales_lag_364', 'store_sales_lag_365', 'store_sales_rolling_1', 'store_sales_rolling_2', 'store_sales_rolling_3', 'store_sales_rolling_4', 'store_sales_rolling_5', 'store_sales_rolling_6', 'store_sales_rolling_7', 'store_sales_rolling_12', 'store_sales_rolling_14', 'store_sales_rolling_18', 'store_sales_rolling_21', 'store_sales_rolling_24', 'store_sales_rolling_312', 'store_sales_rolling_313', 'store_sales_rolling_364', 'store_sales_rolling_365', 'store_sales_diff_1', 'store_sales_diff_2', 'store_sales_diff_3', 'store_sales_diff_4', 'store_sales_diff_5', 'store_sales_diff_6', 'store_sales_diff_7', 'store_sales_diff_12', 'store_sales_diff_14', 'store_sales_diff_18', 'store_sales_diff_21', 'store_sales_diff_24', 'store_sales_diff_312', 'store_sales_diff_313', 'store_sales_diff_364', 'store_sales_diff_365', 'store_sales_ewm_0.99', 'store_sales_ewm_0.95', 'store_sales_ewm_0.7', 'store_sales_ewm_0.1', 'day', 'month', 'year', 'day_of_week', 'day_of_year', 'name_of_day', 'week_of_year', 'quarter', 'day_of_the_month', 'is_weekend_c', 'is_weekend_j', 'MEST_day_store', 'MEST_day_sku', 'MEST_month_store', 'MEST_month_sku', 'MEST_quarter_store', 'MEST_quarter_sku', 'tavg', 'tmin', 'tmax', 'prcp', 'snow', 'wspd', 'pres', 'is_weekend', 'is_event', 'event_id_list', 'duration_list', 'min_date_list', 'sub_event_id_list', 'is_old_list', 'max_date_list', 'duration_list_mean_event', 'duration_list_median_event', 'duration_list_std_event', 'num_event_id_list', 'num_sub_event_id_list', 'sales_diff', 'event_frequency', 'ind_change_combo_event', 'sales_log', 'amount_of_days_pass_from_start_of_event', 'amount_of_days_pass_from_start_of_event_most_new', 'holiday_name', 'type', 'comments', 'is_holday', 'is_sunday', 'type_holiday_name', 'cumulative_sum_sales', 'fft_real', 'fft_imag', 'skewness', 'kurtosis', 'slope', 'PC1', 'PC2', 'is_tomorrow_event', 'is_2_days_event', 'MEstimateEncoder_of_type_holiday_name', 'MEstimateEncoder_of_num_sub_event_id_list', 'MEstimateEncoder_of_cumulative_sum_sales', 'MEstimateEncoder_of_PC1', 'MEstimateEncoder_of_PC2', 'MEstimateEncoder_of_comments', 'MEstimateEncoder_of_fft_real', 'MEstimateEncoder_of_fft_imag', 'MEstimateEncoder_of_num_event_id_list', 'MEstimateEncoder_of_duration_list_mean_event', 'MEstimateEncoder_of_duration_list_median_event', 'MEstimateEncoder_of_duration_list_std_event', 'MEstimateEncoder_of_is_weekend', 'MEstimateEncoder_of_ind_change_combo_event', 'MEstimateEncoder_of_is_sunday', 'MEstimateEncoder_of_is_tomorrow_event', 'MEstimateEncoder_of_is_2_days_event', 'CatBoostEncoder_of_type_holiday_name', 'CatBoostEncoder_of_num_sub_event_id_list', 'CatBoostEncoder_of_cumulative_sum_sales', 'CatBoostEncoder_of_PC1', 'CatBoostEncoder_of_PC2', 'CatBoostEncoder_of_comments', 'CatBoostEncoder_of_fft_real', 'CatBoostEncoder_of_fft_imag', 'CatBoostEncoder_of_num_event_id_list', 'CatBoostEncoder_of_duration_list_mean_event', 'CatBoostEncoder_of_duration_list_median_event', 'CatBoostEncoder_of_duration_list_std_event', 'CatBoostEncoder_of_is_weekend', 'CatBoostEncoder_of_ind_change_combo_event', 'CatBoostEncoder_of_is_sunday', 'CatBoostEncoder_of_is_tomorrow_event', 'CatBoostEncoder_of_is_2_days_event', 'MEstimateEncoder_of_all_type_holiday_name', 'MEstimateEncoder_of_all_num_sub_event_id_list', 'MEstimateEncoder_of_all_cumulative_sum_sales', 'MEstimateEncoder_of_all_PC1', 'MEstimateEncoder_of_all_PC2', 'MEstimateEncoder_of_all_comments', 'MEstimateEncoder_of_all_fft_real', 'MEstimateEncoder_of_all_fft_imag', 'MEstimateEncoder_of_all_num_event_id_list', 'MEstimateEncoder_of_all_duration_list_mean_event', 'MEstimateEncoder_of_all_duration_list_median_event', 'MEstimateEncoder_of_all_duration_list_std_event', 'MEstimateEncoder_of_all_is_weekend', 'MEstimateEncoder_of_all_ind_change_combo_event', 'MEstimateEncoder_of_all_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event', 'MEstimateEncoder_of_all_is_2_days_event', 'CatBoostEncoder_of_all_type_holiday_name', 'CatBoostEncoder_of_all_num_sub_event_id_list', 'CatBoostEncoder_of_all_cumulative_sum_sales', 'CatBoostEncoder_of_all_PC1', 'CatBoostEncoder_of_all_PC2', 'CatBoostEncoder_of_all_comments', 'CatBoostEncoder_of_all_fft_real', 'CatBoostEncoder_of_all_fft_imag', 'CatBoostEncoder_of_all_num_event_id_list', 'CatBoostEncoder_of_all_duration_list_mean_event', 'CatBoostEncoder_of_all_duration_list_median_event', 'CatBoostEncoder_of_all_duration_list_std_event', 'CatBoostEncoder_of_all_is_weekend', 'CatBoostEncoder_of_all_ind_change_combo_event', 'CatBoostEncoder_of_all_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event', 'CatBoostEncoder_of_all_is_2_days_event', 'num_sub_event_id_list_interactions_day_of_week', 'num_sub_event_id_list_interactions_week_of_year', 'num_sub_event_id_list_interactions_quarter', 'num_sub_event_id_list_interactions_is_weekend', 'num_sub_event_id_list_interactions_ind_change_combo_event', 'num_sub_event_id_list_interactions_is_sunday', 'num_sub_event_id_list_interactions_is_holday', 'num_event_id_list_interactions_day_of_week', 'num_event_id_list_interactions_week_of_year', 'num_event_id_list_interactions_quarter', 'num_event_id_list_interactions_is_weekend', 'num_event_id_list_interactions_ind_change_combo_event', 'num_event_id_list_interactions_is_sunday', 'num_event_id_list_interactions_is_holday', 'PC1_interactions_day_of_week', 'PC1_interactions_week_of_year', 'PC1_interactions_quarter', 'PC1_interactions_is_weekend', 'PC1_interactions_ind_change_combo_event', 'PC1_interactions_is_sunday', 'PC1_interactions_is_holday', 'PC2_interactions_day_of_week', 'PC2_interactions_week_of_year', 'PC2_interactions_quarter', 'PC2_interactions_is_weekend', 'PC2_interactions_ind_change_combo_event', 'PC2_interactions_is_sunday', 'PC2_interactions_is_holday', 'fft_real_interactions_day_of_week', 'fft_real_interactions_week_of_year', 'fft_real_interactions_quarter', 'fft_real_interactions_is_weekend', 'fft_real_interactions_ind_change_combo_event', 'fft_real_interactions_is_sunday', 'fft_real_interactions_is_holday', 'fft_imag_interactions_day_of_week', 'fft_imag_interactions_week_of_year', 'fft_imag_interactions_quarter', 'fft_imag_interactions_is_weekend', 'fft_imag_interactions_ind_change_combo_event', 'fft_imag_interactions_is_sunday', 'fft_imag_interactions_is_holday', 'cumulative_sum_sales_interactions_day_of_week', 'cumulative_sum_sales_interactions_week_of_year', 'cumulative_sum_sales_interactions_quarter', 'cumulative_sum_sales_interactions_is_weekend', 'cumulative_sum_sales_interactions_ind_change_combo_event', 'cumulative_sum_sales_interactions_is_sunday', 'cumulative_sum_sales_interactions_is_holday', 'duration_list_mean_event_interactions_day_of_week', 'duration_list_mean_event_interactions_week_of_year', 'duration_list_mean_event_interactions_quarter', 'duration_list_mean_event_interactions_is_weekend', 'duration_list_mean_event_interactions_ind_change_combo_event', 'duration_list_mean_event_interactions_is_sunday', 'duration_list_mean_event_interactions_is_holday', 'duration_list_std_event_interactions_day_of_week', 'duration_list_std_event_interactions_week_of_year', 'duration_list_std_event_interactions_quarter', 'duration_list_std_event_interactions_is_weekend', 'duration_list_std_event_interactions_ind_change_combo_event', 'duration_list_std_event_interactions_is_sunday', 'duration_list_std_event_interactions_is_holday', 'duration_list_median_event_interactions_day_of_week', 'duration_list_median_event_interactions_week_of_year', 'duration_list_median_event_interactions_quarter', 'duration_list_median_event_interactions_is_weekend', 'duration_list_median_event_interactions_ind_change_combo_event', 'duration_list_median_event_interactions_is_sunday', 'duration_list_median_event_interactions_is_holday', 'is_tomorrow_event_interactions_day_of_week', 'is_tomorrow_event_interactions_week_of_year', 'is_tomorrow_event_interactions_quarter', 'is_tomorrow_event_interactions_is_weekend', 'is_tomorrow_event_interactions_ind_change_combo_event', 'is_tomorrow_event_interactions_is_sunday', 'is_tomorrow_event_interactions_is_holday', 'is_2_days_event_interactions_day_of_week', 'is_2_days_event_interactions_week_of_year', 'is_2_days_event_interactions_quarter', 'is_2_days_event_interactions_is_weekend', 'is_2_days_event_interactions_ind_change_combo_event', 'is_2_days_event_interactions_is_sunday', 'is_2_days_event_interactions_is_holday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_PC1_interactions_day_of_week', 'MEstimateEncoder_of_all_PC1_interactions_week_of_year', 'MEstimateEncoder_of_all_PC1_interactions_quarter', 'MEstimateEncoder_of_all_PC1_interactions_is_weekend', 'MEstimateEncoder_of_all_PC1_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC1_interactions_is_sunday', 'MEstimateEncoder_of_all_PC1_interactions_is_holday', 'MEstimateEncoder_of_all_PC2_interactions_day_of_week', 'MEstimateEncoder_of_all_PC2_interactions_week_of_year', 'MEstimateEncoder_of_all_PC2_interactions_quarter', 'MEstimateEncoder_of_all_PC2_interactions_is_weekend', 'MEstimateEncoder_of_all_PC2_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC2_interactions_is_sunday', 'MEstimateEncoder_of_all_PC2_interactions_is_holday', 'MEstimateEncoder_of_all_fft_real_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_real_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_real_interactions_quarter', 'MEstimateEncoder_of_all_fft_real_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_real_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_real_interactions_is_holday', 'MEstimateEncoder_of_all_fft_imag_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_imag_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_imag_interactions_quarter', 'MEstimateEncoder_of_all_fft_imag_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_imag_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_imag_interactions_is_holday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_quarter', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_2_days_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_2_days_event_interactions_quarter', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_holday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_PC1_interactions_day_of_week', 'CatBoostEncoder_of_all_PC1_interactions_week_of_year', 'CatBoostEncoder_of_all_PC1_interactions_quarter', 'CatBoostEncoder_of_all_PC1_interactions_is_weekend', 'CatBoostEncoder_of_all_PC1_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC1_interactions_is_sunday', 'CatBoostEncoder_of_all_PC1_interactions_is_holday', 'CatBoostEncoder_of_all_PC2_interactions_day_of_week', 'CatBoostEncoder_of_all_PC2_interactions_week_of_year', 'CatBoostEncoder_of_all_PC2_interactions_quarter', 'CatBoostEncoder_of_all_PC2_interactions_is_weekend', 'CatBoostEncoder_of_all_PC2_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC2_interactions_is_sunday', 'CatBoostEncoder_of_all_PC2_interactions_is_holday', 'CatBoostEncoder_of_all_fft_real_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_real_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_real_interactions_quarter', 'CatBoostEncoder_of_all_fft_real_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_real_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_real_interactions_is_holday', 'CatBoostEncoder_of_all_fft_imag_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_imag_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_imag_interactions_quarter', 'CatBoostEncoder_of_all_fft_imag_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_imag_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_imag_interactions_is_holday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_quarter', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_2_days_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_2_days_event_interactions_quarter', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_holday', 'Palmers Week', 'Maria Galland', 'Black Weekend', 'Cyber Monday', 'Valentine', 'Bride', 'Frühling', 'Ostern', 'Muttertag', 'Vatertag', 'Glamour Week', 'Palmers x Marina Hoermanseder', 'Palmers x Lenzing', 'Black  Week', 'Osterpromotion PALMERS Münz-Ei', 'Woman’s Day', '20% auf alle Herrenartikel', 'WOMAN SOMMER SHOPPING', 'Palmers Münze 50+10', '- 20% auf Strümpfe Shade', 'ab 80€ Einkauf', 'Palmers Münze 100+10', 'Kampagne Bademode', '20€ geschenkt', 'SHADE Promotion', '10€ Palmers Münze geschenkt', 'CLUB PROMO', 'WELTFRAUENTAG', '2+1 STRUMPFKATION', 'Muttertag Münze 100+10', '20€ geschenkt Palmers Club', 'FINAL SALE WITH NUM', 'FINAL SALE', 'MID SEASON SALE', 'PALMERS CLUB SALE', 'lag_-1_Palmers Week', 'lag_-1_Maria Galland', 'lag_-1_Black Weekend', 'lag_-1_Cyber Monday', 'lag_-1_Valentine', 'lag_-1_Bride', 'lag_-1_Frühling', 'lag_-1_Ostern', 'lag_-1_Muttertag', 'lag_-1_Vatertag', 'lag_-1_Glamour Week', 'lag_-1_Palmers x Marina Hoermanseder', 'lag_-1_Palmers x Lenzing', 'lag_-1_Black  Week', 'lag_-1_Osterpromotion PALMERS Münz-Ei', 'lag_-1_Woman’s Day', 'lag_-1_20% auf alle Herrenartikel', 'lag_-1_WOMAN SOMMER SHOPPING', 'lag_-1_Palmers Münze 50+10', 'lag_-1_- 20% auf Strümpfe Shade', 'lag_-1_ab 80€ Einkauf', 'lag_-1_Palmers Münze 100+10', 'lag_-1_Kampagne Bademode', 'lag_-1_20€ geschenkt', 'lag_-1_SHADE Promotion', 'lag_-1_10€ Palmers Münze geschenkt', 'lag_-1_CLUB PROMO', 'lag_-1_WELTFRAUENTAG', 'lag_-1_2+1 STRUMPFKATION', 'lag_-1_Muttertag Münze 100+10', 'lag_-1_20€ geschenkt Palmers Club', 'lag_-1_FINAL SALE WITH NUM', 'lag_-1_FINAL SALE', 'lag_-1_MID SEASON SALE', 'lag_-1_PALMERS CLUB SALE', 'lag_-2_Palmers Week', 'lag_-2_Maria Galland', 'lag_-2_Black Weekend', 'lag_-2_Cyber Monday', 'lag_-2_Valentine', 'lag_-2_Bride', 'lag_-2_Frühling', 'lag_-2_Ostern', 'lag_-2_Muttertag', 'lag_-2_Vatertag', 'lag_-2_Glamour Week', 'lag_-2_Palmers x Marina Hoermanseder', 'lag_-2_Palmers x Lenzing', 'lag_-2_Black  Week', 'lag_-2_Osterpromotion PALMERS Münz-Ei', 'lag_-2_Woman’s Day', 'lag_-2_20% auf alle Herrenartikel', 'lag_-2_WOMAN SOMMER SHOPPING', 'lag_-2_Palmers Münze 50+10', 'lag_-2_- 20% auf Strümpfe Shade', 'lag_-2_ab 80€ Einkauf', 'lag_-2_Palmers Münze 100+10', 'lag_-2_Kampagne Bademode', 'lag_-2_20€ geschenkt', 'lag_-2_SHADE Promotion', 'lag_-2_10€ Palmers Münze geschenkt', 'lag_-2_CLUB PROMO', 'lag_-2_WELTFRAUENTAG', 'lag_-2_2+1 STRUMPFKATION', 'lag_-2_Muttertag Münze 100+10', 'lag_-2_20€ geschenkt Palmers Club', 'lag_-2_FINAL SALE WITH NUM', 'lag_-2_FINAL SALE', 'lag_-2_MID SEASON SALE', 'lag_-2_PALMERS CLUB SALE', 'sales_cumulative_store_sku_D', 'sales_cumulative_store_sku_W-Mon', 'sales_cumulative_store_sku_M', 'sales_cumulative_store_sku_Y', 'sales_expected_store_sku_D', 'sales_expected_store_sku_W-Mon', 'sales_expected_store_sku_M', 'sales_expected_store_sku_Y']
+some_columns = ['date', 'sales', 'id_sales_lag_1', 'id_sales_lag_2', 'id_sales_lag_3', 'id_sales_lag_4', 'id_sales_lag_5', 'id_sales_lag_6', 'id_sales_lag_7', 'id_sales_lag_12', 'id_sales_lag_14', 'id_sales_lag_18', 'id_sales_lag_21', 'id_sales_lag_24', 'id_sales_lag_312', 'id_sales_lag_313', 'id_sales_lag_364', 'id_sales_lag_365', 'id_sales_rolling_1', 'id_sales_rolling_2', 'id_sales_rolling_3', 'id_sales_rolling_4', 'id_sales_rolling_5', 'id_sales_rolling_6', 'id_sales_rolling_7', 'id_sales_rolling_12', 'id_sales_rolling_14', 'id_sales_rolling_18', 'id_sales_rolling_21', 'id_sales_rolling_24', 'id_sales_rolling_312', 'id_sales_rolling_313', 'id_sales_rolling_364', 'id_sales_rolling_365', 'id_sales_diff_1', 'id_sales_diff_2', 'id_sales_diff_3', 'id_sales_diff_4', 'id_sales_diff_5', 'id_sales_diff_6', 'id_sales_diff_7', 'id_sales_diff_12', 'id_sales_diff_14', 'id_sales_diff_18', 'id_sales_diff_21', 'id_sales_diff_24', 'id_sales_diff_312', 'id_sales_diff_313', 'id_sales_diff_364', 'id_sales_diff_365', 'id_sales_ewm_0.99', 'id_sales_ewm_0.95', 'id_sales_ewm_0.7', 'id_sales_ewm_0.1', 'sku', 'store', 'sku, store', 'year', 'month', 'day', 'day_of_week', 'week_of_year', 'quarter', 'is_weekend', 'day_of_year', 'day_of_the_month', 'is_weekend_c', 'is_weekend_j', 'Palmers Week', 'Maria Galland', 'Black Weekend', 'Cyber Monday', 'Valentine', 'Bride', 'Frühling', 'Ostern', 'Muttertag', 'Vatertag', 'Glamour Week', 'Palmers x Marina Hoermanseder', 'Palmers x Lenzing', 'Black  Week', 'Osterpromotion PALMERS Münz-Ei', 'Woman’s Day', '20% auf alle Herrenartikel', 'WOMAN SOMMER SHOPPING', 'Palmers Münze 50+10', '- 20% auf Strümpfe Shade', 'ab 80€ Einkauf', 'Palmers Münze 100+10', 'Kampagne Bademode', '20€ geschenkt', 'SHADE Promotion', '10€ Palmers Münze geschenkt', 'CLUB PROMO', 'WELTFRAUENTAG', '2+1 STRUMPFKATION', 'Muttertag Münze 100+10', '20€ geschenkt Palmers Club', 'FINAL SALE WITH NUM', 'FINAL SALE', 'MID SEASON SALE', 'PALMERS CLUB SALE', 'lag_-1_Palmers Week', 'lag_-1_Maria Galland', 'lag_-1_Black Weekend', 'lag_-1_Cyber Monday', 'lag_-1_Valentine', 'lag_-1_Bride', 'lag_-1_Frühling', 'lag_-1_Ostern', 'lag_-1_Muttertag', 'lag_-1_Vatertag', 'lag_-1_Glamour Week', 'lag_-1_Palmers x Marina Hoermanseder', 'lag_-1_Palmers x Lenzing', 'lag_-1_Black  Week', 'lag_-1_Osterpromotion PALMERS Münz-Ei', 'lag_-1_Woman’s Day', 'lag_-1_20% auf alle Herrenartikel', 'lag_-1_WOMAN SOMMER SHOPPING', 'lag_-1_Palmers Münze 50+10', 'lag_-1_- 20% auf Strümpfe Shade', 'lag_-1_ab 80€ Einkauf', 'lag_-1_Palmers Münze 100+10', 'lag_-1_Kampagne Bademode', 'lag_-1_20€ geschenkt', 'lag_-1_SHADE Promotion', 'lag_-1_10€ Palmers Münze geschenkt', 'lag_-1_CLUB PROMO', 'lag_-1_WELTFRAUENTAG', 'lag_-1_2+1 STRUMPFKATION', 'lag_-1_Muttertag Münze 100+10', 'lag_-1_20€ geschenkt Palmers Club', 'lag_-1_FINAL SALE WITH NUM', 'lag_-1_FINAL SALE', 'lag_-1_MID SEASON SALE', 'lag_-1_PALMERS CLUB SALE', 'lag_-2_Palmers Week', 'lag_-2_Maria Galland', 'lag_-2_Black Weekend', 'lag_-2_Cyber Monday', 'lag_-2_Valentine', 'lag_-2_Bride', 'lag_-2_Frühling', 'lag_-2_Ostern', 'lag_-2_Muttertag', 'lag_-2_Vatertag', 'lag_-2_Glamour Week', 'lag_-2_Palmers x Marina Hoermanseder', 'lag_-2_Palmers x Lenzing', 'lag_-2_Black  Week', 'lag_-2_Osterpromotion PALMERS Münz-Ei', 'lag_-2_Woman’s Day', 'lag_-2_20% auf alle Herrenartikel', 'lag_-2_WOMAN SOMMER SHOPPING', 'lag_-2_Palmers Münze 50+10', 'lag_-2_- 20% auf Strümpfe Shade', 'lag_-2_ab 80€ Einkauf', 'lag_-2_Palmers Münze 100+10', 'lag_-2_Kampagne Bademode', 'lag_-2_20€ geschenkt', 'lag_-2_SHADE Promotion', 'lag_-2_10€ Palmers Münze geschenkt', 'lag_-2_CLUB PROMO', 'lag_-2_WELTFRAUENTAG', 'lag_-2_2+1 STRUMPFKATION', 'lag_-2_Muttertag Münze 100+10', 'lag_-2_20€ geschenkt Palmers Club', 'lag_-2_FINAL SALE WITH NUM', 'lag_-2_FINAL SALE', 'lag_-2_MID SEASON SALE', 'lag_-2_PALMERS CLUB SALE', 'MEST_day_store', 'MEST_day_sku', 'MEST_month_store', 'MEST_month_sku', 'MEST_quarter_store', 'MEST_quarter_sku', 'store_sales_lag_1', 'store_sales_lag_2', 'store_sales_lag_3', 'store_sales_lag_4', 'store_sales_lag_5', 'store_sales_lag_6', 'store_sales_lag_7', 'store_sales_lag_12', 'store_sales_lag_14', 'store_sales_lag_18', 'store_sales_lag_21', 'store_sales_lag_24', 'store_sales_lag_312', 'store_sales_lag_313', 'store_sales_lag_364', 'store_sales_lag_365', 'store_sales_rolling_1', 'store_sales_rolling_2', 'store_sales_rolling_3', 'store_sales_rolling_4', 'store_sales_rolling_5', 'store_sales_rolling_6', 'store_sales_rolling_7', 'store_sales_rolling_12', 'store_sales_rolling_14', 'store_sales_rolling_18', 'store_sales_rolling_21', 'store_sales_rolling_24', 'store_sales_rolling_312', 'store_sales_rolling_313', 'store_sales_rolling_364', 'store_sales_rolling_365', 'store_sales_diff_1', 'store_sales_diff_2', 'store_sales_diff_3', 'store_sales_diff_4', 'store_sales_diff_5', 'store_sales_diff_6', 'store_sales_diff_7', 'store_sales_diff_12', 'store_sales_diff_14', 'store_sales_diff_18', 'store_sales_diff_21', 'store_sales_diff_24', 'store_sales_diff_312', 'store_sales_diff_313', 'store_sales_diff_364', 'store_sales_diff_365', 'store_sales_ewm_0.99', 'store_sales_ewm_0.95', 'store_sales_ewm_0.7', 'store_sales_ewm_0.1', 'tavg', 'tmin', 'tmax', 'prcp', 'snow', 'wspd', 'pres', 'sales_cumulative_store_sku_D', 'sales_cumulative_store_sku_W-Mon', 'sales_cumulative_store_sku_M', 'sales_cumulative_store_sku_Y', 'sales_expected_store_sku_D', 'sales_expected_store_sku_W-Mon', 'sales_expected_store_sku_M', 'sales_expected_store_sku_Y', 'sku_sales_lag_1', 'sku_sales_lag_2', 'sku_sales_lag_3', 'sku_sales_lag_4', 'sku_sales_lag_5', 'sku_sales_lag_6', 'sku_sales_lag_7', 'sku_sales_lag_12', 'sku_sales_lag_14', 'sku_sales_lag_18', 'sku_sales_lag_21', 'sku_sales_lag_24', 'sku_sales_lag_312', 'sku_sales_lag_313', 'sku_sales_lag_364', 'sku_sales_lag_365', 'sku_sales_rolling_1', 'sku_sales_rolling_2', 'sku_sales_rolling_3', 'sku_sales_rolling_4', 'sku_sales_rolling_5', 'sku_sales_rolling_6', 'sku_sales_rolling_7', 'sku_sales_rolling_12', 'sku_sales_rolling_14', 'sku_sales_rolling_18', 'sku_sales_rolling_21', 'sku_sales_rolling_24', 'sku_sales_rolling_312', 'sku_sales_rolling_313', 'sku_sales_rolling_364', 'sku_sales_rolling_365', 'sku_sales_diff_1', 'sku_sales_diff_2', 'sku_sales_diff_3', 'sku_sales_diff_4', 'sku_sales_diff_5', 'sku_sales_diff_6', 'sku_sales_diff_7', 'sku_sales_diff_12', 'sku_sales_diff_14', 'sku_sales_diff_18', 'sku_sales_diff_21', 'sku_sales_diff_24', 'sku_sales_diff_312', 'sku_sales_diff_313', 'sku_sales_diff_364', 'sku_sales_diff_365', 'sku_sales_ewm_0.99', 'sku_sales_ewm_0.95', 'sku_sales_ewm_0.7', 'sku_sales_ewm_0.1', 'is_event', 'event_id_list', 'duration_list', 'min_date_list', 'sub_event_id_list', 'is_old_list', 'max_date_list', 'duration_list_mean_event', 'duration_list_median_event', 'duration_list_std_event', 'num_event_id_list', 'num_sub_event_id_list', 'sales_diff', 'event_frequency', 'ind_change_combo_event', 'sales_log', 'amount_of_days_pass_from_start_of_event', 'amount_of_days_pass_from_start_of_event_most_new', 'holiday_name', 'type', 'comments', 'is_holday', 'is_sunday', 'type_holiday_name', 'cumulative_sum_sales', 'fft_real', 'fft_imag', 'skewness', 'kurtosis', 'slope', 'is_tomorrow_event', 'is_2_days_event', 'PC1', 'PC2', 'MEstimateEncoder_of_type_holiday_name', 'MEstimateEncoder_of_num_sub_event_id_list', 'MEstimateEncoder_of_cumulative_sum_sales', 'MEstimateEncoder_of_PC1', 'MEstimateEncoder_of_PC2', 'MEstimateEncoder_of_comments', 'MEstimateEncoder_of_fft_real', 'MEstimateEncoder_of_fft_imag', 'MEstimateEncoder_of_num_event_id_list', 'MEstimateEncoder_of_duration_list_mean_event', 'MEstimateEncoder_of_duration_list_median_event', 'MEstimateEncoder_of_duration_list_std_event', 'MEstimateEncoder_of_is_weekend', 'MEstimateEncoder_of_ind_change_combo_event', 'MEstimateEncoder_of_is_sunday', 'MEstimateEncoder_of_is_tomorrow_event', 'MEstimateEncoder_of_is_2_days_event', 'CatBoostEncoder_of_type_holiday_name', 'CatBoostEncoder_of_num_sub_event_id_list', 'CatBoostEncoder_of_cumulative_sum_sales', 'CatBoostEncoder_of_PC1', 'CatBoostEncoder_of_PC2', 'CatBoostEncoder_of_comments', 'CatBoostEncoder_of_fft_real', 'CatBoostEncoder_of_fft_imag', 'CatBoostEncoder_of_num_event_id_list', 'CatBoostEncoder_of_duration_list_mean_event', 'CatBoostEncoder_of_duration_list_median_event', 'CatBoostEncoder_of_duration_list_std_event', 'CatBoostEncoder_of_is_weekend', 'CatBoostEncoder_of_ind_change_combo_event', 'CatBoostEncoder_of_is_sunday', 'CatBoostEncoder_of_is_tomorrow_event', 'CatBoostEncoder_of_is_2_days_event', 'MEstimateEncoder_of_all_type_holiday_name', 'MEstimateEncoder_of_all_num_sub_event_id_list', 'MEstimateEncoder_of_all_cumulative_sum_sales', 'MEstimateEncoder_of_all_PC1', 'MEstimateEncoder_of_all_PC2', 'MEstimateEncoder_of_all_comments', 'MEstimateEncoder_of_all_fft_real', 'MEstimateEncoder_of_all_fft_imag', 'MEstimateEncoder_of_all_num_event_id_list', 'MEstimateEncoder_of_all_duration_list_mean_event', 'MEstimateEncoder_of_all_duration_list_median_event', 'MEstimateEncoder_of_all_duration_list_std_event', 'MEstimateEncoder_of_all_is_weekend', 'MEstimateEncoder_of_all_ind_change_combo_event', 'MEstimateEncoder_of_all_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event', 'MEstimateEncoder_of_all_is_2_days_event', 'CatBoostEncoder_of_all_type_holiday_name', 'CatBoostEncoder_of_all_num_sub_event_id_list', 'CatBoostEncoder_of_all_cumulative_sum_sales', 'CatBoostEncoder_of_all_PC1', 'CatBoostEncoder_of_all_PC2', 'CatBoostEncoder_of_all_comments', 'CatBoostEncoder_of_all_fft_real', 'CatBoostEncoder_of_all_fft_imag', 'CatBoostEncoder_of_all_num_event_id_list', 'CatBoostEncoder_of_all_duration_list_mean_event', 'CatBoostEncoder_of_all_duration_list_median_event', 'CatBoostEncoder_of_all_duration_list_std_event', 'CatBoostEncoder_of_all_is_weekend', 'CatBoostEncoder_of_all_ind_change_combo_event', 'CatBoostEncoder_of_all_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event', 'CatBoostEncoder_of_all_is_2_days_event', 'num_sub_event_id_list_interactions_day_of_week', 'num_sub_event_id_list_interactions_week_of_year', 'num_sub_event_id_list_interactions_quarter', 'num_sub_event_id_list_interactions_is_weekend', 'num_sub_event_id_list_interactions_ind_change_combo_event', 'num_sub_event_id_list_interactions_is_sunday', 'num_sub_event_id_list_interactions_is_holday', 'num_event_id_list_interactions_day_of_week', 'num_event_id_list_interactions_week_of_year', 'num_event_id_list_interactions_quarter', 'num_event_id_list_interactions_is_weekend', 'num_event_id_list_interactions_ind_change_combo_event', 'num_event_id_list_interactions_is_sunday', 'num_event_id_list_interactions_is_holday', 'PC1_interactions_day_of_week', 'PC1_interactions_week_of_year', 'PC1_interactions_quarter', 'PC1_interactions_is_weekend', 'PC1_interactions_ind_change_combo_event', 'PC1_interactions_is_sunday', 'PC1_interactions_is_holday', 'PC2_interactions_day_of_week', 'PC2_interactions_week_of_year', 'PC2_interactions_quarter', 'PC2_interactions_is_weekend', 'PC2_interactions_ind_change_combo_event', 'PC2_interactions_is_sunday', 'PC2_interactions_is_holday', 'fft_real_interactions_day_of_week', 'fft_real_interactions_week_of_year', 'fft_real_interactions_quarter', 'fft_real_interactions_is_weekend', 'fft_real_interactions_ind_change_combo_event', 'fft_real_interactions_is_sunday', 'fft_real_interactions_is_holday', 'fft_imag_interactions_day_of_week', 'fft_imag_interactions_week_of_year', 'fft_imag_interactions_quarter', 'fft_imag_interactions_is_weekend', 'fft_imag_interactions_ind_change_combo_event', 'fft_imag_interactions_is_sunday', 'fft_imag_interactions_is_holday', 'cumulative_sum_sales_interactions_day_of_week', 'cumulative_sum_sales_interactions_week_of_year', 'cumulative_sum_sales_interactions_quarter', 'cumulative_sum_sales_interactions_is_weekend', 'cumulative_sum_sales_interactions_ind_change_combo_event', 'cumulative_sum_sales_interactions_is_sunday', 'cumulative_sum_sales_interactions_is_holday', 'duration_list_mean_event_interactions_day_of_week', 'duration_list_mean_event_interactions_week_of_year', 'duration_list_mean_event_interactions_quarter', 'duration_list_mean_event_interactions_is_weekend', 'duration_list_mean_event_interactions_ind_change_combo_event', 'duration_list_mean_event_interactions_is_sunday', 'duration_list_mean_event_interactions_is_holday', 'duration_list_std_event_interactions_day_of_week', 'duration_list_std_event_interactions_week_of_year', 'duration_list_std_event_interactions_quarter', 'duration_list_std_event_interactions_is_weekend', 'duration_list_std_event_interactions_ind_change_combo_event', 'duration_list_std_event_interactions_is_sunday', 'duration_list_std_event_interactions_is_holday', 'duration_list_median_event_interactions_day_of_week', 'duration_list_median_event_interactions_week_of_year', 'duration_list_median_event_interactions_quarter', 'duration_list_median_event_interactions_is_weekend', 'duration_list_median_event_interactions_ind_change_combo_event', 'duration_list_median_event_interactions_is_sunday', 'duration_list_median_event_interactions_is_holday', 'is_tomorrow_event_interactions_day_of_week', 'is_tomorrow_event_interactions_week_of_year', 'is_tomorrow_event_interactions_quarter', 'is_tomorrow_event_interactions_is_weekend', 'is_tomorrow_event_interactions_ind_change_combo_event', 'is_tomorrow_event_interactions_is_sunday', 'is_tomorrow_event_interactions_is_holday', 'is_2_days_event_interactions_day_of_week', 'is_2_days_event_interactions_week_of_year', 'is_2_days_event_interactions_quarter', 'is_2_days_event_interactions_is_weekend', 'is_2_days_event_interactions_ind_change_combo_event', 'is_2_days_event_interactions_is_sunday', 'is_2_days_event_interactions_is_holday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_day_of_week', 'MEstimateEncoder_of_all_num_event_id_list_interactions_week_of_year', 'MEstimateEncoder_of_all_num_event_id_list_interactions_quarter', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_weekend', 'MEstimateEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_sunday', 'MEstimateEncoder_of_all_num_event_id_list_interactions_is_holday', 'MEstimateEncoder_of_all_PC1_interactions_day_of_week', 'MEstimateEncoder_of_all_PC1_interactions_week_of_year', 'MEstimateEncoder_of_all_PC1_interactions_quarter', 'MEstimateEncoder_of_all_PC1_interactions_is_weekend', 'MEstimateEncoder_of_all_PC1_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC1_interactions_is_sunday', 'MEstimateEncoder_of_all_PC1_interactions_is_holday', 'MEstimateEncoder_of_all_PC2_interactions_day_of_week', 'MEstimateEncoder_of_all_PC2_interactions_week_of_year', 'MEstimateEncoder_of_all_PC2_interactions_quarter', 'MEstimateEncoder_of_all_PC2_interactions_is_weekend', 'MEstimateEncoder_of_all_PC2_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_PC2_interactions_is_sunday', 'MEstimateEncoder_of_all_PC2_interactions_is_holday', 'MEstimateEncoder_of_all_fft_real_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_real_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_real_interactions_quarter', 'MEstimateEncoder_of_all_fft_real_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_real_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_real_interactions_is_holday', 'MEstimateEncoder_of_all_fft_imag_interactions_day_of_week', 'MEstimateEncoder_of_all_fft_imag_interactions_week_of_year', 'MEstimateEncoder_of_all_fft_imag_interactions_quarter', 'MEstimateEncoder_of_all_fft_imag_interactions_is_weekend', 'MEstimateEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_fft_imag_interactions_is_sunday', 'MEstimateEncoder_of_all_fft_imag_interactions_is_holday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'MEstimateEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_std_event_interactions_is_holday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_quarter', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'MEstimateEncoder_of_all_duration_list_median_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_quarter', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_day_of_week', 'MEstimateEncoder_of_all_is_2_days_event_interactions_week_of_year', 'MEstimateEncoder_of_all_is_2_days_event_interactions_quarter', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_weekend', 'MEstimateEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_sunday', 'MEstimateEncoder_of_all_is_2_days_event_interactions_is_holday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_sub_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_day_of_week', 'CatBoostEncoder_of_all_num_event_id_list_interactions_week_of_year', 'CatBoostEncoder_of_all_num_event_id_list_interactions_quarter', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_weekend', 'CatBoostEncoder_of_all_num_event_id_list_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_sunday', 'CatBoostEncoder_of_all_num_event_id_list_interactions_is_holday', 'CatBoostEncoder_of_all_PC1_interactions_day_of_week', 'CatBoostEncoder_of_all_PC1_interactions_week_of_year', 'CatBoostEncoder_of_all_PC1_interactions_quarter', 'CatBoostEncoder_of_all_PC1_interactions_is_weekend', 'CatBoostEncoder_of_all_PC1_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC1_interactions_is_sunday', 'CatBoostEncoder_of_all_PC1_interactions_is_holday', 'CatBoostEncoder_of_all_PC2_interactions_day_of_week', 'CatBoostEncoder_of_all_PC2_interactions_week_of_year', 'CatBoostEncoder_of_all_PC2_interactions_quarter', 'CatBoostEncoder_of_all_PC2_interactions_is_weekend', 'CatBoostEncoder_of_all_PC2_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_PC2_interactions_is_sunday', 'CatBoostEncoder_of_all_PC2_interactions_is_holday', 'CatBoostEncoder_of_all_fft_real_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_real_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_real_interactions_quarter', 'CatBoostEncoder_of_all_fft_real_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_real_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_real_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_real_interactions_is_holday', 'CatBoostEncoder_of_all_fft_imag_interactions_day_of_week', 'CatBoostEncoder_of_all_fft_imag_interactions_week_of_year', 'CatBoostEncoder_of_all_fft_imag_interactions_quarter', 'CatBoostEncoder_of_all_fft_imag_interactions_is_weekend', 'CatBoostEncoder_of_all_fft_imag_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_fft_imag_interactions_is_sunday', 'CatBoostEncoder_of_all_fft_imag_interactions_is_holday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_day_of_week', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_week_of_year', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_quarter', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_weekend', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_sunday', 'CatBoostEncoder_of_all_cumulative_sum_sales_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_mean_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_std_event_interactions_is_holday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_day_of_week', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_week_of_year', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_quarter', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_weekend', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_sunday', 'CatBoostEncoder_of_all_duration_list_median_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_quarter', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_tomorrow_event_interactions_is_holday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_day_of_week', 'CatBoostEncoder_of_all_is_2_days_event_interactions_week_of_year', 'CatBoostEncoder_of_all_is_2_days_event_interactions_quarter', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_weekend', 'CatBoostEncoder_of_all_is_2_days_event_interactions_ind_change_combo_event', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_sunday', 'CatBoostEncoder_of_all_is_2_days_event_interactions_is_holday']
+
+
+
+
+def func(list1, list2):
+    not_in_list1 = set(list2).difference(list1)
+    print("Values not in list1 but in list2:", not_in_list1)
+    # find values not in list2 but in list1
+    not_in_list2 = set(list1).difference(list2)
+    print("Values not in list2 but in list1:", not_in_list2)
+
+
 func(all_columns, some_columns)
```

### Comparing `palmers_preprocess-0.0.8/src/palmers_preprocessing/tests/weather_test.py` & `palmers_preprocess-0.0.9/src/palmers_preprocessing/tests/weather_test.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import sys
-sys.path.append('../..')
-from src.palmers_preprocessing.features.weather_features import WeatherFeatureGenerator, StoreLocationLoader
-
-
-def test_weather_feature_generator():
-    store_location_df = StoreLocationLoader.load()
-    print(WeatherFeatureGenerator.load(store_location_df, store_id=100, start_date='2023-01-01', end_date='2023-01-01'))
-    print(WeatherFeatureGenerator.load(store_location_df, store_id=109, start_date='2023-04-25', end_date='2023-05-25'))
-
-
-
-
-def test_store_location_df():
-    store_location_df = StoreLocationLoader.load()
-    print(store_location_df)
-    print(store_location_df.columns)
-
-#test_store_location_df()
-test_weather_feature_generator()
+import sys
+sys.path.append('../..')
+from src.palmers_preprocessing.features.weather_features import WeatherFeatureGenerator, StoreLocationLoader
+
+
+def test_weather_feature_generator():
+    store_location_df = StoreLocationLoader.load()
+    print(WeatherFeatureGenerator.load(store_location_df, store_id=100, start_date='2023-01-01', end_date='2023-01-01'))
+    print(WeatherFeatureGenerator.load(store_location_df, store_id=109, start_date='2023-04-25', end_date='2023-05-25'))
+
+
+
+
+def test_store_location_df():
+    store_location_df = StoreLocationLoader.load()
+    print(store_location_df)
+    print(store_location_df.columns)
+
+#test_store_location_df()
+test_weather_feature_generator()
```

### Comparing `palmers_preprocess-0.0.8/LICENSE` & `palmers_preprocess-0.0.9/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `palmers_preprocess-0.0.8/pyproject.toml` & `palmers_preprocess-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "palmers_preprocess"
-version = "0.0.8"
-authors = [
-  { name="Roy ", email="roy@sdatta.ai" },
-  { name="Assaf", email="assafm@sdatta.ai" },
-  { name="Guy", email="assafm@sdatta.ai" },
-  { name="Oran", email="assafm@sdatta.ai" },
-  { name="Yotam", email="assafm@sdatta.ai" },
-]
-description = "A package to preprocess data for Palmer's project"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-
-[project.urls]
-"Homepage" = "https://github.com/pypa/sampleproject"
-"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "palmers_preprocess"
+version = "0.0.9"
+authors = [
+  { name="Roy ", email="roy@sdatta.ai" },
+  { name="Assaf", email="assafm@sdatta.ai" },
+  { name="Guy", email="assafm@sdatta.ai" },
+  { name="Oran", email="assafm@sdatta.ai" },
+  { name="Yotam", email="assafm@sdatta.ai" },
+]
+description = "A package to preprocess data for Palmer's project"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+
+[project.urls]
+"Homepage" = "https://github.com/pypa/sampleproject"
+"Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `palmers_preprocess-0.0.8/PKG-INFO` & `palmers_preprocess-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_preprocess
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Roy  <roy@sdatta.ai>, Assaf <assafm@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

