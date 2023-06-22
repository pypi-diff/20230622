# Comparing `tmp/gama-22.0.0.tar.gz` & `tmp/gama-23.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gama-22.0.0.tar", last modified: Fri Sep 16 08:25:59 2022, max compression
+gzip compressed data, was "gama-23.0.0.tar", last modified: Thu Jun 22 20:19:51 2023, max compression
```

## Comparing `gama-22.0.0.tar` & `gama-23.0.0.tar`

### file list

```diff
@@ -1,91 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.009049 gama-22.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)    11345 2022-09-16 08:25:45.000000 gama-22.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5241 2022-09-16 08:25:59.009049 gama-22.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4810 2022-09-16 08:25:45.000000 gama-22.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.001049 gama-22.0.0/gama/
--rw-r--r--   0 runner    (1001) docker     (121)     5416 2022-09-16 08:25:45.000000 gama-22.0.0/gama/GamaClassifier.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-09-16 08:25:45.000000 gama-22.0.0/gama/GamaRegressor.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-16 08:25:45.000000 gama-22.0.0/gama/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-09-16 08:25:45.000000 gama-22.0.0/gama/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.005049 gama-22.0.0/gama/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:45.000000 gama-22.0.0/gama/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4751 2022-09-16 08:25:45.000000 gama-22.0.0/gama/configuration/classification.py
--rw-r--r--   0 runner    (1001) docker     (121)     5995 2022-09-16 08:25:45.000000 gama-22.0.0/gama/configuration/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-09-16 08:25:45.000000 gama-22.0.0/gama/configuration/regression.py
--rw-r--r--   0 runner    (1001) docker     (121)     4873 2022-09-16 08:25:45.000000 gama-22.0.0/gama/configuration/testconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.005049 gama-22.0.0/gama/dashboard/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4083 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.005049 gama-22.0.0/gama/dashboard/components/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/components/cli_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/components/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/components/input_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.005049 gama-22.0.0/gama/dashboard/pages/
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8544 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/pages/analysispage.py
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/pages/base_page.py
--rw-r--r--   0 runner    (1001) docker     (121)    12519 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/pages/homepage.py
--rw-r--r--   0 runner    (1001) docker     (121)     8469 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/pages/runningpage.py
--rw-r--r--   0 runner    (1001) docker     (121)    12007 2022-09-16 08:25:45.000000 gama-22.0.0/gama/dashboard/plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3669 2022-09-16 08:25:45.000000 gama-22.0.0/gama/data_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     6843 2022-09-16 08:25:45.000000 gama-22.0.0/gama/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (121)    29326 2022-09-16 08:25:45.000000 gama-22.0.0/gama/gama.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.005049 gama-22.0.0/gama/genetic_programming/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.005049 gama-22.0.0/gama/genetic_programming/compilers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/compilers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7896 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/compilers/scikitlearn.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.009049 gama-22.0.0/gama/genetic_programming/components/
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/components/fitness.py
--rw-r--r--   0 runner    (1001) docker     (121)     6695 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/components/individual.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/components/primitive.py
--rw-r--r--   0 runner    (1001) docker     (121)     5247 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/components/primitive_node.py
--rw-r--r--   0 runner    (1001) docker     (121)      920 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/components/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)     5535 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/crossover.py
--rw-r--r--   0 runner    (1001) docker     (121)     6094 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/mutation.py
--rw-r--r--   0 runner    (1001) docker     (121)     5999 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/nsga2.py
--rw-r--r--   0 runner    (1001) docker     (121)     1584 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)     3968 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/operator_set.py
--rw-r--r--   0 runner    (1001) docker     (121)     1451 2022-09-16 08:25:45.000000 gama-22.0.0/gama/genetic_programming/selection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.009049 gama-22.0.0/gama/logging/
--rw-r--r--   0 runner    (1001) docker     (121)     5417 2022-09-16 08:25:45.000000 gama-22.0.0/gama/logging/GamaReport.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-09-16 08:25:45.000000 gama-22.0.0/gama/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3073 2022-09-16 08:25:45.000000 gama-22.0.0/gama/logging/evaluation_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      831 2022-09-16 08:25:45.000000 gama-22.0.0/gama/logging/utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.009049 gama-22.0.0/gama/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-09-16 08:25:45.000000 gama-22.0.0/gama/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3573 2022-09-16 08:25:46.000000 gama-22.0.0/gama/postprocessing/base_post_processing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1687 2022-09-16 08:25:46.000000 gama-22.0.0/gama/postprocessing/best_fit.py
--rw-r--r--   0 runner    (1001) docker     (121)    20762 2022-09-16 08:25:46.000000 gama-22.0.0/gama/postprocessing/ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.009049 gama-22.0.0/gama/search_methods/
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-09-16 08:25:46.000000 gama-22.0.0/gama/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9100 2022-09-16 08:25:46.000000 gama-22.0.0/gama/search_methods/asha.py
--rw-r--r--   0 runner    (1001) docker     (121)     5985 2022-09-16 08:25:46.000000 gama-22.0.0/gama/search_methods/async_ea.py
--rw-r--r--   0 runner    (1001) docker     (121)     4155 2022-09-16 08:25:46.000000 gama-22.0.0/gama/search_methods/base_search.py
--rw-r--r--   0 runner    (1001) docker     (121)     2166 2022-09-16 08:25:46.000000 gama-22.0.0/gama/search_methods/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.009049 gama-22.0.0/gama/utilities/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5702 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    10553 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/evaluation_library.py
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/export.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.009049 gama-22.0.0/gama/utilities/generic/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14857 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/generic/async_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (121)     3466 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/generic/paretofront.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/generic/stopwatch.py
--rw-r--r--   0 runner    (1001) docker     (121)     4159 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/generic/timekeeper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2753 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-09-16 08:25:46.000000 gama-22.0.0/gama/utilities/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-16 08:25:59.001049 gama-22.0.0/gama.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5241 2022-09-16 08:25:58.000000 gama-22.0.0/gama.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2022-09-16 08:25:58.000000 gama-22.0.0/gama.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-16 08:25:58.000000 gama-22.0.0/gama.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-16 08:25:58.000000 gama-22.0.0/gama.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-09-16 08:25:58.000000 gama-22.0.0/gama.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-16 08:25:58.000000 gama-22.0.0/gama.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-09-16 08:25:46.000000 gama-22.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-16 08:25:59.009049 gama-22.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-09-16 08:25:46.000000 gama-22.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.394341 gama-23.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-22 20:19:41.000000 gama-23.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-22 20:19:51.394341 gama-23.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-06-22 20:19:41.000000 gama-23.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.386341 gama-23.0.0/gama/
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-06-22 20:19:41.000000 gama-23.0.0/gama/GamaClassifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-22 20:19:41.000000 gama-23.0.0/gama/GamaRegressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 20:19:41.000000 gama-23.0.0/gama/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-22 20:19:41.000000 gama-23.0.0/gama/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.386341 gama-23.0.0/gama/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:41.000000 gama-23.0.0/gama/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-06-22 20:19:41.000000 gama-23.0.0/gama/configuration/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-22 20:19:41.000000 gama-23.0.0/gama/configuration/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-22 20:19:41.000000 gama-23.0.0/gama/configuration/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-22 20:19:41.000000 gama-23.0.0/gama/configuration/testconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-22 20:19:41.000000 gama-23.0.0/gama/data_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-22 20:19:41.000000 gama-23.0.0/gama/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30418 2023-06-22 20:19:41.000000 gama-23.0.0/gama/gama.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.390341 gama-23.0.0/gama/genetic_programming/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.390341 gama-23.0.0/gama/genetic_programming/compilers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/compilers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7791 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/compilers/scikitlearn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.390341 gama-23.0.0/gama/genetic_programming/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/components/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/components/individual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/components/primitive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/components/primitive_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/components/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/crossover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/operator_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-22 20:19:41.000000 gama-23.0.0/gama/genetic_programming/selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.390341 gama-23.0.0/gama/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-06-22 20:19:41.000000 gama-23.0.0/gama/logging/GamaReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-06-22 20:19:41.000000 gama-23.0.0/gama/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-22 20:19:41.000000 gama-23.0.0/gama/logging/evaluation_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-22 20:19:41.000000 gama-23.0.0/gama/logging/utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.390341 gama-23.0.0/gama/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-22 20:19:41.000000 gama-23.0.0/gama/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-06-22 20:19:41.000000 gama-23.0.0/gama/postprocessing/base_post_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-22 20:19:41.000000 gama-23.0.0/gama/postprocessing/best_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-06-22 20:19:41.000000 gama-23.0.0/gama/postprocessing/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.390341 gama-23.0.0/gama/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-22 20:19:41.000000 gama-23.0.0/gama/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-06-22 20:19:41.000000 gama-23.0.0/gama/search_methods/asha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5985 2023-06-22 20:19:41.000000 gama-23.0.0/gama/search_methods/async_ea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-06-22 20:19:41.000000 gama-23.0.0/gama/search_methods/base_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-22 20:19:41.000000 gama-23.0.0/gama/search_methods/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.394341 gama-23.0.0/gama/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5656 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10413 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/evaluation_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.394341 gama-23.0.0/gama/utilities/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14836 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/generic/async_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/generic/paretofront.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/generic/stopwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/generic/timekeeper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-22 20:19:41.000000 gama-23.0.0/gama/utilities/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:19:51.386341 gama-23.0.0/gama.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-22 20:19:51.000000 gama-23.0.0/gama.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-22 20:19:51.000000 gama-23.0.0/gama.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:19:51.000000 gama-23.0.0/gama.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 20:19:51.000000 gama-23.0.0/gama.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-22 20:19:51.000000 gama-23.0.0/gama.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 20:19:51.000000 gama-23.0.0/gama.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-22 20:19:41.000000 gama-23.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:19:51.394341 gama-23.0.0/setup.cfg
```

### Comparing `gama-22.0.0/LICENSE` & `gama-23.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/PKG-INFO` & `gama-23.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: gama
-Version: 22.0.0
+Version: 23.0.0
 Summary: A package for automated machine learning based on scikit-learn.
 Author-email: Pieter Gijsbers <p.gijsbers@tue.nl>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
