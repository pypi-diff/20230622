# Comparing `tmp/saqc-2.4.0.tar.gz` & `tmp/saqc-2.4.1-1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saqc-2.4.0.tar", last modified: Tue Apr 25 21:43:39 2023, max compression
+gzip compressed data, was "saqc-2.4.1.tar", last modified: Thu Jun 22 09:15:36 2023, max compression
```

## Comparing `saqc-2.4.0.tar` & `saqc-2.4.1-1.tar`

### file list

```diff
@@ -1,103 +1,109 @@
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.163224 saqc-2.4.0/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2796 2022-11-18 08:39:03.000000 saqc-2.4.0/LICENSE.md
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.153225 saqc-2.4.0/LICENSES/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    34670 2022-11-18 08:39:03.000000 saqc-2.4.0/LICENSES/GPL-3.0-or-later.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6130 2023-04-25 21:43:39.163224 saqc-2.4.0/PKG-INFO
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5720 2023-04-25 20:52:46.000000 saqc-2.4.0/README.md
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      346 2022-11-18 08:39:03.000000 saqc-2.4.0/pyproject.toml
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      550 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3507 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/__main__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1604 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/constants.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/core/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      414 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8452 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/core.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16823 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/flags.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5563 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/frame.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18033 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/history.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16349 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/register.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/core/translation/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      466 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7188 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/basescheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6355 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/dmpscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2766 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/positionalscheme.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      760 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/core/translation/simplescheme.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc/funcs/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1330 2022-11-18 08:39:03.000000 saqc-2.4.0/saqc/funcs/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6685 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/breaks.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    13510 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/changepoints.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5010 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/constants.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8250 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/curvefit.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    27888 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/drift.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19297 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/flagtools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8968 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/generic.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20621 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/interpolation.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2531 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/noise.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    58930 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/outliers.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6466 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/pattern.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    15415 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/resampling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4684 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/residuals.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6222 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/rolling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19477 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/scores.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11417 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1943 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/funcs/transformation.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/saqc/lib/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/saqc/lib/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3237 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/docs.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9483 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/plotting.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5073 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/rolling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18924 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19963 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/ts_operators.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      942 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/lib/types.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/saqc/parsing/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2303 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/environ.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2800 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/reader.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5704 2023-04-25 20:52:46.000000 saqc-2.4.0/saqc/parsing/visitor.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      173 2023-04-25 21:43:10.000000 saqc-2.4.0/saqc/version.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.156558 saqc-2.4.0/saqc.egg-info/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6130 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/PKG-INFO
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2127 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/SOURCES.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)        1 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/dependency_links.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       44 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/entry_points.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      122 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/requires.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       11 2023-04-25 21:43:39.000000 saqc-2.4.0/saqc.egg-info/top_level.txt
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)       38 2023-04-25 21:43:39.163224 saqc-2.4.0/setup.cfg
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1590 2023-04-25 21:30:42.000000 saqc-2.4.0/setup.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/api/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/api/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      538 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/api/test_creation.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/cli/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/cli/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3560 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/cli/test_integration.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/core/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/core/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11372 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_core.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11200 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_flags.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      262 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_frame.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6164 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_history.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4737 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_reader.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8529 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/core/test_translator.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/funcs/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/funcs/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1323 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_constants_detection.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7810 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_flagtools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9332 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6300 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_generic_api_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8453 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_generic_config_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6465 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_outlier_detection.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1254 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_pattern_rec.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4715 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_proc_functions.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12142 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_resampling.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1111 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/funcs/test_tools.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.159891 saqc-2.4.0/tests/fuzzy/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/fuzzy/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4968 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/fuzzy/lib.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5991 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/fuzzy/test_masking.py
-drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-04-25 21:43:39.163224 saqc-2.4.0/tests/lib/
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/lib/__init__.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2882 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/lib/test_periodicMask.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1747 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/lib/test_tools.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7063 2023-04-25 20:52:46.000000 saqc-2.4.0/tests/lib/test_ts_operators.py
--rw-r--r--   0 schaefed  (1000) schaefed  (1000)      531 2022-11-18 08:39:03.000000 saqc-2.4.0/tests/test__main__.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.466904 saqc-2.4.1/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2796 2022-07-08 08:06:22.000000 saqc-2.4.1/LICENSE.md
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.456904 saqc-2.4.1/LICENSES/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    34670 2022-07-08 08:06:22.000000 saqc-2.4.1/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6130 2023-06-22 09:15:36.466904 saqc-2.4.1/PKG-INFO
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5720 2023-04-05 11:41:00.000000 saqc-2.4.1/README.md
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      346 2023-03-30 19:15:16.000000 saqc-2.4.1/pyproject.toml
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.456904 saqc-2.4.1/saqc/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      550 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3507 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/__main__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1604 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/constants.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.460238 saqc-2.4.1/saqc/core/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      414 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/core/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8452 2023-05-24 06:55:14.000000 saqc-2.4.1/saqc/core/core.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16822 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/core/flags.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4555 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/core/frame.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    18033 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/core/history.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1180 2023-01-30 06:47:58.000000 saqc-2.4.1/saqc/core/mixins.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    16349 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/core/register.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.460238 saqc-2.4.1/saqc/core/translation/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      466 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/core/translation/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7188 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/core/translation/basescheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6355 2023-05-24 06:55:14.000000 saqc-2.4.1/saqc/core/translation/dmpscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1534 2023-01-30 06:47:58.000000 saqc-2.4.1/saqc/core/translation/floatscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2766 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/core/translation/positionalscheme.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      760 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/core/translation/simplescheme.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/saqc/funcs/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1330 2023-03-30 19:15:16.000000 saqc-2.4.1/saqc/funcs/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6685 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/breaks.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    13510 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/changepoints.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5010 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/constants.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8250 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/curvefit.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    28443 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/funcs/drift.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19432 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/funcs/flagtools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8968 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/generic.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20899 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/funcs/interpolation.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2531 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/noise.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    58930 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/outliers.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6466 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/pattern.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    15916 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/funcs/resampling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4684 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/residuals.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6307 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/funcs/rolling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19477 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/scores.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11731 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/funcs/tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1943 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/funcs/transformation.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/saqc/lib/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.4.1/saqc/lib/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3237 2023-05-24 06:55:17.000000 saqc-2.4.1/saqc/lib/docs.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1178 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/lib/exceptions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9483 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/lib/plotting.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5073 2023-05-24 06:55:14.000000 saqc-2.4.1/saqc/lib/rolling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    19941 2023-06-22 07:49:30.000000 saqc-2.4.1/saqc/lib/tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    20008 2023-06-07 07:36:15.000000 saqc-2.4.1/saqc/lib/ts_operators.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      942 2023-04-19 15:26:39.000000 saqc-2.4.1/saqc/lib/types.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/saqc/parsing/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/parsing/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2303 2023-05-24 06:55:14.000000 saqc-2.4.1/saqc/parsing/environ.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2800 2023-04-05 11:41:00.000000 saqc-2.4.1/saqc/parsing/reader.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5704 2023-06-07 07:36:11.000000 saqc-2.4.1/saqc/parsing/visitor.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      173 2023-06-22 09:14:21.000000 saqc-2.4.1/saqc/version.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.460238 saqc-2.4.1/saqc.egg-info/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6130 2023-06-22 09:15:36.000000 saqc-2.4.1/saqc.egg-info/PKG-INFO
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2256 2023-06-22 09:15:36.000000 saqc-2.4.1/saqc.egg-info/SOURCES.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)        1 2023-06-22 09:15:36.000000 saqc-2.4.1/saqc.egg-info/dependency_links.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       44 2023-06-22 09:15:36.000000 saqc-2.4.1/saqc.egg-info/entry_points.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      146 2023-06-22 09:15:36.000000 saqc-2.4.1/saqc.egg-info/requires.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       11 2023-06-22 09:15:36.000000 saqc-2.4.1/saqc.egg-info/top_level.txt
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)       38 2023-06-22 09:15:36.466904 saqc-2.4.1/setup.cfg
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1625 2023-06-22 07:49:30.000000 saqc-2.4.1/setup.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/tests/
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/tests/api/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.4.1/tests/api/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      538 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/api/test_creation.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/tests/cli/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.4.1/tests/cli/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     3560 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/cli/test_integration.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/tests/core/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.4.1/tests/core/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11372 2023-04-20 14:53:28.000000 saqc-2.4.1/tests/core/test_core.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    11200 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/core/test_flags.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      262 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/core/test_frame.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6164 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/core/test_history.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4737 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/core/test_reader.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8529 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/core/test_translator.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.463571 saqc-2.4.1/tests/funcs/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      176 2022-07-08 08:06:22.000000 saqc-2.4.1/tests/funcs/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1323 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/funcs/test_constants_detection.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7810 2023-05-24 06:55:14.000000 saqc-2.4.1/tests/funcs/test_flagtools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     9334 2023-06-22 07:49:30.000000 saqc-2.4.1/tests/funcs/test_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6300 2023-04-19 15:26:39.000000 saqc-2.4.1/tests/funcs/test_generic_api_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     8453 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/funcs/test_generic_config_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     6465 2023-05-24 06:55:17.000000 saqc-2.4.1/tests/funcs/test_outlier_detection.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1254 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/funcs/test_pattern_rec.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4715 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/funcs/test_proc_functions.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)    12142 2023-04-24 12:41:44.000000 saqc-2.4.1/tests/funcs/test_resampling.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1111 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/funcs/test_tools.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.466904 saqc-2.4.1/tests/fuzzy/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.4.1/tests/fuzzy/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     4968 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/fuzzy/lib.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     5991 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/fuzzy/test_masking.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.466904 saqc-2.4.1/tests/lib/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      150 2022-07-08 08:06:22.000000 saqc-2.4.1/tests/lib/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     2882 2023-03-30 19:15:16.000000 saqc-2.4.1/tests/lib/test_periodicMask.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     1747 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/lib/test_tools.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)     7063 2023-04-05 11:41:00.000000 saqc-2.4.1/tests/lib/test_ts_operators.py
+drwxr-xr-x   0 schaefed  (1000) schaefed  (1000)        0 2023-06-22 09:15:36.466904 saqc-2.4.1/tests/misc/
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      147 2023-06-22 07:49:30.000000 saqc-2.4.1/tests/misc/__init__.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      609 2023-06-22 07:49:30.000000 saqc-2.4.1/tests/misc/test_pickle.py
+-rw-r--r--   0 schaefed  (1000) schaefed  (1000)      531 2023-03-30 19:15:16.000000 saqc-2.4.1/tests/test__main__.py
```

### Comparing `saqc-2.4.0/LICENSE.md` & `saqc-2.4.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/LICENSES/GPL-3.0-or-later.txt` & `saqc-2.4.1/LICENSES/GPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/PKG-INFO` & `saqc-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saqc
-Version: 2.4.0
+Version: 2.4.1
 Summary: A timeseries data quality control and processing tool/framework
 Home-page: https://git.ufz.de/rdm-software/saqc
 Author: Bert Palm, David Schaefer, Florian Gransee, Peter Luenenschloss
 Author-email: david.schaefer@ufz.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `saqc-2.4.0/README.md` & `saqc-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/__init__.py` & `saqc-2.4.1/saqc/__init__.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/__main__.py` & `saqc-2.4.1/saqc/__main__.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/constants.py` & `saqc-2.4.1/saqc/constants.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/core/core.py` & `saqc-2.4.1/saqc/core/core.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/core/flags.py` & `saqc-2.4.1/saqc/core/flags.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,15 +475,14 @@
     # ----------------------------------------------------------------------
     # transformation and representation
 
     def toDios(self) -> DictOfSeries:
         """
         Transform the flags container to a ``DictOfSeries``.
 
-
         .. deprecated:: 2.4
            use `saqc.DictOfSeries(obj)` instead.
 
         Returns
         -------
         DictOfSeries
         """
```

