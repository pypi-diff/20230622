# Comparing `tmp/substrate-interface-1.7.2.tar.gz` & `tmp/substrate-interface-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-interface-1.7.2.tar", last modified: Wed Jun  7 13:46:41 2023, max compression
+gzip compressed data, was "substrate-interface-1.7.3.tar", last modified: Thu Jun 22 11:56:41 2023, max compression
```

## Comparing `substrate-interface-1.7.2.tar` & `substrate-interface-1.7.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.008362 substrate-interface-1.7.2/substrate_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-07 13:46:40.000000 substrate-interface-1.7.2/substrate_interface.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.008362 substrate-interface-1.7.2/substrateinterface/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   126315 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    31530 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/key.py
--rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/substrateinterface/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/ecdsa_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/encrypted_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/substrateinterface/utils/ss58.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:46:41.012362 substrate-interface-1.7.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_contracts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_create_extrinsics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_extension_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_rpc_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_runtime_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_ss58.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-06-07 13:40:34.000000 substrate-interface-1.7.2/test/test_type_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:56:41.281583 substrate-interface-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-22 11:56:41.281583 substrate-interface-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 11:56:41.281583 substrate-interface-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:56:41.269582 substrate-interface-1.7.3/substrate_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-06-22 11:56:40.000000 substrate-interface-1.7.3/substrate_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-22 11:56:41.000000 substrate-interface-1.7.3/substrate_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:56:40.000000 substrate-interface-1.7.3/substrate_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-22 11:56:40.000000 substrate-interface-1.7.3/substrate_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-22 11:56:40.000000 substrate-interface-1.7.3/substrate_interface.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:56:41.273583 substrate-interface-1.7.3/substrateinterface/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   126427 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31630 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20655 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:56:41.277583 substrate-interface-1.7.3/substrateinterface/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/utils/ecdsa_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/utils/encrypted_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/utils/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/substrateinterface/utils/ss58.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:56:41.281583 substrate-interface-1.7.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    16994 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17433 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16587 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_create_extrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_extension_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19797 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20044 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_rpc_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_runtime_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9374 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_ss58.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-06-22 11:50:30.000000 substrate-interface-1.7.3/test/test_type_registry.py
```

### Comparing `substrate-interface-1.7.2/LICENSE` & `substrate-interface-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/PKG-INFO` & `substrate-interface-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.2
+Version: 1.7.3
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.2/README.md` & `substrate-interface-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/setup.py` & `substrate-interface-1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
         'requests>=2.21.0,<3',
         'xxhash>=1.3.0,<4',
         'ecdsa>=0.17.0,<1',
         'eth-keys>=0.2.1,<1',
         'eth_utils>=1.3.0,<3',
         'pycryptodome>=3.11.0,<4',
         'PyNaCl>=1.0.1,<2',
-        'scalecodec>=1.2.4,<1.3',
+        'scalecodec>=1.2.6,<1.3',
         'py-sr25519-bindings>=0.2.0,<1',
         'py-ed25519-zebra-bindings>=1.0,<2',
         'py-bip39-bindings>=0.1.9,<1'
     ],
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
```

### Comparing `substrate-interface-1.7.2/substrate_interface.egg-info/PKG-INFO` & `substrate-interface-1.7.3/substrate_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate-interface
-Version: 1.7.2
+Version: 1.7.3
 Summary: Library for interfacing with a Substrate node
 Home-page: https://github.com/polkascan/py-substrate-interface
 Author: Stichting Polkascan (Polkascan Foundation)
 Author-email: info@polkascan.org
 License: UNKNOWN
 Description: # Python Substrate Interface
```

### Comparing `substrate-interface-1.7.2/substrate_interface.egg-info/SOURCES.txt` & `substrate-interface-1.7.3/substrate_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/__init__.py` & `substrate-interface-1.7.3/substrateinterface/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/base.py` & `substrate-interface-1.7.3/substrateinterface/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1198,23 +1198,24 @@
         for extrinsic_data in result_data['result']:
             extrinsic = self.runtime_config.create_scale_object('Extrinsic', metadata=self.metadata)
             extrinsic.decode(ScaleBytes(extrinsic_data))
             extrinsics.append(extrinsic)
 
         return extrinsics
 
