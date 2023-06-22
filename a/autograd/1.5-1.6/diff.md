# Comparing `tmp/autograd-1.5.tar.gz` & `tmp/autograd-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autograd-1.5.tar", last modified: Thu Sep 29 07:07:31 2022, max compression
+gzip compressed data, was "autograd-1.6.tar", last modified: Thu Jun 22 12:40:43 2023, max compression
```

## Comparing `autograd-1.5.tar` & `autograd-1.6.tar`

### file list

```diff
@@ -1,55 +1,79 @@
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2022-09-29 07:07:31.772336 autograd-1.5/
--rw-r--r--   0 jamietownsend   (501) staff       (20)       41 2020-03-21 18:01:53.000000 autograd-1.5/MANIFEST.in
--rw-r--r--   0 jamietownsend   (501) staff       (20)      640 2022-09-29 07:07:31.772657 autograd-1.5/PKG-INFO
--rw-r--r--   0 jamietownsend   (501) staff       (20)     4443 2020-03-21 18:01:53.000000 autograd-1.5/README.md
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2022-09-29 07:07:31.730227 autograd-1.5/autograd/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      504 2020-03-21 18:01:53.000000 autograd-1.5/autograd/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     6110 2020-03-21 18:01:53.000000 autograd-1.5/autograd/builtins.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    12235 2020-11-14 15:24:12.000000 autograd-1.5/autograd/core.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     8515 2022-06-15 10:01:07.000000 autograd-1.5/autograd/differential_operators.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      304 2020-03-21 18:01:53.000000 autograd-1.5/autograd/extend.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2022-09-29 07:07:31.737337 autograd-1.5/autograd/misc/
--rw-r--r--   0 jamietownsend   (501) staff       (20)       62 2020-03-21 18:01:53.000000 autograd-1.5/autograd/misc/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      771 2020-03-21 18:01:53.000000 autograd-1.5/autograd/misc/fixed_points.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1120 2020-03-21 18:01:53.000000 autograd-1.5/autograd/misc/flatten.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2757 2020-03-21 18:01:53.000000 autograd-1.5/autograd/misc/optimizers.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2200 2020-03-21 18:01:53.000000 autograd-1.5/autograd/misc/tracers.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2022-09-29 07:07:31.750859 autograd-1.5/autograd/numpy/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      232 2020-03-21 18:01:53.000000 autograd-1.5/autograd/numpy/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5250 2020-03-21 18:01:53.000000 autograd-1.5/autograd/numpy/fft.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    11352 2022-09-29 07:03:46.000000 autograd-1.5/autograd/numpy/linalg.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     3124 2020-03-21 18:01:53.000000 autograd-1.5/autograd/numpy/numpy_boxes.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    10766 2020-03-21 18:01:53.000000 autograd-1.5/autograd/numpy/numpy_jvps.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)    32566 2020-03-21 18:01:53.000000 autograd-1.5/autograd/numpy/numpy_vjps.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2004 2020-03-21 18:01:53.000000 autograd-1.5/autograd/numpy/numpy_vspaces.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5459 2021-03-03 09:26:31.000000 autograd-1.5/autograd/numpy/numpy_wrapper.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      149 2020-03-21 18:01:53.000000 autograd-1.5/autograd/numpy/random.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2022-09-29 07:07:31.759670 autograd-1.5/autograd/scipy/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      183 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2867 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/integrate.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2363 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/linalg.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      168 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/misc.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5924 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/signal.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     5135 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/special.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2022-09-29 07:07:31.771401 autograd-1.5/autograd/scipy/stats/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      391 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/__init__.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1332 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/beta.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      809 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/chi2.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      772 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/dirichlet.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      987 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/gamma.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2509 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/multivariate_normal.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2758 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/norm.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)      715 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/poisson.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2670 2020-03-21 18:01:53.000000 autograd-1.5/autograd/scipy/stats/t.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     2881 2020-03-21 18:01:53.000000 autograd-1.5/autograd/test_util.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     3951 2020-03-21 18:01:53.000000 autograd-1.5/autograd/tracer.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1482 2020-03-21 18:01:53.000000 autograd-1.5/autograd/util.py
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1581 2020-03-21 18:01:53.000000 autograd-1.5/autograd/wrap_util.py
-drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2022-09-29 07:07:31.733193 autograd-1.5/autograd.egg-info/
--rw-r--r--   0 jamietownsend   (501) staff       (20)      640 2022-09-29 07:07:31.000000 autograd-1.5/autograd.egg-info/PKG-INFO
--rw-r--r--   0 jamietownsend   (501) staff       (20)     1217 2022-09-29 07:07:31.000000 autograd-1.5/autograd.egg-info/SOURCES.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)        1 2022-09-29 07:07:31.000000 autograd-1.5/autograd.egg-info/dependency_links.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)       27 2022-09-29 07:07:31.000000 autograd-1.5/autograd.egg-info/requires.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)        9 2022-09-29 07:07:31.000000 autograd-1.5/autograd.egg-info/top_level.txt
--rw-r--r--   0 jamietownsend   (501) staff       (20)       79 2022-09-29 07:07:31.773697 autograd-1.5/setup.cfg
--rw-r--r--   0 jamietownsend   (501) staff       (20)      950 2022-09-29 07:04:08.000000 autograd-1.5/setup.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.498795 autograd-1.6/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       41 2020-03-21 18:01:53.000000 autograd-1.6/MANIFEST.in
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      640 2023-06-22 12:40:43.499024 autograd-1.6/PKG-INFO
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     4443 2020-03-21 18:01:53.000000 autograd-1.6/README.md
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.342162 autograd-1.6/autograd/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      504 2020-03-21 18:01:53.000000 autograd-1.6/autograd/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     6328 2023-06-22 12:39:21.000000 autograd-1.6/autograd/builtins.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    12235 2023-06-22 12:38:25.000000 autograd-1.6/autograd/core.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     8515 2022-06-15 10:01:07.000000 autograd-1.6/autograd/differential_operators.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      304 2020-03-21 18:01:53.000000 autograd-1.6/autograd/extend.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.367648 autograd-1.6/autograd/misc/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       62 2020-03-21 18:01:53.000000 autograd-1.6/autograd/misc/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      771 2020-03-21 18:01:53.000000 autograd-1.6/autograd/misc/fixed_points.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1120 2020-03-21 18:01:53.000000 autograd-1.6/autograd/misc/flatten.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2757 2020-03-21 18:01:53.000000 autograd-1.6/autograd/misc/optimizers.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2200 2020-03-21 18:01:53.000000 autograd-1.6/autograd/misc/tracers.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.398344 autograd-1.6/autograd/numpy/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      232 2020-03-21 18:01:53.000000 autograd-1.6/autograd/numpy/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5250 2020-03-21 18:01:53.000000 autograd-1.6/autograd/numpy/fft.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    11352 2022-09-29 07:03:46.000000 autograd-1.6/autograd/numpy/linalg.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3493 2023-06-22 12:39:21.000000 autograd-1.6/autograd/numpy/numpy_boxes.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    10766 2020-03-21 18:01:53.000000 autograd-1.6/autograd/numpy/numpy_jvps.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    32566 2020-03-21 18:01:53.000000 autograd-1.6/autograd/numpy/numpy_vjps.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2843 2023-06-22 12:39:21.000000 autograd-1.6/autograd/numpy/numpy_vspaces.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5459 2021-03-03 09:26:31.000000 autograd-1.6/autograd/numpy/numpy_wrapper.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      149 2020-03-21 18:01:53.000000 autograd-1.6/autograd/numpy/random.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.416013 autograd-1.6/autograd/scipy/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      183 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2867 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/integrate.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2363 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/linalg.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      168 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/misc.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5924 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/signal.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5135 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/special.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.442973 autograd-1.6/autograd/scipy/stats/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      391 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/__init__.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1332 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/beta.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      809 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/chi2.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      772 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/dirichlet.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      987 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/gamma.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2509 2023-03-22 11:58:08.000000 autograd-1.6/autograd/scipy/stats/multivariate_normal.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2758 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/norm.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      715 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/poisson.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2670 2020-03-21 18:01:53.000000 autograd-1.6/autograd/scipy/stats/t.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2881 2020-03-21 18:01:53.000000 autograd-1.6/autograd/test_util.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3951 2023-06-22 12:38:25.000000 autograd-1.6/autograd/tracer.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1482 2020-03-21 18:01:53.000000 autograd-1.6/autograd/util.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1581 2020-03-21 18:01:53.000000 autograd-1.6/autograd/wrap_util.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.352763 autograd-1.6/autograd.egg-info/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      640 2023-06-22 12:40:43.000000 autograd-1.6/autograd.egg-info/PKG-INFO
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1710 2023-06-22 12:40:43.000000 autograd-1.6/autograd.egg-info/SOURCES.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)        1 2023-06-22 12:40:43.000000 autograd-1.6/autograd.egg-info/dependency_links.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       27 2023-06-22 12:40:43.000000 autograd-1.6/autograd.egg-info/requires.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)        9 2023-06-22 12:40:43.000000 autograd-1.6/autograd.egg-info/top_level.txt
+-rw-r--r--   0 jamietownsend   (501) staff       (20)       79 2023-06-22 12:40:43.499963 autograd-1.6/setup.cfg
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      950 2023-06-22 12:39:28.000000 autograd-1.6/setup.py
+drwxr-xr-x   0 jamietownsend   (501) staff       (20)        0 2023-06-22 12:40:43.497798 autograd-1.6/tests/
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3217 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_binary_ops.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      644 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_builtins.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1151 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_complex.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1653 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_core.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     3599 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_dict.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      860 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_direct.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     6104 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_fft.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     4963 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_graphs.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1444 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_jacobian.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    11222 2023-03-22 10:31:09.000000 autograd-1.6/tests/test_linalg.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1842 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_list.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1563 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_logic.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     2970 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_misc.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    17858 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_numpy.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      144 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_performance.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     4514 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_scalar_ops.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    14435 2023-06-22 10:48:10.000000 autograd-1.6/tests/test_scipy.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    15326 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_systematic.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      785 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_tests.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)      515 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_truediv.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     1791 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_tuple.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)     5016 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_vspaces.py
+-rw-r--r--   0 jamietownsend   (501) staff       (20)    10495 2020-03-21 18:01:53.000000 autograd-1.6/tests/test_wrappers.py
```

### Comparing `autograd-1.5/PKG-INFO` & `autograd-1.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autograd
-Version: 1.5
+Version: 1.6
 Summary: Efficiently computes derivatives of numpy code.
 Home-page: https://github.com/HIPS/autograd
 Author: Dougal Maclaurin and David Duvenaud and Matthew Johnson
 Author-email: maclaurin@physics.harvard.edu, duvenaud@cs.toronto.edu, mattjj@csail.mit.edu
 License: MIT
 Keywords: Automatic differentiation,backpropagation,gradients,machine learning,optimization,neural networks,Python,Numpy,Scipy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autograd-1.5/README.md` & `autograd-1.6/README.md`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/builtins.py` & `autograd-1.6/autograd/builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,7 +163,13 @@
         d = dict(xs.items())
         d[idx] = x
         return d
 
 ListVSpace.register(list_)
 TupleVSpace.register(tuple_)
 DictVSpace.register(dict_)
+
+class NamedTupleVSpace(SequenceVSpace):
+    def _map(self, f, *args):
+        return self.seq_type(*map(f, self.shape, *args))
+    def _subval(self, xs, idx, x):
+        return self.seq_type(*subvals(xs, [(idx, x)]))
```

