# Comparing `tmp/geneabacus-0.2.1.tar.gz` & `tmp/geneabacus-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneabacus-0.2.1.tar", last modified: Fri Apr 14 20:12:16 2023, max compression
+gzip compressed data, was "geneabacus-0.3.1.tar", last modified: Thu Jun 22 18:43:22 2023, max compression
```

## Comparing `geneabacus-0.2.1.tar` & `geneabacus-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.443937 geneabacus-0.2.1/
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)       17 2022-10-24 20:18:10.000000 geneabacus-0.2.1/.gitignore
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)    16726 2022-10-24 20:18:10.000000 geneabacus-0.2.1/LICENSE
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1448 2023-04-14 20:12:16.443937 geneabacus-0.2.1/PKG-INFO
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1137 2023-03-09 17:37:32.000000 geneabacus-0.2.1/README.md
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)      131 2022-10-24 20:35:35.000000 geneabacus-0.2.1/pyproject.toml
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)      465 2023-04-14 20:12:16.443937 geneabacus-0.2.1/setup.cfg
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.440604 geneabacus-0.2.1/src/
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.440604 geneabacus-0.2.1/src/geneabacus/
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)        0 2022-10-24 20:18:10.000000 geneabacus-0.2.1/src/geneabacus/__init__.py
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     4907 2023-04-13 22:24:08.000000 geneabacus-0.2.1/src/geneabacus/profileio.py
-drwxr-xr-x   0 charles   (1000) giraldezlab  (1200)        0 2023-04-14 20:12:16.443937 geneabacus-0.2.1/src/geneabacus.egg-info/
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)     1448 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)      297 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)        1 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)       10 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) giraldezlab  (1200)       11 2023-04-14 20:12:16.000000 geneabacus-0.2.1/src/geneabacus.egg-info/top_level.txt
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/
+-rw-r--r--   0 build     (1000) build     (1001)       17 2023-06-22 18:42:53.000000 geneabacus-0.3.1/.gitignore
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/.sourcehut/
+-rw-r--r--   0 build     (1000) build     (1001)     1290 2023-06-22 18:42:53.000000 geneabacus-0.3.1/.sourcehut/arch.yml
+-rw-r--r--   0 build     (1000) build     (1001)    16726 2023-06-22 18:42:53.000000 geneabacus-0.3.1/LICENSE
+-rw-r--r--   0 build     (1000) build     (1001)     1448 2023-06-22 18:43:22.002443 geneabacus-0.3.1/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)     1137 2023-06-22 18:42:53.000000 geneabacus-0.3.1/README.md
+-rw-r--r--   0 build     (1000) build     (1001)      131 2023-06-22 18:42:53.000000 geneabacus-0.3.1/pyproject.toml
+-rw-r--r--   0 build     (1000) build     (1001)      465 2023-06-22 18:43:22.002443 geneabacus-0.3.1/setup.cfg
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:21.999108 geneabacus-0.3.1/src/
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/src/geneabacus/
+-rw-r--r--   0 build     (1000) build     (1001)        0 2023-06-22 18:42:53.000000 geneabacus-0.3.1/src/geneabacus/__init__.py
+-rw-r--r--   0 build     (1000) build     (1001)     5222 2023-06-22 18:42:53.000000 geneabacus-0.3.1/src/geneabacus/profileio.py
+drwxr-xr-x   0 build     (1000) build     (1001)        0 2023-06-22 18:43:22.002443 geneabacus-0.3.1/src/geneabacus.egg-info/
+-rw-r--r--   0 build     (1000) build     (1001)     1448 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/PKG-INFO
+-rw-r--r--   0 build     (1000) build     (1001)      317 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/SOURCES.txt
+-rw-r--r--   0 build     (1000) build     (1001)        1 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/dependency_links.txt
+-rw-r--r--   0 build     (1000) build     (1001)       10 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/requires.txt
+-rw-r--r--   0 build     (1000) build     (1001)       11 2023-06-22 18:43:21.000000 geneabacus-0.3.1/src/geneabacus.egg-info/top_level.txt
```

### Comparing `geneabacus-0.2.1/LICENSE` & `geneabacus-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneabacus-0.2.1/PKG-INFO` & `geneabacus-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneabacus
-Version: 0.2.1
+Version: 0.3.1
 Summary: Python IO functions for GeneAbacus
 Home-page: https://git.sr.ht/~vejnar/GeneAbacus-python
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `geneabacus-0.2.1/README.md` & `geneabacus-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `geneabacus-0.2.1/src/geneabacus/profileio.py` & `geneabacus-0.3.1/src/geneabacus/profileio.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 import json
 import os
 import zlib
 
 import lz4.frame
 import numpy as np
+import zstandard as zstd
 
 def get_flength(features):
     return sum([e-s for s, e in features])
 
 def parse_feat_line(line):
     cells = line.rstrip().split('\t')
     return [cells[0], int(cells[1])]
@@ -30,16 +31,17 @@
     elif filename.endswith('.bin.lz4'):
         f = lz4.frame.open(filename, 'rb')
     else:
         raise ValueError('Invalid format')
     # Open feature file
     if path_features is not None:
         assert os.path.exists(path_features), f'{path_features} not found'
-        if path_features.endswith('.fon1.json'):
-            features = [[ft[fon_name], get_flength(ft[fon_coords])] for ft in json.load(open(path_features, 'rt'))['features']]
+        if path_features.endswith('.fon1.json') or path_features.endswith('.fon1.json.zst'):
+            with zstd.open(path_features, 'rt') if path_features.endswith('.zst') else open(path_features, 'rt') as fp:
+                features = [[ft[fon_name], get_flength(ft[fon_coords])] for ft in json.load(fp)['features']]
         elif path_features.endswith('.tab'):
             with open(path_features, 'rt') as ftab:
                 features = [parse_feat_line(l) for l in ftab]
         else:
             raise ValueError(f'Unknown format: {path_features}')
     elif len(features) == 0:
         raise ValueError('No input features')
@@ -69,16 +71,17 @@
     assert i == len(raw_profiles), f'{i} out of {len(raw_profiles)} was read from input'
     return profiles
 
 def pfwrite(profiles, filename, path_features=None, fon_name='transcript_stable_id', fon_coords='exons', features=[], pformat='binary'):
     # Open feature
     if path_features is not None:
         assert os.path.exists(path_features), f'{path_features} not found'
-        if path_features.endswith('.fon1.json'):
-            features = [[ft[fon_name], get_flength(ft[fon_coords])] for ft in json.load(open(path_features, 'rt'))['features']]
+        if path_features.endswith('.fon1.json') or path_features.endswith('.fon1.json.zst'):
+            with zstd.open(path_features, 'rt') if path_features.endswith('.zst') else open(path_features, 'rt') as fp:
+                features = [[ft[fon_name], get_flength(ft[fon_coords])] for ft in json.load(fp)['features']]
         elif path_features.endswith('.tab'):
             with open(path_features, 'rt') as ftab:
                 features = [parse_feat_line(l) for l in ftab]
         else:
             raise ValueError(f'Unknown format: {path_features}')
     elif len(features) == 0:
         raise ValueError('No input features')
```

### Comparing `geneabacus-0.2.1/src/geneabacus.egg-info/PKG-INFO` & `geneabacus-0.3.1/src/geneabacus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneabacus
-Version: 0.2.1
+Version: 0.3.1
 Summary: Python IO functions for GeneAbacus
 Home-page: https://git.sr.ht/~vejnar/GeneAbacus-python
 Author: Charles E. Vejnar
 License: Mozilla Public License 2.0 (MPL 2.0)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

