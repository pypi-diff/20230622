# Comparing `tmp/ypricemagic-2.3.8.tar.gz` & `tmp/ypricemagic-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.3.8.tar", last modified: Thu Jun 22 00:01:41 2023, max compression
+gzip compressed data, was "ypricemagic-2.4.0.tar", last modified: Thu Jun 22 19:10:40 2023, max compression
```

## Comparing `ypricemagic-2.3.8.tar` & `ypricemagic-2.4.0.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.930053 ypricemagic-2.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20584 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19868 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6847 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11264 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8741 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.628031 ypricemagic-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.588031 ypricemagic-2.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.600031 ypricemagic-2.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-22 19:10:40.628031 ypricemagic-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-22 19:10:40.632031 ypricemagic-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.604031 ypricemagic-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.604031 ypricemagic-2.4.0/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.604031 ypricemagic-2.4.0/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.608031 ypricemagic-2.4.0/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.608031 ypricemagic-2.4.0/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.608031 ypricemagic-2.4.0/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.608031 ypricemagic-2.4.0/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.608031 ypricemagic-2.4.0/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.612031 ypricemagic-2.4.0/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.612031 ypricemagic-2.4.0/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20584 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19868 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.616031 ypricemagic-2.4.0/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.620031 ypricemagic-2.4.0/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.620031 ypricemagic-2.4.0/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.620031 ypricemagic-2.4.0/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9131 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11264 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.620031 ypricemagic-2.4.0/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.620031 ypricemagic-2.4.0/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.624031 ypricemagic-2.4.0/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8741 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.628031 ypricemagic-2.4.0/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.628031 ypricemagic-2.4.0/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-22 19:10:27.000000 ypricemagic-2.4.0/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 19:10:40.628031 ypricemagic-2.4.0/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-22 19:10:40.000000 ypricemagic-2.4.0/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-22 19:10:40.000000 ypricemagic-2.4.0/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 19:10:40.000000 ypricemagic-2.4.0/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-22 19:10:40.000000 ypricemagic-2.4.0/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-22 19:10:40.000000 ypricemagic-2.4.0/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.3.8/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.4.0/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/.github/workflows/pytest.yaml` & `ypricemagic-2.4.0/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/.github/workflows/release.yaml` & `ypricemagic-2.4.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/LICENSE.txt` & `ypricemagic-2.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/README.md` & `ypricemagic-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/setup.py` & `ypricemagic-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/classes/test_erc20.py` & `ypricemagic-2.4.0/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/classes/test_singleton.py` & `ypricemagic-2.4.0/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/fixtures.py` & `ypricemagic-2.4.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.4.0/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/lending/test_aave.py` & `ypricemagic-2.4.0/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/lending/test_compound.py` & `ypricemagic-2.4.0/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/test_chainlink.py` & `ypricemagic-2.4.0/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/test_magic.py` & `ypricemagic-2.4.0/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/test_popsicle.py` & `ypricemagic-2.4.0/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/test_synthetix.py` & `ypricemagic-2.4.0/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/test_yearn.py` & `ypricemagic-2.4.0/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/tests/prices/utils/test_buckets.py` & `ypricemagic-2.4.0/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/__init__.py` & `ypricemagic-2.4.0/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/classes/common.py` & `ypricemagic-2.4.0/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/classes/singleton.py` & `ypricemagic-2.4.0/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/constants.py` & `ypricemagic-2.4.0/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/contracts.py` & `ypricemagic-2.4.0/y/contracts.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/datatypes.py` & `ypricemagic-2.4.0/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/decorators.py` & `ypricemagic-2.4.0/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/erc20.py` & `ypricemagic-2.4.0/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/exceptions.py` & `ypricemagic-2.4.0/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/interfaces/ERC20.py` & `ypricemagic-2.4.0/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.4.0/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/interfaces/compound/unitroller.py` & `ypricemagic-2.4.0/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.4.0/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/interfaces/multicall2.py` & `ypricemagic-2.4.0/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.4.0/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.4.0/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/networks.py` & `ypricemagic-2.4.0/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/band.py` & `ypricemagic-2.4.0/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/chainlink.py` & `ypricemagic-2.4.0/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/convex.py` & `ypricemagic-2.4.0/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.4.0/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/balancer/v1.py` & `ypricemagic-2.4.0/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/balancer/v2.py` & `ypricemagic-2.4.0/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/genericamm.py` & `ypricemagic-2.4.0/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/mooniswap.py` & `ypricemagic-2.4.0/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.4.0/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.4.0/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.4.0/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.4.0/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.4.0/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/eth_derivs/creth.py` & `ypricemagic-2.4.0/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.4.0/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/gearbox.py` & `ypricemagic-2.4.0/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/lending/aave.py` & `ypricemagic-2.4.0/y/prices/lending/aave.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,17 +31,43 @@
         "0xcE744a9BAf573167B2CF138114BA32ed7De274Fa", # umee
     ],
     Network.Polygon: [
         "0x8dFf5E27EA6b7AC08EbFdf9eB090F32ee9a30fcf", # aave
     ],
     Network.Avalanche: [
         "0x70BbE4A294878a14CB3CDD9315f5EB490e346163", # blizz
-    ]
+    ],
 }.get(chain.id, [])        
 
