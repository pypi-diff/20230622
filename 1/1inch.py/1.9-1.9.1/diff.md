# Comparing `tmp/1inch.py-1.9.tar.gz` & `tmp/1inch.py-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "1inch.py-1.9.tar", last modified: Mon Mar 20 07:04:48 2023, max compression
+gzip compressed data, was "1inch.py-1.9.1.tar", last modified: Thu Jun 22 16:47:01 2023, max compression
```

## Comparing `1inch.py-1.9.tar` & `1inch.py-1.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 richardatkinson   (501) staff       (20)        0 2023-03-20 07:04:48.355728 1inch.py-1.9/
-drwxr-xr-x   0 richardatkinson   (501) staff       (20)        0 2023-03-20 07:04:48.354469 1inch.py-1.9/1inch.py.egg-info/
--rw-r--r--   0 richardatkinson   (501) staff       (20)     6996 2023-03-20 07:04:48.000000 1inch.py-1.9/1inch.py.egg-info/PKG-INFO
--rw-r--r--   0 richardatkinson   (501) staff       (20)      358 2023-03-20 07:04:48.000000 1inch.py-1.9/1inch.py.egg-info/SOURCES.txt
--rw-r--r--   0 richardatkinson   (501) staff       (20)        1 2023-03-20 07:04:48.000000 1inch.py-1.9/1inch.py.egg-info/dependency_links.txt
--rw-r--r--   0 richardatkinson   (501) staff       (20)       49 2023-03-20 07:04:48.000000 1inch.py-1.9/1inch.py.egg-info/requires.txt
--rw-r--r--   0 richardatkinson   (501) staff       (20)       11 2023-03-20 07:04:48.000000 1inch.py-1.9/1inch.py.egg-info/top_level.txt
--rw-r--r--   0 richardatkinson   (501) staff       (20)     1072 2022-07-13 09:37:14.000000 1inch.py-1.9/LICENCE.txt
--rw-r--r--   0 richardatkinson   (501) staff       (20)       31 2022-11-19 07:37:33.000000 1inch.py-1.9/MANIFEST.in
--rw-r--r--   0 richardatkinson   (501) staff       (20)     6996 2023-03-20 07:04:48.355620 1inch.py-1.9/PKG-INFO
--rw-r--r--   0 richardatkinson   (501) staff       (20)     6625 2022-10-11 16:51:11.000000 1inch.py-1.9/README.md
-drwxr-xr-x   0 richardatkinson   (501) staff       (20)        0 2023-03-20 07:04:48.355457 1inch.py-1.9/oneinch_py/
--rw-r--r--   0 richardatkinson   (501) staff       (20)       74 2022-07-31 17:44:29.000000 1inch.py-1.9/oneinch_py/__init__.py
--rw-r--r--   0 richardatkinson   (501) staff       (20)    31284 2023-03-20 06:55:23.000000 1inch.py-1.9/oneinch_py/aggregatorv5.json
--rw-r--r--   0 richardatkinson   (501) staff       (20)     9889 2022-11-18 03:14:29.000000 1inch.py-1.9/oneinch_py/erc20.json
--rw-r--r--   0 richardatkinson   (501) staff       (20)    15464 2023-03-20 07:00:57.000000 1inch.py-1.9/oneinch_py/main.py
--rw-r--r--   0 richardatkinson   (501) staff       (20)      587 2022-11-18 03:14:29.000000 1inch.py-1.9/oneinch_py/multicall.json
--rw-r--r--   0 richardatkinson   (501) staff       (20)     5153 2022-11-18 03:14:29.000000 1inch.py-1.9/oneinch_py/oracle.json
--rw-r--r--   0 richardatkinson   (501) staff       (20)       86 2022-11-17 17:30:42.000000 1inch.py-1.9/pyproject.toml
--rw-r--r--   0 richardatkinson   (501) staff       (20)       38 2023-03-20 07:04:48.355764 1inch.py-1.9/setup.cfg
--rw-r--r--   0 richardatkinson   (501) staff       (20)      857 2023-03-20 07:02:47.000000 1inch.py-1.9/setup.py
+drwxr-xr-x   0 richardatkinson   (501) staff       (20)        0 2023-06-22 16:47:01.621544 1inch.py-1.9.1/
+drwxr-xr-x   0 richardatkinson   (501) staff       (20)        0 2023-06-22 16:47:01.619791 1inch.py-1.9.1/1inch.py.egg-info/
+-rw-r--r--   0 richardatkinson   (501) staff       (20)     7252 2023-06-22 16:47:01.000000 1inch.py-1.9.1/1inch.py.egg-info/PKG-INFO
+-rw-r--r--   0 richardatkinson   (501) staff       (20)      358 2023-06-22 16:47:01.000000 1inch.py-1.9.1/1inch.py.egg-info/SOURCES.txt
+-rw-r--r--   0 richardatkinson   (501) staff       (20)        1 2023-06-22 16:47:01.000000 1inch.py-1.9.1/1inch.py.egg-info/dependency_links.txt
+-rw-r--r--   0 richardatkinson   (501) staff       (20)       49 2023-06-22 16:47:01.000000 1inch.py-1.9.1/1inch.py.egg-info/requires.txt
+-rw-r--r--   0 richardatkinson   (501) staff       (20)       11 2023-06-22 16:47:01.000000 1inch.py-1.9.1/1inch.py.egg-info/top_level.txt
+-rw-r--r--   0 richardatkinson   (501) staff       (20)     1072 2022-07-13 09:37:14.000000 1inch.py-1.9.1/LICENCE.txt
+-rw-r--r--   0 richardatkinson   (501) staff       (20)       31 2022-11-19 07:37:33.000000 1inch.py-1.9.1/MANIFEST.in
+-rw-r--r--   0 richardatkinson   (501) staff       (20)     7252 2023-06-22 16:47:01.621428 1inch.py-1.9.1/PKG-INFO
+-rw-r--r--   0 richardatkinson   (501) staff       (20)     6879 2023-04-21 09:08:27.000000 1inch.py-1.9.1/README.md
+drwxr-xr-x   0 richardatkinson   (501) staff       (20)        0 2023-06-22 16:47:01.621218 1inch.py-1.9.1/oneinch_py/
+-rw-r--r--   0 richardatkinson   (501) staff       (20)       74 2022-07-31 17:44:29.000000 1inch.py-1.9.1/oneinch_py/__init__.py
+-rw-r--r--   0 richardatkinson   (501) staff       (20)    31284 2023-03-21 16:51:38.000000 1inch.py-1.9.1/oneinch_py/aggregatorv5.json
+-rw-r--r--   0 richardatkinson   (501) staff       (20)     9889 2023-03-21 16:51:38.000000 1inch.py-1.9.1/oneinch_py/erc20.json
+-rw-r--r--   0 richardatkinson   (501) staff       (20)    15619 2023-06-22 16:44:01.000000 1inch.py-1.9.1/oneinch_py/main.py
+-rw-r--r--   0 richardatkinson   (501) staff       (20)      587 2022-11-18 03:14:29.000000 1inch.py-1.9.1/oneinch_py/multicall.json
+-rw-r--r--   0 richardatkinson   (501) staff       (20)     5153 2023-03-21 16:51:38.000000 1inch.py-1.9.1/oneinch_py/oracle.json
+-rw-r--r--   0 richardatkinson   (501) staff       (20)       86 2022-11-17 17:30:42.000000 1inch.py-1.9.1/pyproject.toml
+-rw-r--r--   0 richardatkinson   (501) staff       (20)       38 2023-06-22 16:47:01.621587 1inch.py-1.9.1/setup.cfg
+-rw-r--r--   0 richardatkinson   (501) staff       (20)      859 2023-06-22 16:45:03.000000 1inch.py-1.9.1/setup.py
```

### Comparing `1inch.py-1.9/1inch.py.egg-info/PKG-INFO` & `1inch.py-1.9.1/1inch.py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1inch.py
-Version: 1.9
+Version: 1.9.1
 Summary: a Python wrapper for the 1inch API
 Home-page: https://github.com/RichardAtCT/1inch_wrapper
 Author: RichardAt
 Author-email: richardatk01@gmail.com
 License: MIT
 Keywords: 1inch,wrapper,aggregator,DEX
 Platform: UNKNOWN
