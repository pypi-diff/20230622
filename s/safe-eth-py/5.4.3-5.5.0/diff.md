# Comparing `tmp/safe-eth-py-5.4.3.tar.gz` & `tmp/safe-eth-py-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safe-eth-py-5.4.3.tar", last modified: Tue May 23 14:51:22 2023, max compression
+gzip compressed data, was "safe-eth-py-5.5.0.tar", last modified: Thu Jun 22 15:02:46 2023, max compression
```

## Comparing `safe-eth-py-5.4.3.tar` & `safe-eth-py-5.5.0.tar`

### file list

```diff
@@ -1,195 +1,195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.134838 safe-eth-py-5.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-23 14:51:22.134838 safe-eth-py-5.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.086838 safe-eth-py-5.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.090838 safe-eth-py-5.4.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.eth.clients.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.eth.contracts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.eth.django.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.eth.eip712.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.eth.oracles.abis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.eth.oracles.rst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.eth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/gnosis.safe.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/docs/source/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.090838 safe-eth-py-5.4.3/gnosis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.094838 safe-eth-py-5.4.3/gnosis/eth/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.094838 safe-eth-py-5.4.3/gnosis/eth/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/abis/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.094838 safe-eth-py-5.4.3/gnosis/eth/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/clients/blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/clients/contract_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/clients/etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/clients/sourcify.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.106838 safe-eth-py-5.4.3/gnosis/eth/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/CPKFactory.json
--rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/DelegateConstructorProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/ERC1155.json
--rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20.json
--rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20TestToken.json
--rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/ERC721.json
--rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
--rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/MultiSend.json
--rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/PayingProxy.json
--rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_0_0.json
--rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_1_1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_3_0.json
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/kyber_network_proxy.json
--rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_exchange.json
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_factory.json
--rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_pair.json
--rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_router.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.110838 safe-eth-py-5.4.3/gnosis/eth/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.114838 safe-eth-py-5.4.3/gnosis/eth/django/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/django/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.114838 safe-eth-py-5.4.3/gnosis/eth/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    77427 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20850 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/ethereum_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/multicall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.114838 safe-eth-py-5.4.3/gnosis/eth/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.118838 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/aave_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/balancer_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/cream_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/curve_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/mooniswap_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/superfluid_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/yearn_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/abis/zerion_abis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.118838 safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/curve_gauge_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)    32144 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/oracles/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.118838 safe-eth-py-5.4.3/gnosis/eth/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.122838 safe-eth-py-5.4.3/gnosis/eth/tests/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/clients/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_blockscout_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_etherscan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_sourcify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.122838 safe-eth-py-5.4.3/gnosis/eth/tests/eip712/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/eip712/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/eip712/test_eip712.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/ethereum_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.122838 safe-eth-py-5.4.3/gnosis/eth/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_internal_txs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_log_receipts.py
--rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_block.py
--rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.126838 safe-eth-py-5.4.3/gnosis/eth/tests/oracles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/oracles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_cowswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_kyber.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_superfluid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_sushiswap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_uniswap_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/test_ethereum_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/test_oracles.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/eth/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.126838 safe-eth-py-5.4.3/gnosis/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/protocol/gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/protocol/order.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.126838 safe-eth-py-5.4.3/gnosis/protocol/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/protocol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/protocol/tests/test_gnosis_protocol_api.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.130838 safe-eth-py-5.4.3/gnosis/safe/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32077 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/addresses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.130838 safe-eth-py-5.4.3/gnosis/safe/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/api/base_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/api/relay_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/api/transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    42768 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/signatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.134838 safe-eth-py-5.4.3/gnosis/safe/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.134838 safe-eth-py-5.4.3/gnosis/safe/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/api/test_transaction_service_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/safe_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_multi_send.py
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_proxy_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    34197 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_create2_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_creation_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_signature.py
--rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_tx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/test_signatures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/safe/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.134838 safe-eth-py-5.4.3/gnosis/util/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/gnosis/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 14:51:22.134838 safe-eth-py-5.4.3/safe_eth_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-23 14:51:22.000000 safe-eth-py-5.4.3/safe_eth_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-23 14:51:22.000000 safe-eth-py-5.4.3/safe_eth_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 14:51:22.000000 safe-eth-py-5.4.3/safe_eth_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-23 14:51:22.000000 safe-eth-py-5.4.3/safe_eth_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-23 14:51:22.000000 safe-eth-py-5.4.3/safe_eth_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-23 14:51:22.138838 safe-eth-py-5.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 14:51:02.000000 safe-eth-py-5.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.507445 safe-eth-py-5.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.511445 safe-eth-py-5.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.clients.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.contracts.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.django.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.eip712.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.oracles.abis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.oracles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.eth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/gnosis.safe.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8492 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/docs/source/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.511445 safe-eth-py-5.5.0/gnosis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.511445 safe-eth-py-5.5.0/gnosis/eth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.515445 safe-eth-py-5.5.0/gnosis/eth/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/abis/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.515445 safe-eth-py-5.5.0/gnosis/eth/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/contract_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/clients/sourcify.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)   328664 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/CPKFactory.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28908 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26897 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/DelegateConstructorProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29068 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC1155.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54748 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89890 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20TestToken.json
+-rw-r--r--   0 runner    (1001) docker     (123)   622260 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ERC721.json
+-rw-r--r--   0 runner    (1001) docker     (123)   983403 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1158944 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1347363 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   119875 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19886 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/MultiSend.json
+-rw-r--r--   0 runner    (1001) docker     (123)    78793 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/PayingProxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)   136946 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)   288861 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18975 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32495 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_0_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)    39032 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_1_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_3_0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/kyber_network_proxy.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17165 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_exchange.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_factory.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8293 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_pair.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11889 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_router.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5740 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/django/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/tests/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/django/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.527445 safe-eth-py-5.5.0/gnosis/eth/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77429 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/ethereum_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13603 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/multicall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.531445 safe-eth-py-5.5.0/gnosis/eth/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.531445 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/aave_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30036 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/balancer_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29731 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/cream_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27567 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/curve_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/mooniswap_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/superfluid_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45208 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36257 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/yearn_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/abis/zerion_abis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/curve_gauge_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4194 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32229 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/oracles/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/tests/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107062 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_blockscout_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_etherscan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_sourcify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.535445 safe-eth-py-5.5.0/gnosis/eth/tests/eip712/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/eip712/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/eip712/test_eip712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/ethereum_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.539445 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31306 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_internal_txs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_log_receipts.py
+-rw-r--r--   0 runner    (1001) docker     (123)   793149 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92795 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)   171076 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.539445 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_cowswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_kyber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_superfluid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_sushiswap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_uniswap_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61046 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_ethereum_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_oracles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/eth/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.539445 safe-eth-py-5.5.0/gnosis/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9511 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/order.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.543445 safe-eth-py-5.5.0/gnosis/protocol/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/protocol/tests/test_gnosis_protocol_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.543445 safe-eth-py-5.5.0/gnosis/safe/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32683 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/addresses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/safe/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/base_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/relay_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/api/transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8070 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42768 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16881 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/signatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/safe/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/safe/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/api/test_transaction_service_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/safe_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10515 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_multi_send.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_proxy_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34197 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16628 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_create2_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_creation_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14117 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_tx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/test_signatures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/safe/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.547445 safe-eth-py-5.5.0/gnosis/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/gnosis/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/safe_eth_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 15:02:46.000000 safe-eth-py-5.5.0/safe_eth_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-22 15:02:46.551445 safe-eth-py-5.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-22 15:02:22.000000 safe-eth-py-5.5.0/setup.py
```

### Comparing `safe-eth-py-5.4.3/LICENSE` & `safe-eth-py-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/PKG-INFO` & `safe-eth-py-5.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.4.3
+Version: 5.5.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.4.3/README.rst` & `safe-eth-py-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/Makefile` & `safe-eth-py-5.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/make.bat` & `safe-eth-py-5.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/conf.py` & `safe-eth-py-5.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/gnosis.eth.clients.rst` & `safe-eth-py-5.5.0/docs/source/gnosis.eth.clients.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/gnosis.eth.django.rst` & `safe-eth-py-5.5.0/docs/source/gnosis.eth.django.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/gnosis.eth.oracles.abis.rst` & `safe-eth-py-5.5.0/docs/source/gnosis.eth.oracles.abis.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/gnosis.eth.rst` & `safe-eth-py-5.5.0/docs/source/gnosis.eth.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/gnosis.safe.rst` & `safe-eth-py-5.5.0/docs/source/gnosis.safe.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/index.rst` & `safe-eth-py-5.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/docs/source/quickstart.rst` & `safe-eth-py-5.5.0/docs/source/quickstart.rst`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/__init__.py` & `safe-eth-py-5.5.0/gnosis/eth/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/abis/multicall.py` & `safe-eth-py-5.5.0/gnosis/eth/abis/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/clients/__init__.py` & `safe-eth-py-5.5.0/gnosis/eth/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/clients/blockscout_client.py` & `safe-eth-py-5.5.0/gnosis/eth/clients/blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/clients/etherscan_client.py` & `safe-eth-py-5.5.0/gnosis/eth/clients/etherscan_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,34 +71,57 @@
         EthereumNetwork.NEON_EVM_DEVNET: "https://devnet-api.neonscan.org",
         EthereumNetwork.SEPOLIA: "https://api-sepolia.etherscan.io",
     }
     HTTP_HEADERS = {
         "User-Agent": "curl/7.77.0",
     }
 
-    def __init__(self, network: EthereumNetwork, api_key: Optional[str] = None):
+    def __init__(
+        self,
+        network: EthereumNetwork,
+        api_key: Optional[str] = None,
+        request_timeout: int = 10,
+    ):
         self.network = network
         self.api_key = api_key
         self.base_url = self.NETWORK_WITH_URL.get(network)
         self.base_api_url = self.NETWORK_WITH_API_URL.get(network)
         if self.base_api_url is None:
             raise EtherscanClientConfigurationProblem(
                 f"Network {network.name} - {network.value} not supported"
             )
-        self.http_session = requests.Session()
+        self.http_session = self._prepare_http_session()
         self.http_session.headers = self.HTTP_HEADERS
+        self.request_timeout = request_timeout
+
+    def _prepare_http_session(self) -> requests.Session:
+        """
+        Prepare http session with custom pooling. See:
+        https://urllib3.readthedocs.io/en/stable/advanced-usage.html
+        https://docs.python-requests.org/en/v1.2.3/api/#requests.adapters.HTTPAdapter
+        https://web3py.readthedocs.io/en/stable/providers.html#httpprovider
+        """
+        session = requests.Session()
+        adapter = requests.adapters.HTTPAdapter(
+            pool_connections=10,
+            pool_maxsize=100,
+            pool_block=False,
+        )
+        session.mount("http://", adapter)
+        session.mount("https://", adapter)
+        return session
 
     def build_url(self, path: str):
         url = urljoin(self.base_api_url, path)
         if self.api_key:
             url += f"&apikey={self.api_key}"
         return url
 
     def _do_request(self, url: str) -> Optional[Dict[str, Any]]:
-        response = self.http_session.get(url)
+        response = self.http_session.get(url, timeout=self.request_timeout)
 
         if response.ok:
             response_json = response.json()
             result = response_json["result"]
             if "Max rate limit reached" in result:
                 # Max rate limit reached, please use API Key for higher rate limit
                 raise EtherscanRateLimitError
```

