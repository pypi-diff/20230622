# Comparing `tmp/snapatac2-2.3.0.tar.gz` & `tmp/snapatac2-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapatac2-2.3.0.tar", last modified: Sat Apr 15 05:58:14 2023, max compression
+gzip compressed data, was "snapatac2-2.3.1.tar", last modified: Thu Jun 22 16:01:45 2023, max compression
```

## Comparing `snapatac2-2.3.0.tar` & `snapatac2-2.3.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-15 05:58:10.000000 snapatac2-2.3.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-15 05:58:10.000000 snapatac2-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-15 05:58:10.000000 snapatac2-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-15 05:58:14.214284 snapatac2-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-15 05:58:10.000000 snapatac2-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-15 05:58:10.000000 snapatac2-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 05:58:14.214284 snapatac2-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-15 05:58:10.000000 snapatac2-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/genome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)    11720 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/plotting/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/plotting/_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21050 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_harmony.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_knn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_mnn_correct.py
--rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/preprocessing/_scrublet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/snapatac2/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_call_peaks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    15443 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_motif.py
--rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-04-15 05:58:10.000000 snapatac2-2.3.0/snapatac2/tools/_smooth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.210284 snapatac2-2.3.0/snapatac2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 05:58:14.000000 snapatac2-2.3.0/snapatac2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/call_peaks.rs
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/embedding.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/export.rs
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/motif.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/network.rs
--rw-r--r--   0 runner    (1001) docker     (123)     7971 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/preprocessing.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/utils/anndata.rs
--rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-04-15 05:58:10.000000 snapatac2-2.3.0/src/utils.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 05:58:14.214284 snapatac2-2.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-04-15 05:58:10.000000 snapatac2-2.3.0/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.164649 snapatac2-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-22 16:01:39.000000 snapatac2-2.3.1/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 16:01:39.000000 snapatac2-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 16:01:39.000000 snapatac2-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 16:01:45.164649 snapatac2-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 16:01:39.000000 snapatac2-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-22 16:01:39.000000 snapatac2-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:01:45.164649 snapatac2-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-22 16:01:39.000000 snapatac2-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.160649 snapatac2-2.3.1/snapatac2/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.160649 snapatac2-2.3.1/snapatac2/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/genome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.160649 snapatac2-2.3.1/snapatac2/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/plotting/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/plotting/_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.160649 snapatac2-2.3.1/snapatac2/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23906 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/preprocessing/_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/preprocessing/_harmony.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/preprocessing/_knn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/preprocessing/_mnn_correct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/preprocessing/_scrublet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.164649 snapatac2-2.3.1/snapatac2/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_call_peaks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9214 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16916 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10992 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_motif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19635 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-22 16:01:39.000000 snapatac2-2.3.1/snapatac2/tools/_smooth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.160649 snapatac2-2.3.1/snapatac2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-22 16:01:45.000000 snapatac2-2.3.1/snapatac2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-06-22 16:01:45.000000 snapatac2-2.3.1/snapatac2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:01:45.000000 snapatac2-2.3.1/snapatac2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:01:45.000000 snapatac2-2.3.1/snapatac2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-22 16:01:45.000000 snapatac2-2.3.1/snapatac2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 16:01:45.000000 snapatac2-2.3.1/snapatac2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.164649 snapatac2-2.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/call_peaks.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/embedding.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/export.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/motif.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/network.rs
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/preprocessing.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.164649 snapatac2-2.3.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/utils/anndata.rs
+-rw-r--r--   0 runner    (1001) docker     (123)    12545 2023-06-22 16:01:39.000000 snapatac2-2.3.1/src/utils.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:01:45.164649 snapatac2-2.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-22 16:01:39.000000 snapatac2-2.3.1/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-22 16:01:39.000000 snapatac2-2.3.1/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-22 16:01:39.000000 snapatac2-2.3.1/tests/test_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-06-22 16:01:39.000000 snapatac2-2.3.1/tests/test_tools.py
```

### Comparing `snapatac2-2.3.0/Cargo.toml` & `snapatac2-2.3.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 readme = "README.md"
 repository = "https://github.com/"
 homepage = "https://github.com/"
 keywords = ["single-cell", "biology"]
 
 [dependencies]
 #snapatac2-core = { path = "../snapatac2-core" }
-snapatac2-core = { git = "https://github.com/kaizhang/SnapATAC2.git", rev = "9285fa5be15287870a6af7b0d2bfdec225c3127e" }
+snapatac2-core = { git = "https://github.com/kaizhang/SnapATAC2.git", rev = "8d71ec94ec741abbb5950f889436cb8da5593332" }
 #anndata = { path = "../../anndata-rs/anndata" }
 #anndata-hdf5 = { path = "../../anndata-rs/anndata-hdf5" }
 #pyanndata = { path = "../../anndata-rs/pyanndata" }
 anndata = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "1aba156d6c2f63c16433c7385fd26a8960162283" }
 anndata-hdf5 = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "1aba156d6c2f63c16433c7385fd26a8960162283" }
 pyanndata = { git = "https://github.com/kaizhang/anndata-rs.git", rev = "1aba156d6c2f63c16433c7385fd26a8960162283" }
 anyhow = "1.0"
 bed-utils = { git = "https://github.com/kaizhang/bed-utils.git", rev = "19832eda2909dbe87289e09ba966af0797adb9f8" }
 flate2 = "1.0"
 hora = "0.1"
 itertools = "0.8"
+indicatif = "0.17"
 linreg = "0.2"
 log = "0.4"
 linfa = "0.6"
 linfa-clustering = "0.6"
 noodles = { version = "0.34.0", features = ["bam", "sam"] }
 numpy = "0.18.0"
 nalgebra-sparse = "0.9"
```

### Comparing `snapatac2-2.3.0/LICENSE` & `snapatac2-2.3.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 Kai Zhang
+Copyright (c) 2022-2023 Kai Zhang
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `snapatac2-2.3.0/setup.py` & `snapatac2-2.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,10 +47,10 @@
         "pyarrow",
         "pyfaidx",
         "rustworkx",
         "scipy>=1.4",
         "scikit-learn>=0.22",
         "tqdm>=4.62",
         "typing_extensions",
-        "umap-learn>=0.3.10",
+        "umap-learn>=0.5.0",
     ],
 )
```

### Comparing `snapatac2-2.3.0/snapatac2/__init__.py` & `snapatac2-2.3.1/snapatac2/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/_io.py` & `snapatac2-2.3.1/snapatac2/_io.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/_utils.py` & `snapatac2-2.3.1/snapatac2/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,27 +25,29 @@
         else:
             adatas_list.append(data.filename)
             data.close()
 
     with get_context("spawn").Pool(n_jobs) as p:
         result = p.map(_func, adatas_list)
     