### Comparing `saqc-2.4.0/saqc/core/frame.py` & `saqc-2.4.1/saqc/core/frame.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 #! /usr/bin/env python
 # SPDX-FileCopyrightText: 2021 Helmholtz-Zentrum für Umweltforschung GmbH - UFZ
 # SPDX-License-Identifier: GPL-3.0-or-later
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
-import warnings
 from typing import Any, Hashable, Mapping
 
-import numpy as np
 import pandas as pd
 from fancy_collections import DictOfPandas
 
 
 class DictOfSeries(DictOfPandas):
     _key_types = (str, int, float)
     _value_types = (pd.Series,)
@@ -33,44 +31,21 @@
             self._attrs = {}
         return self._attrs
 
     @attrs.setter
     def attrs(self, value: Mapping[Hashable, Any]) -> None:
         self._attrs = dict(value)
 
-    def to_df(self, how="outer") -> pd.DataFrame:
-        """
-        Transform DictOfSeries to a pandas.DataFrame.
-
-        .. deprecated:: 2.4
-           use `DictOfSeries.to_pandas()` instead.
-        """
-        warnings.warn(
-            f"`to_df()` is deprecated use `to_pandas()` instead.",
-            category=DeprecationWarning,
-        )
-        return self.to_pandas(how)
-
     def flatten(self, promote_index: bool = False) -> DictOfSeries:
         """
         Return a copy.
         DictOfPandas compatibility
         """
         return self.copy()
 
