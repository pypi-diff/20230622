# Comparing `tmp/ProcessOptimizer-0.8.0.tar.gz` & `tmp/ProcessOptimizer-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProcessOptimizer-0.8.0.tar", last modified: Thu Apr 13 12:33:23 2023, max compression
+gzip compressed data, was "ProcessOptimizer-0.8.1.tar", last modified: Thu Jun 22 06:57:36 2023, max compression
```

## Comparing `ProcessOptimizer-0.8.0.tar` & `ProcessOptimizer-0.8.1.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:23.305995 ProcessOptimizer-0.8.0/
--rw-rw-rw-   0        0        0    11783 2023-04-13 12:33:23.301193 ProcessOptimizer-0.8.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:21.478931 ProcessOptimizer-0.8.0/ProcessOptimizer/
--rw-rw-rw-   0        0        0     1845 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/__init__.py
--rw-rw-rw-   0        0        0    11574 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/acquisition.py
--rw-rw-rw-   0        0        0    29142 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/bokeh_plot.py
--rw-rw-rw-   0        0        0     8781 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/callbacks.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:21.692027 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/
--rw-rw-rw-   0        0        0      425 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/__init__.py
--rw-rw-rw-   0        0        0    18835 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/forest.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:21.856753 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gaussian_process/
--rw-rw-rw-   0        0        0       85 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gaussian_process/__init__.py
--rw-rw-rw-   0        0        0    17518 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gaussian_process/gpr.py
--rw-rw-rw-   0        0        0    15219 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gaussian_process/kernels.py
--rw-rw-rw-   0        0        0     4809 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gbrt.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:22.505514 ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/
--rw-rw-rw-   0        0        0        0 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/__init__.py
--rw-rw-rw-   0        0        0     3586 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/benchmarks.py
--rw-rw-rw-   0        0        0      605 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/branin_hoo.py
--rw-rw-rw-   0        0        0     2952 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/model_system.py
--rw-rw-rw-   0        0        0     6372 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/noise_models.py
--rw-rw-rw-   0        0        0     1359 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:23.096709 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/
--rw-rw-rw-   0        0        0     3562 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/_NSGA2.py
--rw-rw-rw-   0        0        0      334 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/__init__.py
--rw-rw-rw-   0        0        0    11223 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/base.py
--rw-rw-rw-   0        0        0     4335 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/dummy.py
--rw-rw-rw-   0        0        0     7101 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/forest.py
--rw-rw-rw-   0        0        0     6836 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/gbrt.py
--rw-rw-rw-   0        0        0    10770 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/gp.py
--rw-rw-rw-   0        0        0    47713 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/optimizer.py
--rw-rw-rw-   0        0        0    89769 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/plots.py
--rw-rw-rw-   0        0        0    28205 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/searchcv.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:23.245896 ProcessOptimizer-0.8.0/ProcessOptimizer/space/
--rw-rw-rw-   0        0        0       71 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/space/__init__.py
--rw-rw-rw-   0        0        0    41037 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/space/constraints.py
--rw-rw-rw-   0        0        0    30734 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/space/space.py
--rw-rw-rw-   0        0        0     5265 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/space/transformers.py
--rw-rw-rw-   0        0        0    33016 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/ProcessOptimizer/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 12:33:21.565997 ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/
--rw-rw-rw-   0        0        0    11783 2023-04-13 12:33:20.000000 ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1411 2023-04-13 12:33:20.000000 ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 12:33:20.000000 ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-04-13 12:33:20.000000 ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-04-13 12:33:20.000000 ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    10315 2022-09-06 07:46:58.000000 ProcessOptimizer-0.8.0/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 12:33:23.306995 ProcessOptimizer-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1613 2023-04-13 12:27:44.000000 ProcessOptimizer-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.642037 ProcessOptimizer-0.8.1/
+-rw-rw-rw-   0        0        0     1238 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/AUTHORS_scikit_optimize.md
+-rw-rw-rw-   0        0        0     1598 2023-02-14 09:41:21.000000 ProcessOptimizer-0.8.1/LICENSE.md
+-rw-rw-rw-   0        0        0    10809 2023-06-22 06:57:36.642037 ProcessOptimizer-0.8.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.428574 ProcessOptimizer-0.8.1/ProcessOptimizer/
+-rw-rw-rw-   0        0        0     1845 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/__init__.py
+-rw-rw-rw-   0        0        0    11574 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/acquisition.py
+-rw-rw-rw-   0        0        0    29142 2022-03-10 13:53:50.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/bokeh_plot.py
+-rw-rw-rw-   0        0        0     8781 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/callbacks.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.458753 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/
+-rw-rw-rw-   0        0        0      425 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/__init__.py
+-rw-rw-rw-   0        0        0    18835 2023-01-26 13:09:11.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/forest.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.480910 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/
+-rw-rw-rw-   0        0        0       85 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/__init__.py
+-rw-rw-rw-   0        0        0    17518 2023-06-07 11:59:09.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/gpr.py
+-rw-rw-rw-   0        0        0    15220 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/kernels.py
+-rw-rw-rw-   0        0        0     4809 2021-09-23 13:20:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gbrt.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.541304 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/
+-rw-rw-rw-   0        0        0        0 2022-11-09 08:13:46.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/__init__.py
+-rw-rw-rw-   0        0        0     7547 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/benchmarks.py
+-rw-rw-rw-   0        0        0      605 2022-11-09 08:13:46.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/branin_hoo.py
+-rw-rw-rw-   0        0        0     4455 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/model_system.py
+-rw-rw-rw-   0        0        0     7440 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/noise_models.py
+-rw-rw-rw-   0        0        0     1359 2022-11-09 08:13:46.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/second_order_polynomial_2d.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.591637 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/
+-rw-rw-rw-   0        0        0     3562 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/_NSGA2.py
+-rw-rw-rw-   0        0        0      334 2021-03-19 12:03:36.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/__init__.py
+-rw-rw-rw-   0        0        0    11223 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/base.py
+-rw-rw-rw-   0        0        0     4335 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/dummy.py
+-rw-rw-rw-   0        0        0     7101 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/forest.py
+-rw-rw-rw-   0        0        0     6836 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gbrt.py
+-rw-rw-rw-   0        0        0    10770 2023-05-16 08:56:50.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gp.py
+-rw-rw-rw-   0        0        0    50046 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/optimizer.py
+-rw-rw-rw-   0        0        0    89768 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/plots.py
+-rw-rw-rw-   0        0        0    28205 2022-01-13 12:11:20.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/searchcv.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.640006 ProcessOptimizer-0.8.1/ProcessOptimizer/space/
+-rw-rw-rw-   0        0        0       71 2021-07-29 06:17:13.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/__init__.py
+-rw-rw-rw-   0        0        0    41031 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/constraints.py
+-rw-rw-rw-   0        0        0    30787 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/space.py
+-rw-rw-rw-   0        0        0     5265 2023-05-02 07:34:39.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/space/transformers.py
+-rw-rw-rw-   0        0        0    33016 2023-03-30 10:22:43.000000 ProcessOptimizer-0.8.1/ProcessOptimizer/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:57:36.440656 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/
+-rw-rw-rw-   0        0        0    10809 2023-06-22 06:57:34.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1449 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      224 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-22 06:57:35.000000 ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10361 2023-05-16 08:56:50.000000 ProcessOptimizer-0.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 06:57:36.642037 ProcessOptimizer-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1613 2023-06-22 06:54:32.000000 ProcessOptimizer-0.8.1/setup.py
```

### Comparing `ProcessOptimizer-0.8.0/PKG-INFO` & `ProcessOptimizer-0.8.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,144 +1,132 @@
-Metadata-Version: 2.1
-Name: ProcessOptimizer
-Version: 0.8.0
-Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
-Home-page: https://github.com/novonordisk-research/ProcessOptimizer
-Author: Novo Nordisk, Research & Early Development
-License: BSD
-Description: <div align="center">
-        <pre>
-          _____                              ____        _   _           _              
-         |  __ \                            / __ \      | | (_)         (_)             
-         | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
-         |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
-         | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
-         |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|   
-                                                  | |                                   
-                                                  |_|                                   
-        </pre>
-        <a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version" height="18"></a>
-        <a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/workflows/Python%20package/badge.svg" alt="Tests" height="18"></a>
-        <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
-        <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue" alt="Runs on" /></a>
-        <a href="https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/LICENSE.md"><img src="https://img.shields.io/pypi/l/ProcessOptimizer" alt="PyPI - License" /></a>
-        <a href="https://scikit-optimize.github.io/stable/"><img src="https://img.shields.io/badge/BuildOn-Scikit--Optimize-brightgreen" alt="Scikit-Optimize" /></a>
-        <a href="https://doi.org/10.5281/zenodo.5155295"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5155295.svg" alt="DOI"></a>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)](https://pepy.tech/project/processoptimizer)
-        </div>
-        
-        ----------
-        This readme.md is work in progress
-        
-        ## Table of Contents
-         * [ProcessOptimizer](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#processoptimizer)
-         * [Installation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#installation)
-         * [How does it work?](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#how-does-it-work?)
-         * [Citation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#Citation)
-         * [Contributions](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#contributions)
-         * [Related work](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#related-work)
-         * [PyPi](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#pypi)
-         
-        
-        ## ProcessOptimizer
-        
-        ProcessOptimizer is a fork of scikit-optimize. ProcessOptimizer will fundamentally function like scikit-optimize, 
-        yet developments are focussed on bringing improvements to help optimizing real world processes, like chemistry or baking.
-        For examples on use, checkout https://github.com/novonordisk-research/ProcessOptimizer/tree/develop/examples.
-        
-        ## Installation
-        
-        ProcessOptimizer can be installed using `pip install ProcessOptimizer`
-        The repository and examples can be found at https://github.com/novonordisk-research/ProcessOptimizer
-        ProcessOptimizer can also be installed by running `pip install -e .` in top directory of the cloned repository.
-        
-        ## How does it work?
-        
-        This package is intended for real world process optimization problems of black-box functions. This could e.g. be some complex chemical reaction where no reliable analytical model mapping input variables to the output is readily available. <br/>
-        Bayesian optimization is a great tool for optimizing black-box functions where the input space has many dimensions and the function is expensive to evaluate in terms of time and/or resources.<br/>
-        **Notice that this tool is designed to solve minimization problems.** It is therefore important to define the scoring function such that it turns into a minimization problem. <br/>
-        Below is an illustrative example of minimization of the Booth function in 2 dimensions using the `ProcessOptimizer` package. Notice that in real world applications the function would be black box (and typically the input space would have more than 2 dimensions). However, it would still be possible to evaluate the function given a set of input values and thus use the same framework for optimization. <br/>
-        The Booth function is a 2-dimensional function defined by [Booth Function (sfu.ca)](https://www.sfu.ca/~ssurjano/booth.html). In this example uniformly distributed random noise between 0-5% of the function value is added using `np.random`.
-        ```python
-        def Booth(x0, x1):
-            return ((x0 + 2 * x1 - 7)**2 + (2 * x0 + x1 - 5)**2) * (1 + 0.05 * np.random.rand())
-        ```
-        Below is an image of the Booth function on the square <img src="https://render.githubusercontent.com/render/math?math=x_i \in \left[ 0,5 \right]"> for i=0,1.
-        
-        
-        ![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Booth_function.png)
-        
-        Suppose you are given the task of minimizing the function on the domain only using empirical observations and without any analytical function. <br/>
-        Working with the ProcessOptimizer package you simply define the `Space` and create an `Optimizer` object.<br/>
-        The `Space` object takes a list of dimensions which can either be `Real`, `Integer` or `Categorical`. `Real` dimensions are defined by the maximum and minimum values.<br/>
-        The `Optimizer` object initialized below uses GP (Gaussian Process). This means that after each step a Gaussian Process is fitted to the observations, which is used as a posterior distribution. Combined with an acquisition function the next point that should be explored can be determined. Notice that this process only takes place once n_initial_points of initial data has been aqcuired. In this case `LHS = True` (latin hypercube sampling) has been used as the initial sampling strategy for the first 6 points.
-        ```python
-        SPACE = Space([Real(0,5), Real(0,5)])   
-        
-        opt = Optimizer(SPACE, base_estimator = "GP", n_initial_points = 6, lhs = True)
-        ```
-        The optimizer can now be used in steps by calling the `.ask()` function, evaluating the function at the given point and use `.tell()` the `Optimizer` the result. In practise it would work like this. First ask the optimizer for the next point to perform an experiment:
-        ```python
-        opt.ask()
-        >>> [3.75, 3.75]
-        ```
-        Now go to the laboratory or wherever the experiment can be performed and use the values above. In this example the experiment can simply be performed by evaluating the Booth function using the values above:
-        ```python
-        Booth(3.75, 3.75)
-        >>> 59.313996676981354
-        ```
-        When a result has been obtained the user needs to tell the output to the `Optimizer`. This is done using the `.tell()` function:
-        ```python
-        res = opt.tell([3.75, 3.75], 59.313996676981354)
-        ```
-        The `res` object returned by tell contains a model of the Gaussian Process predicted mean. This model can be plotted using `plot_objective(res)`. Below is a gif of how the Gaussian Process predicted mean evolves after the first 6 initial points and until 20 points have been sampled in total. The orange dots visualise each evaluation of the function and the red dot shows the position of the expected minimum. In the diagonal of the figure dependence plots are shown. These show how the function depend on each input variable with other input variables kept constant at the expected minimum.
-        
-        <img src="https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/BO_GIF.gif" width="500">
-        
-         
-        Notice that this is an optimization tool and not a modelling tool. This means that the optimizer finds an approximate solution for the global minimum quickly however it does not guarantee that the Gaussian Process predicted mean is an accurate model on the entire domain.<br/>
-        
-        The best observation against the number of observations can be plotted with `plot_convergence(res)`:
-         
-        ![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Convergence_plot.png)
-        
-        ## Citation
-        
-        If you use the package in relation to a citation, please cite: https://doi.org/10.5281/zenodo.5155295.<br>
-        Please also cite the underlaying package (scikit-optimize).
-        
-        ## Contributions
-        
-        Feel free to play around with algorithm. Should you encounter errors while using ProcessOptimizer, please report them
-        at https://github.com/novonordisk-research/ProcessOptimizer/issues. <br>
-        To help solve the issues, please: <br>
-        
-        - Provide minimal amount of code to reproduce the error
-        - State versions of ProcesOptimizer, sklearn, numpy, ...
-        - Describe the expected behavior of the code <br>
-        
-        If you would like to contribute by making anything from documentation to feature-additions, THANK YOU. Please open a pull request 
-        marked as *WIP* as early as possible and describe the issue you seek to solve and outline your planned solution. <br>
-        Pull requests to the develop branch will be automatically tested using pytest and flake8. We'll be happy to help solving potential
-        issues that could arise here.
-        
-        ## Related work
-        
-        We are currently building a GUI to offer the power of Bayesian Process Optimization to non-coders. Stay tuned. (Sneak-peak at https://www.browniebee.dk/uk/)
-        
-        ## PyPi
-        
-        If you have not packaged before check out https://packaging.python.org/tutorials/packaging-projects/
-        To upload a new version to PyPi do the following in the root folder of the project:
-        
-        - In terminal run the command "pytest" and make sure there are no errors
-        - Change version number in setup.py
-        - Change version number in ProcessOptimizer/\_\_init\_\_.py
-        - Remember to `pip install twine` if running in a new virtual env
-        - Run `python setup.py sdist bdist_wheel`
-        - Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-Provides-Extra: bokeh
-Provides-Extra: browniebee
+<div align="center">
+<pre>
+  _____                              ____        _   _           _              
+ |  __ \                            / __ \      | | (_)         (_)             
+ | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
+ |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
+ | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
+ |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|   
+                                          | |                                   
+                                          |_|                                   
+</pre>
+<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version" height="18"></a>
+<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/workflows/Python%20package/badge.svg" alt="Tests" height="18"></a>
+<a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
+<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue" alt="Runs on" /></a>
+<a href="https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/LICENSE.md"><img src="https://img.shields.io/pypi/l/ProcessOptimizer" alt="PyPI - License" /></a>
+<a href="https://scikit-optimize.github.io/stable/"><img src="https://img.shields.io/badge/BuildOn-Scikit--Optimize-brightgreen" alt="Scikit-Optimize" /></a>
+<a href="https://doi.org/10.5281/zenodo.5155295"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5155295.svg" alt="DOI"></a>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)](https://pepy.tech/project/processoptimizer)
+</div>
+
+----------
+This readme.md is work in progress
+
+## Table of Contents
+ * [ProcessOptimizer](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#processoptimizer)
+ * [Installation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#installation)
+ * [How does it work?](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#how-does-it-work?)
+ * [Citation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#Citation)
+ * [Contributions](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#contributions)
+ * [Related work](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#related-work)
+ * [PyPi](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#pypi)
+ 
+
+## ProcessOptimizer
+
+ProcessOptimizer is a fork of scikit-optimize. ProcessOptimizer will fundamentally function like scikit-optimize, 
+yet developments are focussed on bringing improvements to help optimizing real world processes, like chemistry or baking.
+For examples on use, checkout https://github.com/novonordisk-research/ProcessOptimizer/tree/develop/examples.
+
+## Installation
+
+ProcessOptimizer can be installed using `pip install ProcessOptimizer`
+The repository and examples can be found at https://github.com/novonordisk-research/ProcessOptimizer
+ProcessOptimizer can also be installed by running `pip install -e .` in top directory of the cloned repository.
+
+## How does it work?
+
+This package is intended for real world process optimization problems of black-box functions. This could e.g. be some complex chemical reaction where no reliable analytical model mapping input variables to the output is readily available. <br/>
+Bayesian optimization is a great tool for optimizing black-box functions where the input space has many dimensions and the function is expensive to evaluate in terms of time and/or resources.<br/>
+**Notice that this tool is designed to solve minimization problems.** It is therefore important to define the scoring function such that it turns into a minimization problem. <br/>
+Below is an illustrative example of minimization of the Booth function in 2 dimensions using the `ProcessOptimizer` package. Notice that in real world applications the function would be black box (and typically the input space would have more than 2 dimensions). However, it would still be possible to evaluate the function given a set of input values and thus use the same framework for optimization. <br/>
+The Booth function is a 2-dimensional function defined by [Booth Function (sfu.ca)](https://www.sfu.ca/~ssurjano/booth.html). In this example uniformly distributed random noise between 0-5% of the function value is added using `np.random`.
+```python
+def Booth(x0, x1):
+    return ((x0 + 2 * x1 - 7)**2 + (2 * x0 + x1 - 5)**2) * (1 + 0.05 * np.random.rand())
+```
+Below is an image of the Booth function on the square <img src="https://render.githubusercontent.com/render/math?math=x_i \in \left[ 0,5 \right]"> for i=0,1.
+
+
+![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Booth_function.png)
+
+Suppose you are given the task of minimizing the function on the domain only using empirical observations and without any analytical function. <br/>
+Working with the ProcessOptimizer package you simply define the `Space` and create an `Optimizer` object.<br/>
+The `Space` object takes a list of dimensions which can either be `Real`, `Integer` or `Categorical`. `Real` dimensions are defined by the maximum and minimum values.<br/>
+The `Optimizer` object initialized below uses GP (Gaussian Process). This means that after each step a Gaussian Process is fitted to the observations, which is used as a posterior distribution. Combined with an acquisition function the next point that should be explored can be determined. Notice that this process only takes place once n_initial_points of initial data has been aqcuired. In this case `LHS = True` (latin hypercube sampling) has been used as the initial sampling strategy for the first 6 points.
+```python
+SPACE = Space([Real(0,5), Real(0,5)])   
+
+opt = Optimizer(SPACE, base_estimator = "GP", n_initial_points = 6, lhs = True)
+```
+The optimizer can now be used in steps by calling the `.ask()` function, evaluating the function at the given point and use `.tell()` the `Optimizer` the result. In practise it would work like this. First ask the optimizer for the next point to perform an experiment:
+```python
+opt.ask()
+>>> [3.75, 3.75]
+```
+Now go to the laboratory or wherever the experiment can be performed and use the values above. In this example the experiment can simply be performed by evaluating the Booth function using the values above:
+```python
+Booth(3.75, 3.75)
+>>> 59.313996676981354
+```
+When a result has been obtained the user needs to tell the output to the `Optimizer`. This is done using the `.tell()` function:
+```python
+res = opt.tell([3.75, 3.75], 59.313996676981354)
+```
+The `res` object returned by tell contains a model of the Gaussian Process predicted mean. This model can be plotted using `plot_objective(res)`. Below is a gif of how the Gaussian Process predicted mean evolves after the first 6 initial points and until 20 points have been sampled in total. The orange dots visualise each evaluation of the function and the red dot shows the position of the expected minimum. In the diagonal of the figure dependence plots are shown. These show how the function depend on each input variable with other input variables kept constant at the expected minimum.
+
+<img src="https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/BO_GIF.gif" width="500">
+
+ 
+Notice that this is an optimization tool and not a modelling tool. This means that the optimizer finds an approximate solution for the global minimum quickly however it does not guarantee that the Gaussian Process predicted mean is an accurate model on the entire domain.<br/>
+
+The best observation against the number of observations can be plotted with `plot_convergence(res)`:
+ 
+![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Convergence_plot.png)
+
+## Citation
+
+If you use the package in relation to a citation, please cite: https://doi.org/10.5281/zenodo.5155295.<br>
+Please also cite the underlaying package (scikit-optimize).
+
+## Contributions
+
+Feel free to play around with algorithm. Should you encounter errors while using ProcessOptimizer, please report them
+at https://github.com/novonordisk-research/ProcessOptimizer/issues. <br>
+To help solve the issues, please: <br>
+
+- Provide minimal amount of code to reproduce the error
+- State versions of ProcesOptimizer, sklearn, numpy, ...
+- Describe the expected behavior of the code <br>
+
+If you would like to contribute by making anything from documentation to feature-additions, THANK YOU. Please open a pull request 
+marked as *WIP* as early as possible and describe the issue you seek to solve and outline your planned solution. <br>
+Pull requests to the develop branch will be automatically tested using pytest and flake8. We'll be happy to help solving potential
+issues that could arise here.
+
+## Related work
+
+We are currently building a GUI to offer the power of Bayesian Process Optimization to non-coders. Stay tuned. (Sneak-peak at https://www.browniebee.dk/uk/)
+
+## PyPi
+
+If you have not packaged before check out https://packaging.python.org/tutorials/packaging-projects/
+To upload a new version to PyPi do the following in the root folder of the project:
+
+- In terminal run the command "pytest" and make sure there are no errors
+- Change version number in setup.py
+- Change version number in ProcessOptimizer/\_\_init\_\_.py
+- Remember to `pip install twine` if running in a new virtual env. (You might also have to `pip install wheel`)
+- Run `python setup.py sdist bdist_wheel`
+- Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
```

#### html2text {}

```diff
@@ -1,26 +1,22 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.0 Summary: Sequential
-model-based optimization toolbox (forked from scikit-optimize) Home-page:
-https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
-Research & Early Development License: BSD Description:
-            _____                              ____        _   _           _
-
-           |  __ \                            / __ \      | | (_)         (_)
-
-           | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _
-                                 _______ _ __
-         |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  /
-                                   _ \ '__|
-         | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /
-                                   __/ |
-           |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/
-                                 ___\___|_|
-                                                               | |
+        _____                              ____        _   _           _
 
-                                                               |_|
+       |  __ \                            / __ \      | | (_)         (_)
+
+ | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __
+
+   |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \
+                                     '__|
+  | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |
+
+  |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|
+
+                                                           | |
+
+                                                           |_|
 [PyPI_version] [Tests] [built_with_Python3] [Runs_on] [PyPI_-_License] [Scikit-
   Optimize] [DOI] [![Downloads](https://static.pepy.tech/personalized-badge/
 processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)]
                  (https://pepy.tech/project/processoptimizer)
 ---------- This readme.md is work in progress ## Table of Contents *
 [ProcessOptimizer](https://github.com/novonordisk-research/ProcessOptimizer/
 blob/develop/README.md#processoptimizer) * [Installation](https://github.com/
@@ -130,11 +126,10 @@
 Bayesian Process Optimization to non-coders. Stay tuned. (Sneak-peak at https:/
 /www.browniebee.dk/uk/) ## PyPi If you have not packaged before check out
 https://packaging.python.org/tutorials/packaging-projects/ To upload a new
 version to PyPi do the following in the root folder of the project: - In
 terminal run the command "pytest" and make sure there are no errors - Change
 version number in setup.py - Change version number in ProcessOptimizer/
 \_\_init\_\_.py - Remember to `pip install twine` if running in a new virtual
-env - Run `python setup.py sdist bdist_wheel` - Run `python -m twine upload
-dist/*` (make sure that /dist only contains relevant version) Platform: UNKNOWN
-Description-Content-Type: text/markdown Provides-Extra: bokeh Provides-Extra:
-browniebee
+env. (You might also have to `pip install wheel`) - Run `python setup.py sdist
+bdist_wheel` - Run `python -m twine upload dist/*` (make sure that /dist only
+contains relevant version)
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/__init__.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from .utils import expected_minimum_random_sampling
 from .utils import load
 from .utils import cook_estimator, create_result, y_coverage
 from .plots import plot_objective, plot_objectives
 from .plots import plot_evaluations, plot_convergence
 from .plots import plot_Pareto, plot_expected_minimum_convergence
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 
 __all__ = (
     "acquisition",
     "benchmarks",
     "callbacks",
     "learning",
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/acquisition.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/acquisition.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/bokeh_plot.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/bokeh_plot.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/callbacks.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/callbacks.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/learning/forest.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/forest.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gaussian_process/gpr.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/gpr.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gaussian_process/kernels.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gaussian_process/kernels.py`

 * *Files 1% similar despite different names*

```diff
@@ -315,15 +315,15 @@
 
 
 class HammingKernel(sk_StationaryKernelMixin, sk_NormalizedKernelMixin,
                     Kernel):
     """
     The HammingKernel is used to handle categorical inputs.
 
-    ``K(x_1, x_2) = exp(\sum_{j=1}^{d} -ls_j * (I(x_1j != x_2j)))``
+    ``K(x_1, x_2) = exp(\\sum_{j=1}^{d} -ls_j * (I(x_1j != x_2j)))``
 
     Parameters
     -----------
     * `length_scale` [float, array-like, shape=[n_features,], 1.0 (default)]
         The length scale of the kernel. If a float, an isotropic kernel is
         used. If an array, an anisotropic kernel is used where each dimension
         of l defines the length-scale of the respective feature dimension.
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/learning/gbrt.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/learning/gbrt.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/branin_hoo.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/branin_hoo.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/noise_models.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/noise_models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,162 +1,192 @@
 from abc import ABC, abstractmethod
 from typing import Callable, List, Union, Optional
 
-from scipy.stats import norm, uniform
+import numpy as np
 
 class NoiseModel(ABC):
     """
     Abstract class that is the basis for noise models.
     """
     def __init__(
-            self,
-            noise_size: Optional[float]):
+        self,
+        noise_size: Optional[float],
+        seed: Optional[int] = 42,
+    ):
         """        
-        Parameters:
-        * `noise_size` [Option[float]]: The size of the noise. If ´None´, it signifies that
-            the class is compound, and should not have its own noise signal, but refer to
-            its compounding NoiseModels instead. An example is SumNoise, which sums the
-            noise of a list of noise models, but doesn't add any noise by itself."""
+        Parameters
+        ----------
+        * `noise_size` [Optional[float]]: 
+            The size (magnitude) of the noise. If ´None´, it signifies that
+            the class is compound, and should not have its own noise signal, 
+            but refer to its compounding NoiseModels instead. An example is 
+            SumNoise, which sums the noise of a list of noise models, but does
+            not add any noise by itself.
+        
+        * `seed` [Optional[int], default=42]:
+            Seed to pass forward to the numpy random number generator that is
+            used when providing samples with noise.
+        """
         # We could just set noise_dist and let that have a size, but being able to
         # directly set the size is more intuitive, and that would be complicated if it
         # was just one variable.
         # Note that this has the potential for problems if _noise_distribution does not
         # have "size" 1, but as long as it is only set by set_noise_type(), it should be
         # safe.
         self.noise_size = noise_size
-        self._noise_distribution: Callable[[],float]
+        self._rng = np.random.default_rng(seed)
         self.set_noise_type("normal")
+        self._noise_distribution: Callable[[], float]
 
     @abstractmethod
-    def get_noise(self,X,Y: float) -> float:
+    def get_noise(self, X, Y: float) -> float:
         pass
     
     @property
     def _sample_noise(self) -> float:
         """A raw noise value, to be used in the get_noise() function."""
         if self.noise_size is None:
             raise TypeError("Method \"raw_noise()\" for NoiseModel class "
                             f"{self.__class__.__name__} is not supposed to be called.")
+            
         return self._noise_distribution()*self.noise_size
     
-    def set_noise_type(self,noise_type: str):
+    def set_noise_type(self, noise_type: str):
         if noise_type in ["normal", "Gaussian", "norm"]:
-            self._noise_distribution = norm.rvs
+            self.noise_type = noise_type
+            self._noise_distribution = self._rng.normal
         elif noise_type == "uniform":
-            self._noise_distribution = uniform(loc=-1,scale=2).rvs
+            self.noise_type = noise_type
+            self._noise_distribution = lambda: self._rng.uniform(low=-1, high=1)
         else:
             raise ValueError(f"Noise distribution \"{noise_type}\" not recognised.")
-
+    
+    def set_seed(self, seed: Optional[int]):
+        # Instantiate the random number generator again
+        self._rng = np.random.default_rng(seed)
+        # Make sure to do the same for the noise distribution
+        if self.noise_type in ["normal", "Gaussian", "norm"]:
+            self._noise_distribution = self._rng.normal
+        elif self.noise_type == "uniform":
+            self._noise_distribution = lambda: self._rng.uniform(low=-1, high=1)
 
 class ConstantNoise(NoiseModel):
     """
     Noise model for noise that is independent of both the sampled point and the
     resulting score; The noise is constant. Another name is "additive noise", as the
     same noise is added to the score. This is typical for many measurements.
 
-    Parameters:
-    * `noise_size` [float, default 1]: The size of the noise. 
+    Parameters
+    ----------
+    * `noise_size` [float, default=1]: 
+        The size (magnitude) of the noise. 
     """
     def __init__(self, noise_size: float = 1, **kwargs):
         super().__init__(noise_size=noise_size, **kwargs)
 
-    def get_noise(self,_,Y: float) -> float:
+    def get_noise(self, _, Y: float) -> float:
         return self._sample_noise
 
     
 class ProportionalNoise(NoiseModel):
     """
     Noise model for noise proportional to the signal, but independent of the sampled
     point. Another name is "multiplicative noise", as the same noise is multiplied with
     the score. This is typical of some electronic measurements.
 
-    Parameters:
-    * `noise_size` [float, default 0.1]: The size of the noise relative to the signal.
+    Parameters
+    ----------
+    * `noise_size` [float, default=0.1]: 
+        The size of the noise relative to the signal.
     """
-    def __init__(self, noise_size : float = 0.1,**kwargs):
-        super().__init__(noise_size=noise_size,**kwargs)
+    def __init__(self, noise_size : float = 0.1, **kwargs):
+        super().__init__(noise_size=noise_size, **kwargs)
     
-    def get_noise(self,_,Y: float) -> float:
+    def get_noise(self, _, Y: float) -> float:
         return self._sample_noise*Y
     
 
 class DataDependentNoise(NoiseModel):
     """
     Noise model for noise that depends on the input parameters.
 
-    Parameters:
-    * `noise_function` [(parameters) -> NoiseModel]: A function that takes a set of
-        parameters, and returns a noise model to apply.
-
-    Examples:
+    Parameters
+    ----------
+    * `noise_function` [(parameters) -> NoiseModel]: 
+        A function that takes a set of parameters, and returns a noise model to 
+        apply.
 
+    Examples
+    --------
     To make additive noise proportional to the input parameter (not to the score):
     ```
-    noise_choice = lambda X: AdditiveNoise(noise_size=X)
+    noise_choice = lambda X: ConstantNoise(noise_size=X)
     noise_model = DataDependentNoise(noise_function=noise_choice)
     ```
 
-    To add additive noise except if X[0] is 0:
+    To add constant noise except if X[0] is 0:
     ```
-    noise_choice = lambda X: ZeroNoise() if X[0]==0 else AdditiveNoise()
+    noise_choice = lambda X: ZeroNoise() if X[0]==0 else ConstantNoise()
     noise_model = DataDependentNoise(noise_function=noise_choice)
     ```
     """
-    def __init__(self, noise_function: Callable[...,NoiseModel], **kwargs):
+    def __init__(self, noise_function: Callable[..., NoiseModel], **kwargs):
         self.noise_function = noise_function
         super().__init__(noise_size=None, **kwargs)
     
-    def get_noise(self,X,Y: float) -> float:
-        return self.noise_function(X).get_noise(X,Y)           
+    def get_noise(self, X, Y: float) -> float:
+        return self.noise_function(X).get_noise(X, Y)           
     
 class ZeroNoise(NoiseModel):
     """
     Noise model for zero noise. Doesn't take any arguments. Exist for consistency,
     and to be used in data dependent noise models.
     """
     def __init__(self):
         super().__init__(noise_size=0)
 
-    def get_noise(self,_,Y: float) -> float:
+    def get_noise(self, _, Y: float) -> float:
         return 0
 
 class SumNoise(NoiseModel):
     """
     Noise model that returns the sum of two or more noise models. Can be used if the
     total noise is a sum of constant and proportional noise.
 
-    Args:
-    * `noise_model_list` [List[Union[dict,NoiseModel]]]: List of either noise models, or
-        dicts containing at least the type of noise model to create.
+    Parameters
+    ----------
+    * `noise_model_list` [List[Union[dict, NoiseModel]]]: 
+        List of either noise models, or dicts containing at least the type of 
+        noise model to create.
 
     """
     def __init__(self,noise_model_list: List[Union[str,dict,NoiseModel]], **kwargs):
         super().__init__(noise_size = None,**kwargs)
         self.noise_model_list: List[NoiseModel]
         self.set_noise_model_list(noise_model_list=noise_model_list)
 
-    def set_noise_model_list(self,noise_model_list: List[Union[dict,NoiseModel]]):
+    def set_noise_model_list(self, noise_model_list: List[Union[dict, NoiseModel]]):
         self.noise_model_list = []
         for model_description in noise_model_list:
             self.noise_model_list.append(parse_noise_model(model_description))
 
-    def get_noise(self,X,Y: float) -> float:
-        noise_list = [model.get_noise(X,Y) for model in self.noise_model_list]
+    def get_noise(self, X, Y: float) -> float:
+        noise_list = [model.get_noise(X, Y) for model in self.noise_model_list]
         return sum(noise_list)
 
 
-def parse_noise_model(model: Union[str,dict,NoiseModel], **kwargs) -> NoiseModel:
-    if isinstance(model,NoiseModel):
+def parse_noise_model(model: Union[str, dict, NoiseModel], **kwargs) -> NoiseModel:
+    if isinstance(model, NoiseModel):
         return model
     elif type(model) == str:
         return noise_model_factory(model_type=model, **kwargs)
     else:
         return noise_model_factory(**model)
 
-def noise_model_factory(model_type: str, **kwargs)-> NoiseModel:
+def noise_model_factory(model_type: str, **kwargs) -> NoiseModel:
     if model_type == "constant":
         return ConstantNoise(**kwargs)
     elif model_type == "proportional":
         return ProportionalNoise(**kwargs)
     elif model_type == "zero":
         return ZeroNoise()
     else:
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/model_systems/second_order_polynomial_2d.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/model_systems/second_order_polynomial_2d.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/_NSGA2.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/_NSGA2.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/base.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/base.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/dummy.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/dummy.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/forest.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/forest.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/gbrt.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gbrt.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/gp.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/gp.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/optimizer/optimizer.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/optimizer/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,24 +24,35 @@
 from ..utils import cook_estimator
 from ..utils import create_result
 from ..utils import has_gradients
 from ..utils import is_listlike
 from ..utils import is_2Dlistlike
 from ..utils import normalize_dimensions
 
+from ..learning.gaussian_process.gpr import _param_for_white_kernel_in_Sum
+from ..learning.gaussian_process.kernels import WhiteKernel
+
 
 class Optimizer(object):
     """Run bayesian optimisation loop.
 
     An `Optimizer` represents the steps of a bayesian optimisation loop. To
     use it you need to provide your own loop mechanism. The various
     optimisers provided by `ProcessOptimizer` use this class under the hood.
 
     Use this class directly if you want to control the iterations of your
     bayesian optimisation loop.
+    
+    In default behavior, the optimizer will reset the modelled experimental
+    noise between each refitting (read: while adding new data). This is
+    described in Rasmussen and Williams chapter 2. 
+    Some users might want to plot, predict or sample from a model that includes
+    the modelling of the experimental noise: in that case, two helper methods
+    can "switch" the noise "on/off". Functions are called 'add_modelled_noise'
+    and 'remove_modelled_noise'.
 
     Parameters
     ----------
     * `dimensions` [list, shape=(n_dims,)]:
         List of search space dimensions.
         Each search dimension can be defined either as
 
@@ -84,17 +95,17 @@
         - `"gp_hedge"` Probabilistically choose one of the above three
           acquisition functions at every iteration.
             - The gains `g_i` are initialized to zero.
             - At every iteration,
                 - Each acquisition function is optimised independently to
                   propose an candidate point `X_i`.
                 - Out of all these candidate points, the next point `X_best` is
-                  chosen by $softmax(\eta g_i)$
+                  chosen by $softmax(\\eta g_i)$
                 - After fitting the surrogate model with `(X_best, y_best)`,
-                  the gains are updated such that $g_i -= \mu(X_i)$
+                  the gains are updated such that $g_i -= \\mu(X_i)$
         - `"EIps" for negated expected improvement per second to take into
           account the function compute time. Then, the objective function is
           assumed to return two values, the first being the objective value and
           the second being the time taken in seconds.
         - `"PIps"` for negated probability of improvement per second. The
           return type of the objective function is assumed to be similar to
           that of `"EIps
@@ -1165,7 +1176,37 @@
             self.n_objectives,
             self.__ObjectiveGP,
             np.array(self.space.transformed_bounds),
             MU=MU,
         )
 
         return pop, logbook, front
+    
+    # This function adds the modelled white noise to the regressor to allow predictions including noise
+    def add_modelled_noise(self):
+        '''
+        This method will add the noise that has been modelled to fit the data. (The noise is disabled
+        by default to reflect description in book on gaussian processes for Machine Learning
+        This has been described in Eq 2.24 of
+        http://www.gaussianprocess.org/gpml/chapters/RW2.pdf)
+        '''
+        if isinstance(self.models[-1].noise, str) and self.models[-1].noise != "gaussian":
+            raise ValueError("expected noise to be 'gaussian', got %s"
+                             % self.models[-1].noise)
+        noise_estimate = self.models[-1].noise_
+        white_present, white_param = _param_for_white_kernel_in_Sum(self.models[-1].kernel_)
+        if white_present:
+            self.models[-1].kernel_.set_params(**{white_param: WhiteKernel(noise_level=noise_estimate)})
+    
+    def remove_modelled_noise(self):
+        '''
+        This method resets the noise levels to only include the "true" uncertaincy of the main kernel
+        used for fitting and predicting. This method can be used in conjunction with the 
+        'add_modelled_noise()'
+        '''
+        if isinstance(self.models[-1].noise, str) and self.models[-1].noise != "gaussian":
+            raise ValueError("expected noise to be 'gaussian', got %s"
+                             % self.models[-1].noise)
+        white_present, white_param = _param_for_white_kernel_in_Sum(self.models[-1].kernel_)
+        if white_present:
+            self.models[-1].kernel_.set_params(**{white_param: WhiteKernel(noise_level=0.0)})
+
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/plots.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -1138,15 +1138,15 @@
     axes.scatter(
         highlighted[0],
         highlighted[1],
         c="k",
         s=30,
         marker="D",
         lw=0.0,
-        zorder=10,
+        zorder=9,
         clip_on=False,
     )
 
 def plot_objective_1d(
     result,
     n_points=40,
     n_samples=250,
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/searchcv.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/searchcv.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/space/constraints.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/space/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -825,20 +825,20 @@
             for ind_dim in constraint.dimensions:
                 if isinstance(space.dimensions[ind_dim], Categorical):
                     raise ValueError('SumEquals constraint can not be applied to categorical dimensions: {}'.format(space.dimensions[ind_dim]))
                 if isinstance(space.dimensions[ind_dim], Integer):
                     raise ValueError('SumEquals constraint can not be applied to integer dimensions: {}'.format(space.dimensions[ind_dim]))
             # Check if the sum equals constraint is below the combined lower 
             # bound of the space dimensions in question
-            low_limit_sum = np.sum(space.bounds[dim][0] for dim in constraint.dimensions)
+            low_limit_sum = sum(space.bounds[dim][0] for dim in constraint.dimensions)
             if low_limit_sum > constraint.value:
                 raise ValueError('Constraint cannot be met inside dimension limits, value ({}) is too small.'.format(constraint.value))
             # Check if the sum equals constraint is above the combined higher
             # bound of the space dimensions in question
-            high_limit_sum = np.sum(space.bounds[dim][1] for dim in constraint.dimensions)
+            high_limit_sum = sum(space.bounds[dim][1] for dim in constraint.dimensions)
             if high_limit_sum < constraint.value:
                 raise ValueError('Constraint cannot be met inside dimension limits, value ({}) is too large.'.format(constraint.value))
         elif isinstance(constraint, Conditional):
             # We run check_constraints on each constraint instance in the
             # conditional constraint. We only check them if they are not None
             if constraint.condition:
                 check_constraints(space, [constraint.condition])
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/space/space.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/space/space.py`

 * *Files 0% similar despite different names*

```diff
@@ -909,7 +909,9 @@
         transposed_samples = []
         for i in range(n):
             row = []
             for j in range(self.n_dims):
                 row.append(samples[j][i])
             transposed_samples.append(row)
         return transposed_samples
+    
+    # TODO: Add a R1 QRS sampling method here
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/space/transformers.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/space/transformers.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer/utils.py` & `ProcessOptimizer-0.8.1/ProcessOptimizer/utils.py`

 * *Files identical despite different names*

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/PKG-INFO` & `ProcessOptimizer-0.8.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,145 @@
 Metadata-Version: 2.1
 Name: ProcessOptimizer
-Version: 0.8.0
+Version: 0.8.1
 Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
 Home-page: https://github.com/novonordisk-research/ProcessOptimizer
 Author: Novo Nordisk, Research & Early Development
 License: BSD
-Description: <div align="center">
-        <pre>
-          _____                              ____        _   _           _              
-         |  __ \                            / __ \      | | (_)         (_)             
-         | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
-         |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
-         | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
-         |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|   
-                                                  | |                                   
-                                                  |_|                                   
-        </pre>
-        <a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version" height="18"></a>
-        <a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/workflows/Python%20package/badge.svg" alt="Tests" height="18"></a>
-        <a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
-        <a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue" alt="Runs on" /></a>
-        <a href="https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/LICENSE.md"><img src="https://img.shields.io/pypi/l/ProcessOptimizer" alt="PyPI - License" /></a>
-        <a href="https://scikit-optimize.github.io/stable/"><img src="https://img.shields.io/badge/BuildOn-Scikit--Optimize-brightgreen" alt="Scikit-Optimize" /></a>
-        <a href="https://doi.org/10.5281/zenodo.5155295"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5155295.svg" alt="DOI"></a>
-        
-        [![Downloads](https://static.pepy.tech/personalized-badge/processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)](https://pepy.tech/project/processoptimizer)
-        </div>
-        
-        ----------
-        This readme.md is work in progress
-        
-        ## Table of Contents
-         * [ProcessOptimizer](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#processoptimizer)
-         * [Installation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#installation)
-         * [How does it work?](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#how-does-it-work?)
-         * [Citation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#Citation)
-         * [Contributions](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#contributions)
-         * [Related work](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#related-work)
-         * [PyPi](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#pypi)
-         
-        
-        ## ProcessOptimizer
-        
-        ProcessOptimizer is a fork of scikit-optimize. ProcessOptimizer will fundamentally function like scikit-optimize, 
-        yet developments are focussed on bringing improvements to help optimizing real world processes, like chemistry or baking.
-        For examples on use, checkout https://github.com/novonordisk-research/ProcessOptimizer/tree/develop/examples.
-        
-        ## Installation
-        
-        ProcessOptimizer can be installed using `pip install ProcessOptimizer`
-        The repository and examples can be found at https://github.com/novonordisk-research/ProcessOptimizer
-        ProcessOptimizer can also be installed by running `pip install -e .` in top directory of the cloned repository.
-        
-        ## How does it work?
-        
-        This package is intended for real world process optimization problems of black-box functions. This could e.g. be some complex chemical reaction where no reliable analytical model mapping input variables to the output is readily available. <br/>
-        Bayesian optimization is a great tool for optimizing black-box functions where the input space has many dimensions and the function is expensive to evaluate in terms of time and/or resources.<br/>
-        **Notice that this tool is designed to solve minimization problems.** It is therefore important to define the scoring function such that it turns into a minimization problem. <br/>
-        Below is an illustrative example of minimization of the Booth function in 2 dimensions using the `ProcessOptimizer` package. Notice that in real world applications the function would be black box (and typically the input space would have more than 2 dimensions). However, it would still be possible to evaluate the function given a set of input values and thus use the same framework for optimization. <br/>
-        The Booth function is a 2-dimensional function defined by [Booth Function (sfu.ca)](https://www.sfu.ca/~ssurjano/booth.html). In this example uniformly distributed random noise between 0-5% of the function value is added using `np.random`.
-        ```python
-        def Booth(x0, x1):
-            return ((x0 + 2 * x1 - 7)**2 + (2 * x0 + x1 - 5)**2) * (1 + 0.05 * np.random.rand())
-        ```
-        Below is an image of the Booth function on the square <img src="https://render.githubusercontent.com/render/math?math=x_i \in \left[ 0,5 \right]"> for i=0,1.
-        
-        
-        ![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Booth_function.png)
-        
-        Suppose you are given the task of minimizing the function on the domain only using empirical observations and without any analytical function. <br/>
-        Working with the ProcessOptimizer package you simply define the `Space` and create an `Optimizer` object.<br/>
-        The `Space` object takes a list of dimensions which can either be `Real`, `Integer` or `Categorical`. `Real` dimensions are defined by the maximum and minimum values.<br/>
-        The `Optimizer` object initialized below uses GP (Gaussian Process). This means that after each step a Gaussian Process is fitted to the observations, which is used as a posterior distribution. Combined with an acquisition function the next point that should be explored can be determined. Notice that this process only takes place once n_initial_points of initial data has been aqcuired. In this case `LHS = True` (latin hypercube sampling) has been used as the initial sampling strategy for the first 6 points.
-        ```python
-        SPACE = Space([Real(0,5), Real(0,5)])   
-        
-        opt = Optimizer(SPACE, base_estimator = "GP", n_initial_points = 6, lhs = True)
-        ```
-        The optimizer can now be used in steps by calling the `.ask()` function, evaluating the function at the given point and use `.tell()` the `Optimizer` the result. In practise it would work like this. First ask the optimizer for the next point to perform an experiment:
-        ```python
-        opt.ask()
-        >>> [3.75, 3.75]
-        ```
-        Now go to the laboratory or wherever the experiment can be performed and use the values above. In this example the experiment can simply be performed by evaluating the Booth function using the values above:
-        ```python
-        Booth(3.75, 3.75)
-        >>> 59.313996676981354
-        ```
-        When a result has been obtained the user needs to tell the output to the `Optimizer`. This is done using the `.tell()` function:
-        ```python
-        res = opt.tell([3.75, 3.75], 59.313996676981354)
-        ```
-        The `res` object returned by tell contains a model of the Gaussian Process predicted mean. This model can be plotted using `plot_objective(res)`. Below is a gif of how the Gaussian Process predicted mean evolves after the first 6 initial points and until 20 points have been sampled in total. The orange dots visualise each evaluation of the function and the red dot shows the position of the expected minimum. In the diagonal of the figure dependence plots are shown. These show how the function depend on each input variable with other input variables kept constant at the expected minimum.
-        
-        <img src="https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/BO_GIF.gif" width="500">
-        
-         
-        Notice that this is an optimization tool and not a modelling tool. This means that the optimizer finds an approximate solution for the global minimum quickly however it does not guarantee that the Gaussian Process predicted mean is an accurate model on the entire domain.<br/>
-        
-        The best observation against the number of observations can be plotted with `plot_convergence(res)`:
-         
-        ![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Convergence_plot.png)
-        
-        ## Citation
-        
-        If you use the package in relation to a citation, please cite: https://doi.org/10.5281/zenodo.5155295.<br>
-        Please also cite the underlaying package (scikit-optimize).
-        
-        ## Contributions
-        
-        Feel free to play around with algorithm. Should you encounter errors while using ProcessOptimizer, please report them
-        at https://github.com/novonordisk-research/ProcessOptimizer/issues. <br>
-        To help solve the issues, please: <br>
-        
-        - Provide minimal amount of code to reproduce the error
-        - State versions of ProcesOptimizer, sklearn, numpy, ...
-        - Describe the expected behavior of the code <br>
-        
-        If you would like to contribute by making anything from documentation to feature-additions, THANK YOU. Please open a pull request 
-        marked as *WIP* as early as possible and describe the issue you seek to solve and outline your planned solution. <br>
-        Pull requests to the develop branch will be automatically tested using pytest and flake8. We'll be happy to help solving potential
-        issues that could arise here.
-        
-        ## Related work
-        
-        We are currently building a GUI to offer the power of Bayesian Process Optimization to non-coders. Stay tuned. (Sneak-peak at https://www.browniebee.dk/uk/)
-        
-        ## PyPi
-        
-        If you have not packaged before check out https://packaging.python.org/tutorials/packaging-projects/
-        To upload a new version to PyPi do the following in the root folder of the project:
-        
-        - In terminal run the command "pytest" and make sure there are no errors
-        - Change version number in setup.py
-        - Change version number in ProcessOptimizer/\_\_init\_\_.py
-        - Remember to `pip install twine` if running in a new virtual env
-        - Run `python setup.py sdist bdist_wheel`
-        - Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: bokeh
 Provides-Extra: browniebee
+License-File: LICENSE.md
+License-File: AUTHORS_scikit_optimize.md
+
+<div align="center">
+<pre>
+  _____                              ____        _   _           _              
+ |  __ \                            / __ \      | | (_)         (_)             
+ | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
+ |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
+ | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
+ |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|   
+                                          | |                                   
+                                          |_|                                   
+</pre>
+<a href="https://badge.fury.io/py/ProcessOptimizer"><img src="https://badge.fury.io/py/ProcessOptimizer.svg" alt="PyPI version" height="18"></a>
+<a href="https://github.com/novonordisk-research/ProcessOptimizer/actions"><img src="https://github.com/novonordisk-research/ProcessOptimizer/workflows/Python%20package/badge.svg" alt="Tests" height="18"></a>
+<a href="https://www.python.org/"><img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3" /></a>
+<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10-blue" alt="Runs on" /></a>
+<a href="https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/LICENSE.md"><img src="https://img.shields.io/pypi/l/ProcessOptimizer" alt="PyPI - License" /></a>
+<a href="https://scikit-optimize.github.io/stable/"><img src="https://img.shields.io/badge/BuildOn-Scikit--Optimize-brightgreen" alt="Scikit-Optimize" /></a>
+<a href="https://doi.org/10.5281/zenodo.5155295"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.5155295.svg" alt="DOI"></a>
+
+[![Downloads](https://static.pepy.tech/personalized-badge/processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)](https://pepy.tech/project/processoptimizer)
+</div>
+
+----------
+This readme.md is work in progress
+
+## Table of Contents
+ * [ProcessOptimizer](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#processoptimizer)
+ * [Installation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#installation)
+ * [How does it work?](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#how-does-it-work?)
+ * [Citation](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#Citation)
+ * [Contributions](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#contributions)
+ * [Related work](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#related-work)
+ * [PyPi](https://github.com/novonordisk-research/ProcessOptimizer/blob/develop/README.md#pypi)
+ 
+
+## ProcessOptimizer
+
+ProcessOptimizer is a fork of scikit-optimize. ProcessOptimizer will fundamentally function like scikit-optimize, 
+yet developments are focussed on bringing improvements to help optimizing real world processes, like chemistry or baking.
+For examples on use, checkout https://github.com/novonordisk-research/ProcessOptimizer/tree/develop/examples.
+
+## Installation
+
+ProcessOptimizer can be installed using `pip install ProcessOptimizer`
+The repository and examples can be found at https://github.com/novonordisk-research/ProcessOptimizer
+ProcessOptimizer can also be installed by running `pip install -e .` in top directory of the cloned repository.
+
+## How does it work?
+
+This package is intended for real world process optimization problems of black-box functions. This could e.g. be some complex chemical reaction where no reliable analytical model mapping input variables to the output is readily available. <br/>
+Bayesian optimization is a great tool for optimizing black-box functions where the input space has many dimensions and the function is expensive to evaluate in terms of time and/or resources.<br/>
+**Notice that this tool is designed to solve minimization problems.** It is therefore important to define the scoring function such that it turns into a minimization problem. <br/>
+Below is an illustrative example of minimization of the Booth function in 2 dimensions using the `ProcessOptimizer` package. Notice that in real world applications the function would be black box (and typically the input space would have more than 2 dimensions). However, it would still be possible to evaluate the function given a set of input values and thus use the same framework for optimization. <br/>
+The Booth function is a 2-dimensional function defined by [Booth Function (sfu.ca)](https://www.sfu.ca/~ssurjano/booth.html). In this example uniformly distributed random noise between 0-5% of the function value is added using `np.random`.
+```python
+def Booth(x0, x1):
+    return ((x0 + 2 * x1 - 7)**2 + (2 * x0 + x1 - 5)**2) * (1 + 0.05 * np.random.rand())
+```
+Below is an image of the Booth function on the square <img src="https://render.githubusercontent.com/render/math?math=x_i \in \left[ 0,5 \right]"> for i=0,1.
+
+
+![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Booth_function.png)
+
+Suppose you are given the task of minimizing the function on the domain only using empirical observations and without any analytical function. <br/>
+Working with the ProcessOptimizer package you simply define the `Space` and create an `Optimizer` object.<br/>
+The `Space` object takes a list of dimensions which can either be `Real`, `Integer` or `Categorical`. `Real` dimensions are defined by the maximum and minimum values.<br/>
+The `Optimizer` object initialized below uses GP (Gaussian Process). This means that after each step a Gaussian Process is fitted to the observations, which is used as a posterior distribution. Combined with an acquisition function the next point that should be explored can be determined. Notice that this process only takes place once n_initial_points of initial data has been aqcuired. In this case `LHS = True` (latin hypercube sampling) has been used as the initial sampling strategy for the first 6 points.
+```python
+SPACE = Space([Real(0,5), Real(0,5)])   
+
+opt = Optimizer(SPACE, base_estimator = "GP", n_initial_points = 6, lhs = True)
+```
+The optimizer can now be used in steps by calling the `.ask()` function, evaluating the function at the given point and use `.tell()` the `Optimizer` the result. In practise it would work like this. First ask the optimizer for the next point to perform an experiment:
+```python
+opt.ask()
+>>> [3.75, 3.75]
+```
+Now go to the laboratory or wherever the experiment can be performed and use the values above. In this example the experiment can simply be performed by evaluating the Booth function using the values above:
+```python
+Booth(3.75, 3.75)
+>>> 59.313996676981354
+```
+When a result has been obtained the user needs to tell the output to the `Optimizer`. This is done using the `.tell()` function:
+```python
+res = opt.tell([3.75, 3.75], 59.313996676981354)
+```
+The `res` object returned by tell contains a model of the Gaussian Process predicted mean. This model can be plotted using `plot_objective(res)`. Below is a gif of how the Gaussian Process predicted mean evolves after the first 6 initial points and until 20 points have been sampled in total. The orange dots visualise each evaluation of the function and the red dot shows the position of the expected minimum. In the diagonal of the figure dependence plots are shown. These show how the function depend on each input variable with other input variables kept constant at the expected minimum.
+
+<img src="https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/BO_GIF.gif" width="500">
+
+ 
+Notice that this is an optimization tool and not a modelling tool. This means that the optimizer finds an approximate solution for the global minimum quickly however it does not guarantee that the Gaussian Process predicted mean is an accurate model on the entire domain.<br/>
+
+The best observation against the number of observations can be plotted with `plot_convergence(res)`:
+ 
+![BayesianOptimization in action](https://raw.githubusercontent.com/novonordisk-research/ProcessOptimizer/a6a59e5aee58d2737feabe7c3fba86c58112e43a/examples/Convergence_plot.png)
+
+## Citation
+
+If you use the package in relation to a citation, please cite: https://doi.org/10.5281/zenodo.5155295.<br>
+Please also cite the underlaying package (scikit-optimize).
+
+## Contributions
+
+Feel free to play around with algorithm. Should you encounter errors while using ProcessOptimizer, please report them
+at https://github.com/novonordisk-research/ProcessOptimizer/issues. <br>
+To help solve the issues, please: <br>
+
+- Provide minimal amount of code to reproduce the error
+- State versions of ProcesOptimizer, sklearn, numpy, ...
+- Describe the expected behavior of the code <br>
+
+If you would like to contribute by making anything from documentation to feature-additions, THANK YOU. Please open a pull request 
+marked as *WIP* as early as possible and describe the issue you seek to solve and outline your planned solution. <br>
+Pull requests to the develop branch will be automatically tested using pytest and flake8. We'll be happy to help solving potential
+issues that could arise here.
+
+## Related work
+
+We are currently building a GUI to offer the power of Bayesian Process Optimization to non-coders. Stay tuned. (Sneak-peak at https://www.browniebee.dk/uk/)
+
+## PyPi
+
+If you have not packaged before check out https://packaging.python.org/tutorials/packaging-projects/
+To upload a new version to PyPi do the following in the root folder of the project:
+
+- In terminal run the command "pytest" and make sure there are no errors
+- Change version number in setup.py
+- Change version number in ProcessOptimizer/\_\_init\_\_.py
+- Remember to `pip install twine` if running in a new virtual env. (You might also have to `pip install wheel`)
+- Run `python setup.py sdist bdist_wheel`
+- Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
```

#### html2text {}

```diff
@@ -1,26 +1,28 @@
-Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.0 Summary: Sequential
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.1 Summary: Sequential
 model-based optimization toolbox (forked from scikit-optimize) Home-page:
 https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
-Research & Early Development License: BSD Description:
-            _____                              ____        _   _           _
+Research & Early Development License: BSD Description-Content-Type: text/
+markdown Provides-Extra: bokeh Provides-Extra: browniebee License-File:
+LICENSE.md License-File: AUTHORS_scikit_optimize.md
+        _____                              ____        _   _           _
 
-           |  __ \                            / __ \      | | (_)         (_)
+       |  __ \                            / __ \      | | (_)         (_)
 
-           | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _
-                                 _______ _ __
-         |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  /
-                                   _ \ '__|
-         | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /
-                                   __/ |
-           |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/
-                                 ___\___|_|
-                                                               | |
+ | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __
 
-                                                               |_|
+   |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \
+                                     '__|
+  | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |
+
+  |_|   |_|  \___/ \___\___||___/___/\____/| .__/ \__|_|_| |_| |_|_/___\___|_|
+
+                                                           | |
+
+                                                           |_|
 [PyPI_version] [Tests] [built_with_Python3] [Runs_on] [PyPI_-_License] [Scikit-
   Optimize] [DOI] [![Downloads](https://static.pepy.tech/personalized-badge/
 processoptimizer?period=total&units=international_system&left_color=brightgreen&right_color=orange&left_text=Downloads)]
                  (https://pepy.tech/project/processoptimizer)
 ---------- This readme.md is work in progress ## Table of Contents *
 [ProcessOptimizer](https://github.com/novonordisk-research/ProcessOptimizer/
 blob/develop/README.md#processoptimizer) * [Installation](https://github.com/
@@ -130,11 +132,10 @@
 Bayesian Process Optimization to non-coders. Stay tuned. (Sneak-peak at https:/
 /www.browniebee.dk/uk/) ## PyPi If you have not packaged before check out
 https://packaging.python.org/tutorials/packaging-projects/ To upload a new
 version to PyPi do the following in the root folder of the project: - In
 terminal run the command "pytest" and make sure there are no errors - Change
 version number in setup.py - Change version number in ProcessOptimizer/
 \_\_init\_\_.py - Remember to `pip install twine` if running in a new virtual
-env - Run `python setup.py sdist bdist_wheel` - Run `python -m twine upload
-dist/*` (make sure that /dist only contains relevant version) Platform: UNKNOWN
-Description-Content-Type: text/markdown Provides-Extra: bokeh Provides-Extra:
-browniebee
+env. (You might also have to `pip install wheel`) - Run `python setup.py sdist
+bdist_wheel` - Run `python -m twine upload dist/*` (make sure that /dist only
+contains relevant version)
```

### Comparing `ProcessOptimizer-0.8.0/ProcessOptimizer.egg-info/SOURCES.txt` & `ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+AUTHORS_scikit_optimize.md
+LICENSE.md
 README.md
 setup.py
 ProcessOptimizer/__init__.py
 ProcessOptimizer/acquisition.py
 ProcessOptimizer/bokeh_plot.py
 ProcessOptimizer/callbacks.py
 ProcessOptimizer/plots.py
```

### Comparing `ProcessOptimizer-0.8.0/README.md` & `ProcessOptimizer-0.8.1/ProcessOptimizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: ProcessOptimizer
+Version: 0.8.1
+Summary: Sequential model-based optimization toolbox     (forked from scikit-optimize)
+Home-page: https://github.com/novonordisk-research/ProcessOptimizer
+Author: Novo Nordisk, Research & Early Development
+License: BSD
+Description-Content-Type: text/markdown
+Provides-Extra: bokeh
+Provides-Extra: browniebee
+License-File: LICENSE.md
+License-File: AUTHORS_scikit_optimize.md
+
 <div align="center">
 <pre>
   _____                              ____        _   _           _              
  |  __ \                            / __ \      | | (_)         (_)             
  | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __ 
  |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \ '__|
  | |   | | | (_) | (_|  __/\__ \__ \ |__| | |_) | |_| | | | | | | |/ /  __/ |   
@@ -123,10 +136,10 @@
 
 If you have not packaged before check out https://packaging.python.org/tutorials/packaging-projects/
 To upload a new version to PyPi do the following in the root folder of the project:
 
 - In terminal run the command "pytest" and make sure there are no errors
 - Change version number in setup.py
 - Change version number in ProcessOptimizer/\_\_init\_\_.py
-- Remember to `pip install twine` if running in a new virtual env
+- Remember to `pip install twine` if running in a new virtual env. (You might also have to `pip install wheel`)
 - Run `python setup.py sdist bdist_wheel`
 - Run `python -m twine upload dist/*` (make sure that /dist only contains relevant version)
```

#### html2text {}

```diff
@@ -1,7 +1,13 @@
+Metadata-Version: 2.1 Name: ProcessOptimizer Version: 0.8.1 Summary: Sequential
+model-based optimization toolbox (forked from scikit-optimize) Home-page:
+https://github.com/novonordisk-research/ProcessOptimizer Author: Novo Nordisk,
+Research & Early Development License: BSD Description-Content-Type: text/
+markdown Provides-Extra: bokeh Provides-Extra: browniebee License-File:
+LICENSE.md License-File: AUTHORS_scikit_optimize.md
         _____                              ____        _   _           _
 
        |  __ \                            / __ \      | | (_)         (_)
 
  | |__) | __ ___   ___ ___  ___ ___| |  | |_ __ | |_ _ _ __ ___  _ _______ _ __
 
    |  ___/ '__/ _ \ / __/ _ \/ __/ __| |  | | '_ \| __| | '_ ` _ \| |_  / _ \
@@ -126,9 +132,10 @@
 Bayesian Process Optimization to non-coders. Stay tuned. (Sneak-peak at https:/
 /www.browniebee.dk/uk/) ## PyPi If you have not packaged before check out
 https://packaging.python.org/tutorials/packaging-projects/ To upload a new
 version to PyPi do the following in the root folder of the project: - In
 terminal run the command "pytest" and make sure there are no errors - Change
 version number in setup.py - Change version number in ProcessOptimizer/
 \_\_init\_\_.py - Remember to `pip install twine` if running in a new virtual
-env - Run `python setup.py sdist bdist_wheel` - Run `python -m twine upload
-dist/*` (make sure that /dist only contains relevant version)
+env. (You might also have to `pip install wheel`) - Run `python setup.py sdist
+bdist_wheel` - Run `python -m twine upload dist/*` (make sure that /dist only
+contains relevant version)
```

### Comparing `ProcessOptimizer-0.8.0/setup.py` & `ProcessOptimizer-0.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='ProcessOptimizer',
-      version='0.8.0',
+      version='0.8.1',
       description='Sequential model-based optimization toolbox \
     (forked from scikit-optimize)',
       url='https://github.com/novonordisk-research/ProcessOptimizer',
       license='BSD',
       author='Novo Nordisk, Research & Early Development',
       packages=[
           'ProcessOptimizer',
```

