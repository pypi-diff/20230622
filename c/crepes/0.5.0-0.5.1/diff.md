# Comparing `tmp/crepes-0.5.0.tar.gz` & `tmp/crepes-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crepes-0.5.0.tar", last modified: Fri Jun  2 13:02:32 2023, max compression
+gzip compressed data, was "crepes-0.5.1.tar", last modified: Thu Jun 22 14:58:36 2023, max compression
```

## Comparing `crepes-0.5.0.tar` & `crepes-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-02 13:02:32.505391 crepes-0.5.0/
--rw-rw-r--   0 henke     (1000) henke     (1000)     1462 2023-05-17 13:34:56.000000 crepes-0.5.0/LICENSE
--rw-rw-r--   0 henke     (1000) henke     (1000)    15151 2023-06-02 13:02:32.505391 crepes-0.5.0/PKG-INFO
--rw-rw-r--   0 henke     (1000) henke     (1000)    14628 2023-05-17 13:34:56.000000 crepes-0.5.0/README.md
--rw-rw-r--   0 henke     (1000) henke     (1000)      108 2023-05-17 13:34:56.000000 crepes-0.5.0/pyproject.toml
--rw-rw-r--   0 henke     (1000) henke     (1000)       38 2023-06-02 13:02:32.505391 crepes-0.5.0/setup.cfg
--rw-rw-r--   0 henke     (1000) henke     (1000)      865 2023-06-02 13:01:47.000000 crepes-0.5.0/setup.py
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-02 13:02:32.505391 crepes-0.5.0/src/
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-02 13:02:32.505391 crepes-0.5.0/src/crepes/
--rw-rw-r--   0 henke     (1000) henke     (1000)      110 2023-05-17 13:34:56.000000 crepes-0.5.0/src/crepes/__init__.py
--rw-rw-r--   0 henke     (1000) henke     (1000)    68243 2023-06-02 12:58:21.000000 crepes-0.5.0/src/crepes/base.py
--rw-rw-r--   0 henke     (1000) henke     (1000)    17388 2023-06-02 12:10:16.000000 crepes-0.5.0/src/crepes/extras.py
-drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-02 13:02:32.505391 crepes-0.5.0/src/crepes.egg-info/
--rw-rw-r--   0 henke     (1000) henke     (1000)    15151 2023-06-02 13:02:32.000000 crepes-0.5.0/src/crepes.egg-info/PKG-INFO
--rw-rw-r--   0 henke     (1000) henke     (1000)      273 2023-06-02 13:02:32.000000 crepes-0.5.0/src/crepes.egg-info/SOURCES.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)        1 2023-06-02 13:02:32.000000 crepes-0.5.0/src/crepes.egg-info/dependency_links.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)       13 2023-06-02 13:02:32.000000 crepes-0.5.0/src/crepes.egg-info/requires.txt
--rw-rw-r--   0 henke     (1000) henke     (1000)        7 2023-06-02 13:02:32.000000 crepes-0.5.0/src/crepes.egg-info/top_level.txt
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-22 14:58:36.942776 crepes-0.5.1/
+-rw-rw-r--   0 henke     (1000) henke     (1000)     1462 2023-06-16 12:19:07.000000 crepes-0.5.1/LICENSE
+-rw-rw-r--   0 henke     (1000) henke     (1000)    15153 2023-06-22 14:58:36.942776 crepes-0.5.1/PKG-INFO
+-rw-rw-r--   0 henke     (1000) henke     (1000)    14630 2023-06-16 12:19:07.000000 crepes-0.5.1/README.md
+-rw-rw-r--   0 henke     (1000) henke     (1000)      108 2023-06-16 12:19:07.000000 crepes-0.5.1/pyproject.toml
+-rw-rw-r--   0 henke     (1000) henke     (1000)       38 2023-06-22 14:58:36.942776 crepes-0.5.1/setup.cfg
+-rw-rw-r--   0 henke     (1000) henke     (1000)      865 2023-06-22 14:56:57.000000 crepes-0.5.1/setup.py
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-22 14:58:36.942776 crepes-0.5.1/src/
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-22 14:58:36.942776 crepes-0.5.1/src/crepes/
+-rw-rw-r--   0 henke     (1000) henke     (1000)      110 2023-06-16 12:19:07.000000 crepes-0.5.1/src/crepes/__init__.py
+-rw-rw-r--   0 henke     (1000) henke     (1000)    68231 2023-06-22 14:42:20.000000 crepes-0.5.1/src/crepes/base.py
+-rw-rw-r--   0 henke     (1000) henke     (1000)    17391 2023-06-16 12:19:07.000000 crepes-0.5.1/src/crepes/extras.py
+drwxrwxr-x   0 henke     (1000) henke     (1000)        0 2023-06-22 14:58:36.942776 crepes-0.5.1/src/crepes.egg-info/
+-rw-rw-r--   0 henke     (1000) henke     (1000)    15153 2023-06-22 14:58:36.000000 crepes-0.5.1/src/crepes.egg-info/PKG-INFO
+-rw-rw-r--   0 henke     (1000) henke     (1000)      273 2023-06-22 14:58:36.000000 crepes-0.5.1/src/crepes.egg-info/SOURCES.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)        1 2023-06-22 14:58:36.000000 crepes-0.5.1/src/crepes.egg-info/dependency_links.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)       13 2023-06-22 14:58:36.000000 crepes-0.5.1/src/crepes.egg-info/requires.txt
+-rw-rw-r--   0 henke     (1000) henke     (1000)        7 2023-06-22 14:58:36.000000 crepes-0.5.1/src/crepes.egg-info/top_level.txt
```

### Comparing `crepes-0.5.0/LICENSE` & `crepes-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crepes-0.5.0/PKG-INFO` & `crepes-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepes
-Version: 0.5.0
+Version: 0.5.1
 Summary: Conformal regressors and predictive systems (crepes)
 Home-page: https://github.com/henrikbostrom/crepes
 Author: Henrik Boström
 Author-email: bostromh@kth.se
 Project-URL: Bug Tracker, https://github.com//henrikbostrom/crepes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -13,26 +13,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center"><a href="https://crepes.readthedocs.io"><img alt="crepes" src="https://github-production-user-asset-6210df.s3.amazonaws.com/7838741/237950772-1d4487b1-7f43-4ce0-9db0-032baeddbece.png"></a></p>
 
 <p align="center">
 <a href="https://pypi.org/project/crepes/"><img src="https://badge.fury.io/py/crepes.svg?dummy=unused" alt="PyPI version" height=20 align="center"></a>
-<a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/version.svg?dummy=unused" alt="Anaconda version" height=20 align="center"></a>
+<a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/version.svg" alt="Anaconda version" height=20 align="center"></a>
 <a href="https://crepes.readthedocs.io/en/latest"><img src="https://readthedocs.org/projects/crepes/badge/?version=latest" alt="docs status" height=20 align="center"></a> 
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/platforms.svg?dummy=unused" alt="Platforms" height=20 align="center"></a>
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/license.svg?dummy=unused" alt="License" height=20 align="center"></a>
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/latest_release_date.svg?dummy=unused" alt="Release date" height=20 align="center"></a>
 </p>
 
 <br>
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
-The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
+The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.extras`, which provides some standard options for these.
 
 ## Installation
 
 From [PyPI](https://pypi.org/project/crepes/)
 
 ```bash
 pip install crepes
@@ -42,15 +42,15 @@
 
 ```bash
 conda install -c conda-forge crepes
 ```
 
 ## Documentation
 