-    def to_pandas(self, how="outer"):
-        # This is a future feature from fancy_collections.DictOfPandas
-        # wich probably will come in the next version 0.1.4.
-        # We adopt this early, to prevent a second refactoring.
-        # The docstring will be different, so we keep the
-        # dynamic docstring allocation, down below.
-        # If the feature is present we just need to delete the
-        # entire method here.
-        return self.to_dataframe(how)
-
     def index_of(self, method="union") -> pd.Index:
         """Return an index with indices from all columns.
 
         .. deprecated:: 2.4
            use `DictOfSeries.union_index()` and `DictOfSeries.shared_index()` instead.
 
         Parameters
@@ -190,12 +165,7 @@
 
 or is dropped if `how='inner'`
 
 >>> di.to_pandas(how='inner')   # doctest: +NORMALIZE_WHITESPACE
       a     b     c
 1  11.0  22.0  33.0
 """
-
-
-DictOfSeries.to_dataframe.__doc__ = DictOfSeries.to_pandas.__doc__.replace(
-    "to_pandas", "to_dataframe"
-)
```

### Comparing `saqc-2.4.0/saqc/core/history.py` & `saqc-2.4.1/saqc/core/history.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/core/register.py` & `saqc-2.4.1/saqc/core/register.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/core/translation/basescheme.py` & `saqc-2.4.1/saqc/core/translation/basescheme.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/core/translation/dmpscheme.py` & `saqc-2.4.1/saqc/core/translation/dmpscheme.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/core/translation/positionalscheme.py` & `saqc-2.4.1/saqc/core/translation/positionalscheme.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/core/translation/simplescheme.py` & `saqc-2.4.1/saqc/core/translation/simplescheme.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/__init__.py` & `saqc-2.4.1/saqc/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/breaks.py` & `saqc-2.4.1/saqc/funcs/breaks.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/changepoints.py` & `saqc-2.4.1/saqc/funcs/changepoints.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/constants.py` & `saqc-2.4.1/saqc/funcs/constants.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/curvefit.py` & `saqc-2.4.1/saqc/funcs/curvefit.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/drift.py` & `saqc-2.4.1/saqc/funcs/drift.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,29 @@
 
 # -*- coding: utf-8 -*-
 
 from __future__ import annotations
 
 import functools
 import inspect
