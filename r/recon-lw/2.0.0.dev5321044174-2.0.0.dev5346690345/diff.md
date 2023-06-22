# Comparing `tmp/recon_lw-2.0.0.dev5321044174.tar.gz` & `tmp/recon_lw-2.0.0.dev5346690345.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5321044174.tar", last modified: Tue Jun 20 09:47:17 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5346690345.tar", last modified: Thu Jun 22 14:20:34 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5321044174.tar` & `recon_lw-2.0.0.dev5346690345.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 09:46:55.000000 recon_lw-2.0.0.dev5321044174/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32984 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 09:47:17.000000 recon_lw-2.0.0.dev5321044174/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-20 09:46:31.000000 recon_lw-2.0.0.dev5321044174/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-22 14:20:07.000000 recon_lw-2.0.0.dev5346690345/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4937 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33393 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6293 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:20:34.000000 recon_lw-2.0.0.dev5346690345/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-22 14:19:43.000000 recon_lw-2.0.0.dev5346690345/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/LastStateMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob.py`

 * *Files 3% similar despite different names*

```diff
@@ -591,29 +591,39 @@
 
 def ob_market_data_trade(trade_price: float, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
 
+    errors = {}
+    if "max_price" not in order_book or order_book["max_price"] is None:
+        errors["trade_book_max_price_eror"] = "max_price not initialized"
+        order_book["max_price"] = trade_price
+
+    if "min_price" not in order_book or order_book["min_price"] is None:
+        errors["trade_book_min_price_eror"] = "min_price not initialized"
+        order_book["min_price"] = trade_price
+
+
     order_book["last_price"] = trade_price
     if trade_price > order_book["max_price"]:
         order_book["max_price"] = trade_price
     if trade_price < order_book["min_price"]:
         order_book["min_price"] = trade_price
     if "total_n_trades" not in order_book:
         order_book["total_n_trades"] = 1
     else:
         order_book["total_n_trades"] += 1
 
     update_time_and_version(str_time_of_event, order_book)
     order_book["aggr_seq"]["top_delta"] = 0
     order_book["aggr_seq"]["limit_delta"] = 0
 
-    return {}, [copy.deepcopy(order_book)]
+    return errors, [copy.deepcopy(order_book)]
 
 
 def ob_indicative_open_price(opening_price: float, str_time_of_event, order_book: dict):
     if "aggr_seq" not in order_book:
         init_aggr_seq(order_book)
     else:
         reset_aggr_seq(order_book)
```

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5346690345/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5346690345/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/setup.py` & `recon_lw-2.0.0.dev5346690345/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5321044174/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5346690345/test/test_recon_ob.py`

 * *Files identical despite different names*

