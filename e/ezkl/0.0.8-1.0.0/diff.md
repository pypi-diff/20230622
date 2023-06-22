# Comparing `tmp/ezkl-0.0.8.tar.gz` & `tmp/ezkl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezkl-0.0.8.tar", max compression
+gzip compressed data, was "ezkl-1.0.0.tar", max compression
```

## Comparing `ezkl-0.0.8.tar` & `ezkl-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-13 19:36:57.630006 ezkl-0.0.8/LICENSE
--rw-r--r--   0        0        0     2412 2023-06-13 19:36:57.630006 ezkl-0.0.8/README.md
--rw-r--r--   0        0        0      273 2023-06-13 19:36:57.630006 ezkl-0.0.8/ezkl/__init__.py
--rw-r--r--   0        0        0     3232 2023-06-13 19:36:57.630006 ezkl-0.0.8/ezkl/export.py
--rw-r--r--   0        0        0      890 2023-06-13 19:37:11.898189 ezkl-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3307 1970-01-01 00:00:00.000000 ezkl-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-22 17:32:38.768713 ezkl-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2692 2023-06-22 17:32:38.768713 ezkl-1.0.0/README.md
+-rw-r--r--   0        0        0      319 2023-06-22 17:32:38.768713 ezkl-1.0.0/ezkl/__init__.py
+-rw-r--r--   0        0        0     4627 2023-06-22 17:32:38.768713 ezkl-1.0.0/ezkl/export.py
+-rw-r--r--   0        0        0      950 2023-06-22 17:32:49.720804 ezkl-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3544 1970-01-01 00:00:00.000000 ezkl-1.0.0/PKG-INFO
```

### Comparing `ezkl-0.0.8/LICENSE` & `ezkl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ezkl-0.0.8/README.md` & `ezkl-1.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,45 @@
 # ezkl
-`pip install ezkl` lets you use [ezkl](https://github.com/zkonduit/ezkl) directly from Python. It also contains an `export` function to generate `.onnx` and `.json` input files that can be ingested by the `ezkl` cli or from Python. [Here is colab notebook](https://colab.research.google.com/drive/1XuXNKqH7axOelZXyU3gpoTOCvFetIsKu?usp=sharing) that shows how to produce and verify a proof from Python.
+This repository contains the Python bindings for [ezkl](https://github.com/zkonduit/ezkl).
 
-Check out [the docs](https://docs.ezkl.xyz) for more. If you want to *develop* the Python bindings, read on.
+
+For more information check out [the docs](https://docs.ezkl.xyz).
+
+## quickstart
+
+To get started with `ezkl` run
+
+```shell
+pip install ezkl
+
+# alternatively, depending on how your environment is setup
+
+pip3 install ezkl
+```
+
+[Try out ezkl on colab here!](https://colab.research.google.com/drive/1XuXNKqH7axOelZXyU3gpoTOCvFetIsKu?usp=sharing).
 
 ## development setup
 
 ### poetry
 
+#### build pyezkl only
+Use this following setup if you would like to access developmental features in the pyezkl repo only. This will rely on the `ezkl_lib` version that is published on PyPI
+
+Clone this repository
+```shell
+poetry install
+poetry build
+cd dist
+poetry shell
+pip install wheel_file_you_just_generated.whl
+
+```
+
+#### build both ezkl and pyezkl
 Use this following setup if you would like to access developmental features in the main ezkl repo that is not released yet.
 
 Clone the ezkl repository.
 ```shell
 git clone https://github.com/zkonduit/ezkl.git
 ```
```

### Comparing `ezkl-0.0.8/pyproject.toml` & `ezkl-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ezkl"
-version = "0.0.8"
+version = "1.0.0"
 description = "Easy zero-knowledge learning in Python"
 authors = [
   "Jason Morton <jason@zkonduit.com>",
   "Dante Camuto <jason@zkonduit.com>",
 ]
 readme = "README.md"
 license = "Apache-2.0"
@@ -14,22 +14,25 @@
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = ">=3.8"
 numpy = "*"
 torch = "*"
 onnx = "*"
-ezkl_lib = ">=0.1.0"
+ezkl_lib = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
+scikit-learn = "^1.2.2"
+pandas = "^2.0.2"
+jupyter = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.4.2"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
 "Homepage" = "https://github.com/zkonduit/pyezkl"
```

### Comparing `ezkl-0.0.8/PKG-INFO` & `ezkl-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,69 @@
 Metadata-Version: 2.1
 Name: ezkl
-Version: 0.0.8
+Version: 1.0.0
 Summary: Easy zero-knowledge learning in Python
 Home-page: https://github.com/zkonduit/pyezkl
 License: Apache-2.0
 Author: Jason Morton
 Author-email: jason@zkonduit.com
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
-Requires-Dist: ezkl_lib (>=0.1.0)
+Requires-Dist: ezkl_lib (>=0.3.0,<0.4.0)
 Requires-Dist: numpy
 Requires-Dist: onnx
 Requires-Dist: torch
 Project-URL: Repository, https://github.com/zkonduit/pyezkl
 Description-Content-Type: text/markdown
 
 # ezkl
-`pip install ezkl` lets you use [ezkl](https://github.com/zkonduit/ezkl) directly from Python. It also contains an `export` function to generate `.onnx` and `.json` input files that can be ingested by the `ezkl` cli or from Python. [Here is colab notebook](https://colab.research.google.com/drive/1XuXNKqH7axOelZXyU3gpoTOCvFetIsKu?usp=sharing) that shows how to produce and verify a proof from Python.
+This repository contains the Python bindings for [ezkl](https://github.com/zkonduit/ezkl).
 
-Check out [the docs](https://docs.ezkl.xyz) for more. If you want to *develop* the Python bindings, read on.
+
+For more information check out [the docs](https://docs.ezkl.xyz).
+
+## quickstart
+
+To get started with `ezkl` run
+
+```shell
+pip install ezkl
+
+# alternatively, depending on how your environment is setup
+
+pip3 install ezkl
+```
+
+[Try out ezkl on colab here!](https://colab.research.google.com/drive/1XuXNKqH7axOelZXyU3gpoTOCvFetIsKu?usp=sharing).
 
 ## development setup
 
 ### poetry
 
+#### build pyezkl only
+Use this following setup if you would like to access developmental features in the pyezkl repo only. This will rely on the `ezkl_lib` version that is published on PyPI
+
+Clone this repository
+```shell
+poetry install
+poetry build
+cd dist
+poetry shell
+pip install wheel_file_you_just_generated.whl
+
+```
+
+#### build both ezkl and pyezkl
 Use this following setup if you would like to access developmental features in the main ezkl repo that is not released yet.
 
 Clone the ezkl repository.
 ```shell
 git clone https://github.com/zkonduit/ezkl.git
 ```
```

