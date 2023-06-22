# Comparing `tmp/spatiafi-1.1.7.tar.gz` & `tmp/spatiafi-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatiafi-1.1.7.tar", last modified: Wed Jun 21 21:51:04 2023, max compression
+gzip compressed data, was "spatiafi-1.1.8.tar", last modified: Thu Jun 22 00:35:58 2023, max compression
```

## Comparing `spatiafi-1.1.7.tar` & `spatiafi-1.1.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.1.7/.dockerignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.1.7/.gitignore
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.1.7/.pre-commit-config.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-06-17 16:21:46.000000 spatiafi-1.1.7/.requirements.sha256
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.1.7/Dockerfile
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.1.7/LICENSE
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-21 21:51:04.464701 spatiafi-1.1.7/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-06-17 16:27:30.000000 spatiafi-1.1.7/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-06-12 18:08:33.000000 spatiafi-1.1.7/pyproject.toml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-06-17 16:21:46.000000 spatiafi-1.1.7/requirements-dev.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-06-17 16:20:25.000000 spatiafi-1.1.7/requirements.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.460701 spatiafi-1.1.7/scripts/
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/bootstrap_dev.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/build_docker.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/gen_requirements.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/install_package.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.1.7/scripts/test.sh
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-06-21 17:00:42.000000 spatiafi-1.1.7/scripts/upload_pypi.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      935 2023-06-21 21:51:04.464701 spatiafi-1.1.7/setup.cfg
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.1.7/setup.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.460701 spatiafi-1.1.7/src/
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/src/spatiafi/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-06-17 16:27:44.000000 spatiafi-1.1.7/src/spatiafi/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:12:50.000000 spatiafi-1.1.7/src/spatiafi/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi/_version.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.1.7/src/spatiafi/auth.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/src/spatiafi/gdal_auth/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       79 2023-06-18 01:03:50.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:27:45.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/__main__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-06-17 16:27:45.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/cli.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4742 2023-06-21 21:50:25.000000 spatiafi-1.1.7/src/spatiafi/gdal_auth/gdal_auth.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-06-17 16:27:45.000000 spatiafi-1.1.7/src/spatiafi/session.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/src/spatiafi.egg-info/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/PKG-INFO
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/SOURCES.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/dependency_links.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/entry_points.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      235 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/requires.txt
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-06-21 21:51:04.000000 spatiafi-1.1.7/src/spatiafi.egg-info/top_level.txt
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/tests/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.1.7/tests/__init__.py
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.1.7/tests/test_dummy.py
-drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-21 21:51:04.464701 spatiafi-1.1.7/workflows/
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/README.md
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/delpoy-sensor.sh
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/kustomization.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/py-spfi-api-build-wf.yaml
--rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/repo-sensor.yaml
--rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.1.7/workflows/submit-wf.sh
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3978 2023-06-12 18:08:33.000000 spatiafi-1.1.8/.dockerignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3996 2023-06-12 18:08:33.000000 spatiafi-1.1.8/.gitignore
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1464 2023-06-12 18:08:33.000000 spatiafi-1.1.8/.pre-commit-config.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      136 2023-06-17 16:21:46.000000 spatiafi-1.1.8/.requirements.sha256
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1148 2023-06-12 18:08:33.000000 spatiafi-1.1.8/Dockerfile
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)    11357 2023-06-12 18:08:33.000000 spatiafi-1.1.8/LICENSE
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-22 00:35:58.156515 spatiafi-1.1.8/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3683 2023-06-17 16:27:30.000000 spatiafi-1.1.8/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      845 2023-06-12 18:08:33.000000 spatiafi-1.1.8/pyproject.toml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4698 2023-06-17 16:21:46.000000 spatiafi-1.1.8/requirements-dev.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      912 2023-06-17 16:20:25.000000 spatiafi-1.1.8/requirements.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/scripts/
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     1517 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/bootstrap_dev.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      486 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/build_docker.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)     2074 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/gen_requirements.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      228 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/install_package.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      322 2023-06-12 18:08:33.000000 spatiafi-1.1.8/scripts/test.sh
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      135 2023-06-21 17:00:42.000000 spatiafi-1.1.8/scripts/upload_pypi.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      935 2023-06-22 00:35:58.156515 spatiafi-1.1.8/setup.cfg
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       92 2023-06-12 18:08:33.000000 spatiafi-1.1.8/setup.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.152515 spatiafi-1.1.8/src/
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/src/spatiafi/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      506 2023-06-17 16:27:44.000000 spatiafi-1.1.8/src/spatiafi/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:12:50.000000 spatiafi-1.1.8/src/spatiafi/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      160 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi/_version.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2370 2023-06-12 18:12:08.000000 spatiafi-1.1.8/src/spatiafi/auth.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/src/spatiafi/gdal_auth/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       79 2023-06-18 01:03:50.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       46 2023-06-17 16:27:45.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/__main__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     3743 2023-06-17 16:27:45.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/cli.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     5981 2023-06-22 00:35:11.000000 spatiafi-1.1.8/src/spatiafi/gdal_auth/gdal_auth.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     2054 2023-06-17 16:27:45.000000 spatiafi-1.1.8/src/spatiafi/session.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/src/spatiafi.egg-info/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     4026 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/PKG-INFO
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      987 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        1 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       53 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/entry_points.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      235 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/requires.txt
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        9 2023-06-22 00:35:58.000000 spatiafi-1.1.8/src/spatiafi.egg-info/top_level.txt
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/tests/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-12 18:08:33.000000 spatiafi-1.1.8/tests/__init__.py
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)       34 2023-06-12 18:08:33.000000 spatiafi-1.1.8/tests/test_dummy.py
+drwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)        0 2023-06-22 00:35:58.156515 spatiafi-1.1.8/workflows/
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1674 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/README.md
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1131 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/delpoy-sensor.sh
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      440 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/kustomization.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)      300 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/py-spfi-api-build-wf.yaml
+-rw-rw-r--   0 bkanuka   (1000) bkanuka   (1000)     1785 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/repo-sensor.yaml
+-rwxrwxr-x   0 bkanuka   (1000) bkanuka   (1000)      831 2023-06-12 18:08:33.000000 spatiafi-1.1.8/workflows/submit-wf.sh
```

### Comparing `spatiafi-1.1.7/.dockerignore` & `spatiafi-1.1.8/.dockerignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/.gitignore` & `spatiafi-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/.pre-commit-config.yaml` & `spatiafi-1.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/Dockerfile` & `spatiafi-1.1.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/LICENSE` & `spatiafi-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/PKG-INFO` & `spatiafi-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.7/README.md` & `spatiafi-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/pyproject.toml` & `spatiafi-1.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/requirements-dev.txt` & `spatiafi-1.1.8/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/requirements.txt` & `spatiafi-1.1.8/requirements.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/scripts/bootstrap_dev.sh` & `spatiafi-1.1.8/scripts/bootstrap_dev.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/scripts/gen_requirements.sh` & `spatiafi-1.1.8/scripts/gen_requirements.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/setup.cfg` & `spatiafi-1.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/src/spatiafi/auth.py` & `spatiafi-1.1.8/src/spatiafi/auth.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/src/spatiafi/gdal_auth/cli.py` & `spatiafi-1.1.8/src/spatiafi/gdal_auth/cli.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/src/spatiafi/gdal_auth/gdal_auth.py` & `spatiafi-1.1.8/src/spatiafi/gdal_auth/gdal_auth.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,25 +5,39 @@
 authenticate using the instance's service account. If you're running locally, GDAL will authenticate using
 the credentials in your local user's Application Default Credentials (ADC) file (usually this is user
 credentials from `gcloud auth application-default login`).
 """
 import json
 import logging
 import os
+import webbrowser
 from typing import Dict, Tuple
 
 import google.auth
 import google.auth.credentials
 import google.auth.transport.requests
 import requests
 from google.oauth2.credentials import Credentials as UserCredentials
 from platformdirs import user_config_dir
 
 logger = logging.getLogger(__name__)
 
+_OAUTH_CONFIG = {
+    "web": {
+        "client_id": "111941376227-3kjeanolo61g8t207od52epjinga0gdo.apps.googleusercontent.com",
+        "project_id": "ce-datasets",
+        "auth_uri": "https://accounts.google.com/o/oauth2/auth",
+        "token_uri": "https://oauth2.googleapis.com/token",
+        "auth_provider_x509_cert_url": "https://www.googleapis.com/oauth2/v1/certs",
+        "client_secret": "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",
+        "redirect_uris": ["https://auth.spatiafi.com/google_auth_helper/"],
+    }
+}
+
+
 _GDAL_SCOPES = [
     "https://www.googleapis.com/auth/devstorage.read_write",
     "https://www.googleapis.com/auth/userinfo.email",
     "https://www.googleapis.com/auth/userinfo.profile",
     "https://www.googleapis.com/auth/accounts.reauth",
     "https://www.googleapis.com/auth/earthengine",
     "openid",
@@ -70,14 +84,38 @@
 
     with open(on_gcp_file, "w") as f:
         f.write("False")
     _on_gcp = False
     return False
 
 
+def oob_auth_flow(open_browser=True, project=None):
+    from google_auth_oauthlib.flow import Flow
+
+    # Create the flow using the client secrets file from the Google API console.
+    flow = Flow.from_client_config(
+        _OAUTH_CONFIG,
+        scopes=_GDAL_SCOPES,
+    )
+    flow.redirect_uri = _OAUTH_CONFIG["web"]["redirect_uris"][0]
+
+    auth_url, _ = flow.authorization_url(prompt="consent")
+    if open_browser:
+        webbrowser.open(auth_url, new=1, autoraise=True)
+
+    print("Please visit this URL to authorize this application: {}".format(auth_url))
+    code = input("Enter the authorization code: ")
+
+    flow.fetch_token(code=code)
+
+    credentials = flow.credentials
+
+    return credentials, flow.client_config["project_id"]
+
+
 def get_user_credentials(
     project=None,
 ) -> Tuple[google.auth.credentials.Credentials, str]:
     """Get or refresh credentials"""
 
     if os.path.exists(user_credentials_file):
         with open(user_credentials_file, "r") as f:
@@ -88,17 +126,16 @@
 
         if project and project != quota_project_id:
             credentials = credentials.with_quota_project(quota_project_id=project)
         if credentials.expired:
             credentials.refresh(google.auth.transport.requests.Request())
         return credentials, project
 
-    credentials, project = google.auth.default(
-        quota_project_id=project, scopes=_GDAL_SCOPES
-    )
+    credentials, project = oob_auth_flow(project=project)
+
     credentials.refresh(
         google.auth.transport.requests.Request()
     )  # need to call once to get token
 
     if isinstance(credentials, UserCredentials):
         with open(user_credentials_file, "w") as f:
             credentials_dict = json.loads(credentials.to_json())
```

### Comparing `spatiafi-1.1.7/src/spatiafi/session.py` & `spatiafi-1.1.8/src/spatiafi/session.py`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/src/spatiafi.egg-info/PKG-INFO` & `spatiafi-1.1.8/src/spatiafi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatiafi
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python library for interacting with the SpatiaFi API
 Home-page: https://github.com/climateengine/py-spfi-api
 Author: Climate Engine Team
 Author-email: admin@climateengine.com
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `spatiafi-1.1.7/src/spatiafi.egg-info/SOURCES.txt` & `spatiafi-1.1.8/src/spatiafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/workflows/README.md` & `spatiafi-1.1.8/workflows/README.md`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/workflows/delpoy-sensor.sh` & `spatiafi-1.1.8/workflows/delpoy-sensor.sh`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/workflows/repo-sensor.yaml` & `spatiafi-1.1.8/workflows/repo-sensor.yaml`

 * *Files identical despite different names*

### Comparing `spatiafi-1.1.7/workflows/submit-wf.sh` & `spatiafi-1.1.8/workflows/submit-wf.sh`

 * *Files identical despite different names*