-    for data in adatas:
-        data.open()
+    # Reopen the files if they were closed
+    for data in adatas_list:
+        if not isinstance(data, ad.AnnData):
+            data.open()
     
     return result
 
 def get_igraph_from_adjacency(adj):
     """Get igraph graph from adjacency matrix."""
     import igraph as ig
     vcount = max(adj.shape)
     sources, targets = adj.nonzero()
     edgelist = list(zip(list(sources), list(targets)))
     weights = np.ravel(adj[(sources, targets)])
-    gr = ig.Graph(n=vcount, edges=edgelist, edge_attrs={"weight": weights})
+    gr = ig.Graph(n=vcount, edges=edgelist, directed=False, edge_attrs={"weight": weights})
     return gr
 
 def chunks(mat, chunk_size: int):
     """
     Return chunks of the input matrix
     """
     n = mat.shape[0]
```

### Comparing `snapatac2-2.3.0/snapatac2/datasets.py` & `snapatac2-2.3.1/snapatac2/datasets.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/export/__init__.py` & `snapatac2-2.3.1/snapatac2/export/__init__.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/genome.py` & `snapatac2-2.3.1/snapatac2/genome.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/plotting/__init__.py` & `snapatac2-2.3.1/snapatac2/plotting/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,15 +214,16 @@
         If `show=False` and `out_file=None`, an `plotly.graph_objects.Figure` will be 
         returned, which can then be further customized using the plotly API.
     """
     import polars as pl
     import plotly.graph_objects as go
 
     count = aggregate_X(data, groupby=groupby, normalize="RPKM")
-    count = pl.DataFrame(count.X.T, schema=list(count.obs_names))
+    count = pl.DataFrame(count.X.T)
+    count.columns = list(count.obs_names)
     idx = data.var_ix(np.concatenate(list(peaks.values())).tolist())
     mat = np.log2(1 + count.to_numpy()[idx, :])
 
     trace = go.Heatmap(
         x=count.columns,
         y=np.concatenate(list(peaks.values()))[::-1],
         z=mat,
```

### Comparing `snapatac2-2.3.0/snapatac2/plotting/_base.py` & `snapatac2-2.3.1/snapatac2/plotting/_base.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/plotting/_network.py` & `snapatac2-2.3.1/snapatac2/plotting/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/preprocessing/_basic.py` & `snapatac2-2.3.1/snapatac2/preprocessing/_basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,19 @@
 import logging
 
 import snapatac2
 from snapatac2._snapatac2 import AnnData, AnnDataSet, PyFlagStat
 import snapatac2._snapatac2 as internal
 from snapatac2.genome import Genome
 
+__all__ = ['make_fragment_file', 'import_data', 'add_tile_matrix',
+           'make_peak_matrix', 'filter_cells', 'select_features',
+           'make_gene_matrix', 'add_frip'
+]
+
 def make_fragment_file(
     bam_file: Path,
     output_file: Path,
     is_paired: bool = True,
     barcode_tag: str | None = None,
     barcode_regex: str | None = None,
     umi_tag: str | None = None,
@@ -97,15 +102,15 @@
     sorted_by_barcode: bool = True,
     low_memory: bool = True,
     whitelist: Path | list[str] | None = None,
     shift_left: int = 0,
     shift_right: int = 0,
     chunk_size: int = 2000,
     tempdir: Path | None = None,
-    backend: str | None = None,
+    backend: Literal['hdf5'] = 'hdf5',
 ) -> AnnData:
     """Import dataset and compute QC metrics.
 
     This function will store fragments as base-resolution TN5 insertions in the
     resulting h5ad file (in `.obsm['insertion']`), along with the chromosome
     sizes (in `.uns['reference_sequences']`). Various QC metrics, including TSSe,
     number of unique fragments, duplication rate, fraction of mitochondrial DNA
@@ -122,20 +127,20 @@
     genome
         A Genome object, providing gene annotation and chromosome sizes.
         If not set, `gff_file` and `chrom_size` must be provided.
         `genome` has lower priority than `gff_file` and `chrom_size`.
     gene_anno
         File name of the gene annotation file in GFF or GTF format.
         This is required if `genome` is not set.
-        Setting `gene_anno` will override the `genome` parameter.
+        Setting `gene_anno` will override the annotations from the `genome` parameter.
     chrom_size
         A dictionary containing chromosome sizes, for example,
         `{"chr1": 2393, "chr2": 2344, ...}`.
         This is required if `genome` is not set.
-        Setting `chrom_size` will override the `genome` parameter.
+        Setting `chrom_size` will override the chrom_size from the `genome` parameter.
     min_num_fragments
         Number of unique fragments threshold used to filter cells
     min_tsse
         TSS enrichment threshold used to filter cells
     sorted_by_barcode
         Whether the fragment file has been sorted by cell barcodes.
         If `sorted_by_barcode == True`, this function makes use of small fixed amout of 
@@ -164,14 +169,20 @@
 
     Returns
     -------
     AnnData | ad.AnnData
         An annotated data matrix of shape `n_obs` x `n_vars`. Rows correspond to
         cells and columns to regions. If `file=None`, an in-memory AnnData will be
         returned, otherwise a backed AnnData is returned.