### Comparing `autograd-1.5/autograd/core.py` & `autograd-1.6/autograd/core.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/differential_operators.py` & `autograd-1.6/autograd/differential_operators.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/misc/fixed_points.py` & `autograd-1.6/autograd/misc/fixed_points.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/misc/flatten.py` & `autograd-1.6/autograd/misc/flatten.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/misc/optimizers.py` & `autograd-1.6/autograd/misc/optimizers.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/misc/tracers.py` & `autograd-1.6/autograd/misc/tracers.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/numpy/fft.py` & `autograd-1.6/autograd/numpy/fft.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/numpy/linalg.py` & `autograd-1.6/autograd/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/numpy/numpy_boxes.py` & `autograd-1.6/autograd/numpy/numpy_boxes.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import absolute_import
 import numpy as np
 from autograd.extend import Box, primitive
+from autograd.builtins import SequenceBox
 from . import numpy_wrapper as anp
 
 Box.__array_priority__ = 90.0
 
 class ArrayBox(Box):
     __slots__ = []
     __array_priority__ = 100.0
@@ -44,23 +45,30 @@
     def __ge__(self, other): return anp.greater_equal(self, other)
     def __lt__(self, other): return anp.less(self, other)
     def __le__(self, other): return anp.less_equal(self, other)
     def __abs__(self): return anp.abs(self)
     def __hash__(self): return id(self)
 
 ArrayBox.register(np.ndarray)
