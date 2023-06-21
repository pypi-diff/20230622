# Comparing `tmp/cvxrisk-0.0.6.tar.gz` & `tmp/cvxrisk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxrisk-0.0.6.tar", max compression
+gzip compressed data, was "cvxrisk-0.0.7.tar", max compression
```

## Comparing `cvxrisk-0.0.6.tar` & `cvxrisk-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0    11375 2023-06-21 16:21:29.636364 cvxrisk-0.0.6/LICENSE
--rw-r--r--   0        0        0     4628 2023-06-21 16:21:29.636364 cvxrisk-0.0.6/README.md
--rw-r--r--   0        0        0      137 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/linalg/__init__.py
--rw-r--r--   0        0        0      252 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/linalg/cholesky.py
--rw-r--r--   0        0        0     1301 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/linalg/pca.py
--rw-r--r--   0        0        0      512 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/linalg/valid.py
--rw-r--r--   0        0        0       91 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/random/__init__.py
--rw-r--r--   0        0        0      159 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/random/rand_cov.py
--rw-r--r--   0        0        0       93 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/__init__.py
--rw-r--r--   0        0        0       83 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/cvar/__init__.py
--rw-r--r--   0        0        0     1321 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/cvar/cvar.py
--rw-r--r--   0        0        0       92 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/factor/__init__.py
--rw-r--r--   0        0        0     1997 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/factor/factor.py
--rw-r--r--   0        0        0     1931 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/model.py
--rw-r--r--   0        0        0       97 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/sample/__init__.py
--rw-r--r--   0        0        0     1154 2023-06-21 16:21:29.664364 cvxrisk-0.0.6/cvx/risk/sample/sample.py
--rw-r--r--   0        0        0      581 2023-06-21 16:22:01.524622 cvxrisk-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5236 1970-01-01 00:00:00.000000 cvxrisk-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11375 2023-06-21 23:05:45.594008 cvxrisk-0.0.7/LICENSE
+-rw-r--r--   0        0        0     4830 2023-06-21 23:05:45.594008 cvxrisk-0.0.7/README.md
+-rw-r--r--   0        0        0      137 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/linalg/__init__.py
+-rw-r--r--   0        0        0      252 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/linalg/cholesky.py
+-rw-r--r--   0        0        0     1301 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/linalg/pca.py
+-rw-r--r--   0        0        0      512 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/linalg/valid.py
+-rw-r--r--   0        0        0        0 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/portfolio/__init__.py
+-rw-r--r--   0        0        0      343 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/portfolio/min_risk.py
+-rw-r--r--   0        0        0       91 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/random/__init__.py
+-rw-r--r--   0        0        0      159 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/random/rand_cov.py
+-rw-r--r--   0        0        0       93 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/risk/__init__.py
+-rw-r--r--   0        0        0     1519 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/risk/bounds.py
+-rw-r--r--   0        0        0       83 2023-06-21 23:05:45.618008 cvxrisk-0.0.7/cvx/risk/cvar/__init__.py
+-rw-r--r--   0        0        0     1347 2023-06-21 23:05:45.622008 cvxrisk-0.0.7/cvx/risk/cvar/cvar.py
+-rw-r--r--   0        0        0       92 2023-06-21 23:05:45.622008 cvxrisk-0.0.7/cvx/risk/factor/__init__.py
+-rw-r--r--   0        0        0     2205 2023-06-21 23:05:45.622008 cvxrisk-0.0.7/cvx/risk/factor/factor.py
+-rw-r--r--   0        0        0      783 2023-06-21 23:05:45.622008 cvxrisk-0.0.7/cvx/risk/model.py
+-rw-r--r--   0        0        0       97 2023-06-21 23:05:45.622008 cvxrisk-0.0.7/cvx/risk/sample/__init__.py
+-rw-r--r--   0        0        0     1170 2023-06-21 23:05:45.622008 cvxrisk-0.0.7/cvx/risk/sample/sample.py
+-rw-r--r--   0        0        0      581 2023-06-21 23:06:10.397955 cvxrisk-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5438 1970-01-01 00:00:00.000000 cvxrisk-0.0.7/PKG-INFO
```

### Comparing `cvxrisk-0.0.6/LICENSE` & `cvxrisk-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.6/README.md` & `cvxrisk-0.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
     )
 ```
 
 The risk model is injected into the function.
 The function is not aware of the precise risk model used.
 All risk models are required to implement the `estimate` method.
 
+Note that factor risk models work with weights for the assets but also with weights for the factors.
+To stay flexible we are applying thiS `**kwargs` pattern to the function above.
 ## A first example
 
 A first example is a risk model based on the sample covariance matrix.
 We construct the risk model as follows
 
 ```python
 import numpy as np
