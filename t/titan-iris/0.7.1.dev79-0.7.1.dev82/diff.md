# Comparing `tmp/titan-iris-0.7.1.dev79.tar.gz` & `tmp/titan-iris-0.7.1.dev82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titan-iris-0.7.1.dev79.tar", last modified: Wed Jun 21 16:25:05 2023, max compression
+gzip compressed data, was "titan-iris-0.7.1.dev82.tar", last modified: Wed Jun 21 16:31:49 2023, max compression
```

## Comparing `titan-iris-0.7.1.dev79.tar` & `titan-iris-0.7.1.dev82.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:05.505529 titan-iris-0.7.1.dev79/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 16:25:05.505529 titan-iris-0.7.1.dev79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 16:25:05.505529 titan-iris-0.7.1.dev79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:05.501529 titan-iris-0.7.1.dev79/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:05.501529 titan-iris-0.7.1.dev79/src/iris/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:05.501529 titan-iris-0.7.1.dev79/src/iris/gradio/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/gradio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/gradio/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    27220 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:05.501529 titan-iris-0.7.1.dev79/src/iris/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/sdk/auth_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/sdk/conf_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/sdk/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/sdk/iris_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/sdk/safe_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/src/iris/sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:05.505529 titan-iris-0.7.1.dev79/src/titan_iris.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 16:25:05.000000 titan-iris-0.7.1.dev79/src/titan_iris.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 16:25:05.000000 titan-iris-0.7.1.dev79/src/titan_iris.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:25:05.000000 titan-iris-0.7.1.dev79/src/titan_iris.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 16:25:05.000000 titan-iris-0.7.1.dev79/src/titan_iris.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 16:25:05.000000 titan-iris-0.7.1.dev79/src/titan_iris.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 16:25:05.000000 titan-iris-0.7.1.dev79/src/titan_iris.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:25:05.505529 titan-iris-0.7.1.dev79/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 16:24:54.000000 titan-iris-0.7.1.dev79/tests/test_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/iris/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/iris/gradio/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/gradio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/gradio/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27220 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.832139 titan-iris-0.7.1.dev82/src/iris/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11319 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/auth_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/conf_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6405 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27387 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/iris_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/safe_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16810 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/src/iris/sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6932 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-21 16:31:49.000000 titan-iris-0.7.1.dev82/src/titan_iris.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 16:31:49.836139 titan-iris-0.7.1.dev82/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-06-21 16:31:32.000000 titan-iris-0.7.1.dev82/tests/test_sdk.py
```

### Comparing `titan-iris-0.7.1.dev79/.gitignore` & `titan-iris-0.7.1.dev82/.gitignore`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/Dockerfile` & `titan-iris-0.7.1.dev82/Dockerfile`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/PKG-INFO` & `titan-iris-0.7.1.dev82/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.7.1.dev79
+Version: 0.7.1.dev82
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.7.1.dev79/README.md` & `titan-iris-0.7.1.dev82/README.md`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/setup.py` & `titan-iris-0.7.1.dev82/setup.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/config.yaml` & `titan-iris-0.7.1.dev82/src/iris/config.yaml`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/gradio/run.py` & `titan-iris-0.7.1.dev82/src/iris/gradio/run.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/main.py` & `titan-iris-0.7.1.dev82/src/iris/main.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/sdk/auth_utils.py` & `titan-iris-0.7.1.dev82/src/iris/sdk/auth_utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/sdk/conf_manager.py` & `titan-iris-0.7.1.dev82/src/iris/sdk/conf_manager.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/sdk/exception.py` & `titan-iris-0.7.1.dev82/src/iris/sdk/exception.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/sdk/iris_sdk.py` & `titan-iris-0.7.1.dev82/src/iris/sdk/iris_sdk.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/sdk/safe_convert.py` & `titan-iris-0.7.1.dev82/src/iris/sdk/safe_convert.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/iris/sdk/utils.py` & `titan-iris-0.7.1.dev82/src/iris/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/src/titan_iris.egg-info/PKG-INFO` & `titan-iris-0.7.1.dev82/src/titan_iris.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titan-iris
-Version: 0.7.1.dev79
+Version: 0.7.1.dev82
 Description-Content-Type: text/markdown
 
 # IRIS CLI Package.
 
 ## Description
 
 Iris is your portal to the TitanML platform. Using Iris, you can launch jobs to run on TitanML servers, run your own models and datasets through our compression algorithms, and explore and download the optimised models from the Titan Store.
```

### Comparing `titan-iris-0.7.1.dev79/src/titan_iris.egg-info/SOURCES.txt` & `titan-iris-0.7.1.dev82/src/titan_iris.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/tests/test_cli.py` & `titan-iris-0.7.1.dev82/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `titan-iris-0.7.1.dev79/tests/test_sdk.py` & `titan-iris-0.7.1.dev82/tests/test_sdk.py`

 * *Files identical despite different names*

