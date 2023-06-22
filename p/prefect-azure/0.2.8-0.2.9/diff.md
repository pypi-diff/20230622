# Comparing `tmp/prefect-azure-0.2.8.tar.gz` & `tmp/prefect-azure-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-bwbm0f6n/prefect-azure-0.2.8.tar", last modified: Thu Jun 15 14:49:58 2023, max compression
+gzip compressed data, was "/home/runner/work/prefect-azure/prefect-azure/dist/.tmp-un4_1p6m/prefect-azure-0.2.9.tar", last modified: Wed Jun 21 17:47:51 2023, max compression
```

## Comparing `prefect-azure-0.2.8.tar` & `prefect-azure-0.2.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32951 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/deployments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/ml_datastore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure/workers/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38423 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/prefect_azure/workers/container_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/prefect_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:49:58.000000 prefect-azure-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_aci_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)    37898 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_aci_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/tests/test_ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-15 14:48:12.000000 prefect-azure-0.2.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7027 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32951 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure/deployments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9879 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/ml_datastore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure/workers/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38409 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/prefect_azure/workers/container_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8040 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/prefect_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:47:51.000000 prefect-azure-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    31858 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/tests/test_aci_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37884 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/tests/test_aci_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/tests/test_cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/tests/test_ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80049 2023-06-21 17:46:03.000000 prefect-azure-0.2.9/versioneer.py
```

### Comparing `prefect-azure-0.2.8/LICENSE` & `prefect-azure-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/PKG-INFO` & `prefect-azure-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prefect integrations with Microsoft Azure services
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-azure-0.2.8/README.md` & `prefect-azure-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/__init__.py` & `prefect-azure-0.2.9/prefect_azure/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/blob_storage.py` & `prefect-azure-0.2.9/prefect_azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/container_instance.py` & `prefect-azure-0.2.9/prefect_azure/container_instance.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/cosmos_db.py` & `prefect-azure-0.2.9/prefect_azure/cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/credentials.py` & `prefect-azure-0.2.9/prefect_azure/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/deployments/steps.py` & `prefect-azure-0.2.9/prefect_azure/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/ml_datastore.py` & `prefect-azure-0.2.9/prefect_azure/ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/prefect_azure/workers/container_instance.py` & `prefect-azure-0.2.9/prefect_azure/workers/container_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
         """
         Add identities to the container group.
 
         Args:
             identities: A list of user-assigned identities to add to
             the container group.
         """
-        self.arm_template["resources"][0]["properties"]["identity"] = {
+        self.arm_template["resources"][0]["identity"] = {
             "type": "UserAssigned",
             "userAssignedIdentities": {
                 # note: For user-assigned identities, the key is the resource ID
                 # of the identity and the value is an empty object. See:
                 # https://docs.microsoft.com/en-us/azure/templates/microsoft.containerinstance/containergroups?tabs=bicep#identity-object # noqa
                 identity: {}
                 for identity in identities
```

### Comparing `prefect-azure-0.2.8/prefect_azure.egg-info/PKG-INFO` & `prefect-azure-0.2.9/prefect_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prefect integrations with Microsoft Azure services
 Home-page: https://github.com/PrefectHQ/prefect-azure
 Author: Prefect Technologies, Inc.
 Author-email: help@prefect.io
 License: Apache License 2.0
 Keywords: prefect
 Classifier: Natural Language :: English
```

### Comparing `prefect-azure-0.2.8/prefect_azure.egg-info/SOURCES.txt` & `prefect-azure-0.2.9/prefect_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/setup.cfg` & `prefect-azure-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/setup.py` & `prefect-azure-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/tests/test_aci_infrastructure.py` & `prefect-azure-0.2.9/tests/test_aci_infrastructure.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/tests/test_aci_worker.py` & `prefect-azure-0.2.9/tests/test_aci_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,15 +963,15 @@
 async def test_add_identities(
     raw_job_configuration, worker_flow_run, mock_aci_client, monkeypatch
 ):
     raw_job_configuration.identities = ["identity1", "identity2", "identity3"]
     raw_job_configuration.prepare_for_flow_run(worker_flow_run)
 
     container_group = raw_job_configuration.arm_template["resources"][0]
-    identities = container_group["properties"]["identity"]["userAssignedIdentities"]
+    identities = container_group["identity"]["userAssignedIdentities"]
     assert len(identities) == 3
     # each of the identities in the input list should be the key of one of the
     # entries in the identities dict. The value of each entry doesn't matter as
     # long as it's not null
     for identity in raw_job_configuration.identities:
         assert identities[identity] is not None
```

### Comparing `prefect-azure-0.2.8/tests/test_blob_storage.py` & `prefect-azure-0.2.9/tests/test_blob_storage.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/tests/test_block_standards.py` & `prefect-azure-0.2.9/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/tests/test_cosmos_db.py` & `prefect-azure-0.2.9/tests/test_cosmos_db.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/tests/test_credentials.py` & `prefect-azure-0.2.9/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/tests/test_ml_datastore.py` & `prefect-azure-0.2.9/tests/test_ml_datastore.py`

 * *Files identical despite different names*

### Comparing `prefect-azure-0.2.8/versioneer.py` & `prefect-azure-0.2.9/versioneer.py`

 * *Files identical despite different names*

