# Comparing `tmp/enfobench-0.0.1.tar.gz` & `tmp/enfobench-0.1.0.tar.gz`

## Comparing `enfobench-0.0.1.tar` & `enfobench-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 enfobench-0.0.1/Makefile
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 enfobench-0.0.1/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 enfobench-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.0.1/src/enfobench/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 enfobench-0.0.1/src/enfobench/__version__.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 enfobench-0.0.1/src/enfobench/example.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 enfobench-0.0.1/src/enfobench/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 enfobench-0.0.1/tests/test_example.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 enfobench-0.0.1/.gitignore
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 enfobench-0.0.1/LICENCE
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 enfobench-0.0.1/README.md
--rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 enfobench-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2837 2020-02-02 00:00:00.000000 enfobench-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 enfobench-0.1.0/Makefile
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 enfobench-0.1.0/README.md
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 enfobench-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/__version__.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/py.typed
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/utils.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/__init__.py
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/_cross_validate.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/_evaluate.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/client.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/metrics.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/protocols.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 enfobench-0.1.0/src/enfobench/evaluation/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 enfobench-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 enfobench-0.1.0/tests/test_metrics.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 enfobench-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 enfobench-0.1.0/LICENCE
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 enfobench-0.1.0/README.md
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 enfobench-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 enfobench-0.1.0/PKG-INFO
```

### Comparing `enfobench-0.0.1/Makefile` & `enfobench-0.1.0/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # COMMANDS                                                                      #
 #################################################################################
 
 ## Install project dependencies
 install:
 	pip install -U pip
 	pip install -e ."[test,dev]"
+	mypy --install-types
 
 ## Delete all compiled Python files
 clean:
 	find . -type f -name "*.py[co]" -delete
 	find . -type d -name "__pycache__" -delete
 
 ## Lint using ruff, mypy, black, and isort
@@ -40,15 +41,15 @@
 	pytest src tests
 
 #################################################################################
 # PROJECT RULES                                                                 #
 #################################################################################
 
 ## Build source distribution and wheel
-build: lint
+build: lint tests
 	hatch build
 
 ## Upload source distribution and wheel to PyPI
 publish: build
 	hatch publish --repo main
 
 ## Upload source distribution and wheel to TestPyPI
```

### Comparing `enfobench-0.0.1/README.md` & `enfobench-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 Energy  Forecast Benchmark Toolkit
 ==============================
+
+[![PyPI version](https://badge.fury.io/py/enfobench.svg)](https://badge.fury.io/py/enfobench)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 
 Energy Forecast Benchmark Toolkit is a Python project that aims to provide common tools to
 benchmark forecast models.
```

### Comparing `enfobench-0.0.1/pyproject.toml` & `enfobench-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,22 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
-    "pandas<2.0.0,>=1.3.5",
+    "fastapi>=0.68.0,<1.0.0",
+    "pandas>=1.3.0,<2.0.0",
+    "pydantic>=1.0.0,<2.0.0",
+    "python-multipart>=0.0.0,<1.0.0",
+    "pyarrow>=12.0.0,<13.0.0",
+    "requests>=2.26.0,<3.0.0",
+    "tqdm>=4.60.0,<5.0.0",
+    "uvicorn>=0.20.0,<1.0.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/attila-balint-kul/energy-forecast-benchmark-toolkit"
 
 [project.optional-dependencies]
```

### Comparing `enfobench-0.0.1/.gitignore` & `enfobench-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `enfobench-0.0.1/LICENCE` & `enfobench-0.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `enfobench-0.0.1/PKG-INFO` & `enfobench-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enfobench
-Version: 0.0.1
+Version: 0.1.0
 Summary: Energy forecast benchmarking toolkit.
 Project-URL: Homepage, https://github.com/attila-balint-kul/energy-forecast-benchmark-toolkit
 Author-email: attila.balint@kuleuven.be
 License-File: LICENCE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -15,28 +15,37 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
-Requires-Dist: pandas<2.0.0,>=1.3.5
+Requires-Dist: fastapi<1.0.0,>=0.68.0
+Requires-Dist: pandas<2.0.0,>=1.3.0
+Requires-Dist: pyarrow<13.0.0,>=12.0.0
+Requires-Dist: pydantic<2.0.0,>=1.0.0
+Requires-Dist: python-multipart<1.0.0,>=0.0.0
+Requires-Dist: requests<3.0.0,>=2.26.0
+Requires-Dist: tqdm<5.0.0,>=4.60.0
+Requires-Dist: uvicorn<1.0.0,>=0.20.0
 Provides-Extra: dev
 Requires-Dist: pre-commit<4.0.0,>=3.0.0; extra == 'dev'
 Requires-Dist: twine<5.0.0,>=4.0.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: black==23.3.0; extra == 'test'
 Requires-Dist: isort==5.12.0; extra == 'test'
 Requires-Dist: mypy==1.4.0; extra == 'test'
 Requires-Dist: pytest==7.3.2; extra == 'test'
 Requires-Dist: ruff==0.0.274; extra == 'test'
 Description-Content-Type: text/markdown
 
 Energy  Forecast Benchmark Toolkit
 ==============================
+
+[![PyPI version](https://badge.fury.io/py/enfobench.svg)](https://badge.fury.io/py/enfobench)
 [![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
 [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v0.json)](https://github.com/charliermarsh/ruff)
 [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy)
 
 Energy Forecast Benchmark Toolkit is a Python project that aims to provide common tools to
 benchmark forecast models.
```

