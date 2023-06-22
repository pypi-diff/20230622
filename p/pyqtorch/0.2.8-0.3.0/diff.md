# Comparing `tmp/pyqtorch-0.2.8.tar.gz` & `tmp/pyqtorch-0.3.0.tar.gz`

## Comparing `pyqtorch-0.2.8.tar` & `pyqtorch-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,61 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/README.md
--rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/mkdocs.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/publish.sh
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/setup.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/.github/workflows/run-tests-and-mypy.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
-
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
-
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/QAOA.ipynb
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/circuit.md
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/essentials.ipynb
--rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/fit_function.ipynb
--rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/gate_composition.ipynb
--rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/hamevo.md
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/matrices.md
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/parametric.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/primitive.md
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/getting_started.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/embedding.py
--rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/abstract.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0    14144 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_converters.py
--rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_modules.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_notebooks.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/LICENSE
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 pyqtorch-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/README.md
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/publish.sh
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/.github/workflows/run-tests-and-mypy.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/CODE_OF_CONDUCT.md -> ../CODE_OF_CONDUCT.md
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/CONTRIBUTING.md -> ../CONTRIBUTING.md
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/QAOA.ipynb
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/circuit.md
+-rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/essentials.ipynb
+-rw-r--r--   0        0        0   154246 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/fit_function.ipynb
+-rw-r--r--   0        0        0     2854 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/gate_composition.ipynb
+-rw-r--r--   0        0        0     4634 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/hamevo.md
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/matrices.md
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/parametric.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/primitive.md
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0    74062 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/getting_started.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     4939 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/abstract.py
+-rw-r--r--   0        0        0     9603 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0    11650 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0    14141 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0    11426 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_converters.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_modules.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 pyqtorch-0.3.0/PKG-INFO
```

### Comparing `pyqtorch-0.2.8/.pre-commit-config.yaml` & `pyqtorch-0.3.0/.pre-commit-config.yaml`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: check-yaml
       - id: check-added-large-files
 
 -   repo: https://github.com/ambv/black
-    rev: 22.10.0
+    rev: 23.3.0
     hooks:
       - id: black
 
 -   repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.243"
+    rev: "v0.0.274"
     hooks:
       - id: ruff
         args: [--fix]
 
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.4.0
     hooks:
       - id: mypy
         exclude: examples|docs
```

### Comparing `pyqtorch-0.2.8/CODE_OF_CONDUCT.md` & `pyqtorch-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/CONTRIBUTING.md` & `pyqtorch-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/mkdocs.yml` & `pyqtorch-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.3.0/.github/workflows/run-tests-and-mypy.yml`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   unit_tests:
     if: |
       github.event_name == 'push' || github.event_name == 'pull_request'
     name: Unit testing
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8","3.9", "3.10", "3.11"]
 
     steps:
 
         - name: Checkout main code and submodules
           uses: actions/checkout@v2
 
         - name: Set up Python ${{ matrix.python-version }}
@@ -38,8 +38,8 @@
 
         - name: Lint
           run: |
             python -m hatch -e tests run pre-commit run --all-files
 
         - name: Perform unit tests
           run: |
-            python -m hatch -e tests run pytest -n auto
+            python -m hatch -e tests run pytest -n auto && hatch -e docs run mkdocs build --clean --strict
```

### Comparing `pyqtorch-0.2.8/docs/QAOA.ipynb` & `pyqtorch-0.3.0/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/essentials.ipynb` & `pyqtorch-0.3.0/docs/essentials.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/fit_function.ipynb` & `pyqtorch-0.3.0/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/gate_composition.ipynb` & `pyqtorch-0.3.0/docs/gate_composition.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/hamevo.md` & `pyqtorch-0.3.0/docs/hamevo.md`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.3.0/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/deprecated/bench.py` & `pyqtorch-0.3.0/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.3.0/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/deprecated/getting_started.ipynb` & `pyqtorch-0.3.0/docs/deprecated/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.3.0/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.3.0/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/__init__.py` & `pyqtorch-0.3.0/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/ansatz.py` & `pyqtorch-0.3.0/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/embedding.py` & `pyqtorch-0.3.0/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/matrices.py` & `pyqtorch-0.3.0/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/matrices_sparse.py` & `pyqtorch-0.3.0/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/converters/store_ops.py` & `pyqtorch-0.3.0/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.3.0/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/core/__init__.py` & `pyqtorch-0.3.0/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/core/batched_operation.py` & `pyqtorch-0.3.0/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/core/circuit.py` & `pyqtorch-0.3.0/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/core/measurement.py` & `pyqtorch-0.3.0/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/core/operation.py` & `pyqtorch-0.3.0/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/core/utils.py` & `pyqtorch-0.3.0/pyqtorch/core/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,17 @@
     mat = mat.reshape([2] * len(qubits) * 2)
     mat_dims = list(range(len(qubits), 2 * len(qubits)))
     state_dims = [N_qubits - i - 1 for i in list(qubits)]
     axes = (mat_dims, state_dims)
 
     state = torch.tensordot(mat, state, dims=axes)
     inv_perm = torch.argsort(
-        torch.tensor(state_dims + [j for j in range(N_qubits + 1) if j not in state_dims])
+        torch.tensor(
+            state_dims + [j for j in range(N_qubits + 1) if j not in state_dims], dtype=torch.int
+        )
     )
     state = torch.permute(state, tuple(inv_perm))
     return state
 
 
 def _apply_einsum_gate(
     state: torch.Tensor, mat: torch.Tensor, qubits: Any, N_qubits: int
```

