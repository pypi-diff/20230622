# Comparing `tmp/datalake-scripts-2.6.7.tar.gz` & `tmp/datalake-scripts-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalake-scripts-2.6.7.tar", last modified: Tue Jun 13 14:11:41 2023, max compression
+gzip compressed data, was "datalake-scripts-2.6.8.tar", last modified: Thu Jun 22 12:57:01 2023, max compression
```

## Comparing `datalake-scripts-2.6.7.tar` & `datalake-scripts-2.6.8.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.862451 datalake-scripts-2.6.7/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.862451 datalake-scripts-2.6.7/datalake/api_objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/api_objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/api_objects/bulk_search_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.866451 datalake-scripts-2.6.7/datalake/common/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/atom_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/ouput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/throttler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/token_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/common/warn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/datalake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/bulk_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/sightings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake/endpoints/threats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/common/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/base_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/base_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/common/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/engines/get_engine.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5400 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/engines/post_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.870451 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/output_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/helper_scripts/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.874451 datalake-scripts-2.6.7/datalake_scripts/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/add_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/add_threats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/advanced_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8317 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/bulk_lookup_threats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/edit_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/get_query_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_by_hashkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_from_query_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/datalake_scripts/scripts/lookup_threats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/datalake_scripts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 14:11:41.000000 datalake-scripts-2.6.7/datalake_scripts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.874451 datalake-scripts-2.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.874451 datalake-scripts-2.6.7/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/common/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.878451 datalake-scripts-2.6.7/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_advanced_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_atom_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_auth_via_tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_bulk_search.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_sightings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/lib/test_threats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:41.882451 datalake-scripts-2.6.7/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_add_new_threats.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_base_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_csv_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_endpoint_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-13 14:11:30.000000 datalake-scripts-2.6.7/tests/scripts/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.009344 datalake-scripts-2.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-22 12:57:01.009344 datalake-scripts-2.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.001344 datalake-scripts-2.6.8/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.001344 datalake-scripts-2.6.8/datalake/api_objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/api_objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/api_objects/bulk_search_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.001344 datalake-scripts-2.6.8/datalake/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/atom_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/ouput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/throttler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/token_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/common/warn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/datalake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.001344 datalake-scripts-2.6.8/datalake/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/endpoints/advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/endpoints/bulk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/endpoints/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/endpoints/sightings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/endpoints/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17520 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake/endpoints/threats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.001344 datalake-scripts-2.6.8/datalake_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/datalake_scripts/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/common/base_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/common/base_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/common/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/datalake_scripts/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/engines/get_engine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5400 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/engines/post_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/datalake_scripts/helper_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/helper_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/helper_scripts/output_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/helper_scripts/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/datalake_scripts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/add_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/add_threats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/advanced_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8317 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/bulk_lookup_threats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/edit_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/get_query_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/get_threats_by_hashkey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/get_threats_from_query_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/datalake_scripts/scripts/lookup_threats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/datalake_scripts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-06-22 12:57:00.000000 datalake-scripts-2.6.8/datalake_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-06-22 12:57:00.000000 datalake-scripts-2.6.8/datalake_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 12:57:00.000000 datalake-scripts-2.6.8/datalake_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 12:57:00.000000 datalake-scripts-2.6.8/datalake_scripts.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 12:57:00.000000 datalake-scripts-2.6.8/datalake_scripts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 12:57:00.000000 datalake-scripts-2.6.8/datalake_scripts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-22 12:57:01.009344 datalake-scripts-2.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/common/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_advanced_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_atom_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_auth_via_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14237 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_bulk_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14739 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_sightings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21118 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/lib/test_threats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 12:57:01.005344 datalake-scripts-2.6.8/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/scripts/test_add_new_threats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/scripts/test_base_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/scripts/test_csv_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/scripts/test_endpoint_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-22 12:56:50.000000 datalake-scripts-2.6.8/tests/scripts/test_utils.py
```

### Comparing `datalake-scripts-2.6.7/PKG-INFO` & `datalake-scripts-2.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake-scripts
-Version: 2.6.7
+Version: 2.6.8
 Summary: A collection of scripts to easily use the API of OCD Datalake
 Home-page: https://github.com/cert-orangecyberdefense/datalake/
 Author: OCD
 Author-email: cert-contact.ocd@orange.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `datalake-scripts-2.6.7/README.md` & `datalake-scripts-2.6.8/README.md`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/__init__.py` & `datalake-scripts-2.6.8/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/api_objects/bulk_search_task.py` & `datalake-scripts-2.6.8/datalake/api_objects/bulk_search_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from datalake.common.utils import parse_api_timestamp
 
 
 class BulkSearchTaskState(Enum):
     NEW = "NEW"
     QUEUED = "QUEUED"
     IN_PROGRESS = "IN_PROGRESS"