+
+    Examples
+    --------
+    >>> import snapatac2 as snap
+    >>> data = snap.pp.import_data(snap.datasets.pbmc500(), genome=snap.genome.hg38, sorted_by_barcode=False)
+    >>> print(data)
     """
     if genome is not None:
         if chrom_size is None:
             chrom_size = genome.chrom_sizes
         if gene_anno is None:
             gene_anno = genome.fetch_annotations()
 
@@ -186,23 +197,71 @@
     internal.import_fragments(
         adata, fragment_file, gene_anno, chrom_size, min_num_fragments,
         min_tsse, sorted_by_barcode, low_memory, shift_left, shift_right,
         chunk_size, whitelist, tempdir,
     )
     return adata
 
+def add_frip(
+    adata: AnnData | list[AnnData],
+    regions: dict[str, Path | list[str]],
+    *,
+    inplace: bool = True,
+    n_jobs: int = 8,
+) -> dict[str, list[float]] | list[dict[str, list[float]]] | None:
+    """ Add fraction of reads in peaks (FRiP) to the AnnData object.
+
+    Parameters
+    ----------
+    adata
+        The (annotated) data matrix of shape `n_obs` x `n_vars`.
+        Rows correspond to cells and columns to regions.
+        `adata` could also be a list of AnnData objects.
+        In this case, the function will be applied to each AnnData object in parallel.
+    regions
+        A dictionary containing the peak sets to compute FRiP.
+        The keys are peak set names and the values are either a bed file name or a list of
+        strings representing genomic regions. For example,
+        `{"promoter_frac": "promoter.bed", "enhancer_frac": ["chr1:100-200", "chr2:300-400"]}`.
+    inplace
+        Whether to add the results to `adata.obs` or return it as a dictionary.
+    n_jobs
+        Number of jobs to run in parallel when `adata` is a list.
+        If `n_jobs=-1`, all CPUs will be used.
+    """
+
+    for k in regions.keys():
+        if isinstance(regions[k], str) or isinstance(regions[k], Path):
+            regions[k] = internal.read_regions(Path(regions[k]))
+        elif not isinstance(regions[k], list):
+            regions[k] = list(iter(regions[k]))
+
+    if isinstance(adata, list):
+        return snapatac2._utils.anndata_par(
+            adata,
+            lambda x: add_frip(x, regions, inplace),
+            n_jobs=n_jobs,
+        )
+    else:
+        frip = internal.add_frip(adata, regions)
+        if inplace:
+            for k, v in frip.items():
+                adata.obs[k] = v
+        else:
+            return frip
+
 def add_tile_matrix(
     adata: AnnData | list[AnnData],
     *,
     bin_size: int = 500,
     inplace: bool = True,
     chunk_size: int = 500,
     exclude_chroms: list[str] | str | None = ["chrM", "chrY", "M", "Y"],
     file: Path | None = None,
-    backend: str | None = None,
+    backend: Literal['hdf5'] = 'hdf5',
     n_jobs: int = 8,
 ) -> AnnData | None:
     """Generate cell by bin count matrix.
 
     This function is used to generate and add a cell by bin count matrix to the AnnData
     object.
 
@@ -222,14 +281,15 @@
     chunk_size
         Increasing the chunk_size speeds up I/O but uses more memory.
     exclude_chroms
         A list of chromosomes to exclude.
     file
         File name of the output file used to store the result. If provided, result will
         be saved to a backed AnnData, otherwise an in-memory AnnData is used.
+        This has no effect when `inplace=True`.
     backend
         The backend to use for storing the result. If `None`, the default backend will be used.
     n_jobs
         Number of jobs to run in parallel when `adata` is a list.
         If `n_jobs=-1`, all CPUs will be used.
     """
     if isinstance(exclude_chroms, str):
@@ -257,15 +317,15 @@
 
 def make_peak_matrix(
     adata: AnnData | AnnDataSet,
     *,
     use_rep: str | list[str] | None = None,
     inplace: bool = False,
     file: Path | None = None,
-    backend: str | None = None,
+    backend: Literal['hdf5'] = 'hdf5',
     peak_file: Path | None = None,
     chunk_size: int = 500,
     use_x: bool = False,
 ) -> AnnData:
     """Generate cell by peak count matrix.
 
     This function will generate a cell by peak count matrix and store it in a 
@@ -283,15 +343,15 @@
         The peaks can also be provided by a list of strings:
         ["chr1:1-100", "chr2:2-200"].
     inplace
         Whether to add the tile matrix to the AnnData object or return a new AnnData object.
     file
         File name of the output h5ad file used to store the result. If provided,
         result will be saved to a backed AnnData, otherwise an in-memory AnnData
-        is used.
+        is used. This has no effect when `inplace=True`.
     backend
         The backend to use for storing the result. If `None`, the default backend will be used.
     peak_file
         Bed file containing the peaks. If provided, peak information will be read
         from this file.
     chunk_size
         Chunk size
@@ -343,15 +403,15 @@
 
 def make_gene_matrix(
     adata: AnnData | AnnDataSet,
     gene_anno: Genome | Path,
     *,
     inplace: bool = False,
     file: Path | None = None,
-    backend: str | None = None,
+    backend: Literal['hdf5'] | None = 'hdf5',
     chunk_size: int = 500,
     use_x: bool = False,
     id_type: Literal['gene', 'transcript'] = "gene",
 ) -> AnnData:
     """Generate cell by gene activity matrix.
 
     Generate cell by gene activity matrix by counting the TN5 insertions in gene
@@ -361,28 +421,34 @@
     Parameters
     ----------
     adata
         The (annotated) data matrix of shape `n_obs` x `n_vars`.
         Rows correspond to cells and columns to regions.
     gene_anno
         Either a Genome object or the path of a gene annotation file in GFF or GTF format.
+    inplace
+        Whether to add the gene matrix to the AnnData object or return a new AnnData object.
     file
-        File name of the h5ad file used to store the result.
+        File name of the h5ad file used to store the result. This has no effect when `inplace=True`.
+    backend
+        The backend to use for storing the result. If `None`, the default backend will be used.
     chunk_size
         Chunk size
     use_x
         If True, use the matrix stored in `.X` to compute the gene activity.
         Otherwise the `.obsm['insertion']` is used.
     id_type
         "gene" or "transcript".
 
     Returns
     -------
     AnnData
-        A new AnnData object, where rows correspond to cells and columns to genes.
+        An annotated data matrix of shape `n_obs` x `n_vars`. Rows correspond to
+        cells and columns to genes. If `file=None`, an in-memory AnnData will be
+        returned, otherwise a backed AnnData is returned.
     """
     if isinstance(gene_anno, Genome):
         gene_anno = gene_anno.fetch_annotations()
 
     if inplace:
         internal.mk_gene_matrix(adata, gene_anno, chunk_size, use_x, id_type, None)
     else:
@@ -499,14 +565,15 @@
         Lower quantile of the feature count distribution to filter out.
     filter_upper_quantile
         Upper quantile of the feature count distribution to filter out.
     whitelist
         A user provided bed file containing genome-wide whitelist regions.
         None-zero features listed here will be kept regardless of the other
         filtering criteria.
+        If a feature is present in both whitelist and blacklist, it will be kept.
     blacklist 
         A user provided bed file containing genome-wide blacklist regions.
         Features that are overlapped with these regions will be removed.
     inplace
         Perform computation inplace or return result.
     n_jobs
         Number of parallel jobs to use when `adata` is a list.
@@ -534,37 +601,39 @@
         count += np.ravel(batch.sum(axis = 0))
     adata.var['count'] = count
 
     selected_features = _find_most_accessible_features(
         count, filter_lower_quantile, filter_upper_quantile, n_features)
 
     if blacklist is not None:
