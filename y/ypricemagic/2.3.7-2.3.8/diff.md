# Comparing `tmp/ypricemagic-2.3.7.tar.gz` & `tmp/ypricemagic-2.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ypricemagic-2.3.7.tar", last modified: Tue Jun 20 14:03:21 2023, max compression
+gzip compressed data, was "ypricemagic-2.3.8.tar", last modified: Thu Jun 22 00:01:41 2023, max compression
```

## Comparing `ypricemagic-2.3.7.tar` & `ypricemagic-2.3.8.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.env.sample
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.803879 ypricemagic-2.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/classes/
--rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/classes/test_erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/classes/test_singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/dex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/dex/test_balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/dex/test_uniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/lending/test_aave.py
--rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/lending/test_compound.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/stable_swap/test_curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_gearbox.py
--rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_magic.py
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_popsicle.py
--rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_synthetix.py
--rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/test_yearn.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/tokenized_fund/test_piedao.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/tests/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/prices/utils/test_buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/
--rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/classes/common.py
--rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/classes/singleton.py
--rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    20385 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/contracts.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/erc20.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/ERC20.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/balancer/WeightedPool.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/balancer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/compound/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/compound/unitroller.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.807879 ypricemagic-2.3.7/y/interfaces/curve/
--rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/curve/CurveRegistry.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/curve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/multicall2.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/interfaces/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/uniswap/factoryv2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/interfaces/uniswap/quoterv3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/band.py
--rw-r--r--   0 runner    (1001) docker     (122)    19868 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/chainlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/convex.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/dex/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/dex/balancer/
--rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/balancer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/balancer/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/genericamm.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/mooniswap.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/dex/uniswap/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/uniswap.py
--rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v1.py
--rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v2.py
--rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v2_forks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/dex/uniswap/v3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/eth_derivs/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/eth_derivs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/eth_derivs/creth.py
--rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/eth_derivs/wsteth.py
--rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/gearbox.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/lending/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6880 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/aave.py
--rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/compound.py
--rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/lending/ib.py
--rw-r--r--   0 runner    (1001) docker     (122)    11264 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/magic.py
--rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/one_to_one.py
--rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/popsicle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/stable_swap/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/belt.py
--rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/curve.py
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/ellipsis.py
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/froyo.py
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/mstablefeederpool.py
--rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/stable_swap/saddle.py
--rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/synthetix.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.811879 ypricemagic-2.3.7/y/prices/tokenized_fund/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/basketdao.py
--rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/gelato.py
--rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/piedao.py
--rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/tokenized_fund/tokensets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/y/prices/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/buckets.py
--rw-r--r--   0 runner    (1001) docker     (122)     8555 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/sense_check.py
--rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/utils/ypriceapi.py
--rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/prices/yearn.py
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/time.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/y/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/client.py
--rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/dank_mids.py
--rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/events.py
--rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/fakes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/middleware.py
--rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/multicall.py
--rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/y/utils/raw_calls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/ypricemagic/
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/ypricemagic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-20 14:03:11.000000 ypricemagic-2.3.7/ypricemagic/magic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 14:03:21.815879 ypricemagic-2.3.7/ypricemagic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-20 14:03:21.000000 ypricemagic-2.3.7/ypricemagic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.env.sample
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.930053 ypricemagic-2.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2467 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3229 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      632 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      139 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1061 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      776 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      840 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)     3851 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/classes/test_erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)      550 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/classes/test_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/dex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/dex/test_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2918 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/dex/test_uniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6458 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/lending/test_aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1298 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/lending/test_compound.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)      379 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/stable_swap/test_curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)      471 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_gearbox.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4496 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_popsicle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1116 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_synthetix.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1017 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/test_yearn.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)      236 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/tokenized_fund/test_piedao.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.934053 ypricemagic-2.3.8/tests/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     2025 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/prices/utils/test_buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      492 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/
+-rw-r--r--   0 runner    (1001) docker     (122)     1876 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7773 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/classes/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2406 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/classes/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10017 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20584 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (122)      493 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)      576 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3187 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/erc20.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2488 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     6400 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/ERC20.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)    23102 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/balancer/WeightedPool.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/balancer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/compound/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32517 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/compound/unitroller.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/curve/
+-rw-r--r--   0 runner    (1001) docker     (122)     7124 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/curve/CurveRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/curve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3802 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/multicall2.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/interfaces/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2248 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/uniswap/factoryv2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/interfaces/uniswap/quoterv3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3271 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2910 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/band.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19868 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/chainlink.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/convex.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/dex/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/dex/balancer/
+-rw-r--r--   0 runner    (1001) docker     (122)       64 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2905 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/balancer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6669 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10744 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/balancer/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2544 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/genericamm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2206 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/mooniswap.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/dex/uniswap/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6370 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/uniswap.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2125 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v1.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23293 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12588 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v2_forks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/dex/uniswap/v3.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/eth_derivs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/eth_derivs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/eth_derivs/creth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1272 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/eth_derivs/wsteth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2940 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/gearbox.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.938053 ypricemagic-2.3.8/y/prices/lending/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6847 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/aave.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10528 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/compound.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/lending/ib.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11264 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/magic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      815 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/one_to_one.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2490 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/popsicle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/prices/stable_swap/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1032 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/belt.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22296 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/curve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/froyo.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1098 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/mstablefeederpool.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/stable_swap/saddle.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/synthetix.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/prices/tokenized_fund/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1079 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/basketdao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1630 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/gelato.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2351 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/piedao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2257 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/tokenized_fund/tokensets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/prices/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4650 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8741 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/sense_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8174 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/utils/ypriceapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5853 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/prices/yearn.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/y/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)      864 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/dank_mids.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7970 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/events.py
+-rw-r--r--   0 runner    (1001) docker     (122)      669 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1063 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2726 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11228 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/multicall.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14776 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/y/utils/raw_calls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/ypricemagic/
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/ypricemagic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-06-22 00:01:29.000000 ypricemagic-2.3.8/ypricemagic/magic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 00:01:41.942053 ypricemagic-2.3.8/ypricemagic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      406 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3161 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      168 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-06-22 00:01:41.000000 ypricemagic-2.3.8/ypricemagic.egg-info/top_level.txt
```

### Comparing `ypricemagic-2.3.7/.github/workflows/codeql-analysis.yml` & `ypricemagic-2.3.8/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/.github/workflows/pytest.yaml` & `ypricemagic-2.3.8/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/.github/workflows/release.yaml` & `ypricemagic-2.3.8/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/LICENSE.txt` & `ypricemagic-2.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/README.md` & `ypricemagic-2.3.8/README.md`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/setup.py` & `ypricemagic-2.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/classes/test_erc20.py` & `ypricemagic-2.3.8/tests/classes/test_erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/classes/test_singleton.py` & `ypricemagic-2.3.8/tests/classes/test_singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/fixtures.py` & `ypricemagic-2.3.8/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/dex/test_uniswap.py` & `ypricemagic-2.3.8/tests/prices/dex/test_uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/lending/test_aave.py` & `ypricemagic-2.3.8/tests/prices/lending/test_aave.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/lending/test_compound.py` & `ypricemagic-2.3.8/tests/prices/lending/test_compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/test_chainlink.py` & `ypricemagic-2.3.8/tests/prices/test_chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/test_magic.py` & `ypricemagic-2.3.8/tests/prices/test_magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/test_popsicle.py` & `ypricemagic-2.3.8/tests/prices/test_popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/test_synthetix.py` & `ypricemagic-2.3.8/tests/prices/test_synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/test_yearn.py` & `ypricemagic-2.3.8/tests/prices/test_yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/tests/prices/utils/test_buckets.py` & `ypricemagic-2.3.8/tests/prices/utils/test_buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/__init__.py` & `ypricemagic-2.3.8/y/__init__.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/classes/common.py` & `ypricemagic-2.3.8/y/classes/common.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/classes/singleton.py` & `ypricemagic-2.3.8/y/classes/singleton.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/constants.py` & `ypricemagic-2.3.8/y/constants.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/contracts.py` & `ypricemagic-2.3.8/y/contracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -265,15 +265,18 @@
                 return await asyncio.get_event_loop().run_in_executor(contract_threads, Contract, address)
     
     def __init_from_abi__(self, build: Dict, owner: Optional[AccountsType] = None, persist: bool = True) -> None:
         _ContractBase.__init__(self, None, build, {})  # type: ignore
         _DeployedContractBase.__init__(self, build['address'], owner, None)
         if persist:
             _add_deployment(self)
-        self.verified = True
+        try:
+            self.verified = True
+        except AttributeError:
+            logger.warning(f'`Contract("{address}").verified` property will not be usable due to the contract having a `verified` method in its ABI.')
         return self
 
     def has_method(self, method: str, return_response: bool = False) -> Union[bool,Any]:
         return has_method(self.address, method, return_response=return_response, sync=False)
 
     async def has_methods(
         self,
```