+    GENERATING_STIX_FILES = "GENERATING_STIX_FILES"
     DONE = "DONE"
     CANCELLED = "CANCELLED"
     FAILED_ERROR = "FAILED_ERROR"
     FAILED_TIMEOUT = "FAILED_TIMEOUT"
 
 
 BULK_SEARCH_FAILED_STATE = {
```

### Comparing `datalake-scripts-2.6.7/datalake/common/atom.py` & `datalake-scripts-2.6.8/datalake/common/atom.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/common/atom_type.py` & `datalake-scripts-2.6.8/datalake/common/atom_type.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/common/ouput.py` & `datalake-scripts-2.6.8/datalake/common/ouput.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 
 class Output(Enum):
     JSON = "application/json"
     CSV = "text/csv"
     MISP = "application/x-misp+json"
     STIX = "application/stix+json"
+    STIX_ZIP = "text/x-stix-zip"
     JSON_ZIP = "application/zip"
     CSV_ZIP = "text/x-csv-zip"
-    STIX_ZIP = "text/x-stix-zip"
 
     def __str__(self):
         return self.name
 
     def __repr__(self):
         return str(self)
 
@@ -23,15 +23,15 @@
 def parse_response(response: Response) -> Union[str, dict]:
     """Parse a Request.Response depending of the Content-Type returned"""
     content_type = response.headers.get("Content-Type", Output.JSON.value)
     content_type = content_type.split(";")[
         0
     ]  # we don't care about extra info on the content
     if content_type in {
-        output.value for output in [Output.CSV, Output.CSV_ZIP, Output.JSON_ZIP]
+        output.value for output in [Output.CSV, Output.CSV_ZIP, Output.JSON_ZIP, Output.STIX_ZIP]
     }:
         return response.text
     else:
         return response.json()
 
 
 def display_outputs(outputs):
```

### Comparing `datalake-scripts-2.6.7/datalake/common/throttler.py` & `datalake-scripts-2.6.8/datalake/common/throttler.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/common/token_manager.py` & `datalake-scripts-2.6.8/datalake/common/token_manager.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/common/utils.py` & `datalake-scripts-2.6.8/datalake/common/utils.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/datalake.py` & `datalake-scripts-2.6.8/datalake/datalake.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/endpoints/advanced_search.py` & `datalake-scripts-2.6.8/datalake/endpoints/advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/endpoints/bulk_search.py` & `datalake-scripts-2.6.8/datalake/endpoints/bulk_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
         bs_as_json = results[0]
         return BulkSearchTask(endpoint=self, **bs_as_json)
 
     @output_supported(
         {
             Output.JSON,
             Output.JSON_ZIP,
-            Output.STIX,
             Output.STIX_ZIP,
             Output.CSV,
             Output.CSV_ZIP,
         }
     )
     def download(self, task_uuid, output=Output.JSON, stream=False):
         """
```

### Comparing `datalake-scripts-2.6.7/datalake/endpoints/endpoint.py` & `datalake-scripts-2.6.8/datalake/endpoints/endpoint.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/endpoints/sightings.py` & `datalake-scripts-2.6.8/datalake/endpoints/sightings.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/endpoints/tags.py` & `datalake-scripts-2.6.8/datalake/endpoints/tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake/endpoints/threats.py` & `datalake-scripts-2.6.8/datalake/endpoints/threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/cli.py` & `datalake-scripts-2.6.8/datalake_scripts/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from datalake_scripts.scripts import add_threats, get_threats_by_hashkey, edit_score, get_threats_from_query_hash, \
     add_comments, lookup_threats, add_tags, get_query_hash, bulk_lookup_threats, advanced_search
 
 
 class Cli:
     CLI_NAME = "ocd-dtl"
-    VERSION = "2.6.7"
+    VERSION = "2.6.8"
 
     def __init__(self):
         parser = argparse.ArgumentParser(
             description='Cli to interact with OCD\'s Datalake',
             usage=f'''
             {self.CLI_NAME} <command> [<args>]
```

### Comparing `datalake-scripts-2.6.7/datalake_scripts/common/__init__.py` & `datalake-scripts-2.6.8/datalake_scripts/common/__init__.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/common/base_engine.py` & `datalake-scripts-2.6.8/datalake_scripts/common/base_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/common/base_script.py` & `datalake-scripts-2.6.8/datalake_scripts/common/base_script.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/common/mixins.py` & `datalake-scripts-2.6.8/datalake_scripts/common/mixins.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/engines/get_engine.py` & `datalake-scripts-2.6.8/datalake_scripts/engines/get_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/engines/post_engine.py` & `datalake-scripts-2.6.8/datalake_scripts/engines/post_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/helper_scripts/output_builder.py` & `datalake-scripts-2.6.8/datalake_scripts/helper_scripts/output_builder.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/helper_scripts/utils.py` & `datalake-scripts-2.6.8/datalake_scripts/helper_scripts/utils.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/add_comments.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/add_comments.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/add_tags.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/add_tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/add_threats.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/add_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/advanced_search.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/bulk_lookup_threats.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/bulk_lookup_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/edit_score.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/edit_score.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/get_query_hash.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/get_query_hash.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_by_hashkey.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/get_threats_by_hashkey.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/get_threats_from_query_hash.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/get_threats_from_query_hash.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts/scripts/lookup_threats.py` & `datalake-scripts-2.6.8/datalake_scripts/scripts/lookup_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/datalake_scripts.egg-info/PKG-INFO` & `datalake-scripts-2.6.8/datalake_scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalake-scripts
-Version: 2.6.7
+Version: 2.6.8
 Summary: A collection of scripts to easily use the API of OCD Datalake
 Home-page: https://github.com/cert-orangecyberdefense/datalake/
 Author: OCD
 Author-email: cert-contact.ocd@orange.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `datalake-scripts-2.6.7/datalake_scripts.egg-info/SOURCES.txt` & `datalake-scripts-2.6.8/datalake_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/setup.py` & `datalake-scripts-2.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/common/fixture.py` & `datalake-scripts-2.6.8/tests/common/fixture.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/lib/test_advanced_search.py` & `datalake-scripts-2.6.8/tests/lib/test_advanced_search.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/lib/test_atom_type.py` & `datalake-scripts-2.6.8/tests/lib/test_atom_type.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/lib/test_auth_via_tokens.py` & `datalake-scripts-2.6.8/tests/lib/test_auth_via_tokens.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/lib/test_bulk_search.py` & `datalake-scripts-2.6.8/tests/lib/test_bulk_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 @responses.activate
 def test_bulk_search_task_download_invalid_output(bulk_search_task: BulkSearchTask):
     with pytest.raises(ValueError) as err:
         bulk_search_task.download(Output.MISP)
     assert (
         str(err.value)
         == f"MISP output type is not supported. Outputs supported are: CSV, CSV_ZIP, JSON, JSON_ZIP,"
-        " STIX, STIX_ZIP"
+        " STIX_ZIP"
     )
 
 
 @responses.activate
 def test_bulk_search_task_download_zip_json_output(bulk_search_task: BulkSearchTask):
     task_uuid = bulk_search_task.uuid
     bs_download_url = f"https://datalake.cert.orangecyberdefense.com/api/v2/mrti/bulk-search/task/{task_uuid}/"
```

### Comparing `datalake-scripts-2.6.7/tests/lib/test_output.py` & `datalake-scripts-2.6.8/tests/lib/test_output.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/lib/test_sightings.py` & `datalake-scripts-2.6.8/tests/lib/test_sightings.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/lib/test_tags.py` & `datalake-scripts-2.6.8/tests/lib/test_tags.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/lib/test_threats.py` & `datalake-scripts-2.6.8/tests/lib/test_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/scripts/test_add_new_threats.py` & `datalake-scripts-2.6.8/tests/scripts/test_add_new_threats.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/scripts/test_base_engine.py` & `datalake-scripts-2.6.8/tests/scripts/test_base_engine.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/scripts/test_csv_builder.py` & `datalake-scripts-2.6.8/tests/scripts/test_csv_builder.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/scripts/test_endpoint_config.py` & `datalake-scripts-2.6.8/tests/scripts/test_endpoint_config.py`

 * *Files identical despite different names*

### Comparing `datalake-scripts-2.6.7/tests/scripts/test_utils.py` & `datalake-scripts-2.6.8/tests/scripts/test_utils.py`

 * *Files identical despite different names*

