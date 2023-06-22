# Comparing `tmp/cardano-clusterlib-0.4.9.tar.gz` & `tmp/cardano-clusterlib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.4.9.tar", last modified: Fri May 12 06:59:22 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.5.0.tar", last modified: Thu Jun 22 11:55:32 2023, max compression
```

## Comparing `cardano-clusterlib-0.4.9.tar` & `cardano-clusterlib-0.5.0.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.564756 cardano-clusterlib-0.4.9/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.557756 cardano-clusterlib-0.4.9/.github/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.559756 cardano-clusterlib-0.4.9/.github/workflows/
--rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.9/.github/workflows/repo_lint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.9/.gitignore
--rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.9/.markdownlint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     1224 2023-05-06 20:29:59.000000 cardano-clusterlib-0.4.9/.pre-commit-config.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.9/.pylintrc
--rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.9/.readthedocs.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.9/CODE-OF-CONDUCT.md
--rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.9/LICENSE
--rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.9/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-12 06:59:22.564756 cardano-clusterlib-0.4.9/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.9/README.md
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.561756 cardano-clusterlib-0.4.9/cardano_clusterlib/
--rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/__init__.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8119 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/address_group.py
--rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)    15619 2023-05-12 06:58:23.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/consts.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/coverage.py
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/exceptions.py
--rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/governance_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/key_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/node_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/py.typed
--rw-r--r--   0 martink   (1000) martink   (1000)    18252 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/query_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6849 2023-04-17 13:43:55.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/structs.py
--rw-r--r--   0 martink   (1000) martink   (1000)    63362 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/txtools.py
--rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/types.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.562756 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 martink   (1000) martink   (1000)       15 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/requires.txt
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.562756 cardano-clusterlib-0.4.9/docs/
--rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.9/docs/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.9/docs/requirements.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.563756 cardano-clusterlib-0.4.9/docs/source/
--rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.9/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.9/docs/source/conf.py
--rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.9/docs/source/index.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.9/docs/source/modules.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.9/docs/source/readme.rst
--rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.9/mypy.ini
--rw-r--r--   0 martink   (1000) martink   (1000)      610 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.9/pyproject.toml
--rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.9/requirements-dev.txt
--rw-r--r--   0 martink   (1000) martink   (1000)      776 2023-05-12 06:59:22.564756 cardano-clusterlib-0.4.9/setup.cfg
--rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.9/setup.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.563756 cardano-clusterlib-0.4.9/upgrading/
--rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.9/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.012097 cardano-clusterlib-0.5.0/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.007097 cardano-clusterlib-0.5.0/.github/
+-rw-r--r--   0 martink   (1000) martink   (1000)      214 2023-06-22 11:16:14.000000 cardano-clusterlib-0.5.0/.github/dependabot.yml
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.007097 cardano-clusterlib-0.5.0/.github/workflows/
+-rw-r--r--   0 martink   (1000) martink   (1000)      353 2023-06-22 11:16:45.000000 cardano-clusterlib-0.5.0/.github/workflows/repo_lint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.5.0/.gitignore
+-rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.5.0/.markdownlint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     1224 2023-05-06 20:29:59.000000 cardano-clusterlib-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.5.0/.pylintrc
+-rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.5.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.5.0/LICENSE
+-rw-r--r--   0 martink   (1000) martink   (1000)     1297 2023-06-22 11:53:24.000000 cardano-clusterlib-0.5.0/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)     8219 2023-06-22 11:55:32.012097 cardano-clusterlib-0.5.0/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.5.0/README.md
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.010097 cardano-clusterlib-0.5.0/cardano_clusterlib/
+-rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/__init__.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8119 2023-04-17 08:42:14.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/address_group.py
+-rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    15509 2023-06-22 11:01:23.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/consts.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/coverage.py
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     4327 2023-05-15 15:10:04.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/key_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/node_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/py.typed
+-rw-r--r--   0 martink   (1000) martink   (1000)    18553 2023-06-22 11:01:23.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/query_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7870 2023-06-13 13:56:12.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/structs.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    63703 2023-06-22 11:01:23.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    44818 2023-06-13 13:56:12.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/txtools.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.5.0/cardano_clusterlib/types.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.011097 cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/
+-rw-r--r--   0 martink   (1000) martink   (1000)     8219 2023-06-22 11:55:31.000000 cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     1406 2023-06-22 11:55:32.000000 cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-06-22 11:55:31.000000 cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 martink   (1000) martink   (1000)       15 2023-06-22 11:55:31.000000 cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/requires.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-06-22 11:55:31.000000 cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.011097 cardano-clusterlib-0.5.0/docs/
+-rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.5.0/docs/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.011097 cardano-clusterlib-0.5.0/docs/source/
+-rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.5.0/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.5.0/docs/source/conf.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.5.0/docs/source/index.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.5.0/docs/source/modules.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.5.0/docs/source/readme.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.5.0/mypy.ini
+-rw-r--r--   0 martink   (1000) martink   (1000)     1531 2023-06-22 11:53:24.000000 cardano-clusterlib-0.5.0/pyproject.toml
+-rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.5.0/requirements-dev.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)      352 2023-06-22 11:55:32.012097 cardano-clusterlib-0.5.0/setup.cfg
+-rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.5.0/setup.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-06-22 11:55:32.011097 cardano-clusterlib-0.5.0/upgrading/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.5.0/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.4.9/.gitignore` & `cardano-clusterlib-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/.markdownlint.yaml` & `cardano-clusterlib-0.5.0/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/.pre-commit-config.yaml` & `cardano-clusterlib-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/.pylintrc` & `cardano-clusterlib-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.5.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/LICENSE` & `cardano-clusterlib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/Makefile` & `cardano-clusterlib-0.5.0/Makefile`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 lint:
 	pre-commit run -a
 	if type pytype >/dev/null 2>&1; then pytype cardano_clusterlib; fi
 
 # build package
 .PHONY: build
 build:
-	python3 -m pip install --upgrade build
+	python -c "import build" || python3 -m pip install build
 	python3 -m build
 
 # upload package to PyPI
 .PHONY: upload
 upload:
 	if ! type twine >/dev/null 2>&1; then python3 -m pip install --upgrade twine; fi
 	twine upload --skip-existing dist/*
```