### Comparing `ypricemagic-2.3.7/y/datatypes.py` & `ypricemagic-2.3.8/y/datatypes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/decorators.py` & `ypricemagic-2.3.8/y/decorators.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/erc20.py` & `ypricemagic-2.3.8/y/erc20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/exceptions.py` & `ypricemagic-2.3.8/y/exceptions.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/interfaces/ERC20.py` & `ypricemagic-2.3.8/y/interfaces/ERC20.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/interfaces/balancer/WeightedPool.py` & `ypricemagic-2.3.8/y/interfaces/balancer/WeightedPool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/interfaces/compound/unitroller.py` & `ypricemagic-2.3.8/y/interfaces/compound/unitroller.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/interfaces/curve/CurveRegistry.py` & `ypricemagic-2.3.8/y/interfaces/curve/CurveRegistry.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/interfaces/multicall2.py` & `ypricemagic-2.3.8/y/interfaces/multicall2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/interfaces/uniswap/factoryv2.py` & `ypricemagic-2.3.8/y/interfaces/uniswap/factoryv2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/interfaces/uniswap/quoterv3.py` & `ypricemagic-2.3.8/y/interfaces/uniswap/quoterv3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/networks.py` & `ypricemagic-2.3.8/y/networks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/band.py` & `ypricemagic-2.3.8/y/prices/band.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/chainlink.py` & `ypricemagic-2.3.8/y/prices/chainlink.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/convex.py` & `ypricemagic-2.3.8/y/prices/convex.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/balancer/balancer.py` & `ypricemagic-2.3.8/y/prices/dex/balancer/balancer.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/balancer/v1.py` & `ypricemagic-2.3.8/y/prices/dex/balancer/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/balancer/v2.py` & `ypricemagic-2.3.8/y/prices/dex/balancer/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/genericamm.py` & `ypricemagic-2.3.8/y/prices/dex/genericamm.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/mooniswap.py` & `ypricemagic-2.3.8/y/prices/dex/mooniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/uniswap/uniswap.py` & `ypricemagic-2.3.8/y/prices/dex/uniswap/uniswap.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/uniswap/v1.py` & `ypricemagic-2.3.8/y/prices/dex/uniswap/v1.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/uniswap/v2.py` & `ypricemagic-2.3.8/y/prices/dex/uniswap/v2.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/uniswap/v2_forks.py` & `ypricemagic-2.3.8/y/prices/dex/uniswap/v2_forks.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/dex/uniswap/v3.py` & `ypricemagic-2.3.8/y/prices/dex/uniswap/v3.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/eth_derivs/creth.py` & `ypricemagic-2.3.8/y/prices/eth_derivs/creth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/eth_derivs/wsteth.py` & `ypricemagic-2.3.8/y/prices/eth_derivs/wsteth.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/gearbox.py` & `ypricemagic-2.3.8/y/prices/gearbox.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/lending/aave.py` & `ypricemagic-2.3.8/y/prices/lending/aave.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     @a_sync.a_sync(cache_type='memory')
     async def is_atoken(self, token_address: AnyAddressType) -> bool:
         return any(await asyncio.gather(*[pool.contains(token_address, sync=False) for pool in await self.__pools__(sync=False)]))
     
     async def is_wrapped_atoken(self, token_address: AnyAddressType) -> bool:
         try:
             contract = await Contract.coroutine(token_address)
