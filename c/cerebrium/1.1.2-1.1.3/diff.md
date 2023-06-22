# Comparing `tmp/cerebrium-1.1.2.tar.gz` & `tmp/cerebrium-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.1.2.tar", max compression
+gzip compressed data, was "cerebrium-1.1.3.tar", max compression
```

## Comparing `cerebrium-1.1.2.tar` & `cerebrium-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-21 15:33:31.298231 cerebrium-1.1.2/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-21 15:33:31.298231 cerebrium-1.1.2/README.md
--rw-r--r--   0        0        0      330 2023-06-21 15:37:17.443700 cerebrium-1.1.2/cerebrium/__init__.py
--rwxr-xr-x   0        0        0    10122 2023-06-21 15:33:31.298231 cerebrium-1.1.2/cerebrium/cli.py
--rw-r--r--   0        0        0    31667 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/conduit.py
--rw-r--r--   0        0        0     5049 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/core.py
--rw-r--r--   0        0        0     2476 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/errors.py
--rw-r--r--   0        0        0    11299 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/models/torch.py
--rw-r--r--   0        0        0     8540 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-21 15:33:31.302230 cerebrium-1.1.2/cerebrium/utils.py
--rw-r--r--   0        0        0     2546 2023-06-21 15:37:17.443700 cerebrium-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 cerebrium-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-22 13:13:58.786651 cerebrium-1.1.3/LICENSE
+-rw-r--r--   0        0        0     3473 2023-06-22 13:13:58.786651 cerebrium-1.1.3/README.md
+-rw-r--r--   0        0        0      330 2023-06-22 13:18:23.835744 cerebrium-1.1.3/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0    10167 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/cli.py
+-rw-r--r--   0        0        0    31667 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/conduit.py
+-rw-r--r--   0        0        0     5049 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/core.py
+-rw-r--r--   0        0        0     2476 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/errors.py
+-rw-r--r--   0        0        0    11299 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     8540 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-22 13:13:58.786651 cerebrium-1.1.3/cerebrium/utils.py
+-rw-r--r--   0        0        0     2546 2023-06-22 13:18:23.831744 cerebrium-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5617 1970-01-01 00:00:00.000000 cerebrium-1.1.3/PKG-INFO
```

### Comparing `cerebrium-1.1.2/LICENSE` & `cerebrium-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/README.md` & `cerebrium-1.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -59,14 +59,20 @@
 ```
 
 If the patch version is not up to date, merge the latest version tag into the branch:
 ```bash
 git merge v<tag>
 ```
 
+## Push a worker development build to ECR
+To push a worker development build to ECR, run the following command:
+```bash
+depot build -t 288552132534.dkr.ecr.eu-west-1.amazonaws.com/worker:dev --platform=linux/amd64 . --push --file worker/docker/Dockerfile --build-arg env=dev
+```
+
 ## Install a development build (DEPRECATED)
 To install a development build, run the following command to configure pip (**NOTE** this WILL change your default pip index URL):
 ```bash
 
 aws codeartifact login --tool pip --repository cerebrium-pypi --domain cerebrium --domain-owner 288552132534 --region eu-west-1
 ```
 Then, pip install:
```

### Comparing `cerebrium-1.1.2/cerebrium/cli.py` & `cerebrium-1.1.3/cerebrium/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     )
 ):
     """
     Set private API key for the user in ~/.cerebrium/config.yaml
     """
     config_path = os.path.expanduser("~/.cerebrium/config.yaml")
     os.makedirs(os.path.dirname(config_path), exist_ok=True)
-    config = yaml.full_load(open(config_path, "r"))
+    config = None if not os.path.exists(config_path) else yaml.full_load(open(config_path, "r"))
     if config is None:
         config = {"api_key": private_api_key}
     else:
         config["api_key"] = private_api_key
     with open(config_path, "w") as f:
         yaml.dump(config, f)
     print("✅  Logged in successfully.")
```

### Comparing `cerebrium-1.1.2/cerebrium/conduit.py` & `cerebrium-1.1.3/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/core.py` & `cerebrium-1.1.3/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/errors.py` & `cerebrium-1.1.3/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/flow.py` & `cerebrium-1.1.3/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/logging/arize.py` & `cerebrium-1.1.3/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/logging/base.py` & `cerebrium-1.1.3/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/logging/censius.py` & `cerebrium-1.1.3/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/models/base.py` & `cerebrium-1.1.3/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/models/sklearn.py` & `cerebrium-1.1.3/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/cerebrium/requests.py` & `cerebrium-1.1.3/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.1.2/pyproject.toml` & `cerebrium-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.1.2"
+version = "1.1.3"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.1.2/PKG-INFO` & `cerebrium-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.1.2
+Version: 1.1.3
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -110,14 +110,20 @@
 ```
 
 If the patch version is not up to date, merge the latest version tag into the branch:
 ```bash
 git merge v<tag>
 ```
 
+## Push a worker development build to ECR
+To push a worker development build to ECR, run the following command:
+```bash
+depot build -t 288552132534.dkr.ecr.eu-west-1.amazonaws.com/worker:dev --platform=linux/amd64 . --push --file worker/docker/Dockerfile --build-arg env=dev
+```
+
 ## Install a development build (DEPRECATED)
 To install a development build, run the following command to configure pip (**NOTE** this WILL change your default pip index URL):
 ```bash
 
 aws codeartifact login --tool pip --repository cerebrium-pypi --domain cerebrium --domain-owner 288552132534 --region eu-west-1
 ```
 Then, pip install:
```