### Comparing `safe-eth-py-5.4.3/gnosis/eth/constants.py` & `safe-eth-py-5.5.0/gnosis/eth/constants.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/CPKFactory.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/CPKFactory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/CompatibilityFallbackHandler_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/DelegateConstructorProxy.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/DelegateConstructorProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/ERC1155.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC1155.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/ERC20TestToken.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC20TestToken.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/ERC721.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/ERC721.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V0_0_1.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V0_0_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_0_0.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_1_1.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/GnosisSafe_V1_3_0.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/GnosisSafe_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/MultiSend.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/MultiSend.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/PayingProxy.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/PayingProxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_0_0.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_1_1.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/ProxyFactory_V1_3_0.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/ProxyFactory_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_0_0.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_0_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_1_1.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_1_1.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/Proxy_V1_3_0.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/Proxy_V1_3_0.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/__init__.py` & `safe-eth-py-5.5.0/gnosis/eth/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/kyber_network_proxy.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/kyber_network_proxy.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_exchange.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_exchange.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_factory.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_factory.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_factory.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_pair.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_pair.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/contracts/uniswap_v2_router.json` & `safe-eth-py-5.5.0/gnosis/eth/contracts/uniswap_v2_router.json`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/admin.py` & `safe-eth-py-5.5.0/gnosis/eth/django/admin.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/forms.py` & `safe-eth-py-5.5.0/gnosis/eth/django/forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/models.py` & `safe-eth-py-5.5.0/gnosis/eth/django/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/serializers.py` & `safe-eth-py-5.5.0/gnosis/eth/django/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/tests/models.py` & `safe-eth-py-5.5.0/gnosis/eth/django/tests/models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/tests/test_forms.py` & `safe-eth-py-5.5.0/gnosis/eth/django/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/tests/test_models.py` & `safe-eth-py-5.5.0/gnosis/eth/django/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/django/tests/test_serializers.py` & `safe-eth-py-5.5.0/gnosis/eth/django/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/eip712/__init__.py` & `safe-eth-py-5.5.0/gnosis/eth/eip712/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/ethereum_client.py` & `safe-eth-py-5.5.0/gnosis/eth/ethereum_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
             cls.instance = EthereumClient(
                 settings.ETHEREUM_NODE_URL,
                 provider_timeout=int(os.environ.get("ETHEREUM_RPC_TIMEOUT", 10)),
                 slow_provider_timeout=int(
                     os.environ.get("ETHEREUM_RPC_SLOW_TIMEOUT", 60)
                 ),
-                retry_count=int(os.environ.get("ETHEREUM_RPC_RETRY_COUNT", 60)),
+                retry_count=int(os.environ.get("ETHEREUM_RPC_RETRY_COUNT", 1)),
                 batch_request_max_size=int(
                     os.environ.get("ETHEREUM_RPC_BATCH_REQUEST_MAX_SIZE", 500)
                 ),
             )
         return cls.instance
 
 