-            attrs = "ATOKEN", "STATIC_ATOKEN_LM_REVISION", "staticToDynamicAmount"
+            attrs = "ATOKEN", "AAVE_POOL", "UNDERLYING"
             return all(hasattr(contract, attr) for attr in attrs)
         except ContractNotVerified:
             return False
     
     @a_sync.a_sync(cache_type='memory')
     async def underlying(self, token_address: AddressOrContract) -> ERC20:
         pool: Union[AaveMarketV1, AaveMarketV2] = await self.pool_for_atoken(token_address, sync=False)
@@ -143,14 +143,14 @@
         underlying = await self.underlying(token_address, sync=False)
         return await underlying.price(block, sync=False)
     
     async def get_price_wrapped(self, token_address: AddressOrContract, block: Optional[Block] = None) -> UsdPrice:
         contract, scale = await asyncio.gather(Contract.coroutine(token_address), ERC20(token_address, asynchronous=True).scale)
         underlying, price_per_share = await asyncio.gather(
             contract.ATOKEN.coroutine(block_identifier=block),
-            contract.staticToDynamicAmount.coroutine(scale, block_identifier=block),
+            contract.convertToAssets.coroutine(scale, block_identifier=block),
         )
         price_per_share /= scale
         return price_per_share * await ERC20(underlying, asynchronous=True).price(block)
 
 
 aave = AaveRegistry(asynchronous=True)
