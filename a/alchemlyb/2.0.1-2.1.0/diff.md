# Comparing `tmp/alchemlyb-2.0.1.tar.gz` & `tmp/alchemlyb-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alchemlyb-2.0.1.tar", last modified: Fri Apr  7 18:11:16 2023, max compression
+gzip compressed data, was "alchemlyb-2.1.0.tar", last modified: Thu Jun 22 16:34:11 2023, max compression
```

## Comparing `alchemlyb-2.0.1.tar` & `alchemlyb-2.1.0.tar`

### file list

```diff
@@ -1,72 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1758 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.931970 alchemlyb-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/src/alchemlyb/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/src/alchemlyb/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.935970 alchemlyb-2.0.1/src/alchemlyb/convergence/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/convergence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/convergence/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/convergence/pade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.935970 alchemlyb-2.0.1/src/alchemlyb/estimators/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/estimators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/estimators/bar_.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/estimators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/estimators/mbar_.py
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/estimators/ti_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.935970 alchemlyb-2.0.1/src/alchemlyb/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15383 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/parsing/amber.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/parsing/gmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/parsing/gomc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17782 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/parsing/namd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/parsing/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.935970 alchemlyb-2.0.1/src/alchemlyb/postprocessors/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/postprocessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/postprocessors/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.935970 alchemlyb-2.0.1/src/alchemlyb/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19392 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/preprocessing/subsampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/src/alchemlyb/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6589 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/src/alchemlyb/tests/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_amber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_gmx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_gomc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_namd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_fep_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)    18260 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_ti_estimators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_visualisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    15033 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/tests/test_workflow_ABFE.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/src/alchemlyb/visualisation/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/visualisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/visualisation/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/visualisation/dF_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/visualisation/mbar_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/visualisation/ti_dhdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.939970 alchemlyb-2.0.1/src/alchemlyb/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32537 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/workflows/abfe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/src/alchemlyb/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 18:11:16.935970 alchemlyb-2.0.1/src/alchemlyb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-04-07 18:11:16.000000 alchemlyb-2.0.1/src/alchemlyb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-04-07 18:11:16.000000 alchemlyb-2.0.1/src/alchemlyb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 18:11:16.000000 alchemlyb-2.0.1/src/alchemlyb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-07 18:11:16.000000 alchemlyb-2.0.1/src/alchemlyb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-07 18:11:16.000000 alchemlyb-2.0.1/src/alchemlyb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    68573 2023-04-07 18:10:48.000000 alchemlyb-2.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1795 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.828814 alchemlyb-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/src/alchemlyb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/src/alchemlyb/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/convergence/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/convergence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/convergence/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/convergence/pade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/estimators/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/bar_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/mbar_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/estimators/ti_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/amber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/gmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/gomc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17739 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/namd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/parsing/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb/postprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/postprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/postprocessors/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19870 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/preprocessing/subsampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6829 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_amber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9633 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gomc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14650 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_namd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_fep_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19051 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_ti_estimators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17238 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow_ABFE.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.836814 alchemlyb-2.1.0/src/alchemlyb/visualisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8391 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/dF_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/mbar_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/visualisation/ti_dhdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.840813 alchemlyb-2.1.0/src/alchemlyb/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33217 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/workflows/abfe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/src/alchemlyb/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:34:11.832814 alchemlyb-2.1.0/src/alchemlyb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 16:34:11.000000 alchemlyb-2.1.0/src/alchemlyb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68573 2023-06-22 16:33:34.000000 alchemlyb-2.1.0/versioneer.py
```

### Comparing `alchemlyb-2.0.1/AUTHORS` & `alchemlyb-2.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/LICENSE` & `alchemlyb-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/PKG-INFO` & `alchemlyb-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemlyb
-Version: 2.0.1
+Version: 2.1.0
 Summary: the simple alchemistry library
 Author: David Dotson
 Author-email: dotsdl@gmail.com
 Maintainer: Oliver Beckstein
 Maintainer-email: orbeckst@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alchemlyb-2.0.1/README.rst` & `alchemlyb-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/setup.py` & `alchemlyb-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,9 +48,11 @@
     install_requires=[
         "numpy",
         "pandas>=1.4",
         "pymbar>=4",
         "scipy",
         "scikit-learn",
         "matplotlib",
+        "loguru",
+        "pyarrow",
     ],
 )
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/__init__.py` & `alchemlyb-2.1.0/src/alchemlyb/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/convergence/convergence.py` & `alchemlyb-2.1.0/src/alchemlyb/convergence/convergence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Functions for assessing convergence of free energy estimates and raw data."""
 
-import logging
 from warnings import warn
 
 import numpy as np
 import pandas as pd
+from loguru import logger
 
 from .. import concat
 from ..estimators import BAR, TI, MBAR, FEP_ESTIMATORS, TI_ESTIMATORS
 from ..postprocessors.units import to_kT
 
 estimators_dispatch = {"BAR": BAR, "TI": TI, "MBAR": MBAR}
 
@@ -61,15 +61,14 @@
        The ``estimator`` accepts uppercase input.
        The default for using ``estimator='MBAR'`` was changed from
        :class:`~alchemlyb.estimators.MBAR` to :class:`~alchemlyb.estimators.AutoMBAR`.
     .. versionchanged:: 2.0.0
        Use pymbar.MBAR instead of the AutoMBAR option.
 
     """
