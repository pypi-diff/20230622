# Comparing `tmp/pipeline_viz-0.1.0.tar.gz` & `tmp/pipeline_viz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_viz-0.1.0.tar", last modified: Thu Jun 22 04:59:30 2023, max compression
+gzip compressed data, was "pipeline_viz-0.1.1.tar", last modified: Thu Jun 22 05:36:13 2023, max compression
```

## Comparing `pipeline_viz-0.1.0.tar` & `pipeline_viz-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 04:59:30.374943 pipeline_viz-0.1.0/
--rw-r--r--   0 priti      (501) staff       (20)     1068 2023-06-21 21:56:09.000000 pipeline_viz-0.1.0/LICENSE
--rw-r--r--   0 priti      (501) staff       (20)      291 2023-06-22 04:59:30.374432 pipeline_viz-0.1.0/PKG-INFO
--rw-r--r--   0 priti      (501) staff       (20)      277 2023-06-21 21:56:09.000000 pipeline_viz-0.1.0/README.md
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 04:59:30.365106 pipeline_viz-0.1.0/pipeline_viz/
--rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:17:34.000000 pipeline_viz-0.1.0/pipeline_viz/__init__.py
--rw-r--r--   0 priti      (501) staff       (20)     8142 2023-06-22 04:50:51.000000 pipeline_viz-0.1.0/pipeline_viz/pipeline_viz.py
--rw-r--r--   0 priti      (501) staff       (20)      454 2023-06-21 21:17:24.000000 pipeline_viz-0.1.0/pipeline_viz/utils.py
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 04:59:30.368000 pipeline_viz-0.1.0/pipeline_viz.egg-info/
--rw-r--r--   0 priti      (501) staff       (20)      291 2023-06-22 04:59:30.000000 pipeline_viz-0.1.0/pipeline_viz.egg-info/PKG-INFO
--rw-r--r--   0 priti      (501) staff       (20)      349 2023-06-22 04:59:30.000000 pipeline_viz-0.1.0/pipeline_viz.egg-info/SOURCES.txt
--rw-r--r--   0 priti      (501) staff       (20)        1 2023-06-22 04:59:30.000000 pipeline_viz-0.1.0/pipeline_viz.egg-info/dependency_links.txt
--rw-r--r--   0 priti      (501) staff       (20)       46 2023-06-22 04:59:30.000000 pipeline_viz-0.1.0/pipeline_viz.egg-info/requires.txt
--rw-r--r--   0 priti      (501) staff       (20)       19 2023-06-22 04:59:30.000000 pipeline_viz-0.1.0/pipeline_viz.egg-info/top_level.txt
--rw-r--r--   0 priti      (501) staff       (20)       38 2023-06-22 04:59:30.375060 pipeline_viz-0.1.0/setup.cfg
--rw-r--r--   0 priti      (501) staff       (20)      408 2023-06-21 21:39:46.000000 pipeline_viz-0.1.0/setup.py
-drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 04:59:30.372439 pipeline_viz-0.1.0/tests/
--rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:42:27.000000 pipeline_viz-0.1.0/tests/__init__.py
--rw-r--r--   0 priti      (501) staff       (20)     1189 2023-06-22 04:48:12.000000 pipeline_viz-0.1.0/tests/pipeline_test.py
--rw-r--r--   0 priti      (501) staff       (20)     1342 2023-06-21 21:17:20.000000 pipeline_viz-0.1.0/tests/test_pipeline_viz.py
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.712960 pipeline_viz-0.1.1/
+-rw-r--r--   0 priti      (501) staff       (20)     1068 2023-06-21 21:56:09.000000 pipeline_viz-0.1.1/LICENSE
+-rw-r--r--   0 priti      (501) staff       (20)     3116 2023-06-22 05:36:13.712499 pipeline_viz-0.1.1/PKG-INFO
+-rw-r--r--   0 priti      (501) staff       (20)     2784 2023-06-22 05:31:27.000000 pipeline_viz-0.1.1/README.md
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.701622 pipeline_viz-0.1.1/pipeline_viz/
+-rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:17:34.000000 pipeline_viz-0.1.1/pipeline_viz/__init__.py
+-rw-r--r--   0 priti      (501) staff       (20)     8142 2023-06-22 04:50:51.000000 pipeline_viz-0.1.1/pipeline_viz/pipeline_viz.py
+-rw-r--r--   0 priti      (501) staff       (20)      454 2023-06-21 21:17:24.000000 pipeline_viz-0.1.1/pipeline_viz/utils.py
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.706110 pipeline_viz-0.1.1/pipeline_viz.egg-info/
+-rw-r--r--   0 priti      (501) staff       (20)     3116 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/PKG-INFO
+-rw-r--r--   0 priti      (501) staff       (20)      349 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/SOURCES.txt
+-rw-r--r--   0 priti      (501) staff       (20)        1 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/dependency_links.txt
+-rw-r--r--   0 priti      (501) staff       (20)       46 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/requires.txt
+-rw-r--r--   0 priti      (501) staff       (20)       19 2023-06-22 05:36:13.000000 pipeline_viz-0.1.1/pipeline_viz.egg-info/top_level.txt
+-rw-r--r--   0 priti      (501) staff       (20)       38 2023-06-22 05:36:13.713119 pipeline_viz-0.1.1/setup.cfg
+-rw-r--r--   0 priti      (501) staff       (20)      593 2023-06-22 05:31:52.000000 pipeline_viz-0.1.1/setup.py
+drwxr-xr-x   0 priti      (501) staff       (20)        0 2023-06-22 05:36:13.709816 pipeline_viz-0.1.1/tests/
+-rw-r--r--   0 priti      (501) staff       (20)      101 2023-06-21 21:42:27.000000 pipeline_viz-0.1.1/tests/__init__.py
+-rw-r--r--   0 priti      (501) staff       (20)     1189 2023-06-22 04:48:12.000000 pipeline_viz-0.1.1/tests/pipeline_test.py
+-rw-r--r--   0 priti      (501) staff       (20)     1342 2023-06-21 21:17:20.000000 pipeline_viz-0.1.1/tests/test_pipeline_viz.py
```

### Comparing `pipeline_viz-0.1.0/LICENSE` & `pipeline_viz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_viz-0.1.0/pipeline_viz/pipeline_viz.py` & `pipeline_viz-0.1.1/pipeline_viz/pipeline_viz.py`

 * *Files identical despite different names*

### Comparing `pipeline_viz-0.1.0/tests/pipeline_test.py` & `pipeline_viz-0.1.1/tests/pipeline_test.py`

 * *Files identical despite different names*

### Comparing `pipeline_viz-0.1.0/tests/test_pipeline_viz.py` & `pipeline_viz-0.1.1/tests/test_pipeline_viz.py`

 * *Files identical despite different names*

