# Comparing `tmp/pythclient-0.1.6.tar.gz` & `tmp/pythclient-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythclient-0.1.6.tar", last modified: Mon Jun 19 11:36:51 2023, max compression
+gzip compressed data, was "pythclient-0.1.7.tar", last modified: Thu Jun 22 09:41:13 2023, max compression
```

## Comparing `pythclient-0.1.6.tar` & `pythclient-0.1.7.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.621892 pythclient-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-19 11:36:33.000000 pythclient-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-19 11:36:51.617892 pythclient-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-19 11:36:33.000000 pythclient-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-19 11:36:33.000000 pythclient-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.613892 pythclient-0.1.6/pythclient/
--rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/calendar.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/config.py
--rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/pythaccounts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/pythclient.py
--rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/solana.py
--rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-19 11:36:33.000000 pythclient-0.1.6/pythclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.613892 pythclient-0.1.6/pythclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      699 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-19 11:36:51.000000 pythclient-0.1.6/pythclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 11:36:51.621892 pythclient-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-19 11:36:33.000000 pythclient-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 11:36:51.617892 pythclient-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_mapping_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_account_header.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_component.py
--rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_price_info.py
--rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_product_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_pyth_account.py
--rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_pyth_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_solana_account.py
--rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-19 11:36:33.000000 pythclient-0.1.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)    11354 2023-06-22 09:40:59.000000 pythclient-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-22 09:41:13.429975 pythclient-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3347 2023-06-22 09:40:59.000000 pythclient-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-22 09:40:59.000000 pythclient-0.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/pythclient/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6795 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)      266 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)      574 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24180 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/pythaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18523 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/pythclient.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6338 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15635 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/solana.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1249 2023-06-22 09:40:59.000000 pythclient-0.1.7/pythclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/pythclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3950 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      722 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-22 09:41:13.000000 pythclient-0.1.7/pythclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 09:41:13.429975 pythclient-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1171 2023-06-22 09:40:59.000000 pythclient-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:41:13.429975 pythclient-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    11068 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_calendar.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2768 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_mapping_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8640 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2170 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_account_header.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3592 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_price_info.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3992 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_product_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3706 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_pyth_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17146 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_pyth_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3047 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_solana_account.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3478 2023-06-22 09:40:59.000000 pythclient-0.1.7/tests/test_utils.py
```

### Comparing `pythclient-0.1.6/LICENSE` & `pythclient-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/PKG-INFO` & `pythclient-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 Pyth Client in Python
 =====================
```

### Comparing `pythclient-0.1.6/README.md` & `pythclient-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/pythclient/calendar.py` & `pythclient-0.1.7/pythclient/calendar.py`

 * *Files 19% similar despite different names*

```diff
@@ -43,27 +43,27 @@
     day, date, time = dt.weekday(), dt.date(), dt.time()
 
     if asset_type == "equity":
         if date in EQUITY_HOLIDAYS or date in EQUITY_EARLY_HOLIDAYS:
             if (
                 date in EQUITY_EARLY_HOLIDAYS
                 and time >= EQUITY_OPEN
-                and time <= EQUITY_EARLY_CLOSE
+                and time < EQUITY_EARLY_CLOSE
             ):
                 return True
             return False
-        if day < 5 and time >= EQUITY_OPEN and time <= EQUITY_CLOSE:
+        if day < 5 and time >= EQUITY_OPEN and time < EQUITY_CLOSE:
             return True
         return False
 
     if asset_type in ["fx", "metal"]:
         if date in FX_METAL_HOLIDAYS:
             return False
         # On Friday the market is closed after 5pm
-        if day == 4 and time > FX_METAL_OPEN_CLOSE_TIME:
+        if day == 4 and time >= FX_METAL_OPEN_CLOSE_TIME:
             return False
         # On Saturday the market is closed all the time
         if day == 5:
             return False
         # On Sunday the market is closed before 5pm
         if day == 6 and time < FX_METAL_OPEN_CLOSE_TIME:
             return False
