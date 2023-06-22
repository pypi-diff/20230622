# Comparing `tmp/mycoinlib-1.1.tar.gz` & `tmp/mycoinlib-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mycoinlib-1.1.tar", last modified: Thu Jun 22 07:10:04 2023, max compression
+gzip compressed data, was "mycoinlib-1.2.tar", last modified: Thu Jun 22 07:22:57 2023, max compression
```

## Comparing `mycoinlib-1.1.tar` & `mycoinlib-1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:10:04.037168 mycoinlib-1.1/
--rw-rw-rw-   0        0        0       54 2023-06-22 07:10:04.030216 mycoinlib-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 07:10:03.769404 mycoinlib-1.1/mycoinlib/
--rw-rw-rw-   0        0        0      130 2023-06-22 06:40:32.000000 mycoinlib-1.1/mycoinlib/__init__.py
--rw-rw-rw-   0        0        0     1909 2023-06-22 06:55:17.000000 mycoinlib-1.1/mycoinlib/btc.py
--rw-rw-rw-   0        0        0     1955 2023-06-22 07:03:16.000000 mycoinlib-1.1/mycoinlib/eth.py
--rw-rw-rw-   0        0        0     2070 2023-06-22 06:54:59.000000 mycoinlib-1.1/mycoinlib/ltc.py
--rw-rw-rw-   0        0        0      637 2023-06-22 06:44:33.000000 mycoinlib-1.1/mycoinlib/mycoin.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:10:04.018295 mycoinlib-1.1/mycoinlib.egg-info/
--rw-rw-rw-   0        0        0       54 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-22 07:10:03.000000 mycoinlib-1.1/mycoinlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 07:10:04.038162 mycoinlib-1.1/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-06-22 07:09:43.000000 mycoinlib-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:22:56.713339 mycoinlib-1.2/
+-rw-rw-rw-   0        0        0       54 2023-06-22 07:22:56.709360 mycoinlib-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 07:22:56.559835 mycoinlib-1.2/mycoinlib/
+-rw-rw-rw-   0        0        0      130 2023-06-22 06:40:32.000000 mycoinlib-1.2/mycoinlib/__init__.py
+-rw-rw-rw-   0        0        0     1944 2023-06-22 07:21:56.000000 mycoinlib-1.2/mycoinlib/btc.py
+-rw-rw-rw-   0        0        0     1990 2023-06-22 07:22:10.000000 mycoinlib-1.2/mycoinlib/eth.py
+-rw-rw-rw-   0        0        0     2105 2023-06-22 07:22:19.000000 mycoinlib-1.2/mycoinlib/ltc.py
+-rw-rw-rw-   0        0        0      637 2023-06-22 06:44:33.000000 mycoinlib-1.2/mycoinlib/mycoin.py
+drwxrwxrwx   0        0        0        0 2023-06-22 07:22:56.698433 mycoinlib-1.2/mycoinlib.egg-info/
+-rw-rw-rw-   0        0        0       54 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-06-22 07:22:56.000000 mycoinlib-1.2/mycoinlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 07:22:55.000000 mycoinlib-1.2/mycoinlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 07:22:56.713339 mycoinlib-1.2/setup.cfg
+-rw-rw-rw-   0        0        0      257 2023-06-22 07:22:41.000000 mycoinlib-1.2/setup.py
```

### Comparing `mycoinlib-1.1/mycoinlib/btc.py` & `mycoinlib-1.2/mycoinlib/btc.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     # Create a new BTC wallet
     def create_wallet():
         key = HDKey(network='bitcoin')
         private_key = key.wif()
         public_key = key.public_hex
         address = key.address()
         info = {
+            'crypto_type': 'BTC',
             'private_key': private_key,
             'public_key': public_key,
             'wallet_address': address
         }
         return info
```

### Comparing `mycoinlib-1.1/mycoinlib/eth.py` & `mycoinlib-1.2/mycoinlib/eth.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class ETH:
     # Create a new ETH wallet
     def create_wallet():
         account = Account.create()
         private_key = account._private_key.hex()
         address = account.address
         info = {
+            'crypto_type': 'ETH',
             'private_key': private_key,
             'public_key': address,
             'wallet_address': address
         }
         return info
```

### Comparing `mycoinlib-1.1/mycoinlib/ltc.py` & `mycoinlib-1.2/mycoinlib/ltc.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     # Create a new LTC wallet
     def create_wallet():
         key = HDKey(network='litecoin')
         private_key = key.wif()
         public_key = key.public_hex
         address = key.address()
         info = {
+            'crypto_type': 'LTC',
             'private_key': private_key,
             'public_key': public_key,
             'wallet_address': address
         }
         return info
```

### Comparing `mycoinlib-1.1/mycoinlib/mycoin.py` & `mycoinlib-1.2/mycoinlib/mycoin.py`

 * *Files identical despite different names*