-Provides-Extra: vis
 License-File: LICENSE
 
 ![GAMA logo](https://github.com/openml-labs/gama/blob/master/images/logos/Logo-With-Grey-Name-Transparent.png)
 
 **G**eneral **A**utomated **M**achine learning **A**ssistant  
 An automated machine learning tool based on genetic programming.  
 Make sure to check out the [documentation](https://openml-labs.github.io/gama/).
@@ -35,15 +34,15 @@
 
 In addition to its general use AutoML functionality, GAMA aims to serve AutoML researchers as well.
 During the optimization process, GAMA keeps an extensive log of progress made.
 Using this log, insight can be obtained on the behaviour of the search procedure.
 For example, it can produce a graph that shows pipeline fitness over time:
 ![graph of fitness over time](https://github.com/openml-lab/gama/blob/master/docs/source/technical_guide/images/viz.gif)
 
-For more examples and information on the visualization, see [the technical guide](https://openml-labs.github.io/gama/master/user_guide/index.html#dashboard).
+*Note: we temporarily disabled support for the GAMA Dashboard, we will add out-of-the-box visualization again later this year.* 
 
 ## Installing GAMA
 
 You can install GAMA with pip: `pip install gama`
 
 ## Minimal Example
 
@@ -96,7 +95,10 @@
 publisher="Springer International Publishing",
 address="Cham",
 pages="560--564",
 abstract="The General Automated Machine learning Assistant (GAMA) is a modular AutoML system developed to empower users to track and control how AutoML algorithms search for optimal machine learning pipelines, and facilitate AutoML research itself. In contrast to current, often black-box systems, GAMA allows users to plug in different AutoML and post-processing techniques, logs and visualizes the search process, and supports easy benchmarking. It currently features three AutoML search algorithms, two model post-processing steps, and is designed to allow for more components to be added.",
 isbn="978-3-030-67670-4"
 }
 ```
+
+## License
+The contents of this repository is under an [Apache-2.0 License](https://github.com/openml-labs/gama/blob/master/LICENSE).
```

### Comparing `gama-22.0.0/README.md` & `gama-23.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 In addition to its general use AutoML functionality, GAMA aims to serve AutoML researchers as well.
 During the optimization process, GAMA keeps an extensive log of progress made.
 Using this log, insight can be obtained on the behaviour of the search procedure.
 For example, it can produce a graph that shows pipeline fitness over time:
 ![graph of fitness over time](https://github.com/openml-lab/gama/blob/master/docs/source/technical_guide/images/viz.gif)
 
-For more examples and information on the visualization, see [the technical guide](https://openml-labs.github.io/gama/master/user_guide/index.html#dashboard).
+*Note: we temporarily disabled support for the GAMA Dashboard, we will add out-of-the-box visualization again later this year.* 
 
 ## Installing GAMA
 
 You can install GAMA with pip: `pip install gama`
 
 ## Minimal Example
 
@@ -81,7 +81,10 @@
 publisher="Springer International Publishing",
 address="Cham",
 pages="560--564",
 abstract="The General Automated Machine learning Assistant (GAMA) is a modular AutoML system developed to empower users to track and control how AutoML algorithms search for optimal machine learning pipelines, and facilitate AutoML research itself. In contrast to current, often black-box systems, GAMA allows users to plug in different AutoML and post-processing techniques, logs and visualizes the search process, and supports easy benchmarking. It currently features three AutoML search algorithms, two model post-processing steps, and is designed to allow for more components to be added.",
 isbn="978-3-030-67670-4"
 }
 ```
+
+## License
+The contents of this repository is under an [Apache-2.0 License](https://github.com/openml-labs/gama/blob/master/LICENSE).
```

### Comparing `gama-22.0.0/gama/GamaClassifier.py` & `gama-23.0.0/gama/GamaClassifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 from gama.configuration.classification import clf_config
 from gama.utilities.metrics import scoring_to_metric
 
 
 class GamaClassifier(Gama):
     """Gama with adaptations for (multi-class) classification."""
 
-    def __init__(self, config=None, scoring="neg_log_loss", *args, **kwargs):
-        if not config:
+    def __init__(self, search_space=None, scoring="neg_log_loss", *args, **kwargs):
+        if not search_space:
             # Do this to avoid the whole dictionary being included in the documentation.
-            config = clf_config
+            search_space = clf_config
 
         self._metrics = scoring_to_metric(scoring)
         if any(metric.requires_probabilities for metric in self._metrics):
             # we don't want classifiers that do not have `predict_proba`,
             # because then we have to start doing one hot encodings of predictions etc.
-            config = {
+            search_space = {
                 alg: hp
-                for (alg, hp) in config.items()
+                for (alg, hp) in search_space.items()
                 if not (
                     inspect.isclass(alg)
                     and issubclass(alg, ClassifierMixin)
                     and not hasattr(alg(), "predict_proba")
                 )
             }
 
         self._label_encoder = None
-        super().__init__(*args, **kwargs, config=config, scoring=scoring)
+        super().__init__(*args, search_space=search_space, scoring=scoring, **kwargs)
 
     def _predict(self, x: pd.DataFrame):
         """Predict the target for input X.
 
         Parameters
         ----------
         x: pandas.DataFrame
@@ -123,15 +123,15 @@
         x = self._prepare_for_prediction(x)
         return self._predict_proba(x)
 
     def fit(self, x, y, *args, **kwargs):
         """Should use base class documentation."""
         y_ = y.squeeze() if isinstance(y, pd.DataFrame) else y
         self._label_encoder = LabelEncoder().fit(y_)
-        if any([isinstance(yi, str) for yi in y_]):
+        if any(isinstance(yi, str) for yi in y_):
             # If target values are `str` we encode them or scikit-learn will complain.
             y = self._label_encoder.transform(y_)
         self._evaluation_library.determine_sample_indices(stratify=y)
 
         # Add label information for classification to the scorer such that
         # the cross validator does not encounter unseen labels in smaller
         # data sets during pipeline evaluation.
```

### Comparing `gama-22.0.0/gama/GamaRegressor.py` & `gama-23.0.0/gama/GamaRegressor.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 from .gama import Gama
 from gama.configuration.regression import reg_config
 
 
 class GamaRegressor(Gama):
     """Gama with adaptations for regression."""
 
-    def __init__(self, config=None, scoring="neg_mean_squared_error", *args, **kwargs):
+    def __init__(
+        self, search_space=None, scoring="neg_mean_squared_error", *args, **kwargs
+    ):
         """ """
         # Empty docstring overwrites base __init__ doc string.
         # Prevents duplication of the __init__ doc string on the API page.
 
-        if not config:
-            config = reg_config
-        super().__init__(*args, **kwargs, config=config, scoring=scoring)
+        if not search_space:
+            search_space = reg_config
+        super().__init__(*args, search_space=search_space, scoring=scoring, **kwargs)
 
     def _predict(self, x: pd.DataFrame):
         """Predict the target for input X.
 
         Parameters
         ----------
         x: pandas.DataFrame
```

### Comparing `gama-22.0.0/gama/configuration/classification.py` & `gama-23.0.0/gama/configuration/classification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# sourcery skip: de-morgan
 import numpy as np
 
 from sklearn.naive_bayes import GaussianNB, BernoulliNB, MultinomialNB
 from sklearn.tree import DecisionTreeClassifier
 from sklearn.ensemble import (
     ExtraTreesClassifier,
     RandomForestClassifier,
@@ -104,15 +105,15 @@
         "tol": np.arange(0.0, 1.01, 0.05),
         "whiten": ["unit-variance"],
     },
     FeatureAgglomeration: {
         "linkage": ["ward", "complete", "average"],
         "affinity": ["euclidean", "l1", "l2", "manhattan", "cosine", "precomputed"],
         "param_check": [
-            lambda params: (not params["linkage"] == "ward")
+            lambda params: params["linkage"] != "ward"
             or params["affinity"] == "euclidean"
         ],
     },
     MaxAbsScaler: {},
     MinMaxScaler: {},
     Normalizer: {"norm": ["l1", "l2", "max"]},
     Nystroem: {
```

### Comparing `gama-22.0.0/gama/configuration/parser.py` & `gama-23.0.0/gama/configuration/parser.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/configuration/regression.py` & `gama-23.0.0/gama/configuration/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         "tol": np.arange(0.0, 1.01, 0.05),
         "whiten": ["unit-variance"],
     },
     FeatureAgglomeration: {
         "linkage": ["ward", "complete", "average"],
         "affinity": ["euclidean", "l1", "l2", "manhattan", "cosine", "precomputed"],
         "param_check": [
-            lambda params: (not params["linkage"] == "ward")
+            lambda params: params["linkage"] != "ward"
             or params["affinity"] == "euclidean"
         ],
     },
     MaxAbsScaler: {},
     MinMaxScaler: {},
     Normalizer: {"norm": ["l1", "l2", "max"]},
     Nystroem: {
```

### Comparing `gama-22.0.0/gama/configuration/testconfiguration.py` & `gama-23.0.0/gama/configuration/testconfiguration.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         "tol": np.arange(0.0, 1.01, 0.05),
         "whiten": ["unit-variance"],
     },
     FeatureAgglomeration: {
         "linkage": ["ward", "complete", "average"],
         "affinity": ["euclidean", "l1", "l2", "manhattan", "cosine", "precomputed"],
         "param_check": [
-            lambda params: (not params["linkage"] == "ward")
+            lambda params: params["linkage"] != "ward"
             or params["affinity"] == "euclidean"
         ],
     },
     MaxAbsScaler: {},
     MinMaxScaler: {},
     Normalizer: {"norm": ["l1", "l2", "max"]},
     Nystroem: {
```

### Comparing `gama-22.0.0/gama/data_formatting.py` & `gama-23.0.0/gama/data_formatting.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,19 +40,15 @@
     if not isinstance(y, (np.ndarray, pd.Series, pd.DataFrame)):
         raise TypeError("y must be np.ndarray, pd.Series or pd.DataFrame.")
     if y_type not in [pd.Series, pd.DataFrame]:
         raise ValueError(f"`y_type` must be pd.Series or pd.DataFrame but is {y_type}.")
 
     if isinstance(y, np.ndarray) and y.ndim == 2:
         # Either indicator matrix or should be a vector.
-        if y.shape[1] > 1:
-            y = np.argmax(y, axis=1)
-        else:
-            y = y.squeeze()
-
+        y = np.argmax(y, axis=1) if y.shape[1] > 1 else y.squeeze()
     if y_type == pd.Series:
         if isinstance(y, pd.DataFrame):
             y = y.squeeze()
         elif isinstance(y, np.ndarray):
             y = pd.Series(y)
     elif y_type == pd.DataFrame:
         if not isinstance(y, pd.DataFrame):
```

### Comparing `gama-22.0.0/gama/data_loading.py` & `gama-23.0.0/gama/data_loading.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/gama.py` & `gama-23.0.0/gama/gama.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,53 +77,55 @@
 
 
 class Gama(ABC):
     """Wrapper for the toolbox logic surrounding executing the AutoML pipeline."""
 
     def __init__(
         self,
+        search_space: Dict[Union[str, object], Any],
         scoring: Union[
             str, Metric, Iterable[str], Iterable[Metric]
         ] = "filled_in_by_child_class",
         regularize_length: bool = True,
         max_pipeline_length: Optional[int] = None,
-        config: Dict[Union[str, object], Any] = {},
         random_state: Optional[int] = None,
         max_total_time: int = 3600,
         max_eval_time: Optional[int] = None,
         n_jobs: Optional[int] = None,
         max_memory_mb: Optional[int] = None,
         verbosity: int = logging.WARNING,
-        search: BaseSearch = AsyncEA(),
-        post_processing: BasePostProcessing = BestFitPostProcessing(),
+        search: Optional[BaseSearch] = None,
+        post_processing: Optional[BasePostProcessing] = None,
         output_directory: Optional[str] = None,
         store: str = "logs",
+        config: None = None,
+        preset: str = "simple",
     ):
         """
 
         Parameters
         ----------
+        search_space: Dict
+            Specifies available components and their valid hyperparameter settings.
+            For more information, see :ref:`search_space_configuration`.
+
         scoring: str, Metric or Tuple
             Specifies the/all metric(s) to optimize towards.
             A string will be converted to Metric.
             A tuple must specify each metric with the same type (e.g. all str).
             See :ref:`Metrics` for built-in metrics.
 
         regularize_length: bool (default=True)
             If True, add pipeline length as an optimization metric.
             Short pipelines should then be preferred over long ones.
 
         max_pipeline_length: int, optional (default=None)
             If set, limit the maximum number of steps in any evaluated pipeline.
             Encoding and imputation are excluded.
 
-        config: Dict
-            Specifies available components and their valid hyperparameter settings.
-            For more information, see :ref:`search_space_configuration`.
-
         random_state:  int, optional (default=None)
             Seed for the random number generators used in the process.
             However, with `n_jobs > 1`,
             there will be randomization introduced by multi-processing.
             For reproducible results, set this and use `n_jobs=1`.
 
         max_total_time: positive int (default=3600)
@@ -144,48 +146,75 @@
             If not set, GAMA will use as much as it needs.
             GAMA is not guaranteed to respect this limit at all times,
             but it should never violate it for too long.
 
         verbosity: int (default=logging.WARNING)
             Sets the level of log messages to be automatically output to terminal.
 
-        search: BaseSearch (default=AsyncEA())
+        search: BaseSearch, optional
             Search method to use to find good pipelines. Should be instantiated.
+            Default depends on ``goal``.
 
-        post_processing: BasePostProcessing (default=BestFitPostProcessing())
+        post_processing: BasePostProcessing, optional
             Post-processing method to create a model after the search phase.
             Should be an instantiated subclass of BasePostProcessing.
+            Default depends on ``goal``.
 
         output_directory: str, optional (default=None)
             Directory to use to save GAMA output. This includes both intermediate
             results during search and logs.
             This directory must be empty or not exist.
             If set to None, generate a unique name ("gama_HEXCODE").
 
         store: str (default='logs')
             Determines which data is stored after each run:
              - 'nothing': keep nothing from this run
              - 'models': keep only cache with models and predictions
              - 'logs': keep only the logs
              - 'all': keep logs and cache with models and predictions
+
+        preset: str (default='simple')
+            Determines the steps of the AutoML pipeline when they are not
+            provided explicitly, based on the given goal.
+            One of:
+                - simple: Create a simple pipeline with good performance.
+                - performance: Try to get the best performing model.
         """
+        if config:
+            warnings.warn(
+                "Hyperparameter `config` is renamed to `search_space`. "
+                "Using `config` will lead to an error with `gama>=24`.",
+                FutureWarning,
+            )
+            search_space = config
+
+        if search is None:
+            search = AsyncEA()
+        if post_processing is None:
+            if preset == "simple":
+                post_processing = BestFitPostProcessing()
+            elif preset == "performance":
+                post_processing = EnsemblePostProcessing()
+            else:
+                raise ValueError(f"Unknown value for {preset=}'")
+
         if not output_directory:
             output_directory = f"gama_{str(uuid.uuid4())}"
         self.output_directory = os.path.abspath(os.path.expanduser(output_directory))
 
         if not os.path.exists(self.output_directory):
             os.mkdir(self.output_directory)
         elif len(os.listdir(self.output_directory)) > 0:
             raise ValueError(
                 f"""`output_directory` ('{self.output_directory}')
                  must be empty or non-existent."""
             )
 
         register_stream_log(verbosity)
-        if store in ["logs", "all"]:
+        if store in {"logs", "all"}:
             log_file = os.path.join(self.output_directory, "gama.log")
             log_handler = logging.FileHandler(log_file)
             log_handler.setLevel(logging.DEBUG)
             log_format = logging.Formatter("[%(asctime)s - %(name)s] %(message)s")
             log_handler.setFormatter(log_format)
             logging.getLogger("gama").addHandler(log_handler)
 
@@ -268,15 +297,15 @@
         else:
             # Don't keep memory-heavy evaluation meta-data (predictions, estimators)
             self._evaluation_library = EvaluationLibrary(m=0, cache=cache_directory)
         self.evaluation_completed(self._evaluation_library.save_evaluation)
         e = search.logger(os.path.join(self.output_directory, "evaluations.log"))
         self.evaluation_completed(e.log_evaluation)
 
-        self._pset, parameter_checks = pset_from_config(config)
+        self._pset, parameter_checks = pset_from_config(search_space)
 
         if DATA_TERMINAL not in self._pset:
             if max_pipeline_length is None:
                 log.info(
                     "Setting `max_pipeline_length` to 1 "
                     "because there are no preprocessing steps in the search space."
                 )
@@ -581,25 +610,25 @@
             self._post_processing.dynamic_defaults(self)
             self.model = self._post_processing.post_process(
                 self._x,
                 self._y,
                 self._time_manager.total_time_remaining,
                 best_individuals,
             )
-        if not self._store == "all":
+        if self._store != "all":
             to_clean = dict(nothing="all", logs="evaluations", models="logs")
             self.cleanup(to_clean[self._store])
         return self
 
     def _search_phase(
         self, warm_start: Optional[List[Individual]] = None, timeout: float = 1e6
     ) -> None:
         """Invoke the search algorithm, populate `final_pop`."""
         if warm_start:
-            if not all([isinstance(i, Individual) for i in warm_start]):
+            if not all(isinstance(i, Individual) for i in warm_start):
                 raise TypeError("`warm_start` must be a list of Individual.")
             pop = warm_start
         elif warm_start is None and len(self._final_pop) > 0:
             pop = self._final_pop
         else:
             pop = [self._operator_set.individual() for _ in range(50)]
```

### Comparing `gama-22.0.0/gama/genetic_programming/compilers/scikitlearn.py` & `gama-23.0.0/gama/genetic_programming/compilers/scikitlearn.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,23 +28,23 @@
         terminal.output: terminal.value for terminal in primitive_node._terminals
     }
     return primitive_node._primitive.identifier(**hyperparameters)
 
 
 def compile_individual(
     individual: Individual,
-    parameter_checks=None,
-    preprocessing_steps: Sequence[Tuple[str, TransformerMixin]] = None,
+    _parameter_checks=None,
+    preprocessing_steps: Optional[Sequence[Tuple[str, TransformerMixin]]] = None,
 ) -> Pipeline:
     steps = [
         (str(i), primitive_node_to_sklearn(primitive))
         for i, primitive in enumerate(individual.primitives)
     ]
     if preprocessing_steps:
-        steps = steps + list(reversed(preprocessing_steps))
+        steps += list(reversed(preprocessing_steps))
     return Pipeline(list(reversed(steps)))
 
 
 def object_is_valid_pipeline(o: object) -> bool:
     """Determines if object behaves like a scikit-learn pipeline."""
     return (
         o is not None
@@ -71,15 +71,15 @@
         prediction: np.ndarray if successful, None if not
         scores: tuple with one float per metric, each value is -inf on fail.
         estimators: list of fitted pipelines if successful, None if not
         error: None if successful, otherwise an Exception
     """
     if not object_is_valid_pipeline(pipeline):
         raise TypeError("Pipeline must not be None and requires fit, predict, steps.")
-    if not timeout > 0:
+    if timeout <= 0:
         raise ValueError(f"`timeout` must be greater than 0, is {timeout}.")
 
     prediction, estimators = None, None
     # default score for e.g. timeout or failure
     scores = tuple([float("-inf")] * len(metrics))
     is_classification = is_classifier(pipeline)
 
@@ -115,22 +115,22 @@
                 x,
                 y_train,
                 cv=splitter,
                 return_estimator=True,
                 scoring=dict([(m.name, m) for m in metrics]),
                 error_score="raise",
             )
-            scores = tuple([np.mean(result[f"test_{m.name}"]) for m in metrics])
+            scores = tuple(np.mean(result[f"test_{m.name}"]) for m in metrics)
             estimators = result["estimator"]
 
             splitter = (
                 splitter if isinstance(splitter, list) else splitter.split(x, y_train)
             )
-            for (estimator, (_, test)) in zip(estimators, splitter):
-                if any([m.requires_probabilities for m in metrics]):
+            for estimator, (_, test) in zip(estimators, splitter):
+                if any(m.requires_probabilities for m in metrics):
                     fold_pred = estimator.predict_proba(x.iloc[test, :])
                 else:
                     fold_pred = estimator.predict(x.iloc[test, :])
 
                 if prediction is None:
                     if fold_pred.ndim == 2:
                         prediction = np.empty(shape=(len(y_train), fold_pred.shape[1]))
@@ -147,20 +147,19 @@
             return prediction, scores, estimators, e
 
     if c_mgr.state == c_mgr.INTERRUPTED:
         # A TimeoutException was raised, but not by the context manager.
         # This indicates that the outer context manager (the ea) timed out.
         raise stopit.utils.TimeoutException()
 
-    if not c_mgr:
-        # For now we treat an eval timeout the same way as
-        # e.g. NaN exceptions and use the default score.
-        return prediction, scores, estimators, stopit.TimeoutException()
-
-    return prediction, tuple(scores), estimators, None
+    return (
+        (prediction, tuple(scores), estimators, None)
+        if c_mgr
+        else (prediction, scores, estimators, stopit.TimeoutException())
+    )
 
 
 def evaluate_individual(
     individual: Individual,
     evaluate_pipeline: Callable,
     timeout: float = 1e6,
     deadline: Optional[float] = None,
```

### Comparing `gama-22.0.0/gama/genetic_programming/components/__init__.py` & `gama-23.0.0/gama/genetic_programming/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/genetic_programming/components/individual.py` & `gama-23.0.0/gama/genetic_programming/components/individual.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
 
     def __init__(
         self, main_node: PrimitiveNode, to_pipeline: Optional[Callable] = None
     ):
         self.fitness: Optional[Fitness] = None
         self.main_node = main_node
-        self.meta: Dict[str, Any] = dict()
+        self.meta: Dict[str, Any] = {}
         self._id = uuid.uuid4()
         self._to_pipeline = to_pipeline
 
     def __eq__(self, other) -> bool:
         return isinstance(other, Individual) and other._id == self._id
 
     def __hash__(self) -> int:
@@ -85,23 +85,22 @@
         new_terminal: Terminal
             The new terminal to replace the old one with. Must share output type.
         """
         scan_position = 0
         for primitive in self.primitives:
             if scan_position + len(primitive._terminals) > position:
                 terminal_to_be_replaced = primitive._terminals[position - scan_position]
-                if terminal_to_be_replaced.identifier == new_terminal.identifier:
-                    primitive._terminals[position - scan_position] = new_terminal
-                    return
-                else:
+                if terminal_to_be_replaced.identifier != new_terminal.identifier:
                     raise ValueError(
                         f"New terminal does not share output type with the old."
                         f"Old: {terminal_to_be_replaced.identifier}"
                         f"New: {new_terminal.identifier}."
                     )
+                primitive._terminals[position - scan_position] = new_terminal
+                return
             else:
                 scan_position += len(primitive._terminals)
         if scan_position < position:
             raise ValueError(
                 f"Position {position} is out of range with {scan_position} terminals."
             )
```

### Comparing `gama-22.0.0/gama/genetic_programming/components/primitive_node.py` & `gama-23.0.0/gama/genetic_programming/components/primitive_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,18 @@
     def __str__(self) -> str:
         """Recursively stringify all primitive nodes (primitive and hyperparameters).
 
         Examples: - "GaussianNB(data)"
                   - "BernoulliNB(data, alpha=1.0)"
                   - "BernoulliNB(FastICA(data, tol=0.5), alpha=1.0)"
         """
-        if self._terminals:
-            terminal_str = ", ".join([repr(terminal) for terminal in self._terminals])
-            return f"{self._primitive}({self._data_node}, {terminal_str})"
-        else:
+        if not self._terminals:
             return f"{self._primitive}({self._data_node})"
+        terminal_str = ", ".join([repr(terminal) for terminal in self._terminals])
+        return f"{self._primitive}({self._data_node}, {terminal_str})"
 
     @property
     def str_nonrecursive(self) -> str:
         """Stringify primitive node with its hyperparameter configuration
 
         Examples: - "GaussianNB()"
                   - "BernoulliNB(alpha=1.0)"
```

### Comparing `gama-22.0.0/gama/genetic_programming/components/terminal.py` & `gama-23.0.0/gama/genetic_programming/components/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,10 +25,10 @@
         return f"{self.identifier}={format_hyperparameter_value(self.value)}"
 
 
 def format_hyperparameter_value(value: object) -> str:
     if isinstance(value, str):
         return f"'{value}'"  # Quoted
     elif callable(value) and hasattr(value, "__name__"):
-        return f"{value.__name__}"  # type: ignore
+        return f"{value.__name__}"
     else:
         return str(value)
```

### Comparing `gama-22.0.0/gama/genetic_programming/crossover.py` & `gama-23.0.0/gama/genetic_programming/crossover.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/genetic_programming/mutation.py` & `gama-23.0.0/gama/genetic_programming/mutation.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
 
     def terminal_replaceable(index_terminal):
         _, terminal = index_terminal
         return len(primitive_set[terminal.identifier]) > 1
 
     terminals = list(filter(terminal_replaceable, enumerate(individual.terminals)))
-    if len(terminals) == 0:
+    if not terminals:
         raise ValueError("Individual has no terminals suitable for mutation.")
 
     terminal_index, old = random.choice(terminals)
     candidates = filter(lambda t: t.value != old.value, primitive_set[old.identifier])
 
     new_terminal = random.choice(list(candidates))
     individual.replace_terminal(terminal_index, new_terminal)
@@ -47,38 +47,40 @@
     """
 
     def primitive_replaceable(index_primitive):
         _, primitive = index_primitive
         return len(primitive_set[primitive._primitive.output]) > 1
 
     primitives = list(filter(primitive_replaceable, enumerate(individual.primitives)))
-    if len(primitives) == 0:
+    if not primitives:
         raise ValueError("Individual has no primitives suitable for replacement.")
 
     primitive_index, old_primitive_node = random.choice(primitives)
     primitive_node = random_primitive_node(
         output_type=old_primitive_node._primitive.output,
         primitive_set=primitive_set,
         exclude=old_primitive_node._primitive,
     )
     individual.replace_primitive(primitive_index, primitive_node)
 
 
 def mut_shrink(
-    individual: Individual, primitive_set: dict = None, shrink_by: Optional[int] = None
+    individual: Individual,
+    _primitive_set: Optional[dict] = None,
+    shrink_by: Optional[int] = None,
 ) -> None:
     """Mutates an Individual in-place by removing any number of primitive nodes.
 
     Primitive nodes are removed from the preprocessing end.
 
     Parameters
     ----------
     individual: Individual
         Individual to mutate in-place.
-    primitive_set: dict, optional
+    _primitive_set: dict, optional
         Not used. Present to create a matching function signature with other mutations.
     shrink_by: int, optional (default=None)
         Number of primitives to remove.
         Must be at least one greater than the number of primitives in `individual`.
         If None, a random number of primitives is removed.
     """
     n_primitives = len(list(individual.primitives))
```

### Comparing `gama-22.0.0/gama/genetic_programming/nsga2.py` & `gama-23.0.0/gama/genetic_programming/nsga2.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
         self.values = tuple((m(obj) for m in metrics))
         self.rank = 0
         self.distance = 0.0
         self.dominating: List["NSGAMeta"] = []
         self.domination_counter = 0
 
     def dominates(self, other: "NSGAMeta") -> bool:
-        for self_val, other_val in zip(self.values, other.values):
-            if self_val <= other_val:  # or maybe <?
-                return False
-        return True
+        return all(
+            self_val > other_val
+            for self_val, other_val in zip(self.values, other.values)
+        )
 
     def crowd_compare(self, other: "NSGAMeta") -> int:
         """Favor higher rank, if equal, favor less crowded."""
         self_better = self.rank < other.rank or (
             self.rank == other.rank and self.distance > other.distance
         )
         return -1 if self_better else 1
```

### Comparing `gama-22.0.0/gama/genetic_programming/operations.py` & `gama-23.0.0/gama/genetic_programming/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import List
+from typing import List, Optional
 
 from gama.genetic_programming.components import (
     Primitive,
     Terminal,
     PrimitiveNode,
     DATA_TERMINAL,
 )
@@ -13,15 +13,15 @@
     primitive_set: dict, primitive: Primitive
 ) -> List[Terminal]:
     """Return a list with a random Terminal for each required input to Primitive."""
     return [random.choice(primitive_set[term_type]) for term_type in primitive.input]
 
 
 def random_primitive_node(
-    output_type: str, primitive_set: dict, exclude: Primitive = None
+    output_type: str, primitive_set: dict, exclude: Optional[Primitive] = None
 ) -> PrimitiveNode:
     """Create a PrimitiveNode with specified output_type and random terminals."""
     primitive = random.choice([p for p in primitive_set[output_type] if p != exclude])
     terminals = random_terminals_for_primitive(primitive_set, primitive)
     return PrimitiveNode(primitive, data_node=DATA_TERMINAL, terminals=terminals)
```

### Comparing `gama-22.0.0/gama/genetic_programming/operator_set.py` & `gama-23.0.0/gama/genetic_programming/operator_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,33 +39,29 @@
         self.evaluate: Optional[Callable[..., Evaluation]] = None
 
         self._completed_evaluations = completed_evaluations
 
     def wait_next(self, async_evaluator):
         """Wrapper for wait_next() to forward evaluation and log exceptions."""
         future = async_evaluator.wait_next()
-        if future.result is not None:
-            evaluation = future.result
-            if self._evaluate_callback is not None:
-                self._evaluate_callback(evaluation)
-
-        elif future.exception is not None:
+        if future.result and self._evaluate_callback:
+            self._evaluate_callback(future.result)
+        elif future.exception:
             log.warning(f"Error raised during evaluation: {str(future.exception)}.")
         return future
 
     def try_until_new(self, operator, *args, **kwargs):
         """Keep executing `operator` until a new individual is created."""
         for _ in range(self._max_retry):
             individual = operator(*args, **kwargs)
             if str(individual.main_node) not in self._completed_evaluations:
                 return individual
-        else:
-            log.debug(f"50 iterations of {operator.__name__} did not yield new ind.")
-            # For progress on solving this, see #11
-            return individual
+        log.debug(f"50 iterations of {operator.__name__} did not yield new ind.")
+        # For progress on solving this, see #11
+        return individual
 
     def mate(self, ind1: Individual, ind2: Individual, *args, **kwargs) -> Individual:
         def mate_with_log():
             new_individual1, new_individual2 = ind1.copy_as_new(), ind2.copy_as_new()
             self._mate(new_individual1, new_individual2, *args, **kwargs)
             new_individual1.meta = dict(parents=[ind1._id, ind2._id], origin="cx")
             return new_individual1
@@ -79,19 +75,15 @@
             new_individual.meta = dict(parents=[ind._id], origin=mutator.__name__)
             return new_individual
 
         return self.try_until_new(mutate_with_log)
 
     def individual(self, *args, **kwargs) -> Individual:
         expression = self._create_new(*args, **kwargs)
-        if self._safe_compile is not None:
-            compile_ = self._safe_compile
-        else:
-            compile_ = self._compile
-
+        compile_ = self._safe_compile or self._compile
         ind = Individual(expression, to_pipeline=compile_)
         ind.meta["origin"] = "new"
         return ind
 
     def create(self, *args, **kwargs) -> List[Individual]:
         return self._create_from_population(self, *args, **kwargs)
```

### Comparing `gama-22.0.0/gama/genetic_programming/selection.py` & `gama-23.0.0/gama/genetic_programming/selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     cxpb: float,
     mutpb: float,
 ) -> List[Individual]:
     """Creates n new individuals based on the population."""
     offspring = []
     metrics = [lambda ind: ind.fitness.values[0], lambda ind: ind.fitness.values[1]]
     parent_pairs = nsga2_select(pop, n, metrics)
-    for (ind1, ind2) in parent_pairs:
+    for ind1, ind2 in parent_pairs:
         if random.random() < cxpb and len(_valid_crossover_functions(ind1, ind2)) > 0:
             ind1 = operator_shell.mate(ind1, ind2)
         else:
             ind1 = operator_shell.mutate(ind1)
         offspring.append(ind1)
     return offspring
```

### Comparing `gama-22.0.0/gama/logging/GamaReport.py` & `gama-23.0.0/gama/logging/GamaReport.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             and old log with a slightly different search space.
         """
         self._log_directory = os.path.expanduser(log_directory)
         self.name = os.path.split(log_directory)[-1]
         self.phases: List[Tuple[str, str, datetime, float]] = []
         self._last_tell = 0
         self.evaluations: pd.DataFrame = pd.DataFrame()
-        self.individuals: Dict[str, Individual] = dict()
+        self.individuals: Dict[str, Individual] = {}
         self.strict = strict
 
         # Parse initialization/progress information from gama.log
         with open(os.path.join(log_directory, "gama.log")) as fh:
             gama_lines = fh.readlines()
 
         for line in gama_lines:
@@ -85,15 +85,17 @@
             df["n"] = df.index
             df = df.rename(columns=dict(t_start="start", t_wallclock="duration"))
 
             def tuple_to_metrics(tuple_str):
                 return pd.Series([float(value) for value in tuple_str[1:-1].split(",")])
 
             df[self.metrics] = df.score.apply(tuple_to_metrics)
-            df.start = pd.to_datetime(df.start)  # needed?
+            df.start = pd.to_datetime(
+                df.start, format="%Y-%m-%d %H:%M:%S,%f"
+            )  # needed?
             df.duration = pd.to_timedelta(df.duration, unit="s")
 
             new_individuals = {
                 id_: Individual.from_string(pipeline, pset, strict=self.strict)
                 for id_, pipeline in zip(df.id, df.pipeline)
             }
```

### Comparing `gama-22.0.0/gama/logging/evaluation_logger.py` & `gama-23.0.0/gama/logging/evaluation_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,12 +70,10 @@
         with open(self._file_path, "a") as evaluations:
             evaluations.write(self._sep.join(values) + "\n")
 
     def log_evaluation(self, evaluation) -> None:
         values = [getter(evaluation) for getter in self.fields.values()]
 
         def format_value(v):
-            if isinstance(v, datetime):
-                return v.strftime(TIME_FORMAT)
-            return str(v)
+            return v.strftime(TIME_FORMAT) if isinstance(v, datetime) else str(v)
 
         self.log_line(map(format_value, values))
```

### Comparing `gama-22.0.0/gama/logging/utility_functions.py` & `gama-23.0.0/gama/logging/utility_functions.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/postprocessing/base_post_processing.py` & `gama-23.0.0/gama/postprocessing/base_post_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC
-from typing import List, Union, Dict, Any, Tuple, TYPE_CHECKING, Sequence
+from typing import List, Union, Dict, Any, Tuple, TYPE_CHECKING, Sequence, Optional
 
 import pandas as pd
 from sklearn.base import TransformerMixin
 
 from gama.genetic_programming.components import Individual
 
 
@@ -83,15 +83,15 @@
         -------
         Any
             A model with `predict` and optionally `predict_proba`.
         """
         raise NotImplementedError("Method must be implemented by child class.")
 
     def to_code(
-        self, preprocessing: Sequence[Tuple[str, TransformerMixin]] = None
+        self, preprocessing: Optional[Sequence[Tuple[str, TransformerMixin]]] = None
     ) -> str:
         """Generate Python code to reconstruct a pipeline that constructs the model.
 
         Parameters
         ----------
         preprocessing: Sequence[TransformerMixin], optional (default=None)
             Preprocessing steps that need be executed before the model.
```

### Comparing `gama-22.0.0/gama/postprocessing/best_fit.py` & `gama-23.0.0/gama/postprocessing/best_fit.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,22 +23,21 @@
     def post_process(
         self, x: pd.DataFrame, y: pd.Series, timeout: float, selection: List[Individual]
     ) -> object:
         self._selected_individual = selection[0]
         return self._selected_individual.pipeline.fit(x, y)
 
     def to_code(
-        self, preprocessing: Sequence[Tuple[str, TransformerMixin]] = None
+        self, preprocessing: Optional[Sequence[Tuple[str, TransformerMixin]]] = None
     ) -> str:
         if self._selected_individual is None:
             raise RuntimeError("`to_code` can only be called after `post_process`.")
 
         imports, steps = imports_and_steps_for_individual(self._selected_individual)
         if preprocessing is not None:
             trans_strs = transformers_to_str([t for _, t in preprocessing])
             names = [name for name, _ in preprocessing]
             steps = list(zip(names, trans_strs)) + steps
             imports = imports.union({format_import(t) for _, t in preprocessing})
 
         pipeline_statement = format_pipeline(steps)
-        script = "\n".join(imports) + "\n\n" + pipeline_statement
-        return script
+        return "\n".join(imports) + "\n\n" + pipeline_statement
```

### Comparing `gama-22.0.0/gama/postprocessing/ensemble.py` & `gama-23.0.0/gama/postprocessing/ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
             timeout,
             self.hyperparameters["metric"],
             self.hyperparameters["evaluation_library"],
         )
         return self._ensemble
 
     def to_code(
-        self, preprocessing: Sequence[Tuple[str, TransformerMixin]] = None
+        self, preprocessing: Optional[Sequence[Tuple[str, TransformerMixin]]] = None
     ) -> str:
         if isinstance(self._ensemble, EnsembleClassifier):
             voter = "VotingClassifier"
         elif isinstance(self._ensemble, EnsembleRegressor):
             voter = "VotingRegressor"
         else:
             raise RuntimeError(f"Can't export ensemble of type {type(self._ensemble)}.")
@@ -219,51 +219,49 @@
 
         return self._model_library
 
     def _ensemble_validation_score(self, prediction_to_validate=None):
         raise NotImplementedError("Must be implemented by child class.")
 
     def _total_fit_weights(self):
-        return sum([weight for (model, weight) in self._fit_models])
+        return sum(weight for (model, weight) in self._fit_models)
 
     def _total_model_weights(self):
-        return sum([weight for (model, weight) in self._models.values()])
+        return sum(weight for (model, weight) in self._models.values())
 
     def _averaged_validation_predictions(self):
         """Weighted average of predictions of current models on the hillclimb set."""
         weighted_sum_predictions = sum(
-            [model.predictions * weight for (model, weight) in self._models.values()]
+            model.predictions * weight for (model, weight) in self._models.values()
         )
         return weighted_sum_predictions / self._total_model_weights()
 
     def build_initial_ensemble(self, n: int):
         """Add top n models in EvaluationLibrary to the ensemble.
 
         Parameters
         ----------
         n: int
             Number of models to include.
         """
-        if not n > 0:
+        if n <= 0:
             raise ValueError("Ensemble must include at least one model.")
         if self._models:
             log.warning(
                 "The ensemble already contained models. Overwriting the ensemble."
             )
             self._models = {}
 
         # Since the model library only features unique models,
         # we do not need to check for duplicates here.
         for model in self.model_library[:n]:
             self._add_model(model)
 
         log.debug(
-            "Initial ensemble created with score {}".format(
-                self._ensemble_validation_score()
-            )
+            f"Initial ensemble created with score {self._ensemble_validation_score()}"
         )
 
     def _add_model(self, model, add_weight=1):
         """Add a specific model to the ensemble or increases its weight."""
         model, weight = self._models.pop(model.individual._id, (model, 0))
         new_weight = weight + add_weight
         self._models[model.individual._id] = (model, new_weight)
@@ -273,15 +271,15 @@
         """Adds new models to the ensemble based on earlier given data.
 
         Parameters
         ----------
         n: int
             Number of models to add to current ensemble.
         """
-        if not n > 0:
+        if n <= 0:
             raise ValueError("n must be greater than 0.")
 
         for _ in range(n):
             best_addition_score = -float("inf")
             current_weighted_average = self._averaged_validation_predictions()
             current_total_weight = self._total_model_weights()
             for model in self.model_library:
@@ -295,17 +293,16 @@
                 )
                 if best_addition_score < candidate_ensemble_score:
                     best_addition, best_addition_score = model, candidate_ensemble_score
 
             self._add_model(best_addition)
             self._internal_score = best_addition_score
             log.info(
-                "Ensemble size {} , best score: {}".format(
-                    self._total_model_weights(), best_addition_score
-                )
+                f"Ensemble size {self._total_model_weights()}, "
+                f"best score: {best_addition_score}"
             )
 
     def fit(self, x, y, timeout=1e6):
         """Constructs an Ensemble out of the library of models.
 
         Parameters
         ----------
@@ -348,15 +345,15 @@
         #             self._fit_models.append((pipeline, weight))
         #
         # if not c_mgr:
         #     log.info("Fitting of ensemble stopped early.")
 
     def _get_weighted_mean_predictions(self, X, predict_method="predict"):
         weighted_predictions = []
-        for (model, weight) in self._fit_models:
+        for model, weight in self._fit_models:
             target_prediction = getattr(model, predict_method)(X)
             if self._prediction_transformation:
                 target_prediction = self._prediction_transformation(target_prediction)
             weighted_predictions.append(target_prediction * weight)
 
         return sum(weighted_predictions) / self._total_fit_weights()
 
@@ -437,20 +434,19 @@
 
     def _ensemble_validation_score(self, prediction_to_validate=None):
         if prediction_to_validate is None:
             prediction_to_validate = self._averaged_validation_predictions()
 
         if self._metric.requires_probabilities:
             return self._metric.maximizable_score(self._y, prediction_to_validate)
-        else:
-            # argmax returns (N, 1) matrix, need to squeeze it to (N,) for scoring.
-            class_predictions = self._one_hot_encoder.inverse_transform(
-                prediction_to_validate.toarray()
-            )
-            return self._metric.maximizable_score(self._y, class_predictions)
+        # argmax returns (N, 1) matrix, need to squeeze it to (N,) for scoring.
+        class_predictions = self._one_hot_encoder.inverse_transform(
+            prediction_to_validate.toarray()
+        )
+        return self._metric.maximizable_score(self._y, class_predictions)
 
     def predict(self, X):
         if self._metric.requires_probabilities:
             log.warning(
                 "Ensemble was tuned with a class-probabilities metric. "
                 "Using argmax of probabilities, which may not give optimal predictions."
             )
@@ -467,20 +463,19 @@
             class_predictions = self._label_encoder.inverse_transform(class_predictions)
 
         return class_predictions.ravel()
 
     def predict_proba(self, X):
         if self._metric.requires_probabilities:
             return self._get_weighted_mean_predictions(X, "predict_proba")
-        else:
-            log.warning(
-                "Ensemble was tuned with a class label predictions metric, "
-                "not probabilities. Using weighted mean of class predictions."
-            )
-            return self._get_weighted_mean_predictions(X, "predict").toarray()
+        log.warning(
+            "Ensemble was tuned with a class label predictions metric, "
+            "not probabilities. Using weighted mean of class predictions."
+        )
+        return self._get_weighted_mean_predictions(X, "predict").toarray()
 
 
 class EnsembleRegressor(Ensemble):
     def _ensemble_validation_score(self, prediction_to_validate=None):
         if prediction_to_validate is None:
             prediction_to_validate = self._averaged_validation_predictions()
         return self._metric.maximizable_score(self._y, prediction_to_validate)
@@ -520,14 +515,14 @@
             ensemble.build_initial_ensemble(10)
 
         remainder = ensemble_size - ensemble._total_model_weights()
         if remainder > 0:
             ensemble.expand_ensemble(remainder)
 
         build_time = time.time() - start_build
-        timeout = timeout - build_time
+        timeout -= build_time
         log.info(f"Ensemble build took {build_time}s. Fit with timeout {timeout}s.")
         ensemble.fit(x, y, timeout)
     except Exception as e:
         log.warning(f"Error during auto ensemble: {e}", exc_info=True)
 
     return ensemble
```

### Comparing `gama-22.0.0/gama/search_methods/__init__.py` & `gama-23.0.0/gama/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/search_methods/asha.py` & `gama-23.0.0/gama/search_methods/asha.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,18 +157,17 @@
                 # Problem: equal loss falls back on comparison of individual
                 not_promoted = set(individuals) - set(promoted_individuals[rung])
                 if len(not_promoted) > 0:
                     to_promote = max(not_promoted, key=lambda i: i[0])
                     promoted_individuals[rung].append(to_promote)
                     return to_promote[1], rung + 1
 
-        if start_candidates is not None and len(start_candidates) > 0:
+        if start_candidates:
             return start_candidates.pop(), minimum_early_stopping_rate
-        else:
-            return operations.individual(), minimum_early_stopping_rate
+        return operations.individual(), minimum_early_stopping_rate
 
     try:
         with AsyncEvaluator() as async_:
             log.info("ASHA start")
 
             def start_new_job():
                 individual, rung = get_job()
```

### Comparing `gama-22.0.0/gama/search_methods/async_ea.py` & `gama-23.0.0/gama/search_methods/async_ea.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/search_methods/base_search.py` & `gama-23.0.0/gama/search_methods/base_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 class BaseSearch(ABC):
     """All search methods should be derived from this class.
     This class should not be directly used to configure GAMA.
     """
 
     def __init__(self):
         # hyperparameters can be used to safe/process search hyperparameters
-        self._hyperparameters: Dict[str, Tuple[Any, Any]] = dict()
+        self._hyperparameters: Dict[str, Tuple[Any, Any]] = {}
         self.output: List[Individual] = []
         self.logger = EvaluationLogger
 
     def __str__(self) -> str:
         # Not sure if I should report actual used hyperparameters (i.e. include default)
         # or only those set by user.
         user_set_hps = {
```

### Comparing `gama-22.0.0/gama/search_methods/random_search.py` & `gama-23.0.0/gama/search_methods/random_search.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/utilities/cli.py` & `gama-23.0.0/gama/utilities/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,18 +149,15 @@
 
     x, y = X_y_from_file(
         file_path=args.input_file.lower(),
         split_column=args.target,
         **kwargs,
     )
     if args.mode is None:
-        if is_categorical_dtype(y.dtype):
-            args.mode = "classification"
-        else:
-            args.mode = "regression"
+        args.mode = "classification" if is_categorical_dtype(y.dtype) else "regression"
         print(f"Detected a {args.mode} problem.")
 
     print("CLI: Initializing GAMA")
     log_level = logging.INFO if args.verbose else logging.WARNING
     configuration = dict(
         regularize_length=args.prefer_short,
         max_total_time=args.time_limit_m * 60,
```

### Comparing `gama-22.0.0/gama/utilities/evaluation_library.py` & `gama-23.0.0/gama/utilities/evaluation_library.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self,
         individual: Individual,
         predictions: Optional[Union[np.ndarray, pd.Series, pd.DataFrame]] = None,
         score: Tuple[float, ...] = (),
         estimators: Optional[List] = None,
         start_time: Optional[datetime.datetime] = None,
         duration: float = -1,
-        error: str = None,
+        error: Optional[str] = None,
         pid: Optional[int] = None,
     ):
         self.individual: Individual = individual
         self.score = score
         self._estimators: List[BaseEstimator] = [] if estimators is None else estimators
         self.start_time = start_time
         self.duration = duration
@@ -40,41 +40,39 @@
 
         if isinstance(predictions, (pd.Series, pd.DataFrame)):
             predictions = predictions.values
         self._predictions: Optional[np.ndarray] = predictions
 
     def to_disk(self, directory: str) -> None:
         """Save Evaluation in the provided directory."""
-        self._cache_file = os.path.join(directory, str(self.individual._id) + ".pkl")
+        self._cache_file = os.path.join(directory, f"{str(self.individual._id)}.pkl")
         with open(self._cache_file, "wb") as fh:
             pickle.dump((self._estimators, self._predictions), fh)
         self._estimators, self._predictions = [], None
 
     def remove_from_disk(self) -> None:
         """Remove the related file from disk."""
         os.remove(os.path.join(self._cache_file))
         self._cache_file = ""
 
     @property
     def estimators(self) -> List[BaseEstimator]:
         if self._estimators or not self._cache_file:
             return self._estimators
-        else:
-            with open(self._cache_file, "rb") as fh:
-                estimators, _ = pickle.load(fh)
-                return estimators
+        with open(self._cache_file, "rb") as fh:
+            estimators, _ = pickle.load(fh)
+            return estimators
 
     @property
     def predictions(self):
         if self._predictions is not None or not self._cache_file:
             return self._predictions
-        else:
-            with open(self._cache_file, "rb") as fh:
-                _, predictions = pickle.load(fh)
-                return predictions
+        with open(self._cache_file, "rb") as fh:
+            _, predictions = pickle.load(fh)
+            return predictions
 
     # Is there a better way to do this?
     # Assignment in __init__ is not preferred even if it saves lines.
     def __lt__(self, other):
         return self.score.__lt__(other.score)
 
     def __le__(self, other):
@@ -194,31 +192,28 @@
             raise ValueError(
                 "Exactly one of `prediction_size` and `stratify` must be set."
             )
         if len(self.top_evaluations) > 0:
             log.warning("New subsample not used for already stored evaluations.")
         n = self._sample_n if n is None else n
 
-        if n is not None:
-            if prediction_size is not None and n < prediction_size:
-                # Subsample is to be chosen uniformly random.
-                self._sample = np.random.choice(
-                    range(prediction_size), size=n, replace=False
-                )
-            elif stratify is not None and n < len(stratify):
-                splitter = StratifiedShuffleSplit(n_splits=1, train_size=n)
-                self._sample, _ = next(
-                    splitter.split(np.zeros(len(stratify)), stratify)
-                )
-            else:
-                # Specified sample size exceeds size of predictions
-                self._sample = None
-        else:
+        if n is None:
             # No n was provided here nor set on initialization
             self._sample = None
+        elif prediction_size is not None and n < prediction_size:
+            # Subsample is to be chosen uniformly random.
+            self._sample = np.random.choice(
+                range(prediction_size), size=n, replace=False
+            )
+        elif stratify is not None and n < len(stratify):
+            splitter = StratifiedShuffleSplit(n_splits=1, train_size=n)
+            self._sample, _ = next(splitter.split(np.zeros(len(stratify)), stratify))
+        else:
+            # Specified sample size exceeds size of predictions
+            self._sample = None
 
     def _process_predictions(self, evaluation: Evaluation) -> None:
         """Downsample evaluation predictions if required."""
         if self._sample_n == 0:
             evaluation._predictions = None
         if evaluation.predictions is None:
             return  # Predictions either not provided or removed because sample_n is 0.
```

### Comparing `gama-22.0.0/gama/utilities/export.py` & `gama-23.0.0/gama/utilities/export.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import copy
-from typing import Tuple, List, Set
+from typing import Tuple, List, Set, Optional
 
 from sklearn.base import TransformerMixin
 from gama.genetic_programming.components import Individual
 
 
 def transformers_to_str(transformers: List[TransformerMixin]) -> List[str]:
     """Format a transformer for code export, removes any mapping."""
     copies = list(map(copy.copy, transformers))
     for transformer in copies:
         if hasattr(transformer, "mapping"):
-            transformer.mapping = None  # type: ignore  # ignore no attr 'mapping'
+            transformer.mapping = None
     return list(map(str, copies))
 
 
 def format_import(o: object) -> str:
     """Creates the import statement for `o`'s class."""
     if o.__module__.split(".")[-1].startswith("_"):
         module = ".".join(o.__module__.split(".")[:-1])
@@ -41,29 +41,27 @@
     """
     imports = ["from numpy import nan", "from sklearn.pipeline import Pipeline"]
     imports += [format_import(step) for name, step in individual.pipeline.steps]
 
     steps = []
     for i, primitive_node in reversed(list(enumerate(individual.primitives))):
         steps.append((str(i), primitive_node.str_nonrecursive))
-        for terminal in primitive_node._terminals:
-            if callable(terminal.value) and hasattr(terminal.value, "__name__"):
-                imports.append(
-                    f"from {terminal.value.__module__} import {terminal.value.__name__}"  # type: ignore # noqa: E501
-                )
-
+        imports.extend(
+            f"from {terminal.value.__module__} import {terminal.value.__name__}"
+            for terminal in primitive_node._terminals
+            if callable(terminal.value) and hasattr(terminal.value, "__name__")
+        )
     return set(imports), steps
 
 
 def individual_to_python(
-    individual: Individual, prepend_steps: List[Tuple[str, TransformerMixin]] = None
+    individual: Individual,
+    prepend_steps: Optional[List[Tuple[str, TransformerMixin]]] = None,
 ) -> str:
     """Generate code for the machine learning pipeline represented by `individual`."""
     imports, steps = imports_and_steps_for_individual(individual)
     if prepend_steps is not None:
         steps = prepend_steps + steps
         imports = imports.union({format_import(step) for _, step in prepend_steps})
     steps_str = ",\n".join([f"('{name}', {step})" for name, step in steps])
     pipeline = f"Pipeline([{steps_str}])"
-    script = "\n".join(sorted(imports)) + "\n\n" + "pipeline = " + pipeline + "\n"
-
-    return script
+    return "\n".join(sorted(imports)) + "\n\n" + "pipeline = " + pipeline + "\n"
```

### Comparing `gama-22.0.0/gama/utilities/generic/async_evaluator.py` & `gama-23.0.0/gama/utilities/generic/async_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,16 @@
       Unfortunately it is possible the subprocesses can be running non-Python code,
       e.g. a C implementation of SVC whose subprocess won't end until fit is complete.
     - even if that is overwritten and no wait is performed,
       the subprocess will raise an error when it is done.
       Though that does not hinder the execution of the program,
       I don't want errors for expected behavior.
 """
+
+import contextlib
 import datetime
 import gc
 import logging
 import multiprocessing
 import os
 import psutil
 import queue
@@ -137,15 +139,15 @@
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         log.debug(f"Signaling {len(self._processes)} subprocesses to stop.")
 
         for _ in self._processes:
             self._command.put("stop")
 
-        for i in range(self._wait_time_before_forced_shutdown + 1):
+        for _ in range(self._wait_time_before_forced_shutdown + 1):
             if self._command.empty():
                 break
             time.sleep(1)
 
         self.clear_queue(self._input)
         self.clear_queue(self._output)
         self.clear_queue(self._command)
@@ -159,18 +161,16 @@
             except psutil.NoSuchProcess:
                 self.job_queue_size -= 1
                 self._processes.remove(self._processes[0])
         return False
 
     def clear_queue(self, q: multiprocessing.Queue):
         while not q.empty():
-            try:
+            with contextlib.suppress(queue.Empty):
                 q.get(timeout=0.001)
-            except queue.Empty:
-                pass
         q.close()
 
     def submit(self, fn: Callable, *args, **kwargs) -> AsyncFuture:
         """Submit fn(*args, **kwargs) to be evaluated on a subprocess.
 
         Parameters
         ----------
@@ -215,15 +215,14 @@
         if len(self.futures) == 0:
             raise RuntimeError("No Futures queued, must call `submit` first.")
         while True:
             self._control_memory_usage()
             self._log_memory_usage()
 
             try:
-
                 completed_future = self._output.get(block=False)
                 self.job_queue_size -= 1
             except queue.Empty:
                 time.sleep(poll_time)
                 continue
 
             match = self.futures.pop(completed_future.id)
@@ -345,20 +344,17 @@
         Queue should be managed by multiprocessing.manager.
     default_parameters: Dict, optional (default=None)
         Additional parameters to pass to AsyncFuture.Execute.
         This is useful to avoid passing lots of repetitive data through AsyncFuture.
     """
     try:
         while True:
-            try:
+            with contextlib.suppress(queue.Empty):
                 command_queue.get(block=False)
                 break
-            except queue.Empty:
-                pass
-
             try:
                 future = input_queue.get(block=False)
                 future.execute(default_parameters)
                 if future.result:
                     if isinstance(future.result, tuple):
                         result = future.result[0]
                     else:
```

### Comparing `gama-22.0.0/gama/utilities/generic/paretofront.py` & `gama-23.0.0/gama/utilities/generic/paretofront.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,18 +26,15 @@
         if start_list:
             for item in start_list:
                 self.update(item)
 
         self._iterator_index = 0
 
     def _get_item_value(self, item):
-        if self._get_values_fn is not None:
-            return self._get_values_fn(item)
-        else:
-            return item
+        return self._get_values_fn(item) if self._get_values_fn is not None else item
 
     def update(self, new_item: Any):
         """Update the Pareto front with new_item if it qualifies.
 
         Parameters
         ----------
         new_item: Any
```

### Comparing `gama-22.0.0/gama/utilities/generic/stopwatch.py` & `gama-23.0.0/gama/utilities/generic/stopwatch.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/utilities/generic/timekeeper.py` & `gama-23.0.0/gama/utilities/generic/timekeeper.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama/utilities/metrics.py` & `gama-23.0.0/gama/utilities/metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,20 +63,21 @@
         return self.scorer._sign * self.score(*args, **kwargs)
 
 
 def scoring_to_metric(
     scoring: Union[str, Metric, Iterable[str], Iterable[Metric]]
 ) -> Tuple[Metric, ...]:
     if isinstance(scoring, str):
-        return tuple([Metric(scoring)])
+        return (Metric(scoring),)
     if isinstance(scoring, Metric):
-        return tuple([scoring])
+        return (scoring,)
 
-    if isinstance(scoring, Iterable):
-        if all([isinstance(scorer, (Metric, str)) for scorer in scoring]):
-            converted_metrics = [
-                scorer if isinstance(scorer, Metric) else Metric(scorer)
-                for scorer in scoring
-            ]
-            return tuple(converted_metrics)
+    if isinstance(scoring, Iterable) and all(
+        isinstance(scorer, (Metric, str)) for scorer in scoring
+    ):
+        converted_metrics = [
+            scorer if isinstance(scorer, Metric) else Metric(scorer)
+            for scorer in scoring
+        ]
+        return tuple(converted_metrics)
 
     raise TypeError("scoring must be str, Metric or Iterable (of str or Metric).")
```

### Comparing `gama-22.0.0/gama/utilities/preprocessing.py` & `gama-23.0.0/gama/utilities/preprocessing.py`

 * *Files identical despite different names*

### Comparing `gama-22.0.0/gama.egg-info/PKG-INFO` & `gama-23.0.0/gama.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: gama
-Version: 22.0.0
+Version: 23.0.0
 Summary: A package for automated machine learning based on scikit-learn.
 Author-email: Pieter Gijsbers <p.gijsbers@tue.nl>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: test
-Provides-Extra: vis
 License-File: LICENSE
 
 ![GAMA logo](https://github.com/openml-labs/gama/blob/master/images/logos/Logo-With-Grey-Name-Transparent.png)
 
 **G**eneral **A**utomated **M**achine learning **A**ssistant  
 An automated machine learning tool based on genetic programming.  
 Make sure to check out the [documentation](https://openml-labs.github.io/gama/).
@@ -35,15 +34,15 @@
 
 In addition to its general use AutoML functionality, GAMA aims to serve AutoML researchers as well.
 During the optimization process, GAMA keeps an extensive log of progress made.
 Using this log, insight can be obtained on the behaviour of the search procedure.
 For example, it can produce a graph that shows pipeline fitness over time:
 ![graph of fitness over time](https://github.com/openml-lab/gama/blob/master/docs/source/technical_guide/images/viz.gif)
 
-For more examples and information on the visualization, see [the technical guide](https://openml-labs.github.io/gama/master/user_guide/index.html#dashboard).
+*Note: we temporarily disabled support for the GAMA Dashboard, we will add out-of-the-box visualization again later this year.* 
 
 ## Installing GAMA
 
 You can install GAMA with pip: `pip install gama`
 
 ## Minimal Example
 
@@ -96,7 +95,10 @@
 publisher="Springer International Publishing",
 address="Cham",
 pages="560--564",
 abstract="The General Automated Machine learning Assistant (GAMA) is a modular AutoML system developed to empower users to track and control how AutoML algorithms search for optimal machine learning pipelines, and facilitate AutoML research itself. In contrast to current, often black-box systems, GAMA allows users to plug in different AutoML and post-processing techniques, logs and visualizes the search process, and supports easy benchmarking. It currently features three AutoML search algorithms, two model post-processing steps, and is designed to allow for more components to be added.",
 isbn="978-3-030-67670-4"
 }
 ```
+
+## License
+The contents of this repository is under an [Apache-2.0 License](https://github.com/openml-labs/gama/blob/master/LICENSE).
```

### Comparing `gama-22.0.0/gama.egg-info/SOURCES.txt` & `gama-23.0.0/gama.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-setup.py
 gama/GamaClassifier.py
 gama/GamaRegressor.py
 gama/__init__.py
 gama/__version__.py
 gama/data_formatting.py
 gama/data_loading.py
 gama/gama.py
@@ -16,27 +15,14 @@
 gama.egg-info/requires.txt
 gama.egg-info/top_level.txt
 gama/configuration/__init__.py
 gama/configuration/classification.py
 gama/configuration/parser.py
 gama/configuration/regression.py
 gama/configuration/testconfiguration.py
-gama/dashboard/__init__.py
-gama/dashboard/app.py
-gama/dashboard/controller.py
-gama/dashboard/plotting.py
-gama/dashboard/components/__init__.py
-gama/dashboard/components/cli_window.py
-gama/dashboard/components/headers.py
-gama/dashboard/components/input_group.py
-gama/dashboard/pages/__init__.py
-gama/dashboard/pages/analysispage.py
-gama/dashboard/pages/base_page.py
-gama/dashboard/pages/homepage.py
-gama/dashboard/pages/runningpage.py
 gama/genetic_programming/__init__.py
 gama/genetic_programming/crossover.py
 gama/genetic_programming/mutation.py
 gama/genetic_programming/nsga2.py
 gama/genetic_programming/operations.py
 gama/genetic_programming/operator_set.py
 gama/genetic_programming/selection.py
```