+import warnings
 from typing import TYPE_CHECKING, Callable, Optional, Sequence, Tuple
 
 import numpy as np
 import pandas as pd
 from scipy.optimize import curve_fit
 from scipy.spatial.distance import pdist
 from typing_extensions import Literal
 
 from saqc import BAD
 from saqc.core import DictOfSeries, Flags, flagging, register
 from saqc.funcs.changepoints import _getChangePoints
 from saqc.lib.docs import DOC_TEMPLATES
-from saqc.lib.tools import detectDeviants, filterKwargs, toSequence
+from saqc.lib.exceptions import ParameterOutOfBounds
+from saqc.lib.tools import detectDeviants, filterKwargs, isInBounds, toSequence
 from saqc.lib.ts_operators import expDriftModel, linearDriftModel
 from saqc.lib.types import CurveFitter
 
 if TYPE_CHECKING:
     from saqc import SaQC
 
 
@@ -49,15 +51,15 @@
         multivariate=True,
         handles_target=False,
         docstring=DOC_TEMPLATES["field"],
     )
     def flagDriftFromNorm(
         self: "SaQC",
         field: Sequence[str],
-        freq: str,
+        window: str,
         spread: float,
         frac: float = 0.5,
         metric: Callable[
             [np.ndarray | pd.Series, np.ndarray | pd.Series], np.ndarray
         ] = cityblock,
         method: LinkageString = "single",
         flag: float = BAD,
@@ -70,15 +72,15 @@
         that members of a normal group must not exceed. In addition, only a group is considered
         "normal" if it contains more then `frac` percent of the variables in "field".
 
         See the Notes section for a more detailed presentation of the algorithm
 
         Parameters
         ----------
-        freq :
+        window :
             Frequency, that split the data in chunks.
 
         spread :
             Maximum spread allowed in the group of *normal* data. See Notes section for more details.
 
         frac :
             Fraction defining the normal group. Use a value from the interval [0,1].
@@ -126,20 +128,33 @@
         References
         ----------
         Documentation of the underlying hierarchical clustering algorithm:
             [1] https://docs.scipy.org/doc/scipy/reference/generated/scipy.cluster.hierarchy.linkage.html
         Introduction to Hierarchical clustering:
             [2] https://en.wikipedia.org/wiki/Hierarchical_clustering
         """
+        if not isInBounds(frac, (0.5, 1), closed="both"):
+            raise ParameterOutOfBounds(frac, "frac", (0.5, 1), "both")
+
+        if "freq" in kwargs:
+            warnings.warn(
+                """
+                The parameter `freq` is deprecated and will be removed in version 3.0 of saqc.
+                Please us the parameter `window` instead.'
+                """,
+                DeprecationWarning,
+            )
+            window = kwargs["freq"]
+
         fields = toSequence(field)
 
         data = self._data[fields].to_pandas()
         data.dropna(inplace=True)
 
-        segments = data.groupby(pd.Grouper(freq=freq))
+        segments = data.groupby(pd.Grouper(freq=window))
         for segment in segments:
             if len(segment[1]) <= 1:
                 continue
 
             drifters = detectDeviants(
                 segment[1], metric, spread, frac, method, "variables"
             )
```

### Comparing `saqc-2.4.0/saqc/funcs/flagtools.py` & `saqc-2.4.1/saqc/funcs/flagtools.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,17 @@
         field: str,
         target: str,
         **kwargs,
     ) -> "SaQC":
         """
         Transfer Flags of one variable to another.
 
+        .. deprecated:: 2.4.0
+           Use :py:meth:`~saqc.SaQC.concatFlags` with ``method="match"`` and ``squeeze=False`` instead.
+
         See Also
         --------
         * :py:meth:`saqc.SaQC.flagGeneric`
         * :py:meth:`saqc.SaQC.concatFlags`
 
         Examples
         --------
```

### Comparing `saqc-2.4.0/saqc/funcs/generic.py` & `saqc-2.4.1/saqc/funcs/generic.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/interpolation.py` & `saqc-2.4.1/saqc/funcs/interpolation.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,14 +140,17 @@
         extrapolate: Literal["forward", "backward", "both"] | None = None,
         flag: float = UNFLAGGED,
         **kwargs,
     ) -> "SaQC":
         """
         Fill NaN and flagged values using an interpolation method.
 
+        .. deprecated:: 2.4.0
+           Use :py:meth:`~saqc.SaQC.align` instead.
+
         Parameters
         ----------
         method :
             Interpolation technique to use. One of:
 
             * ‘linear’: Ignore the index and treat the values as equally spaced.
             * ‘time’: Works on daily and higher resolution data to interpolate given length of interval.
@@ -395,14 +398,17 @@
         limit: int | None = 2,
         extrapolate: Literal["forward", "backward", "both"] = None,
         **kwargs,
     ) -> "SaQC":
         """
         Function to interpolate the data at regular (äquidistant) timestamps (or Grid points).
 
