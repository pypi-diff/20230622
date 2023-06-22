# Comparing `tmp/sam_ml-py-0.4.2.tar.gz` & `tmp/sam_ml-py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sam_ml-py-0.4.2.tar", last modified: Fri Jun 16 18:36:23 2023, max compression
+gzip compressed data, was "sam_ml-py-0.5.0.tar", last modified: Thu Jun 22 06:54:01 2023, max compression
```

## Comparing `sam_ml-py-0.4.2.tar` & `sam_ml-py-0.5.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.587647 sam_ml-py-0.4.2/sam_ml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.587647 sam_ml-py-0.4.2/sam_ml/config/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/config/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.591647 sam_ml-py-0.4.2/sam_ml/data/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/data/synthetic_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.595647 sam_ml-py-0.4.2/sam_ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/AdaBoostClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/BaggingClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/BernoulliNB.py
--rw-r--r--   0 runner    (1001) docker     (123)    16019 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/ClassifierTest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/DecisionTreeClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/ExtraTreesClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/GaussianNB.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/GaussianProcessClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/GradientBoostingMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/KNeighborsClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/LinearDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/LinearSupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/LogisticRegression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/MLPClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/QuadraticDiscriminantAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/RandomForestClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/SupportVectorClassifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16681 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/main_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/main_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/main_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/sam_ml/models/scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/sam_ml_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-16 18:36:23.000000 sam_ml-py-0.4.2/sam_ml_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 18:36:23.599647 sam_ml-py-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-16 18:36:13.000000 sam_ml-py-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.682299 sam_ml-py-0.5.0/sam_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.682299 sam_ml-py-0.5.0/sam_ml/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/config/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.682299 sam_ml-py-0.5.0/sam_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/data/synthetic_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.686299 sam_ml-py-0.5.0/sam_ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/AdaBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/BaggingClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/BernoulliNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16163 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/ClassifierTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/DecisionTreeClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/ExtraTreesClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/GaussianNB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/GaussianProcessClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/GradientBoostingMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/KNeighborsClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/LinearDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/LinearSupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/LogisticRegression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/MLPClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/QuadraticDiscriminantAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/RandomForestClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/SupportVectorClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/XGBoostClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20573 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/main_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/main_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9806 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/main_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/sam_ml/models/scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/sam_ml_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 06:54:01.000000 sam_ml-py-0.5.0/sam_ml_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 06:54:01.690299 sam_ml-py-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 06:53:50.000000 sam_ml-py-0.5.0/setup.py
```

### Comparing `sam_ml-py-0.4.2/LICENSE` & `sam_ml-py-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/PKG-INFO` & `sam_ml-py-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam_ml-py
-Version: 0.4.2
+Version: 0.5.0
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sam_ml-py-0.4.2/README.md` & `sam_ml-py-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/config/logging.py` & `sam_ml-py-0.5.0/sam_ml/config/logging.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/data/embeddings.py` & `sam_ml-py-0.5.0/sam_ml/data/embeddings.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/data/feature_selection.py` & `sam_ml-py-0.5.0/sam_ml/data/feature_selection.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/data/sampling.py` & `sam_ml-py-0.5.0/sam_ml/data/sampling.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/data/scaler.py` & `sam_ml-py-0.5.0/sam_ml/data/scaler.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/data/synthetic_data.py` & `sam_ml-py-0.5.0/sam_ml/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/models/AdaBoostClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/AdaBoostClassifier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from numpy import arange
+from ConfigSpace import Beta, Categorical, ConfigurationSpace, Float, Integer
 from sklearn.ensemble import (AdaBoostClassifier, GradientBoostingClassifier,
                               RandomForestClassifier)
 from sklearn.linear_model import LogisticRegression
 from sklearn.svm import SVC
 from sklearn.tree import DecisionTreeClassifier
 
 from .main_classifier import Classifier
@@ -15,33 +15,32 @@
         self,
         model_name: str = "AdaBoostClassifier",
         random_state: int = 42,
         **kwargs,
     ):
         """
         @param (important one):
-            base_estimator: base estimator from which the boosted ensemble is built (default: DecisionTreeClassifier with max_depth=1)
+            estimator: base estimator from which the boosted ensemble is built (default: DecisionTreeClassifier with max_depth=1)
             n_estimator: number of boosting stages to perform
             learning_rate: shrinks the contribution of each tree by learning rate
             algorithm: boosting algorithm
             random_state: random_state for model
         """
         model_type = "ABC"
         model = AdaBoostClassifier(
             random_state=random_state,
             **kwargs,
         )
-        if type(model.base_estimator) == RandomForestClassifier:
-            grid = {
-                "base_estimator": [RandomForestClassifier(max_depth=i, n_estimators=j) for i in range(1,11) for j in (5, 10, 20, 50, 100)]+[SVC(probability=True, kernel='linear'), LogisticRegression(), GradientBoostingClassifier()],
-                "n_estimators": list(range(10, 101, 10)) + [200, 500, 1000, 1500, 3000],
-                "learning_rate": [0.1, 0.05, 0.01, 0.005]+list(arange(0.2,2.1,0.1)),
-                "algorithm": ["SAMME.R", "SAMME"],
-            }
+        if type(model.estimator) == RandomForestClassifier:
+            core_estimator = [RandomForestClassifier(max_depth=i, n_estimators=j) for i in range(1,11) for j in (5, 10, 20, 50, 100)]
         else:
-            grid = {
-                "base_estimator": [DecisionTreeClassifier(max_depth=i) for i in range(1,11)]+[SVC(probability=True, kernel='linear'), LogisticRegression(), GradientBoostingClassifier()],
-                "n_estimators": list(range(10, 101, 10)) + [200, 500, 1000, 1500, 3000],
-                "learning_rate": [0.1, 0.05, 0.01, 0.005]+list(arange(0.2,2.1,0.1)),
-                "algorithm": ["SAMME.R", "SAMME"],
-            }
+            core_estimator= [DecisionTreeClassifier(max_depth=i) for i in range(1,11)]
+        
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "estimator": Categorical("estimator", core_estimator+[SVC(probability=True, kernel='linear'), LogisticRegression(), GradientBoostingClassifier()]),
+            "n_estimators": Integer("n_estimators", (10, 3000), log=True),
+            "learning_rate": Float("learning_rate", (0.005, 2), distribution=Beta(10, 5)),
+            "algorithm": Categorical("algorithm", ["SAMME.R", "SAMME"]),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/BernoulliNB.py` & `sam_ml-py-0.5.0/sam_ml/models/BernoulliNB.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Integer
 from sklearn.naive_bayes import BernoulliNB
 
 from .main_classifier import Classifier
 
 
 class BNB(Classifier):
     """ BernoulliNB Wrapper class """