@@ -27,28 +27,33 @@
 
 ```bash
 pip install 1inch.py
 ```
 
 ## Usage
 
+A quick note on decimals. The wrapper is designed for ease of use, and as such accepts amounts in "Ether" or whole units. 
+If you prefer, you can use decimal=0 and specify amounts in wei. This will also help with any potential floating point errors. 
+
+
 ```python
 from oneinch_py import OneInchSwap, TransactionHelper, OneInchOracle
 
 rpc_url = "yourRPCURL.com"
 binance_rpc = "adifferentRPCurl.com"
 public_key = "yourWalletAddress"
 private_key = "yourPrivateKey" #remember to protect your private key. Using environmental variables is recommended. 
 
 exchange = OneInchSwap(public_key)
 bsc_exchange = OneInchSwap(public_key, chain='binance')
 helper = TransactionHelper(rpc_url, public_key, private_key)
 bsc_helper = TransactionHelper(binance_rpc, public_key, private_key, chain='binance')
 oracle = OneInchOracle(rpc_url, chain='ethereum')
 
+
 # See chains currently supported by the helper method:
 helper.chains
 # {"ethereum": "1", "binance": "56", "polygon": "137", "avalanche": "43114"}
 
 # Straight to business:
 # Get a swap and do the swap
 result = exchange.get_swap("USDT", "ETH", 10, 0.5) # get the swap transaction
```

