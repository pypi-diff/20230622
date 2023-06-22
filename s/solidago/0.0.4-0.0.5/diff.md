# Comparing `tmp/solidago-0.0.4.tar.gz` & `tmp/solidago-0.0.5.tar.gz`

## Comparing `solidago-0.0.4.tar` & `solidago-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/__init__.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/__version__.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/comparisons_to_scores/__init__.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/comparisons_to_scores/base.py
--rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/comparisons_to_scores/continuous_bradley_terry.py
--rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/comparisons_to_scores/hooke_individual_scores.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/resilient_primitives/__init__.py
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/resilient_primitives/_primitives.py
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 solidago-0.0.4/src/solidago/solvers/optimize.py
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 solidago-0.0.4/tests/test_comparisons_to_scores.py
--rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 solidago-0.0.4/tests/test_resilient_primitives.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 solidago-0.0.4/.gitignore
--rw-r--r--   0        0        0    35147 2020-02-02 00:00:00.000000 solidago-0.0.4/LICENSE
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 solidago-0.0.4/LICENSE.LESSER
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 solidago-0.0.4/README.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 solidago-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 solidago-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/__version__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/comparisons_to_scores/__init__.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/comparisons_to_scores/base.py
+-rw-r--r--   0        0        0     5069 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/comparisons_to_scores/continuous_bradley_terry.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/comparisons_to_scores/hooke_individual_scores.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/resilient_primitives/__init__.py
+-rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/resilient_primitives/_primitives.py
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 solidago-0.0.5/src/solidago/solvers/optimize.py
+-rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 solidago-0.0.5/tests/test_comparisons_to_scores.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 solidago-0.0.5/tests/test_resilient_primitives.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 solidago-0.0.5/.gitignore
+-rw-r--r--   0        0        0    35147 2020-02-02 00:00:00.000000 solidago-0.0.5/LICENSE
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 solidago-0.0.5/LICENSE.LESSER
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 solidago-0.0.5/README.md
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 solidago-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 solidago-0.0.5/PKG-INFO
```

### Comparing `solidago-0.0.4/src/solidago/comparisons_to_scores/base.py` & `solidago-0.0.5/src/solidago/comparisons_to_scores/base.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/src/solidago/comparisons_to_scores/continuous_bradley_terry.py` & `solidago-0.0.5/src/solidago/comparisons_to_scores/continuous_bradley_terry.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/src/solidago/comparisons_to_scores/hooke_individual_scores.py` & `solidago-0.0.5/src/solidago/comparisons_to_scores/hooke_individual_scores.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/src/solidago/resilient_primitives/_primitives.py` & `solidago-0.0.5/src/solidago/resilient_primitives/_primitives.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/src/solidago/solvers/optimize.py` & `solidago-0.0.5/src/solidago/solvers/optimize.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/tests/test_comparisons_to_scores.py` & `solidago-0.0.5/tests/test_comparisons_to_scores.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/tests/test_resilient_primitives.py` & `solidago-0.0.5/tests/test_resilient_primitives.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/LICENSE` & `solidago-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/LICENSE.LESSER` & `solidago-0.0.5/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/README.md` & `solidago-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `solidago-0.0.4/pyproject.toml` & `solidago-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 description = "Algorithms for Secure Algorithmic Governance"
 readme = "README.md"
 requires-python = ">=3.9"
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
+    "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",
 ]
 keywords = ["tournesol", "collaborative recommendations", "judgement aggregation", "comparison based", "mehestan"]
 dependencies = [
     "pandas>=1.5.3,<2.0",
     "numpy>=1.24.3,<1.25",
     "numba==0.57.0",
 ]
```

### Comparing `solidago-0.0.4/PKG-INFO` & `solidago-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: solidago
-Version: 0.0.4
+Version: 0.0.5
 Summary: Algorithms for Secure Algorithmic Governance
 Project-URL: Homepage, https://github.com/tournesol-app/tournesol/tree/main/solidago
 Project-URL: Bug Tracker, https://github.com/tournesol-app/tournesol/issues
 Author-email: Tournesol Association <hello@tournesol.app>
 License-Expression: LGPL-3.0-or-later
 License-File: LICENSE
 License-File: LICENSE.LESSER
 Keywords: collaborative recommendations,comparison based,judgement aggregation,mehestan,tournesol
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: numba==0.57.0
 Requires-Dist: numpy<1.25,>=1.24.3
 Requires-Dist: pandas<2.0,>=1.5.3
 Provides-Extra: test
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: solidago Version: 0.0.4 Summary: Algorithms for
+Metadata-Version: 2.1 Name: solidago Version: 0.0.5 Summary: Algorithms for
 Secure Algorithmic Governance Project-URL: Homepage, https://github.com/
 tournesol-app/tournesol/tree/main/solidago Project-URL: Bug Tracker, https://
 github.com/tournesol-app/tournesol/issues Author-email: Tournesol Association
 tournesol.app> License-Expression: LGPL-3.0-or-later License-File: LICENSE
 License-File: LICENSE.LESSER Keywords: collaborative recommendations,comparison
-based,judgement aggregation,mehestan,tournesol Classifier: Operating System ::
-OS Independent Classifier: Programming Language :: Python :: 3 Requires-Python:
->=3.9 Requires-Dist: numba==0.57.0 Requires-Dist: numpy<1.25,>=1.24.3 Requires-
-Dist: pandas<2.0,>=1.5.3 Provides-Extra: test Requires-Dist:
-pytest<8.0.0,>=7.1.3; extra == 'test' Description-Content-Type: text/markdown #
-Solidago **Solid** **A**lgorithmic **Go**vernance, used by the Tournesol
-platform [Package_version] [PyPI_-_License] ## Usage > **Warning** > This
-library is WIP; its API may change in the near future. ```py import numpy as np
-from solidago.resilient_primitives import QrMed score = QrMed(W=1, w=1,
+based,judgement aggregation,mehestan,tournesol Classifier: License :: OSI
+Approved :: GNU Lesser General Public License v3 or later (LGPLv3+) Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3 Requires-Python: >=3.9 Requires-Dist: numba==0.57.0 Requires-Dist:
+numpy<1.25,>=1.24.3 Requires-Dist: pandas<2.0,>=1.5.3 Provides-Extra: test
+Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test' Description-Content-Type:
+text/markdown # Solidago **Solid** **A**lgorithmic **Go**vernance, used by the
+Tournesol platform [Package_version] [PyPI_-_License] ## Usage > **Warning** >
+This library is WIP; its API may change in the near future. ```py import numpy
+as np from solidago.resilient_primitives import QrMed score = QrMed(W=1, w=1,
 x=np.array([-1.0, 1.0, 2.0]), delta=np.array([1.0, 1.0, 1.0])) ``` ## Publish a
 new release 1. In a Pull Request, update the version number in [`./src/
 solidago/__version__.py`](./src/solidago/__version__.py) 2. The package will be
 published automatically when the new version is merged into "main", by [this
 Github Action](../.github/workflows/solidago-publish.yml). ## Copyright &
 License Copyright 2023 Tournesol Association and contributors. This program is
 free software: you can redistribute it and/or modify it under the terms of the
```