@@ -1154,15 +1154,15 @@
     NULL_ADDRESS = NULL_ADDRESS
 
     def __init__(
         self,
         ethereum_node_url: URI = URI("http://localhost:8545"),
         provider_timeout: int = 15,
         slow_provider_timeout: int = 60,
-        retry_count: int = 3,
+        retry_count: int = 1,
         use_caching_middleware: bool = True,
         batch_request_max_size: int = 500,
     ):
         """
         :param ethereum_node_url: Ethereum RPC uri
         :param provider_timeout: Timeout for regular RPC queries
         :param slow_provider_timeout: Timeout for slow (tracing, logs...) and custom RPC queries
@@ -1207,15 +1207,15 @@
     def __str__(self):
         return f"EthereumClient for url={self.ethereum_node_url}"
 
     def _prepare_http_session(self, retry_count: int) -> requests.Session:
         """
         Prepare http session with custom pooling. See:
         https://urllib3.readthedocs.io/en/stable/advanced-usage.html
-        https://2.python-requests.org/en/latest/api/#requests.adapters.HTTPAdapter
+        https://docs.python-requests.org/en/v1.2.3/api/#requests.adapters.HTTPAdapter
         https://web3py.readthedocs.io/en/stable/providers.html#httpprovider
         """
         session = requests.Session()
         adapter = requests.adapters.HTTPAdapter(
             pool_connections=1,  # Doing all the connections to the same url
             pool_maxsize=100,  # Number of concurrent connections
             max_retries=retry_count,  # Nodes are not very responsive some times
```

### Comparing `safe-eth-py-5.4.3/gnosis/eth/ethereum_network.py` & `safe-eth-py-5.5.0/gnosis/eth/ethereum_network.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,14 +130,15 @@
     FACTORY_127_MAINNET = 127
     HUOBI_ECO_CHAIN_MAINNET = 128
     ALYX_CHAIN_TESTNET = 135
     POLYGON = 137
     OPENPIECE_TESTNET = 141
     DAX_CHAIN = 142
     PHI_NETWORK_V2 = 144
+    TENET_TESTNET = 155
     ARMONIA_EVA_CHAIN_MAINNET = 160
     ARMONIA_EVA_CHAIN_TESTNET = 161
     LIGHTSTREAMS_TESTNET = 162
     LIGHTSTREAMS_MAINNET = 163
     AIOZ_NETWORK = 168
     HOO_SMART_CHAIN_TESTNET = 170
     LATAM_BLOCKCHAIN_RESIL_TESTNET = 172
@@ -303,14 +304,15 @@
     GANACHE = 1337
     CIC_CHAIN_MAINNET = 1353
     POLYGON_ZKEVM_TESTNET = 1402
     CTEX_SCAN_BLOCKCHAIN = 1455
     SHERPAX_MAINNET = 1506
     SHERPAX_TESTNET = 1507
     BEAGLE_MESSAGING_CHAIN = 1515
+    TENET = 1559
     CATECOIN_CHAIN_MAINNET = 1618
     ATHEIOS = 1620
     BTACHAIN = 1657
     LUDAN_MAINNET = 1688
     ANYTYPE_EVM_CHAIN = 1701
     TBSI_MAINNET = 1707
     TBSI_TESTNET = 1708
```

### Comparing `safe-eth-py-5.4.3/gnosis/eth/exceptions.py` & `safe-eth-py-5.5.0/gnosis/eth/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/multicall.py` & `safe-eth-py-5.5.0/gnosis/eth/multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/__init__.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/aave_abis.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/aave_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/balancer_abis.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/balancer_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/cream_abis.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/cream_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/curve_abis.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/curve_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/mooniswap_abis.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/mooniswap_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/uniswap_v3.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/yearn_abis.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/yearn_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/abis/zerion_abis.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/abis/zerion_abis.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/cowswap.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/helpers/curve_gauge_list.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/helpers/curve_gauge_list.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/kyber.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/oracles.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/oracles.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,19 @@
                 "jsonrpc": "2.0",
                 "method": "eth_call",
                 "params": [{"to": token_address, "data": data}, "latest"],
             }
             for i, data in enumerate(datas)
         ]
         payloads = [payload_balance] + payload_calls
-        r = requests.post(self.ethereum_client.ethereum_node_url, json=payloads)
+        r = requests.post(
+            self.ethereum_client.ethereum_node_url,
+            json=payloads,
+            timeout=self.ethereum_client.timeout,
+        )
         if not r.ok:
             raise CannotGetPriceFromOracle(
                 f"Error from node with url={self.ethereum_client.ethereum_node_url}"
             )
 
         results = []
         for result in r.json():
```

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/superfluid.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/sushiswap.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/uniswap_v3.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/oracles/utils.py` & `safe-eth-py-5.5.0/gnosis/eth/oracles/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/clients/mocks.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/clients/mocks.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_blockscout_client.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_blockscout_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_etherscan_client.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_etherscan_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/clients/test_sourcify.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/clients/test_sourcify.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/eip712/test_eip712.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/eip712/test_eip712.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/ethereum_test_case.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/ethereum_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_internal_txs.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_internal_txs.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_log_receipts.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_log_receipts.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_block.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_block.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_filter.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_filter.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/mocks/mock_trace_transaction.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/mocks/mock_trace_transaction.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_cowswap.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_cowswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_kyber.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_kyber.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_superfluid.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_superfluid.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_sushiswap.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_sushiswap.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/oracles/test_uniswap_v3.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/oracles/test_uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/test_ethereum_client.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/test_ethereum_client.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/test_multicall.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/test_multicall.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/test_oracles.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/test_oracles.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/test_utils.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/eth/tests/utils.py` & `safe-eth-py-5.5.0/gnosis/eth/tests/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+import json
 import os
+from copy import deepcopy
+from typing import Any
 
 import pytest
 import requests
 from eth_account.signers.local import LocalAccount
+from hexbytes import HexBytes
 from web3 import Web3
 from web3.contract import Contract
 from web3.types import TxParams
 
 from ..contracts import get_example_erc20_contract
 
 
@@ -136,7 +140,39 @@
         ).transact({"from": deployer})
 
     tx_receipt = w3.eth.wait_for_transaction_receipt(tx_hash)
     erc20_address = tx_receipt.contractAddress
     deployed_erc20 = get_example_erc20_contract(w3, erc20_address)
     assert deployed_erc20.functions.balanceOf(owner).call() == amount
     return deployed_erc20
+
+
+def bytes_to_str(o: Any) -> Any:
+    """
+    Converts bytes (and hexbytes) fields to `str` in nested data types
+
+    :param o:
+    :return:
+    """
+    if isinstance(o, bytes):
+        return HexBytes(o).hex()
+    if isinstance(o, dict):
+        o = dict(o)  # Remove AttributeDict
+        for k in o.keys():
+            o[k] = bytes_to_str(o[k])
+    elif isinstance(o, (list, tuple)):
+        o = deepcopy(o)
+        for i, v in enumerate(o):
+            o[i] = bytes_to_str(o[i])
+    elif isinstance(o, set):
+        o = {bytes_to_str(element) for element in o}
+    return o
+
+
+def to_json_with_hexbytes(o: Any) -> str:
+    """
+    Convert RPC calls with nested bytes/Hexbytes to json and compare. Useful for RPC calls
+
+    :param o:
+    :return: Object as JSON with Hexbytes/bytes parsed correctly as an hex string
+    """
+    return json.dumps(bytes_to_str(o), indent=4, sort_keys=True)
```

### Comparing `safe-eth-py-5.4.3/gnosis/eth/utils.py` & `safe-eth-py-5.5.0/gnosis/eth/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/protocol/gnosis_protocol_api.py` & `safe-eth-py-5.5.0/gnosis/protocol/gnosis_protocol_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,25 +50,43 @@
 
     API_BASE_URLS = {
         EthereumNetwork.MAINNET: "https://api.cow.fi/mainnet/api/v1/",
         EthereumNetwork.GOERLI: "https://api.cow.fi/goerli/api/v1/",
         EthereumNetwork.GNOSIS: "https://api.cow.fi/xdai/api/v1/",
     }
 
-    def __init__(self, ethereum_network: EthereumNetwork):
+    def __init__(self, ethereum_network: EthereumNetwork, request_timeout: int = 10):
         self.network = ethereum_network
         if self.network not in self.API_BASE_URLS:
             raise EthereumNetworkNotSupported(
                 f"{self.network.name} network not supported by Gnosis Protocol"
             )
         self.settlement_contract_address = self.SETTLEMENT_CONTRACT_ADDRESSES[
             self.network
         ]
         self.base_url = self.API_BASE_URLS[self.network]
-        self.http_session = requests.Session()
+        self.http_session = self._prepare_http_session()
+        self.request_timeout = request_timeout
+
+    def _prepare_http_session(self) -> requests.Session:
+        """
+        Prepare http session with custom pooling. See:
+        https://urllib3.readthedocs.io/en/stable/advanced-usage.html
+        https://docs.python-requests.org/en/v1.2.3/api/#requests.adapters.HTTPAdapter
+        https://web3py.readthedocs.io/en/stable/providers.html#httpprovider
+        """
+        session = requests.Session()
+        adapter = requests.adapters.HTTPAdapter(
+            pool_connections=10,
+            pool_maxsize=100,
+            pool_block=False,
+        )
+        session.mount("http://", adapter)
+        session.mount("https://", adapter)
+        return session
 
     @cached_property
     def weth_address(self) -> ChecksumAddress:
         """
         :return: Wrapped ether checksummed address
         """
         if self.network == EthereumNetwork.GNOSIS:  # WXDAI
@@ -94,15 +112,15 @@
             "feeAmount": str(order.feeAmount),
             "kind": order.kind,
             "partiallyFillable": order.partiallyFillable,
             "signingScheme": "ethsign",
             "from": from_address,
             "priceQuality": "fast",
         }
-        r = self.http_session.post(url, json=data_json)
+        r = self.http_session.post(url, json=data_json, timeout=self.request_timeout)
         if r.ok:
             return r.json()
         else:
             return ErrorResponse(r.json())
 
     def get_fee(
         self, order: Order, from_address: ChecksumAddress
@@ -155,15 +173,15 @@
             "feeAmount": str(order.feeAmount),
             "kind": order.kind,
             "partiallyFillable": order.partiallyFillable,
             "signature": signed_message.signature.hex(),
             "signingScheme": "ethsign",
             "from": from_address,
         }
-        r = self.http_session.post(url, json=data_json)
+        r = self.http_session.post(url, json=data_json, timeout=self.request_timeout)
         if r.ok:
             return HexStr(r.json())
         else:
             return ErrorResponse(r.json())
 
     def get_orders(
         self, owner: ChecksumAddress, offset: int = 0, limit=10
@@ -175,15 +193,15 @@
         :return: Orders of one user paginated. The orders are ordered by their creation
             date descending (newest orders first).
             To enumerate all orders start with offset 0 and keep increasing the offset by the
             total number of returned results. When a response contains less than the limit
             the last page has been reached.
         """
         url = self.base_url + f"account/{owner}/orders"