### Comparing `cardano-clusterlib-0.4.9/PKG-INFO` & `cardano-clusterlib-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
+Author-email: Martin Kourim <martin.kourim@iohk.io>
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
+License: Apache License 2.0
+Project-URL: homepage, https://github.com/input-output-hk/cardano-clusterlib-py
+Project-URL: documentation, https://cardano-clusterlib-py.readthedocs.io/
+Project-URL: repository, https://github.com/input-output-hk/cardano-clusterlib-py
+Keywords: cardano,cardano-node,cardano-cli,cardano-node-tests
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # README for cardano-clusterlib
 
 [![Documentation Status](https://readthedocs.org/projects/cardano-clusterlib-py/badge/?version=latest)](https://cardano-clusterlib-py.readthedocs.io/en/latest/?badge=latest)
 [![PyPi Version](https://img.shields.io/pypi/v/cardano-clusterlib.svg)](https://pypi.org/project/cardano-clusterlib/)
```

### Comparing `cardano-clusterlib-0.4.9/README.md` & `cardano-clusterlib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/clusterlib_helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/clusterlib_klass.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,17 +87,14 @@
         self.slots_offset = slots_offset or consts.SLOTS_OFFSETS.get(self.network_magic) or 0
         self.ttl_length = 1000
         # TODO: proper calculation based on `utxoCostPerWord` needed
         self._min_change_value = 1800_000
 
         self.tx_era = tx_era
 
-        # TODO: add temporary switch for CDDL format, until it is made default
-        self.use_cddl = False
-
         self.overwrite_outfiles = True
 
         # groups of commands
         self._transaction_group: Optional[transaction_group.TransactionGroup] = None
         self._query_group: Optional[query_group.QueryGroup] = None
         self._address_group: Optional[address_group.AddressGroup] = None
         self._stake_address_group: Optional[stake_address_group.StakeAddressGroup] = None
```

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/genesis_group.py`

 * *Files 9% similar despite different names*

```diff
@@ -101,9 +101,29 @@
                 str(out_file),
             ]
         )
 
         helpers._check_outfiles(out_file)
         return helpers.read_address_from_file(out_file)
 
+    def get_genesis_vkey_hash(self, vkey_file: FileType) -> str:
+        """Return the hash of a genesis public key.
+
+        Args:
+            vkey_file: A path to corresponding vkey file.
+
+        Returns:
+            str: A generated key-hash.
+        """
+        cli_out = self._clusterlib_obj.cli(
+            [
+                "genesis",
+                "key-hash",
+                "--verification-key-file",
+                str(vkey_file),
+            ]
+        )
+
+        return cli_out.stdout.rstrip().decode("ascii")
+
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: clusterlib_obj={id(self._clusterlib_obj)}>"
```

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/query_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -483,9 +483,17 @@
             dict: A dictionary containing mempool information.
         """
         tx_mempool: Dict[str, Any] = json.loads(
             self.query_cli(["tx-mempool"], cli_sub_args=[consts.SUBCOMMAND_MARK, "tx-exists", txid])
         )
         return tx_mempool
 
+    def get_slot_number(self, timestamp: datetime.datetime) -> int:
+        """Return slot number for UTC timestamp."""
+        timestamp_str = timestamp.strftime("%Y-%m-%dT%H:%M:%SZ")
+
+        slot_number: int = json.loads(self.query_cli(["slot-number", timestamp_str]))
+
+        return slot_number
+
     def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: clusterlib_obj={id(self._clusterlib_obj)}>"
```

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/stake_address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/structs.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,36 +178,38 @@
     pool_metadata_hash: str = ""
     pool_relay_dns: str = ""
     pool_relay_ipv4: str = ""
     pool_relay_port: int = 0
 
 
 class TxRawOutput(NamedTuple):
-    txins: List[UTXOData]
-    txouts: List[TxOut]
-    txouts_count: int
-    tx_files: TxFiles
-    out_file: Path
-    fee: int
-    build_args: List[str]
-    era: str = ""
-    script_txins: OptionalScriptTxIn = ()
-    script_withdrawals: OptionalScriptWithdrawals = ()
-    complex_certs: OptionalScriptCerts = ()
-    mint: OptionalMint = ()
-    invalid_hereafter: Optional[int] = None
-    invalid_before: Optional[int] = None
-    withdrawals: OptionalTxOuts = ()
-    change_address: str = ""
-    return_collateral_txouts: OptionalTxOuts = ()
-    total_collateral_amount: Optional[int] = None
-    readonly_reference_txins: OptionalUTXOData = ()
-    script_valid: bool = True
-    required_signers: OptionalFiles = ()
-    required_signer_hashes: Optional[List[str]] = None
+    txins: List[UTXOData]  # UTXOs used as inputs
+    txouts: List[TxOut]  # Tx outputs
+    txouts_count: int  # Final number of tx outputs after adding change address and joining outputs
+    tx_files: TxFiles  # Files needed for transaction building (certificates, signing keys, etc.)
+    out_file: Path  # Output file path for the transaction body
+    fee: int  # Tx fee
+    build_args: List[str]  # Arguments that were passed to `cardano-cli transaction build*`
+    era: str = ""  # Era used for the transaction
+    script_txins: OptionalScriptTxIn = ()  # Tx inputs that are combined with scripts
+    script_withdrawals: OptionalScriptWithdrawals = ()  # Withdrawals that are combined with scripts
+    complex_certs: OptionalScriptCerts = ()  # Certificates that are combined with scripts
+    mint: OptionalMint = ()  # Minting data (Tx outputs, script, etc.)
+    invalid_hereafter: Optional[int] = None  # Validity interval upper bound
+    invalid_before: Optional[int] = None  # Validity interval lower bound
+    withdrawals: OptionalTxOuts = ()  # All withdrawals (including those combined with scripts)
+    change_address: str = ""  # Address for change
+    return_collateral_txouts: OptionalTxOuts = ()  # Tx outputs for returning collateral
+    total_collateral_amount: Optional[int] = None  # Total collateral amount
+    readonly_reference_txins: OptionalUTXOData = ()  # Tx inputs for plutus script context
+    script_valid: bool = True  # Whether the plutus script is valid
+    required_signers: OptionalFiles = ()  # Signing keys that are required for the transaction
+    # Hashes of signing keys that are required for the transaction
+    required_signer_hashes: Union[List[str], Tuple[()]] = ()
+    combined_reference_txins: OptionalUTXOData = ()  # All reference tx inputs
 
 
 class PoolCreationOutput(NamedTuple):
     stake_pool_id: str
     vrf_key_pair: KeyPair
     cold_key_pair: ColdKeyPair
     pool_reg_cert_file: Path
```

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/transaction_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,16 +270,14 @@
                     str(self._clusterlib_obj.pparams_file),
                 ]
             )
 
         if total_collateral_amount:
             misc_args.extend(["--tx-total-collateral", str(total_collateral_amount)])
 
-        misc_args.extend(["--cddl-format"] if self._clusterlib_obj.use_cddl else [])
-
         if tx_files.metadata_json_files and tx_files.metadata_json_detailed_schema:
             misc_args.append("--json-metadata-detailed-schema")
 
         cli_args = [
             "transaction",
             "build-raw",
             "--fee",
@@ -322,14 +320,21 @@
             withdrawals=withdrawals,
             return_collateral_txouts=return_collateral_txouts,
             total_collateral_amount=total_collateral_amount,
             readonly_reference_txins=readonly_reference_txins,
             script_valid=script_valid,
             required_signers=required_signers,
             required_signer_hashes=required_signer_hashes,
+            combined_reference_txins=txtools._get_reference_txins(
+                readonly_reference_txins=readonly_reference_txins,
+                script_txins=script_txins,
+                mint=mint,
+                complex_certs=complex_certs,
+                script_withdrawals=script_withdrawals,
+            ),
         )
 
     def build_raw_tx(
         self,
         src_address: str,
         tx_name: str,
         txins: structs.OptionalUTXOData = (),
@@ -824,38 +829,22 @@
             script_txins=script_txins,
             mint=mint,
             complex_certs=complex_certs,
             script_withdrawals=collected_data.script_withdrawals,
             for_build=True,
         )
 
-        grouped_args_str = " ".join(grouped_args)
-        pparams_for_txins = grouped_args and (
-            "-datum-" in grouped_args_str or "-redeemer-" in grouped_args_str
-        )
-        # TODO: see https://github.com/input-output-hk/cardano-node/issues/4058
-        pparams_for_txouts = "-embed-" in " ".join(txout_args)
-        if pparams_for_txins or pparams_for_txouts:
-            grouped_args.extend(
-                [
-                    "--protocol-params-file",
-                    str(self._clusterlib_obj.pparams_file),
-                ]
-            )
-
         misc_args.extend(["--change-address", change_address])
 
         if witness_override is not None:
             misc_args.extend(["--witness-override", str(witness_override)])
 
         if total_collateral_amount:
             misc_args.extend(["--tx-total-collateral", str(total_collateral_amount)])
 
-        misc_args.extend(["--cddl-format"] if self._clusterlib_obj.use_cddl else [])
-
         if calc_script_cost_file:
             misc_args.extend(["--calculate-plutus-script-cost", str(calc_script_cost_file)])
             out_file = Path(calc_script_cost_file)
         else:
             misc_args.extend(["--out-file", str(out_file)])
 
         if tx_files.metadata_json_files and tx_files.metadata_json_detailed_schema:
@@ -909,14 +898,21 @@
             change_address=change_address or src_address,
             return_collateral_txouts=return_collateral_txouts,
             total_collateral_amount=total_collateral_amount,
             readonly_reference_txins=readonly_reference_txins,
             script_valid=script_valid,
             required_signers=required_signers,
             required_signer_hashes=required_signer_hashes,
+            combined_reference_txins=txtools._get_reference_txins(
+                readonly_reference_txins=readonly_reference_txins,
+                script_txins=script_txins,
+                mint=mint,
+                complex_certs=complex_certs,
+                script_withdrawals=script_withdrawals,
+            ),
         )
 
     def sign_tx(
         self,
         signing_key_files: OptionalFiles,
         tx_name: str,
         tx_body_file: Optional[FileType] = None,
@@ -1061,46 +1057,48 @@
 
         Args:
             tx_file: A path to signed transaction file.
             txins: An iterable of `structs.UTXOData`, specifying input UTxOs.
             wait_blocks: A number of new blocks to wait for (default = 2).
         """
         txid = ""
-        for r in range(5):
+        for r in range(20):
             err = None
 
             if r == 0:
                 self.submit_tx_bare(tx_file)
             else:
                 txid = txid or self.get_txid(tx_file=tx_file)
                 LOGGER.info(f"Resubmitting transaction '{txid}' (from '{tx_file}').")
                 try:
                     self.submit_tx_bare(tx_file)
                 except exceptions.CLIError as exc:
-                    # check if resubmitting failed because an input UTxO was already spent
+                    # Check if resubmitting failed because an input UTxO was already spent
                     if "(BadInputsUTxO" not in str(exc):
                         raise
                     err = exc
+                    # If here, the TX is likely still in mempool and we need to wait
 
-            # wait for new blocks even in case of error, so `query utxo` returns up-to-date data
             self._clusterlib_obj.wait_for_new_block(wait_blocks)
 
             # Check that one of the input UTxOs can no longer be queried in order to verify
             # the TX was successfully submitted to the chain (that the TX is no longer in mempool).
             # An input is spent when its combination of hash and ix is not found in the list
             # of current UTxOs.
             # TODO: check that the transaction is 1-block deep (can't be done in CLI alone)
             utxo_data = self._clusterlib_obj.g_query.get_utxo(utxo=txins[0])
             if not utxo_data:
                 break
         else:
             if err is not None:
                 # Submitting the TX raised an exception as if the input was already
-                # spent, but it was not the case. Re-raising the exception.
-                raise err
+                # spent, but it was either not the case, or the TX is still in mempool.
+                raise exceptions.CLIError(
+                    f"Failed to resubmit the transaction '{txid}' (from '{tx_file}')."
+                ) from err
 
             raise exceptions.CLIError(
                 f"Transaction '{txid}' didn't make it to the chain (from '{tx_file}')."
             )
 
     def send_tx(
         self,
@@ -1113,14 +1111,15 @@
         return_collateral_txouts: structs.OptionalTxOuts = (),
         total_collateral_amount: Optional[int] = None,
         mint: structs.OptionalMint = (),
         tx_files: Optional[structs.TxFiles] = None,
         complex_certs: structs.OptionalScriptCerts = (),
         fee: Optional[int] = None,
         required_signers: OptionalFiles = (),
+        required_signer_hashes: Optional[List[str]] = None,
         ttl: Optional[int] = None,
         withdrawals: structs.OptionalTxOuts = (),
         script_withdrawals: structs.OptionalScriptWithdrawals = (),
         deposit: Optional[int] = None,
         invalid_hereafter: Optional[int] = None,
         invalid_before: Optional[int] = None,
         witness_count_add: int = 0,
@@ -1153,14 +1152,16 @@
             tx_files: A `structs.TxFiles` tuple containing files needed for the transaction
                 (optional).
             complex_certs: An iterable of `ComplexCert`, specifying certificates script data
                 (optional).
             fee: A fee amount (optional).
             required_signers: An iterable of filepaths of the signing keys whose signatures
                 are required (optional).
+            required_signer_hashes: A list of hashes of the signing keys whose signatures
+                are required (optional).
             ttl: A last block when the transaction is still valid
                 (deprecated in favor of `invalid_hereafter`, optional).
             withdrawals: A list (iterable) of `TxOuts`, specifying reward withdrawals (optional).
             script_withdrawals: An iterable of `ScriptWithdrawal`, specifying withdrawal script
                 data (optional).
             deposit: A deposit amount needed by the transaction (optional).
             invalid_hereafter: A last block when the transaction is still valid (optional).
@@ -1198,14 +1199,15 @@
                 script_txins=script_txins,
                 return_collateral_txouts=return_collateral_txouts,
                 total_collateral_amount=total_collateral_amount,
                 mint=mint,
                 tx_files=tx_files,
                 complex_certs=complex_certs,
                 required_signers=required_signers,
+                required_signer_hashes=required_signer_hashes,
                 withdrawals=withdrawals,
                 script_withdrawals=script_withdrawals,
                 invalid_hereafter=invalid_hereafter or ttl,
                 witness_count_add=witness_count_add,
                 join_txouts=join_txouts,
                 destination_dir=destination_dir,
             )
@@ -1224,14 +1226,15 @@
             return_collateral_txouts=return_collateral_txouts,
             total_collateral_amount=total_collateral_amount,
             mint=mint,
             tx_files=tx_files,
             complex_certs=complex_certs,
             fee=fee,
             required_signers=required_signers,
+            required_signer_hashes=required_signer_hashes,
             withdrawals=withdrawals,
             script_withdrawals=script_withdrawals,
             deposit=deposit,
             invalid_hereafter=invalid_hereafter or ttl,
             invalid_before=invalid_before,
             join_txouts=join_txouts,
             destination_dir=destination_dir,
```

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/txtools.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,36 @@
         )
         for s in script_withdrawals
     ]
     withdrawals_txouts = [*withdrawals, *[s.txout for s in script_withdrawals]]
     return withdrawals, script_withdrawals, withdrawals_txouts
 
 
+def _get_reference_txins(
+    readonly_reference_txins: structs.OptionalUTXOData,
+    script_txins: structs.OptionalScriptTxIn,
+    mint: structs.OptionalMint,
+    complex_certs: structs.OptionalScriptCerts,
+    script_withdrawals: structs.OptionalScriptWithdrawals,
+) -> List[structs.UTXOData]:
+    """Get list of reference txins."""
+    script_ref_txins = [
+        r.reference_txin
+        for r in (
+            *script_txins,
+            *mint,
+            *complex_certs,
+            *script_withdrawals,
+        )
+        if r.reference_txin
+    ]
+
+    return [*readonly_reference_txins, *script_ref_txins]
+
+
 def _get_txin_strings(
     txins: structs.OptionalUTXOData, script_txins: structs.OptionalScriptTxIn
 ) -> Set[str]:
     """Get list of txin strings for normal (non-script) inputs."""
     # filter out duplicate txins
     txins_utxos = {f"{x.utxo_hash}#{x.utxo_ix}" for x in txins}
```

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib/types.py` & `cardano-clusterlib-0.5.0/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.9
+Version: 0.5.0
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
+Author-email: Martin Kourim <martin.kourim@iohk.io>
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
+License: Apache License 2.0
+Project-URL: homepage, https://github.com/input-output-hk/cardano-clusterlib-py
+Project-URL: documentation, https://cardano-clusterlib-py.readthedocs.io/
+Project-URL: repository, https://github.com/input-output-hk/cardano-clusterlib-py
+Keywords: cardano,cardano-node,cardano-cli,cardano-node-tests
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # README for cardano-clusterlib
 
 [![Documentation Status](https://readthedocs.org/projects/cardano-clusterlib-py/badge/?version=latest)](https://cardano-clusterlib-py.readthedocs.io/en/latest/?badge=latest)
 [![PyPi Version](https://img.shields.io/pypi/v/cardano-clusterlib.svg)](https://pypi.org/project/cardano-clusterlib/)
```

### Comparing `cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.5.0/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Makefile
 README.md
 mypy.ini
 pyproject.toml
 requirements-dev.txt
 setup.cfg
 setup.py
+.github/dependabot.yml
 .github/workflows/repo_lint.yaml
 cardano_clusterlib/__init__.py
 cardano_clusterlib/address_group.py
 cardano_clusterlib/clusterlib.py
 cardano_clusterlib/clusterlib_helpers.py
 cardano_clusterlib/clusterlib_klass.py
 cardano_clusterlib/consts.py
```

### Comparing `cardano-clusterlib-0.4.9/docs/Makefile` & `cardano-clusterlib-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.5.0/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/docs/source/conf.py` & `cardano-clusterlib-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.9/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.5.0/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

