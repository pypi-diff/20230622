# Comparing `tmp/s11-classifier-3.4.1.tar.gz` & `tmp/s11-classifier-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/s11-classifier-3.4.1.tar", last modified: Fri Feb 24 15:54:14 2023, max compression
+gzip compressed data, was "s11-classifier-3.5.2.tar", last modified: Thu Jun 22 16:08:18 2023, max compression
```

## Comparing `s11-classifier-3.4.1.tar` & `s11-classifier-3.5.2.tar`

### file list

```diff
@@ -1,43 +1,41 @@
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1537 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/setup.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/s11_classifier.egg-info/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)       17 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/s11_classifier.egg-info/top_level.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      986 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/s11_classifier.egg-info/SOURCES.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/s11_classifier.egg-info/dependency_links.txt
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1627 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/s11_classifier.egg-info/PKG-INFO
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)        1 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/s11_classifier.egg-info/not-zip-safe
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      478 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/s11_classifier.egg-info/requires.txt
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/tests/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      780 2022-04-13 07:52:28.000000 s11-classifier-3.4.1/tests/samples_test.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2019-11-26 08:27:00.000000 s11-classifier-3.4.1/tests/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8087 2022-05-13 07:58:28.000000 s11-classifier-3.4.1/tests/conftest.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/tests/integration/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2022-02-15 12:45:18.000000 s11-classifier-3.4.1/tests/integration/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3413 2022-05-23 09:04:20.000000 s11-classifier-3.4.1/tests/integration/integration_supervised_singleraster_test.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2595 2022-04-28 13:05:14.000000 s11-classifier-3.4.1/tests/integration/integration_different_configs_test.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1423 2022-05-12 20:14:51.000000 s11-classifier-3.4.1/tests/integration/integration_unsupervised_test.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     2662 2022-05-23 09:04:20.000000 s11-classifier-3.4.1/tests/integration/integration_supervised_timeseries_test.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     5906 2023-02-24 10:35:47.000000 s11-classifier-3.4.1/tests/config_test.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1627 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/PKG-INFO
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/classifier/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10974 2023-02-24 10:35:47.000000 s11-classifier-3.4.1/classifier/timeseries.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     8400 2022-05-18 09:42:23.000000 s11-classifier-3.4.1/classifier/classify.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      224 2022-02-15 12:45:18.000000 s11-classifier-3.4.1/classifier/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1711 2022-04-13 07:43:29.000000 s11-classifier-3.4.1/classifier/dataprep.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    29389 2022-05-13 13:27:03.000000 s11-classifier-3.4.1/classifier/samples.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     4062 2022-11-29 08:40:18.000000 s11-classifier-3.4.1/classifier/cli.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    10177 2023-02-24 10:35:47.000000 s11-classifier-3.4.1/classifier/train.py
-drwxr-xr-x   0 gitlab-runner   (999) gitlab-runner   (998)        0 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/classifier/utils/
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)        0 2019-11-26 08:27:00.000000 s11-classifier-3.4.1/classifier/utils/__init__.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    15556 2022-11-29 08:40:18.000000 s11-classifier-3.4.1/classifier/utils/general.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     7459 2022-05-23 14:33:22.000000 s11-classifier-3.4.1/classifier/utils/raster.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    20326 2023-02-24 10:35:47.000000 s11-classifier-3.4.1/classifier/utils/config.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     3254 2022-04-06 13:03:40.000000 s11-classifier-3.4.1/classifier/utils/vector.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     9434 2022-05-13 09:27:55.000000 s11-classifier-3.4.1/classifier/accuracy.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    14400 2023-02-24 10:35:47.000000 s11-classifier-3.4.1/classifier/models.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      624 2022-05-24 08:31:19.000000 s11-classifier-3.4.1/classifier/settings.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)    11365 2022-05-12 20:14:51.000000 s11-classifier-3.4.1/classifier/predict.py
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     1035 2019-11-26 08:27:00.000000 s11-classifier-3.4.1/README.md
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)       38 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/setup.cfg
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)      104 2019-11-26 08:27:00.000000 s11-classifier-3.4.1/MANIFEST.in
--rw-r--r--   0 gitlab-runner   (999) gitlab-runner   (998)     6068 2023-02-24 15:54:14.000000 s11-classifier-3.4.1/CHANGES.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:08:18.708968 s11-classifier-3.5.2/
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-06-22 16:08:18.708968 s11-classifier-3.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:08:18.704968 s11-classifier-3.5.2/classifier/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9434 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/accuracy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8400 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/classify.py
+-rw-rw-rw-   0 root         (0) root         (0)     4062 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     1711 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/dataprep.py
+-rw-rw-rw-   0 root         (0) root         (0)    14400 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/models.py
+-rw-rw-rw-   0 root         (0) root         (0)    11365 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/predict.py
+-rw-rw-rw-   0 root         (0) root         (0)    29529 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/samples.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    10967 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)    10405 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:08:18.705968 s11-classifier-3.5.2/classifier/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20302 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/utils/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15595 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/utils/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     7459 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/utils/raster.py
+-rw-rw-rw-   0 root         (0) root         (0)     3254 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/classifier/utils/vector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:08:18.706968 s11-classifier-3.5.2/s11_classifier.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1309 2023-06-22 16:08:18.000000 s11-classifier-3.5.2/s11_classifier.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      963 2023-06-22 16:08:18.000000 s11-classifier-3.5.2/s11_classifier.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:08:18.000000 s11-classifier-3.5.2/s11_classifier.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 16:00:01.000000 s11-classifier-3.5.2/s11_classifier.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      478 2023-06-22 16:08:18.000000 s11-classifier-3.5.2/s11_classifier.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-22 16:08:18.000000 s11-classifier-3.5.2/s11_classifier.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 16:08:18.708968 s11-classifier-3.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1537 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:08:18.707968 s11-classifier-3.5.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5898 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/config_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     8087 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 16:08:18.708968 s11-classifier-3.5.2/tests/integration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2595 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/integration/integration_different_configs_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3413 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/integration/integration_supervised_singleraster_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2663 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/integration/integration_supervised_timeseries_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/integration/integration_unsupervised_test.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-22 15:58:15.000000 s11-classifier-3.5.2/tests/samples_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `s11-classifier-3.4.1/setup.py` & `s11-classifier-3.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 # (c) Satelligence, see LICENSE.
 # pylint: skip-file
 from setuptools import setup
 import setuptools
 
-version = '3.4.1'
+version = '3.5.2'
 
 long_description = open('README.md').read()
 
 test_requirements = [
     'pytest'
 ]
```