@@ -14,12 +15,14 @@
         """
         @params (important one):
             binarize: threshold for binarizing (mapping to booleans) of sample features. If None, input is presumed to already consist of binary vectors
             fit_prior: whether to learn class prior probabilities or not. If false, a uniform prior will be used
         """
         model_type = "BNB"
         model = BernoulliNB(**kwargs,)
-        grid = {
-            "fit_prior": [True, False],
-            "binarize": list(range(0, 10)),
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "fit_prior": Categorical("fit_prior", [True, False]),
+            "binarize": Integer("binarize", (0, 10)),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/ClassifierTest.py` & `sam_ml-py-0.5.0/sam_ml/models/ClassifierTest.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,25 +144,25 @@
                 DTC(),
                 RFC(),
                 SVC(model_name="SupportVectorClassifier (rbf-kernel)"),
                 GBM(),
                 
                 ABC(model_name="AdaBoostClassifier (DTC based)"),
                 ABC(
-                    base_estimator=RandomForestClassifier(max_depth=5, random_state=42),
+                    estimator=RandomForestClassifier(max_depth=5, random_state=42),
                     model_name="AdaBoostClassifier (RFC based)",
                 ),
                 KNC(),
                 ETC(),
                 GNB(),
                 BNB(),
                 GPC(),
                 BC(model_name="BaggingClassifier (DTC based)"),
                 BC(
-                    base_estimator=RandomForestClassifier(max_depth=5, random_state=42),
+                    estimator=RandomForestClassifier(max_depth=5, random_state=42),
                     model_name="BaggingClassifier (RFC based)",
                 ),
             ]
         elif kind == "basic":
             models = [
                 LR(),
                 MLPC(),
@@ -296,92 +296,92 @@
                 print(scores)
         else:
             logger.warning("no scores are created -> use 'eval_models()'/'eval_models_cv()' to create scores")
             scores = None
 
         return scores
 
-    def find_best_model(
-        self,
-        x_train: pd.DataFrame,
-        y_train: pd.Series,
-        x_test: pd.DataFrame,
-        y_test: pd.Series,
-        cv_kind: str = "no",
-        scoring: str = "accuracy",
-        avg: str = "macro",
-        pos_label: Union[int, str] = -1,
-        rand_search: bool = True,
-        n_iter_num: int = 75,
-        cv_num: int = 10,
-        console_out: bool = False,
-        secondary_scoring: str = None,
-        strength: int = 3,
-    ) -> Pipeline:
-        """
-        @param:
-            cv_kind: which kind of cross validation shall be used to create the scores to find the best model type
-                'no': use eval_models on x_train, y_train, x_test, y_test
-                'small': use eval_models_cv with small_data_eval=True on x_train, y_train
-                'multi': use eval_models_cv with small_data_eval=False on x_train, y_train
-            scoring: "accuracy" / "precision" / "recall" / "s_score" / "l_score"
-
-            avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
-            pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
-            rand_search: True: RandomizedSearchCV, False: GridSearchCV
-            n_iter_num: Combinations to try out if rand_search=True
-            cv_num: number of different splits
-            console_out: outputs intermidiate results into the console
-            secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
-
-        @return:
-            - prints parameters and metrics of best model
-            - saves best model in self.best_model
-            - returns best model
-        """
-
-        if cv_kind == "no":
-            logger.debug("creating scores using 'eval_models()'")
-            self.eval_models(x_train, y_train, x_test, y_test, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
-        elif cv_kind == "small":
-            logger.debug("creating scores using 'eval_models_cv(small_data_eval=True)'")
-            self.eval_models_cv(x_train, y_train, avg=avg, pos_label=pos_label, small_data_eval=True, secondary_scoring=secondary_scoring, strength=strength)
-        elif cv_kind == "multi":
-            logger.debug("creating scores using 'eval_models_cv(small_data_eval=False)'")
-            self.eval_models_cv(x_train, y_train, avg=avg, pos_label=pos_label, small_data_eval=False, secondary_scoring=secondary_scoring, strength=strength, cv_num=cv_num)
-        else:
-            logger.error(f"wrong input '{cv_kind}' for cv_kind")
-            return
-
-        sorted_scores = self.output_scores_as_pd(sort_by=[scoring, "s_score"])
-        best_model_type = sorted_scores.iloc[0].name
-        best_model_value = sorted_scores.iloc[0][scoring]
-
-        print()
-        print(f"best model type ({scoring}): ", best_model_type, " - ", best_model_value)
-        print()
-
-        logger.info(f"hyperparametertuning for best model type (rand_search = {rand_search}) - started")
-        self.models[best_model_type].gridsearch(
-            x_train,
-            y_train,
-            scoring=scoring,
-            train_afterwards=True,
-            avg=avg,
-            pos_label=pos_label,
-            rand_search=rand_search,
-            n_iter_num=n_iter_num,
-            cv_num=cv_num,
-            console_out=console_out,
-            secondary_scoring=secondary_scoring,
-            strength=strength,
-        )
-        logger.info(f"hyperparametertuning for best model type (rand_search = {rand_search}) - finished")
-
-        # Set self.best_model = hyperparameter tuned model
-        self.best_model = self.models[best_model_type]
-
-        self.best_model.evaluate(x_test, y_test, avg=avg, pos_label=pos_label)
-        self.best_model.feature_importance()
-        self.__finish_sound()
-        return self.best_model
+    # def find_best_model(
+    #     self,
+    #     x_train: pd.DataFrame,
+    #     y_train: pd.Series,
+    #     x_test: pd.DataFrame,
+    #     y_test: pd.Series,
+    #     cv_kind: str = "no",
+    #     scoring: str = "accuracy",
+    #     avg: str = "macro",
+    #     pos_label: Union[int, str] = -1,
+    #     rand_search: bool = True,
+    #     n_iter_num: int = 75,
+    #     cv_num: int = 10,
+    #     console_out: bool = False,
+    #     secondary_scoring: str = None,
+    #     strength: int = 3,
+    # ) -> Pipeline:
+    #     """
+    #     @param:
+    #         cv_kind: which kind of cross validation shall be used to create the scores to find the best model type
+    #             'no': use eval_models on x_train, y_train, x_test, y_test
+    #             'small': use eval_models_cv with small_data_eval=True on x_train, y_train
+    #             'multi': use eval_models_cv with small_data_eval=False on x_train, y_train
+    #         scoring: "accuracy" / "precision" / "recall" / "s_score" / "l_score"
+
+    #         avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
+    #         pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
+    #         rand_search: True: RandomizedSearchCV, False: GridSearchCV
+    #         n_iter_num: Combinations to try out if rand_search=True
+    #         cv_num: number of different splits
+    #         console_out: outputs intermidiate results into the console
+    #         secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
+    #         strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+
+    #     @return:
+    #         - prints parameters and metrics of best model
+    #         - saves best model in self.best_model
+    #         - returns best model
+    #     """
+
+    #     if cv_kind == "no":
+    #         logger.debug("creating scores using 'eval_models()'")
+    #         self.eval_models(x_train, y_train, x_test, y_test, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
+    #     elif cv_kind == "small":
+    #         logger.debug("creating scores using 'eval_models_cv(small_data_eval=True)'")
+    #         self.eval_models_cv(x_train, y_train, avg=avg, pos_label=pos_label, small_data_eval=True, secondary_scoring=secondary_scoring, strength=strength)
+    #     elif cv_kind == "multi":
+    #         logger.debug("creating scores using 'eval_models_cv(small_data_eval=False)'")
+    #         self.eval_models_cv(x_train, y_train, avg=avg, pos_label=pos_label, small_data_eval=False, secondary_scoring=secondary_scoring, strength=strength, cv_num=cv_num)
+    #     else:
+    #         logger.error(f"wrong input '{cv_kind}' for cv_kind")
+    #         return
+
+    #     sorted_scores = self.output_scores_as_pd(sort_by=[scoring, "s_score"])
+    #     best_model_type = sorted_scores.iloc[0].name
+    #     best_model_value = sorted_scores.iloc[0][scoring]
+
+    #     print()
+    #     print(f"best model type ({scoring}): ", best_model_type, " - ", best_model_value)
+    #     print()
+
+    #     logger.info(f"hyperparametertuning for best model type (rand_search = {rand_search}) - started")
+    #     self.models[best_model_type].gridsearch(
+    #         x_train,
+    #         y_train,
+    #         scoring=scoring,
+    #         train_afterwards=True,
+    #         avg=avg,
+    #         pos_label=pos_label,
+    #         rand_search=rand_search,
+    #         n_iter_num=n_iter_num,
+    #         cv_num=cv_num,
+    #         console_out=console_out,
+    #         secondary_scoring=secondary_scoring,
+    #         strength=strength,
+    #     )
+    #     logger.info(f"hyperparametertuning for best model type (rand_search = {rand_search}) - finished")
+
+    #     # Set self.best_model = hyperparameter tuned model
+    #     self.best_model = self.models[best_model_type]
+
+    #     self.best_model.evaluate(x_test, y_test, avg=avg, pos_label=pos_label)
+    #     self.best_model.feature_importance()
+    #     self.__finish_sound()
+    #     return self.best_model
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/DecisionTreeClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/DecisionTreeClassifier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Integer
 from sklearn.tree import DecisionTreeClassifier
 
 from .main_classifier import Classifier
 
 
 class DTC(Classifier):
     """ DecisionTreeClassifier Wrapper class """
@@ -21,14 +22,16 @@
             random_state: random_state for model
         """
         model_type = "DTC"
         model = DecisionTreeClassifier(
             random_state=random_state,
             **kwargs,
         )
-        grid = {
-            "criterion": ["gini", "entropy"],
-            "max_depth": list(range(1, 10)),
-            "min_samples_split": list(range(2, 10)),
-            "min_samples_leaf": list(range(1, 5)),
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "criterion": Categorical("criterion", ["gini", "entropy"]),
+            "max_depth": Integer("max_depth", (1, 10)),
+            "min_samples_split": Integer("min_samples_split", (2, 10)),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 5)),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/ExtraTreesClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/ExtraTreesClassifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Integer, Normal
 from sklearn.ensemble import ExtraTreesClassifier
 
 from .main_classifier import Classifier
 
 
 class ETC(Classifier):
     """ ExtraTreesClassifier Wrapper class """
@@ -30,16 +31,18 @@
         """
         model_type = "ETC"
         model = ExtraTreesClassifier(
             n_jobs=n_jobs,
             random_state=random_state,
             **kwargs,
         )
-        grid = {
-            "n_estimators": [1, 2, 4, 8, 16, 32, 64, 100, 200, 500, 1000],
-            "max_depth": [2, 3, 4, 5, 6, 7, 8, 10, 15],
-            "min_samples_split": [2, 3, 5, 10],
-            "min_samples_leaf": [1, 2, 4],
-            "bootstrap": [True, False],
-            "criterion": ["gini", "entropy"],
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True),
+            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3)),
+            "min_samples_split": Integer("min_samples_split", (2, 10)),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4)),
+            "bootstrap": Categorical("bootstrap", [True, False], default=False),
+            "criterion": Categorical("criterion", ["gini", "entropy"]),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/GaussianNB.py` & `sam_ml-py-0.5.0/sam_ml/models/GaussianNB.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import ConfigurationSpace, Float
 from sklearn.naive_bayes import GaussianNB
 
 from .main_classifier import Classifier
 
 
 class GNB(Classifier):
     """ GaussianNB Wrapper class """
