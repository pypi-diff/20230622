# Comparing `tmp/cca_zoo-2.0.3.tar.gz` & `tmp/cca_zoo-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-2.0.3.tar", last modified: Mon Jun 19 12:41:14 2023, max compression
+gzip compressed data, was "dist/cca_zoo-2.0.4.tar", last modified: Thu Jun 22 14:21:16 2023, max compression
```

## Comparing `cca_zoo-2.0.3.tar` & `cca_zoo-2.0.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/classical/
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_gcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_grcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_altmaxvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    13664 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_deflation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13828 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_elasticnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gradkcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_incrementalpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pls_als.py
--rw-r--r--   0 runner    (1001) docker     (123)     6823 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_admm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_hsic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_parkhomenko.py
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_span.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_stochasticpls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_iterative/_swcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    12655 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_kcca.py
--rw-r--r--   0 runner    (1001) docker     (123)    10134 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_mcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_ncca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_partialcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_pcacca.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_pls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_prcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/classical/_tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/data/deep.py
--rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/data/simulated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/deep/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_ey.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_gh.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_sdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dgcca.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dtcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_dccae.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/_generative/_splitae.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/architectures.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/deep/objectives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/model_selection/_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/model_selection/_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/probabilistic/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/probabilistic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/probabilistic/_probabilisticcca.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_probabilistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_regularised.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_stochastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_unregularized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/utils/check_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/cca_zoo/visualisation/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/cca_zoo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dcca_custom_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dcca_multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_dvcca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_hyperparameter_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_kernel_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_many_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_sparse_cca.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-19 12:41:04.000000 cca_zoo-2.0.3/examples/plot_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:41:14.000000 cca_zoo-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-19 12:41:13.000000 cca_zoo-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/classical/
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_gcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_grcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_altmaxvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_deflation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_elasticnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_gradkcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_incrementalpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_pls_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_pmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_admm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_stochasticpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_iterative/_swcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12556 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_kcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_mcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_ncca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_partialcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_pcacca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_pls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_prcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/classical/_tcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/data/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7088 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/data/simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/deep/
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_noi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_sdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dgcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dtcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/deep/_generative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_generative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_generative/_dccae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_generative/_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/_generative/_splitae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/deep/objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/model_selection/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/model_selection/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/probabilistic/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/probabilistic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/probabilistic/_probabilisticcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13073 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_deepmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_probabilistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8021 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_regularised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_unregularized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/utils/check_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/cca_zoo/visualisation/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/cca_zoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_dcca_custom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_dcca_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_hyperparameter_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_kernel_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_many_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_sparse_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-06-22 14:21:03.000000 cca_zoo-2.0.4/examples/plot_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:21:16.000000 cca_zoo-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-22 14:21:15.000000 cca_zoo-2.0.4/setup.py
```

### Comparing `cca_zoo-2.0.3/PKG-INFO` & `cca_zoo-2.0.4/cca_zoo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cca_zoo
-Version: 2.0.3
+Name: cca-zoo
+Version: 2.0.4
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.3/README.md` & `cca_zoo-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/__init__.py` & `cca_zoo-2.0.4/cca_zoo/classical/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_base.py` & `cca_zoo-2.0.4/cca_zoo/classical/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_dummy.py` & `cca_zoo-2.0.4/cca_zoo/classical/_dummy.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_gcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_gcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_grcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_grcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/__init__.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_altmaxvar.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_altmaxvar.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,19 +88,23 @@
         weights,
         k=None,
         gamma=0.1,
         T=100,
         learning_rate=1e-1,
         proximal_operators=None,
     ):
-        super().__init__(weights, k)
+        super().__init__(weights, k, learning_rate=learning_rate)
         self.gamma = gamma
         self.proximal_operators = proximal_operators
         self.T = T
-        self.learning_rate = learning_rate
+
+    def forward(self, views: list) -> list:
+        # views detach and numpy
+        views = [view.detach().numpy() for view in views]
+        return [view @ weight for view, weight in zip(views, self.weights)]
 
     def _get_target(self, scores):
         if hasattr(self, "G"):
             R = self.gamma * scores.mean(axis=0) + (1 - self.gamma) * self.G
         else:
             R = scores.mean(axis=0)
         U, S, Vt = np.linalg.svd(R, full_matrices=False)
@@ -115,18 +119,18 @@
                 for view in range(self.n_views)
             ]
         ).sum()
         return least_squares + regularization
 
     def training_step(self, batch, batch_idx):
         scores = np.stack(self(batch["views"]))
-        old_weights = self.weights.copy()
         self.G = self._get_target(scores)
         converged = False
         for i, view in enumerate(batch["views"]):