-    def runtime_call(self, api: str, method: str, params: Union[list, dict] = None) -> ScaleType:
+    def runtime_call(self, api: str, method: str, params: Union[list, dict] = None, block_hash: str = None) -> ScaleType:
         """
         Calls a runtime API method
 
         Parameters
         ----------
         api: Name of the runtime API e.g. 'TransactionPaymentApi'
         method: Name of the method e.g. 'query_fee_details'
         params: List of parameters needed to call the runtime API
+        block_hash: Hash of the block at which to make the runtime API call
 
         Returns
         -------
         ScaleType
         """
         self.init_runtime()
 
@@ -1247,15 +1248,15 @@
             else:
                 if param['name'] not in params:
                     raise ValueError(f"Runtime Call param '{param['name']}' is missing")
 
                 param_data += scale_obj.encode(params[param['name']])
 
         # RPC request
-        result_data = self.rpc_request("state_call", [f'{api}_{method}', str(param_data)])
+        result_data = self.rpc_request("state_call", [f'{api}_{method}', str(param_data), block_hash])
 
         # Decode result
         result_obj = self.runtime_config.create_scale_object(runtime_call_def['type'])
         result_obj.decode(ScaleBytes(result_data['result']))
 
         return result_obj
```

### Comparing `substrate-interface-1.7.2/substrateinterface/constants.py` & `substrate-interface-1.7.3/substrateinterface/constants.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/contracts.py` & `substrate-interface-1.7.3/substrateinterface/contracts.py`

 * *Files 0% similar despite different names*

```diff
@@ -737,27 +737,28 @@
         """
 
         metadata = ContractMetadata.create_from_file(metadata_file, substrate=substrate)
 
         return cls(contract_address=contract_address, metadata=metadata, substrate=substrate)
 
     def read(self, keypair: Keypair, method: str, args: dict = None,
-             value: int = 0, gas_limit: int = None) -> GenericContractExecResult:
+             value: int = 0, gas_limit: int = None, block_hash: str = None) -> GenericContractExecResult:
         """
         Used to execute non-mutable messages to for example read data from the contract using getters. Can also be used
         to predict gas limits and 'dry-run' the execution when a mutable message is used.
         This method does not submit an extrinsic.
 
         Parameters
         ----------
         keypair
         method: name of message to execute
         args: arguments of message in {'name': value} format
         value: value to send when executing the message
         gas_limit: dict repesentation of `WeightV2` type