### Comparing `1inch.py-1.9/LICENCE.txt` & `1inch.py-1.9.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `1inch.py-1.9/PKG-INFO` & `1inch.py-1.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: 1inch.py
-Version: 1.9
+Version: 1.9.1
 Summary: a Python wrapper for the 1inch API
 Home-page: https://github.com/RichardAtCT/1inch_wrapper
 Author: RichardAt
 Author-email: richardatk01@gmail.com
 License: MIT
 Keywords: 1inch,wrapper,aggregator,DEX
 Platform: UNKNOWN
@@ -27,28 +27,33 @@
 
 ```bash
 pip install 1inch.py
 ```
 
 ## Usage
 
+A quick note on decimals. The wrapper is designed for ease of use, and as such accepts amounts in "Ether" or whole units. 
+If you prefer, you can use decimal=0 and specify amounts in wei. This will also help with any potential floating point errors. 
+
+
 ```python
 from oneinch_py import OneInchSwap, TransactionHelper, OneInchOracle
 
 rpc_url = "yourRPCURL.com"
 binance_rpc = "adifferentRPCurl.com"
 public_key = "yourWalletAddress"
 private_key = "yourPrivateKey" #remember to protect your private key. Using environmental variables is recommended. 
 
 exchange = OneInchSwap(public_key)
 bsc_exchange = OneInchSwap(public_key, chain='binance')
 helper = TransactionHelper(rpc_url, public_key, private_key)
 bsc_helper = TransactionHelper(binance_rpc, public_key, private_key, chain='binance')
 oracle = OneInchOracle(rpc_url, chain='ethereum')
 
+
 # See chains currently supported by the helper method:
 helper.chains
 # {"ethereum": "1", "binance": "56", "polygon": "137", "avalanche": "43114"}
 
 # Straight to business:
 # Get a swap and do the swap
 result = exchange.get_swap("USDT", "ETH", 10, 0.5) # get the swap transaction
```

### Comparing `1inch.py-1.9/README.md` & `1inch.py-1.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,33 @@
 
 ```bash
 pip install 1inch.py
 ```
 
 ## Usage
 
