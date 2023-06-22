# Comparing `tmp/obsln-0.0.2.tar.gz` & `tmp/obsln-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsln-0.0.2.tar", last modified: Fri Jun  9 17:17:01 2023, max compression
+gzip compressed data, was "obsln-0.0.3.tar", last modified: Thu Jun 22 10:36:44 2023, max compression
```

## Comparing `obsln-0.0.2.tar` & `obsln-0.0.3.tar`

### file list

```diff
@@ -1,81 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:01.091807 obsln-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1607 2023-06-09 17:17:01.086657 obsln-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-09 16:14:18.000000 obsln-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:16:59.854859 obsln-0.0.2/obsln/
--rw-r--r--   0 root         (0) root         (0)     1710 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.082861 obsln-0.0.2/obsln/core/
--rw-r--r--   0 root         (0) root         (0)     1698 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8880 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/compatibility.py
--rw-r--r--   0 root         (0) root         (0)     1628 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/futureutils.py
--rw-r--r--   0 root         (0) root         (0)   156910 2021-12-07 11:48:32.000000 obsln-0.0.2/obsln/core/stream.py
--rw-r--r--   0 root         (0) root         (0)   124491 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/trace.py
--rw-r--r--   0 root         (0) root         (0)    59441 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/utcdatetime.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.201952 obsln-0.0.2/obsln/core/util/
--rw-r--r--   0 root         (0) root         (0)     2269 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7929 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/util/attribdict.py
--rw-r--r--   0 root         (0) root         (0)    32827 2021-12-07 11:48:32.000000 obsln-0.0.2/obsln/core/util/base.py
--rw-r--r--   0 root         (0) root         (0)    12709 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/util/decorator.py
--rw-r--r--   0 root         (0) root         (0)     6000 2021-06-11 09:23:04.000000 obsln-0.0.2/obsln/core/util/libnames.py
--rw-r--r--   0 root         (0) root         (0)    29058 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/core/util/misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.219894 obsln-0.0.2/obsln/io/
--rw-r--r--   0 root         (0) root         (0)     1513 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.286390 obsln-0.0.2/obsln/io/seg2/
--rw-r--r--   0 root         (0) root         (0)      827 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/README.txt
--rw-r--r--   0 root         (0) root         (0)      630 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/header.py
--rw-r--r--   0 root         (0) root         (0)    14940 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/seg2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.324162 obsln-0.0.2/obsln/io/seg2/tests/
--rw-r--r--   0 root         (0) root         (0)      485 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.379612 obsln-0.0.2/obsln/io/seg2/tests/data/
--rw-r--r--   0 root         (0) root         (0)    10829 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.DAT.gz
--rw-r--r--   0 root         (0) root         (0)     7718 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.seg2.gz
--rw-r--r--   0 root         (0) root         (0)    14639 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/tests/data/20180307_031245000.0.DAT.gz
--rw-r--r--   0 root         (0) root         (0)     5530 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/seg2/tests/test_seg2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.536661 obsln-0.0.2/obsln/io/segy/
--rw-r--r--   0 root         (0) root         (0)      860 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/README.txt
--rw-r--r--   0 root         (0) root         (0)    12011 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32149 2021-12-07 11:48:32.000000 obsln-0.0.2/obsln/io/segy/core.py
--rw-r--r--   0 root         (0) root         (0)    10465 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/header.py
--rw-r--r--   0 root         (0) root         (0)     6391 2021-06-11 08:35:55.000000 obsln-0.0.2/obsln/io/segy/pack.py
--rw-r--r--   0 root         (0) root         (0)    61511 2021-12-07 11:48:32.000000 obsln-0.0.2/obsln/io/segy/segy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.561871 obsln-0.0.2/obsln/io/segy/src/
--rw-r--r--   0 root         (0) root         (0)     1815 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/src/ibm2ieee.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:00.679991 obsln-0.0.2/obsln/io/segy/tests/
--rw-r--r--   0 root         (0) root         (0)     1066 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:17:01.068961 obsln-0.0.2/obsln/io/segy/tests/data/
--rw-r--r--   0 root         (0) root         (0)    11844 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/00001034.sgy_first_trace
--rw-r--r--   0 root         (0) root         (0)     8084 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/00001034.sgy_first_trace.npy
--rw-r--r--   0 root         (0) root         (0)    35840 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/1.sgy_first_trace
--rw-r--r--   0 root         (0) root         (0)    32080 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/1.sgy_first_trace.npy
--rw-r--r--   0 root         (0) root         (0)    32240 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/1.su_first_trace
--rw-r--r--   0 root         (0) root         (0)     4840 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/example.y_first_trace
--rw-r--r--   0 root         (0) root         (0)     2080 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/example.y_first_trace.npy
--rw-r--r--   0 root         (0) root         (0)    12040 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace
--rw-r--r--   0 root         (0) root         (0)     8280 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace.npy
--rw-r--r--   0 root         (0) root         (0)    35840 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_11.sgy
--rw-r--r--   0 root         (0) root         (0)    32080 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_11.sgy.npy
--rw-r--r--   0 root         (0) root         (0)    32240 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_11.su
--rw-r--r--   0 root         (0) root         (0)    35840 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_99.sgy
--rw-r--r--   0 root         (0) root         (0)    32080 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_99.sgy.npy
--rw-r--r--   0 root         (0) root         (0)    32240 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_99.su
--rw-r--r--   0 root         (0) root         (0)     5888 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/planes.segy_first_trace
--rw-r--r--   0 root         (0) root         (0)     2128 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/planes.segy_first_trace.npy
--rw-r--r--   0 root         (0) root         (0)     1175 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/data/readme.txt
--rw-r--r--   0 root         (0) root         (0)     3335 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/header.py
--rw-r--r--   0 root         (0) root         (0)    30280 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/test_core.py
--rw-r--r--   0 root         (0) root         (0)    36321 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/test_segy.py
--rw-r--r--   0 root         (0) root         (0)     5150 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/tests/test_su.py
--rw-r--r--   0 root         (0) root         (0)     6225 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/unpack.py
--rw-r--r--   0 root         (0) root         (0)     2317 2021-04-21 14:38:19.000000 obsln-0.0.2/obsln/io/segy/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 17:16:59.967806 obsln-0.0.2/obsln.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1607 2023-06-09 17:16:59.000000 obsln-0.0.2/obsln.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-09 17:16:59.000000 obsln-0.0.2/obsln.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 17:16:59.000000 obsln-0.0.2/obsln.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      707 2023-06-09 17:16:59.000000 obsln-0.0.2/obsln.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 17:16:59.000000 obsln-0.0.2/obsln.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 17:16:58.000000 obsln-0.0.2/obsln.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       31 2023-06-09 17:16:59.000000 obsln-0.0.2/obsln.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-09 17:16:59.000000 obsln-0.0.2/obsln.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      681 2023-06-09 17:16:47.000000 obsln-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 17:17:01.094913 obsln-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)    27189 2023-06-09 17:12:54.000000 obsln-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:44.561547 obsln-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-06-22 10:36:44.557074 obsln-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-06-09 16:14:18.000000 obsln-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:43.580669 obsln-0.0.3/obsln/
+-rw-r--r--   0 root         (0) root         (0)     1710 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:43.783071 obsln-0.0.3/obsln/core/
+-rw-r--r--   0 root         (0) root         (0)     1698 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8880 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/compatibility.py
+-rw-r--r--   0 root         (0) root         (0)     1628 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/futureutils.py
+-rw-r--r--   0 root         (0) root         (0)   156910 2021-12-07 11:48:32.000000 obsln-0.0.3/obsln/core/stream.py
+-rw-r--r--   0 root         (0) root         (0)   124491 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/trace.py
+-rw-r--r--   0 root         (0) root         (0)    59441 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/utcdatetime.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:43.880090 obsln-0.0.3/obsln/core/util/
+-rw-r--r--   0 root         (0) root         (0)     2269 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7929 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/util/attribdict.py
+-rw-r--r--   0 root         (0) root         (0)    32827 2021-12-07 11:48:32.000000 obsln-0.0.3/obsln/core/util/base.py
+-rw-r--r--   0 root         (0) root         (0)    12709 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/util/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     6000 2021-06-11 09:23:04.000000 obsln-0.0.3/obsln/core/util/libnames.py
+-rw-r--r--   0 root         (0) root         (0)    29058 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/core/util/misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:43.898704 obsln-0.0.3/obsln/io/
+-rw-r--r--   0 root         (0) root         (0)     1513 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:43.954031 obsln-0.0.3/obsln/io/seg2/
+-rw-r--r--   0 root         (0) root         (0)      827 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/README.txt
+-rw-r--r--   0 root         (0) root         (0)      630 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/header.py
+-rw-r--r--   0 root         (0) root         (0)    14940 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/seg2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:43.982103 obsln-0.0.3/obsln/io/seg2/tests/
+-rw-r--r--   0 root         (0) root         (0)      485 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:44.028947 obsln-0.0.3/obsln/io/seg2/tests/data/
+-rw-r--r--   0 root         (0) root         (0)    10829 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.DAT.gz
+-rw-r--r--   0 root         (0) root         (0)     7718 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.seg2.gz
+-rw-r--r--   0 root         (0) root         (0)    14639 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/tests/data/20180307_031245000.0.DAT.gz
+-rw-r--r--   0 root         (0) root         (0)     5530 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/seg2/tests/test_seg2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:44.169563 obsln-0.0.3/obsln/io/segy/
+-rw-r--r--   0 root         (0) root         (0)      860 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/README.txt
+-rw-r--r--   0 root         (0) root         (0)    12011 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32149 2021-12-07 11:48:32.000000 obsln-0.0.3/obsln/io/segy/core.py
+-rw-r--r--   0 root         (0) root         (0)    10465 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/header.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2021-06-11 08:35:55.000000 obsln-0.0.3/obsln/io/segy/pack.py
+-rw-r--r--   0 root         (0) root         (0)    61511 2021-12-07 11:48:32.000000 obsln-0.0.3/obsln/io/segy/segy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:44.189849 obsln-0.0.3/obsln/io/segy/src/
+-rw-r--r--   0 root         (0) root         (0)     1815 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/src/ibm2ieee.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:44.265835 obsln-0.0.3/obsln/io/segy/tests/
+-rw-r--r--   0 root         (0) root         (0)     1066 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:44.547216 obsln-0.0.3/obsln/io/segy/tests/data/
+-rw-r--r--   0 root         (0) root         (0)    11844 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/00001034.sgy_first_trace
+-rw-r--r--   0 root         (0) root         (0)     8084 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/00001034.sgy_first_trace.npy
+-rw-r--r--   0 root         (0) root         (0)    35840 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/1.sgy_first_trace
+-rw-r--r--   0 root         (0) root         (0)    32080 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/1.sgy_first_trace.npy
+-rw-r--r--   0 root         (0) root         (0)    32240 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/1.su_first_trace
+-rw-r--r--   0 root         (0) root         (0)     4840 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/example.y_first_trace
+-rw-r--r--   0 root         (0) root         (0)     2080 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/example.y_first_trace.npy
+-rw-r--r--   0 root         (0) root         (0)    12040 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace
+-rw-r--r--   0 root         (0) root         (0)     8280 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace.npy
+-rw-r--r--   0 root         (0) root         (0)    35840 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_11.sgy
+-rw-r--r--   0 root         (0) root         (0)    32080 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_11.sgy.npy
+-rw-r--r--   0 root         (0) root         (0)    32240 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_11.su
+-rw-r--r--   0 root         (0) root         (0)    35840 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_99.sgy
+-rw-r--r--   0 root         (0) root         (0)    32080 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_99.sgy.npy
+-rw-r--r--   0 root         (0) root         (0)    32240 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_99.su
+-rw-r--r--   0 root         (0) root         (0)     5888 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/planes.segy_first_trace
+-rw-r--r--   0 root         (0) root         (0)     2128 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/planes.segy_first_trace.npy
+-rw-r--r--   0 root         (0) root         (0)     1175 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/data/readme.txt
+-rw-r--r--   0 root         (0) root         (0)     3335 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/header.py
+-rw-r--r--   0 root         (0) root         (0)    30280 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/test_core.py
+-rw-r--r--   0 root         (0) root         (0)    36321 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/test_segy.py
+-rw-r--r--   0 root         (0) root         (0)     5150 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/tests/test_su.py
+-rw-r--r--   0 root         (0) root         (0)     6225 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/unpack.py
+-rw-r--r--   0 root         (0) root         (0)     2317 2021-04-21 14:38:19.000000 obsln-0.0.3/obsln/io/segy/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 10:36:43.693453 obsln-0.0.3/obsln.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1607 2023-06-22 10:36:43.000000 obsln-0.0.3/obsln.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2196 2023-06-22 10:36:43.000000 obsln-0.0.3/obsln.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:36:43.000000 obsln-0.0.3/obsln.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-22 10:36:43.000000 obsln-0.0.3/obsln.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:36:43.000000 obsln-0.0.3/obsln.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 10:36:42.000000 obsln-0.0.3/obsln.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-22 10:36:43.000000 obsln-0.0.3/obsln.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      714 2023-06-22 10:36:32.000000 obsln-0.0.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 10:36:44.564960 obsln-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    27189 2023-06-09 17:12:54.000000 obsln-0.0.3/setup.py
```

### Comparing `obsln-0.0.2/PKG-INFO` & `obsln-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsln
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very limited range of functionality from ObsPy without many of the dependencies and size
 Author: Bateared Collie
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/batearedcollie/obsln
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `obsln-0.0.2/README.md` & `obsln-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/__init__.py` & `obsln-0.0.3/obsln/__init__.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/__init__.py` & `obsln-0.0.3/obsln/core/__init__.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/compatibility.py` & `obsln-0.0.3/obsln/core/compatibility.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/futureutils.py` & `obsln-0.0.3/obsln/core/futureutils.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/stream.py` & `obsln-0.0.3/obsln/core/stream.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/trace.py` & `obsln-0.0.3/obsln/core/trace.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/utcdatetime.py` & `obsln-0.0.3/obsln/core/utcdatetime.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/util/__init__.py` & `obsln-0.0.3/obsln/core/util/__init__.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/util/attribdict.py` & `obsln-0.0.3/obsln/core/util/attribdict.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/util/base.py` & `obsln-0.0.3/obsln/core/util/base.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/util/decorator.py` & `obsln-0.0.3/obsln/core/util/decorator.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/util/libnames.py` & `obsln-0.0.3/obsln/core/util/libnames.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/core/util/misc.py` & `obsln-0.0.3/obsln/core/util/misc.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/__init__.py` & `obsln-0.0.3/obsln/io/__init__.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/README.txt` & `obsln-0.0.3/obsln/io/seg2/README.txt`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/__init__.py` & `obsln-0.0.3/obsln/io/seg2/__init__.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/header.py` & `obsln-0.0.3/obsln/io/seg2/header.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/seg2.py` & `obsln-0.0.3/obsln/io/seg2/seg2.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.DAT.gz` & `obsln-0.0.3/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.DAT.gz`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.seg2.gz` & `obsln-0.0.3/obsln/io/seg2/tests/data/20130107_103041000.CET.3c.cont.0.seg2.gz`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/tests/data/20180307_031245000.0.DAT.gz` & `obsln-0.0.3/obsln/io/seg2/tests/data/20180307_031245000.0.DAT.gz`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/seg2/tests/test_seg2.py` & `obsln-0.0.3/obsln/io/seg2/tests/test_seg2.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/README.txt` & `obsln-0.0.3/obsln/io/segy/README.txt`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/__init__.py` & `obsln-0.0.3/obsln/io/segy/__init__.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/core.py` & `obsln-0.0.3/obsln/io/segy/core.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/header.py` & `obsln-0.0.3/obsln/io/segy/header.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/pack.py` & `obsln-0.0.3/obsln/io/segy/pack.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/segy.py` & `obsln-0.0.3/obsln/io/segy/segy.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/src/ibm2ieee.c` & `obsln-0.0.3/obsln/io/segy/src/ibm2ieee.c`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/__init__.py` & `obsln-0.0.3/obsln/io/segy/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/00001034.sgy_first_trace` & `obsln-0.0.3/obsln/io/segy/tests/data/00001034.sgy_first_trace`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/00001034.sgy_first_trace.npy` & `obsln-0.0.3/obsln/io/segy/tests/data/00001034.sgy_first_trace.npy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/1.sgy_first_trace` & `obsln-0.0.3/obsln/io/segy/tests/data/1.sgy_first_trace`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/1.sgy_first_trace.npy` & `obsln-0.0.3/obsln/io/segy/tests/data/1.sgy_first_trace.npy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/1.su_first_trace` & `obsln-0.0.3/obsln/io/segy/tests/data/1.su_first_trace`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/example.y_first_trace` & `obsln-0.0.3/obsln/io/segy/tests/data/example.y_first_trace`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/example.y_first_trace.npy` & `obsln-0.0.3/obsln/io/segy/tests/data/example.y_first_trace.npy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace` & `obsln-0.0.3/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace.npy` & `obsln-0.0.3/obsln/io/segy/tests/data/ld0042_file_00018.sgy_first_trace.npy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_11.sgy` & `obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_11.sgy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_11.sgy.npy` & `obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_11.sgy.npy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_11.su` & `obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_11.su`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_99.sgy` & `obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_99.sgy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_99.sgy.npy` & `obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_99.sgy.npy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/one_trace_year_99.su` & `obsln-0.0.3/obsln/io/segy/tests/data/one_trace_year_99.su`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/planes.segy_first_trace` & `obsln-0.0.3/obsln/io/segy/tests/data/planes.segy_first_trace`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/planes.segy_first_trace.npy` & `obsln-0.0.3/obsln/io/segy/tests/data/planes.segy_first_trace.npy`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/data/readme.txt` & `obsln-0.0.3/obsln/io/segy/tests/data/readme.txt`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/header.py` & `obsln-0.0.3/obsln/io/segy/tests/header.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/test_core.py` & `obsln-0.0.3/obsln/io/segy/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/test_segy.py` & `obsln-0.0.3/obsln/io/segy/tests/test_segy.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/tests/test_su.py` & `obsln-0.0.3/obsln/io/segy/tests/test_su.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/unpack.py` & `obsln-0.0.3/obsln/io/segy/unpack.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln/io/segy/util.py` & `obsln-0.0.3/obsln/io/segy/util.py`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/obsln.egg-info/PKG-INFO` & `obsln-0.0.3/obsln.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsln
-Version: 0.0.2
+Version: 0.0.3
 Summary: A very limited range of functionality from ObsPy without many of the dependencies and size
 Author: Bateared Collie
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/batearedcollie/obsln
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `obsln-0.0.2/obsln.egg-info/SOURCES.txt` & `obsln-0.0.3/obsln.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 obsln/__init__.py
 obsln.egg-info/PKG-INFO
 obsln.egg-info/SOURCES.txt
 obsln.egg-info/dependency_links.txt
 obsln.egg-info/entry_points.txt
 obsln.egg-info/namespace_packages.txt
 obsln.egg-info/not-zip-safe
-obsln.egg-info/requires.txt
 obsln.egg-info/top_level.txt
 obsln/core/__init__.py
 obsln/core/compatibility.py
 obsln/core/futureutils.py
 obsln/core/stream.py
 obsln/core/trace.py
 obsln/core/utcdatetime.py
```

### Comparing `obsln-0.0.2/obsln.egg-info/entry_points.txt` & `obsln-0.0.3/obsln.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `obsln-0.0.2/pyproject.toml` & `obsln-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+#requires = ["setuptools>=61.0","numpy>=1.18.2","decorator>=4.4.2"]
+requires = ["setuptools>=59.6","numpy>=1.18.2","decorator>=4.4.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "obsln"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A very limited range of functionality from ObsPy without many of the dependencies and size"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
     "Operating System :: OS Independent",
 ]
 
-dependencies = ["decorator>=4.4.2",
-                "numpy>=1.18.2"]
-
 [project.urls]
 "Homepage" = "https://github.com/batearedcollie/obsln"
```

### Comparing `obsln-0.0.2/setup.py` & `obsln-0.0.3/setup.py`

 * *Files identical despite different names*