-for type_ in [float, np.float64, np.float32, np.float16,
-              complex, np.complex64, np.complex128]:
+for type_ in [float, np.float128, np.float64, np.float32, np.float16,
+              complex, np.complex64, np.complex128, np.complex256]:
     ArrayBox.register(type_)
 
 # These numpy.ndarray methods are just refs to an equivalent numpy function
 nondiff_methods = ['all', 'any', 'argmax', 'argmin', 'argpartition',
                    'argsort', 'nonzero', 'searchsorted', 'round']
 diff_methods = ['clip', 'compress', 'cumprod', 'cumsum', 'diagonal',
                 'max', 'mean', 'min', 'prod', 'ptp', 'ravel', 'repeat',
                 'reshape', 'squeeze', 'std', 'sum', 'swapaxes', 'take',
                 'trace', 'transpose', 'var']
 for method_name in nondiff_methods + diff_methods:
     setattr(ArrayBox, method_name, anp.__dict__[method_name])
 
 # Flatten has no function, only a method.
 setattr(ArrayBox, 'flatten', anp.__dict__['ravel'])
+
+if np.__version__ >= '1.25':
+    SequenceBox.register(np.linalg.linalg.EigResult)
+    SequenceBox.register(np.linalg.linalg.EighResult)
+    SequenceBox.register(np.linalg.linalg.QRResult)
+    SequenceBox.register(np.linalg.linalg.SlogdetResult)
+    SequenceBox.register(np.linalg.linalg.SVDResult)
```

### Comparing `autograd-1.5/autograd/numpy/numpy_jvps.py` & `autograd-1.6/autograd/numpy/numpy_jvps.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/numpy/numpy_vjps.py` & `autograd-1.6/autograd/numpy/numpy_vjps.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/numpy/numpy_wrapper.py` & `autograd-1.6/autograd/numpy/numpy_wrapper.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/integrate.py` & `autograd-1.6/autograd/scipy/integrate.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/linalg.py` & `autograd-1.6/autograd/scipy/linalg.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/signal.py` & `autograd-1.6/autograd/scipy/signal.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/special.py` & `autograd-1.6/autograd/scipy/special.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/beta.py` & `autograd-1.6/autograd/scipy/stats/beta.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/chi2.py` & `autograd-1.6/autograd/scipy/stats/chi2.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/dirichlet.py` & `autograd-1.6/autograd/scipy/stats/dirichlet.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/gamma.py` & `autograd-1.6/autograd/scipy/stats/gamma.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/multivariate_normal.py` & `autograd-1.6/autograd/scipy/stats/multivariate_normal.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/norm.py` & `autograd-1.6/autograd/scipy/stats/norm.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/poisson.py` & `autograd-1.6/autograd/scipy/stats/poisson.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/scipy/stats/t.py` & `autograd-1.6/autograd/scipy/stats/t.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/test_util.py` & `autograd-1.6/autograd/test_util.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/tracer.py` & `autograd-1.6/autograd/tracer.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/util.py` & `autograd-1.6/autograd/util.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd/wrap_util.py` & `autograd-1.6/autograd/wrap_util.py`

 * *Files identical despite different names*

### Comparing `autograd-1.5/autograd.egg-info/PKG-INFO` & `autograd-1.6/autograd.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autograd
-Version: 1.5
+Version: 1.6
 Summary: Efficiently computes derivatives of numpy code.
 Home-page: https://github.com/HIPS/autograd
 Author: Dougal Maclaurin and David Duvenaud and Matthew Johnson
 Author-email: maclaurin@physics.harvard.edu, duvenaud@cs.toronto.edu, mattjj@csail.mit.edu
 License: MIT
 Keywords: Automatic differentiation,backpropagation,gradients,machine learning,optimization,neural networks,Python,Numpy,Scipy
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autograd-1.5/autograd.egg-info/SOURCES.txt` & `autograd-1.6/autograd.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -40,8 +40,31 @@
 autograd/scipy/stats/beta.py
 autograd/scipy/stats/chi2.py
 autograd/scipy/stats/dirichlet.py
 autograd/scipy/stats/gamma.py
 autograd/scipy/stats/multivariate_normal.py
 autograd/scipy/stats/norm.py
 autograd/scipy/stats/poisson.py