@@ -14,11 +15,13 @@
         """
         @params:
             priors: Prior probabilities of the classes. If specified the priors are not adjusted according to the data
             var_smoothing: Portion of the largest variance of all features that is added to variances for calculation stability
         """
         model_type = "GNB"
         model = GaussianNB(**kwargs,)
-        grid = {
-            "var_smoothing": [10**i for i in range(-11, 1)]
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "var_smoothing": Float("var_smoothing", (0.00000000001, 1), log=True)
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/GaussianProcessClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/GaussianProcessClassifier.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Integer
 from sklearn.gaussian_process import GaussianProcessClassifier
 
 from .main_classifier import Classifier
 
 
 class GPC(Classifier):
     """ GaussianProcessClassifier Wrapper class """
@@ -18,12 +19,14 @@
             multi_class: specifies how multi-class classification problems are handled
             max_iter_predict: the maximum number of iterations in Newton's method for approximating the posterior during predict
         """
         model_type = "GPC"
         model = GaussianProcessClassifier(
             n_jobs=n_jobs, random_state=random_state, **kwargs,
         )
-        grid = {
-            "multi_class": ["one_vs_rest", "one_vs_one"],
-            "max_iter_predict": [1, 10, 50, 100, 200, 500, 1000],
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "multi_class": Categorical("multi_class", ["one_vs_rest", "one_vs_one"]),
+            "max_iter_predict": Integer("max_iter_predict", (1, 1000), log=True),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/GradientBoostingMachine.py` & `sam_ml-py-0.5.0/sam_ml/models/GradientBoostingMachine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Float, Integer, Normal
 from sklearn.ensemble import GradientBoostingClassifier
 
 from .main_classifier import Classifier
 
 
 class GBM(Classifier):
     """ GradientBoostingMachine Wrapper class """
@@ -25,19 +26,21 @@
             learning_rate: shrinks the contribution of each tree by learning rate
 
             warm_start: work with previous fit and add more estimator
             random_state: random_state for model
         """
         model_type = "GBM"
         model = GradientBoostingClassifier(random_state=random_state, **kwargs,)
-        grid = {
-            "n_estimators": list(range(20, 101, 10)) + [200, 500, 1000, 1500],
-            "max_depth": list(range(1, 8)) + [10, 12, 15],
-            "min_samples_split": [2, 4, 6, 8, 10, 20, 40, 60, 100],
-            "min_samples_leaf": [2, 4, 6, 8, 10, 20, 40, 60, 100],
-            "max_features": ["auto", "sqrt", "log2", None],
-            "subsample": [0.7, 0.75, 0.8, 0.85, 0.9, 0.95, 1],
-            "criterion": ["friedman_mse", "mse"],
-            "loss": ["deviance", "exponential"],
-            "learning_rate": [0.1, 0.05, 0.01, 0.005],
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "n_estimators": Integer("n_estimators", (20, 1500), log=True),
+            "max_depth": Integer("max_depth", (1, 15), distribution=Normal(4, 4)),
+            "min_samples_split": Integer("min_samples_split", (2, 100), log=True),
+            "min_samples_leaf": Integer("min_samples_leaf", (2, 100), log=True),
+            "max_features": Categorical("max_features", ["auto", "sqrt", "log2"]),
+            "subsample": Float("subsample", (0.7, 1)),
+            "criterion": Categorical("criterion", ["friedman_mse", "mse"]),
+            "loss": Categorical("loss", ["deviance", "exponential"]),
+            "learning_rate": Float("learning_rate", (0.005, 0.1), log=True),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/KNeighborsClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/KNeighborsClassifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Integer
 from sklearn.neighbors import KNeighborsClassifier
 
 from .main_classifier import Classifier
 
 
 class KNC(Classifier):
     """ KNeighborsClassifier Wrapper class """
@@ -18,14 +19,16 @@
             algorithm: Algorithm used to compute the nearest neighbors
             leaf_size: Leaf size passed to BallTree or KDTree
             p: number of metric that is used (manhattan, euclidean, minkowski)
             n_jobs: the number of parallel jobs to run for neighbors search [problem with n_jobs = -1 --> kernel dies]
         """
         model_type = "KNC"
         model = KNeighborsClassifier(**kwargs,)
-        grid = {
-            "n_neighbors": list(range(1,30)),
-            "p": [1, 2, 3, 4, 5],
-            "leaf_size": list(range(1,50)),
-            "weights": ["uniform", "distance"],
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "n_neighbors": Integer("n_neighbors", (1, 30)),
+            "p": Integer("p", (1, 5)),
+            "leaf_size": Integer("leaf_size", (1, 50)),
+            "weights": Categorical("weights", ["uniform", "distance"]),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/LinearSupportVectorClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/LinearSupportVectorClassifier.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Float
 from sklearn.svm import LinearSVC
 
 from .main_classifier import Classifier
 
 
 class LSVC(Classifier):
     """ LinearSupportVectorClassifier Wrapper class """
@@ -22,13 +23,15 @@
             max_iter: Maximum number of iterations taken for the solvers to converge
         """
         model_type = "LSVC"
         model = LinearSVC(
             random_state=random_state,
             **kwargs,
         )
-        grid = {
-            "penalty": ["l1", "l2"],
-            "dual": [True, False],
-            "C": [10**i for i in range(-5, 6)]
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "penalty": Categorical("penalty", ["l1", "l2"]),
+            "dual": Categorical("dual", [True, False]),
+            "C": Float("C", (0.00001, 1000000), log=True),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/LogisticRegression.py` & `sam_ml-py-0.5.0/sam_ml/models/LogisticRegression.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import numpy as np
+from ConfigSpace import (Categorical, ConfigurationSpace, EqualsCondition,
+                         Float, ForbiddenAndConjunction, ForbiddenEqualsClause,
+                         ForbiddenInClause)
 from sklearn.linear_model import LogisticRegression
 
 from .main_classifier import Classifier
 
 
 class LR(Classifier):
     """ LogisticRegression Wrapper class """
@@ -27,21 +30,23 @@
             penalty: Specify the norm of the penalty
         """
         model_type = "LR"
         model = LogisticRegression(
             random_state=random_state,
             **kwargs,
         )
-        if model.penalty == "l2":
-            grid = {
-                "solver": ["newton-cg", "lbfgs", "liblinear", "sag", "saga"],
-                "penalty": ["l2"],
-                "C": [100, 10, 1.0, 0.1, 0.01],
-            }
-        else:
-            grid = {
-                "solver": ["saga"],
-                "penalty": ["elasticnet"],
-                "C": [100, 10, 1.0, 0.1, 0.01],
-                "l1_ratio": list(np.linspace(0, 1, num=5))+[0.01],
-            }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "solver": Categorical("solver", ["newton-cg", "lbfgs", "liblinear", "sag", "saga"], weights=[0.15, 0.15, 0.15, 0.15, 0.4], default="lbfgs"),
+            "penalty": Categorical("penalty", ["l2", "elasticnet"]),
+            "C": Float("C", (0.01, 100), log=True),
+            "l1_ratio": Float("l1_ratio", (0.01, 1)),
+            })
+        solver_and_penalty = ForbiddenAndConjunction(
+            ForbiddenEqualsClause(grid["penalty"], "elasticnet"),
+            ForbiddenInClause(grid["solver"], ["newton-cg", "lbfgs", "liblinear", "sag"]),
+        )
+        l1_ratio_cond = EqualsCondition(grid["l1_ratio"], grid["penalty"], "elasticnet")
+        grid.add_forbidden_clause(solver_and_penalty)
+        grid.add_condition(l1_ratio_cond)
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/MLPClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/MLPClassifier.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Float
 from sklearn.neural_network import MLPClassifier
 
 from .main_classifier import Classifier
 
 
 class MLPC(Classifier):
     """ MLP Classifier Wrapper class """
@@ -29,15 +30,17 @@
             early_stopping: True: tests on 10% of train data and stops if there is for 'n_iter_no_change' no improvement in the metrics
         """
         model_type = "MLPC"
         model = MLPClassifier(
             random_state=random_state,
             **kwargs,
         )
-        grid = {
-            "hidden_layer_sizes": [(10, 30, 10), (20,), (10,), (100,), (50,50,50), (50,100,50)],
-            "activation": ["tanh", "relu", "logistic"],
-            "solver": ["sgd", "adam"],
-            "alpha": [0.0001, 0.001, 0.01, 0.05],
-            "learning_rate": ["constant", "adaptive"],
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "hidden_layer_sizes": Categorical("hidden_layer_sizes", ((10, 30, 10), (20,), (10,), (100,), (50,50,50), (50,100,50))),
+            "activation": Categorical("activation", ["tanh", "relu", "logistic"]),
+            "solver": Categorical("solver", ["sgd", "adam"]),
+            "alpha": Float("alpha", (0.0001, 0.05), log=True),
+            "learning_rate": Categorical("learning_rate", ["constant", "adaptive"]),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/RandomForestClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/RandomForestClassifier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Integer, Normal
 from sklearn.ensemble import RandomForestClassifier
 
 from .main_classifier import Classifier
 
 
 class RFC(Classifier):
     """ RandomForestClassifier Wrapper class """
@@ -30,16 +31,18 @@
         """
         model_type = "RFC"
         model = RandomForestClassifier(
             n_jobs=n_jobs,
             random_state=random_state,
             **kwargs,
         )
-        grid = {
-            "n_estimators": [1, 2, 4, 8, 16, 32, 64, 100, 200, 500, 1000],
-            "max_depth": [2, 3, 4, 5, 6, 7, 8, 10, 15],
-            "min_samples_split": [2, 3, 5, 10],
-            "min_samples_leaf": [1, 2, 4],
-            "bootstrap": [True, False],
-            "criterion": ["gini", "entropy"],
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "n_estimators": Integer("n_estimators", (10, 1000), log=True),
+            "max_depth": Integer("max_depth", (3, 15), distribution=Normal(5, 3)),
+            "min_samples_split": Integer("min_samples_split", (2, 10)),
+            "min_samples_leaf": Integer("min_samples_leaf", (1, 4)),
+            "bootstrap": Categorical("bootstrap", [True, False], default=True),
+            "criterion": Categorical("criterion", ["gini", "entropy"]),
+            })
         super().__init__(model, model_name, model_type, grid)
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/SupportVectorClassifier.py` & `sam_ml-py-0.5.0/sam_ml/models/SupportVectorClassifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from ConfigSpace import Categorical, ConfigurationSpace, Float
 from sklearn.svm import SVC as svc
 
 from .main_classifier import Classifier
 
 
 class SVC(Classifier):
     """ SupportVectorClassifier Wrapper class """
@@ -28,20 +29,22 @@
         """
         model_type = "SVC"
         model = svc(
             kernel=kernel,
             random_state=random_state,
             **kwargs,
         )
-        grid = {
-            "kernel": ["rbf", "poly", "sigmoid"],
-            "gamma": [1, 0.1, 0.01, 0.001, 0.0001, "scale", "auto"],
-            "C": [0.1, 1, 10, 100, 1000],
-            "probability": [True, False],
-        }
+        grid = ConfigurationSpace(
+            seed=42,
+            space={
+            "kernel": Categorical("kernel", ["rbf", "poly", "sigmoid"]),
+            "gamma": Float("gamma", (0.0001, 1), log=True),
+            "C": Float("C", (0.1, 1000), log=True),
+            "probability": Categorical("probability", [True, False]),
+            })
         super().__init__(model, model_name, model_type, grid)
 
     def feature_importance(self):
         if self.model.kernel == "linear":
             super().feature_importance()
         else:
             print(f"feature importance is only available for a linear kernel. You are currently using: {self.model.kernel}")
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/__init__.py` & `sam_ml-py-0.5.0/sam_ml/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .main_classifier import Classifier
 from .main_model import Model
 from .main_pipeline import Pipeline
 from .MLPClassifier import MLPC
 from .QuadraticDiscriminantAnalysis import QDA
 from .RandomForestClassifier import RFC
 from .SupportVectorClassifier import SVC
+from .XGBoostClassifier import XGBC
 
 __all__ = {
     "model parent class": "Model",
     "classifier parent class": "Classifier",
     "pipeline class": "Pipeline",
     "AutoML class": "CTest",
     "RandomForestClassifier": "RFC",
@@ -36,8 +37,9 @@
     "GaussianNaiveBayes": "GNB",
     "BernoulliNaiveBayes": "BNB",
     "GaussianProcessClassifier": "GPC",
     "QuadraticDiscriminantAnalysis": "QDA",
     "LinearDiscriminantAnalysis": "LDA",
     "BaggingClassifier": "BC",
     "LinearSupportVectorClassifier": "LSVC",
+    "XGBoostClassifier": "XGBC",
 }
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/main_classifier.py` & `sam_ml-py-0.5.0/sam_ml/models/main_classifier.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+from copy import copy
 from datetime import timedelta
 from statistics import mean
 from typing import Union
 
 import numpy as np
 import pandas as pd
+from ConfigSpace import Configuration, ConfigurationSpace
 from matplotlib import pyplot as plt
 from sklearn.metrics import (accuracy_score, classification_report,
                              make_scorer, precision_score, recall_score)
 from sklearn.model_selection import (GridSearchCV, RandomizedSearchCV,
                                      cross_validate)
+# from smac import (HyperparameterOptimizationFacade, MultiFidelityFacade,
+#                   RandomFacade, Scenario)
 from tqdm.auto import tqdm
 
 from sam_ml.config import setup_logger
 
 from .main_model import Model
 from .scorer import l_scoring, s_scoring
 
@@ -30,14 +34,15 @@
             model_type: kind of estimator (e.g. 'RFC' for RandomForestClassifier)
             grid: hyperparameter grid for the model
         """
         super().__init__(model_object, model_name, model_type)
         self._grid = grid
         self.is_pipeline = is_pipeline
         self.cv_scores: dict[str, float] = {}
+        self.rCVsearch_results: pd.DataFrame|None = None
 
     def __repr__(self) -> str:
         params: str = ""
         param_dict = self.get_params(False)
         for key in param_dict:
             if type(param_dict[key]) == str:
                 params+= key+"='"+str(param_dict[key])+"', "
@@ -50,25 +55,35 @@
     @property
     def grid(self):
         """
         @return:
             hyperparameter tuning grid of the model
         """
         return self._grid
+    
+    def get_random_params(self):
+        """
+        @return;
+            set of random parameter from grid
+        """
+        return dict(self.grid.sample_configuration(1))
 
-    def update_grid(self, **kwargs):
+    def replace_grid(self, new_grid: ConfigurationSpace):
         """
-        function to update self.grid 
+        function to replace self.grid 
 
         e.g.:
-            - model.grid {"n_estimators": [3, 4, 5]}
-            - model.update_grid(n_estimators = [10, 3, 5], solver = ["sag", "l1"])
-            - model.grid {"n_estimators": [10, 3, 5], "solver": ["sag", "l1"]}
+            ConfigurationSpace(
+                seed=42,
+                space={
+                    "solver": Categorical("solver", ["lsqr", "eigen", "svd"]),
+                    "shrinkage": Float("shrinkage", (0, 1)),
+                })
         """
-        self._grid.update(kwargs)
+        self._grid = new_grid
 
     def evaluate(
         self,
         x_test: pd.DataFrame,
         y_test: pd.Series,
         avg: str = None,
         pos_label: Union[int, str] = -1,
@@ -283,15 +298,15 @@
         """
         if not self.trained:
             logger.error("You have to first train the classifier before getting the feature importance")
             return
 
         if self.model_type == "MLPC":
             importances = [np.mean(i) for i in self.model.coefs_[0]]  # MLP Classifier
-        elif self.model_type in ("DTC", "RFC", "GBM", "CBC", "ABC", "ETC"):
+        elif self.model_type in ("DTC", "RFC", "GBM", "CBC", "ABC", "ETC", "XGBC"):
             importances = self.model.feature_importances_
         elif self.model_type in ("KNC", "GNB", "BNB", "GPC", "QDA", "BC"):
             logger.warning(f"{self.model_name} does not have a feature importance")
             return
         else:
             importances = self.model.coef_[0]  # "normal"
 
@@ -306,122 +321,204 @@
             elif self.model_type == "GBM":
                 std = np.std(
                     [tree[0].feature_importances_ for tree in self.model.estimators_], axis=0,
                 )
             feature_importances.plot.bar(yerr=std, ax=ax)
         else:
             feature_importances.plot.bar(ax=ax)
-        ax.set_title("Feature importances of " + self.model_name)
+        ax.set_title("Feature importances of " + str(self.model_name))
         ax.set_ylabel("use of coefficients as importance scores")
         fig.tight_layout()
         plt.show()
+    
+    # def smac_search(
+    #         self,
+    #         x_train: pd.DataFrame, 
+    #         y_train: pd.Series
+    # ):
+    #     # Next, we create an object, holding general information about the run
+    #     scenario = Scenario(
+    #         self.grid,
+    #         n_trials=5,  # We want to run max 50 trials (combination of config and seed)
+    #         deterministic=True,
+    #         min_budget=5,
+    #         max_budget=25,
+    #     )
+
+    #     # We want to run the facade's default initial design, but we want to change the number
+    #     # of initial configs to 5.
+    #     initial_design = MultiFidelityFacade.get_initial_design(scenario)
+
+    #     # define target function
+    #     def grid_train(config: Configuration, seed: int, budget) -> float:
+    #         print(config)
+    #         print(seed)
+    #         print(budget)
+    #         params = self.get_params()
+    #         #print(params)
+    #         params.update(config)
+    #         #print(params)
+    #         model = type(self)(**params)
+    #         score = model.cross_validation(x_train, y_train, console_out=False, cv_num=2)
+    #         print(1 - score["accuracy"])
+    #         return 1 - score["accuracy"]  # SMAC always minimizes (the smaller the better)
+
+    #     # Now we use SMAC to find the best hyperparameters
+    #     smac = MultiFidelityFacade(
+    #         scenario,
+    #         grid_train,
+    #         initial_design=initial_design,
+    #         overwrite=True,  # If the run exists, we overwrite it; alternatively, we can continue from last state
+    #     )
+
+    #     incumbent = smac.optimize()
+
+    #     # Get cost of default configuration
+    #     default_cost = smac.validate(self.grid.get_default_configuration())
+    #     print(f"Default cost: {default_cost}")
+
+    #     # Let's calculate the cost of the incumbent
+    #     incumbent_cost = smac.validate(incumbent)
+    #     print(f"Incumbent cost: {incumbent_cost}")
 
-    def gridsearch(
+    def randomCVsearch(
         self,
         x_train: pd.DataFrame,
         y_train: pd.Series,
-        grid: dict = None,
+        n_trails: int = 10,
+        cv_num: int = 5,
         scoring: str = "accuracy",
         avg: str = "macro",
-        pos_label: Union[int, str] = 1,
-        cv_num: int = 10,
-        verbose: int = 0,
-        rand_search: bool = True,
-        n_iter_num: int = 75,
-        console_out: bool = True,
-        train_afterwards: bool = True,
+        pos_label: Union[int, str] = -1,
         secondary_scoring: str = None,
         strength: int = 3,
     ):
-        """
-        @param:
-            x_train: DataFrame with train features
-            y_train: Series with labels
-
-            grid: dictonary of parameters to tune (default: default parameter dictionary self.grid)
-
-            scoring: metrics to evaluate the models
-            avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
-            pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
-
-            rand_search: True: RandomizedSearchCV, False: GridSearchCV
-            n_iter_num: Combinations to try out if rand_search=True
-
-            cv_num: number of different splits
-
-            verbose: log level (higher number --> more logs)
-            console_out: output the the results of the different iterations
-            train_afterwards: train the best model after finding it
-
-            secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
-            strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
-
-        @return:
-            set self.model = best model from search
-        """
-        if grid is None:
-            grid = self.grid
-
-        if console_out:
-            print()
-            print("grid: ", grid)
-            print()
-
-        if scoring == "precision":
-            scoring = make_scorer(precision_score, average=avg, pos_label=pos_label)
-        elif scoring == "recall":
-            scoring = make_scorer(recall_score, average=avg, pos_label=pos_label)
-        elif scoring == "s_score":
-            scoring = make_scorer(s_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
-        elif scoring == "l_score":
-            scoring = make_scorer(l_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
-
-        if rand_search:
-            grid_search = RandomizedSearchCV(
-                estimator=self,
-                param_distributions=grid,
-                n_iter=n_iter_num,
-                cv=cv_num,
-                verbose=verbose,
-                random_state=42,
-                n_jobs=-1,
-                scoring=scoring,
-            )
-        else:
-            grid_search = GridSearchCV(
-                estimator=self,
-                param_grid=grid,
-                n_jobs=-1,
-                cv=cv_num,
-                verbose=verbose,
-                scoring=scoring,
-                error_score=0,
-            )
-        logger.debug(f"hyperparameter tuning {self.model_name} - started")
-        grid_result = grid_search.fit(x_train, y_train)
-        logger.debug(f"hyperparameter tuning {self.model_name} - finished")
-
-        if console_out:
-            means = grid_result.cv_results_["mean_test_score"]
-            stds = grid_result.cv_results_["std_test_score"]
-            params = grid_result.cv_results_["params"]
-            print()
-            for mean, stdev, param in zip(means, stds, params):
-                print("mean: %f (stdev: %f) with: %r" % (mean, stdev, param))
-            print()
+        results = []
+        configs = self._grid.sample_configuration(n_trails)
+        # remove duplicates
+        configs = list(dict.fromkeys(configs))
+
+        for config in tqdm(configs, desc="randomCVsearch"):
+            model = copy(self)
+            model.set_params(**config)
+            score = model.cross_validation(x_train, y_train, cv_num=cv_num, console_out=False, avg=avg, pos_label=pos_label, secondary_scoring=secondary_scoring, strength=strength)
+            config_dict = dict(config)
+            config_dict[scoring] = score[scoring]
+            results.append(config_dict)
+
+        self.rCVsearch_results = pd.DataFrame(results).sort_values(by=scoring, ascending=False)
+        best_hyperparameters = dict(self.rCVsearch_results.iloc[0])
+        best_score = best_hyperparameters[scoring]
+        best_hyperparameters.pop(scoring)
+        
+        return best_hyperparameters, best_score
 
-        self.model = grid_result.best_estimator_.model
-        if self.is_pipeline:
-            self.vectorizer = grid_result.best_estimator_.vectorizer
-            self.scaler = grid_result.best_estimator_.scaler
-            self.selector = grid_result.best_estimator_.selector
-            self.sampler = grid_result.best_estimator_.sampler
-            self._classifier = (self.model, self.model_type, self._grid)
-
-        print()
-        print("Best: %f using %s" % (grid_result.best_score_, grid_result.best_params_))
-        print()
-
-        if train_afterwards:
-            logger.debug(f"best model training {self.model_name} - started")
-            self.train(x_train, y_train, console_out=False)
-            logger.debug(f"best model training {self.model_name} - finished")
+    # def gridsearch(
+    #     self,
+    #     x_train: pd.DataFrame,
+    #     y_train: pd.Series,
+    #     grid: dict = None,
+    #     scoring: str = "accuracy",
+    #     avg: str = "macro",
+    #     pos_label: Union[int, str] = -1,
+    #     cv_num: int = 10,
+    #     verbose: int = 0,
+    #     rand_search: bool = True,
+    #     n_iter_num: int = 75,
+    #     console_out: bool = True,
+    #     train_afterwards: bool = True,
+    #     secondary_scoring: str = None,
+    #     strength: int = 3,
+    # ):
+    #     """
+    #     @param:
+    #         x_train: DataFrame with train features
+    #         y_train: Series with labels
+
+    #         grid: dictonary of parameters to tune (default: default parameter dictionary self.grid)
+
+    #         scoring: metrics to evaluate the models
+    #         avg: average to use for precision and recall score (e.g. "micro", "weighted", "binary")
+    #         pos_label: if avg="binary", pos_label says which class to score. Else pos_label is ignored (except scoring='s_score'/'l_score')
+
+    #         rand_search: True: RandomizedSearchCV, False: GridSearchCV
+    #         n_iter_num: Combinations to try out if rand_search=True
+
+    #         cv_num: number of different splits
+
+    #         verbose: log level (higher number --> more logs)
+    #         console_out: output the the results of the different iterations
+    #         train_afterwards: train the best model after finding it
+
+    #         secondary_scoring: weights the scoring (only for scoring='s_score'/'l_score')
+    #         strength: higher strength means a higher weight for the prefered secondary_scoring/pos_label (only for scoring='s_score'/'l_score')
+
+    #     @return:
+    #         set self.model = best model from search
+    #     """
+    #     if grid is None:
+    #         grid = self.grid
+
+    #     if console_out:
+    #         print()
+    #         print("grid: ", grid)
+    #         print()
+
+    #     if scoring == "precision":
+    #         scoring = make_scorer(precision_score, average=avg, pos_label=pos_label)
+    #     elif scoring == "recall":
+    #         scoring = make_scorer(recall_score, average=avg, pos_label=pos_label)
+    #     elif scoring == "s_score":
+    #         scoring = make_scorer(s_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
+    #     elif scoring == "l_score":
+    #         scoring = make_scorer(l_scoring, strength=strength, scoring=secondary_scoring, pos_label=pos_label)
+
+    #     if rand_search:
+    #         grid_search = RandomizedSearchCV(
+    #             estimator=self,
+    #             param_distributions=grid,
+    #             n_iter=n_iter_num,
+    #             cv=cv_num,
+    #             verbose=verbose,
+    #             random_state=42,
+    #             n_jobs=-1,
+    #             scoring=scoring,
+    #         )
+    #     else:
+    #         grid_search = GridSearchCV(
+    #             estimator=self,
+    #             param_grid=grid,
+    #             n_jobs=-1,
+    #             cv=cv_num,
+    #             verbose=verbose,
+    #             scoring=scoring,
+    #             error_score=0,
+    #         )
+    #     logger.debug(f"hyperparameter tuning {self.model_name} - started")
+    #     grid_result = grid_search.fit(x_train, y_train)
+    #     logger.debug(f"hyperparameter tuning {self.model_name} - finished")
+
+    #     if console_out:
+    #         means = grid_result.cv_results_["mean_test_score"]
+    #         stds = grid_result.cv_results_["std_test_score"]
+    #         params = grid_result.cv_results_["params"]
+    #         print()
+    #         for mean, stdev, param in zip(means, stds, params):
+    #             print("mean: %f (stdev: %f) with: %r" % (mean, stdev, param))
+    #         print()
+
+    #     self.model = grid_result.best_estimator_.model
+    #     if self.is_pipeline:
+    #         self.vectorizer = grid_result.best_estimator_.vectorizer
+    #         self.scaler = grid_result.best_estimator_.scaler
+    #         self.selector = grid_result.best_estimator_.selector
+    #         self.sampler = grid_result.best_estimator_.sampler
+    #         self._classifier = (self.model, self.model_type, self._grid)
+
+    #     print()
+    #     print("Best: %f using %s" % (grid_result.best_score_, grid_result.best_params_))
+    #     print()
+
+    #     if train_afterwards:
+    #         logger.debug(f"best model training {self.model_name} - started")
+    #         self.train(x_train, y_train, console_out=False)
+    #         logger.debug(f"best model training {self.model_name} - finished")
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/main_model.py` & `sam_ml-py-0.5.0/sam_ml/models/main_model.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml/models/main_pipeline.py` & `sam_ml-py-0.5.0/sam_ml/models/main_pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -89,48 +89,48 @@
 
         return f"Pipeline({params})"
 
     @property
     def steps(self) -> list[tuple[str, any]]:
         return [("vectorizer", self.vectorizer), ("scaler", self.scaler), ("selector", self.selector), ("sampler", self.sampler), ("model", self._classifier)]
 
-    @property
-    def grid(self) -> dict[str, list]:
-        pre_grid = {}
-        if self.vectorizer is not None:
-            vectorizer_grid = {f"vectorizer__{k}": v for k, v in self.vectorizer._grid.items()}
-            pre_grid.update(vectorizer_grid)
-        if self.scaler is not None:
-            scaler_grid = {f"scaler__{k}": v for k, v in self.scaler._grid.items()}
-            pre_grid.update(scaler_grid)
-        if self.selector is not None:
-            selector_grid = {f"selector__{k}": v for k, v in self.selector._grid.items()}
-            pre_grid.update(selector_grid)
-        if self.sampler is not None:
-            sampler_grid = {f"sampler__{k}": v for k, v in self.sampler._grid.items()}
-            pre_grid.update(sampler_grid)
-        model_grid = {f"model__{k}": v for k, v in self._grid.items()}
-        pre_grid.update(model_grid)
-        return pre_grid
-
-    def update_grid(self, **kwargs) -> None:
-        if self.vectorizer is not None:
-            vectorizer_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "vectorizer"])
-            self.vectorizer._grid.update(vectorizer_params)
-        if self.scaler is not None:
-            scaler_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "scaler"])
-            self.scaler._grid.update(scaler_params)
-        if self.selector is not None:
-            selector_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "selector"])
-            self.selector._grid.update(selector_params)
-        if self.sampler is not None:
-            sampler_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "sampler"])
-            self.sampler._grid.update(sampler_params)
-        model_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "model"])
-        super().update_grid(**model_params)
+    # @property
+    # def grid(self) -> dict[str, list]:
+    #     pre_grid = {}
+    #     if self.vectorizer is not None:
+    #         vectorizer_grid = {f"vectorizer__{k}": v for k, v in self.vectorizer._grid.items()}
+    #         pre_grid.update(vectorizer_grid)
+    #     if self.scaler is not None:
+    #         scaler_grid = {f"scaler__{k}": v for k, v in self.scaler._grid.items()}
+    #         pre_grid.update(scaler_grid)
+    #     if self.selector is not None:
+    #         selector_grid = {f"selector__{k}": v for k, v in self.selector._grid.items()}
+    #         pre_grid.update(selector_grid)
+    #     if self.sampler is not None:
+    #         sampler_grid = {f"sampler__{k}": v for k, v in self.sampler._grid.items()}
+    #         pre_grid.update(sampler_grid)
+    #     model_grid = {f"model__{k}": v for k, v in self._grid.items()}
+    #     pre_grid.update(model_grid)
+    #     return pre_grid
+
+    # def update_grid(self, **kwargs) -> None:
+    #     if self.vectorizer is not None:
+    #         vectorizer_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "vectorizer"])
+    #         self.vectorizer._grid.update(vectorizer_params)
+    #     if self.scaler is not None:
+    #         scaler_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "scaler"])
+    #         self.scaler._grid.update(scaler_params)
+    #     if self.selector is not None:
+    #         selector_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "selector"])
+    #         self.selector._grid.update(selector_params)
+    #     if self.sampler is not None:
+    #         sampler_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "sampler"])
+    #         self.sampler._grid.update(sampler_params)
+    #     model_params = dict([[i.split("__")[1], kwargs[i]] for i in list(kwargs.keys()) if i.split("__")[0] == "model"])
+    #     super().update_grid(**model_params)
     
     def __auto_vectorizing(self, X: pd.DataFrame, train_on: bool = True) -> pd.DataFrame:
         """ detects string columns, creates a vectorizer for each, and vectorizes them """
         if train_on:
             X = X.convert_dtypes()
             string_columns = list(X.select_dtypes(include="string").columns)
             self._string_columns = string_columns