+            view = view.detach().numpy()
             t = 0
             # initialize the previous weights to None
             prev_weights = None
             while t < self.T and not converged:
                 # update the weights using the gradient descent and proximal operator
                 self.weights[i] -= self.learning_rate * (
                     view.T @ (view @ self.weights[i] - self.G)
@@ -144,18 +148,9 @@
                 # update the previous weights for the next iteration
                 prev_weights = self.weights[i]
                 t += 1
 
         # if tracking or convergence_checking is enabled, compute the objective function
         if self.tracking or self.convergence_checking:
             objective = self.objective(batch["views"])
-            # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
-            weights_change = torch.tensor(
-                np.max(
-                    [
-                        np.max(np.abs(old_weights[i] - self.weights[i]))
-                        / np.max(np.abs(self.weights[i]))
-                        for i in range(len(self.weights))
-                    ]
-                )
-            )
-            return {"loss": torch.tensor(objective), "weights_change": weights_change}
+
+            return {"loss": torch.tensor(objective)}
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_base.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from abc import abstractmethod
 from typing import Iterable, List, Optional, Union, Any
 
 import numpy as np
 import pytorch_lightning as pl
-import torch
 from pytorch_lightning.callbacks import Callback, EarlyStopping
 from torch.utils import data
 from torch.utils.data import DataLoader
 
 from cca_zoo.data.deep import NumpyDataset
 from cca_zoo.classical import MCCA, rCCA
 from cca_zoo.classical._base import BaseModel
 from cca_zoo.classical._dummy import DummyCCA
+import torch
 
 # Default Trainer kwargs
 DEFAULT_TRAINER_KWARGS = dict(
     enable_checkpointing=False,
     logger=False,
     enable_model_summary=False,
     enable_progress_bar=False,
@@ -137,14 +137,15 @@
         if hasattr(loop, "epoch_objective"):
             self.objective = loop.epoch_objective
         return weights
 
     def get_dataloader(self, views: Iterable[np.ndarray]):
         if self.batch_size is None:
             dataset = BatchNumpyDataset(views)
+            # collate_fn should return the batch but with arrays in 'views' and 'labels' as tensors
             collate_fn = lambda x: x[0]
         else:
             dataset = NumpyDataset(views)
             collate_fn = None
         if self.val_split is not None:
             train_size = int((1 - self.val_split) * len(dataset))
             val_size = len(dataset) - train_size
@@ -194,110 +195,60 @@
     def __init__(
         self,
         weights=None,
         k=None,
         automatic_optimization=False,
         tracking=False,
         convergence_checking=False,
+        optimizer_kwargs=None,
+        learning_rate=1e-3,
     ):
         super().__init__()
         if k is not None:
             self.weights = [weight[:, k] for weight in weights]
         else:
             self.weights = weights
+
         self.automatic_optimization = automatic_optimization
         self.tracking = tracking
         self.convergence_checking = convergence_checking
+        if self.automatic_optimization:
+            # Set the weights attribute as torch parameters with gradients
+            self.weights = [
+                torch.nn.Parameter(torch.from_numpy(weight), requires_grad=True)
+                for weight in self.weights
+            ]
+            self.weights = torch.nn.ParameterList(self.weights)
+        # Set the optimizer keyword arguments attribute with default values if none provided
+        self.optimizer_kwargs = optimizer_kwargs or {}
+        self.learning_rate = learning_rate
 
     def objective(self, *args, **kwargs) -> float:
         raise NotImplementedError
 
     def forward(self, views: list) -> list:
-        """Compute the score vectors for each view.
-
-        Parameters
-        ----------
-        views : list
-            The input views to compute the score vectors from
-
-        Returns
-        -------
-        list
-            The score vectors for each view
-        """
         return [view @ weight for view, weight in zip(views, self.weights)]
 
     def configure_optimizers(self):
-        """
-        We don't need an optimizer for manual optimization.
-        """
-        pass
-
-
-class BaseGradientLoop(BaseLoop):
-    def __init__(
-        self,
-        weights: list = None,
-        k: int = None,
-        learning_rate: float = 1e-3,
-        optimizer_kwargs: dict = None,
-        tracking: bool = False,
-        convergence_checking: bool = False,
-    ):
-        """Initialize the gradient-based CCA loop.
-
-        Parameters
-        ----------
-        weights : list, optional
-            The initial weights for the CCA loop, by default None
-        k : int, optional
-            The index of the latent dimension to use for the CCA loop, by default None
-        learning_rate : float, optional
-            The learning rate for the optimizer, by default 1e-3
-        optimizer_kwargs : dict, optional
-            The keyword arguments for the optimizer creation, by default None
-        """
-        super().__init__(
-            weights=weights,
-            k=k,
-            automatic_optimization=True,
-            tracking=tracking,
-            convergence_checking=convergence_checking,
-        )
-        # Set the weights attribute as torch parameters with gradients
-        self.weights = [
-            torch.nn.Parameter(torch.from_numpy(weight), requires_grad=True)
-            for weight in self.weights
-        ]
-        self.weights = torch.nn.ParameterList(self.weights)
-
-        # Set the optimizer keyword arguments attribute with default values if none provided
-        self.optimizer_kwargs = optimizer_kwargs or {}
-        self.learning_rate = learning_rate
-
-    def configure_optimizers(self):
-        # construct optimizer using optimizer_kwargs
-        optimizer_name = self.optimizer_kwargs.get("optimizer", "Adam")
-        optimizer_kwargs = self.optimizer_kwargs.get("optimizer_kwargs", {})
-        optimizer = getattr(torch.optim, optimizer_name)(
-            self.weights, lr=self.learning_rate, **optimizer_kwargs
-        )
-        return optimizer
+        if self.automatic_optimization:
+            # construct optimizer using optimizer_kwargs
+            optimizer_name = self.optimizer_kwargs.get("optimizer", "Adam")
+            optimizer_kwargs = self.optimizer_kwargs.get("optimizer_kwargs", {})
+            optimizer = getattr(torch.optim, optimizer_name)(
+                self.weights, lr=self.learning_rate, **optimizer_kwargs
+            )
+            return optimizer
 
     def on_fit_end(self) -> None:
-        # weights to numpy arrays from torch parameters
-        weights = [weight.detach().cpu().numpy() for weight in self.weights]
-        del self.weights
-        self.weights = weights
-
-    def forward(self, views):
-        # if views are numpy arrays, convert to torch tensors
-        if isinstance(views[0], np.ndarray):
-            views = [torch.from_numpy(view) for view in views]
-        return [view @ weight for view, weight in zip(views, self.weights)]
+        # if self.weights are torch parameters, convert them to numpy arrays
+        if isinstance(self.weights, torch.nn.ParameterList):
+            # weights to numpy arrays from torch parameters
+            weights = [weight.detach().cpu().numpy() for weight in self.weights]
+            del self.weights
+            self.weights = weights
 
 
 def _default_initializer(initialization, random_state, latent_dims):
     if initialization == "random":
         initializer = DummyCCA(latent_dims, random_state=random_state, uniform=False)
     elif initialization == "uniform":
         initializer = DummyCCA(latent_dims, random_state=random_state, uniform=True)
@@ -392,16 +343,16 @@
             print(
                 f"Objective: {pl_module.epoch_objective[-1]:.3f} | Epoch: {trainer.current_epoch}",
             )
 
 
 class BatchNumpyDataset:
     def __init__(self, views, labels=None):
-        self.views = [view.astype(np.float32) for view in views]
-        self.labels = labels if labels is not None else None
+        self.views = [torch.from_numpy(view).float() for view in views]
+        self.labels = torch.from_numpy(labels).float() if labels is not None else None
 
     def __len__(self):
         return 1
 
     def __getitem__(self, index):
         if self.labels is not None:
             return {"views": self.views, "label": self.labels}
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_deflation.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_deflation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_elasticnet.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_elasticnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,14 @@
         random_state=None,
         tracking=False,
         convergence_checking=False,
     ):
         super().__init__(
             weights=weights,
             k=k,
-            automatic_optimization=False,
             tracking=tracking,
             convergence_checking=convergence_checking,
         )
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.n_views = len(self.weights)
         self.n_samples_ = self.weights[0].shape[0]
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_ey.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_ey.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 
 import numpy as np
 import torch
 
-from cca_zoo.classical._iterative._base import BaseGradientLoop, BaseIterative
+from cca_zoo.classical._iterative._base import BaseIterative, BaseLoop
 from cca_zoo.classical._pls import PLSMixin
 
 
 class CCAEY(BaseIterative):
     """
     A class used to fit Regularized CCA by Delta-EigenGame
 
@@ -158,15 +158,15 @@
             convergence_checking=self.convergence_checking,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
-class EYLoop(BaseGradientLoop):
+class EYLoop(BaseLoop):
     def __init__(
         self,
         weights=None,
         k=None,
         learning_rate=1e-3,
         optimizer_kwargs=None,
         objective="cca",
@@ -176,14 +176,15 @@
         super().__init__(
             weights=weights,
             k=k,
             learning_rate=learning_rate,
             optimizer_kwargs=optimizer_kwargs,
             tracking=tracking,
             convergence_checking=convergence_checking,
+            automatic_optimization=True,
         )
         self.objective = objective
         self.batch_queue = []
         self.val_batch_queue = []
 
     def training_step(self, batch, batch_idx):
         # Checking if the queue has at least one batch
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gh.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_gradkcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_gradkcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_incrementalpls.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_incrementalpls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pls_als.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_pls_als.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_pmd.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_pmd.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import torch
 
 from cca_zoo.classical._iterative._base import BaseLoop
 from cca_zoo.classical._iterative._deflation import BaseDeflation
 from cca_zoo.classical._pls import PLSMixin
 from cca_zoo.classical._search import _delta_search
-from cca_zoo.utils import _check_converged_weights, _process_parameter
+from cca_zoo.utils import _process_parameter
 
 
 class SCCA_PMD(BaseDeflation, PLSMixin):
     r"""
     A class used to fit a sparse CCA model by penalized matrix decomposition (PMD).
 
     This model finds the linear projections of two views that maximize their correlation while enforcing sparsity constraints on the projection vectors.
@@ -143,25 +143,30 @@
         self.t = [max(1, x * y) for x, y in zip(self.tau, shape_sqrts)]
 
     def training_step(self, batch, batch_idx):
         scores = np.stack(self(batch["views"]))
         old_weights = self.weights.copy()
         # Update each view using loop update function
         for view_index, view in enumerate(batch["views"]):
+            view = view.detach().cpu().numpy()
             # create a mask that is True for elements not equal to k along dim k
             mask = np.arange(scores.shape[0]) != view_index
             # apply the mask to scores and sum along dim k
             target = np.sum(scores[mask], axis=0)
-            self.weights[view_index] = batch["views"][view_index].T @ target
+            self.weights[view_index] = view.T @ target
             self.weights[view_index] = _delta_search(
                 self.weights[view_index],
                 self.t[view_index],
                 tol=self.tol,
             )
-            _check_converged_weights(self.weights[view_index], view_index)
+            if np.linalg.norm(self.weights[view_index]) <= 0:
+                warnings.warn(
+                    f"All result weights are zero in view {view_index}. "
+                    "Try less regularisation or another initialisation"
+                )
         # if tracking or convergence_checking is enabled, compute the objective function
         if self.tracking or self.convergence_checking:
             objective = self.objective(batch["views"])
             # check that the maximum change in weights is smaller than the tolerance times the maximum absolute value of the weights
             weights_change = torch.tensor(
                 np.max(
                     [
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_admm.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_admm.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_hsic.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_hsic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_parkhomenko.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_parkhomenko.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_scca_span.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_scca_span.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Iterable, Union
 
 import numpy as np
+import torch
 
 from cca_zoo.classical._iterative._base import BaseIterative, BaseLoop
 from cca_zoo.classical._search import _delta_search, support_threshold
 from cca_zoo.utils import _process_parameter
 
 
 class SCCA_Span(BaseIterative):
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_stochasticpls.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_stochasticpls.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 
+from cca_zoo.classical._iterative._base import BaseLoop
 from cca_zoo.classical._iterative._ey import PLSEY
-from cca_zoo.classical._iterative._base import BaseGradientLoop
 from cca_zoo.classical._pls import PLSMixin
 
 
 class PLSStochasticPower(PLSEY, PLSMixin):
     def _get_module(self, weights=None, k=None):
         return StochasticPowerLoopBase(
             weights=weights,
@@ -14,21 +14,22 @@
             optimizer_kwargs=self.optimizer_kwargs,
         )
 
     def _more_tags(self):
         return {"multiview": True, "stochastic": True}
 
 
-class StochasticPowerLoopBase(BaseGradientLoop):
+class StochasticPowerLoopBase(BaseLoop):
     def __init__(self, weights=None, k=None, learning_rate=1e-3, optimizer_kwargs=None):
         super().__init__(
             weights=weights,
             k=k,
             learning_rate=learning_rate,
             optimizer_kwargs=optimizer_kwargs,
+            automatic_optimization=True,
         )
 
     def training_step(self, batch, batch_idx):
         for weight in self.weights:
             weight.data = self._orth(weight)
         scores = self(batch["views"])
         # find the pairwise covariance between the scores
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_svd.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_iterative/_swcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_iterative/_swcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_kcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_kcca.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,36 +21,38 @@
         self.kernel_params = _process_parameter(
             "kernel_params", self.kernel_params, {}, self.n_views_
         )
 
     def _process_data(self, views, K=None):
         self.train_views = views
         kernels = [
-            get_kernel(
+            pairwise_kernels(
                 view,
                 metric=self.kernel[i],
                 gamma=self.gamma[i],
                 degree=self.degree[i],
                 coef0=self.coef0[i],
+                filter_params=True,
                 **self.kernel_params[i]
             )
             for i, view in enumerate(self.train_views)
         ]
         return kernels
 
-    def transform(self, views: np.ndarray, **kwargs):
+    def transform(self, views: Iterable[np.ndarray], **kwargs):
         check_is_fitted(self, attributes=["alphas"])
         Ktest = [
-            get_kernel(
+            pairwise_kernels(
                 self.train_views[i],
                 Y=view,
                 metric=self.kernel[i],
                 gamma=self.gamma[i],
                 degree=self.degree[i],
                 coef0=self.coef0[i],
+                filter_params=True,
                 **self.kernel_params[i]
             )
             for i, view in enumerate(views)
         ]
         transformed_views = [
             kernel.T @ self.alphas[i] for i, kernel in enumerate(Ktest)
         ]
@@ -241,20 +243,21 @@
         self.gamma = gamma
         self.coef0 = coef0
         self.kernel = kernel
         self.degree = degree
 
     def _weights(self, eigvals, eigvecs, views, **kwargs):
         kernels = [
-            get_kernel(
+            pairwise_kernels(
                 view,
                 metric=self.kernel[i],
                 gamma=self.gamma[i],
                 degree=self.degree[i],
                 coef0=self.coef0[i],
+                filter_params=True,
                 **self.kernel_params[i]
             )
             for i, view in enumerate(self.train_views)
         ]
         self.weights = [
             np.linalg.pinv(kernel) @ eigvecs[:, : self.latent_dimensions]
             for kernel in kernels
@@ -322,35 +325,23 @@
         self.coef0 = coef0
         self.kernel = kernel
         self.degree = degree
 
     def _setup_tensor(self, views: Iterable[np.ndarray], **kwargs):
         self.train_views = views
         kernels = [
-            get_kernel(
+            pairwise_kernels(
                 view,
                 metric=self.kernel[i],
                 gamma=self.gamma[i],
                 degree=self.degree[i],
                 coef0=self.coef0[i],
+                filter_params=True,
                 **self.kernel_params[i]
             )
             for i, view in enumerate(self.train_views)
         ]
         return super()._setup_tensor(kernels)
 
     def _more_tags(self):
         # Indicate that this class is for multiview data
         return {"multiview": True, "kernel": True}
-
-
-def get_kernel(X, Y=None, metric="linear", gamma=None, degree=1, coef0=1, **kwargs):
-    return pairwise_kernels(
-        X,
-        Y,
-        metric=metric,
-        gamma=gamma,
-        degree=degree,
-        coef0=coef0,
-        filter_params=True,
-        **kwargs
-    )
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_mcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_mcca.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,14 +80,17 @@
         self._validate_data(views)
         # Check the parameters
         self._check_params()
         views = self._process_data(views, **kwargs)
         eigvals, eigvecs = self._solve_gevp(views, y=y, **kwargs)
         # Compute the weights for each view
         self._weights(eigvals, eigvecs, views, **kwargs)
+        # delete pca to save memory
+        if self.pca:
+            del self.pca_models
         return self
 
     def _process_data(self, views, **kwargs):
         if self.pca:
             views = self._apply_pca(views)
         return views
 
@@ -112,38 +115,39 @@
 
     def _weights(self, eigvals, eigvecs, views, **kwargs):
         # split eigvecs into weights for each view
         self.weights = np.split(eigvecs, self.splits[:-1], axis=0)
         if self.pca:
             # go from weights in PCA space to weights in original space
             self.weights = [
-                pca.components_.T @ self.weights[i] for i, pca in enumerate(self.pca)
+                pca.components_.T @ self.weights[i]
+                for i, pca in enumerate(self.pca_models)
             ]
 
     def _apply_pca(self, views):
         """
         Do data driven PCA on each view
         """
-        self.pca = [PCA() for _ in views]
+        self.pca_models = [PCA() for _ in views]
         # Fit PCA on each view
-        return [self.pca[i].fit_transform(view) for i, view in enumerate(views)]
+        return [self.pca_models[i].fit_transform(view) for i, view in enumerate(views)]
 
     def C(self, views, **kwargs):
         all_views = np.hstack(views)
         C = np.cov(all_views, rowvar=False)
         C -= block_diag(*[np.cov(view, rowvar=False) for view in views])
         return C / len(views)
 
     def D(self, views, **kwargs):
         if self.pca:
             # Can regularise by adding to diagonal
             D = block_diag(
                 *[
                     np.diag((1 - self.c[i]) * pc.explained_variance_ + self.c[i])
-                    for i, pc in enumerate(self.pca)
+                    for i, pc in enumerate(self.pca_models)
                 ]
             )
         else:
             D = block_diag(
                 *[
                     (1 - self.c[i]) * np.cov(view, rowvar=False)
                     + self.c[i] * np.eye(view.shape[1])
@@ -186,15 +190,15 @@
         if len(views) != 2:
             raise ValueError(
                 f"Model can only be used with two views, but {len(views)} were given. Use MCCA or GCCA instead."
             )
         # Compute the B matrices for each view
         B = [
             (1 - self.c[i]) * pc.explained_variance_ + self.c[i]
-            for i, pc in enumerate(self.pca)
+            for i, pc in enumerate(self.pca_models)
         ]
         C = np.cov(views[0] / np.sqrt(B[0]), views[1] / np.sqrt(B[1]), rowvar=False)[
             0 : views[0].shape[1], views[0].shape[1] :
         ]
         # if views[0].shape[1] <= views[1].shape[1] then return R@R^T else return R^T@R
         if views[0].shape[1] <= views[1].shape[1]:
             self.primary_view = 0
@@ -205,24 +209,24 @@
 
     def D(self, views, **kwargs):
         return None
 
     def _weights(self, eigvals, eigvecs, views):
         B = [
             (1 - self.c[i]) * pc.singular_values_**2 / self.n_samples_ + self.c[i]
-            for i, pc in enumerate(self.pca)
+            for i, pc in enumerate(self.pca_models)
         ]
         C = np.cov(
             views[self.primary_view], views[1 - self.primary_view], rowvar=False
         )[0 : views[self.primary_view].shape[1], views[self.primary_view].shape[1] :]
         self.weights = [None] * 2
         # Compute the weight matrix for primary view
         self.weights[1 - self.primary_view] = (
             # Project view 1 onto its principal components
-            self.pca[1 - self.primary_view].components_.T
+            self.pca_models[1 - self.primary_view].components_.T
             # Scale by the inverse of B[0]
             @ np.diag(1 / B[1 - self.primary_view])
             # Multiply by the cross-covariance matrix
             @ C.T
             # Scale by the inverse of the square root of B[1]
             @ np.diag(1 / np.sqrt(B[self.primary_view]))
             # Multiply by the eigenvectors
@@ -230,15 +234,15 @@
             # Scale by the inverse of the square root of eigenvalues
             / np.sqrt(eigvals)
         )
 
         # Compute the weight matrix for view 2
         self.weights[self.primary_view] = (
             # Project view 2 onto its principal components
-            self.pca[self.primary_view].components_.T
+            self.pca_models[self.primary_view].components_.T
             # Scale by the inverse of the square root of B[1]
             @ np.diag(1 / np.sqrt(B[self.primary_view]))
             # Multiply by the eigenvectors
             @ eigvecs
         )
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_ncca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_ncca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_partialcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_partialcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_pcacca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_pcacca.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Iterable, Union
 
-from sklearn.decomposition import PCA
 import numpy as np
-from sklearn.utils.validation import check_is_fitted
 
 from cca_zoo.classical._mcca import MCCA
 
 
 class PCACCA(MCCA):
     """
     Principal Component Analysis CCA
@@ -34,15 +32,19 @@
         assert percent_variance <= 1, "percent_variance must be less than 1"
         self.percent_variance = percent_variance
 
     def _process_data(self, views, **kwargs):
         views = self._apply_pca(views)
         for i, view in enumerate(views):
             # Keep the components that explain the percentage of variance
-            explained_variance = self.pca[i].explained_variance_ratio_
+            explained_variance = self.pca_models[i].explained_variance_ratio_
             n_components_ = (
                 np.where(np.cumsum(explained_variance) >= self.percent_variance)[0][0]
                 + 1
             )
-            self.pca[i].n_components_ = n_components_
-            self.pca[i].components_ = self.pca[i].components_[:n_components_]
-        return [view[:, : self.pca[i].n_components_] for i, view in enumerate(views)]
+            self.pca_models[i].n_components_ = n_components_
+            self.pca_models[i].components_ = self.pca_models[i].components_[
+                :n_components_
+            ]
+        return [
+            view[:, : self.pca_models[i].n_components_] for i, view in enumerate(views)
+        ]
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_pls.py` & `cca_zoo-2.0.4/cca_zoo/classical/_pls.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_prcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_prcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_search.py` & `cca_zoo-2.0.4/cca_zoo/classical/_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
     Returns
     -------
     updated weights
 
     """
     # First normalise the weights unit length
+    w = w
     w = w / np.linalg.norm(w, 2)
     converged = False
     min_ = 0
     max_ = 10
     current = init
     previous = current
     previous_val = 0
```

### Comparing `cca_zoo-2.0.3/cca_zoo/classical/_tcca.py` & `cca_zoo-2.0.4/cca_zoo/classical/_tcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/data/deep.py` & `cca_zoo-2.0.4/cca_zoo/data/deep.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/data/simulated.py` & `cca_zoo-2.0.4/cca_zoo/data/simulated.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/__init__.py` & `cca_zoo-2.0.4/cca_zoo/deep/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_base.py` & `cca_zoo-2.0.4/cca_zoo/deep/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_barlow_twins.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_ey.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_ey.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_gh.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_gh.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_noi.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_noi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_sdl.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_sdl.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dcca_svd.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dcca_svd.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dgcca.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dgcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_discriminative/_dtcca.py` & `cca_zoo-2.0.4/cca_zoo/deep/_discriminative/_dtcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_generative/_base.py` & `cca_zoo-2.0.4/cca_zoo/deep/_generative/_base.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_generative/_dccae.py` & `cca_zoo-2.0.4/cca_zoo/deep/_generative/_dccae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_generative/_dvcca.py` & `cca_zoo-2.0.4/cca_zoo/deep/_generative/_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/_generative/_splitae.py` & `cca_zoo-2.0.4/cca_zoo/deep/_generative/_splitae.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/architectures.py` & `cca_zoo-2.0.4/cca_zoo/deep/architectures.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/metrics.py` & `cca_zoo-2.0.4/cca_zoo/deep/metrics.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/deep/objectives.py` & `cca_zoo-2.0.4/cca_zoo/deep/objectives.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/model_selection/_search.py` & `cca_zoo-2.0.4/cca_zoo/model_selection/_search.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/model_selection/_validation.py` & `cca_zoo-2.0.4/cca_zoo/model_selection/_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/probabilistic/_probabilisticcca.py` & `cca_zoo-2.0.4/cca_zoo/probabilistic/_probabilisticcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_callbacks.py` & `cca_zoo-2.0.4/cca_zoo/test/test_callbacks.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 X -= X.mean(axis=0)
 Y -= Y.mean(axis=0)
 Z -= Z.mean(axis=0)
 
 
 def test_tracking():
     ey = CCAEY(latent_dimensions=2, track="loss").fit([X, Y])
-    pmd = SCCA_PMD(latent_dimensions=2, track="weights_change", tau=0.5).fit([X, Y])
+    pmd = SCCA_PMD(latent_dimensions=2, track="loss", tau=0.5).fit([X, Y])
     elastic = ElasticCCA(latent_dimensions=2, track="loss").fit([X, Y])
 
 
 def test_convergence():
     elastic = ElasticCCA(
         latent_dimensions=2,
         convergence_checking="loss",
         track="loss",
         alpha=5e-3,
         l1_ratio=0.5,
     ).fit([X, Y])
     pmd = SCCA_PMD(
         latent_dimensions=2,
-        convergence_checking="weights_change",
-        track="weights_change",
+        convergence_checking="loss",
+        track="loss",
         tau=0.5,
     ).fit([X, Y])
```

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_data.py` & `cca_zoo-2.0.4/cca_zoo/test/test_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_deepmodels.py` & `cca_zoo-2.0.4/cca_zoo/test/test_deepmodels.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_kernel.py` & `cca_zoo-2.0.4/cca_zoo/test/test_kernel.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_probabilistic.py` & `cca_zoo-2.0.4/cca_zoo/test/test_probabilistic.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_regularised.py` & `cca_zoo-2.0.4/cca_zoo/test/test_regularised.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from cca_zoo.model_selection import GridSearchCV, RandomizedSearchCV
 from cca_zoo.classical import (
     CCA,
     GCCA,
     GRCCA,
     KCCA,
     MCCA,
-    NCCA,  # SCCA_ADMM,
+    NCCA,
     PLS,
     PRCCA,
     SCCA_IPLS,
     SCCA_PMD,
     AltMaxVar,
     ElasticCCA,
     PartialCCA,
```

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_stochastic.py` & `cca_zoo-2.0.4/cca_zoo/test/test_stochastic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 import pytest
 import scipy.sparse as sp
 from sklearn.utils import check_random_state
 
-from cca_zoo.classical import CCA, PLS, MCCA
+from cca_zoo.classical import CCA, PLS
 
 n = 50
 rng = check_random_state(0)
 X = rng.rand(n, 10)
 Y = rng.rand(n, 11)
 Z = rng.rand(n, 12)
 X_sp = sp.random(n, 10, density=0.5, random_state=rng)
@@ -28,56 +28,76 @@
 
 def scale_objective(obj):
     # log scale the objective if negative, otherwise nan
     obj = np.array(obj)
     return np.sign(obj) * np.log(np.abs(obj) + 1e-10)
 
 
+def scale_transform(model, X, Y):
+    Zx, Zy = model.transform((X, Y))
+    Zx /= np.linalg.norm(model.weights[0], axis=0, keepdims=True)
+    Zy /= np.linalg.norm(model.weights[1], axis=0, keepdims=True)
+    return np.abs(np.cov(Zx, Zy, rowvar=False)[:latent_dims, latent_dims:])
+
+
+def test_batch_pls():
+    pytest.importorskip("torch")
+    from torch import manual_seed
+
+    from cca_zoo.classical import PLSEY, PLSSVD, PLSStochasticPower
+
+    pls = PLS(latent_dimensions=3).fit((X, Y))
+    manual_seed(42)
+    plsey = PLSEY(
+        latent_dimensions=latent_dims,
+        epochs=epochs,
+        batch_size=None,
+        learning_rate=10 * learning_rate,
+        random_state=random_state,
+        track="loss",
+        verbose=False,
+    ).fit((X, Y))
+    pls_score = scale_transform(pls, X, Y)
+    plsey_score = scale_transform(plsey, X, Y)
+    assert np.allclose(pls_score, plsey_score, atol=1e-2)
+
+
 def test_stochastic_pls():
     pytest.importorskip("torch")
     from torch import manual_seed
 
     from cca_zoo.classical import PLSEY, PLSSVD, PLSStochasticPower
 
     pls = PLS(latent_dimensions=3).fit((X, Y))
     manual_seed(42)
     plsey = PLSEY(
         latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
-        track=True,
         verbose=False,
     ).fit((X, Y))
     plssvd = PLSSVD(
         latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
-        track=True,
         verbose=False,
     ).fit((X, Y))
     spls = PLSStochasticPower(
         latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
-        track=True,
         verbose=False,
     ).fit((X, Y))
 
-    def scale_transform(model, X, Y):
-        Zx, Zy = model.transform((X, Y))
-        Zx /= np.linalg.norm(model.weights[0], axis=0, keepdims=True)
-        Zy /= np.linalg.norm(model.weights[1], axis=0, keepdims=True)
-        return np.abs(np.cov(Zx, Zy, rowvar=False)[:latent_dims, latent_dims:])
-
     pls_score = scale_transform(pls, X, Y)
     spls_score = scale_transform(spls, X, Y)
     plsey_score = scale_transform(plsey, X, Y)
     plssvd_score = scale_transform(plssvd, X, Y)
     # check all methods are similar to pls
     assert np.allclose(np.trace(pls_score), np.trace(spls_score), atol=1e-1)
     assert np.allclose(np.trace(pls_score), np.trace(plsey_score), atol=1e-1)
@@ -91,33 +111,30 @@
     cca = CCA(latent_dimensions=3).fit((X, Y))
     ccaey = CCAEY(
         latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
-        track=True,
         verbose=False,
     ).fit((X, Y))
     ccagh = CCAGH(
         latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
-        track=True,
         verbose=False,
     ).fit((X, Y))
     ccasvd = CCASVD(
         latent_dimensions=latent_dims,
         epochs=epochs,
         batch_size=batch_size,
         learning_rate=learning_rate,
         random_state=random_state,
-        track=True,
         verbose=False,
     ).fit((X, Y))
     cca_score = cca.score((X, Y))
     ccaey_score = ccaey.score((X, Y))
     ccagh_score = ccagh.score((X, Y))
     ccasvd_score = ccasvd.score((X, Y))
     # check all methods are similar to cca
```

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_unregularized.py` & `cca_zoo-2.0.4/cca_zoo/test/test_unregularized.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/test/test_utils.py` & `cca_zoo-2.0.4/cca_zoo/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo/utils/check_values.py` & `cca_zoo-2.0.4/cca_zoo/utils/check_values.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,23 +17,14 @@
         raise ValueError(
             f"number of views passed should match number of parameter {parameter_name}"
             f"len(views)={n_views} and "
             f"len({parameter_name})={len(parameter)}"
         )
 
 
-def _check_converged_weights(weights, view_index):
-    """check the converged weights are not zero."""
-    if np.linalg.norm(weights) <= 0:
-        warnings.warn(
-            f"All result weights are zero in view {view_index}. "
-            "Try less regularisation or another initialisation"
-        )
-
-
 def _check_Parikh2014(mus, lams, views):
     """Return index of the view which the data not matching the condition
     documented in Parikh 2014."""
     failed_check = [
         i
         for i, (mu, lam, view) in enumerate(zip(mus, lams, views))
         if mu < lam / np.linalg.norm(view) ** 2
```

### Comparing `cca_zoo-2.0.3/cca_zoo/visualisation/plotting.py` & `cca_zoo-2.0.4/cca_zoo/visualisation/plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/cca_zoo.egg-info/PKG-INFO` & `cca_zoo-2.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cca-zoo
-Version: 2.0.3
+Name: cca_zoo
+Version: 2.0.4
 Summary: Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework
 Home-page: https://github.com/jameschapman19/cca_zoo
 Author: jameschapman
 Author-email: james.chapman.19@ucl.ac.uk
 License: MIT
 Description: [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5748062.svg)](https://doi.org/10.5281/zenodo.4382739)
         [![codecov](https://codecov.io/gh/jameschapman19/cca_zoo/branch/main/graph/badge.svg?token=JHG9VUB0L8)](https://codecov.io/gh/jameschapman19/cca_zoo)
```

### Comparing `cca_zoo-2.0.3/cca_zoo.egg-info/SOURCES.txt` & `cca_zoo-2.0.4/cca_zoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/__init__.py` & `cca_zoo-2.0.4/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_dcca.py` & `cca_zoo-2.0.4/examples/plot_dcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_dcca_custom_data.py` & `cca_zoo-2.0.4/examples/plot_dcca_custom_data.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_dcca_multi.py` & `cca_zoo-2.0.4/examples/plot_dcca_multi.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_dvcca.py` & `cca_zoo-2.0.4/examples/plot_dvcca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_hyperparameter_selection.py` & `cca_zoo-2.0.4/examples/plot_hyperparameter_selection.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_kernel_cca.py` & `cca_zoo-2.0.4/examples/plot_kernel_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_many_views.py` & `cca_zoo-2.0.4/examples/plot_many_views.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_plotting.py` & `cca_zoo-2.0.4/examples/plot_plotting.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_sparse_cca.py` & `cca_zoo-2.0.4/examples/plot_sparse_cca.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/examples/plot_validation.py` & `cca_zoo-2.0.4/examples/plot_validation.py`

 * *Files identical despite different names*

### Comparing `cca_zoo-2.0.3/setup.py` & `cca_zoo-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "deep": ["torch", "torchvision", "pytorch-lightning"],
     "probabilistic": ["jax", "numpyro", "arviz"],
 }
 EXTRA_PACKAGES["all"] = EXTRA_PACKAGES["deep"] + EXTRA_PACKAGES["probabilistic"]
 
 setup(
     name="cca_zoo",
-    version="2.0.3",
+    version="2.0.4",
     include_package_data=True,
     keywords="cca",
     packages=find_packages(),
     url="https://github.com/jameschapman19/cca_zoo",
     license="MIT",
     author="jameschapman",
     description=(
```