@@ -55,16 +57,16 @@
 ```
 
 The risk model and the actual optimization problem are decoupled.
 This is good practice and keeps the code clean and maintainable.
 
 In a backtest we don't have to reconstruct the problem in every iteration.
 We can simply update the risk model with the new data and solve the problem again.
-If the dimension of the problem is changing during the test we expect
-a new problem has to be constructed though.
+The implementation of the risk models is flexible enough to deal with changing dimensions
+of the underlying weight space.
 
 ## Risk models
 
 ### Sample covariance
 
 We offer a `SampleCovariance` class as seen above.
 
@@ -76,20 +78,20 @@
 ```math
 r_i = \sum_{j=1}^k f_j \beta_{ji} + \epsilon_i
 ```
 The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients
 $\beta_{ji}$.
 The residual returns $\epsilon_i$ are assumed to be uncorrelated with the factors.
 
-Any position $w$ in weight space projects to a position $y = \beta w$ in factor space.
+Any position $w$ in weight space projects to a position $y = \beta^T w$ in factor space.
 The variance for a position $w$ is the sum of the variance of the
 systematic returns explained by the factors and the variance of the idiosyncratic returns.
 
 ```math
-Var(r) = Var(\beta w) + Var(\epsilon w)
+Var(r) = Var(\beta^T w) + Var(\epsilon w)
 ```
 
 We assume the residual returns are uncorrelated and hence
 
 ```math
 Var(r) = y^T \Sigma_f y + \sum_i w_i^2 Var(\epsilon_i)
 ```
@@ -109,16 +111,15 @@
 of the observed residuals.
 The factor covariance matrix $\Sigma_f$ may even be diagonal in this case as the factors are orthogonal.
 
 We expose a method to compute the first $k$ principal components.
 
 ### cvar
 
-XXX: Conditional value at risk
-Relies on cxxpy's `sum_largest` function.
+We currently also support the conditional value at risk (CVaR) as a risk measure.
 
 
 
 
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
```

### Comparing `cvxrisk-0.0.6/cvx/linalg/pca.py` & `cvxrisk-0.0.7/cvx/linalg/pca.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.6/cvx/linalg/valid.py` & `cvxrisk-0.0.7/cvx/linalg/valid.py`

 * *Files identical despite different names*

### Comparing `cvxrisk-0.0.6/cvx/risk/cvar/cvar.py` & `cvxrisk-0.0.7/cvx/risk/cvar/cvar.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 
 import cvxpy as cvx
 import numpy as np
 
-from cvx.risk.model import Bounds
+from cvx.risk.bounds import Bounds
 from cvx.risk.model import Model
 
 
 @dataclass
 class CVar(Model):
     """Conditional value at risk model"""
 
@@ -19,15 +19,15 @@
     m: int = 0
 
     def __post_init__(self):
         self.k = int(self.n * (1 - self.alpha))
         self.parameter["R"] = cvx.Parameter(
             shape=(self.n, self.m), name="returns", value=np.zeros((self.n, self.m))
         )
-        self.bounds = Bounds(m=self.m)
+        self.bounds = Bounds(m=self.m, name="assets")
 
     def estimate(self, weights, **kwargs):
         """Estimate the risk by computing the Cholesky decomposition of self.cov"""
         # R is a matrix of returns, n is the number of rows in R
         # n = self.R.shape[0]
         # k is the number of returns in the left tail
         # k = int(n * (1 - self.alpha))
@@ -37,9 +37,9 @@
     def update(self, **kwargs):
         ret = kwargs["returns"]
         m = ret.shape[1]
 
         self.parameter["R"].value[:, :m] = kwargs["returns"]
         self.bounds.update(**kwargs)
 
-    def constraints(self, weights):
+    def constraints(self, weights, **kwargs):
         return self.bounds.constraints(weights)
```

### Comparing `cvxrisk-0.0.6/cvx/risk/factor/factor.py` & `cvxrisk-0.0.7/cvx/risk/factor/factor.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dataclasses import dataclass
 
 import cvxpy as cvx
 import numpy as np
 
 from cvx.linalg import cholesky
-from cvx.risk.model import Bounds
+from cvx.risk.bounds import Bounds
 from cvx.risk.model import Model
 
 
 @dataclass
 class FactorModel(Model):
     """Factor risk model"""
 
@@ -33,15 +33,16 @@
 
         self.parameter["chol"] = cvx.Parameter(
             shape=(self.k, self.k),
             name="cholesky of covariance",
             value=np.zeros((self.k, self.k)),
         )
 