-    logger = logging.getLogger("alchemlyb.convergence." "forward_backward_convergence")
     logger.info("Start convergence analysis.")
     logger.info("Check data availability.")
     if estimator.upper() != estimator:
         warn(
             "Using lower-case strings for the 'estimator' kwarg in "
             "convergence.forward_backward_convergence() is deprecated in "
             "1.0.0 and only upper case will be accepted in 2.0.0",
@@ -331,15 +330,14 @@
 
     .. versionadded:: 1.0.0
 
     .. _`equation 18`:
        https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8397498/#FD18
 
     """
-    logger = logging.getLogger("alchemlyb.convergence.A_c")
     n_R_c = len(series_list)
     R_c_list = [fwdrev_cumavg_Rc(series, precision, tol)[0] for series in series_list]
     logger.info(f"R_c list: {R_c_list}")
     # Integrate the R_c_list <= R_c over the range of 0 to 1
     array_01 = np.hstack((R_c_list, [0, 1]))
     sorted_array = np.sort(np.unique(array_01))
     result = 0
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/estimators/bar_.py` & `alchemlyb-2.1.0/src/alchemlyb/estimators/bar_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/estimators/ti_.py` & `alchemlyb-2.1.0/src/alchemlyb/estimators/ti_.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/parsing/__init__.py` & `alchemlyb-2.1.0/src/alchemlyb/parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/parsing/amber.py` & `alchemlyb-2.1.0/src/alchemlyb/parsing/amber.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,24 @@
 
 .. versionchanged:: 1.0.0
     Now raises :exc:`ValueError` when an invalid file is given to the parser.
     Now raises :exc:`ValueError` when inconsistency in MBAR states/data is found.
 
 """
 
-import logging
 import re
 
 import numpy as np
 import pandas as pd
+from loguru import logger
 
 from . import _init_attrs_dict
 from .util import anyopen
 from ..postprocessors.units import R_kJmol, kJ2kcal
 
-logger = logging.getLogger("alchemlyb.parsers.Amber")
-
 k_b = R_kJmol * kJ2kcal
 
 _FP_RE = r"[+-]?(\d+(\.\d*)?|\.\d+)([eE][+-]?\d+)?"
 
 
 def convert_to_pandas(file_datum):
     """Convert the data structure from numpy to pandas format"""
@@ -69,15 +67,15 @@
 
     def __init__(self, filename):
         """Opens a file according to its file type."""
         self.filename = filename
         try:
             self.fileh = anyopen(self.filename, "r")
         except:
-            logger.exception("Cannot open file %s", filename)
+            logger.exception("Cannot open file {}", filename)
             raise
         self.lineno = 0
 
     def skip_lines(self, nlines):
         """Skip a given number of lines."""
         lineno = 0
         for line in self:
@@ -196,34 +194,34 @@
     """
 
     file_datum = FEData()
     with SectionParser(outfile) as secp:
         line = secp.skip_lines(5)
 
         if not line:
-            logger.error("The file %s does not contain any data, it's empty.", outfile)
+            logger.error("The file {} does not contain any data, it's empty.", outfile)
             raise ValueError(f"file {outfile} does not contain any data.")
 
         if not secp.skip_after("^   2.  CONTROL  DATA  FOR  THE  RUN"):
-            logger.error('No "CONTROL DATA" section found in file %s.', outfile)
+            logger.error('No "CONTROL DATA" section found in file {}.', outfile)
             raise ValueError(f'no "CONTROL DATA" section found in file {outfile}')
 
         (ntpr,) = secp.extract_section("^Nature and format of output:", "^$", ["ntpr"])
         nstlim, dt = secp.extract_section("Molecular dynamics:", "^$", ["nstlim", "dt"])
         (T,) = secp.extract_section("temperature regulation:", "^$", ["temp0"])
         if not T:
-            logger.error('No valid "temp0" record found in file %s.', outfile)
+            logger.error('No valid "temp0" record found in file {}.', outfile)
             raise ValueError(f'no valid "temp0" record found in file {outfile}')
 
         (clambda,) = secp.extract_section(
             "^Free energy options:", "^$", ["clambda"], "^---"
         )
         if clambda is None:
             logger.error(
-                'No free energy section found in file %s, "clambda" was None.', outfile
+                'No free energy section found in file {}, "clambda" was None.', outfile
             )
             raise ValueError(f"no free energy section found in file {outfile}")
 
         mbar_ndata = 0
         have_mbar, mbar_ndata, mbar_states = secp.extract_section(
             "^FEP MBAR options:",
             "^$",
@@ -234,50 +232,50 @@
             mbar_ndata = int(nstlim / mbar_ndata)
             mbar_lambdas = _process_mbar_lambdas(secp)
             file_datum.mbar_lambdas = mbar_lambdas
             clambda_str = f"{clambda:6.4f}"
 
             if clambda_str not in mbar_lambdas:
                 logger.warning(
-                    "WARNING: lamba %s not contained in set of "
-                    "MBAR lambas: %s\nNot using MBAR.",
+                    "WARNING: lamba {} not contained in set of "
+                    "MBAR lambas: {}\nNot using MBAR.",
                     clambda_str,
                     ", ".join(mbar_lambdas),
                 )
                 have_mbar = False
             else:
                 mbar_nlambda = len(mbar_lambdas)
                 if mbar_nlambda != mbar_states:
                     logger.error(
-                        "the number of lambda windows read (%s)"
-                        "is different from what expected (%d)",
+                        "the number of lambda windows read ({})"
+                        "is different from what expected ({})",
                         ",".join(mbar_lambdas),
                         mbar_states,
                     )
                     raise ValueError(
                         f"the number of lambda windows read ({mbar_nlambda})"
                         f" is different from what expected ({mbar_states})"
                     )
                 mbar_lambda_idx = mbar_lambdas.index(clambda_str)
                 file_datum.mbar_lambda_idx = mbar_lambda_idx
 
                 for _ in range(mbar_nlambda):
                     file_datum.mbar_energies.append([])
 
         if not secp.skip_after("^   3.  ATOMIC "):
-            logger.error('No "ATOMIC" section found in the file %s.', outfile)
+            logger.error('No "ATOMIC" section found in the file {}.', outfile)
             raise ValueError(f'no "ATOMIC" section found in file {outfile}')
 
         (t0,) = secp.extract_section("^ begin time", "^$", ["coords"])
         if t0 is None:
-            logger.error("No starting simulation time in file %s.", outfile)
+            logger.error("No starting simulation time in file {}.", outfile)
             raise ValueError(f"No starting simulation time in file {outfile}")
 
         if not secp.skip_after("^   4.  RESULTS"):
-            logger.error('No "RESULTS" section found in the file %s.', outfile)
+            logger.error('No "RESULTS" section found in the file {}.', outfile)
             raise ValueError(f'no "RESULTS" section found in file {outfile}')
 
     file_datum.clambda = clambda
     file_datum.t0 = t0
     file_datum.dt = dt
     file_datum.ntpr = ntpr
     file_datum.T = T
@@ -330,49 +328,56 @@
             if "      A V E R A G E S   O V E R" in line:
                 _ = secp.skip_after("^|=========================================")
             elif line.startswith(" NSTEP"):
                 nstep, dvdl = secp.extract_section(
                     "^ NSTEP", "^ ---", ["NSTEP", "DV/DL"], extra=line
                 )
                 if nstep != old_nstep and dvdl is not None and nstep is not None:
+                    if finished:
+                        raise ValueError(
+                            "TI Energy detected after the TIMINGS section. Did you concatenate the output file?"
+                        )
                     file_datum.gradients.append(dvdl)
                     nensec += 1
                     old_nstep = nstep
             elif line.startswith("MBAR Energy analysis") and file_datum.have_mbar:
+                if finished:
+                    raise ValueError(
+                        "MBAR Energy detected after the TIMINGS section. Did you concatenate the output file?"
+                    )
                 mbar = secp.extract_section(
                     "^MBAR", "^ ---", file_datum.mbar_lambdas, extra=line
                 )
 
                 if None in mbar:
                     msg = "Something strange parsing the following MBAR section."
                     msg += "\nMaybe the mbar_lambda values are incorrect?"
-                    logger.error("%s\n%s", msg, mbar)
+                    logger.error("{}\n{}", msg, mbar)
                     raise ValueError(msg)
 
                 reference_energy = mbar[file_datum.mbar_lambda_idx]
                 for lmbda, energy in enumerate(mbar):
                     if energy > 0.0:
                         high_E_cnt += 1
 
                     file_datum.mbar_energies[lmbda].append(
                         beta * (energy - reference_energy)
                     )
             elif line == "   5.  TIMINGS\n":
                 finished = True
-                break
 
         if high_E_cnt:
             logger.warning(
-                "%i MBAR energ%s > 0.0 kcal/mol",
+                "{} MBAR energ{} > 0.0 kcal/mol",
                 high_E_cnt,
                 "ies are" if high_E_cnt > 1 else "y is",
             )
 
     if not finished:
-        logger.warning("WARNING: file %s is a prematurely terminated run", outfile)
+        logger.warning("WARNING: file {} is a prematurely terminated run", outfile)
 
     if file_datum.have_mbar:
         mbar_time = [
             file_datum.t0 + (frame_index + 1) * file_datum.dt * file_datum.ntpr
             for frame_index in range(len(file_datum.mbar_energies[0]))
         ]
 
@@ -385,18 +390,18 @@
             ),
         ).T
     else:
         logger.info('WARNING: No MBAR energies found! "u_nk" entry will be None')
         mbar_df = None
 
     if not nensec:
-        logger.warning("WARNING: File %s does not contain any dV/dl data", outfile)
+        logger.warning("WARNING: File {} does not contain any dV/dl data", outfile)
         dHdl_df = None
     else:
-        logger.info("Read %s dV/dl data points in file %s", nensec, outfile)
+        logger.info("Read {} dV/dl data points in file {}", nensec, outfile)
         dHdl_df = convert_to_pandas(file_datum)
         dHdl_df["dHdl"] *= beta
 
     return {"u_nk": mbar_df, "dHdl": dHdl_df}
 
 
 def extract_dHdl(outfile, T):
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/parsing/gmx.py` & `alchemlyb-2.1.0/src/alchemlyb/parsing/gmx.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/parsing/gomc.py` & `alchemlyb-2.1.0/src/alchemlyb/parsing/gomc.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/parsing/namd.py` & `alchemlyb-2.1.0/src/alchemlyb/parsing/namd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """Parsers for extracting alchemical data from `NAMD <http://www.ks.uiuc.edu/Research/namd/>`_ output files.
 
 """
-import logging
 from os.path import basename
 from re import split
 
 import numpy as np
 import pandas as pd
+from loguru import logger
 
 from . import _init_attrs
 from .util import anyopen
 from ..postprocessors.units import R_kJmol, kJ2kcal
 
-logger = logging.getLogger("alchemlyb.parsers.NAMD")
-
 k_b = R_kJmol * kJ2kcal
 
 
 def _filename_sort_key(s):
     """Key for natural-sorting filenames, ignoring the path.
 
     This means that unlike with the standard Python sorted() function, "foo9" < "foo10".
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/parsing/util.py` & `alchemlyb-2.1.0/src/alchemlyb/parsing/util.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/postprocessors/units.py` & `alchemlyb-2.1.0/src/alchemlyb/postprocessors/units.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/preprocessing/__init__.py` & `alchemlyb-2.1.0/src/alchemlyb/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/preprocessing/subsampling.py` & `alchemlyb-2.1.0/src/alchemlyb/preprocessing/subsampling.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import warnings
 
 import pandas as pd
 from pymbar.timeseries import detect_equilibration as _detect_equilibration
 from pymbar.timeseries import statistical_inefficiency as _statistical_inefficiency
 from pymbar.timeseries import subsample_correlated_data as _subsample_correlated_data
+from loguru import logger
 
 from .. import pass_attrs
 
 
 def decorrelate_u_nk(
     df, method="dE", drop_duplicates=True, sort=True, remove_burnin=False, **kwargs
 ):
@@ -512,20 +513,23 @@
     df, series = _prepare_input(df, series, drop_duplicates, sort)
 
     if series is not None:
         series = slicing(series, lower=lower, upper=upper, step=step)
         df = slicing(df, lower=lower, upper=upper, step=step)
 
         # calculate statistical inefficiency of series (could use fft=True but needs test)
+        logger.debug("Running statistical inefficiency analysis.")
         statinef = _statistical_inefficiency(series)
+        logger.debug("Statistical inefficiency: {:.2f}.", statinef)
 
         # use the subsample_correlated_data function to get the subsample index
         indices = _subsample_correlated_data(
             series, g=statinef, conservative=conservative
         )
+        logger.debug("Number of uncorrelated samples: {}.", len(indices))
         df = df.iloc[indices]
     else:
         df = slicing(df, lower=lower, upper=upper, step=step)
 
     return df
 
 
@@ -588,18 +592,22 @@
     df, series = _prepare_input(df, series, drop_duplicates, sort)
 
     if series is not None:
         series = slicing(series, lower=lower, upper=upper, step=step)
         df = slicing(df, lower=lower, upper=upper, step=step)
 
         # calculate statistical inefficiency of series, with equilibrium detection
+        logger.debug("Running equilibration detection.")
         t, statinef, Neff_max = _detect_equilibration(series.values)
+        logger.debug("Start index: {}.", t)
+        logger.debug("Statistical inefficiency: {:.2f}.", statinef)
 
         series_equil = series[t:]
         df_equil = df[t:]
 
         indices = _subsample_correlated_data(series_equil, g=statinef)
+        logger.debug("Number of uncorrelated samples: {}.", len(indices))
         df = df_equil.iloc[indices]
     else:
         df = slicing(df, lower=lower, upper=upper, step=step)
 
     return df
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/conftest.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Storing the fixture to be used for the tests. Note that this file will only contain
 fixture that are made directly from parsing the files. Any additional operations like
 concat should be done at local level."""
 
 import pytest
+from _pytest.logging import LogCaptureFixture
 from alchemtest.amber import load_bace_example, load_simplesolvated
 from alchemtest.gmx import (
     load_benzene,
     load_expanded_ensemble_case_1,
     load_expanded_ensemble_case_2,
     load_expanded_ensemble_case_3,
     load_water_particle_with_total_energy,
@@ -17,14 +18,15 @@
 from alchemtest.gomc import load_benzene as gomc_load_benzene
 from alchemtest.namd import (
     load_tyr2ala,
     load_idws,
     load_restarted,
     load_restarted_reversed,
 )
+from loguru import logger
 
 from alchemlyb.parsing import gmx, amber, gomc, namd
 
 
 @pytest.fixture
 def gmx_benzene():
     dataset = load_benzene()
@@ -265,7 +267,14 @@
 
 @pytest.fixture
 def namd_idws_restarted_reversed():
     dataset = load_restarted_reversed()
     u_nk = namd.extract_u_nk(dataset["data"]["both"], T=300)
 
     return u_nk
+
+
+@pytest.fixture
+def caplog(caplog: LogCaptureFixture):
+    handler_id = logger.add(caplog.handler, format="{message}")
+    yield caplog
+    logger.remove(handler_id)
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_amber.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_amber.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Amber parser tests.
 
 """
+import bz2
 import logging
 
 import pandas as pd
 import pytest
 from alchemtest.amber import load_bace_example
 from alchemtest.amber import load_bace_improper
 from alchemtest.amber import load_simplesolvated
@@ -246,7 +247,39 @@
 def test_u_nk_improper(improper_filename, names=("time", "lambdas")):
     """Test the u_nk has the correct form when extracted from files"""
     try:
         u_nk = extract_u_nk(improper_filename, T=298.0)
         assert u_nk.index.names == names
     except Exception:
         assert "0.5626" in improper_filename
+
+
+def test_concatenated_amber_u_nk(tmp_path):
+    with bz2.open(load_bace_example()["data"]["complex"]["decharge"][0], "rt") as file:
+        content = file.read()
+
+    with open(tmp_path / "amber.out", "w") as f:
+        f.write(content)
+        f.write("\n")
+        f.write(content)
+
+    with pytest.raises(
+        ValueError,
+        match="MBAR Energy detected after the TIMINGS section.",
+    ):
+        extract(tmp_path / "amber.out", 298)
+
+
+def test_concatenated_amber_dhdl(tmp_path):
+    with bz2.open(load_bace_example()["data"]["complex"]["decharge"][0], "rt") as file:
+        content = file.read().replace("MBAR Energy analysis", "")
+
+    with open(tmp_path / "amber.out", "w") as f:
+        f.write(content)
+        f.write("\n")
+        f.write(content)
+
+    with pytest.raises(
+        ValueError,
+        match="TI Energy detected after the TIMINGS section.",
+    ):
+        extract(tmp_path / "amber.out", 298)
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_gmx.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gmx.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_gomc.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_gomc.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_namd.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_namd.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/parsing/test_util.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/parsing/test_util.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_convergence.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_convergence.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_fep_estimators.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_fep_estimators.py`

 * *Files 18% similar despite different names*

```diff
@@ -130,7 +130,23 @@
             _estimator.delta_f_ = 1
 
     @pytest.mark.parametrize("estimator", [MBAR, BAR])
     def test_states_(self, estimator):
         _estimator = estimator()
         with pytest.raises(AttributeError):
             _estimator.states_ = 1
+
+
+def test_bootstrap(gmx_benzene_Coulomb_u_nk):
+    u_nk = alchemlyb.concat(gmx_benzene_Coulomb_u_nk)
+    mbar = MBAR(n_bootstraps=2)
+    mbar.fit(u_nk)
+    mbar_bootstrap_mean = mbar.delta_f_.loc[0.00, 1.00]
+    mbar_bootstrap_err = mbar.d_delta_f_.loc[0.00, 1.00]
+
+    mbar = MBAR()
+    mbar.fit(u_nk)
+    mbar_mean = mbar.delta_f_.loc[0.00, 1.00]
+    mbar_err = mbar.d_delta_f_.loc[0.00, 1.00]
+
+    assert mbar_bootstrap_mean == mbar_mean
+    assert mbar_bootstrap_err != mbar_err
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_preprocessing.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_preprocessing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Tests for preprocessing functions.
 
 """
+import logging
+
 import numpy as np
 import pytest
 from numpy.testing import assert_allclose
 
 import alchemlyb
 from alchemlyb.preprocessing import (
     slicing,
@@ -519,7 +521,26 @@
             series = u_nk2series(u_nk, **methodargs)
         assert len(series) == len(u_nk)
         assert_allclose(series.sum(), reference)
 
     def test_other_method_ValueError(self, u_nk):
         with pytest.raises(ValueError, match="Decorrelation method bogus not found."):
             u_nk2series(u_nk, method="bogus")
+
+
+class TestLogging:
+    def test_detect_equilibration(self, caplog, u_nk):
+        with caplog.at_level(logging.DEBUG):
+            decorrelate_u_nk(u_nk, remove_burnin=True)
+
+            assert "Running equilibration detection." in caplog.text
+            assert "Start index:" in caplog.text
+            assert "Statistical inefficiency:" in caplog.text
+            assert "Number of uncorrelated samples:" in caplog.text
+
+    def test_statistical_inefficiency(self, caplog, u_nk):
+        with caplog.at_level(logging.DEBUG):
+            decorrelate_u_nk(u_nk)
+
+            assert "Running statistical inefficiency analysis." in caplog.text
+            assert "Statistical inefficiency:" in caplog.text
+            assert "Number of uncorrelated samples:" in caplog.text
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_ti_estimators.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_ti_estimators.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_units.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_visualisation.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_visualisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,30 @@
     )
     df.attrs = estimate.delta_f_.attrs
     ax = plot_convergence(df)
     assert isinstance(ax, matplotlib.axes.Axes)
     plt.close(ax.figure)
 
 
+def test_plot_convergence_final_nan():
+    """Test the case where the Error of the final estimate is NaN."""
+    df = pd.DataFrame(
+        data={
+            "Forward": [1, 2],
+            "Forward_Error": [np.nan, np.nan],
+            "Backward": [1, 2],
+            "Backward_Error": [np.nan, np.nan],
+        }
+    )
+    df.attrs = {"temperature": 300, "energy_unit": "kT"}
+    ax = plot_convergence(df)
+    assert isinstance(ax, matplotlib.axes.Axes)
+    plt.close(ax.figure)
+
+
 class Test_Units:
     @staticmethod
     @pytest.fixture()
     def estimaters(gmx_benzene_Coulomb_dHdl, gmx_benzene_Coulomb_u_nk):
         dHdl_coul = alchemlyb.concat(gmx_benzene_Coulomb_dHdl)
         ti = TI().fit(dHdl_coul)
         u_nk_coul = alchemlyb.concat(gmx_benzene_Coulomb_u_nk)
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_workflow.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/tests/test_workflow_ABFE.py` & `alchemlyb-2.1.0/src/alchemlyb/tests/test_workflow_ABFE.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 import numpy as np
 import pytest
 from alchemtest.amber import load_bace_example
 from alchemtest.gmx import load_ABFE
 
+import alchemlyb.parsing.amber
 from alchemlyb.workflows.abfe import ABFE
 
 
 @pytest.fixture(scope="module")
 def workflow(tmp_path_factory):
     outdir = tmp_path_factory.mktemp("out")
     dir = os.path.dirname(load_ABFE()["data"]["complex"][0])
@@ -39,14 +40,33 @@
             ABFE(
                 dir="./",
                 prefix="dhdl",
                 suffix="xvg",
                 T=310,
             )
 
+    def test_notdir(self):
+        with pytest.raises(ValueError, match="The input directory `dir`="):
+            ABFE(
+                dir="abfasfsd",
+                prefix="dhdl",
+                suffix="xvg",
+                T=310,
+            )
+
+    def test_wildcard_in_dir(self):
+        with pytest.raises(ValueError):
+            with pytest.warns(match="A real directory is expected in `dir`="):
+                ABFE(
+                    dir="/*/",
+                    prefix="dhdl",
+                    suffix="xvg",
+                    T=310,
+                )
+
 
 class TestRun:
     def test_none(self, workflow):
         """Don't run anything"""
         workflow.run(
             uncorr=None, estimators=None, overlap=None, breakdown=None, forwrev=None
         )
@@ -216,14 +236,25 @@
         monkeypatch.setattr(workflow, "estimator", dict())
         workflow.estimate(estimators="MBAR")
         assert len(workflow.estimator) == 1
         assert "MBAR" in workflow.estimator
         summary = workflow.generate_result()
         assert np.isclose(summary["MBAR"]["Stages"]["TOTAL"], 21.645742066696315, 0.1)
 
+    def test_mbar_n_bootstraps(self, workflow, monkeypatch):
+        monkeypatch.setattr(workflow, "estimator", dict())
+        workflow.estimate(estimators="MBAR", n_bootstraps=2)
+        summary = workflow.generate_result()
+        bootstrap_error = summary["MBAR_Error"]["Stages"]["TOTAL"]
+        monkeypatch.setattr(workflow, "estimator", dict())
+        workflow.estimate(estimators="MBAR", n_bootstraps=0)
+        summary = workflow.generate_result()
+        non_bootstrap_error = summary["MBAR_Error"]["Stages"]["TOTAL"]
+        assert bootstrap_error != non_bootstrap_error
+
     def test_single_estimator_ti(self, workflow, monkeypatch):
         monkeypatch.setattr(workflow, "estimator", dict())
         monkeypatch.setattr(workflow, "summary", None)
         workflow.estimate(estimators="TI")
         summary = workflow.generate_result()
         assert np.isclose(summary["TI"]["Stages"]["TOTAL"], 21.51472826028906, 0.1)
 
@@ -374,7 +405,37 @@
         workflow.estimate(estimators="TI")
         return workflow
 
     def test_summary(self, workflow):
         """Test if if the summary is right."""
         summary = workflow.generate_result()
         assert np.isclose(summary["TI"]["Stages"]["TOTAL"], 1.40405980473, 0.1)
+
+
+class Test_automatic_parquet:
+    """Test the full automatic workflow for load_ABFE from parquet data."""
+
+    @staticmethod
+    @pytest.fixture(scope="class")
+    def workflow(tmp_path_factory):
+        outdir = tmp_path_factory.mktemp("out")
+        for i, u_nk in enumerate(load_bace_example()["data"]["complex"]["vdw"]):
+            df = alchemlyb.parsing.amber.extract_u_nk(u_nk, T=298)
+            df.to_parquet(path=f"{outdir}/u_nk_{i}.parquet", index=True)
+
+        workflow = ABFE(
+            units="kcal/mol",
+            software="PARQUET",
+            dir=str(outdir),
+            prefix="u_nk_",
+            suffix="parquet",
+            T=298.0,
+            outdirectory=str(outdir),
+        )
+        workflow.read()
+        workflow.estimate(estimators="BAR")
+        return workflow
+
+    def test_summary(self, workflow):
+        """Test if if the summary is right."""
+        summary = workflow.generate_result()
+        assert np.isclose(summary["BAR"]["Stages"]["TOTAL"], 1.40405980473, 0.1)
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/visualisation/convergence.py` & `alchemlyb-2.1.0/src/alchemlyb/visualisation/convergence.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,21 +89,22 @@
 
     f_ts = np.linspace(0, 1, len(forward) + 1)[1:]
     r_ts = np.linspace(0, 1, len(backward) + 1)[1:]
 
     if final_error is None:
         final_error = backward_error[-1]
 
-    line0 = ax.fill_between(
-        [0, 1],
-        backward[-1] - final_error,
-        backward[-1] + final_error,
-        color="#D2B9D3",
-        zorder=1,
-    )
+    if np.isfinite(backward[-1]) and np.isfinite(final_error):
+        line0 = ax.fill_between(
+            [0, 1],
+            backward[-1] - final_error,
+            backward[-1] + final_error,
+            color="#D2B9D3",
+            zorder=1,
+        )
     line1 = ax.errorbar(
         f_ts,
         forward,
         yerr=forward_error,
         color="#736AFF",
         lw=3,
         zorder=2,
@@ -125,15 +126,15 @@
         mew=2.5,
         mec="#C11B17",
         ms=12,
     )
 
     xticks_spacing = len(r_ts) // 10 or 1
     xticks = r_ts[::xticks_spacing]
-    plt.xticks(xticks, ["%.2f" % i for i in xticks], fontsize=10)
+    plt.xticks(xticks, [f"{i:.2f}" for i in xticks], fontsize=10)
     plt.yticks(fontsize=10)
 
     ax.legend(
         (line1[0], line2[0]),
         ("Forward", "Reverse"),
         loc=9,
         prop=FP(size=18),
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/visualisation/dF_state.py` & `alchemlyb-2.1.0/src/alchemlyb/visualisation/dF_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,15 @@
                 ax.spines[dir].set_color("none")
 
         if orientation == "landscape":
             plt.yticks(fontsize=8)
             ax.set_xlim(x[0] - width, x[-1] + len(lines) * width)
             plt.xticks(
                 x + 0.5 * width * len(estimators),
-                tuple(["%d--%d" % (i, i + 1) for i in x]),
+                tuple([f"{i}--{i+1}" for i in x]),
                 fontsize=8,
             )
         elif orientation == "portrait":
             plt.yticks(fontsize=10)
             ax.xaxis.set_ticks([])
             for i in x + 0.5 * width * len(estimators):
                 ax.annotate(
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/visualisation/mbar_matrix.py` & `alchemlyb-2.1.0/src/alchemlyb/visualisation/mbar_matrix.py`

 * *Files identical despite different names*

### Comparing `alchemlyb-2.0.1/src/alchemlyb/visualisation/ti_dhdl.py` & `alchemlyb-2.1.0/src/alchemlyb/visualisation/ti_dhdl.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     # Modified so that the x label won't conflict with the lambda label
     min_y -= (max_y - min_y) * 0.1
 
     ax.set_ylim(min_y, max_y)
 
     for i, j in zip(xs[1:], xt[1:]):
         ax.annotate(
-            ("%.2f" % (i - 1.0 if i > 1.0 else i) if not j == "" else ""),
+            ("{:.2f}".format(i - 1.0 if i > 1.0 else i) if not j == "" else ""),
             xy=(i, 0),
             size=10,
             rotation=90,
             va="bottom",
             ha="center",
             color="#151B54",
         )
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/workflows/abfe.py` & `alchemlyb-2.1.0/src/alchemlyb/workflows/abfe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import logging
 import os
+import warnings
 from os.path import join
 from pathlib import Path
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+from loguru import logger
 
 from .base import WorkflowBase
 from .. import concat
 from ..convergence import forward_backward_convergence
 from ..estimators import MBAR, BAR, TI, FEP_ESTIMATORS, TI_ESTIMATORS
-from ..parsing import gmx, amber
+from ..parsing import gmx, amber, parquet
 from ..postprocessors.units import get_unit_converter
 from ..preprocessing.subsampling import decorrelate_dhdl, decorrelate_u_nk
 from ..visualisation import (
     plot_mbar_overlap_matrix,
     plot_ti_dhdl,
     plot_dF_state,
     plot_convergence,
@@ -34,22 +35,22 @@
     ----------
     T : float
         Temperature in K.
     units : str
         The unit used for printing and plotting results. {'kcal/mol', 'kJ/mol',
         'kT'}. Default: 'kT'.
     software : str
-        The software used for generating input (case-insensitive). {'GROMACS', 'AMBER'}.
+        The software used for generating input (case-insensitive). {'GROMACS', 'AMBER', 'PARQUET'}.
         This option chooses the appropriate parser for the input file.
     dir : str
         Directory in which data files are stored. Default: os.path.curdir.
-        The input files are searched using the pattern of
-        ``dir + '/**/' + prefix + '*' + suffix``.
     prefix : str
-        Prefix for datafile sets. Default: 'dhdl'.
+        Prefix for datafile sets. This argument accepts regular expressions and
+        the input files are searched using
+        ``Path(dir).glob("**/" + prefix + "*" + suffix)``. Default: 'dhdl'.
     suffix : str
         Suffix for datafile sets. Default: 'xvg'.
     outdirectory : str
         Directory in which the output files produced by this script will be
         stored. Default: os.path.curdir.
 
     Attributes
@@ -57,56 +58,67 @@
     logger : Logger
         The logging object.
     file_list : list
         The list of filenames sorted by the lambda state.
 
 
     .. versionadded:: 1.0.0
+    .. versionchanged:: 2.0.1
+        The `dir` argument expects a real directory without wildcards and wildcards will no longer
+        work as expected. Use `prefix` to specify wildcard-based patterns to search under `dir`.
+    .. versionchanged:: 2.1.0
+        The serialised dataframe could be read via software='PARQUET'.
     """
 
     def __init__(
         self,
         T,
         units="kT",
         software="GROMACS",
         dir=os.path.curdir,
         prefix="dhdl",
         suffix="xvg",
         outdirectory=os.path.curdir,
     ):
         super().__init__(units, software, T, outdirectory)
-        self.logger.info("Initialise Alchemlyb ABFE Workflow")
+        logger.info("Initialise Alchemlyb ABFE Workflow")
         self.update_units(units)
-        self.logger.info(
+        logger.info(
             f"Finding files with prefix: {prefix}, suffix: "
             f"{suffix} under directory {dir} produced by "
             f"{software}"
         )
         reg_exp = "**/" + prefix + "*" + suffix
+        if "*" in dir:
+            warnings.warn(
+                f"A real directory is expected in `dir`={dir}, wildcard expressions should be supplied to `prefix`."
+            )
+        if not Path(dir).is_dir():
+            raise ValueError(f"The input directory `dir`={dir} is not a directory.")
         self.file_list = list(map(str, Path(dir).glob(reg_exp)))
 
         if len(self.file_list) == 0:
             raise ValueError(f"No file has been matched to {reg_exp}.")
 
-        self.logger.info(f"Found {len(self.file_list)} xvg files.")
-        self.logger.info("Unsorted file list: \n %s", "\n".join(self.file_list))
+        logger.info(f"Found {len(self.file_list)} {suffix} files.")
+        logger.info("Unsorted file list: \n {}", "\n".join(self.file_list))
 
         if software == "GROMACS":
-            self.logger.info(f"Using {software} parser to read the data.")
+            logger.info(f"Using {software} parser to read the data.")
             self._extract_u_nk = gmx.extract_u_nk
             self._extract_dHdl = gmx.extract_dHdl
         elif software == "AMBER":
             self._extract_u_nk = amber.extract_u_nk
             self._extract_dHdl = amber.extract_dHdl
+        elif software == "PARQUET":
+            self._extract_u_nk = parquet.extract_u_nk
+            self._extract_dHdl = parquet.extract_dHdl
         else:
             raise NotImplementedError(f"{software} parser not found.")
 
-    def _logger_setup(self):
-        self.logger = logging.getLogger("alchemlyb.workflows.ABFE")
-
     def read(self, read_u_nk=True, read_dHdl=True):
         """Read the u_nk and dHdL data from the
         :attr:`~alchemlyb.workflows.ABFE.file_list`
 
         Parameters
         ----------
         read_u_nk : bool
@@ -126,54 +138,54 @@
 
         u_nk_list = []
         dHdl_list = []
         for file in self.file_list:
             if read_u_nk:
                 try:
                     u_nk = self._extract_u_nk(file, T=self.T)
-                    self.logger.info(f"Reading {len(u_nk)} lines of u_nk from {file}")
+                    logger.info(f"Reading {len(u_nk)} lines of u_nk from {file}")
                     u_nk_list.append(u_nk)
                 except Exception as exc:
                     msg = f"Error reading u_nk from {file}."
-                    self.logger.error(msg)
+                    logger.error(msg)
                     raise OSError(msg) from exc
 
             if read_dHdl:
                 try:
                     dhdl = self._extract_dHdl(file, T=self.T)
-                    self.logger.info(f"Reading {len(dhdl)} lines of dhdl from {file}")
+                    logger.info(f"Reading {len(dhdl)} lines of dhdl from {file}")
                     dHdl_list.append(dhdl)
                 except Exception as exc:
                     msg = f"Error reading dHdl from {file}."
-                    self.logger.error(msg)
+                    logger.error(msg)
                     raise OSError(msg) from exc
 
         # Sort the files according to the state
         if read_u_nk:
-            self.logger.info("Sort files according to the u_nk.")
+            logger.info("Sort files according to the u_nk.")
             column_names = u_nk_list[0].columns.values.tolist()
             index_list = sorted(
                 range(len(self.file_list)),
                 key=lambda x: column_names.index(
                     u_nk_list[x].reset_index("time").index.values[0]
                 ),
             )
         elif read_dHdl:
-            self.logger.info("Sort files according to the dHdl.")
+            logger.info("Sort files according to the dHdl.")
             index_list = sorted(
                 range(len(self.file_list)),
                 key=lambda x: dHdl_list[x].reset_index("time").index.values[0],
             )
         else:
             self.u_nk_list = []
             self.dHdl_list = []
             return
 
         self.file_list = [self.file_list[i] for i in index_list]
-        self.logger.info("Sorted file list: \n%s", "\n".join(self.file_list))
+        logger.info("Sorted file list: \n{}", "\n".join(self.file_list))
         if read_u_nk:
             self.u_nk_list = [u_nk_list[i] for i in index_list]
         else:
             self.u_nk_list = []
 
         if read_dHdl:
             self.dHdl_list = [dHdl_list[i] for i in index_list]
@@ -248,15 +260,15 @@
                 elif estimator in TI_ESTIMATORS:
                     use_TI = True
                 else:
                     msg = (
                         f"Estimator {estimator} is not supported. Choose one from "
                         f"{FEP_ESTIMATORS + TI_ESTIMATORS}."
                     )
-                    self.logger.error(msg)
+                    logger.error(msg)
                     raise ValueError(msg)
 
             self.read(use_FEP, use_TI)
 
         if uncorr is not None:
             self.preprocess(skiptime=skiptime, uncorr=uncorr, threshold=threshold)
         if estimators is not None:
@@ -288,15 +300,15 @@
         Parameters
         ----------
         units : {'kcal/mol', 'kJ/mol', 'kT'}
             The unit used for printing and plotting results.
 
         """
         if units is not None:
-            self.logger.info(f"Set unit to {units}.")
+            logger.info(f"Set unit to {units}.")
             self.units = units or None
 
     def preprocess(self, skiptime=0, uncorr="dE", threshold=50):
         """Preprocess the data by removing the equilibration time and
         decorrelate the date.
 
         Parameters
@@ -314,69 +326,67 @@
         Attributes
         ----------
         u_nk_sample_list : list
             The list of u_nk after decorrelation.
         dHdl_sample_list : list
             The list of dHdl after decorrelation.
         """
-        self.logger.info(
+        logger.info(
             f"Start preprocessing with skiptime of {skiptime} "
             f"uncorrelation method of {uncorr} and threshold of "
             f"{threshold}"
         )
         if len(self.u_nk_list) > 0:
-            self.logger.info(
-                f"Processing the u_nk data set with skiptime of {skiptime}."
-            )
+            logger.info(f"Processing the u_nk data set with skiptime of {skiptime}.")
 
             self.u_nk_sample_list = []
             for index, u_nk in enumerate(self.u_nk_list):
                 # Find the starting frame
 
                 u_nk = u_nk[u_nk.index.get_level_values("time") >= skiptime]
                 subsample = decorrelate_u_nk(u_nk, uncorr, remove_burnin=True)
 
                 if len(subsample) < threshold:
-                    self.logger.warning(
+                    logger.warning(
                         f"Number of u_nk {len(subsample)} "
                         f"for state {index} is less than the "
                         f"threshold {threshold}."
                     )
-                    self.logger.info(f"Take all the u_nk for state {index}.")
+                    logger.info(f"Take all the u_nk for state {index}.")
                     self.u_nk_sample_list.append(u_nk)
                 else:
-                    self.logger.info(
+                    logger.info(
                         f"Take {len(subsample)} uncorrelated "
                         f"u_nk for state {index}."
                     )
                     self.u_nk_sample_list.append(subsample)
         else:
-            self.logger.info("No u_nk data being subsampled")
+            logger.info("No u_nk data being subsampled")
 
         if len(self.dHdl_list) > 0:
             self.dHdl_sample_list = []
             for index, dHdl in enumerate(self.dHdl_list):
                 dHdl = dHdl[dHdl.index.get_level_values("time") >= skiptime]
                 subsample = decorrelate_dhdl(dHdl, remove_burnin=True)
                 if len(subsample) < threshold:
-                    self.logger.warning(
+                    logger.warning(
                         f"Number of dHdl {len(subsample)} for "
                         f"state {index} is less than the "
                         f"threshold {threshold}."
                     )
-                    self.logger.info(f"Take all the dHdl for state {index}.")
+                    logger.info(f"Take all the dHdl for state {index}.")
                     self.dHdl_sample_list.append(dHdl)
                 else:
-                    self.logger.info(
+                    logger.info(
                         f"Take {len(subsample)} uncorrelated "
                         f"dHdl for state {index}."
                     )
                     self.dHdl_sample_list.append(subsample)
         else:
-            self.logger.info("No dHdl data being subsampled")
+            logger.info("No dHdl data being subsampled")
 
     def estimate(self, estimators=("MBAR", "BAR", "TI"), **kwargs):
         """Estimate the free energy using the selected estimator.
 
         Parameters
         ----------
         estimators : str or list of str
@@ -389,53 +399,61 @@
         Attributes
         ----------
         estimator : dict
             The dictionary of estimators. The keys are in ['TI', 'BAR',
             'MBAR']. Note that the estimators are in their original form where
             no unit conversion has been attempted.
 
+
+        .. versionchanged:: 2.1.0
+            DeprecationWarning for using analytic error for MBAR estimator.
+
         """
         # Make estimators into a tuple
         if isinstance(estimators, str):
             estimators = (estimators,)
 
         for estimator in estimators:
             if estimator not in (FEP_ESTIMATORS + TI_ESTIMATORS):
                 msg = f"Estimator {estimator} is not available in {FEP_ESTIMATORS + TI_ESTIMATORS}."
-                self.logger.error(msg)
+                logger.error(msg)
                 raise ValueError(msg)
 
-        self.logger.info(f"Start running estimator: {','.join(estimators)}.")
+        logger.info(f"Start running estimator: {','.join(estimators)}.")
         self.estimator = {}
         # Use unprocessed data if preprocess is not performed.
         if "TI" in estimators:
             if self.dHdl_sample_list is not None:
                 dHdl = concat(self.dHdl_sample_list)
             else:
                 dHdl = concat(self.dHdl_list)
-                self.logger.warning("dHdl has not been preprocessed.")
-            self.logger.info(f"A total {len(dHdl)} lines of dHdl is used.")
+                logger.warning("dHdl has not been preprocessed.")
+            logger.info(f"A total {len(dHdl)} lines of dHdl is used.")
 
         if "BAR" in estimators or "MBAR" in estimators:
             if self.u_nk_sample_list is not None:
                 u_nk = concat(self.u_nk_sample_list)
             else:
                 u_nk = concat(self.u_nk_list)
-                self.logger.warning("u_nk has not been preprocessed.")
-            self.logger.info(f"A total {len(u_nk)} lines of u_nk is used.")
+                logger.warning("u_nk has not been preprocessed.")
+            logger.info(f"A total {len(u_nk)} lines of u_nk is used.")
 
         for estimator in estimators:
             if estimator == "MBAR":
-                self.logger.info("Run MBAR estimator.")
+                logger.info("Run MBAR estimator.")
+                warnings.warn(
+                    "From 2.2.0, n_bootstraps=50 will be the default for estimating MBAR error.",
+                    DeprecationWarning,
+                )
                 self.estimator[estimator] = MBAR(**kwargs).fit(u_nk)
             elif estimator == "BAR":
-                self.logger.info("Run BAR estimator.")
+                logger.info("Run BAR estimator.")
                 self.estimator[estimator] = BAR(**kwargs).fit(u_nk)
             elif estimator == "TI":
-                self.logger.info("Run TI estimator.")
+                logger.info("Run TI estimator.")
                 self.estimator[estimator] = TI(**kwargs).fit(dHdl)
 
     def generate_result(self):
         """Summarise the result into a dataframe.
 
         Returns
         -------
@@ -480,42 +498,42 @@
         Attributes
         ----------
         summary : Dataframe
             The summary of the free energy estimate.
         """
 
         # Write estimate
-        self.logger.info("Summarise the estimate into a dataframe.")
+        logger.info("Summarise the estimate into a dataframe.")
         # Make the header name
-        self.logger.info("Generate the row names.")
+        logger.info("Generate the row names.")
         estimator_names = list(self.estimator.keys())
         num_states = len(self.estimator[estimator_names[0]].states_)
         data_dict = {"name": [], "state": []}
         for i in range(num_states - 1):
             data_dict["name"].append(str(i) + " -- " + str(i + 1))
             data_dict["state"].append("States")
 
         try:
             u_nk = self.u_nk_list[0]
             stages = u_nk.reset_index("time").index.names
-            self.logger.info("use the stage name from u_nk")
+            logger.info("use the stage name from u_nk")
         except:
             dHdl = self.dHdl_list[0]
             stages = dHdl.reset_index("time").index.names
-            self.logger.info("use the stage name from dHdl")
+            logger.info("use the stage name from dHdl")
 
         for stage in stages:
             data_dict["name"].append(stage.split("-")[0])
             data_dict["state"].append("Stages")
         data_dict["name"].append("TOTAL")
         data_dict["state"].append("Stages")
 
         col_names = []
         for estimator_name, estimator in self.estimator.items():
-            self.logger.info(f"Read the results from estimator {estimator_name}")
+            logger.info(f"Read the results from estimator {estimator_name}")
 
             # Do the unit conversion
             delta_f_ = estimator.delta_f_
             d_delta_f_ = estimator.d_delta_f_
             # Write the estimator header
 
             col_names.append(estimator_name)
@@ -524,17 +542,15 @@
             data_dict[estimator_name + "_Error"] = []
             for index in range(1, num_states):
                 data_dict[estimator_name].append(delta_f_.iloc[index - 1, index])
                 data_dict[estimator_name + "_Error"].append(
                     d_delta_f_.iloc[index - 1, index]
                 )
 
-            self.logger.info(
-                f"Generate the staged result from estimator {estimator_name}"
-            )
+            logger.info(f"Generate the staged result from estimator {estimator_name}")
             for index, stage in enumerate(stages):
                 if len(stages) == 1:
                     start = 0
                     end = len(estimator.states_) - 1
                 else:
                     # Get the start and the end of the state
                     lambda_min = min([state[index] for state in estimator.states_])
@@ -545,15 +561,15 @@
                         start = 0
                         end = 0
                     else:
                         states = [state[index] for state in estimator.states_]
                         start = list(reversed(states)).index(lambda_min)
                         start = num_states - start - 1
                         end = states.index(lambda_max)
-                self.logger.info(f"Stage {stage} is from state {start} to state {end}.")
+                logger.info(f"Stage {stage} is from state {start} to state {end}.")
                 # This assumes that the indexes are sorted as the
                 # preprocessing should sort the index of the df.
                 result = delta_f_.iloc[start, end]
                 if estimator_name != "BAR":
                     error = d_delta_f_.iloc[start, end]
                 else:
                     error = np.sqrt(
@@ -587,15 +603,15 @@
         # Remove the name of the index column to make it prettier
         summary.index.names = [None, None]
 
         summary.attrs = estimator.delta_f_.attrs
         converter = get_unit_converter(self.units)
         summary = converter(summary)
         self.summary = summary
-        self.logger.info(f"Write results:\n{summary.to_string()}")
+        logger.info(f"Write results:\n{summary.to_string()}")
         return summary
 
     def plot_overlap_matrix(self, overlap="O_MBAR.pdf", ax=None):
         """Plot the overlap matrix for MBAR estimator using
         :func:`~alchemlyb.visualisation.plot_mbar_overlap_matrix`.
 
         Parameters
@@ -607,24 +623,22 @@
             ``ax=None``, a new axes will be generated.
 
         Returns
         -------
         matplotlib.axes.Axes
             An axes with the overlap matrix drawn.
         """
-        self.logger.info("Plot overlap matrix.")
+        logger.info("Plot overlap matrix.")
         if "MBAR" in self.estimator:
             ax = plot_mbar_overlap_matrix(self.estimator["MBAR"].overlap_matrix, ax=ax)
             ax.figure.savefig(join(self.out, overlap))
-            self.logger.info(f"Plot overlap matrix to {self.out} under {overlap}.")
+            logger.info(f"Plot overlap matrix to {self.out} under {overlap}.")
             return ax
         else:
-            self.logger.warning(
-                "MBAR estimator not found. " "Overlap matrix not plotted."
-            )
+            logger.warning("MBAR estimator not found. " "Overlap matrix not plotted.")
 
     def plot_ti_dhdl(self, dhdl_TI="dhdl_TI.pdf", labels=None, colors=None, ax=None):
         """Plot the dHdl for TI estimator using
         :func:`~alchemlyb.visualisation.plot_ti_dhdl`.
 
         Parameters
         ----------
@@ -640,25 +654,25 @@
             a new axes will be generated.
 
         Returns
         -------
         matplotlib.axes.Axes
             An axes with the TI dhdl drawn.
         """
-        self.logger.info("Plot TI dHdl.")
+        logger.info("Plot TI dHdl.")
         if "TI" in self.estimator:
             ax = plot_ti_dhdl(
                 self.estimator["TI"],
                 units=self.units,
                 labels=labels,
                 colors=colors,
                 ax=ax,
             )
             ax.figure.savefig(join(self.out, dhdl_TI))
-            self.logger.info(f"Plot TI dHdl to {dhdl_TI} under {self.out}.")
+            logger.info(f"Plot TI dHdl to {dhdl_TI} under {self.out}.")
             return ax
         else:
             raise ValueError("No TI data available in estimators.")
 
     def plot_dF_state(
         self,
         dF_state="dF_state.pdf",
@@ -684,25 +698,25 @@
             Maximum number of dF states in one row in the `portrait` mode
 
         Returns
         -------
         matplotlib.figure.Figure
             An Figure with the dF states drawn.
         """
-        self.logger.info("Plot dF states.")
+        logger.info("Plot dF states.")
         fig = plot_dF_state(
             self.estimator.values(),
             labels=labels,
             colors=colors,
             units=self.units,
             orientation=orientation,
             nb=nb,
         )
         fig.savefig(join(self.out, dF_state))
-        self.logger.info(f"Plot dF state to {dF_state} under {self.out}.")
+        logger.info(f"Plot dF state to {dF_state} under {self.out}.")
         return fig
 
     def check_convergence(
         self, forwrev, estimator="MBAR", dF_t="dF_t.pdf", ax=None, **kwargs
     ):
         """Compute the forward and backward convergence using
         :func:`~alchemlyb.convergence.forward_backward_convergence`and
@@ -731,66 +745,66 @@
 
         Returns
         -------
         matplotlib.axes.Axes
             An axes with the convergence drawn.
 
         """
-        self.logger.info("Start convergence analysis.")
-        self.logger.info("Checking data availability.")
+        logger.info("Start convergence analysis.")
+        logger.info("Checking data availability.")
 
         if estimator in FEP_ESTIMATORS:
             if self.u_nk_sample_list is not None:
                 u_nk_list = self.u_nk_sample_list
-                self.logger.info("Subsampled u_nk is available.")
+                logger.info("Subsampled u_nk is available.")
             else:
                 if self.u_nk_list is not None:
                     u_nk_list = self.u_nk_list
-                    self.logger.info(
+                    logger.info(
                         "Subsampled u_nk not available, " "use original data instead."
                     )
                 else:
                     msg = (
                         f"u_nk is needed for the f{estimator} estimator. "
                         f"If the dataset only has dHdl, "
                         f"run ABFE.check_convergence(estimator='TI') to "
                         f"use a TI estimator."
                     )
-                    self.logger.error(msg)
+                    logger.error(msg)
                     raise ValueError(msg)
             convergence = forward_backward_convergence(
                 u_nk_list, estimator=estimator, num=forwrev, **kwargs
             )
         elif estimator in TI_ESTIMATORS:
-            self.logger.warning(
+            logger.warning(
                 "No valid FEP estimator or dataset found. " "Fallback to TI."
             )
             if self.dHdl_sample_list is not None:
                 dHdl_list = self.dHdl_sample_list
-                self.logger.info("Subsampled dHdl is available.")
+                logger.info("Subsampled dHdl is available.")
             else:
                 if self.dHdl_list is not None:
                     dHdl_list = self.dHdl_list
-                    self.logger.info(
+                    logger.info(
                         "Subsampled dHdl not available, " "use original data instead."
                     )
                 else:
-                    self.logger.error(f"dHdl is needed for the f{estimator} estimator.")
+                    logger.error(f"dHdl is needed for the f{estimator} estimator.")
                     raise ValueError(f"dHdl is needed for the f{estimator} estimator.")
             convergence = forward_backward_convergence(
                 dHdl_list, estimator=estimator, num=forwrev, **kwargs
             )
         else:
             msg = (
                 f"Estimator {estimator} is not supported. Choose one from "
                 f"{FEP_ESTIMATORS + TI_ESTIMATORS}."
             )
-            self.logger.error(msg)
+            logger.error(msg)
             raise ValueError(msg)
 
         self.convergence = get_unit_converter(self.units)(convergence)
 
-        self.logger.info(f"Plot convergence analysis to {dF_t} under {self.out}.")
+        logger.info(f"Plot convergence analysis to {dF_t} under {self.out}.")
 
         ax = plot_convergence(self.convergence, units=self.units, ax=ax)
         ax.figure.savefig(join(self.out, dF_t))
         return ax
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb/workflows/base.py` & `alchemlyb-2.1.0/src/alchemlyb/workflows/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Basic building blocks for free energy workflows."""
 
-import logging
 from pathlib import Path
 
 import pandas as pd
+from loguru import logger
 
 from .. import __version__
 
 
 class WorkflowBase:
     """The base class for the Workflow.
 
@@ -43,30 +43,26 @@
 
     .. versionadded:: 0.7.0
     """
 
     def __init__(
         self, units="kT", software="Gromacs", T=298, out="./", *args, **kwargs
     ):
-        self._logger_setup()
-        self.logger.info(f"Alchemlyb Version: f{__version__}")
-        self.logger.info(f"Set Temperature to {T} K.")
+        logger.info(f"Alchemlyb Version: f{__version__}")
+        logger.info(f"Set Temperature to {T} K.")
         self.T = T
-        self.logger.info(f"Set Software to {software}.")
+        logger.info(f"Set Software to {software}.")
         self.software = software
         self.unit = units
         self.file_list = []
         self.out = out
         if not Path(out).is_dir():
-            self.logger.info(f"Make output folder {out}.")
+            logger.info(f"Make output folder {out}.")
             Path(out).mkdir(parents=True)
 
-    def _logger_setup(self):
-        self.logger = logging.getLogger("alchemlyb.workflows.WorkflowBase")
-
     def run(self, *args, **kwargs):
         """Run the workflow in an automatic fashion.
 
         This method would execute the
         :func:`~alchemlyb.workflows.WorkflowBase.read`,
         :func:`~alchemlyb.workflows.WorkflowBase.preprocess`,
         :func:`~alchemlyb.workflows.WorkflowBase.estimate`,
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb.egg-info/PKG-INFO` & `alchemlyb-2.1.0/src/alchemlyb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemlyb
-Version: 2.0.1
+Version: 2.1.0
 Summary: the simple alchemistry library
 Author: David Dotson
 Author-email: dotsdl@gmail.com
 Maintainer: Oliver Beckstein
 Maintainer-email: orbeckst@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `alchemlyb-2.0.1/src/alchemlyb.egg-info/SOURCES.txt` & `alchemlyb-2.1.0/src/alchemlyb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 src/alchemlyb/estimators/mbar_.py
 src/alchemlyb/estimators/ti_.py
 src/alchemlyb/parsing/__init__.py
 src/alchemlyb/parsing/amber.py
 src/alchemlyb/parsing/gmx.py
 src/alchemlyb/parsing/gomc.py
 src/alchemlyb/parsing/namd.py
+src/alchemlyb/parsing/parquet.py
 src/alchemlyb/parsing/util.py
 src/alchemlyb/postprocessors/__init__.py
 src/alchemlyb/postprocessors/units.py
 src/alchemlyb/preprocessing/__init__.py
 src/alchemlyb/preprocessing/subsampling.py
 src/alchemlyb/tests/__init__.py
 src/alchemlyb/tests/conftest.py
@@ -43,14 +44,15 @@
 src/alchemlyb/tests/test_workflow.py
 src/alchemlyb/tests/test_workflow_ABFE.py
 src/alchemlyb/tests/parsing/__init__.py
 src/alchemlyb/tests/parsing/test_amber.py
 src/alchemlyb/tests/parsing/test_gmx.py
 src/alchemlyb/tests/parsing/test_gomc.py
 src/alchemlyb/tests/parsing/test_namd.py
+src/alchemlyb/tests/parsing/test_parquet.py
 src/alchemlyb/tests/parsing/test_util.py
 src/alchemlyb/visualisation/__init__.py
 src/alchemlyb/visualisation/convergence.py
 src/alchemlyb/visualisation/dF_state.py
 src/alchemlyb/visualisation/mbar_matrix.py
 src/alchemlyb/visualisation/ti_dhdl.py
 src/alchemlyb/workflows/__init__.py
```

### Comparing `alchemlyb-2.0.1/versioneer.py` & `alchemlyb-2.1.0/versioneer.py`

 * *Files identical despite different names*