+        block_hash: hash of the block to execute the message on
 
         Returns
         -------
         GenericContractExecResult
         """
 
         input_data = self.metadata.generate_message_data(name=method, args=args)
@@ -766,15 +767,15 @@
         call_result = self.substrate.runtime_call("ContractsApi", "call", {
             'dest': self.contract_address,
             'gas_limit': gas_limit,
             'input_data': input_data.to_hex(),
             'origin': keypair.ss58_address,
             'value': value,
             'storage_deposit_limit': None
-        })
+        }, block_hash)
         if 'Error' in call_result['result']:
             raise ContractReadFailedException(call_result.value['result']['Error'])
 
         if 'Ok' in call_result['result']:
 
             try:
                 return_type_string = self.metadata.get_return_type_string_for_message(method)
```

### Comparing `substrate-interface-1.7.2/substrateinterface/exceptions.py` & `substrate-interface-1.7.3/substrateinterface/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/extensions.py` & `substrate-interface-1.7.3/substrateinterface/extensions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/interfaces.py` & `substrate-interface-1.7.3/substrateinterface/interfaces.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/key.py` & `substrate-interface-1.7.3/substrateinterface/key.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/keypair.py` & `substrate-interface-1.7.3/substrateinterface/keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/storage.py` & `substrate-interface-1.7.3/substrateinterface/storage.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/utils/__init__.py` & `substrate-interface-1.7.3/substrateinterface/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/utils/caching.py` & `substrate-interface-1.7.3/substrateinterface/utils/caching.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/utils/ecdsa_helpers.py` & `substrate-interface-1.7.3/substrateinterface/utils/ecdsa_helpers.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/utils/encrypted_json.py` & `substrate-interface-1.7.3/substrateinterface/utils/encrypted_json.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/utils/hasher.py` & `substrate-interface-1.7.3/substrateinterface/utils/hasher.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/substrateinterface/utils/ss58.py` & `substrate-interface-1.7.3/substrateinterface/utils/ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_block.py` & `substrate-interface-1.7.3/test/test_block.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_contracts.py` & `substrate-interface-1.7.3/test/test_contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,14 +389,20 @@
 
     def test_instance_read(self):
 
         result = self.contract.read(self.keypair, 'get')
 
         self.assertEqual(False, result.contract_result_data.value)
 
+    def test_instance_read_at_not_best_block(self):
+        parent_hash = self.substrate.get_block_header()['header']['parentHash']
+        result = self.contract.read(self.keypair, 'get', block_hash = parent_hash)
+
+        self.assertEqual(False, result.contract_result_data.value)
+
 
 class FlipperInstanceV4TestCase(FlipperInstanceTestCase):
     def setUp(self) -> None:
         self.contract = ContractInstance.create_from_address(
             contract_address="5DaohteAvvR9PZEhynqWvbFT8HEaHNuiiPTZV61VEUHnqsfU",
             metadata_file=os.path.join(os.path.dirname(__file__), 'fixtures', 'flipper-v4.json'),
             substrate=self.substrate
```

### Comparing `substrate-interface-1.7.2/test/test_create_extrinsics.py` & `substrate-interface-1.7.3/test/test_create_extrinsics.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_extension_interface.py` & `substrate-interface-1.7.3/test/test_extension_interface.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_helper_functions.py` & `substrate-interface-1.7.3/test/test_helper_functions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_init.py` & `substrate-interface-1.7.3/test/test_init.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_keypair.py` & `substrate-interface-1.7.3/test/test_keypair.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_query.py` & `substrate-interface-1.7.3/test/test_query.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_query_map.py` & `substrate-interface-1.7.3/test/test_query_map.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_rpc_compatibility.py` & `substrate-interface-1.7.3/test/test_rpc_compatibility.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_runtime_call.py` & `substrate-interface-1.7.3/test/test_runtime_call.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,14 +37,21 @@
 
     def test_core_version(self):
         result = self.substrate.runtime_call("Core", "version")
 
         self.assertGreater(result.value['spec_version'], 0)
         self.assertEqual('polkadot', result.value['spec_name'])
 
+    def test_core_version_at_not_best_block(self):
+        parent_hash = self.substrate.get_block_header()['header']['parentHash']
+        result = self.substrate.runtime_call("Core", "version", block_hash = parent_hash)
+
+        self.assertGreater(result.value['spec_version'], 0)
+        self.assertEqual('polkadot', result.value['spec_name'])
+
     def test_transaction_payment(self):
         call = self.substrate.compose_call(
             call_module='Balances',
             call_function='transfer',
             call_params={
                 'dest': 'EaG2CRhJWPb7qmdcJvy3LiWdh26Jreu9Dx6R1rXxPmYXoDk',
                 'value': 3 * 10 ** 3
```

### Comparing `substrate-interface-1.7.2/test/test_ss58.py` & `substrate-interface-1.7.3/test/test_ss58.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_subscriptions.py` & `substrate-interface-1.7.3/test/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `substrate-interface-1.7.2/test/test_type_registry.py` & `substrate-interface-1.7.3/test/test_type_registry.py`

 * *Files identical despite different names*