-For the complete documentation, see [here](https://crepes.readthedocs.io/en/latest/).
+For the complete documentation, see [crepes.readthedocs.io](https://crepes.readthedocs.io/en/latest/).
 
 ## Quickstart
 
 Let us illustrate the use of `crepes` by importing a dataset from [www.openml.org](https://www.openml.org),
 which we split into a training and a test set using `train_test_split` from [sklearn](https://scikit-learn.org),
 and then further split the training set into a proper training set and a calibration set:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crepes Version: 0.5.0 Summary: Conformal regressors
+Metadata-Version: 2.1 Name: crepes Version: 0.5.1 Summary: Conformal regressors
 and predictive systems (crepes) Home-page: https://github.com/henrikbostrom/
 crepes Author: Henrik BostrÃ¶m Author-email: bostromh@kth.se Project-URL: Bug
 Tracker, https://github.com//henrikbostrom/crepes/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                                    [crepes]
@@ -12,119 +12,120 @@
 `crepes` is a Python package for generating *conformal regressors*, which
 transform point predictions of any underlying regression model into prediction
 intervals for specified levels of confidence. The package also implements
 *conformal predictive systems*, which transform the point predictions into
 cumulative distribution functions. The `crepes` package implements standard,
 normalized and Mondrian conformal regressors and predictive systems. While the
 package allows you to use your own difficulty estimates and Mondrian
-categories, there is also a separate module, called `crepes.fillings`, which
+categories, there is also a separate module, called `crepes.extras`, which
 provides some standard options for these. ## Installation From [PyPI](https://
 pypi.org/project/crepes/) ```bash pip install crepes ``` From [conda-forge]
 (https://anaconda.org/conda-forge/crepes) ```bash conda install -c conda-forge
-crepes ``` ## Documentation For the complete documentation, see [here](https://
-crepes.readthedocs.io/en/latest/). ## Quickstart Let us illustrate the use of
-`crepes` by importing a dataset from [www.openml.org](https://www.openml.org),
-which we split into a training and a test set using `train_test_split` from
-[sklearn](https://scikit-learn.org), and then further split the training set
-into a proper training set and a calibration set: ```python from
-sklearn.datasets import fetch_openml from sklearn.model_selection import
-train_test_split dataset = fetch_openml(name="house_sales", version=3) X =
-dataset.data.values.astype(float) y = dataset.target.values.astype(float)
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.5)
-X_prop_train, X_cal, y_prop_train, y_cal = train_test_split(X_train, y_train,
-test_size=0.25) ``` Let us now "wrap" a `RandomForestRegressor` from [sklearn]
-(https://scikit-learn.org) using the class `Wrap` from `crepes` and fit it (in
-the usual way) to the proper training set: ```python from sklearn.ensemble
-import RandomForestRegressor from crepes import Wrap rf = Wrap
-(RandomForestRegressor()) rf.fit(X_prop_train, y_prop_train) ``` We can use the
-fitted model to obtain point predictions (again, in the usual way) for the
-calibration objects, from which we can calculate the residuals. These residuals
-are exactly what we need to "calibrate" the learner: ```python residuals =
-y_cal - rf.predict(X_cal) rf.calibrate(residuals) ``` A (standard) conformal
-regressor was formed (under the hood). We may now use it for obtaining
-prediction intervals for the test set, here using a confidence level of 99%:
-```python rf.predict_int(X_test, confidence=0.99) ``` ```numpy array([[-
-171902.2 , 953866.2 ], [-276818.01, 848950.39], [ 22679.37, 1148447.77], ...,
-[ 242954.02, 1368722.42], [-308093.73, 817674.67], [-227057.4 , 898711. ]]) ```
-The output is a [NumPy](https://numpy.org) array with a row for each test
-instance, and where the two columns specify the lower and upper bound of each
-prediction interval. We may request that the intervals are cut to exclude
-impossible values, in this case below 0, and if we also rely on the default
-confidence level (0.95), the output intervals will be a bit tighter: ```python
-rf.predict_int(X_test, y_min=0) ``` ```numpy array([[ 152258.55, 629705.45],
-[ 47342.74, 524789.64], [ 346840.12, 824287.02], ..., [ 567114.77, 1044561.67],
-[ 16067.02, 493513.92], [ 97103.35, 574550.25]]) ``` The above intervals are
-not normalized, i.e., they are all of the same size (at least before they are
-cut). We could make them more informative through normalization using
-difficulty estimates; objects considered more difficult will be assigned wider
-intervals. We will use a `DifficultyEstimator` from the `crepes.extras` module
-for this purpose. Here we estimate the difficulty by the standard deviation of
-the target of the k (default `k=25`) nearest neighbors in the proper training
-set to each object in the calibration set. A small value (beta) is added to the
-estimates, which may be given through an argument to the function; below we
-just use the default, i.e., `beta=0.01`. We first obtain the difficulty
-estimates for the calibration set: ```python from crepes.extras import
-DifficultyEstimator de = DifficultyEstimator() de.fit(X_prop_train,
-y=y_prop_train) sigmas_cal = de.apply(X_cal) ``` These can now be used for the
-calibration, which (under the hood) will produce a normalized conformal
-regressor: ```python rf.calibrate(residuals, sigmas=sigmas_cal) ``` We need
-difficulty estimates for the test set too, which we provide as input to
-`predict_int`: ```python sigmas_test = de.apply(X_test) rf.predict_int(X_test,
-sigmas=sigmas_test, y_min=0) ``` ```numpy array([[ 226719.06607977,
-555244.93392023], [ 173767.90753715, 398364.47246285], [ 124690.70166966,
-1046436.43833034], ..., [ 607949.71540572, 1003726.72459428], [ 188671.3752278
-, 320909.5647722 ], [ 145340.39076824, 526313.20923176]]) ``` Depending on the
-employed difficulty estimator, the normalized intervals may sometimes be
-unreasonably large, in the sense that they may be several times larger than any
-previously observed error. Moreover, if the difficulty estimator is
-uninformative, e.g., completely random, the varying interval sizes may give a
-false impression of that we can expect lower prediction errors for instances
-with tighter intervals. Ideally, a difficulty estimator providing little or no
-information on the expected error should instead lead to more uniformly
-distributed interval sizes. A Mondrian conformal regressor can be used to
-address these problems, by dividing the object space into non-overlapping so-
-called Mondrian categories, and forming a (standard) conformal regressor for
-each category. The category membership of the objects can be provided as an
-additional argument, named `bins`, for the `fit` method. Here we use the helper
-function `binning` from `crepes.extras` to form Mondrian categories by equal-
-sized binning of the difficulty estimates; the function returns labels for the
-calibration objects the we provide as input to the calibration, and we also get
-thresholds for the bins, which can use later when binning the test objects:
-```python from crepes.extras import binning bins_cal, bin_thresholds = binning
-(sigmas_cal, bins=20) rf.calibrate(residuals, bins=bins_cal) ``` Let us now get
-the labels of the Mondrian categories for the test objects and use them when
-predicting intervals: ```python bins_test = binning(sigmas_test,
-bins=bin_thresholds) rf.predict_int(X_test, bins=bins_test, y_min=0) ```
-```numpy array([[ 206379.7 , 575584.3 ], [ 144014.65, 428117.73], [ 17965.57,
-1153161.57], ..., [ 653865.22, 957811.22], [ 174264.87, 335316.07],
-[ 140587.46, 531066.14]]) ``` We could very easily switch from conformal
-regressors to conformal predictive systems. The latter produce cumulative
-distribution functions (conformal predictive distributions). From these we can
-generate prediction intervals, but we can also obtain percentiles, calibrated
-point predictions, as well as p-values for given target values. Let us see how
-we can go ahead to do that. Well, there is only one thing above that changes:
-just provide `cps=True` to the `calibrate` method. We can, for example, form
-normalized Mondrian conformal predictive systems, by providing both `bins` and
-`sigmas` to the `calibrate` method. Here we will consider Mondrian categories
-formed from binning the point predictions: ```python bins_cal, bin_thresholds =
-binning(rf.predict(X_cal), bins=5) rf.calibrate(residuals, sigmas=sigmas_cal,
-bins=bins_cal, cps=True) ``` By providing the bins (and sigmas) for the test
-objects, we can now make predictions with the conformal predictive system,
-through the method `predict_cps`. The output of this method can be controlled
-quite flexibly; here we request prediction intervals with 95% confidence to be
-output: ```python bins_test = binning(rf.predict(X_test), bins=bin_thresholds)
-rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test,
-lower_percentiles=2.5, higher_percentiles=97.5, y_min=0) ``` ```numpy array([
-[ 245826.3422693 , 517315.83618985], [ 145348.03415848, 392968.15587997],
-[ 148774.65461212, 1034300.84195976], ..., [ 589200.5725957 ,
-1057013.89102007], [ 171938.29382952, 317732.31611141], [ 167498.01540504,
-482328.98552632]]) ``` If we would like to take a look at the p-values for the
-true targets (these should be uniformly distributed), we can do the following:
-```python rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test, y=y_test)
-``` ```numpy array([0.98603614, 0.87178256, 0.44201984, ..., 0.05688804,
+crepes ``` ## Documentation For the complete documentation, see
+[crepes.readthedocs.io](https://crepes.readthedocs.io/en/latest/). ##
+Quickstart Let us illustrate the use of `crepes` by importing a dataset from
+[www.openml.org](https://www.openml.org), which we split into a training and a
+test set using `train_test_split` from [sklearn](https://scikit-learn.org), and
+then further split the training set into a proper training set and a
+calibration set: ```python from sklearn.datasets import fetch_openml from
+sklearn.model_selection import train_test_split dataset = fetch_openml
+(name="house_sales", version=3) X = dataset.data.values.astype(float) y =
+dataset.target.values.astype(float) X_train, X_test, y_train, y_test =
+train_test_split(X, y, test_size=0.5) X_prop_train, X_cal, y_prop_train, y_cal
+= train_test_split(X_train, y_train, test_size=0.25) ``` Let us now "wrap" a
+`RandomForestRegressor` from [sklearn](https://scikit-learn.org) using the
+class `Wrap` from `crepes` and fit it (in the usual way) to the proper training
+set: ```python from sklearn.ensemble import RandomForestRegressor from crepes
+import Wrap rf = Wrap(RandomForestRegressor()) rf.fit(X_prop_train,
+y_prop_train) ``` We can use the fitted model to obtain point predictions
+(again, in the usual way) for the calibration objects, from which we can
+calculate the residuals. These residuals are exactly what we need to
+"calibrate" the learner: ```python residuals = y_cal - rf.predict(X_cal)
+rf.calibrate(residuals) ``` A (standard) conformal regressor was formed (under
+the hood). We may now use it for obtaining prediction intervals for the test
+set, here using a confidence level of 99%: ```python rf.predict_int(X_test,
+confidence=0.99) ``` ```numpy array([[-171902.2 , 953866.2 ], [-276818.01,
+848950.39], [ 22679.37, 1148447.77], ..., [ 242954.02, 1368722.42], [-
+308093.73, 817674.67], [-227057.4 , 898711. ]]) ``` The output is a [NumPy]
+(https://numpy.org) array with a row for each test instance, and where the two
+columns specify the lower and upper bound of each prediction interval. We may
+request that the intervals are cut to exclude impossible values, in this case
+below 0, and if we also rely on the default confidence level (0.95), the output
+intervals will be a bit tighter: ```python rf.predict_int(X_test, y_min=0) ```
+```numpy array([[ 152258.55, 629705.45], [ 47342.74, 524789.64], [ 346840.12,
+824287.02], ..., [ 567114.77, 1044561.67], [ 16067.02, 493513.92], [ 97103.35,
+574550.25]]) ``` The above intervals are not normalized, i.e., they are all of
+the same size (at least before they are cut). We could make them more
+informative through normalization using difficulty estimates; objects
+considered more difficult will be assigned wider intervals. We will use a
+`DifficultyEstimator` from the `crepes.extras` module for this purpose. Here we
+estimate the difficulty by the standard deviation of the target of the k
+(default `k=25`) nearest neighbors in the proper training set to each object in
+the calibration set. A small value (beta) is added to the estimates, which may
+be given through an argument to the function; below we just use the default,
+i.e., `beta=0.01`. We first obtain the difficulty estimates for the calibration
+set: ```python from crepes.extras import DifficultyEstimator de =
+DifficultyEstimator() de.fit(X_prop_train, y=y_prop_train) sigmas_cal =
+de.apply(X_cal) ``` These can now be used for the calibration, which (under the
+hood) will produce a normalized conformal regressor: ```python rf.calibrate
+(residuals, sigmas=sigmas_cal) ``` We need difficulty estimates for the test
+set too, which we provide as input to `predict_int`: ```python sigmas_test =
+de.apply(X_test) rf.predict_int(X_test, sigmas=sigmas_test, y_min=0) ```
+```numpy array([[ 226719.06607977, 555244.93392023], [ 173767.90753715,
+398364.47246285], [ 124690.70166966, 1046436.43833034], ..., [ 607949.71540572,
+1003726.72459428], [ 188671.3752278 , 320909.5647722 ], [ 145340.39076824,
+526313.20923176]]) ``` Depending on the employed difficulty estimator, the
+normalized intervals may sometimes be unreasonably large, in the sense that
+they may be several times larger than any previously observed error. Moreover,
+if the difficulty estimator is uninformative, e.g., completely random, the
+varying interval sizes may give a false impression of that we can expect lower
+prediction errors for instances with tighter intervals. Ideally, a difficulty
+estimator providing little or no information on the expected error should
+instead lead to more uniformly distributed interval sizes. A Mondrian conformal
+regressor can be used to address these problems, by dividing the object space
+into non-overlapping so-called Mondrian categories, and forming a (standard)
+conformal regressor for each category. The category membership of the objects
+can be provided as an additional argument, named `bins`, for the `fit` method.
+Here we use the helper function `binning` from `crepes.extras` to form Mondrian
+categories by equal-sized binning of the difficulty estimates; the function
+returns labels for the calibration objects the we provide as input to the
+calibration, and we also get thresholds for the bins, which can use later when
+binning the test objects: ```python from crepes.extras import binning bins_cal,
+bin_thresholds = binning(sigmas_cal, bins=20) rf.calibrate(residuals,
+bins=bins_cal) ``` Let us now get the labels of the Mondrian categories for the
+test objects and use them when predicting intervals: ```python bins_test =
+binning(sigmas_test, bins=bin_thresholds) rf.predict_int(X_test,
+bins=bins_test, y_min=0) ``` ```numpy array([[ 206379.7 , 575584.3 ],
+[ 144014.65, 428117.73], [ 17965.57, 1153161.57], ..., [ 653865.22, 957811.22],
+[ 174264.87, 335316.07], [ 140587.46, 531066.14]]) ``` We could very easily
+switch from conformal regressors to conformal predictive systems. The latter
+produce cumulative distribution functions (conformal predictive distributions).
+From these we can generate prediction intervals, but we can also obtain
+percentiles, calibrated point predictions, as well as p-values for given target
+values. Let us see how we can go ahead to do that. Well, there is only one
+thing above that changes: just provide `cps=True` to the `calibrate` method. We
+can, for example, form normalized Mondrian conformal predictive systems, by
+providing both `bins` and `sigmas` to the `calibrate` method. Here we will
+consider Mondrian categories formed from binning the point predictions:
+```python bins_cal, bin_thresholds = binning(rf.predict(X_cal), bins=5)
+rf.calibrate(residuals, sigmas=sigmas_cal, bins=bins_cal, cps=True) ``` By
+providing the bins (and sigmas) for the test objects, we can now make
+predictions with the conformal predictive system, through the method
+`predict_cps`. The output of this method can be controlled quite flexibly; here
+we request prediction intervals with 95% confidence to be output: ```python
+bins_test = binning(rf.predict(X_test), bins=bin_thresholds) rf.predict_cps
+(X_test, sigmas=sigmas_test, bins=bins_test, lower_percentiles=2.5,
+higher_percentiles=97.5, y_min=0) ``` ```numpy array([[ 245826.3422693 ,
+517315.83618985], [ 145348.03415848, 392968.15587997], [ 148774.65461212,
+1034300.84195976], ..., [ 589200.5725957 , 1057013.89102007],
+[ 171938.29382952, 317732.31611141], [ 167498.01540504, 482328.98552632]]) ```
+If we would like to take a look at the p-values for the true targets (these
+should be uniformly distributed), we can do the following: ```python
+rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test, y=y_test) ```
+```numpy array([0.98603614, 0.87178256, 0.44201984, ..., 0.05688804,
 0.09473604, 0.31069913]) ``` We may request that the `predict_cps` method
 returns the full conformal predictive distribution (CPD) for each test
 instance, as defined by the threshold values, by setting `return_cpds=True`.
 The format of the distributions vary with the type of conformal predictive
 system; for a standard and normalized CPS, the output is an array with a row
 for each test instance and a column for each calibration instance (residual),
 while for a Mondrian CPS, the default output is a vector containing one CPD per
```

### Comparing `crepes-0.5.0/README.md` & `crepes-0.5.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 <p align="center"><a href="https://crepes.readthedocs.io"><img alt="crepes" src="https://github-production-user-asset-6210df.s3.amazonaws.com/7838741/237950772-1d4487b1-7f43-4ce0-9db0-032baeddbece.png"></a></p>
 
 <p align="center">
 <a href="https://pypi.org/project/crepes/"><img src="https://badge.fury.io/py/crepes.svg?dummy=unused" alt="PyPI version" height=20 align="center"></a>
-<a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/version.svg?dummy=unused" alt="Anaconda version" height=20 align="center"></a>
+<a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/version.svg" alt="Anaconda version" height=20 align="center"></a>
 <a href="https://crepes.readthedocs.io/en/latest"><img src="https://readthedocs.org/projects/crepes/badge/?version=latest" alt="docs status" height=20 align="center"></a> 
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/platforms.svg?dummy=unused" alt="Platforms" height=20 align="center"></a>
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/license.svg?dummy=unused" alt="License" height=20 align="center"></a>
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/latest_release_date.svg?dummy=unused" alt="Release date" height=20 align="center"></a>
 </p>
 
 <br>
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
-The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
+The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.extras`, which provides some standard options for these.
 
 ## Installation
 
 From [PyPI](https://pypi.org/project/crepes/)
 
 ```bash
 pip install crepes
@@ -27,15 +27,15 @@
 
 ```bash
 conda install -c conda-forge crepes
 ```
 
 ## Documentation
 
-For the complete documentation, see [here](https://crepes.readthedocs.io/en/latest/).
+For the complete documentation, see [crepes.readthedocs.io](https://crepes.readthedocs.io/en/latest/).
 
 ## Quickstart
 
 Let us illustrate the use of `crepes` by importing a dataset from [www.openml.org](https://www.openml.org),
 which we split into a training and a test set using `train_test_split` from [sklearn](https://scikit-learn.org),
 and then further split the training set into a proper training set and a calibration set:
```

#### html2text {}

```diff
@@ -5,119 +5,120 @@
 `crepes` is a Python package for generating *conformal regressors*, which
 transform point predictions of any underlying regression model into prediction
 intervals for specified levels of confidence. The package also implements
 *conformal predictive systems*, which transform the point predictions into
 cumulative distribution functions. The `crepes` package implements standard,
 normalized and Mondrian conformal regressors and predictive systems. While the
 package allows you to use your own difficulty estimates and Mondrian
-categories, there is also a separate module, called `crepes.fillings`, which
+categories, there is also a separate module, called `crepes.extras`, which
 provides some standard options for these. ## Installation From [PyPI](https://
 pypi.org/project/crepes/) ```bash pip install crepes ``` From [conda-forge]
 (https://anaconda.org/conda-forge/crepes) ```bash conda install -c conda-forge
-crepes ``` ## Documentation For the complete documentation, see [here](https://
-crepes.readthedocs.io/en/latest/). ## Quickstart Let us illustrate the use of
-`crepes` by importing a dataset from [www.openml.org](https://www.openml.org),
-which we split into a training and a test set using `train_test_split` from
-[sklearn](https://scikit-learn.org), and then further split the training set
-into a proper training set and a calibration set: ```python from
-sklearn.datasets import fetch_openml from sklearn.model_selection import
-train_test_split dataset = fetch_openml(name="house_sales", version=3) X =
-dataset.data.values.astype(float) y = dataset.target.values.astype(float)
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.5)
-X_prop_train, X_cal, y_prop_train, y_cal = train_test_split(X_train, y_train,
-test_size=0.25) ``` Let us now "wrap" a `RandomForestRegressor` from [sklearn]
-(https://scikit-learn.org) using the class `Wrap` from `crepes` and fit it (in
-the usual way) to the proper training set: ```python from sklearn.ensemble
-import RandomForestRegressor from crepes import Wrap rf = Wrap
-(RandomForestRegressor()) rf.fit(X_prop_train, y_prop_train) ``` We can use the
-fitted model to obtain point predictions (again, in the usual way) for the
-calibration objects, from which we can calculate the residuals. These residuals
-are exactly what we need to "calibrate" the learner: ```python residuals =
-y_cal - rf.predict(X_cal) rf.calibrate(residuals) ``` A (standard) conformal
-regressor was formed (under the hood). We may now use it for obtaining
-prediction intervals for the test set, here using a confidence level of 99%:
-```python rf.predict_int(X_test, confidence=0.99) ``` ```numpy array([[-
-171902.2 , 953866.2 ], [-276818.01, 848950.39], [ 22679.37, 1148447.77], ...,
-[ 242954.02, 1368722.42], [-308093.73, 817674.67], [-227057.4 , 898711. ]]) ```
-The output is a [NumPy](https://numpy.org) array with a row for each test
-instance, and where the two columns specify the lower and upper bound of each
-prediction interval. We may request that the intervals are cut to exclude
-impossible values, in this case below 0, and if we also rely on the default
-confidence level (0.95), the output intervals will be a bit tighter: ```python
-rf.predict_int(X_test, y_min=0) ``` ```numpy array([[ 152258.55, 629705.45],
-[ 47342.74, 524789.64], [ 346840.12, 824287.02], ..., [ 567114.77, 1044561.67],
-[ 16067.02, 493513.92], [ 97103.35, 574550.25]]) ``` The above intervals are
-not normalized, i.e., they are all of the same size (at least before they are
-cut). We could make them more informative through normalization using
-difficulty estimates; objects considered more difficult will be assigned wider
-intervals. We will use a `DifficultyEstimator` from the `crepes.extras` module
-for this purpose. Here we estimate the difficulty by the standard deviation of
-the target of the k (default `k=25`) nearest neighbors in the proper training
-set to each object in the calibration set. A small value (beta) is added to the
-estimates, which may be given through an argument to the function; below we
-just use the default, i.e., `beta=0.01`. We first obtain the difficulty
-estimates for the calibration set: ```python from crepes.extras import
-DifficultyEstimator de = DifficultyEstimator() de.fit(X_prop_train,
-y=y_prop_train) sigmas_cal = de.apply(X_cal) ``` These can now be used for the
-calibration, which (under the hood) will produce a normalized conformal
-regressor: ```python rf.calibrate(residuals, sigmas=sigmas_cal) ``` We need
-difficulty estimates for the test set too, which we provide as input to
-`predict_int`: ```python sigmas_test = de.apply(X_test) rf.predict_int(X_test,
-sigmas=sigmas_test, y_min=0) ``` ```numpy array([[ 226719.06607977,
-555244.93392023], [ 173767.90753715, 398364.47246285], [ 124690.70166966,
-1046436.43833034], ..., [ 607949.71540572, 1003726.72459428], [ 188671.3752278
-, 320909.5647722 ], [ 145340.39076824, 526313.20923176]]) ``` Depending on the
-employed difficulty estimator, the normalized intervals may sometimes be
-unreasonably large, in the sense that they may be several times larger than any
-previously observed error. Moreover, if the difficulty estimator is
-uninformative, e.g., completely random, the varying interval sizes may give a
-false impression of that we can expect lower prediction errors for instances
-with tighter intervals. Ideally, a difficulty estimator providing little or no
-information on the expected error should instead lead to more uniformly
-distributed interval sizes. A Mondrian conformal regressor can be used to
-address these problems, by dividing the object space into non-overlapping so-
-called Mondrian categories, and forming a (standard) conformal regressor for
-each category. The category membership of the objects can be provided as an
-additional argument, named `bins`, for the `fit` method. Here we use the helper
-function `binning` from `crepes.extras` to form Mondrian categories by equal-
-sized binning of the difficulty estimates; the function returns labels for the
-calibration objects the we provide as input to the calibration, and we also get
-thresholds for the bins, which can use later when binning the test objects:
-```python from crepes.extras import binning bins_cal, bin_thresholds = binning
-(sigmas_cal, bins=20) rf.calibrate(residuals, bins=bins_cal) ``` Let us now get
-the labels of the Mondrian categories for the test objects and use them when
-predicting intervals: ```python bins_test = binning(sigmas_test,
-bins=bin_thresholds) rf.predict_int(X_test, bins=bins_test, y_min=0) ```
-```numpy array([[ 206379.7 , 575584.3 ], [ 144014.65, 428117.73], [ 17965.57,
-1153161.57], ..., [ 653865.22, 957811.22], [ 174264.87, 335316.07],
-[ 140587.46, 531066.14]]) ``` We could very easily switch from conformal
-regressors to conformal predictive systems. The latter produce cumulative
-distribution functions (conformal predictive distributions). From these we can
-generate prediction intervals, but we can also obtain percentiles, calibrated
-point predictions, as well as p-values for given target values. Let us see how
-we can go ahead to do that. Well, there is only one thing above that changes:
-just provide `cps=True` to the `calibrate` method. We can, for example, form
-normalized Mondrian conformal predictive systems, by providing both `bins` and
-`sigmas` to the `calibrate` method. Here we will consider Mondrian categories
-formed from binning the point predictions: ```python bins_cal, bin_thresholds =
-binning(rf.predict(X_cal), bins=5) rf.calibrate(residuals, sigmas=sigmas_cal,
-bins=bins_cal, cps=True) ``` By providing the bins (and sigmas) for the test
-objects, we can now make predictions with the conformal predictive system,
-through the method `predict_cps`. The output of this method can be controlled
-quite flexibly; here we request prediction intervals with 95% confidence to be
-output: ```python bins_test = binning(rf.predict(X_test), bins=bin_thresholds)
-rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test,
-lower_percentiles=2.5, higher_percentiles=97.5, y_min=0) ``` ```numpy array([
-[ 245826.3422693 , 517315.83618985], [ 145348.03415848, 392968.15587997],
-[ 148774.65461212, 1034300.84195976], ..., [ 589200.5725957 ,
-1057013.89102007], [ 171938.29382952, 317732.31611141], [ 167498.01540504,
-482328.98552632]]) ``` If we would like to take a look at the p-values for the
-true targets (these should be uniformly distributed), we can do the following:
-```python rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test, y=y_test)
-``` ```numpy array([0.98603614, 0.87178256, 0.44201984, ..., 0.05688804,
+crepes ``` ## Documentation For the complete documentation, see
+[crepes.readthedocs.io](https://crepes.readthedocs.io/en/latest/). ##
+Quickstart Let us illustrate the use of `crepes` by importing a dataset from
+[www.openml.org](https://www.openml.org), which we split into a training and a
+test set using `train_test_split` from [sklearn](https://scikit-learn.org), and
+then further split the training set into a proper training set and a
+calibration set: ```python from sklearn.datasets import fetch_openml from
+sklearn.model_selection import train_test_split dataset = fetch_openml
+(name="house_sales", version=3) X = dataset.data.values.astype(float) y =
+dataset.target.values.astype(float) X_train, X_test, y_train, y_test =
+train_test_split(X, y, test_size=0.5) X_prop_train, X_cal, y_prop_train, y_cal
+= train_test_split(X_train, y_train, test_size=0.25) ``` Let us now "wrap" a
+`RandomForestRegressor` from [sklearn](https://scikit-learn.org) using the
+class `Wrap` from `crepes` and fit it (in the usual way) to the proper training
+set: ```python from sklearn.ensemble import RandomForestRegressor from crepes
+import Wrap rf = Wrap(RandomForestRegressor()) rf.fit(X_prop_train,
+y_prop_train) ``` We can use the fitted model to obtain point predictions
+(again, in the usual way) for the calibration objects, from which we can
+calculate the residuals. These residuals are exactly what we need to
+"calibrate" the learner: ```python residuals = y_cal - rf.predict(X_cal)
+rf.calibrate(residuals) ``` A (standard) conformal regressor was formed (under
+the hood). We may now use it for obtaining prediction intervals for the test
+set, here using a confidence level of 99%: ```python rf.predict_int(X_test,
+confidence=0.99) ``` ```numpy array([[-171902.2 , 953866.2 ], [-276818.01,
+848950.39], [ 22679.37, 1148447.77], ..., [ 242954.02, 1368722.42], [-
+308093.73, 817674.67], [-227057.4 , 898711. ]]) ``` The output is a [NumPy]
+(https://numpy.org) array with a row for each test instance, and where the two
+columns specify the lower and upper bound of each prediction interval. We may
+request that the intervals are cut to exclude impossible values, in this case
+below 0, and if we also rely on the default confidence level (0.95), the output
+intervals will be a bit tighter: ```python rf.predict_int(X_test, y_min=0) ```
+```numpy array([[ 152258.55, 629705.45], [ 47342.74, 524789.64], [ 346840.12,
+824287.02], ..., [ 567114.77, 1044561.67], [ 16067.02, 493513.92], [ 97103.35,
+574550.25]]) ``` The above intervals are not normalized, i.e., they are all of
+the same size (at least before they are cut). We could make them more
+informative through normalization using difficulty estimates; objects
+considered more difficult will be assigned wider intervals. We will use a
+`DifficultyEstimator` from the `crepes.extras` module for this purpose. Here we
+estimate the difficulty by the standard deviation of the target of the k
+(default `k=25`) nearest neighbors in the proper training set to each object in
+the calibration set. A small value (beta) is added to the estimates, which may
+be given through an argument to the function; below we just use the default,
+i.e., `beta=0.01`. We first obtain the difficulty estimates for the calibration
+set: ```python from crepes.extras import DifficultyEstimator de =
+DifficultyEstimator() de.fit(X_prop_train, y=y_prop_train) sigmas_cal =
+de.apply(X_cal) ``` These can now be used for the calibration, which (under the
+hood) will produce a normalized conformal regressor: ```python rf.calibrate
+(residuals, sigmas=sigmas_cal) ``` We need difficulty estimates for the test
+set too, which we provide as input to `predict_int`: ```python sigmas_test =
+de.apply(X_test) rf.predict_int(X_test, sigmas=sigmas_test, y_min=0) ```
+```numpy array([[ 226719.06607977, 555244.93392023], [ 173767.90753715,
+398364.47246285], [ 124690.70166966, 1046436.43833034], ..., [ 607949.71540572,
+1003726.72459428], [ 188671.3752278 , 320909.5647722 ], [ 145340.39076824,
+526313.20923176]]) ``` Depending on the employed difficulty estimator, the
+normalized intervals may sometimes be unreasonably large, in the sense that
+they may be several times larger than any previously observed error. Moreover,
+if the difficulty estimator is uninformative, e.g., completely random, the
+varying interval sizes may give a false impression of that we can expect lower
+prediction errors for instances with tighter intervals. Ideally, a difficulty
+estimator providing little or no information on the expected error should
+instead lead to more uniformly distributed interval sizes. A Mondrian conformal
+regressor can be used to address these problems, by dividing the object space
+into non-overlapping so-called Mondrian categories, and forming a (standard)
+conformal regressor for each category. The category membership of the objects
+can be provided as an additional argument, named `bins`, for the `fit` method.
+Here we use the helper function `binning` from `crepes.extras` to form Mondrian
+categories by equal-sized binning of the difficulty estimates; the function
+returns labels for the calibration objects the we provide as input to the
+calibration, and we also get thresholds for the bins, which can use later when
+binning the test objects: ```python from crepes.extras import binning bins_cal,
+bin_thresholds = binning(sigmas_cal, bins=20) rf.calibrate(residuals,
+bins=bins_cal) ``` Let us now get the labels of the Mondrian categories for the
+test objects and use them when predicting intervals: ```python bins_test =
+binning(sigmas_test, bins=bin_thresholds) rf.predict_int(X_test,
+bins=bins_test, y_min=0) ``` ```numpy array([[ 206379.7 , 575584.3 ],
+[ 144014.65, 428117.73], [ 17965.57, 1153161.57], ..., [ 653865.22, 957811.22],
+[ 174264.87, 335316.07], [ 140587.46, 531066.14]]) ``` We could very easily
+switch from conformal regressors to conformal predictive systems. The latter
+produce cumulative distribution functions (conformal predictive distributions).
+From these we can generate prediction intervals, but we can also obtain
+percentiles, calibrated point predictions, as well as p-values for given target
+values. Let us see how we can go ahead to do that. Well, there is only one
+thing above that changes: just provide `cps=True` to the `calibrate` method. We
+can, for example, form normalized Mondrian conformal predictive systems, by
+providing both `bins` and `sigmas` to the `calibrate` method. Here we will
+consider Mondrian categories formed from binning the point predictions:
+```python bins_cal, bin_thresholds = binning(rf.predict(X_cal), bins=5)
+rf.calibrate(residuals, sigmas=sigmas_cal, bins=bins_cal, cps=True) ``` By
+providing the bins (and sigmas) for the test objects, we can now make
+predictions with the conformal predictive system, through the method
+`predict_cps`. The output of this method can be controlled quite flexibly; here
+we request prediction intervals with 95% confidence to be output: ```python
+bins_test = binning(rf.predict(X_test), bins=bin_thresholds) rf.predict_cps
+(X_test, sigmas=sigmas_test, bins=bins_test, lower_percentiles=2.5,
+higher_percentiles=97.5, y_min=0) ``` ```numpy array([[ 245826.3422693 ,
+517315.83618985], [ 145348.03415848, 392968.15587997], [ 148774.65461212,
+1034300.84195976], ..., [ 589200.5725957 , 1057013.89102007],
+[ 171938.29382952, 317732.31611141], [ 167498.01540504, 482328.98552632]]) ```
+If we would like to take a look at the p-values for the true targets (these
+should be uniformly distributed), we can do the following: ```python
+rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test, y=y_test) ```
+```numpy array([0.98603614, 0.87178256, 0.44201984, ..., 0.05688804,
 0.09473604, 0.31069913]) ``` We may request that the `predict_cps` method
 returns the full conformal predictive distribution (CPD) for each test
 instance, as defined by the threshold values, by setting `return_cpds=True`.
 The format of the distributions vary with the type of conformal predictive
 system; for a standard and normalized CPS, the output is an array with a row
 for each test instance and a column for each calibration instance (residual),
 while for a Mondrian CPS, the default output is a vector containing one CPD per
```

### Comparing `crepes-0.5.0/setup.py` & `crepes-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crepes",
-    version="0.5.0",
+    version="0.5.1",
     author="Henrik Boström",
     author_email="bostromh@kth.se",
     description="Conformal regressors and predictive systems (crepes)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/henrikbostrom/crepes",
     project_urls={
```

### Comparing `crepes-0.5.0/src/crepes/base.py` & `crepes-0.5.1/src/crepes/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Author: Henrik Boström (bostromh@kth.se)
 
 Copyright 2023 Henrik Boström
 
 License: BSD 3 clause
 """
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 import numpy as np
 import pandas as pd
 import time
 import warnings
 
 warnings.simplefilter("always", UserWarning)
@@ -929,20 +929,20 @@
         is generated for which the number of elements is the product of the 
         number of calibration and test objects, unless a Mondrian approach is 
         employed; for the latter, this number is reduced by increasing the number 
         of bins.
         """
 
         tic = time.time()
+        test_results = {}
+        lower_percentile = (1-confidence)/2*100
+        higher_percentile = (confidence+(1-confidence)/2)*100
         if metrics is None:
             metrics = ["error","eff_mean","eff_med","CRPS","time_fit",
                        "time_evaluate"]
-            lower_percentile = (1-confidence)/2*100
-            higher_percentile = (confidence+(1-confidence)/2)*100
-            test_results = {}
         if "CRPS" in metrics:
             results, cpds = self.predict(y_hat, sigmas=sigmas, bins=bins, y=y,
                                          lower_percentiles=lower_percentile,
                                          higher_percentiles=higher_percentile,
                                          y_min=y_min, y_max=y_max,
                                          return_cpds=True, cpds_by_bins=True)
             intervals = results[:,[1,2]]
```

### Comparing `crepes-0.5.0/src/crepes/extras.py` & `crepes-0.5.1/src/crepes/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,15 @@
         beta is added after the normalization, which means that the range of
         scores after normalization will be [0+beta, 1+beta]. Below, we use 
         ``beta=0.001`` together with 10 neighbors (``k=10``):
 
         .. code-block:: python
         
            de_knn_mod = DifficultyEstimator() 
-           de_knn_dist.fit(X_prop_train, k=10, beta=0.001, scaler=True)
+           de_knn_mod.fit(X_prop_train, k=10, beta=0.001, scaler=True)
 
         Note
         ----
         The use of out-of-bag calibration, as enabled by ``oob=True``, 
         does not come with the theoretical validity guarantees of the regular
         (inductive) conformal regressors and predictive systems, due to that 
         calibration and test instances are not handled in exactly the same way.
@@ -280,15 +280,15 @@
         If ``de_oob`` is a :class:`.DifficultyEstimator` that has been fitted 
         with the option ``oob=True`` and a training set, then a call to 
         :meth:`.apply` without any objects will return the estimates for the 
         training set:
 
         .. code-block:: python
         
-           oob_difficulty_estimates = de.apply()
+           oob_difficulty_estimates = de_oob.apply()
 
         For a difficulty estimator employing any of the k-nearest neighbor 
         approaches, the above will return an estimate for the difficulty 
         of each object in the training set computed using a leave-one-out 
         procedure, while for the variance-based approach the out-of-bag 
         predictions will instead be used. 
         """
```

### Comparing `crepes-0.5.0/src/crepes.egg-info/PKG-INFO` & `crepes-0.5.1/src/crepes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crepes
-Version: 0.5.0
+Version: 0.5.1
 Summary: Conformal regressors and predictive systems (crepes)
 Home-page: https://github.com/henrikbostrom/crepes
 Author: Henrik Boström
 Author-email: bostromh@kth.se
 Project-URL: Bug Tracker, https://github.com//henrikbostrom/crepes/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -13,26 +13,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center"><a href="https://crepes.readthedocs.io"><img alt="crepes" src="https://github-production-user-asset-6210df.s3.amazonaws.com/7838741/237950772-1d4487b1-7f43-4ce0-9db0-032baeddbece.png"></a></p>
 
 <p align="center">
 <a href="https://pypi.org/project/crepes/"><img src="https://badge.fury.io/py/crepes.svg?dummy=unused" alt="PyPI version" height=20 align="center"></a>
-<a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/version.svg?dummy=unused" alt="Anaconda version" height=20 align="center"></a>
+<a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/version.svg" alt="Anaconda version" height=20 align="center"></a>
 <a href="https://crepes.readthedocs.io/en/latest"><img src="https://readthedocs.org/projects/crepes/badge/?version=latest" alt="docs status" height=20 align="center"></a> 
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/platforms.svg?dummy=unused" alt="Platforms" height=20 align="center"></a>
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/license.svg?dummy=unused" alt="License" height=20 align="center"></a>
 <a href="https://anaconda.org/conda-forge/crepes"><img src="https://anaconda.org/conda-forge/crepes/badges/latest_release_date.svg?dummy=unused" alt="Release date" height=20 align="center"></a>
 </p>
 
 <br>
 
 `crepes` is a Python package for generating *conformal regressors*, which transform point predictions of any underlying regression model into prediction intervals for specified levels of confidence. The package also implements *conformal predictive systems*, which transform the point predictions into cumulative distribution functions.
 
-The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.fillings`, which provides some standard options for these.
+The `crepes` package implements standard, normalized and Mondrian conformal regressors and predictive systems. While the package allows you to use your own difficulty estimates and Mondrian categories, there is also a separate module, called `crepes.extras`, which provides some standard options for these.
 
 ## Installation
 
 From [PyPI](https://pypi.org/project/crepes/)
 
 ```bash
 pip install crepes
@@ -42,15 +42,15 @@
 
 ```bash
 conda install -c conda-forge crepes
 ```
 
 ## Documentation
 
-For the complete documentation, see [here](https://crepes.readthedocs.io/en/latest/).
+For the complete documentation, see [crepes.readthedocs.io](https://crepes.readthedocs.io/en/latest/).
 
 ## Quickstart
 
 Let us illustrate the use of `crepes` by importing a dataset from [www.openml.org](https://www.openml.org),
 which we split into a training and a test set using `train_test_split` from [sklearn](https://scikit-learn.org),
 and then further split the training set into a proper training set and a calibration set:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crepes Version: 0.5.0 Summary: Conformal regressors
+Metadata-Version: 2.1 Name: crepes Version: 0.5.1 Summary: Conformal regressors
 and predictive systems (crepes) Home-page: https://github.com/henrikbostrom/
 crepes Author: Henrik BostrÃ¶m Author-email: bostromh@kth.se Project-URL: Bug
 Tracker, https://github.com//henrikbostrom/crepes/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                                    [crepes]
@@ -12,119 +12,120 @@
 `crepes` is a Python package for generating *conformal regressors*, which
 transform point predictions of any underlying regression model into prediction
 intervals for specified levels of confidence. The package also implements
 *conformal predictive systems*, which transform the point predictions into
 cumulative distribution functions. The `crepes` package implements standard,
 normalized and Mondrian conformal regressors and predictive systems. While the
 package allows you to use your own difficulty estimates and Mondrian
-categories, there is also a separate module, called `crepes.fillings`, which
+categories, there is also a separate module, called `crepes.extras`, which
 provides some standard options for these. ## Installation From [PyPI](https://
 pypi.org/project/crepes/) ```bash pip install crepes ``` From [conda-forge]
 (https://anaconda.org/conda-forge/crepes) ```bash conda install -c conda-forge
-crepes ``` ## Documentation For the complete documentation, see [here](https://
-crepes.readthedocs.io/en/latest/). ## Quickstart Let us illustrate the use of
-`crepes` by importing a dataset from [www.openml.org](https://www.openml.org),
-which we split into a training and a test set using `train_test_split` from
-[sklearn](https://scikit-learn.org), and then further split the training set
-into a proper training set and a calibration set: ```python from
-sklearn.datasets import fetch_openml from sklearn.model_selection import
-train_test_split dataset = fetch_openml(name="house_sales", version=3) X =
-dataset.data.values.astype(float) y = dataset.target.values.astype(float)
-X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.5)
-X_prop_train, X_cal, y_prop_train, y_cal = train_test_split(X_train, y_train,
-test_size=0.25) ``` Let us now "wrap" a `RandomForestRegressor` from [sklearn]
-(https://scikit-learn.org) using the class `Wrap` from `crepes` and fit it (in
-the usual way) to the proper training set: ```python from sklearn.ensemble
-import RandomForestRegressor from crepes import Wrap rf = Wrap
-(RandomForestRegressor()) rf.fit(X_prop_train, y_prop_train) ``` We can use the
-fitted model to obtain point predictions (again, in the usual way) for the
-calibration objects, from which we can calculate the residuals. These residuals
-are exactly what we need to "calibrate" the learner: ```python residuals =
-y_cal - rf.predict(X_cal) rf.calibrate(residuals) ``` A (standard) conformal
-regressor was formed (under the hood). We may now use it for obtaining
-prediction intervals for the test set, here using a confidence level of 99%:
-```python rf.predict_int(X_test, confidence=0.99) ``` ```numpy array([[-
-171902.2 , 953866.2 ], [-276818.01, 848950.39], [ 22679.37, 1148447.77], ...,
-[ 242954.02, 1368722.42], [-308093.73, 817674.67], [-227057.4 , 898711. ]]) ```
-The output is a [NumPy](https://numpy.org) array with a row for each test
-instance, and where the two columns specify the lower and upper bound of each
-prediction interval. We may request that the intervals are cut to exclude
-impossible values, in this case below 0, and if we also rely on the default
-confidence level (0.95), the output intervals will be a bit tighter: ```python
-rf.predict_int(X_test, y_min=0) ``` ```numpy array([[ 152258.55, 629705.45],
-[ 47342.74, 524789.64], [ 346840.12, 824287.02], ..., [ 567114.77, 1044561.67],
-[ 16067.02, 493513.92], [ 97103.35, 574550.25]]) ``` The above intervals are
-not normalized, i.e., they are all of the same size (at least before they are
-cut). We could make them more informative through normalization using
-difficulty estimates; objects considered more difficult will be assigned wider
-intervals. We will use a `DifficultyEstimator` from the `crepes.extras` module
-for this purpose. Here we estimate the difficulty by the standard deviation of
-the target of the k (default `k=25`) nearest neighbors in the proper training
-set to each object in the calibration set. A small value (beta) is added to the
-estimates, which may be given through an argument to the function; below we
-just use the default, i.e., `beta=0.01`. We first obtain the difficulty
-estimates for the calibration set: ```python from crepes.extras import
-DifficultyEstimator de = DifficultyEstimator() de.fit(X_prop_train,
-y=y_prop_train) sigmas_cal = de.apply(X_cal) ``` These can now be used for the
-calibration, which (under the hood) will produce a normalized conformal
-regressor: ```python rf.calibrate(residuals, sigmas=sigmas_cal) ``` We need
-difficulty estimates for the test set too, which we provide as input to
-`predict_int`: ```python sigmas_test = de.apply(X_test) rf.predict_int(X_test,
-sigmas=sigmas_test, y_min=0) ``` ```numpy array([[ 226719.06607977,
-555244.93392023], [ 173767.90753715, 398364.47246285], [ 124690.70166966,
-1046436.43833034], ..., [ 607949.71540572, 1003726.72459428], [ 188671.3752278
-, 320909.5647722 ], [ 145340.39076824, 526313.20923176]]) ``` Depending on the
-employed difficulty estimator, the normalized intervals may sometimes be
-unreasonably large, in the sense that they may be several times larger than any
-previously observed error. Moreover, if the difficulty estimator is
-uninformative, e.g., completely random, the varying interval sizes may give a
-false impression of that we can expect lower prediction errors for instances
-with tighter intervals. Ideally, a difficulty estimator providing little or no
-information on the expected error should instead lead to more uniformly
-distributed interval sizes. A Mondrian conformal regressor can be used to
-address these problems, by dividing the object space into non-overlapping so-
-called Mondrian categories, and forming a (standard) conformal regressor for
-each category. The category membership of the objects can be provided as an
-additional argument, named `bins`, for the `fit` method. Here we use the helper
-function `binning` from `crepes.extras` to form Mondrian categories by equal-
-sized binning of the difficulty estimates; the function returns labels for the
-calibration objects the we provide as input to the calibration, and we also get
-thresholds for the bins, which can use later when binning the test objects:
-```python from crepes.extras import binning bins_cal, bin_thresholds = binning
-(sigmas_cal, bins=20) rf.calibrate(residuals, bins=bins_cal) ``` Let us now get
-the labels of the Mondrian categories for the test objects and use them when
-predicting intervals: ```python bins_test = binning(sigmas_test,
-bins=bin_thresholds) rf.predict_int(X_test, bins=bins_test, y_min=0) ```
-```numpy array([[ 206379.7 , 575584.3 ], [ 144014.65, 428117.73], [ 17965.57,
-1153161.57], ..., [ 653865.22, 957811.22], [ 174264.87, 335316.07],
-[ 140587.46, 531066.14]]) ``` We could very easily switch from conformal
-regressors to conformal predictive systems. The latter produce cumulative
-distribution functions (conformal predictive distributions). From these we can
-generate prediction intervals, but we can also obtain percentiles, calibrated
-point predictions, as well as p-values for given target values. Let us see how
-we can go ahead to do that. Well, there is only one thing above that changes:
-just provide `cps=True` to the `calibrate` method. We can, for example, form
-normalized Mondrian conformal predictive systems, by providing both `bins` and
-`sigmas` to the `calibrate` method. Here we will consider Mondrian categories
-formed from binning the point predictions: ```python bins_cal, bin_thresholds =
-binning(rf.predict(X_cal), bins=5) rf.calibrate(residuals, sigmas=sigmas_cal,
-bins=bins_cal, cps=True) ``` By providing the bins (and sigmas) for the test
-objects, we can now make predictions with the conformal predictive system,
-through the method `predict_cps`. The output of this method can be controlled
-quite flexibly; here we request prediction intervals with 95% confidence to be
-output: ```python bins_test = binning(rf.predict(X_test), bins=bin_thresholds)
-rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test,
-lower_percentiles=2.5, higher_percentiles=97.5, y_min=0) ``` ```numpy array([
-[ 245826.3422693 , 517315.83618985], [ 145348.03415848, 392968.15587997],
-[ 148774.65461212, 1034300.84195976], ..., [ 589200.5725957 ,
-1057013.89102007], [ 171938.29382952, 317732.31611141], [ 167498.01540504,
-482328.98552632]]) ``` If we would like to take a look at the p-values for the
-true targets (these should be uniformly distributed), we can do the following:
-```python rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test, y=y_test)
-``` ```numpy array([0.98603614, 0.87178256, 0.44201984, ..., 0.05688804,
+crepes ``` ## Documentation For the complete documentation, see
+[crepes.readthedocs.io](https://crepes.readthedocs.io/en/latest/). ##
+Quickstart Let us illustrate the use of `crepes` by importing a dataset from
+[www.openml.org](https://www.openml.org), which we split into a training and a
+test set using `train_test_split` from [sklearn](https://scikit-learn.org), and
+then further split the training set into a proper training set and a
+calibration set: ```python from sklearn.datasets import fetch_openml from
+sklearn.model_selection import train_test_split dataset = fetch_openml
+(name="house_sales", version=3) X = dataset.data.values.astype(float) y =
+dataset.target.values.astype(float) X_train, X_test, y_train, y_test =
+train_test_split(X, y, test_size=0.5) X_prop_train, X_cal, y_prop_train, y_cal
+= train_test_split(X_train, y_train, test_size=0.25) ``` Let us now "wrap" a
+`RandomForestRegressor` from [sklearn](https://scikit-learn.org) using the
+class `Wrap` from `crepes` and fit it (in the usual way) to the proper training
+set: ```python from sklearn.ensemble import RandomForestRegressor from crepes
+import Wrap rf = Wrap(RandomForestRegressor()) rf.fit(X_prop_train,
+y_prop_train) ``` We can use the fitted model to obtain point predictions
+(again, in the usual way) for the calibration objects, from which we can
+calculate the residuals. These residuals are exactly what we need to
+"calibrate" the learner: ```python residuals = y_cal - rf.predict(X_cal)
+rf.calibrate(residuals) ``` A (standard) conformal regressor was formed (under
+the hood). We may now use it for obtaining prediction intervals for the test
+set, here using a confidence level of 99%: ```python rf.predict_int(X_test,
+confidence=0.99) ``` ```numpy array([[-171902.2 , 953866.2 ], [-276818.01,
+848950.39], [ 22679.37, 1148447.77], ..., [ 242954.02, 1368722.42], [-
+308093.73, 817674.67], [-227057.4 , 898711. ]]) ``` The output is a [NumPy]
+(https://numpy.org) array with a row for each test instance, and where the two
+columns specify the lower and upper bound of each prediction interval. We may
+request that the intervals are cut to exclude impossible values, in this case
+below 0, and if we also rely on the default confidence level (0.95), the output
+intervals will be a bit tighter: ```python rf.predict_int(X_test, y_min=0) ```
+```numpy array([[ 152258.55, 629705.45], [ 47342.74, 524789.64], [ 346840.12,
+824287.02], ..., [ 567114.77, 1044561.67], [ 16067.02, 493513.92], [ 97103.35,
+574550.25]]) ``` The above intervals are not normalized, i.e., they are all of
+the same size (at least before they are cut). We could make them more
+informative through normalization using difficulty estimates; objects
+considered more difficult will be assigned wider intervals. We will use a
+`DifficultyEstimator` from the `crepes.extras` module for this purpose. Here we
+estimate the difficulty by the standard deviation of the target of the k
+(default `k=25`) nearest neighbors in the proper training set to each object in
+the calibration set. A small value (beta) is added to the estimates, which may
+be given through an argument to the function; below we just use the default,
+i.e., `beta=0.01`. We first obtain the difficulty estimates for the calibration
+set: ```python from crepes.extras import DifficultyEstimator de =
+DifficultyEstimator() de.fit(X_prop_train, y=y_prop_train) sigmas_cal =
+de.apply(X_cal) ``` These can now be used for the calibration, which (under the
+hood) will produce a normalized conformal regressor: ```python rf.calibrate
+(residuals, sigmas=sigmas_cal) ``` We need difficulty estimates for the test
+set too, which we provide as input to `predict_int`: ```python sigmas_test =
+de.apply(X_test) rf.predict_int(X_test, sigmas=sigmas_test, y_min=0) ```
+```numpy array([[ 226719.06607977, 555244.93392023], [ 173767.90753715,
+398364.47246285], [ 124690.70166966, 1046436.43833034], ..., [ 607949.71540572,
+1003726.72459428], [ 188671.3752278 , 320909.5647722 ], [ 145340.39076824,
+526313.20923176]]) ``` Depending on the employed difficulty estimator, the
+normalized intervals may sometimes be unreasonably large, in the sense that
+they may be several times larger than any previously observed error. Moreover,
+if the difficulty estimator is uninformative, e.g., completely random, the
+varying interval sizes may give a false impression of that we can expect lower
+prediction errors for instances with tighter intervals. Ideally, a difficulty
+estimator providing little or no information on the expected error should
+instead lead to more uniformly distributed interval sizes. A Mondrian conformal
+regressor can be used to address these problems, by dividing the object space
+into non-overlapping so-called Mondrian categories, and forming a (standard)
+conformal regressor for each category. The category membership of the objects
+can be provided as an additional argument, named `bins`, for the `fit` method.
+Here we use the helper function `binning` from `crepes.extras` to form Mondrian
+categories by equal-sized binning of the difficulty estimates; the function
+returns labels for the calibration objects the we provide as input to the
+calibration, and we also get thresholds for the bins, which can use later when
+binning the test objects: ```python from crepes.extras import binning bins_cal,
+bin_thresholds = binning(sigmas_cal, bins=20) rf.calibrate(residuals,
+bins=bins_cal) ``` Let us now get the labels of the Mondrian categories for the
+test objects and use them when predicting intervals: ```python bins_test =
+binning(sigmas_test, bins=bin_thresholds) rf.predict_int(X_test,
+bins=bins_test, y_min=0) ``` ```numpy array([[ 206379.7 , 575584.3 ],
+[ 144014.65, 428117.73], [ 17965.57, 1153161.57], ..., [ 653865.22, 957811.22],
+[ 174264.87, 335316.07], [ 140587.46, 531066.14]]) ``` We could very easily
+switch from conformal regressors to conformal predictive systems. The latter
+produce cumulative distribution functions (conformal predictive distributions).
+From these we can generate prediction intervals, but we can also obtain
+percentiles, calibrated point predictions, as well as p-values for given target
+values. Let us see how we can go ahead to do that. Well, there is only one
+thing above that changes: just provide `cps=True` to the `calibrate` method. We
+can, for example, form normalized Mondrian conformal predictive systems, by
+providing both `bins` and `sigmas` to the `calibrate` method. Here we will
+consider Mondrian categories formed from binning the point predictions:
+```python bins_cal, bin_thresholds = binning(rf.predict(X_cal), bins=5)
+rf.calibrate(residuals, sigmas=sigmas_cal, bins=bins_cal, cps=True) ``` By
+providing the bins (and sigmas) for the test objects, we can now make
+predictions with the conformal predictive system, through the method
+`predict_cps`. The output of this method can be controlled quite flexibly; here
+we request prediction intervals with 95% confidence to be output: ```python
+bins_test = binning(rf.predict(X_test), bins=bin_thresholds) rf.predict_cps
+(X_test, sigmas=sigmas_test, bins=bins_test, lower_percentiles=2.5,
+higher_percentiles=97.5, y_min=0) ``` ```numpy array([[ 245826.3422693 ,
+517315.83618985], [ 145348.03415848, 392968.15587997], [ 148774.65461212,
+1034300.84195976], ..., [ 589200.5725957 , 1057013.89102007],
+[ 171938.29382952, 317732.31611141], [ 167498.01540504, 482328.98552632]]) ```
+If we would like to take a look at the p-values for the true targets (these
+should be uniformly distributed), we can do the following: ```python
+rf.predict_cps(X_test, sigmas=sigmas_test, bins=bins_test, y=y_test) ```
+```numpy array([0.98603614, 0.87178256, 0.44201984, ..., 0.05688804,
 0.09473604, 0.31069913]) ``` We may request that the `predict_cps` method
 returns the full conformal predictive distribution (CPD) for each test
 instance, as defined by the threshold values, by setting `return_cpds=True`.
 The format of the distributions vary with the type of conformal predictive
 system; for a standard and normalized CPS, the output is an array with a row
 for each test instance and a column for each calibration instance (residual),
 while for a Mondrian CPS, the default output is a vector containing one CPD per
```

