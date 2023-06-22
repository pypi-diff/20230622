# Comparing `tmp/wiremind-kubernetes-7.1.1.tar.gz` & `tmp/wiremind-kubernetes-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wiremind-kubernetes-7.1.1.tar", last modified: Mon Mar 27 17:30:50 2023, max compression
+gzip compressed data, was "wiremind-kubernetes-7.2.0.tar", last modified: Thu Jun 22 12:34:04 2023, max compression
```

## Comparing `wiremind-kubernetes-7.1.1.tar` & `wiremind-kubernetes-7.2.0.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.147805 wiremind-kubernetes-7.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/LICENCE.md
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-27 17:30:50.147805 wiremind-kubernetes-7.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-27 17:30:50.147805 wiremind-kubernetes-7.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.139804 wiremind-kubernetes-7.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.143804 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/kube_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)    19647 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/kubernetes_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.143804 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.143804 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.143804 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.147805 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3887 2023-03-27 17:30:36.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 17:30:50.143804 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-27 17:30:50.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-27 17:30:50.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 17:30:50.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-27 17:30:50.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-27 17:30:50.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 17:30:49.000000 wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.227086 wiremind-kubernetes-7.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kube_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19825 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3887 2023-06-22 12:33:48.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:34:04.231086 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:34:04.000000 wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/zip-safe
```

### Comparing `wiremind-kubernetes-7.1.1/LICENCE.md` & `wiremind-kubernetes-7.2.0/LICENCE.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/PKG-INFO` & `wiremind-kubernetes-7.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.1.1
+Version: 7.2.0
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.1.1/README.md` & `wiremind-kubernetes-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/setup.cfg` & `wiremind-kubernetes-7.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/setup.py` & `wiremind-kubernetes-7.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/exceptions.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/kube_config.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kube_config.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_client_additional_arguments.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,7 +69,12 @@
     def __init__(self, *args: Any, dry_run: bool = False, pretty: bool = False, **kwargs: Any) -> None:
         super().__init__(client=kubernetes.client.CustomObjectsApi, dry_run=dry_run, pretty=pretty)
 
 
 class RbacAuthorizationV1ApiWithArguments(ClientWithArguments):
     def __init__(self, *args: Any, dry_run: bool = False, pretty: bool = False, **kwargs: Any) -> None:
         super().__init__(client=kubernetes.client.RbacAuthorizationV1Api, dry_run=dry_run, pretty=pretty)
+
+
+class NetworkingV1ApiWithArguments(ClientWithArguments):
+    def __init__(self, *args: Any, dry_run: bool = False, pretty: bool = False, **kwargs: Any) -> None:
+        super().__init__(client=kubernetes.client.NetworkingV1Api, dry_run=dry_run, pretty=pretty)
```

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/kubernetes_helper.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/kubernetes_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 
 import kubernetes
 
 from wiremind_kubernetes.exceptions import PodNotFound
 
 from .kube_config import load_kubernetes_config
 from .kubernetes_client_additional_arguments import (
-    AppV1ApiWithArguments,
-    AutoscalingV1ApiWithArguments,
-    BatchV1ApiWithArguments,
-    CoreV1ApiWithArguments,
-    CustomObjectsApiWithArguments,
-    RbacAuthorizationV1ApiWithArguments,
-)
+    AppV1ApiWithArguments, AutoscalingV1ApiWithArguments,
+    BatchV1ApiWithArguments, CoreV1ApiWithArguments,
+    CustomObjectsApiWithArguments, NetworkingV1ApiWithArguments,
+    RbacAuthorizationV1ApiWithArguments)
 from .utils import retry_kubernetes_request, retry_kubernetes_request_no_ignore
 
 logger = logging.getLogger(__name__)
 
 HPA_ID_PREFIX = "wm--disabled--kube"
 
 
@@ -59,14 +56,17 @@
         )
         self.client_custom_objects_api: kubernetes.client.CustomObjectsApi = CustomObjectsApiWithArguments(
             dry_run=dry_run, pretty=pretty
         )
         self.client_rbac_authorization_v1_api: kubernetes.client.RbacAuthorizationV1Api = (
             RbacAuthorizationV1ApiWithArguments(dry_run=dry_run, pretty=pretty)
         )
+        self.client_networking_v1_api: kubernetes.client.NetworkingV1Api = NetworkingV1ApiWithArguments(
+            dry_run=dry_run, pretty=pretty
+        )
 
         self.dry_run: bool = dry_run
         self.pretty: bool = pretty
 
 
 def _get_namespace_from_kube() -> str:
     return open("/var/run/secrets/kubernetes.io/serviceaccount/namespace").read()
```

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/conftest.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/create_job_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/helpers.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/helpers.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/e2e_tests/start_stop_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kube_config_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_client_additional_arguments_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/kubernetes_deployment_manager_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/namespaced_kubernetes_helper_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/retry_kubernetes_request_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/tests/unit_tests/utils_test/run_command_test.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes/utils.py` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/PKG-INFO` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wiremind-kubernetes
-Version: 7.1.1
+Version: 7.2.0
 Summary: Helper for Kubernetes.
 Home-page: https://github.com/wiremind/wiremind-kubernetes
 Author: Wiremind
 Author-email: dev@wiremind.io
 License: LGPLv3+
 Keywords: kubernetes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `wiremind-kubernetes-7.1.1/src/wiremind_kubernetes.egg-info/SOURCES.txt` & `wiremind-kubernetes-7.2.0/src/wiremind_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