-autograd/scipy/stats/t.py
+autograd/scipy/stats/t.py
+tests/test_binary_ops.py
+tests/test_builtins.py
+tests/test_complex.py
+tests/test_core.py
+tests/test_dict.py
+tests/test_direct.py
+tests/test_fft.py
+tests/test_graphs.py
+tests/test_jacobian.py
+tests/test_linalg.py
+tests/test_list.py
+tests/test_logic.py
+tests/test_misc.py
+tests/test_numpy.py
+tests/test_performance.py
+tests/test_scalar_ops.py
+tests/test_scipy.py
+tests/test_systematic.py
+tests/test_tests.py
+tests/test_truediv.py
+tests/test_tuple.py
+tests/test_vspaces.py
+tests/test_wrappers.py
```

### Comparing `autograd-1.5/setup.py` & `autograd-1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='autograd',
-    version='1.5',
+    version='1.6',
     description='Efficiently computes derivatives of numpy code.',
     author='Dougal Maclaurin and David Duvenaud and Matthew Johnson',
     author_email="maclaurin@physics.harvard.edu, duvenaud@cs.toronto.edu, mattjj@csail.mit.edu",
     packages=['autograd', 'autograd.numpy', 'autograd.scipy', 'autograd.scipy.stats', 'autograd.misc'],
     install_requires=['numpy>=1.12', 'future>=0.15.2'],
     keywords=['Automatic differentiation', 'backpropagation', 'gradients',
               'machine learning', 'optimization', 'neural networks',
```