-        blacklist = np.logical_not(internal.intersect_bed(adata.var_names, str(blacklist)))
+        blacklist = np.array(internal.intersect_bed(adata.var_names, str(blacklist)))
         selected_features = selected_features[np.logical_not(blacklist[selected_features])]
 
     # Iteratively select features
     iter = 1
     while iter < max_iter:
         embedding = snapatac2.tl.spectral(adata, features=selected_features, inplace=False)[1]
         clusters = snapatac2.tl.leiden(snapatac2.pp.knn(embedding, inplace=False))
         rpm = snapatac2.tl.aggregate_X(adata, groupby=clusters).X
         var = np.var(np.log(rpm + 1), axis=0)
         selected_features = np.argsort(var)[::-1][:n_features]
 
+        # Apply blacklist to the result
         if blacklist is not None:
             selected_features = selected_features[np.logical_not(blacklist[selected_features])]
         iter += 1
 
     result = np.zeros(adata.shape[1], dtype=bool)
     result[selected_features] = True
 
+    # Finally, apply whitelist to the result
     if whitelist is not None:
         whitelist = np.array(internal.intersect_bed(adata.var_names, str(whitelist)))
         whitelist &= count != 0
         result |= whitelist
     
     logging.info(f"Selected {result.sum()} features.")
 
     if inplace:
         adata.var["selected"] = result
     else:
-        return result
+        return result
```

### Comparing `snapatac2-2.3.0/snapatac2/preprocessing/_harmony.py` & `snapatac2-2.3.1/snapatac2/preprocessing/_harmony.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/preprocessing/_knn.py` & `snapatac2-2.3.1/snapatac2/preprocessing/_knn.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/preprocessing/_mnn_correct.py` & `snapatac2-2.3.1/snapatac2/preprocessing/_mnn_correct.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/preprocessing/_scrublet.py` & `snapatac2-2.3.1/snapatac2/preprocessing/_scrublet.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/tools/_call_peaks.py` & `snapatac2-2.3.1/snapatac2/tools/_call_peaks.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/tools/_clustering.py` & `snapatac2-2.3.1/snapatac2/tools/_clustering.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
 from typing_extensions import Literal
 
 import scipy.sparse as ss
 import numpy as np
 
 from snapatac2._snapatac2 import AnnData, AnnDataSet
+import snapatac2._snapatac2 as _snapatac2
 from snapatac2._utils import get_igraph_from_adjacency, is_anndata 
 
 def leiden(
     adata: AnnData | AnnDataSet | ss.spmatrix,
     resolution: float = 1,
     objective_function: Literal['CPM', 'modularity', 'RBConfiguration'] = 'modularity',
     min_cluster_size: int = 5,
     n_iterations: int = -1,
     random_state: int = 0,
     key_added: str = 'leiden',
     use_leidenalg: bool = False,
+    weighted: bool = False,
     inplace: bool = True,
 ) -> np.ndarray | None:
     """
     Cluster cells into subgroups [Traag18]_.
 
     Cluster cells using the Leiden algorithm [Traag18]_,
     an improved version of the Louvain algorithm [Blondel08]_.
@@ -47,14 +49,16 @@
         -1 has the algorithm run until it reaches its optimal clustering.
     random_state
         Change the initialization of the optimization.
     key_added
         `adata.obs` key under which to add the cluster labels.
     use_leidenalg
         If `True`, `leidenalg` package is used. Otherwise, `python-igraph` is used.
+    weighted
+        Whether to use the edge weights in the graph
     inplace
         Whether to store the result in the anndata object.
 
     Returns
     -------
     np.ndarray | None
         If `inplace=True`, update `adata.obs[key_added]` to store an array of
@@ -68,14 +72,20 @@
         adjacency = adata.obsp["distances"]
     else:
         inplace = False
         adjacency = adata
     
     gr = get_igraph_from_adjacency(adjacency)
 
+    if weighted:
+        weights = np.array(gr.es["weight"])
+        weights = np.exp(-weights)
+    else:
+        weights = None
+
     if use_leidenalg or objective_function == "RBConfiguration":
         import leidenalg
         from leidenalg.VertexPartition import MutableVertexPartition
 
         if objective_function == "modularity":
             partition_type = leidenalg.ModularityVertexPartition
         elif objective_function == "CPM":
@@ -85,24 +95,24 @@
         else:
             raise ValueError(
                 'objective function is not supported: ' + partition_type
             )
 
         partition = leidenalg.find_partition(
             gr, partition_type, n_iterations=n_iterations,
-            seed=random_state, resolution_parameter=resolution, weights=None
+            seed=random_state, resolution_parameter=resolution, weights=weights
         )
     else:
         from igraph import set_random_number_generator
         import random
         random.seed(random_state)
         set_random_number_generator(random)
         partition = gr.community_leiden(
             objective_function=objective_function,
-            weights=None,
+            weights=weights,
             resolution_parameter=resolution,
             beta=0.01,
             initial_membership=None,
             n_iterations=n_iterations,
         )
 
     groups = partition.membership
@@ -132,15 +142,16 @@
     n_iterations: int = -1,
     random_state: int = 0,
     use_rep: str = "X_spectral",
     key_added: str = 'kmeans',
     inplace: bool = True,
 ) -> np.ndarray | None:
     """
-    Cluster cells into subgroups using the K-means algorithm.
+    Cluster cells into subgroups using the K-means algorithm, a classical algorithm in data mining.
+
 
     Parameters
     ----------
     adata
         The annotated data matrix.
     n_clusters
         Number of clusters to return.
```

### Comparing `snapatac2-2.3.0/snapatac2/tools/_diff.py` & `snapatac2-2.3.1/snapatac2/tools/_diff.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,64 @@
 from __future__ import annotations
 from typing_extensions import Literal
 
 import numpy as np
-from scipy.stats import chi2
+from scipy.stats import chi2, norm
 import logging
 
 from snapatac2._snapatac2 import AnnData, AnnDataSet
 from snapatac2.tools._misc import aggregate_X
 
 def marker_regions(
     data: AnnData | AnnDataSet,
     groupby: str | list[str],
-    pvalue: float = 0.01,
+    fdr: float = 0.01,
 ) -> dict[str, list[str]]:
     """
     A quick-and-dirty way to get marker regions.
+
+    Parameters
+    ----------
+    data
+        AnnData or AnnDataSet object.
+    groupby
+        Grouping variable.
+    fdr
+        FDR threshold.
     """
-    import scipy.stats
+    from statsmodels.stats.multitest import fdrcorrection
 
     count = aggregate_X(data, groupby, normalize="RPKM")