-        self.bounds = Bounds(m=self.assets)
+        self.bounds_assets = Bounds(m=self.assets, name="assets")
+        self.bounds_factors = Bounds(m=self.k, name="factors")
 
     def estimate(self, weights, **kwargs):
         """
         Compute the total variance
         """
         var_residual = cvx.norm2(
             cvx.multiply(self.parameter["idiosyncratic_risk"], weights)
@@ -58,15 +59,18 @@
         k, assets = exposure.shape
 
         self.parameter["exposure"].value[:k, :assets] = kwargs["exposure"]
         self.parameter["idiosyncratic_risk"].value[:assets] = kwargs[
             "idiosyncratic_risk"
         ]
         self.parameter["chol"].value[:k, :k] = cholesky(kwargs["cov"])
-        self.bounds.update(**kwargs)
+        self.bounds_assets.update(**kwargs)
+        self.bounds_factors.update(**kwargs)
 
     def constraints(self, weights, **kwargs):
         y = kwargs.get("y", self.parameter["exposure"] @ weights)
 
-        return self.bounds.constraints(weights) + [
-            y == self.parameter["exposure"] @ weights
-        ]
+        return (
+            self.bounds_assets.constraints(weights)
+            + self.bounds_factors.constraints(y)
+            + [y == self.parameter["exposure"] @ weights]
+        )
```

### Comparing `cvxrisk-0.0.6/cvx/risk/sample/sample.py` & `cvxrisk-0.0.7/cvx/risk/sample/sample.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from dataclasses import dataclass
 
 import cvxpy as cvx
 import numpy as np
 
 from cvx.linalg import cholesky
-from cvx.risk.model import Bounds
+from cvx.risk.bounds import Bounds
 from cvx.risk.model import Model
 
 
 @dataclass
 class SampleCovariance(Model):
     """Risk model based on the Cholesky decomposition of the sample cov matrix"""
 
@@ -21,15 +21,15 @@
 
     def __post_init__(self):
         self.parameter["chol"] = cvx.Parameter(
             shape=(self.num, self.num),
             name="cholesky of covariance",
             value=np.zeros((self.num, self.num)),
         )
-        self.bounds = Bounds(m=self.num)
+        self.bounds = Bounds(m=self.num, name="assets")
 
     def estimate(self, weights, **kwargs):
         """Estimate the risk by computing the Cholesky decomposition of self.cov"""
         return cvx.norm2(self.parameter["chol"] @ weights)
 
     def update(self, **kwargs):
         cov = kwargs["cov"]
```

### Comparing `cvxrisk-0.0.6/pyproject.toml` & `cvxrisk-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxrisk"
-version = "v0.0.6"
+version = "v0.0.7"
 description = "Simple riskengine for cvxpy"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/cvxrisk"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxrisk-0.0.6/PKG-INFO` & `cvxrisk-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxrisk
-Version: 0.0.6
+Version: 0.0.7
 Summary: Simple riskengine for cvxpy
 Home-page: https://github.com/cvxgrp/cvxrisk
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -48,14 +48,16 @@
     )
 ```
 
 The risk model is injected into the function.
 The function is not aware of the precise risk model used.
 All risk models are required to implement the `estimate` method.
 
+Note that factor risk models work with weights for the assets but also with weights for the factors.
+To stay flexible we are applying thiS `**kwargs` pattern to the function above.
 ## A first example
 
 A first example is a risk model based on the sample covariance matrix.
 We construct the risk model as follows
 
 ```python
 import numpy as np
@@ -73,16 +75,16 @@
 ```
 
 The risk model and the actual optimization problem are decoupled.
 This is good practice and keeps the code clean and maintainable.
 
 In a backtest we don't have to reconstruct the problem in every iteration.
 We can simply update the risk model with the new data and solve the problem again.
-If the dimension of the problem is changing during the test we expect
-a new problem has to be constructed though.
+The implementation of the risk models is flexible enough to deal with changing dimensions
+of the underlying weight space.
 
 ## Risk models
 
 ### Sample covariance
 
 We offer a `SampleCovariance` class as seen above.
 
@@ -94,20 +96,20 @@
 ```math
 r_i = \sum_{j=1}^k f_j \beta_{ji} + \epsilon_i
 ```
 The factor time series are $f_1, \ldots, f_k$. The loadings are the coefficients
 $\beta_{ji}$.
 The residual returns $\epsilon_i$ are assumed to be uncorrelated with the factors.
 
-Any position $w$ in weight space projects to a position $y = \beta w$ in factor space.
+Any position $w$ in weight space projects to a position $y = \beta^T w$ in factor space.
 The variance for a position $w$ is the sum of the variance of the
 systematic returns explained by the factors and the variance of the idiosyncratic returns.
 
 ```math
-Var(r) = Var(\beta w) + Var(\epsilon w)
+Var(r) = Var(\beta^T w) + Var(\epsilon w)
 ```
 
 We assume the residual returns are uncorrelated and hence
 
 ```math
 Var(r) = y^T \Sigma_f y + \sum_i w_i^2 Var(\epsilon_i)
 ```
@@ -127,16 +129,15 @@
 of the observed residuals.
 The factor covariance matrix $\Sigma_f$ may even be diagonal in this case as the factors are orthogonal.
 
 We expose a method to compute the first $k$ principal components.
 
 ### cvar
 
-XXX: Conditional value at risk
-Relies on cxxpy's `sum_largest` function.
+We currently also support the conditional value at risk (CVaR) as a risk measure.
 
 
 
 
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
```

