# Comparing `tmp/recon_lw-2.0.0.dev5346690345.tar.gz` & `tmp/recon_lw-2.0.0.dev5347019501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5346690345.tar", last modified: Thu Jun 22 14:20:34 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5347019501.tar", last modified: Thu Jun 22 14:51:29 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5346690345.tar` & `recon_lw-2.0.0.dev5347019501.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 14:20:07.000000 recon_lw-2.0.0.dev5346690345/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    33393 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 14:51:04.000000 recon_lw-2.0.0.dev5347019501/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33393 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:51:29.000000 recon_lw-2.0.0.dev5347019501/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-22 14:50:39.000000 recon_lw-2.0.0.dev5347019501/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5347019501/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5347019501/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/setup.py` & `recon_lw-2.0.0.dev5347019501/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5346690345/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5347019501/test/test_recon_ob.py`

 * *Files identical despite different names*