### Comparing `pyqtorch-0.2.8/pyqtorch/modules/abstract.py` & `pyqtorch-0.3.0/pyqtorch/modules/abstract.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/modules/circuit.py` & `pyqtorch-0.3.0/pyqtorch/modules/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
         self.thetas = Parameter(torch.empty(n_qubits, Op.n_params))
         self.reset_parameters()
 
     def reset_parameters(self) -> None:
         init.uniform_(self.thetas, -2 * PI, 2 * PI)
 
     def forward(self, state: torch.Tensor, _: torch.Tensor = None) -> torch.Tensor:
-        for (op, t) in zip(self.operations, self.thetas):
+        for op, t in zip(self.operations, self.thetas):
             state = op(state, t)
         return state
 
 
 class EntanglingLayer(QuantumCircuit):
     def __init__(self, n_qubits: int):
         """
```

### Comparing `pyqtorch-0.2.8/pyqtorch/modules/hamevo.py` & `pyqtorch-0.3.0/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/modules/parametric.py` & `pyqtorch-0.3.0/pyqtorch/modules/parametric.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,17 @@
         return self.apply(mats, state)
 
     def extra_repr(self) -> str:
         return f"qubits={self.qubits}, n_qubits={self.n_qubits}"
 
 
 class U(AbstractGate):
-
     n_params = 3
 
     def __init__(self, qubits: ArrayLike, n_qubits: int):
-
         """
         Represents a parametrized arbitrary rotation along the axes of the Bloch sphere.
 
         The angles `phi, theta, omega` in tensor format, applied as:
 
             U(phi, theta, omega) = RZ(omega)RY(theta)RZ(phi)
 
@@ -360,15 +358,14 @@
         super().__init__("Z", qubits, n_qubits)
 
 
 class CPHASE(AbstractGate):
     n_params = 1
 
     def __init__(self, qubits: ArrayLike, n_qubits: int):
-
         """
         Represents a controlled-phase (CPHASE) gate in a quantum circuit.
         The CPhase gate class creates a controlled Phase gate, applying the PhaseGate
         according to the control qubit state.
 
         Arguments:
             qubits (ArrayLike): The control and target qubits for the CPHASE gate.
```

### Comparing `pyqtorch-0.2.8/pyqtorch/modules/primitive.py` & `pyqtorch-0.3.0/pyqtorch/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyqtorch/modules/utils.py` & `pyqtorch-0.3.0/pyqtorch/modules/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/tests/conftest.py` & `pyqtorch-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/tests/test_batched_operations.py` & `pyqtorch-0.3.0/tests/test_batched_operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 state_01 = torch.tensor([[0, 0], [1, 0]], dtype=torch.cdouble).unsqueeze(2)
 state_11 = torch.tensor([[0, 0], [0, 1]], dtype=torch.cdouble).unsqueeze(2)
 
 pi = torch.tensor(torch.pi, dtype=torch.cdouble)
 
 
 def test_batched_ops() -> None:
-
     n_qubits: int = 2
     batch_size: int = 10
     qc = QuantumCircuit(n_qubits)
 
     theta_dim = torch.Size([batch_size])
 
     theta = torch.randn(theta_dim)
@@ -29,14 +28,13 @@
 
     for op in [batchedCPHASE, batchedCRX, batchedCRY, batchedCRZ, batchedCPHASE]:
         res = op(theta, psi, [i for i in range(n_qubits)], n_qubits)
         assert not torch.any(torch.isnan(res))
 
 
 def test_batched_cphase() -> None:
-
     n_qubits: int = 2
     psi = torch.tensor([[0, 0], [0, 1]], dtype=torch.cdouble).unsqueeze(2)
     psi_target = torch.tensor([[0, 0], [0, -1]], dtype=torch.cdouble).unsqueeze(2)
     angle = pi.unsqueeze(0)
     res = batchedCPHASE(angle, psi, [i for i in range(n_qubits)], n_qubits)
     assert torch.allclose(res, psi_target, atol=1e-16)
```

### Comparing `pyqtorch-0.2.8/tests/test_converters.py` & `pyqtorch-0.3.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/tests/test_module_hamevo.py` & `pyqtorch-0.3.0/tests/test_module_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/tests/test_modules.py` & `pyqtorch-0.3.0/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/tests/test_notebooks.py` & `pyqtorch-0.3.0/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/tests/test_operations.py` & `pyqtorch-0.3.0/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/tests/test_operations_hamevo.py` & `pyqtorch-0.3.0/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/.gitignore` & `pyqtorch-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/LICENSE` & `pyqtorch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.8/pyproject.toml` & `pyqtorch-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 authors = [
     { name = "Slimane Thabet", email = "slimane.thabet@pasqal.com" },
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
-requires-python = ">=3.8.1,<3.11"
+requires-python = ">=3.8,<3.12"
 license = {text = "Proprietary"}
-version = "0.2.8"
+version = "0.3.0"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
     "openfermion>=1.5",
     "torch"
 ]
```

### Comparing `pyqtorch-0.2.8/PKG-INFO` & `pyqtorch-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.2.8
+Version: 0.3.0
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: <3.11,>=3.8.1
+Requires-Python: <3.12,>=3.8
 Requires-Dist: openfermion>=1.5
 Requires-Dist: torch
 Provides-Extra: converters
 Requires-Dist: qiskit; extra == 'converters'
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
```