-        r = self.http_session.get(url)
+        r = self.http_session.get(url, timeout=self.request_timeout)
         if r.ok:
             return cast(List[Dict[str, Any]], r.json())
         else:
             return ErrorResponse(r.json())
 
     def get_trades(
         self, order_ui: Optional[HexStr] = None, owner: Optional[ChecksumAddress] = None
@@ -193,15 +211,15 @@
         ), "order_ui or owner must be provided, but not both"
         url = self.base_url + "trades/?"
         if order_ui:
             url += f"orderUid={order_ui}"
         elif owner:
             url += f"owner={owner}"
 
-        r = self.http_session.get(url)
+        r = self.http_session.get(url, timeout=self.request_timeout)
         if r.ok:
             return cast(List[TradeResponse], r.json())
         else:
             return ErrorResponse(r.json())
 
     def get_estimated_amount(
         self,
```

### Comparing `safe-eth-py-5.4.3/gnosis/protocol/order.py` & `safe-eth-py-5.5.0/gnosis/protocol/order.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/protocol/tests/test_gnosis_protocol_api.py` & `safe-eth-py-5.5.0/gnosis/protocol/tests/test_gnosis_protocol_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/__init__.py` & `safe-eth-py-5.5.0/gnosis/safe/__init__.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/addresses.py` & `safe-eth-py-5.5.0/gnosis/safe/addresses.py`

 * *Files 2% similar despite different names*

```diff
@@ -460,14 +460,22 @@
         ),  # Default singleton address
         (
             "0x69f4D1788e39c87893C980c06EdF4b7f686e2938",
             2087040,
             "1.3.0",
         ),  # Safe singleton address
     ],