+        .. deprecated:: 2.4.0
+           Use :py:meth:`~saqc.SaQC.align` instead.
+
         Parameters
         ----------
         freq :
             An Offset String, interpreted as the frequency of
             the grid you want to interpolate your data to.
 
         method :
@@ -467,14 +473,18 @@
         method: INTERPOLATION_METHODS,
         order: int = 2,
         limit: int | None = None,
         extrapolate: Literal["forward", "backward", "both"] | None = None,
         flag: float = UNFLAGGED,
         **kwargs,
     ) -> "SaQC":
+        """
+        .. deprecated:: 2.4.0
+           Use :py:meth:`~saqc.SaQC.interpolate` instead.
+        """
         warnings.warn(
             f"""
             The method `intepolateInvalid` is deprecated and will be removed
             with version 3.0 of saqc. To achieve the same behavior, please use
             `qc.interpolate(
                 field={field}, method={method}, order={order},
                 limit={limit}, extrapolate={extrapolate}, flag={flag}
```

### Comparing `saqc-2.4.0/saqc/funcs/noise.py` & `saqc-2.4.1/saqc/funcs/noise.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/outliers.py` & `saqc-2.4.1/saqc/funcs/outliers.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/pattern.py` & `saqc-2.4.1/saqc/funcs/pattern.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/resampling.py` & `saqc-2.4.1/saqc/funcs/resampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,28 +43,38 @@
         field: str,
         freq: str,
         **kwargs,
     ) -> "SaQC":
         """
         A method to "regularize" data by interpolating linearly the data at regular timestamp.
 
-        A series of data is considered "regular", if it is sampled regularly (= having uniform sampling rate).
+        .. deprecated:: 2.4.0
+           Use :py:meth:`~saqc.SaQC.align` with ``method="linear"`` instead.
 
+        A series of data is considered "regular", if it is sampled regularly (= having uniform sampling rate).
         Interpolated values will get assigned the worst flag within freq-range.
-
         Note, that the data only gets interpolated at those (regular) timestamps, that have a valid (existing and
         not-na) datapoint preceeding them and one succeeding them within freq range.
         Regular timestamp that do not suffice this condition get nan assigned AND The associated flag will be of value
         ``UNFLAGGED``.
 
         Parameters
         ----------
         freq :
             An offset string. The frequency of the grid you want to interpolate your data at.
         """
+        warnings.warn(
+            f"""
+            The method `shift` is deprecated and will be removed with version 2.6 of saqc.
+            To achieve the same behavior please use:
+            `qc.align(field={field}, freq={freq}. method="linear")`
+            """,
+            DeprecationWarning,
+        )
+
         reserved = ["method", "order", "limit", "downgrade"]
         kwargs = filterKwargs(kwargs, reserved)
         return self.interpolateIndex(field, freq, "time", **kwargs)
 
     @register(mask=["field"], demask=[], squeeze=[])
     def shift(
         self: "SaQC",
@@ -72,14 +82,17 @@
         freq: str,
         method: Literal["fshift", "bshift", "nshift"] = "nshift",
         **kwargs,
     ) -> "SaQC":
         """
         Shift data points and flags to a regular frequency grid.
 
+        .. deprecated:: 2.4.0
+           Use :py:meth:`~saqc.SaQC.align` instead.
+
         Parameters
         ----------
         freq :
             Offset string. Sampling rate of the target frequency.
 
         method :
             Method to propagate values:
```

### Comparing `saqc-2.4.0/saqc/funcs/residuals.py` & `saqc-2.4.1/saqc/funcs/residuals.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/rolling.py` & `saqc-2.4.1/saqc/funcs/rolling.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,17 @@
         min_periods: int = 0,
         center: bool = True,
         **kwargs,
     ) -> "SaQC":
         """
         Calculate a rolling-window function on the data.
 
+        .. deprecated:: 2.4.0
+           Use :py:meth:`~saqc.SaQC.rolling` instead.
+
         Note, that the data gets assigned the worst flag present in the original data.
 
         Parameters
         ----------
         window :
             The size of the window you want to roll with. If an integer is passed, the size
             refers to the number of periods for every fitting window. If an offset string
```

### Comparing `saqc-2.4.0/saqc/funcs/scores.py` & `saqc-2.4.1/saqc/funcs/scores.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/funcs/tools.py` & `saqc-2.4.1/saqc/funcs/tools.py`

 * *Files 9% similar despite different names*

```diff
@@ -194,73 +194,82 @@
         self._flags[mask, field] = UNFLAGGED
         return self
 
     @register(mask=[], demask=[], squeeze=[])
     def plot(
         self: "SaQC",
         field: str,
-        path: Optional[str] = None,
-        max_gap: Optional[str] = None,
-        history: Optional[Literal["valid", "complete"] | list] = "valid",
-        xscope: Optional[slice] = None,
-        phaseplot: Optional[str] = None,
-        store_kwargs: Optional[dict] = None,
+        path: str | None = None,
+        max_gap: str | None = None,
+        history: Literal["valid", "complete"] | list[str] | None = "valid",
+        xscope: slice | None = None,
+        phaseplot: str | None = None,
+        store_kwargs: dict | None = None,
         ax: mpl.axes.Axes | None = None,
-        ax_kwargs: Optional[dict] = None,
+        ax_kwargs: dict | None = None,
         dfilter: float = FILTER_NONE,
         **kwargs,
     ) -> "SaQC":
         """
         Plot data and flags or store plot to file.
 