+v3_pools = {
+    Network.Mainnet: [
+        "0x87870Bca3F3fD6335C3F4ce8392D69350B4fA4E2", # aave v3
+    ],
+    Network.Optimism: [
+        "0x794a61358D6845594F94dc1DB02A252b5b4814aD", # aave v3
+    ],
+    Network.Arbitrum: [
+        "0x794a61358D6845594F94dc1DB02A252b5b4814aD", # aave v3
+    ],
+    Network.Harmony: [
+        "0x794a61358D6845594F94dc1DB02A252b5b4814aD", # aave v3
+    ],
+    Network.Arbitrum: [
+        "0x794a61358D6845594F94dc1DB02A252b5b4814aD", # aave v3
+    ],
+    Network.Fantom: [
+        "0x794a61358D6845594F94dc1DB02A252b5b4814aD", # aave v3
+    ],
+    Network.Avalanche: [
+        "0x794a61358D6845594F94dc1DB02A252b5b4814aD", # aave v3
+    ],
+    Network.Polygon: [
+        "0x794a61358D6845594F94dc1DB02A252b5b4814aD", # aave v3
+    ],
+}.get(chain.id, [])
 
 class AaveMarketBase(ContractBase):
     def __contains__(self, __o: object) -> bool:
         if not self.asynchronous:
             cls = self.__class__.__name__
             raise RuntimeError(f"'self.asynchronous' must be False to use {cls}.__contains__.\nYou may wish to use {cls}.is_atoken instead.")
         return convert.to_address(__o) in self.atokens
@@ -85,36 +111,68 @@
             for reserve in reserves
         ])
 
         try:
             atokens = [ERC20(reserve_data[7], asynchronous=self.asynchronous) for reserve_data in reserves_data]
             logger.info(f'loaded {len(atokens)} v2 atokens for {self.__repr__()}')
             return atokens
