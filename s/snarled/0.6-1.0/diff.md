# Comparing `tmp/snarled-0.6.tar.gz` & `tmp/snarled-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snarled-0.6.tar", last modified: Fri Apr  8 04:45:58 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `snarled-0.6.tar` & `snarled-1.0.tar`

### file list

```diff
@@ -1,25 +1,16 @@
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-04-08 04:45:58.185805 snarled-0.6/
--rw-r--r--   0 jan       (1000) jan       (1000)    34904 2022-03-28 04:55:34.000000 snarled-0.6/LICENSE.md
--rw-r--r--   0 jan       (1000) jan       (1000)     4051 2022-04-08 04:45:58.185805 snarled-0.6/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)     3106 2022-04-05 06:23:24.000000 snarled-0.6/README.md
--rw-r--r--   0 jan       (1000) jan       (1000)       38 2022-04-08 04:45:58.185805 snarled-0.6/setup.cfg
--rw-r--r--   0 jan       (1000) jan       (1000)     1739 2022-03-31 07:39:01.000000 snarled-0.6/setup.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-04-08 04:45:58.181805 snarled-0.6/snarled/
--rw-r--r--   0 jan       (1000) jan       (1000)      133 2022-04-08 04:45:41.000000 snarled-0.6/snarled/VERSION.py
--rw-r--r--   0 jan       (1000) jan       (1000)      705 2022-04-05 06:26:18.000000 snarled-0.6/snarled/__init__.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1869 2022-04-06 01:24:44.000000 snarled-0.6/snarled/clipper.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-04-08 04:45:58.185805 snarled-0.6/snarled/interfaces/
--rw-r--r--   0 jan       (1000) jan       (1000)        0 2022-03-28 06:37:43.000000 snarled-0.6/snarled/interfaces/__init__.py
--rw-r--r--   0 jan       (1000) jan       (1000)     4360 2022-04-06 01:24:11.000000 snarled-0.6/snarled/interfaces/masque.py
--rw-r--r--   0 jan       (1000) jan       (1000)    15307 2022-04-08 04:45:30.000000 snarled-0.6/snarled/main.py
--rw-r--r--   0 jan       (1000) jan       (1000)     5119 2022-04-08 04:45:30.000000 snarled-0.6/snarled/poly.py
--rw-r--r--   0 jan       (1000) jan       (1000)        0 2022-03-28 06:45:04.000000 snarled-0.6/snarled/py.typed
--rw-r--r--   0 jan       (1000) jan       (1000)     5175 2022-04-05 06:26:18.000000 snarled-0.6/snarled/tracker.py
--rw-r--r--   0 jan       (1000) jan       (1000)      192 2022-03-31 07:07:04.000000 snarled-0.6/snarled/types.py
--rw-r--r--   0 jan       (1000) jan       (1000)      745 2022-03-31 07:07:04.000000 snarled-0.6/snarled/utils.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2022-04-08 04:45:58.185805 snarled-0.6/snarled.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)     4051 2022-04-08 04:45:57.000000 snarled-0.6/snarled.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      403 2022-04-08 04:45:57.000000 snarled-0.6/snarled.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2022-04-08 04:45:57.000000 snarled-0.6/snarled.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) jan       (1000)       81 2022-04-08 04:45:57.000000 snarled-0.6/snarled.egg-info/requires.txt
--rw-r--r--   0 jan       (1000) jan       (1000)        8 2022-04-08 04:45:57.000000 snarled-0.6/snarled.egg-info/top_level.txt
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 snarled-1.0/.flake8
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 snarled-1.0/examples/check.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 snarled-1.0/examples/connectivity.txt
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 snarled-1.0/examples/layermap.txt
+-rwxr-xr-x   0        0        0      147 2020-02-02 00:00:00.000000 snarled-1.0/examples/run.sh
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 snarled-1.0/snarled/__init__.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 snarled-1.0/snarled/__main__.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 snarled-1.0/snarled/main.py
+-rw-r--r--   0        0        0    10550 2020-02-02 00:00:00.000000 snarled-1.0/snarled/trace.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 snarled-1.0/snarled/types.py
+-rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 snarled-1.0/snarled/utils.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snarled-1.0/.gitignore
+-rw-r--r--   0        0        0    34904 2020-02-02 00:00:00.000000 snarled-1.0/LICENSE.md
+-rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 snarled-1.0/README.md
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 snarled-1.0/pyproject.toml
+-rw-r--r--   0        0        0    42996 2020-02-02 00:00:00.000000 snarled-1.0/PKG-INFO
```

### Comparing `snarled-0.6/LICENSE.md` & `snarled-1.0/LICENSE.md`

 * *Files identical despite different names*