+A quick note on decimals. The wrapper is designed for ease of use, and as such accepts amounts in "Ether" or whole units. 
+If you prefer, you can use decimal=0 and specify amounts in wei. This will also help with any potential floating point errors. 
+
+
 ```python
 from oneinch_py import OneInchSwap, TransactionHelper, OneInchOracle
 
 rpc_url = "yourRPCURL.com"
 binance_rpc = "adifferentRPCurl.com"
 public_key = "yourWalletAddress"
 private_key = "yourPrivateKey" #remember to protect your private key. Using environmental variables is recommended. 
 
 exchange = OneInchSwap(public_key)
 bsc_exchange = OneInchSwap(public_key, chain='binance')
 helper = TransactionHelper(rpc_url, public_key, private_key)
 bsc_helper = TransactionHelper(binance_rpc, public_key, private_key, chain='binance')
 oracle = OneInchOracle(rpc_url, chain='ethereum')
 
+
 # See chains currently supported by the helper method:
 helper.chains
 # {"ethereum": "1", "binance": "56", "polygon": "137", "avalanche": "43114"}
 
 # Straight to business:
 # Get a swap and do the swap
 result = exchange.get_swap("USDT", "ETH", 10, 0.5) # get the swap transaction
```

### Comparing `1inch.py-1.9/oneinch_py/aggregatorv5.json` & `1inch.py-1.9.1/oneinch_py/aggregatorv5.json`

 * *Files identical despite different names*

### Comparing `1inch.py-1.9/oneinch_py/erc20.json` & `1inch.py-1.9.1/oneinch_py/erc20.json`

 * *Files identical despite different names*

### Comparing `1inch.py-1.9/oneinch_py/main.py` & `1inch.py-1.9.1/oneinch_py/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 class UnknownToken(Exception):
     pass
 
 
 class OneInchSwap:
-    base_url = 'https://api.1inch.exchange'
+    base_url = 'https://api.1inch.io'
 
     version = {
         "v4.0": "v4.0",
         "v5.0": "v5.0"
     }
 
     chains = {
@@ -54,15 +54,15 @@
         except requests.exceptions.HTTPError:
             print("HTTPError {}".format(url))
             payload = None
         return payload
 
     def _token_to_address(self, token: str):
         if len(token) == 42:
-            return token
+            return self.w3.to_checksum_address(token)
         else:
             try:
                 address = self.tokens[token]['address']
             except:
                 raise UnknownToken("Token not in 1inch Token List")
             return address
 
@@ -126,15 +126,18 @@
                 self.tokens[from_token_symbol]['decimals']
             except KeyError:
                 decimal = 18
             else:
                 decimal = self.tokens[from_token_symbol]['decimals']
         else:
             pass
-        amount_in_wei = Decimal(amount * 10 ** decimal)
+        if decimal == 0:
+            amount_in_wei = int(amount)
+        else:
+            amount_in_wei = int(amount * 10 ** decimal)
         url = f'{self.base_url}/{self.version}/{self.chain_id}/quote'
         url = url + f'?fromTokenAddress={from_address}&toTokenAddress={to_address}&amount={amount_in_wei}'
         if kwargs is not None:
             result = self._get(url, params=kwargs)
         else:
             result = self._get(url)
         from_base = Decimal(result['fromTokenAmount']) / Decimal(10 ** result['fromToken']['decimals'])
@@ -162,15 +165,18 @@
                 self.tokens[from_token_symbol]['decimals']
             except KeyError:
                 decimal = 18
             else:
                 decimal = self.tokens[from_token_symbol]['decimals']
         else:
             pass
-        amount_in_wei = Decimal(amount * 10 ** decimal)
+        if decimal == 0:
+            amount_in_wei = int(amount)
+        else:
+            amount_in_wei = int(amount * 10 ** decimal)
         url = f'{self.base_url}/{self.version}/{self.chain_id}/swap'
         url = url + f'?fromTokenAddress={from_address}&toTokenAddress={to_address}&amount={amount_in_wei}'
         url = url + f'&fromAddress={send_address}&slippage={slippage}'
         if kwargs is not None:
             result = self._get(url, params=kwargs)
         else:
             result = self._get(url)
@@ -196,15 +202,18 @@
                 decimal = self.tokens[from_token_symbol]['decimals']
         else:
             pass
         url = f'{self.base_url}/{self.version}/{self.chain_id}/approve/transaction'
         if amount is None:
             url = url + f"?tokenAddress={from_address}"
         else:
-            amount_in_wei = amount * 10 ** decimal
+            if decimal == 0:
+                amount_in_wei = int(amount)
+            else:
+                amount_in_wei = int(amount * 10 ** decimal)
             url = url + f"?tokenAddress={from_address}&amount={amount_in_wei}"
         result = self._get(url)
         return result
 
 
 class TransactionHelper:
     gas_oracle = "https://gas-price-api.1inch.io/v1.3/"
@@ -213,22 +222,19 @@
         "ethereum": '1',
         "binance": '56',
         "polygon": "137",
         "optimism": "10",
         "arbitrum": "42161",
         "gnosis": "100",
         "avalanche": "43114",
-        "fantom": "250"
+        "fantom": "250",
+        "klaytn": "8217",
+        "aurora": "1313161554"
     }
 