-        There are two modes, 'interactive' and 'store', which are determind through the
+        There are two modes, 'interactive' and 'store', which are determined through the
         ``save_path`` keyword. In interactive mode (default) the plot is shown at runtime
         and the program execution stops until the plot window is closed manually. In
         store mode the generated plot is stored to disk and no manually interaction is
         needed.
 
         Parameters
         ----------
         path :
             If ``None`` is passed, interactive mode is entered; plots are shown immediatly
             and a user need to close them manually before execution continues.
             If a filepath is passed instead, store-mode is entered and
             the plot is stored unter the passed location.
 
         max_gap :
-            If None, all the points in the data will be connected, resulting in long linear
-            lines, where continous chunks of data is missing. Nans in the data get dropped
-            before plotting. If an offset string is passed, only points that have a distance
-            below `max_gap` get connected via the plotting line.
+            If ``None``, all data points will be connected, resulting in long linear
+            lines, in case of large data gaps. ``NaN`` values will be removed before
+            plotting. If an offset string is passed, only points that have a distance
+            below ``max_gap`` are connected via the plotting line.
 
         history :
             Discriminate the plotted flags with respect to the tests they originate from.
 
-            * "valid" - Only plot those flags, that do not get altered or "unflagged" by subsequent tests. Only list tests
-              in the legend, that actually contributed flags to the overall resault.
-            * "complete" - plot all the flags set and list all the tests ran on a variable. Suitable for debugging/tracking.
-            * None - just plot the resulting flags for one variable, without any historical meta information.
-            * list of strings - plot only flags set by those tests listed.
+            * ``"valid"``: Only plot flags, that are not overwritten by subsequent tests.
+              Only list tests in the legend, that actually contributed flags to the overall
+              result.
+            * ``"complete"``: Plot all flags set and list all the tests executed on a variable.
+              Suitable for debugging/tracking.
+            * ``None``: Just plot the resulting flags for one variable, without any historical
+              and/or meta information.
+            * list of strings: List of tests. Plot flags from the given tests, only.
 
         xscope :
-            Parameter, that determines a chunk of the data to be plotted
-            processed. `xscope` can be anything, that is a valid argument to the ``pandas.Series.__getitem__`` method.
+            Determine a chunk of the data to be plotted processed. ``xscope`` can be anything,
+            that is a valid argument to the ``pandas.Series.__getitem__`` method.
 
         phaseplot :
-            If a string is passed, plot ``field`` in the phase space it forms together with the Variable ``phaseplot``.
+            If a string is passed, plot ``field`` in the phase space it forms together with the
+            variable ``phaseplot``.
+
+        ax :
+            If not ``None``, plot into the given ``matplotlib.Axes`` instance, instead of a
+            newly created ``matplotlib.Figure``. This option offers a possibility to integrate
+            ``SaQC`` plots into custom figure layouts.
 
         store_kwargs :
             Keywords to be passed on to the ``matplotlib.pyplot.savefig`` method, handling
             the figure storing. To store an pickle object of the figure, use the option
-            ``{'pickle': True}``, but note that all other store_kwargs are ignored then.
-            Reopen with: ``pickle.load(open(savepath,'w')).show()``
+            ``{"pickle": True}``, but note that all other ``store_kwargs`` are ignored then.
+            To reopen a pickled figure execute: ``pickle.load(open(savepath, "w")).show()``
 
         ax_kwargs :
             Axis keywords. Change the axis labeling defaults. Most important keywords:
-            'x_label', 'y_label', 'title', 'fontsize', 'cycleskip'.
+            ``"xlabel"``, ``"ylabel"``, ``"title"``, ``"fontsize"``, ``"cycleskip"``.
         """
         data, flags = self._data.copy(), self._flags.copy()
 
         level = kwargs.get("flag", UNFLAGGED)
 
         if dfilter < np.inf:
             data[field].loc[flags[field] >= dfilter] = np.nan
```

### Comparing `saqc-2.4.0/saqc/funcs/transformation.py` & `saqc-2.4.1/saqc/funcs/transformation.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/lib/docs.py` & `saqc-2.4.1/saqc/lib/docs.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/lib/plotting.py` & `saqc-2.4.1/saqc/lib/plotting.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/lib/rolling.py` & `saqc-2.4.1/saqc/lib/rolling.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/lib/tools.py` & `saqc-2.4.1/saqc/lib/tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,71 @@
 
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 import collections
 import functools
 import itertools
+import operator as op
 import re
 import warnings
-from typing import Any, Callable, Collection, List, Sequence, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Collection,
+    List,
+    Literal,
+    Sequence,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import numpy as np
 import pandas as pd
 from scipy import fft
 from scipy.cluster.hierarchy import fcluster, linkage
 
 from saqc.lib.types import CompT
 
 T = TypeVar("T", str, float, int)
+BOUND_OPERATORS = {
+    None: (op.le, op.ge),
+    "both": (op.lt, op.gt),
+    "right": (op.le, op.gt),
+    "left": (op.gt, op.le),
+}
+
+
+def isInBounds(
+    val: int | float,
+    bounds: Tuple[int | float],
+    closed: Literal["left", "right", "both"] = None,
+):
+    """
+    check if val falls into the interval [left, right] and return boolean accordingly
+
+    val :
+        value to check
+
+    bounds :
+        Tuple containing left and right interval bounds. Pass `(a, b)` to define the interval [`a`, `b`].
+        Set `a=-inf` or `b=+inf` to set one sided restriction.
+
+    closed :
+        Enclosure includes the interval bounds into the constraint interval. By default, the bounds
+        are not included. Pass:
+        * `"both"`: to include both sides of the interval
+        * `"left"`: to include left bound
+        * `"right"`: to include right bound
+    """
+    ops = BOUND_OPERATORS[closed]
+    if ops[0](val, bounds[0]) or ops[1](val, bounds[1]):
+        return False
+    return True
 
 
 def assertScalar(name, value, optional=False):
     if optional and value is None:
         return
     if np.isscalar(value):
         return
@@ -249,15 +294,14 @@
     if optimize:
         delta_f = np.abs(fft.rfft(delta, fft.next_fast_len(len(delta))))
     else:
         delta_f = np.abs(fft.rfft(delta))
 
     len_f = len(delta_f) * 2
     min_energy = delta_f[0] * min_energy
-    # calc/assign low/high freq cut offs (makes life easier):
     min_rate_i = int(
         len_f / (pd.Timedelta(min_rate).total_seconds() * (10**delta_precision))
     )
     delta_f[:min_rate_i] = 0
     max_rate_i = int(
         len_f / (pd.Timedelta(max_rate).total_seconds() * (10**delta_precision))
     )
@@ -379,15 +423,15 @@
     If yes, the according timedelta value is returned,
 
     If no, ``None`` is returned.
 
     (``None`` will also be returned for pd.RangeIndex type.)
 
     """
-    delta = getattr(index, "freq", None)
+    delta = getattr(index, "window", None)
     if delta is None and not index.empty:
         i = pd.date_range(index[0], index[-1], len(index))
         if i.equals(index):
             return i[1] - i[0]
     return delta
```

### Comparing `saqc-2.4.0/saqc/lib/ts_operators.py` & `saqc-2.4.1/saqc/lib/ts_operators.py`

 * *Files 1% similar despite different names*

```diff
@@ -547,32 +547,32 @@
     mat_[:, 1] = x
     if deg > 1:
         for n in range(2, deg + 1):
             mat_[:, n] = x**n
     return mat_
 
 
-@nb.jit
+@nb.jit(nopython=True)
 def _fitX(a, b):
     # helper function to construct numba-compatible polynomial fit function
     # linalg solves ax = b
     det_ = np.linalg.lstsq(a, b)[0]
     return det_
 
 
-@nb.jit
+@nb.jit(nopython=True)
 def _fitPoly(x, y, deg):
     # a numba compatible polynomial fit function
     a = _coeffMat(x, deg)
     p = _fitX(a, y)
     # Reverse order so p[0] is coefficient of highest order
     return p[::-1]
 
 
-@nb.jit
+@nb.jit(nopython=True)
 def evalPolynomial(P, x):
     # a numba compatible polynomial evaluator
     result = 0
     for coeff in P:
         result = x * result + coeff
     return result