@@ -165,23 +165,23 @@
     def predict(self, x_test: pd.DataFrame) -> list:
         x_test_pre, _ = self.__data_prepare(x_test, None, train_on=False)
         return super().predict(x_test_pre)
 
     def get_params(self, deep: bool = True) -> dict[str, any]:
         return dict(self.steps)
 
-    def set_params(self, **params):
-        if self.vectorizer is not None:
-            vec_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "vectorizer"])
-            self.vectorizer.set_params(**vec_params)
-        if self.scaler is not None:
-            scaler_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "scaler"])
-            self.scaler.set_params(**scaler_params)
-        if self.selector is not None:
-            selector_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "selector"])
-            self.selector.set_params(**selector_params)
-        if self.sampler is not None:
-            sampler_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "sampler"])
-            self.sampler.set_params(**sampler_params)
-        model_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "model"])
-        super().set_params(**model_params)
-        return self
+    # def set_params(self, **params):
+    #     if self.vectorizer is not None:
+    #         vec_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "vectorizer"])
+    #         self.vectorizer.set_params(**vec_params)
+    #     if self.scaler is not None:
+    #         scaler_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "scaler"])
+    #         self.scaler.set_params(**scaler_params)
+    #     if self.selector is not None:
+    #         selector_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "selector"])
+    #         self.selector.set_params(**selector_params)
+    #     if self.sampler is not None:
+    #         sampler_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "sampler"])
+    #         self.sampler.set_params(**sampler_params)
+    #     model_params = dict([[i.split("__")[1], params[i]] for i in list(params.keys()) if i.split("__")[0] == "model"])
+    #     super().set_params(**model_params)
+    #     return self
```

### Comparing `sam_ml-py-0.4.2/sam_ml/models/scorer.py` & `sam_ml-py-0.5.0/sam_ml/models/scorer.py`

 * *Files identical despite different names*

### Comparing `sam_ml-py-0.4.2/sam_ml_py.egg-info/PKG-INFO` & `sam_ml-py-0.5.0/sam_ml_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sam-ml-py
-Version: 0.4.2
+Version: 0.5.0
 Summary: a library for ML programing created by Samuel Brinkmann
 Author: Samuel Brinkmann
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `sam_ml-py-0.4.2/sam_ml_py.egg-info/SOURCES.txt` & `sam_ml-py-0.5.0/sam_ml_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 sam_ml/models/LinearDiscriminantAnalysis.py
 sam_ml/models/LinearSupportVectorClassifier.py
 sam_ml/models/LogisticRegression.py
 sam_ml/models/MLPClassifier.py
 sam_ml/models/QuadraticDiscriminantAnalysis.py
 sam_ml/models/RandomForestClassifier.py
 sam_ml/models/SupportVectorClassifier.py
+sam_ml/models/XGBoostClassifier.py
 sam_ml/models/__init__.py
 sam_ml/models/main_classifier.py
 sam_ml/models/main_model.py
 sam_ml/models/main_pipeline.py
 sam_ml/models/scorer.py
 sam_ml_py.egg-info/PKG-INFO
 sam_ml_py.egg-info/SOURCES.txt
```