+    EthereumNetwork.TENET_TESTNET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 885391, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 885392, "1.3.0"),
+    ],
+    EthereumNetwork.TENET: [
+        ("0xfb1bffC9d739B8D520DaF37dF666da4C687191EA", 727470, "1.3.0+L2"),
+        ("0x69f4D1788e39c87893C980c06EdF4b7f686e2938", 727472, "1.3.0"),
+    ],
 }
 
 PROXY_FACTORIES: Dict[EthereumNetwork, List[Tuple[str, int]]] = {
     EthereumNetwork.MAINNET: [
         (
             "0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC",
             14981216,
@@ -765,8 +773,14 @@
             2087031,
         ),  # v1.3.0  Safe singleton address
         (
             "0xa6B71E26C5e0845f74c812102Ca7114b6a896AB2",
             2086864,
         ),  # v1.3.0  Default singleton address
     ],
+    EthereumNetwork.TENET_TESTNET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 885379),  # v1.3.0
+    ],
+    EthereumNetwork.TENET: [
+        ("0xC22834581EbC8527d974F8a1c97E1bEA4EF910BC", 727457),  # v1.3.0
+    ],
 }
```

### Comparing `safe-eth-py-5.4.3/gnosis/safe/api/relay_service_api.py` & `safe-eth-py-5.5.0/gnosis/safe/api/relay_service_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             "safeTxGas": safe_tx.safe_tx_gas,
             "dataGas": safe_tx.base_gas,
             "gasPrice": safe_tx.gas_price,
             "refundReceiver": safe_tx.refund_receiver,
             "nonce": safe_tx.safe_nonce,
             "signatures": signatures,
         }