```

### Comparing `saqc-2.4.0/saqc/lib/types.py` & `saqc-2.4.1/saqc/lib/types.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/parsing/environ.py` & `saqc-2.4.1/saqc/parsing/environ.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/parsing/reader.py` & `saqc-2.4.1/saqc/parsing/reader.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc/parsing/visitor.py` & `saqc-2.4.1/saqc/parsing/visitor.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/saqc.egg-info/PKG-INFO` & `saqc-2.4.1/saqc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saqc
-Version: 2.4.0
+Version: 2.4.1
 Summary: A timeseries data quality control and processing tool/framework
 Home-page: https://git.ufz.de/rdm-software/saqc
 Author: Bert Palm, David Schaefer, Florian Gransee, Peter Luenenschloss
 Author-email: david.schaefer@ufz.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `saqc-2.4.0/saqc.egg-info/SOURCES.txt` & `saqc-2.4.1/saqc.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,20 @@
 saqc.egg-info/requires.txt
 saqc.egg-info/top_level.txt
 saqc/core/__init__.py
 saqc/core/core.py
 saqc/core/flags.py
 saqc/core/frame.py
 saqc/core/history.py
+saqc/core/mixins.py
 saqc/core/register.py
 saqc/core/translation/__init__.py
 saqc/core/translation/basescheme.py
 saqc/core/translation/dmpscheme.py
+saqc/core/translation/floatscheme.py
 saqc/core/translation/positionalscheme.py
 saqc/core/translation/simplescheme.py
 saqc/funcs/__init__.py
 saqc/funcs/breaks.py
 saqc/funcs/changepoints.py
 saqc/funcs/constants.py
 saqc/funcs/curvefit.py
@@ -40,14 +42,15 @@
 saqc/funcs/residuals.py
 saqc/funcs/rolling.py
 saqc/funcs/scores.py
 saqc/funcs/tools.py
 saqc/funcs/transformation.py
 saqc/lib/__init__.py
 saqc/lib/docs.py
+saqc/lib/exceptions.py
 saqc/lib/plotting.py
 saqc/lib/rolling.py
 saqc/lib/tools.py
 saqc/lib/ts_operators.py
 saqc/lib/types.py
 saqc/parsing/__init__.py
 saqc/parsing/environ.py
@@ -78,8 +81,10 @@
 tests/funcs/test_tools.py
 tests/fuzzy/__init__.py
 tests/fuzzy/lib.py
 tests/fuzzy/test_masking.py
 tests/lib/__init__.py
 tests/lib/test_periodicMask.py
 tests/lib/test_tools.py
-tests/lib/test_ts_operators.py
+tests/lib/test_ts_operators.py
+tests/misc/__init__.py
+tests/misc/test_pickle.py
```

### Comparing `saqc-2.4.0/setup.py` & `saqc-2.4.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,21 +28,22 @@
     long_description_content_type="text/markdown",
     url="https://git.ufz.de/rdm-software/saqc",
     packages=find_packages(exclude=("tests", "docs")),
     python_requires=">=3.8",
     install_requires=[
         "Click",
         "dtw",
-        "fancy_collections",
+        "docstring_parser",
+        "fancy-collections",
         "matplotlib>=3.4",
         "numba",
         "numpy",
         "outlier-utils",
         "pyarrow",
-        "pandas",
+        "pandas>=2.0.0",
         "scikit-learn",
         "scipy",
         "typing_extensions",
     ],
     license_files=("LICENSE.md", "LICENSES/GPL-3.0-or-later.txt"),
     entry_points={
         "console_scripts": ["saqc=saqc.__main__:main"],
```

### Comparing `saqc-2.4.0/tests/api/test_creation.py` & `saqc-2.4.1/tests/api/test_creation.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/cli/test_integration.py` & `saqc-2.4.1/tests/cli/test_integration.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/core/test_core.py` & `saqc-2.4.1/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/core/test_flags.py` & `saqc-2.4.1/tests/core/test_flags.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/core/test_history.py` & `saqc-2.4.1/tests/core/test_history.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/core/test_reader.py` & `saqc-2.4.1/tests/core/test_reader.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/core/test_translator.py` & `saqc-2.4.1/tests/core/test_translator.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_constants_detection.py` & `saqc-2.4.1/tests/funcs/test_constants_detection.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_flagtools.py` & `saqc-2.4.1/tests/funcs/test_flagtools.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_functions.py` & `saqc-2.4.1/tests/funcs/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,15 @@
     data["field3"] = dat(periods=200, peak_level=100, name="field3")[0]["field3"]
 
     fields = ["field1", "field2", "field3"]
 
     flags = initFlagsLike(data)
     qc = SaQC(data, flags).flagDriftFromNorm(
         field=fields,
-        freq="200min",
+        window="200min",
         spread=5,
         flag=BAD,
     )
     assert all(qc._flags["field3"] > UNFLAGGED)
 
 
 @pytest.mark.parametrize("dat", [pytest.lazy_fixture("course_1")])
```

### Comparing `saqc-2.4.0/tests/funcs/test_generic_api_functions.py` & `saqc-2.4.1/tests/funcs/test_generic_api_functions.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_generic_config_functions.py` & `saqc-2.4.1/tests/funcs/test_generic_config_functions.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_outlier_detection.py` & `saqc-2.4.1/tests/funcs/test_outlier_detection.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_pattern_rec.py` & `saqc-2.4.1/tests/funcs/test_pattern_rec.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_proc_functions.py` & `saqc-2.4.1/tests/funcs/test_proc_functions.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_resampling.py` & `saqc-2.4.1/tests/funcs/test_resampling.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/funcs/test_tools.py` & `saqc-2.4.1/tests/funcs/test_tools.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/fuzzy/lib.py` & `saqc-2.4.1/tests/fuzzy/lib.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/fuzzy/test_masking.py` & `saqc-2.4.1/tests/fuzzy/test_masking.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/lib/test_periodicMask.py` & `saqc-2.4.1/tests/lib/test_periodicMask.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/lib/test_tools.py` & `saqc-2.4.1/tests/lib/test_tools.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/lib/test_ts_operators.py` & `saqc-2.4.1/tests/lib/test_ts_operators.py`

 * *Files identical despite different names*

### Comparing `saqc-2.4.0/tests/test__main__.py` & `saqc-2.4.1/tests/test__main__.py`

 * *Files identical despite different names*