### Comparing `s11-classifier-3.4.1/s11_classifier.egg-info/SOURCES.txt` & `s11-classifier-3.5.2/s11_classifier.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-CHANGES.md
-MANIFEST.in
 README.md
 setup.py
 classifier/__init__.py
 classifier/accuracy.py
 classifier/classify.py
 classifier/cli.py
 classifier/dataprep.py
```

### Comparing `s11-classifier-3.4.1/s11_classifier.egg-info/PKG-INFO` & `s11-classifier-3.5.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: s11-classifier
-Version: 3.4.1
+Version: 3.5.2
 Summary: Classifier
 Home-page: https://gitlab.com/satelligence/classifier
 Author: Satelligence
 Author-email: team@satelligence.com
 License: Apache-2.0
-Description: # Classifier
-        
-        A scalable land cover classification tool for humans
-        
-        Go to [the documentation](https://satelligence.gitlab.io/classifier) for more
-         info on how to install and run Classifier!
-        
-        ## Note on performance
-        
-        For now, the multithreading of XGboost is not properly implemented. If you have
-        a lot of input files the XGBoost method is MUCH slower than e.g. scikit-learn's
-        random forest. With single input files (so not a lot of IO operations), the
-        difference in performance is small.
-        
-        ## issues and bugs
-        
-        Issues are tracked on the [issue list of this
-        repo](https://gitlab.com/satelligence/classifier/issues).
-        
-        ## Development
-        
-        Please follow the [Satelligence development guidelines](https://gitlab.com/satelligence/workflow/blob/master/dev_workflow.md)
-        when adding features or fixing bugs.
-        
-        (Fork) Clone this repo:
-        
-        ```sh
-        git clone git@gitlab.com:satelligence/classifier.git
-        ```
-        
-        Make sure you are running the latest docker image.
-        
-        Run docker with a binding to the source files:
-        
-        ```sh
-        docker run  -v $(pwd):/app -t -i classifier
-        ```
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# Classifier
+
+A scalable land cover classification tool for humans
+
+Go to [the documentation](https://satelligence.gitlab.io/classifier) for more
+ info on how to install and run Classifier!
+
+## Note on performance
+
+For now, the multithreading of XGboost is not properly implemented. If you have
+a lot of input files the XGBoost method is MUCH slower than e.g. scikit-learn's
+random forest. With single input files (so not a lot of IO operations), the
+difference in performance is small.
+
+## issues and bugs
+
+Issues are tracked on the [issue list of this
+repo](https://gitlab.com/satelligence/classifier/issues).
+
+## Development
+
+Please follow the [Satelligence development guidelines](https://gitlab.com/satelligence/workflow/blob/master/dev_workflow.md)
+when adding features or fixing bugs.
+
+(Fork) Clone this repo:
+
+```sh
+git clone git@gitlab.com:satelligence/classifier.git
+```
+
+Make sure you are running the latest docker image.
+
+Run docker with a binding to the source files:
+
+```sh
+docker run  -v $(pwd):/app -t -i classifier
+```
```

### Comparing `s11-classifier-3.4.1/tests/samples_test.py` & `s11-classifier-3.5.2/tests/samples_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/tests/conftest.py` & `s11-classifier-3.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/tests/integration/integration_supervised_singleraster_test.py` & `s11-classifier-3.5.2/tests/integration/integration_supervised_singleraster_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/tests/integration/integration_different_configs_test.py` & `s11-classifier-3.5.2/tests/integration/integration_different_configs_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/tests/integration/integration_unsupervised_test.py` & `s11-classifier-3.5.2/tests/integration/integration_unsupervised_test.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/tests/integration/integration_supervised_timeseries_test.py` & `s11-classifier-3.5.2/tests/integration/integration_supervised_timeseries_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     Test for running a supervised knn classification
     on a timeseries
     """
     save_config_as_json(threads=1, algorithm="knn_dtw",
                         remove_outliers=False, rasters_are_timeseries=True)
 
     rois_path = WORKSPACE / 'integration_test_rois.gpkg'
+
     runner.invoke(classification, [
         "--name", 'test_result', '--overwrite', True,
         '--rois', rois_path, "integration_test_rasters"])
     directory = WORKSPACE / 'test_result' / 'classification.tif'
     with rasterio.open(directory, 'r') as dst:
         result = dst.read(1)
         assert np.all(result[:, 0:4] == 0)
```

### Comparing `s11-classifier-3.4.1/tests/config_test.py` & `s11-classifier-3.5.2/tests/config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,26 +81,26 @@
             RandomForestConfiguration(
                 n_estimators=100,
                 criterion="gini",
                 max_depth=None,
                 min_samples_split=2,
                 min_samples_leaf=1,
                 min_weight_fraction_leaf=0.0,
-                max_features="auto",
+                max_features="sqrt",
                 max_leaf_nodes=None,
                 min_impurity_decrease=0.0,
                 bootstrap=True,
                 oob_score=False,
                 random_state=None,
                 verbose=0,
                 class_weight=None,
                 ccp_alpha=0.0,
                 max_samples=None,
                 optimization_parameters={
-                    "max_features": ['auto', 'sqrt', 'log2'],
+                    "max_features": ['sqrt', 'log2'],
                     "max_leaf_nodes": [3, 5, 7],
                     "max_depth": [None, 1, 3, 10, 20000],
                     "n_estimators": [10, 50, 100],
                     "min_samples_split": [2],
                     "min_samples_leaf": [1],
                     "min_weight_fraction_leaf": [0.0],
                     "min_impurity_decrease": [0.0],
```

### Comparing `s11-classifier-3.4.1/PKG-INFO` & `s11-classifier-3.5.2/s11_classifier.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 Metadata-Version: 2.1
 Name: s11-classifier
-Version: 3.4.1
+Version: 3.5.2
 Summary: Classifier
 Home-page: https://gitlab.com/satelligence/classifier
 Author: Satelligence
 Author-email: team@satelligence.com
 License: Apache-2.0
-Description: # Classifier
-        
-        A scalable land cover classification tool for humans
-        
-        Go to [the documentation](https://satelligence.gitlab.io/classifier) for more
-         info on how to install and run Classifier!
-        
-        ## Note on performance
-        
-        For now, the multithreading of XGboost is not properly implemented. If you have
-        a lot of input files the XGBoost method is MUCH slower than e.g. scikit-learn's
-        random forest. With single input files (so not a lot of IO operations), the
-        difference in performance is small.
-        
-        ## issues and bugs
-        
-        Issues are tracked on the [issue list of this
-        repo](https://gitlab.com/satelligence/classifier/issues).
-        
-        ## Development
-        
-        Please follow the [Satelligence development guidelines](https://gitlab.com/satelligence/workflow/blob/master/dev_workflow.md)
-        when adding features or fixing bugs.
-        
-        (Fork) Clone this repo:
-        
-        ```sh
-        git clone git@gitlab.com:satelligence/classifier.git
-        ```
-        
-        Make sure you are running the latest docker image.
-        
-        Run docker with a binding to the source files:
-        
-        ```sh
-        docker run  -v $(pwd):/app -t -i classifier
-        ```
-Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+
+# Classifier
+
+A scalable land cover classification tool for humans
+
+Go to [the documentation](https://satelligence.gitlab.io/classifier) for more
+ info on how to install and run Classifier!
+
+## Note on performance
+
+For now, the multithreading of XGboost is not properly implemented. If you have
+a lot of input files the XGBoost method is MUCH slower than e.g. scikit-learn's
+random forest. With single input files (so not a lot of IO operations), the
+difference in performance is small.
+
+## issues and bugs
+
+Issues are tracked on the [issue list of this
+repo](https://gitlab.com/satelligence/classifier/issues).
+
+## Development
+
+Please follow the [Satelligence development guidelines](https://gitlab.com/satelligence/workflow/blob/master/dev_workflow.md)
+when adding features or fixing bugs.
+
+(Fork) Clone this repo:
+
+```sh
+git clone git@gitlab.com:satelligence/classifier.git
+```
+
+Make sure you are running the latest docker image.
+
+Run docker with a binding to the source files:
+
+```sh
+docker run  -v $(pwd):/app -t -i classifier
+```
```

### Comparing `s11-classifier-3.4.1/classifier/timeseries.py` & `s11-classifier-3.5.2/classifier/timeseries.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,15 +213,15 @@
             all_patterns_per_class_per_band = []
 
             # Index for plot
             i = (subset_pattern_id*len(class_ids))+int(class_id_i)
 
             for j, band_name in enumerate(band_names):
                 # Extract values for given class and band
-                y_values = subset_pattern_df[band_name][class_id].values
+                y_values = subset_pattern_df[band_name][class_id]
 
                 axes[i, j].plot(x_days, y_values, 'r')
                 axes[i, j].set_title(
                     f"Class id: {class_id}, Band name: {band_name}")
                 axes[i, j].scatter(x_days, y_values,
                                    facecolor='gray', edgecolors='none')
```

### Comparing `s11-classifier-3.4.1/classifier/classify.py` & `s11-classifier-3.5.2/classifier/classify.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/classifier/dataprep.py` & `s11-classifier-3.5.2/classifier/dataprep.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/classifier/samples.py` & `s11-classifier-3.5.2/classifier/samples.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,19 +328,26 @@
                     'warp_dst': warp_dst,
                     'dates': dates,
                     'bands': bands,
                     'for_prediction': for_prediction
                 }
                 for roi in rois
             ]
-        gathered_samples_list = parallel_function(
-            self._gather_samples_per_roi,
-            kwargs,
-            ncpus=config.app.threads
-        )
+        if for_prediction:
+            gathered_samples_list = []
+            for roi in kwargs:
+                gathered_samples_list.append(
+                    self._gather_samples_per_roi(**roi)  # type: ignore
+                )
+        else:
+            gathered_samples_list = parallel_function(
+                self._gather_samples_per_roi,
+                kwargs,
+                ncpus=config.app.threads
+            )
         if gathered_samples_list:
             # Concat results from all the rois
             samples_df = pd.concat(gathered_samples_list, axis=0)
         else:
             SAMPLES_LOGGER.error(
                 "Couldn't collect any samples from any roi."
                 "Check your rois or rasters."
@@ -512,20 +519,17 @@
             dataset (pd.DataFrame): DataFrame containing Nans
             config (Configuration): Parameters to use for imputation
 
         Returns:
             dataset (np.ndarray): DataFrame with Nans imputed
         """
 
-        verbosity_level = 0 if config.app.log_level == 'INFO' else 2
-
         # sklearn Imputer
         imputer = SimpleImputer(strategy=config.app.imputation_strategy,
-                                fill_value=config.app.imputation_constant,
-                                verbose=verbosity_level)
+                                fill_value=config.app.imputation_constant)
         # imputer expects ndarray
         return imputer.fit_transform(dataset.values)
 
     @staticmethod
     def outlier_removal(samples: pd.DataFrame) -> pd.DataFrame:
         """Outlier removal from samples using Isolation Forest
```

### Comparing `s11-classifier-3.4.1/classifier/cli.py` & `s11-classifier-3.5.2/classifier/cli.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/classifier/train.py` & `s11-classifier-3.5.2/classifier/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,10 +275,15 @@
     # Optimize model
     if optimize:
         model = optimize_model(
             model, x_train, y_train, out_dir, config)
 
     # y_train_encoded = sample_labels_encoder.transform(y_train)
     TRAIN_LOGGER.info("Train model ...")
+    # Use array repr (x_train.values) to make sure feature names are not used.
+    # Except when we use KNN DTW, because that needs the band names.
+    if not config.app.algorithm == 'knn_dtw':
+        x_train = x_train.values
+
     model.fit(x_train, y_train)
     TRAIN_LOGGER.info("Model trained.")
     return model, xcols, test
```

### Comparing `s11-classifier-3.4.1/classifier/utils/general.py` & `s11-classifier-3.5.2/classifier/utils/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -421,15 +421,17 @@
         iterable (list): List of kwargs for the function
         ncpus (int): number of cpus to use
 
     Returns:
         list of results
     """
     with tqdm_joblib(tqdm(total=len(iterable))) as _:
-        result = Parallel(n_jobs=ncpus)(delayed(func)(**x) for x in iterable)
+        result = Parallel(
+            n_jobs=ncpus, max_nbytes=None
+        )(delayed(func)(**x) for x in iterable)
 
     return result
 
 
 @ contextlib.contextmanager
 def tqdm_joblib(tqdm_object: tqdm) -> None:
     """Patch joblib to report a tqdm progress bar for many thread jobs
```

### Comparing `s11-classifier-3.4.1/classifier/utils/raster.py` & `s11-classifier-3.5.2/classifier/utils/raster.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/classifier/utils/config.py` & `s11-classifier-3.5.2/classifier/utils/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from marshmallow import Schema, ValidationError, fields, validate
 
 UTILS_CONFIG_LOGGER = logging.getLogger(__name__)
 
 LOG_LEVELS = ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
 IMPUTATION_STRATEGIES = ["mean", "median",
                          "most_frequent", "constant", "interpolate"]
-OPTIMIZE_RANDOMFOREST_MAX_FEATURES = ["auto", "sqrt", "log2"]
+OPTIMIZE_RANDOMFOREST_MAX_FEATURES = ["sqrt", "log2"]
 ALGORITHMS = [
     "randomforest", "xgboost", "singleclass", "us_kmeans",
     "us_kmeans_minibatch", "knn_dtw"
 ]
 
 PARAMETERS = {
     "app": {
@@ -70,26 +70,26 @@
     "randomforest": {
         "n_estimators": 100,
         "criterion": "gini",
         "max_depth": None,
         "min_samples_split": 2,
         "min_samples_leaf": 1,
         "min_weight_fraction_leaf": 0.,
-        "max_features": "auto",
+        "max_features": "sqrt",
         "max_leaf_nodes": None,
         "min_impurity_decrease": 0.,
         "bootstrap": True,
         "oob_score": False,
         "random_state": None,
         "verbose": 0,
         "class_weight": None,
         "ccp_alpha": 0.,
         "max_samples": None,
         "optimization_parameters": {
-            "max_features": ['auto', 'sqrt', 'log2'],
+            "max_features": ['sqrt', 'log2'],
             "max_leaf_nodes": [3, 5, 7],
             "max_depth": [None, 1, 3, 10, 20000],
             "n_estimators": [10, 50, 100],
             "min_samples_split": [2],
             "min_samples_leaf": [1],
             "min_weight_fraction_leaf": [0.0],
             "min_impurity_decrease": [0.0],
@@ -373,15 +373,15 @@
                 validate=validate.Range(
                     min=0.01, max=1))
          }
     )
     min_weight_fraction_leaf = fields.Float(validate=validate.Range(
         min=0, error="Value must be >= 0")
     )
-    max_features = fields.Str(validate=validate.OneOf(["auto", "sqrt", "log2"]))
+    max_features = fields.Str(validate=validate.OneOf(["sqrt", "log2"]))
     max_leaf_nodes = fields.Int(validate=validate.Range(
         min=1, error="Value must be >= 1 or NONE."), allow_none=True
     )
     min_impurity_decrease = fields.Float(validate=validate.Range(
         min=0, error="Value must be >=0")
     )
     bootstrap = fields.Bool()
```

### Comparing `s11-classifier-3.4.1/classifier/utils/vector.py` & `s11-classifier-3.5.2/classifier/utils/vector.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/classifier/accuracy.py` & `s11-classifier-3.5.2/classifier/accuracy.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/classifier/models.py` & `s11-classifier-3.5.2/classifier/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
     def __init__(self,
                  n_estimators=100,
                  criterion="gini",
                  max_depth=None,
                  min_samples_split=2,
                  min_samples_leaf=1,
                  min_weight_fraction_leaf=0.,
-                 max_features="auto",
+                 max_features="sqrt",
                  max_leaf_nodes=None,
                  min_impurity_decrease=0.,
                  bootstrap=True,
                  oob_score=False,
                  n_jobs=1,
                  random_state=None,
                  verbose=0,
```

### Comparing `s11-classifier-3.4.1/classifier/settings.py` & `s11-classifier-3.5.2/classifier/settings.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/classifier/predict.py` & `s11-classifier-3.5.2/classifier/predict.py`

 * *Files identical despite different names*

### Comparing `s11-classifier-3.4.1/README.md` & `s11-classifier-3.5.2/README.md`

 * *Files identical despite different names*