-        response = requests.post(url, json=data)
+        response = requests.post(url, json=data, timeout=self.request_timeout)
         if not response.ok:
             raise SafeAPIException(f"Error posting transaction: {response.content}")
         else:
             return RelaySentTransaction(response.json())
 
     def get_estimation(self, safe_address: str, safe_tx: SafeTx) -> RelayEstimation:
         """
@@ -78,15 +78,15 @@
         data = {
             "to": safe_tx.to,
             "value": safe_tx.value,
             "data": safe_tx.data.hex() if safe_tx.data else None,
             "operation": safe_tx.operation,
             "gasToken": safe_tx.gas_token,
         }
-        response = requests.post(url, json=data)
+        response = requests.post(url, json=data, timeout=self.request_timeout)
         if not response.ok:
             raise SafeAPIException(f"Error posting transaction: {response.content}")
         else:
             response_json = response.json()
             # Convert values to int
             for key in ("safeTxGas", "baseGas", "gasPrice"):
                 response_json[key] = int(response_json[key])
```

### Comparing `safe-eth-py-5.4.3/gnosis/safe/api/transaction_service_api.py` & `safe-eth-py-5.5.0/gnosis/safe/api/transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/exceptions.py` & `safe-eth-py-5.5.0/gnosis/safe/exceptions.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/multi_send.py` & `safe-eth-py-5.5.0/gnosis/safe/multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/proxy_factory.py` & `safe-eth-py-5.5.0/gnosis/safe/proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/safe.py` & `safe-eth-py-5.5.0/gnosis/safe/safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/safe_create2_tx.py` & `safe-eth-py-5.5.0/gnosis/safe/safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/safe_creation_tx.py` & `safe-eth-py-5.5.0/gnosis/safe/safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/safe_signature.py` & `safe-eth-py-5.5.0/gnosis/safe/safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/safe_tx.py` & `safe-eth-py-5.5.0/gnosis/safe/safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/serializers.py` & `safe-eth-py-5.5.0/gnosis/safe/serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/signatures.py` & `safe-eth-py-5.5.0/gnosis/safe/signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/api/test_transaction_service_api.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/api/test_transaction_service_api.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/safe_test_case.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/safe_test_case.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_addresses.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_addresses.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_multi_send.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_multi_send.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_proxy_factory.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_safe.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_create2_tx.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_create2_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_creation_tx.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_creation_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_signature.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_signature.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_safe_tx.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_safe_tx.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_serializers.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/test_signatures.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/test_signatures.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/gnosis/safe/tests/utils.py` & `safe-eth-py-5.5.0/gnosis/safe/tests/utils.py`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/safe_eth_py.egg-info/PKG-INFO` & `safe-eth-py-5.5.0/safe_eth_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safe-eth-py
-Version: 5.4.3
+Version: 5.5.0
 Summary: Safe Ecosystem Foundation utilities for Ethereum projects
 Home-page: https://github.com/safe-global/safe-eth-py
 Author: Uxío
 Author-email: uxio@safe.global
 License: MIT License
 Project-URL: Documentation, https://safe-eth-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/safe-global/safe-eth-py
```

### Comparing `safe-eth-py-5.4.3/safe_eth_py.egg-info/SOURCES.txt` & `safe-eth-py-5.5.0/safe_eth_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safe-eth-py-5.4.3/setup.cfg` & `safe-eth-py-5.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = safe-eth-py
-version = 5.4.3
+version = 5.5.0
 description = Safe Ecosystem Foundation utilities for Ethereum projects
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 keywords = 
 	ethereum
 	web3
 	django
```