@@ -75,17 +75,14 @@
 
 
 def get_next_market_open(asset_type: str, dt: datetime.datetime) -> str:
     # make sure time is in NY timezone
     dt = dt.astimezone(NY_TZ)
     time = dt.time()
 
-    if is_market_open(asset_type, dt):
-        return dt.astimezone(UTC_TZ).strftime("%Y-%m-%dT%H:%M:%S") + "Z"
-
     if asset_type == "equity":
         if time < EQUITY_OPEN:
             next_market_open = dt.replace(
                 hour=EQUITY_OPEN.hour,
                 minute=EQUITY_OPEN.minute,
                 second=0,
                 microsecond=0,
@@ -109,50 +106,87 @@
         else:
             next_market_open = dt.replace(
                 hour=FX_METAL_OPEN_CLOSE_TIME.hour,
                 minute=FX_METAL_OPEN_CLOSE_TIME.minute,
                 second=0,
                 microsecond=0,
             )
-            next_market_open += datetime.timedelta(days=1)
+            while is_market_open(asset_type, next_market_open):
+                next_market_open += datetime.timedelta(days=1)
+
     else:
-        next_market_open = dt.replace(hour=0, minute=0, second=0, microsecond=0)
-        next_market_open += datetime.timedelta(days=1)
+        return None
 
     while not is_market_open(asset_type, next_market_open):
         next_market_open += datetime.timedelta(days=1)
 
     return next_market_open.astimezone(UTC_TZ).strftime("%Y-%m-%dT%H:%M:%S") + "Z"
 
+
 def get_next_market_close(asset_type: str, dt: datetime.datetime) -> str:
     # make sure time is in NY timezone
     dt = dt.astimezone(NY_TZ)
-    if not is_market_open(asset_type, dt):
-        return dt.astimezone(UTC_TZ).strftime("%Y-%m-%dT%H:%M:%S") + "Z"
+    time = dt.time()
 
     if asset_type == "equity":
         if dt.date() in EQUITY_EARLY_HOLIDAYS:
-            
-            next_market_close = dt.replace(
-                hour=EQUITY_EARLY_CLOSE.hour,
-                minute=EQUITY_EARLY_CLOSE.minute,
-                second=0,
-                microsecond=0,
+            if time < EQUITY_EARLY_CLOSE:
+                next_market_close = dt.replace(
+                    hour=EQUITY_EARLY_CLOSE.hour,
+                    minute=EQUITY_EARLY_CLOSE.minute,
+                    second=0,
+                    microsecond=0,
+                )
+            else:
+                next_market_close = dt.replace(
+                    hour=EQUITY_CLOSE.hour,
+                    minute=EQUITY_CLOSE.minute,
+                    second=0,
+                    microsecond=0,
+                )
+                next_market_close += datetime.timedelta(days=1)
+        elif dt.date() in EQUITY_HOLIDAYS:
+            next_market_open = get_next_market_open(
+                asset_type, dt + datetime.timedelta(days=1)
+            )
+            next_market_close = (
+                datetime.datetime.fromisoformat(next_market_open.replace("Z", "+00:00"))
+                .astimezone(NY_TZ)
+                .replace(
+                    hour=EQUITY_CLOSE.hour,
+                    minute=EQUITY_CLOSE.minute,
+                    second=0,
+                    microsecond=0,
+                )
             )
         else:
             next_market_close = dt.replace(
                 hour=EQUITY_CLOSE.hour,
                 minute=EQUITY_CLOSE.minute,
                 second=0,
                 microsecond=0,
             )
+            if time >= EQUITY_CLOSE:
+                next_market_close += datetime.timedelta(days=1)
+
+        # while next_market_close.date() is in EQUITY_HOLIDAYS or weekend, add 1 day
+        while (
+            next_market_close.date() in EQUITY_HOLIDAYS
+            or next_market_close.weekday() >= 5
+        ):
+            next_market_close += datetime.timedelta(days=1)
+
     elif asset_type in ["fx", "metal"]:
         next_market_close = dt.replace(
             hour=FX_METAL_OPEN_CLOSE_TIME.hour,
             minute=FX_METAL_OPEN_CLOSE_TIME.minute,
             second=0,
             microsecond=0,
         )
-    else: # crypto markets never close
+        while not is_market_open(asset_type, next_market_close):
+            next_market_close += datetime.timedelta(days=1)
+        while is_market_open(asset_type, next_market_close):
+            next_market_close += datetime.timedelta(days=1)
+    else:  # crypto markets never close
         return None
 
     return next_market_close.astimezone(UTC_TZ).strftime("%Y-%m-%dT%H:%M:%S") + "Z"
```

### Comparing `pythclient-0.1.6/pythclient/exceptions.py` & `pythclient-0.1.7/pythclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/pythclient/pythaccounts.py` & `pythclient-0.1.7/pythclient/pythaccounts.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/pythclient/pythclient.py` & `pythclient-0.1.7/pythclient/pythclient.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/pythclient/ratelimit.py` & `pythclient-0.1.7/pythclient/ratelimit.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/pythclient/solana.py` & `pythclient-0.1.7/pythclient/solana.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/pythclient/utils.py` & `pythclient-0.1.7/pythclient/utils.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/pythclient.egg-info/PKG-INFO` & `pythclient-0.1.7/pythclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pythclient
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library to retrieve Pyth account structures off the Solana blockchain.
 Home-page: https://github.com/pyth-network/pyth-client-py
 Author: Pyth Developers
 Author-email: contact@pyth.network
 Project-URL: Bug Tracker, https://github.com/pyth-network/pyth-client-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7.0
+Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 Pyth Client in Python
 =====================
```

### Comparing `pythclient-0.1.6/pythclient.egg-info/SOURCES.txt` & `pythclient-0.1.7/pythclient.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 pythclient/solana.py
 pythclient/utils.py
 pythclient.egg-info/PKG-INFO
 pythclient.egg-info/SOURCES.txt
 pythclient.egg-info/dependency_links.txt
 pythclient.egg-info/requires.txt
 pythclient.egg-info/top_level.txt
+tests/test_calendar.py
 tests/test_mapping_account.py
 tests/test_price_account.py
 tests/test_price_account_header.py
 tests/test_price_component.py
 tests/test_price_info.py
 tests/test_product_account.py
 tests/test_pyth_account.py
```

### Comparing `pythclient-0.1.6/setup.py` & `pythclient-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requirements = ['aiodns', 'aiohttp>=3.7.4', 'backoff', 'base58', 'dnspython', 'flake8', 'loguru', 'typing-extensions', 'pytz']
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='pythclient',
-    version='0.1.6',
+    version='0.1.7',
     packages=['pythclient'],
     author='Pyth Developers',
     author_email='contact@pyth.network',
     description='A library to retrieve Pyth account structures off the Solana blockchain.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pyth-network/pyth-client-py',
@@ -24,9 +24,9 @@
         'Operating System :: OS Independent',
     ],
     install_requires=requirements,
     extras_require={
         'testing': requirements + ['mock', 'pytest', 'pytest-cov', 'pytest-socket',
                                    'pytest-mock', 'pytest-asyncio'],
     },
-    python_requires='>=3.7.0',
+    python_requires='>=3.9.0',
 )
```

### Comparing `pythclient-0.1.6/tests/test_mapping_account.py` & `pythclient-0.1.7/tests/test_mapping_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_price_account.py` & `pythclient-0.1.7/tests/test_price_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_price_account_header.py` & `pythclient-0.1.7/tests/test_price_account_header.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_price_component.py` & `pythclient-0.1.7/tests/test_price_component.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_price_info.py` & `pythclient-0.1.7/tests/test_price_info.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_product_account.py` & `pythclient-0.1.7/tests/test_product_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_pyth_account.py` & `pythclient-0.1.7/tests/test_pyth_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_pyth_client.py` & `pythclient-0.1.7/tests/test_pyth_client.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_solana_account.py` & `pythclient-0.1.7/tests/test_solana_account.py`

 * *Files identical despite different names*

### Comparing `pythclient-0.1.6/tests/test_utils.py` & `pythclient-0.1.7/tests/test_utils.py`

 * *Files identical despite different names*