-        except TypeError: # TODO figure out what to do about non verified aave markets
+        except TypeError as e: # TODO figure out what to do about non verified aave markets
+            logger.exception(e)
+            logger.warning(f'failed to load tokens for {self.__repr__()}')
+            return []
+
+
+class AaveMarketV3(AaveMarketBase):
+    @a_sync.a_sync(ram_cache_maxsize=256)
+    async def underlying(self, token_address: AddressOrContract) -> ERC20:
+        underlying = await raw_call(token_address, 'UNDERLYING_ASSET_ADDRESS()',output='address', sync=False)
+        logger.debug(f"underlying: {underlying}")
+        return ERC20(underlying, asynchronous=self.asynchronous)
+
+    @a_sync.aka.cached_property
+    async def atokens(self) -> List[ERC20]:
+        reserves = await Call(self.address, ['getReservesList()(address[])'], [[self.address,None]]).coroutine()
+        reserves = reserves[self.address]
+        reserves_data = await asyncio.gather(*[self.contract.getReserveData.coroutine(reserve) for reserve in reserves])
+
+        try:
+            atokens = [ERC20(reserve_data[8], asynchronous=self.asynchronous) for reserve_data in reserves_data]
+            logger.info(f'loaded {len(atokens)} v3 atokens for {self.__repr__()}')
+            return atokens
+        except TypeError as e: # TODO figure out what to do about non verified aave markets
+            logger.exception(e)
             logger.warning(f'failed to load tokens for {self.__repr__()}')
             return []
 
 
 class AaveRegistry(a_sync.ASyncGenericSingleton):
     def __init__(self, asynchronous: bool = False) -> None:
         self.asynchronous = asynchronous
 
     @a_sync.aka.cached_property
     async def pools(self) -> List[Union[AaveMarketV1, AaveMarketV2]]:
-        v1, v2 = await asyncio.gather(self.__pools_v1__(sync=False), self.__pools_v2__(sync=False))
-        return v1 + v2
+        v1, v2, v3 = await asyncio.gather(
+            self.__pools_v1__(sync=False),
+            self.__pools_v2__(sync=False), 
+            self.__pools_v3__(sync=False),
+        )
+        return v1 + v2 + v3
     
     @a_sync.aka.cached_property
     async def pools_v1(self) -> List[AaveMarketV1]:
         return [AaveMarketV1(pool, asynchronous=self.asynchronous) for pool in v1_pools]
     
     @a_sync.aka.cached_property
     async def pools_v2(self) -> List[AaveMarketV2]:
         return [AaveMarketV2(pool, asynchronous=self.asynchronous) for pool in v2_pools]
     
+    @a_sync.aka.cached_property
+    async def pools_v3(self) -> List[AaveMarketV2]:
+        return [AaveMarketV3(pool, asynchronous=self.asynchronous) for pool in v3_pools]
+    
     async def pool_for_atoken(self, token_address: AnyAddressType) -> Optional[Union[AaveMarketV1, AaveMarketV2]]:
         pools = await self.__pools__(sync=False)
         for pool in pools:
             if await pool.contains(token_address, sync=False):
                 return pool
 
     def __contains__(self, __o: object) -> bool:
```

### Comparing `ypricemagic-2.3.8/y/prices/lending/compound.py` & `ypricemagic-2.4.0/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/lending/ib.py` & `ypricemagic-2.4.0/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/magic.py` & `ypricemagic-2.4.0/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/one_to_one.py` & `ypricemagic-2.4.0/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/popsicle.py` & `ypricemagic-2.4.0/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/stable_swap/belt.py` & `ypricemagic-2.4.0/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/stable_swap/curve.py` & `ypricemagic-2.4.0/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.4.0/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/stable_swap/froyo.py` & `ypricemagic-2.4.0/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.4.0/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/stable_swap/saddle.py` & `ypricemagic-2.4.0/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/synthetix.py` & `ypricemagic-2.4.0/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.4.0/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.4.0/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.4.0/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.4.0/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/utils/buckets.py` & `ypricemagic-2.4.0/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/utils/sense_check.py` & `ypricemagic-2.4.0/y/prices/utils/sense_check.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/utils/ypriceapi.py` & `ypricemagic-2.4.0/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/prices/yearn.py` & `ypricemagic-2.4.0/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/time.py` & `ypricemagic-2.4.0/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/utils/client.py` & `ypricemagic-2.4.0/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/utils/events.py` & `ypricemagic-2.4.0/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/utils/fakes.py` & `ypricemagic-2.4.0/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/utils/logging.py` & `ypricemagic-2.4.0/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/utils/middleware.py` & `ypricemagic-2.4.0/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/utils/multicall.py` & `ypricemagic-2.4.0/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/y/utils/raw_calls.py` & `ypricemagic-2.4.0/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/ypricemagic/magic.py` & `ypricemagic-2.4.0/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.8/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.4.0/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