```

### Comparing `ypricemagic-2.3.7/y/prices/lending/compound.py` & `ypricemagic-2.3.8/y/prices/lending/compound.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/lending/ib.py` & `ypricemagic-2.3.8/y/prices/lending/ib.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/magic.py` & `ypricemagic-2.3.8/y/prices/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/one_to_one.py` & `ypricemagic-2.3.8/y/prices/one_to_one.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/popsicle.py` & `ypricemagic-2.3.8/y/prices/popsicle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/stable_swap/belt.py` & `ypricemagic-2.3.8/y/prices/stable_swap/belt.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/stable_swap/curve.py` & `ypricemagic-2.3.8/y/prices/stable_swap/curve.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/stable_swap/ellipsis.py` & `ypricemagic-2.3.8/y/prices/stable_swap/ellipsis.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/stable_swap/froyo.py` & `ypricemagic-2.3.8/y/prices/stable_swap/froyo.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/stable_swap/mstablefeederpool.py` & `ypricemagic-2.3.8/y/prices/stable_swap/mstablefeederpool.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/stable_swap/saddle.py` & `ypricemagic-2.3.8/y/prices/stable_swap/saddle.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/synthetix.py` & `ypricemagic-2.3.8/y/prices/synthetix.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/tokenized_fund/basketdao.py` & `ypricemagic-2.3.8/y/prices/tokenized_fund/basketdao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/tokenized_fund/gelato.py` & `ypricemagic-2.3.8/y/prices/tokenized_fund/gelato.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/tokenized_fund/piedao.py` & `ypricemagic-2.3.8/y/prices/tokenized_fund/piedao.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/tokenized_fund/tokensets.py` & `ypricemagic-2.3.8/y/prices/tokenized_fund/tokensets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/utils/buckets.py` & `ypricemagic-2.3.8/y/prices/utils/buckets.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/utils/sense_check.py` & `ypricemagic-2.3.8/y/prices/utils/sense_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,17 @@
         "0x5e74C9036fb86BD7eCdcb084a0673EFc32eA31cb", # sETH
         "0xae78736Cd615f374D3085123A210448E74Fc6393", # rETH
         "0xE95A203B1a91a908F9B9CE46459d101078c2c3cb", # aETHc
         "0xae7ab96520DE3A18E5e111B5EaAb095312D7fE84", # stETH
         "0x9559Aaa82d9649C7A7b220E7c461d2E74c9a3593", # rETH
         "0x836A808d4828586A69364065A1e064609F5078c7", # pETH
         "0xc3D088842DcF02C13699F936BB83DFBBc6f721Ab", # vETH
+        "0xC1330aCBbcE97cb9695B7ee161c0F95B875a8b0F", # onETH
+        "0x5E8422345238F34275888049021821E8E08CAa1f", # fxsETH
+        "0x856c4Efb76C1D1AE02e20CEB03A2A6a08b0b8dC3", # OETH
         # btc and btc-like
         "0xEB4C2781e4ebA804CE9a9803C67d0893436bB27D", # renbtc
         "0xfE18be6b3Bd88A2D2A7f928d00292E7a9963CfC6", # sbtc
         "0x49849C98ae39Fff122806C06791Fa73784FB3675", # crvrenwbtc
         "0x075b1bb99792c9E1041bA13afEf80C91a1e70fB3", # crvrenwsbtc
         "0xb19059ebb43466C323583928285a49f558E572Fd", # hcrv
         "0x64eda51d3Ad40D56b9dFc5554E06F94e1Dd786Fd", # tbtc/sbtcCrv
```

### Comparing `ypricemagic-2.3.7/y/prices/utils/ypriceapi.py` & `ypricemagic-2.3.8/y/prices/utils/ypriceapi.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/prices/yearn.py` & `ypricemagic-2.3.8/y/prices/yearn.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/time.py` & `ypricemagic-2.3.8/y/time.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/utils/client.py` & `ypricemagic-2.3.8/y/utils/client.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/utils/events.py` & `ypricemagic-2.3.8/y/utils/events.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/utils/fakes.py` & `ypricemagic-2.3.8/y/utils/fakes.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/utils/logging.py` & `ypricemagic-2.3.8/y/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/utils/middleware.py` & `ypricemagic-2.3.8/y/utils/middleware.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/utils/multicall.py` & `ypricemagic-2.3.8/y/utils/multicall.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/y/utils/raw_calls.py` & `ypricemagic-2.3.8/y/utils/raw_calls.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/ypricemagic/magic.py` & `ypricemagic-2.3.8/ypricemagic/magic.py`

 * *Files identical despite different names*

### Comparing `ypricemagic-2.3.7/ypricemagic.egg-info/SOURCES.txt` & `ypricemagic-2.3.8/ypricemagic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

