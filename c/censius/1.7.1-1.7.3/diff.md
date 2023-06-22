# Comparing `tmp/censius-1.7.1.tar.gz` & `tmp/censius-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "censius-1.7.1.tar", last modified: Tue Jun 13 09:21:13 2023, max compression
+gzip compressed data, was "censius-1.7.3.tar", last modified: Thu Jun 22 09:14:06 2023, max compression
```

## Comparing `censius-1.7.1.tar` & `censius-1.7.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-13 09:21:13.710478 censius-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-13 09:21:10.000000 censius-1.7.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-13 09:21:10.000000 censius-1.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:21:13.710478 censius-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-13 09:21:10.000000 censius-1.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.706478 censius-1.7.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/CensiusParent.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius/ml/
--rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/Dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/Explanation.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/ExplanationType.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/Prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/ml/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/CensiusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/DatasetType.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/ModelType.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/UseCase.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-13 09:21:10.000000 censius-1.7.1/src/censius/nlp/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:21:13.710478 censius-1.7.1/src/censius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 09:21:13.000000 censius-1.7.1/src/censius.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:06.570900 censius-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-22 09:14:06.570900 censius-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-22 09:14:03.000000 censius-1.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 09:14:03.000000 censius-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:14:06.570900 censius-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-22 09:14:03.000000 censius-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:06.570900 censius-1.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:06.570900 censius-1.7.3/src/censius/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/CensiusParent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-22 09:14:04.000000 censius-1.7.3/src/censius/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:06.570900 censius-1.7.3/src/censius/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)    33575 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/Dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/Explanation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/ExplanationType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/Prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14033 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/ml/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:06.570900 censius-1.7.3/src/censius/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/nlp/CensiusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/nlp/DatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/nlp/ModelType.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/nlp/UseCase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/nlp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-22 09:14:03.000000 censius-1.7.3/src/censius/nlp/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:14:06.570900 censius-1.7.3/src/censius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-22 09:14:06.000000 censius-1.7.3/src/censius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-22 09:14:06.000000 censius-1.7.3/src/censius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:14:06.000000 censius-1.7.3/src/censius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 09:14:06.000000 censius-1.7.3/src/censius.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 09:14:06.000000 censius-1.7.3/src/censius.egg-info/top_level.txt
```

### Comparing `censius-1.7.1/PKG-INFO` & `censius-1.7.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.7.1
+Version: 1.7.3
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.7.1/setup.py` & `censius-1.7.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="censius",
-    version="1.7.1",
+    version="1.7.3",
     description="API for Censius",
     long_description=long_description,
     long_description_content_type="text/markdown",
     py_modules=["censius/client"],
     package_dir={"": "src"},
     packages=["censius", "censius.nlp", "censius.ml"],
     install_requires=["requests", "jsonschema", "pandas", "numpy"],
```

### Comparing `censius-1.7.1/src/censius/CensiusParent.py` & `censius-1.7.3/src/censius/CensiusParent.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.1/src/censius/ml/CensiusClient.py` & `censius-1.7.3/src/censius/ml/CensiusClient.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.1/src/censius/ml/constants.py` & `censius-1.7.3/src/censius/ml/constants.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.1/src/censius/ml/schemas.py` & `censius-1.7.3/src/censius/ml/schemas.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.1/src/censius/ml/utils.py` & `censius-1.7.3/src/censius/ml/utils.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.1/src/censius/nlp/CensiusClient.py` & `censius-1.7.3/src/censius/nlp/CensiusClient.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,15 @@
 
                 if response.status_code == 200:
                     dataset_id = response.json()["details"]["datasetId"]
                 else:
                     return response.json()
             else:
                 json_data["dataset_id"] = dataset_id
-                url = LLM_REGISTER_DATASET_URL(
-                    project_id=self.project_id
-                )
+                url = LLM_REGISTER_DATASET_URL(project_id=self.project_id)
                 requests.request(
                     "POST",
                     url,
                     headers=self.get_headers(),
                     data=json.dumps(json_data),
                 )
 
@@ -79,22 +77,26 @@
         if error_flag:
             return msg
 
         model_data = {
             "model_name": kwargs["model_name"],
             "model_type": kwargs["model_type"],
             "use_case": kwargs["use_case"],
+            "dataset_id": kwargs["dataset_id"],
+            "parent_model_id": None,
+            "model_version": 1,
+            "project_id": self.project_id,
+            "status": "processed",
         }
-        dataset_id = kwargs["dataset_id"]
-        parent_model_id = None
 
-        url = LLM_REGISTER_MODEL_URL(self.project_id, dataset_id)
-        model_data["parent_model_id"] = parent_model_id
+        url = LLM_REGISTER_MODEL_URL(self.project_id)
         payload = json.dumps(model_data)
-        response = requests.request("POST", url, headers=self.get_headers(), data=payload)
+        response = requests.request(
+            "POST", url, headers=self.get_headers(), data=payload
+        )
         return response.json()
 
     def log(self, *args, **kwargs):
         error_flag, msg = validate_input(kwargs, log_valid)
         if error_flag:
             return msg
 
@@ -121,15 +123,15 @@
             print("Failed to add logs", response.text)
             return
         return response.json()
 
     def bulk_log(self, *args, **kwargs):
         file_path = kwargs["file"]
         model_id = kwargs["model_id"]
-    
+
         reader = pd.read_csv(file_path, chunksize=BULK_CHUNK_SIZE)
         for i, chunk in enumerate(reader):
             json_data = chunk.to_json(orient="records")
             url = LLM_REGISTER_BULK_LOGS(self.project_id, model_id)
             headers = self.get_headers()
             payload = json.dumps(json_data)
             requests.request("POST", url, headers=headers, data=payload)
```

### Comparing `censius-1.7.1/src/censius/nlp/constants.py` & `censius-1.7.3/src/censius/nlp/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 LLM_REGISTER_DATASET_URL = (
     lambda project_id: f"{GATEWAY_URL}/{project_id}/res/nlp-input-training/frd/v1/llm/register_training_data"
 )
 
 LLM_REGISTER_MODEL_URL = (
-    lambda project_id, dataset_id: f"{GATEWAY_LLM_URL}/{project_id}/{dataset_id}/register_model"
+    lambda project_id: f"{GATEWAY_URL}/{project_id}/res/register_model/frd/api/llm/register_model"
 )
 
 LLM_REGISTER_LOGS = (
     lambda project_id: f"{GATEWAY_URL}/{project_id}/res/nlp-input-logs/frd/v1/llm/register_logs"
 )
 
 BULK_CHUNK_SIZE = 2000
```

### Comparing `censius-1.7.1/src/censius/nlp/schema.py` & `censius-1.7.3/src/censius/nlp/schema.py`

 * *Files identical despite different names*

### Comparing `censius-1.7.1/src/censius.egg-info/PKG-INFO` & `censius-1.7.3/src/censius.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: censius
-Version: 1.7.1
+Version: 1.7.3
 Summary: API for Censius
 Home-page: https://github.com/Censius/censius-logs-python-sdk
 Author: Censius
 Author-email: dev@censius.ai
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `censius-1.7.1/src/censius.egg-info/SOURCES.txt` & `censius-1.7.3/src/censius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