-    # MODE = {
-    #     "slow": [10, 20, 30, 40, 50],  # <1min
-    #     "normal": [10, 30, 50, 70, 90],  # <30sec
-    #     "fast": [50, 60, 70, 80, 90],  # <10sec
-    # }
 
     abi = json.loads(pkg_resources.read_text(__package__, 'erc20.json'))['result']
     abi_aggregator = json.loads(pkg_resources.read_text(__package__, 'aggregatorv5.json'))['result']
 
     @staticmethod
     def _get(url, params=None, headers=None):
         """ Implements a get request """
@@ -267,18 +273,16 @@
         tx['to'] = self.w3.to_checksum_address(tx['to'])
         if 'gas' not in tx:
             tx['gas'] = self.w3.eth.estimate_gas(tx)
         tx['nonce'] = nonce
         tx['chainId'] = int(self.chain_id)
         tx['value'] = int(tx['value'])
         tx['gas'] = int(tx['gas'] * 1.25)
-        if self.chain == 'ethereum' or self.chain == 'polygon' or self.chain == 'avalanche' or self.chain == 'gnosis':
+        if self.chain == 'ethereum' or self.chain == 'polygon' or self.chain == 'avalanche' or self.chain == 'gnosis' or self.chain == 'klaytn':
             gas = self._get(self.gas_oracle+self.chain_id)
-            # print(gas)
-            # gas = requests.get(self.gas_oracle, params=self.chain_id)
             tx['maxPriorityFeePerGas'] = int(gas[speed]['maxPriorityFeePerGas'])
             tx['maxFeePerGas'] = int(gas[speed]['maxFeePerGas'])
             tx.pop('gasPrice')
         else:
             tx['gasPrice'] = int(tx['gasPrice'])
         return tx
 
@@ -302,14 +306,16 @@
             return receipt, tx_hash.hex()
 
     def get_ERC20_balance(self, contract_address, decimal=None):
         contract = self.w3.eth.contract(address=self.w3.to_checksum_address(contract_address), abi=self.abi)
         balance_in_wei = contract.functions.balanceOf(self.public_key).call()
         if decimal is None:
             return self.w3.from_wei(balance_in_wei, 'ether')
+        elif decimal == 0:
+            return balance_in_wei
         else:
             return balance_in_wei / 10 ** decimal
 
     def decode_abi(self, transaction):
         contract = self.w3.eth.contract(address=self.w3.to_checksum_address('0x1111111254EEB25477B68fb85Ed929f73A960582'), abi=self.abi_aggregator)
         data = transaction['tx']['data']
         decoded_data = contract.decode_function_input(data)
```

### Comparing `1inch.py-1.9/oneinch_py/multicall.json` & `1inch.py-1.9.1/oneinch_py/multicall.json`

 * *Files identical despite different names*

### Comparing `1inch.py-1.9/oneinch_py/oracle.json` & `1inch.py-1.9.1/oneinch_py/oracle.json`

 * *Files identical despite different names*

### Comparing `1inch.py-1.9/setup.py` & `1inch.py-1.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='1inch.py',
-    version='1.9',
+    version='1.9.1',
     url='https://github.com/RichardAtCT/1inch_wrapper',
     long_description_content_type="text/markdown",
     long_description=long_description,
     keywords="1inch, wrapper, aggregator, DEX",
     packages=find_packages(include=['oneinch_py', 'oneinch_py.*']),
     include_package_data=True,
     install_requires=[
```