-    z = scipy.stats.zscore(np.log2(1 + count.X), axis = 0)
+    z = modified_zscore(np.log2(1 + count.X), axis = 0)
     peaks = {}
     for i in range(z.shape[0]):
-        pvals = scipy.stats.norm.sf(z[i, :])
-        select = pvals < pvalue
+        pvals = norm.sf(z[i, :])
+        select = fdrcorrection(pvals, alpha=fdr)[0]
         if np.where(select)[0].size >= 1:
             peaks[count.obs_names[i]] = count.var_names[select]
     return peaks
 
+def mad(data, axis=None):
+    """ Compute Median Absolute Deviation """
+    return np.median(np.absolute(data - np.median(data, axis)), axis)
+
+def modified_zscore(matrix, axis=0):
+    """ Compute Modified Z-score for a matrix along specified axis """
+    median = np.median(matrix, axis=axis)
+    median_absolute_deviation = mad(matrix, axis=axis)
+
+    if axis == 0:
+        modified_z_scores = 0.6745 * (matrix - median) / median_absolute_deviation
+    elif axis == 1:
+        modified_z_scores = 0.6745 * (matrix.T - median).T / median_absolute_deviation
+    else:
+        raise ValueError("Invalid axis, it should be 0 or 1")
+
+    return modified_z_scores
+
 def diff_test(
     data: AnnData | AnnDataSet,
     cell_group1: list[int] | list[str],
     cell_group2: list[int] | list[str],
     features : list[str] | list[int] | None = None,
     covariates: list[str] | None = None,
     direction: Literal["positive", "negative", "both"] = "both",
```

### Comparing `snapatac2-2.3.0/snapatac2/tools/_embedding.py` & `snapatac2-2.3.1/snapatac2/tools/_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,67 @@
 
 import scipy as sp
 import numpy as np
 import gc
 import logging
 import math
 
-from snapatac2._utils import is_anndata 
+from snapatac2._utils import get_igraph_from_adjacency, is_anndata 
 from snapatac2._snapatac2 import (AnnData, AnnDataSet, jm_regress, jaccard_similarity,
     cosine_similarity, spectral_embedding, multi_spectral_embedding, spectral_embedding_nystrom)
 
-__all__ = ['umap', 'spectral', 'multi_spectral']
+__all__ = ['umap2', 'umap', 'spectral', 'multi_spectral']
+
+def umap2(
+    adata: AnnData | AnnDataSet | np.ndarray,
+    n_comps: int = 2,
+    key_added: str = 'umap',
+    random_state: int = 0,
+    inplace: bool = True,
+) -> np.ndarray | None:
+    """
+    Parameters
+    ----------
+    adata
+        The annotated data matrix.
+    n_comps
+        The number of dimensions of the embedding.
+    key_added
+        `adata.obs` key under which to add the cluster labels.
+    random_state
+        Random seed.
+    inplace
+        Whether to store the result in the anndata object.
+
+    Returns
+    -------
+    np.ndarray | None
+        if `inplace=True` it stores UMAP embedding in
+        `adata.obsm["X_`key_added`"]`.
+        Otherwise, it returns the result as a numpy array.
+    """
+    from igraph import set_random_number_generator
+    import random
+    random.seed(random_state)
+    set_random_number_generator(random)
+
+    if is_anndata(adata):
+        adjacency = adata.obsp["distances"]
+    else:
+        inplace = False
+        adjacency = adata
+    gr = get_igraph_from_adjacency(adjacency)
+    dist = np.array(gr.es["weight"])
+    umap = gr.layout_umap(dist=dist, dim=n_comps, min_dist=0.01, epochs=500)
+    umap = np.array(umap.coords)
+
+    if inplace:
+        adata.obsm["X_" + key_added] = umap
+    else:
+        return umap
 
 def umap(
     adata: AnnData | AnnDataSet | np.ndarray,
     n_comps: int = 2,
     use_dims: int | list[int] | None = None,
     use_rep: str = "X_spectral",
     key_added: str = 'umap',
@@ -80,29 +128,31 @@
     chunk_size: int = 20000,
     distance_metric: Literal["jaccard", "cosine"] = "cosine",
     weighted_by_sd: bool = True,
     feature_weights: list[float] | None = None,
     inplace: bool = True,
 ) -> tuple[np.ndarray, np.ndarray] | None:
     """
-    Compute Laplacian Eigenmaps of chromatin accessibility profiles.
+    Perform dimension reduction using Laplacian Eigenmaps.
 
-    Convert chromatin accessibility profiles of cells into lower dimensional representations
+    Convert the cell-by-feature count matrix into lower dimensional representations
     using the spectrum of the normalized graph Laplacian defined by pairwise similarity
     between cells.
 
     Note
     ----
-    The space complexity of this function is :math:`O(N^2)`, where $N$ is the minimum between
-    the total of cells and the `sample_size`.
+    When using the cosine similarity as the similarity metric, the matrix-free
+    spectral embedding algorithm is used, which scales linearly with the number of cells. 
+    The memory usage is roughly :math:`2 \times input_size`.
+    For other types of similarity metrics, the time and space complexity is :math:`O(N^2)`,
+    where $N$ is the minimum between the total of cells and the `sample_size`.
     The memory usage in bytes is given by $N^2 * 8 * 2$. For example,
     when $N = 10,000$ it will use roughly 745 MB memory.
     When `sample_size` is set, the Nystrom algorithm will be used to approximate
-    the embedding. For large datasets, try to set the `sample_size` appropriately to
-    reduce the memory usage.
+    the embedding. 
 
     Parameters
     ----------
     adata
         AnnData or AnnDataSet object.
     n_comps
         Number of dimensions to keep.
@@ -162,14 +212,15 @@
             if feature_weights is None:
                 feature_weights = idf(adata, features)
             model = Spectral(n_comps, distance_metric, feature_weights)
             X = adata.X[...] if features is None else adata.X[:, features]
             model.fit(X)
             evals, evecs = model.transform()
     else:
+        logging.info("Perform spectral embedding using the Nystrom algorithm...")
         if distance_metric == "cosine":
             if sample_method == "random":
                 weighted_by_degree = False
             else:
                 weighted_by_degree = True
             v, u = spectral_embedding_nystrom(adata, features, n_comps, sample_size, weighted_by_degree, chunk_size)
             evals, evecs = orthogonalize(v, u)
@@ -182,15 +233,14 @@
             else:
                 S = sp.sparse.csr_matrix(adata.chunk_X(sample_size, replace=False))
             if features is not None: S = S[:, features]
 
             model.fit(S)
 
             from tqdm import tqdm
-            logging.info("Perform Nystrom extension")
             for batch, _, _ in tqdm(adata.chunked_X(chunk_size), total=math.ceil(adata.n_obs/chunk_size)):
                 if distance_metric == "jaccard":
                     batch.data = np.ones(batch.indices.shape, dtype=np.float64)
                 if features is not None: batch = batch[:, features]
                 model.extend(batch)
             evals, evecs = model.transform()
 
@@ -302,16 +352,17 @@
                 np.divide(evecs_new, sigma.reshape((-1, 1)), out=evecs_new)
                 self.evecs = Q @ V @ evecs_new
             else:
                 self.evecs = Q
         return (self.evals, self.evecs)
 
 def orthogonalize(evals, evecs):
-    sigma, V = np.linalg.eig(evecs.T @ evecs)
-    sigma = np.sqrt(sigma)
+    _, sigma, Vt = np.linalg.svd(evecs)
+    V = Vt.T
+
     B = np.multiply(V.T, evals.reshape((1,-1))) @ V
     np.multiply(B, sigma.reshape((-1, 1)), out=B)
     np.multiply(B, sigma.reshape((1, -1)), out=B)
     evals_new, evecs_new = np.linalg.eig(B)
 
     # reorder
     ix = evals_new.argsort()[::-1]
```

### Comparing `snapatac2-2.3.0/snapatac2/tools/_integration.py` & `snapatac2-2.3.1/snapatac2/tools/_integration.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/tools/_misc.py` & `snapatac2-2.3.1/snapatac2/tools/_misc.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/tools/_motif.py` & `snapatac2-2.3.1/snapatac2/tools/_motif.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/tools/_network.py` & `snapatac2-2.3.1/snapatac2/tools/_network.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2/tools/_smooth.py` & `snapatac2-2.3.1/snapatac2/tools/_smooth.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/snapatac2.egg-info/SOURCES.txt` & `snapatac2-2.3.1/snapatac2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/src/call_peaks.rs` & `snapatac2-2.3.1/src/call_peaks.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/src/embedding.rs` & `snapatac2-2.3.1/src/embedding.rs`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 use anndata_hdf5::H5;
 use std::ops::Deref;
 use ndarray::{Array1, Array2, Axis};
 use numpy::{PyArray1, PyArray2};
 use pyanndata::data::PyArrayData;
 use pyo3::prelude::*;
 use rand::SeedableRng;
+use indicatif::{ProgressIterator, ProgressStyle};
 use anndata::{ArrayData, AnnDataOp, ArrayOp, ArrayElemOp, data::{SelectInfoElem, BoundedSelectInfoElem, from_csr_rows}, Backend};
-use nalgebra::{DVector, DMatrix};
+use nalgebra::DVector;
 use nalgebra_sparse::CsrMatrix;
 use rayon::prelude::{ParallelBridge, ParallelIterator};
 use anyhow::Result;
 use itertools::Itertools;
 use log::info;
 
 #[pyfunction]
@@ -77,27 +78,28 @@
             };
             let selected_samples = SelectInfoElem::from(idx);
             let mut seed_mat: CsrMatrix<f64> = $data.x().slice(&[selected_samples, selected_features.clone()])?.unwrap();
 
             // feature weighting and L2 norm normalization.
             normalize(&mut seed_mat, &weights);
 
+            info!("Compute embeddings for {} landmarks...", sample_size);
             let (v, mut u, d) = spectral_mf(seed_mat.clone(), n_components)?;
-            anyhow::Ok(nystrom(seed_mat, &v, &mut u, &d,
+            info!("Apply Nystrom to out-of-sample data...");
+            nystrom(py, seed_mat, &v, &mut u, &d,
                 $data.x().iter(chunk_size).map(|x: (CsrMatrix<f64>, _, _)| {
                     let mut mat = x.0.select_axis(1, &selected_features);
                     normalize(&mut mat, &weights);
                     mat
                 })
-            ))
+            )
         }}
     }
 
     let (evals, evecs) = crate::with_anndata!(&anndata, run)?;
-
     Ok((PyArray1::from_owned_array(py, evals), PyArray2::from_owned_array(py, evecs)))
 }
 
 
 /// Matrix-free spectral embedding.
 /// The input is assumed to be a csr matrix with rows normalized to unit L2 norm.
 fn spectral_mf(
@@ -147,56 +149,71 @@
         anyhow::Ok((evals.to_owned_array(), evecs.to_owned_array()))
     })?;
     degree_inv.iter_mut().for_each(|x| *x = x.recip());
     Ok((v, u, degree_inv.into_iter().copied().collect()))
 }
 
 /// The input is assumed to be a csr matrix with rows normalized to unit L2 norm.
-fn nystrom<I>(
+fn nystrom<'py, I>(
+    py: Python<'py>,
     seed_matrix: CsrMatrix<f64>,
     evals: &Array1<f64>,
     evecs: &mut Array2<f64>,
     degrees: &Array1<f64>,
     inputs: I,
-) -> (Array1<f64>, Array2<f64>)
+) -> Result<(Array1<f64>, Array2<f64>)>
 where
     I: IntoIterator<Item = CsrMatrix<f64>>,
+    I::IntoIter: ExactSizeIterator,
 {
     // normalize the eigenvectors by degrees.
     evecs.axis_iter_mut(Axis(0)).zip(degrees.iter()).for_each(|(mut row, d)|
         row *= d.sqrt().recip()
     );
     // normalize the eigenvectors by eigenvalues.
     evecs.axis_iter_mut(Axis(1)).zip(evals.iter()).for_each(|(mut col, v)|
         col *= v.recip()
     );
-    let evecs = DMatrix::from_row_iterator(evecs.shape()[0], evecs.shape()[1], evecs.iter().copied());
-
-    let seed_matrix_t = seed_matrix.transpose_as_csc();
-
-    let vec = inputs.into_iter().flat_map(|mat| {
-        let mut q = mat * (&seed_matrix_t * &evecs);
-        let t = q.column_iter().map(|col| col.sum())
-            .zip(evals.iter()).map(|(x, v)| x * v).collect::<Vec<_>>();
-        let mut d = &q * &DVector::from(t);
-        let mut d_min = f64::INFINITY;
-        d.iter().filter(|x| **x > 0.0).for_each(|x| if *x < d_min { d_min = *x });
-        d.iter_mut().for_each(|x| if *x <= 0.0 { *x = d_min });
-
-        q.row_iter_mut().zip(d.iter()).for_each(|(mut row, dd)|
-            row.iter_mut().for_each(|x| *x *= dd.sqrt().recip())
+    let evecs_py = PyArray2::from_array(py, evecs);
+    let evals_py = PyArray1::from_array(py, evals);
+    let seed_matrix_py = PyArrayData::from(ArrayData::from(seed_matrix)).into_py(py);
+
+    let nystrom_py: Py<PyAny> = PyModule::from_code(
+        py,
+        "def nystrom(seed, sample, evecs, evals):
+            import numpy as np
+            q = sample @ (seed.T @ evecs)
+            t = q.sum(axis=0) * evals
+            d = q @ t.reshape((-1, 1))
+            d[d<=0] = np.min(d[d>0])
+            np.divide(q, np.sqrt(d), out=q)
+            return q",
+        "",
+        "",
+    )?.getattr("nystrom")?.into();
+
+    let style = ProgressStyle::with_template(
+        "[{elapsed}] {bar:40.cyan/blue} {pos:>7}/{len:7} (eta: {eta})"
+    ).unwrap();
+    let output: Vec<f64> = inputs.into_iter().map(|sample| {
+        let args = (
+            &seed_matrix_py,
+            PyArrayData::from(ArrayData::from(sample)),
+            evecs_py,
+            evals_py,
         );
-        q.transpose().into_iter().copied().collect::<Vec<_>>()
-    }).collect::<Vec<_>>();
+        nystrom_py.call1(py, args).unwrap().extract::<&PyArray2<_>>(py).unwrap().to_vec().unwrap()
+    }).progress_with_style(style).flatten().collect();
 
     let ncol = evecs.ncols();
-    let nrows = vec.len() / ncol;
-    (evals.clone(), Array2::from_shape_vec((nrows, ncol), vec).unwrap())
+    let nrows = output.len() / ncol;
+    Ok((evals.clone(), Array2::from_shape_vec((nrows, ncol), output).unwrap()))
 }
 
+
 fn idf(input: &CsrMatrix<f64>) -> Vec<f64> {
     let mut idf = vec![0.0; input.ncols()];
     input.col_indices().iter().for_each(|i| idf[*i] += 1.0);
     let n = input.nrows() as f64;
     if idf.iter().all_equal() {
         vec![1.0; idf.len()]
     } else {
@@ -314,16 +331,16 @@
     n_components: usize,
 ) -> Result<(&'py PyArray1<f64>, &'py PyArray2<f64>)>
 {
     info!("Compute normalized views...");
     let mats = anndata.into_iter().zip(selected_features.into_iter()).map(|(a, s)| {
         macro_rules! get_mat {
             ($data:expr) => {{
-                let slice = pyanndata::data::to_select_elem(s, $data.n_vars()).unwrap();
-                let mut mat: CsrMatrix<f64> = $data.x().slice_axis(1, slice).unwrap().unwrap();
+                let slice = pyanndata::data::to_select_elem(s, $data.n_vars()).expect("Invalid feature selection");
+                let mut mat: CsrMatrix<f64> = $data.x().slice_axis(1, slice).unwrap().expect("X is None");
                 let feature_weights = idf(&mat);
 
                 // feature weighting and L2 norm normalization.
                 normalize(&mut mat, &feature_weights);
                 let norm = if mat.nrows() <= 2000 {
                     frobenius_norm(&mat)
                 } else {
```

### Comparing `snapatac2-2.3.0/src/export.rs` & `snapatac2-2.3.1/src/export.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/src/lib.rs` & `snapatac2-2.3.1/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -36,30 +36,31 @@
     m.add_function(wrap_pyfunction!(motif::read_motifs, m)?)?;
  
     // Preprocessing related functions
     m.add_class::<preprocessing::PyFlagStat>().unwrap();
     m.add_function(wrap_pyfunction!(preprocessing::make_fragment_file, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::import_fragments, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::mk_tile_matrix, m)?)?;
-    m.add_function(wrap_pyfunction!(preprocessing::mk_tile_matrix_par, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::mk_gene_matrix, m)?)?;
     m.add_function(wrap_pyfunction!(preprocessing::mk_peak_matrix, m)?)?;
+    m.add_function(wrap_pyfunction!(preprocessing::add_frip, m)?)?;
 
     m.add_function(wrap_pyfunction!(export::export_bed, m)?)?;
     m.add_function(wrap_pyfunction!(export::export_bigwig, m)?)?;
     m.add_function(wrap_pyfunction!(call_peaks::call_peaks, m)?)?;
 
     m.add_function(wrap_pyfunction!(network::link_region_to_gene, m)?)?;
 
     m.add_function(wrap_pyfunction!(utils::jaccard_similarity, m)?)?;
     m.add_function(wrap_pyfunction!(utils::cosine_similarity, m)?)?;
     m.add_function(wrap_pyfunction!(utils::pearson, m)?)?;
     m.add_function(wrap_pyfunction!(utils::spearman, m)?)?;
     m.add_function(wrap_pyfunction!(utils::simple_lin_reg, m)?)?;
     m.add_function(wrap_pyfunction!(utils::jm_regress, m)?)?;
+    m.add_function(wrap_pyfunction!(utils::read_regions, m)?)?;
     m.add_function(wrap_pyfunction!(utils::intersect_bed, m)?)?;
     m.add_function(wrap_pyfunction!(utils::kmeans, m)?)?;
     m.add_function(wrap_pyfunction!(utils::approximate_nearest_neighbors, m)?)?;
     m.add_function(wrap_pyfunction!(embedding::spectral_embedding, m)?)?;
     m.add_function(wrap_pyfunction!(embedding::multi_spectral_embedding, m)?)?;
     m.add_function(wrap_pyfunction!(embedding::spectral_embedding_nystrom, m)?)?;
```

### Comparing `snapatac2-2.3.0/src/motif.rs` & `snapatac2-2.3.1/src/motif.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/src/network.rs` & `snapatac2-2.3.1/src/network.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/src/preprocessing.rs` & `snapatac2-2.3.1/src/preprocessing.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 use crate::utils::*;
 
 use anndata::Backend;
 use anndata_hdf5::H5;
-use rayon::prelude::{IntoParallelIterator, ParallelIterator};
 use std::path::PathBuf;
 use std::{str::FromStr, collections::BTreeMap, ops::Deref, collections::HashSet};
 use pyo3::prelude::*;
 use bed_utils::{bed, bed::GenomicRange};
 use pyanndata::PyAnnData;
 use anyhow::Result;
 
 use snapatac2_core::{
-    preprocessing::{Fragment, FlagStat},
+    preprocessing::{Fragment, FlagStat, SnapData},
     preprocessing,
 };
 
 #[pyclass]
 pub(crate) struct PyFlagStat(FlagStat);
 
 #[pymethods]
@@ -169,42 +168,14 @@
         };
     }
 
     crate::with_anndata!(&anndata, run);
     Ok(())
 }
 
-/// Create tile matrix in parallel. Due to the limitation of Python GIL,
-/// this function is only applicable to pure Rust AnnData objects.
-#[pyfunction]
-pub(crate) fn mk_tile_matrix_par(
-    adatas: Vec<RustAnnDataLike>, bin_size: usize, chunk_size: usize, 
-    n_jobs: usize, exclude_chroms: Option<Vec<&str>>,
-) -> Result<()>
-{
-    macro_rules! run {
-        ($data:expr) => {
-            preprocessing::create_tile_matrix(
-                $data,
-                bin_size,
-                chunk_size,
-                exclude_chroms.as_ref().map(|x| x.as_slice()),
-                None::<&PyAnnData>
-            ).unwrap()
-        };
-    }
-
-    rayon::ThreadPoolBuilder::new().num_threads(n_jobs).build().unwrap().install(|| {
-        adatas.into_par_iter().for_each(|adata| {
-            crate::with_rs_anndata!(&adata, run);
-        });
-    });
-    Ok(())
-}
-
 #[pyfunction]
 pub(crate) fn mk_peak_matrix(
     anndata: AnnDataLike,
     peaks: &PyAny,
     chunk_size: usize,
     use_x: bool,
     out: Option<AnnDataLike>,
@@ -254,8 +225,32 @@
             } else {
                 preprocessing::create_gene_matrix($data, transcripts, id_type, chunk_size, None::<&PyAnnData>, use_x)?;
             }
         }
     }
     crate::with_anndata!(&anndata, run);
     Ok(())
-}
+}
+
+#[pyfunction]
+pub(crate) fn add_frip(
+    anndata: AnnDataLike,
+    regions: BTreeMap<String, Vec<&str>>,
+) -> Result<BTreeMap<String, Vec<f64>>>
+{
+    let trees: Vec<_> = regions.values().map(|x|
+        x.into_iter().map(|y| (GenomicRange::from_str(y).unwrap(), ())).collect()
+    ).collect();
+
+    macro_rules! run {
+        ($data:expr) => {
+            $data.frip(&trees)
+        }
+    }
+
+    let frip = crate::with_anndata!(&anndata, run)?;
+    Ok(
+        regions.keys().zip(frip.columns())
+            .map(|(k, v)| (k.clone(), v.to_vec()))
+            .collect()
+    )
+}
```

### Comparing `snapatac2-2.3.0/src/utils/anndata.rs` & `snapatac2-2.3.1/src/utils/anndata.rs`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/src/utils.rs` & `snapatac2-2.3.1/src/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 use numpy::{Element, PyReadonlyArrayDyn, PyReadonlyArray, Ix1, Ix2, PyArray, IntoPyArray};
 use snapatac2_core::preprocessing::{Transcript, read_transcripts_from_gff, read_transcripts_from_gtf};
 use snapatac2_core::utils::similarity;
 
 use bed_utils::{bed, bed::GenomicRange, bed::BED};
 use std::io::BufReader;
 use std::{str::FromStr, fs::File};
-use std::path::Path;
+use std::path::{Path, PathBuf};
 use flate2::read::MultiGzDecoder;
 use linreg::lin_reg_imprecise;
 use linfa::{DatasetBase, traits::{Fit, Predict}};
 use linfa_clustering::KMeans;
 use rand_core::SeedableRng;
 use rand_isaac::Isaac64Rng;
 use hora::core::ann_index::ANNIndex;
@@ -222,14 +222,22 @@
     let count = &count_.as_array();
     let iter = (0..n_row).flat_map(|i| (i+1..n_row)
         .map(move |j| (1.0 / (1.0 / count[[i, 0]] + 1.0 / count[[j, 0]] - 1.0), jm[[i, j]]))
     );
     Ok(lin_reg_imprecise(iter).unwrap())
 }
 
+/// Read genomic regions from a bed file.
+/// Returns a list of strings
+#[pyfunction]
+pub(crate) fn read_regions(file: PathBuf) -> Vec<String> {
+    let mut reader = bed::io::Reader::new(open_file(file), None);
+    reader.records::<GenomicRange>().map(|x| x.unwrap().pretty_show()).collect()
+}
+
 #[pyfunction]
 pub(crate) fn intersect_bed<'py>(py: Python<'py>, regions: &'py PyAny, bed_file: &str) -> PyResult<Vec<bool>> {
     let bed_tree: bed::tree::BedTree<()> = bed::io::Reader::new(open_file(bed_file), None)
         .into_records().map(|x: Result<BED<3>, _>| (x.unwrap(), ())).collect();
     let res = PyIterator::from_object(py, regions)?
         .map(|x| bed_tree.is_overlapped(&GenomicRange::from_str(x.unwrap().extract().unwrap()).unwrap()))
         .collect();
```

### Comparing `snapatac2-2.3.0/tests/test_func.py` & `snapatac2-2.3.1/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/tests/test_pipeline.py` & `snapatac2-2.3.1/tests/test_pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import numpy as np
 
 def h5ad(dir=Path("./")):
     import uuid
     dir.mkdir(exist_ok=True)
     return str(dir / Path(str(uuid.uuid4()) + ".h5ad"))
 
+'''
 def test_exclude():
     fragment_file = snap.datasets.pbmc500(True)
 
     chr_sizes = snap.genome.hg38.chrom_sizes
     chr_sizes.pop('chr1', None)
     chr_sizes.pop('chr10', None)
     data1 = snap.pp.import_data(
@@ -64,8 +65,9 @@
     snap.pp.select_features(data)
 
     snap.tl.spectral(data, sample_size=100)
     snap.tl.spectral(data)
     snap.pp.knn(data)
     snap.tl.leiden(data)
 
-    snap.pp.make_gene_matrix(data, gene_anno=snap.genome.hg38)
+    snap.pp.make_gene_matrix(data, gene_anno=snap.genome.hg38)
+'''
```

### Comparing `snapatac2-2.3.0/tests/test_similarity.py` & `snapatac2-2.3.1/tests/test_similarity.py`

 * *Files identical despite different names*

### Comparing `snapatac2-2.3.0/tests/test_tools.py` & `snapatac2-2.3.1/tests/test_tools.py`

 * *Files identical despite different names*

