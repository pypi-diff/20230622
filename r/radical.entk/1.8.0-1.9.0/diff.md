# Comparing `tmp/radical.entk-1.8.0.tar.gz` & `tmp/radical.entk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/radical.entk-1.8.0.tar", last modified: Thu Sep 23 12:39:58 2021, max compression
+gzip compressed data, was "dist/radical.entk-1.9.0.tar", last modified: Tue Nov 23 17:42:12 2021, max compression
```

## Comparing `radical.entk-1.8.0.tar` & `radical.entk-1.9.0.tar`

### file list

```diff
@@ -1,81 +1,79 @@
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.900558 radical.entk-1.8.0/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    10660 2021-09-23 12:38:27.000000 radical.entk-1.8.0/CHANGES.md
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1284 2021-07-15 08:36:42.000000 radical.entk-1.8.0/LICENSE.md
--rw-r--r--   0 merzky    (1001) merzky    (1001)      148 2019-05-11 12:36:04.000000 radical.entk-1.8.0/MANIFEST.in
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      973 2021-09-23 12:39:58.900558 radical.entk-1.8.0/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      674 2021-07-15 08:36:42.000000 radical.entk-1.8.0/README.md
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)        6 2021-09-23 12:37:12.000000 radical.entk-1.8.0/VERSION
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.892558 radical.entk-1.8.0/bin/
--rw-r--r--   0 merzky    (1001) merzky    (1001)       79 2020-02-06 22:43:50.000000 radical.entk-1.8.0/bin/radical-entk-version
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.888558 radical.entk-1.8.0/examples/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.892558 radical.entk-1.8.0/examples/advanced/
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     1767 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/advanced/adapt_ta.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     1778 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/advanced/adapt_tc.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     1683 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/advanced/adapt_to.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.892558 radical.entk-1.8.0/examples/analytics/
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     3847 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/analytics/get_durations.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     3797 2020-02-06 22:43:50.000000 radical.entk-1.8.0/examples/analytics/get_timestamps.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.892558 radical.entk-1.8.0/examples/misc/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     8546 2021-04-13 20:04:33.000000 radical.entk-1.8.0/examples/misc/async_repex.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3593 2021-06-29 08:12:32.000000 radical.entk-1.8.0/examples/misc/lfs_tagging_dd.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     2509 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/misc/suspend_pipelines.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.892558 radical.entk-1.8.0/examples/simple/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3271 2021-07-15 08:36:42.000000 radical.entk-1.8.0/examples/simple/eop.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3835 2021-07-15 08:36:42.000000 radical.entk-1.8.0/examples/simple/poe.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)   326536 2021-01-28 18:09:14.000000 radical.entk-1.8.0/examples/simple/radical.entk.task_processor.log
--rw-r--r--   0 merzky    (1001) merzky    (1001)     1432 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/simple/sow.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.896558 radical.entk-1.8.0/examples/user_guide/
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2537 2021-04-13 20:04:33.000000 radical.entk-1.8.0/examples/user_guide/add_data.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2397 2021-04-13 20:04:33.000000 radical.entk-1.8.0/examples/user_guide/add_pipelines.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     2456 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/user_guide/add_shared_data.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2632 2021-04-13 20:04:33.000000 radical.entk-1.8.0/examples/user_guide/add_stages.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2070 2021-04-13 20:04:33.000000 radical.entk-1.8.0/examples/user_guide/add_tasks.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     2521 2020-11-23 20:13:15.000000 radical.entk-1.8.0/examples/user_guide/change_target.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2015 2021-04-13 20:04:33.000000 radical.entk-1.8.0/examples/user_guide/get_started.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)     2646 2020-02-06 22:43:50.000000 radical.entk-1.8.0/examples/user_guide/profiling.py
--rwxr-xr-x   0 merzky    (1001) merzky    (1001)       54 2021-09-23 12:39:58.900558 radical.entk-1.8.0/setup.cfg
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)     9278 2021-09-23 12:36:51.000000 radical.entk-1.8.0/setup.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.892558 radical.entk-1.8.0/src/
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.896558 radical.entk-1.8.0/src/radical/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       57 2021-09-23 12:36:51.000000 radical.entk-1.8.0/src/radical/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.896558 radical.entk-1.8.0/src/radical/entk/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       40 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical/entk/SDIST
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       20 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical/entk/VERSION
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     1415 2021-09-23 12:36:59.000000 radical.entk-1.8.0/src/radical/entk/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.896558 radical.entk-1.8.0/src/radical/entk/appman/
--rw-r--r--   0 merzky    (1001) merzky    (1001)        0 2019-05-11 12:34:31.000000 radical.entk-1.8.0/src/radical/entk/appman/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    39911 2021-09-23 12:36:59.000000 radical.entk-1.8.0/src/radical/entk/appman/appmanager.py
--rw-r--r--   0 merzky    (1001) merzky    (1001)      488 2020-02-06 22:43:50.000000 radical.entk-1.8.0/src/radical/entk/appman/config.json
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    23481 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/appman/wfprocessor.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      227 2021-09-23 12:36:51.000000 radical.entk-1.8.0/src/radical/entk/constants.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2390 2021-09-23 12:36:51.000000 radical.entk-1.8.0/src/radical/entk/exceptions.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.896558 radical.entk-1.8.0/src/radical/entk/execman/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       55 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/execman/__init__.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.896558 radical.entk-1.8.0/src/radical/entk/execman/base/
--rw-r--r--   0 merzky    (1001) merzky    (1001)       94 2020-11-23 20:54:27.000000 radical.entk-1.8.0/src/radical/entk/execman/base/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    10523 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/execman/base/resource_manager.py
--rwxrwxr-x   0 merzky    (1001) merzky    (1001)    17854 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/execman/base/task_manager.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.900558 radical.entk-1.8.0/src/radical/entk/execman/mock/
--rw-r--r--   0 merzky    (1001) merzky    (1001)       84 2020-11-23 20:54:27.000000 radical.entk-1.8.0/src/radical/entk/execman/mock/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     3425 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/execman/mock/resource_manager.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    12215 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/execman/mock/task_manager.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.900558 radical.entk-1.8.0/src/radical/entk/execman/rp/
--rw-r--r--   0 merzky    (1001) merzky    (1001)       90 2019-12-27 08:49:26.000000 radical.entk-1.8.0/src/radical/entk/execman/rp/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     9342 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/execman/rp/resource_manager.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    21334 2021-07-15 08:36:42.000000 radical.entk-1.8.0/src/radical/entk/execman/rp/task_manager.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    20361 2021-09-23 12:36:51.000000 radical.entk-1.8.0/src/radical/entk/execman/rp/task_processor.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    12485 2021-06-29 08:12:32.000000 radical.entk-1.8.0/src/radical/entk/pipeline.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    12074 2021-09-23 12:36:51.000000 radical.entk-1.8.0/src/radical/entk/stage.py
--rw-r--r--   0 merzky    (1001) merzky    (1001)     2123 2020-02-06 11:06:06.000000 radical.entk-1.8.0/src/radical/entk/states.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)    35568 2021-09-23 12:36:51.000000 radical.entk-1.8.0/src/radical/entk/task.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.900558 radical.entk-1.8.0/src/radical/entk/utils/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      481 2021-01-06 08:55:16.000000 radical.entk-1.8.0/src/radical/entk/utils/__init__.py
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     8471 2021-01-06 08:55:16.000000 radical.entk-1.8.0/src/radical/entk/utils/prof_utils.py
-drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-09-23 12:39:58.896558 radical.entk-1.8.0/src/radical.entk.egg-info/
--rw-rw-r--   0 merzky    (1001) merzky    (1001)      973 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical.entk.egg-info/PKG-INFO
--rw-rw-r--   0 merzky    (1001) merzky    (1001)     2019 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical.entk.egg-info/SOURCES.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical.entk.egg-info/dependency_links.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical.entk.egg-info/namespace_packages.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical.entk.egg-info/not-zip-safe
--rw-rw-r--   0 merzky    (1001) merzky    (1001)       48 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical.entk.egg-info/requires.txt
--rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-09-23 12:39:58.000000 radical.entk-1.8.0/src/radical.entk.egg-info/top_level.txt
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)       54 2021-11-23 17:42:12.000000 radical.entk-1.9.0/setup.cfg
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/examples/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/examples/misc/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3593 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/misc/lfs_tagging_dd.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     8546 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/misc/async_repex.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2509 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/misc/suspend_pipelines.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/examples/analytics/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3847 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/analytics/get_durations.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3797 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/analytics/get_timestamps.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/examples/simple/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3835 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/simple/poe.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     3271 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/simple/eop.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1432 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/simple/sow.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/examples/user_guide/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2646 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/profiling.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2070 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/add_tasks.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2397 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/add_pipelines.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2456 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/add_shared_data.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2537 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/add_data.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2015 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/get_started.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2632 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/add_stages.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     2521 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/user_guide/change_target.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/examples/advanced/
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1683 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/advanced/adapt_to.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1778 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/advanced/adapt_tc.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1767 2021-09-24 08:24:39.000000 radical.entk-1.9.0/examples/advanced/adapt_ta.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    10854 2021-11-23 17:41:46.000000 radical.entk-1.9.0/CHANGES.md
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     9706 2021-11-23 17:41:52.000000 radical.entk-1.9.0/setup.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      674 2021-09-24 08:24:39.000000 radical.entk-1.9.0/README.md
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/bin/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       79 2021-09-24 08:24:39.000000 radical.entk-1.9.0/bin/radical-entk-version
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)     1284 2021-09-24 08:24:39.000000 radical.entk-1.9.0/LICENSE.md
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1010 2021-11-23 17:42:12.000000 radical.entk-1.9.0/PKG-INFO
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)        6 2021-11-23 17:41:49.000000 radical.entk-1.9.0/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      148 2021-09-24 08:24:39.000000 radical.entk-1.9.0/MANIFEST.in
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/namespace_packages.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       48 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/requires.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/dependency_links.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        8 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/top_level.txt
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1010 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/PKG-INFO
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        1 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/not-zip-safe
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1947 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical.entk.egg-info/SOURCES.txt
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       26 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/SDIST
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    12485 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/pipeline.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2390 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/exceptions.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     2123 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/states.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     1415 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    35568 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/task.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/execman/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       55 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/__init__.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/execman/rp/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       90 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/rp/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    20361 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/execman/rp/task_processor.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    21334 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/rp/task_manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     9527 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/execman/rp/resource_manager.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/execman/mock/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       84 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/mock/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    12215 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/mock/task_manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     3425 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/mock/resource_manager.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/execman/base/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       94 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/base/__init__.py
+-rwxrwxr-x   0 merzky    (1001) merzky    (1001)    17854 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/base/task_manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    10523 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/execman/base/resource_manager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      227 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/constants.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/utils/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      481 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/utils/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)     8471 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/utils/prof_utils.py
+drwxrwxr-x   0 merzky    (1001) merzky    (1001)        0 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/appman/
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    23655 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/appman/wfprocessor.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)        0 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/appman/__init__.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)      488 2021-09-24 08:24:39.000000 radical.entk-1.9.0/src/radical/entk/appman/config.json
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    40072 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/appman/appmanager.py
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)       26 2021-11-23 17:42:12.000000 radical.entk-1.9.0/src/radical/entk/VERSION
+-rw-rw-r--   0 merzky    (1001) merzky    (1001)    12074 2021-11-23 17:41:52.000000 radical.entk-1.9.0/src/radical/entk/stage.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `radical.entk-1.8.0/CHANGES.md` & `radical.entk-1.9.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,20 @@
   - For a list of bug fixes, see
     https://github.com/radical-cybertools/radical.entk/ \
             issues?q=is%3Aissue+is%3Aclosed+sort%3Aupdated-desc
   - For a list of open issues and known problems, see
     https://github.com/radical-cybertools/radical.entk/ \
             issues?q=is%3Aissue+is%3Aopen+
 
+1.9.0  Release                                                        2021-11-22
+--------------------------------------------------------------------------------
+
+  - support mem_per_process
+
+
 1.8.0  Release                                                        2021-09-23
 --------------------------------------------------------------------------------
 
   - 'config' param introduced in AppManager to take 'base_path' etc.
   - eliminating warning message for being offline
   - type conversion to str for PosixPath
 
@@ -312,7 +318,8 @@
 ## Changelog for 0.6.0
 
 * ```_parent_pipeline``` and ```_parent_stage``` on Stage and Task objects
   changed to ```parent_pipeline``` and ```parent_stage```.
 
 # ------------------------------------------------------------------------------
 
+
```

### Comparing `radical.entk-1.8.0/LICENSE.md` & `radical.entk-1.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/PKG-INFO` & `radical.entk-1.9.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: radical.entk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Radical Ensemble Toolkit.
 Home-page: https://www.github.com/radical-cybertools/radical.entk/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
-Description: UNKNOWN
 Keywords: ensemble workflow execution
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,7 +19,12 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Requires-Python: >=3.6
+License-File: LICENSE.md
+
+UNKNOWN
+
```

### Comparing `radical.entk-1.8.0/README.md` & `radical.entk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/advanced/adapt_ta.py` & `radical.entk-1.9.0/examples/advanced/adapt_ta.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/advanced/adapt_tc.py` & `radical.entk-1.9.0/examples/advanced/adapt_tc.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/advanced/adapt_to.py` & `radical.entk-1.9.0/examples/advanced/adapt_to.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/analytics/get_durations.py` & `radical.entk-1.9.0/examples/analytics/get_durations.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/analytics/get_timestamps.py` & `radical.entk-1.9.0/examples/analytics/get_timestamps.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/misc/async_repex.py` & `radical.entk-1.9.0/examples/misc/async_repex.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/misc/lfs_tagging_dd.py` & `radical.entk-1.9.0/examples/misc/lfs_tagging_dd.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/misc/suspend_pipelines.py` & `radical.entk-1.9.0/examples/misc/suspend_pipelines.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/simple/eop.py` & `radical.entk-1.9.0/examples/simple/eop.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/simple/poe.py` & `radical.entk-1.9.0/examples/simple/poe.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/simple/sow.py` & `radical.entk-1.9.0/examples/simple/sow.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/add_data.py` & `radical.entk-1.9.0/examples/user_guide/add_data.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/add_pipelines.py` & `radical.entk-1.9.0/examples/user_guide/add_pipelines.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/add_shared_data.py` & `radical.entk-1.9.0/examples/user_guide/add_shared_data.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/add_stages.py` & `radical.entk-1.9.0/examples/user_guide/add_stages.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/add_tasks.py` & `radical.entk-1.9.0/examples/user_guide/add_tasks.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/change_target.py` & `radical.entk-1.9.0/examples/user_guide/change_target.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/get_started.py` & `radical.entk-1.9.0/examples/user_guide/get_started.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/examples/user_guide/profiling.py` & `radical.entk-1.9.0/examples/user_guide/profiling.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/setup.py` & `radical.entk-1.9.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 import os
 import sys
 import glob
 import shutil
 
 import subprocess as sp
 
-from setuptools import setup, Command, find_packages
+
+from setuptools import setup, Command, find_namespace_packages
 
 
 # ------------------------------------------------------------------------------
 name     = 'radical.entk'
 mod_root = 'src/radical/entk/'
 
 
@@ -86,70 +87,71 @@
         _version_detail = _version_detail.decode()
         _version_detail = _version_detail.replace('detached from ', 'detached-')
 
         # remove all non-alphanumeric (and then some) chars
         _version_detail = re.sub('[/ ]+', '-', _version_detail)
         _version_detail = re.sub('[^a-zA-Z0-9_+@.-]+', '', _version_detail)
 
-        if  ret            !=  0  or \
+        if ret              !=  0  or \
             _version_detail == '@' or \
             'git-error'      in _version_detail or \
             'not-a-git-repo' in _version_detail or \
             'not-found'      in _version_detail or \
             'fatal'          in _version_detail :
             _version = _version_base
         elif '@' not in _version_base:
             _version = '%s-%s' % (_version_base, _version_detail)
         else:
             _version = _version_base
 
         # make sure the version files exist for the runtime version inspection
-        path = '%s/%s' % (src_root, _mod_root)
-        with open(path + '/VERSION', 'w') as f:
-            f.write(_version + '\n')
-
-        _sdist_name = '%s-%s.tar.gz' % (name, _version)
-        _sdist_name = _sdist_name.replace('/', '-')
-        _sdist_name = _sdist_name.replace('@', '-')
-        _sdist_name = _sdist_name.replace('#', '-')
-        _sdist_name = _sdist_name.replace('_', '-')
+        _path = '%s/%s' % (src_root, _mod_root)
+        with open(_path + '/VERSION', 'w') as f:
+            f.write(_version_base + '\n')
+            f.write(_version      + '\n')
+
+        _sdist_name = '%s-%s.tar.gz' % (name, _version_base)
+      # _sdist_name = _sdist_name.replace('/', '-')
+      # _sdist_name = _sdist_name.replace('@', '-')
+      # _sdist_name = _sdist_name.replace('#', '-')
+      # _sdist_name = _sdist_name.replace('_', '-')
 
         if '--record'    in sys.argv or \
            'bdist_egg'   in sys.argv or \
            'bdist_wheel' in sys.argv    :
-          # pip install stage 2 or easy_install stage 1
-          #
-          # pip install will untar the sdist in a tmp tree.  In that tmp
-          # tree, we won't be able to derive git version tags -- so we pack the
-          # formerly derived version as ./VERSION
-            shutil.move('VERSION', 'VERSION.bak')            # backup version
-            shutil.copy('%s/VERSION' % path, 'VERSION')      # use full version
-            os.system  ('python3 setup.py sdist')             # build sdist
+            # pip install stage 2 or easy_install stage 1
+            #
+            # pip install will untar the sdist in a tmp tree.  In that tmp
+            # tree, we won't be able to derive git version tags -- so we pack
+            # the formerly derived version as ./VERSION
+            shutil.move("VERSION", "VERSION.bak")              # backup
+            shutil.copy("%s/VERSION" % _path, "VERSION")       # version to use
+            os.system  ("python3 setup.py sdist")               # build sdist
             shutil.copy('dist/%s' % _sdist_name,
                         '%s/%s'   % (_mod_root, _sdist_name))  # copy into tree
-            shutil.move('VERSION.bak', 'VERSION')            # restore version
+            shutil.move('VERSION.bak', 'VERSION')              # restore version
 
-        with open(path + '/SDIST', 'w') as f:
+        with open(_path + '/SDIST', 'w') as f:
             f.write(_sdist_name + '\n')
 
-        return _version_base, _version_detail, _sdist_name
+        return _version_base, _version_detail, _sdist_name, _path
 
     except Exception as e:
         raise RuntimeError('Could not extract/set version: %s' % e) from e
 
 
 # ------------------------------------------------------------------------------
-# check python version. we need >= 3.6
-if  sys.hexversion <= 0x03050000:
-    raise RuntimeError('%s requires Python 3.6 or higher' % name)
+# check python version, should be >= 3.6
+if sys.hexversion < 0x03060000:
+    raise RuntimeError('ERROR: %s requires Python 3.6 or newer' % name)
 
 
 # ------------------------------------------------------------------------------
 # get version info -- this will create VERSION and srcroot/VERSION
-version, version_detail, sdist_name = get_version(mod_root)
+version, version_detail, sdist_name, path = get_version(mod_root)
 
 
 # ------------------------------------------------------------------------------
 #
 def read(fname):
     try:
         return open(fname).read()
@@ -166,25 +168,20 @@
     def run(self):
         _, _, ret = sh_callout('python3 setup.py sdist upload -r pypi')
         raise SystemExit(ret)
 
 
 # ------------------------------------------------------------------------------
 #
-if  sys.hexversion <= 0x03050000:
-    raise RuntimeError('SETUP ERROR: %s requires Python 3.6 or higher' % name)
-
-
-# ------------------------------------------------------------------------------
-#
-df = list()
-df.append(('share/%s/examples/user_guide/' % name, glob.glob('examples/user_guide/*')))
-df.append(('share/%s/examples/simple/'     % name, glob.glob('examples/simple/*')))
-df.append(('share/%s/examples/advanced/'   % name, glob.glob('examples/advanced/*')))
-df.append(('share/%s/examples/analytics/'  % name, glob.glob('examples/analytics/*')))
+base = 'share/%s' % name
+df = [('%s/examples/user_guide/' % base, glob.glob('examples/user_guide/*')),
+      ('%s/examples/simple/'     % base, glob.glob('examples/simple/*')),
+      ('%s/examples/advanced/'   % base, glob.glob('examples/advanced/*')),
+      ('%s/examples/analytics/'  % base, glob.glob('examples/analytics/*'))
+]
 
 
 # ------------------------------------------------------------------------------
 #
 setup_args = {
     'name'               : name,
     'namespace_packages' : ['radical'],
@@ -194,14 +191,15 @@
     'author'             : 'RADICAL Group at Rutgers University',
     'author_email'       : 'radical@rutgers.edu',
     'maintainer'         : 'The RADICAL Group',
     'maintainer_email'   : 'radical@rutgers.edu',
     'url'                : 'https://www.github.com/radical-cybertools/radical.entk/',
     'license'            : 'MIT',
     'keywords'           : "ensemble workflow execution",
+    'python_requires'    : '>=3.6',
     'classifiers'        : [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Environment :: Console',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
@@ -209,19 +207,19 @@
         'Topic :: Utilities',
         'Topic :: System :: Distributed Computing',
         'Topic :: Scientific/Engineering',
         'Operating System :: MacOS :: MacOS X',
         'Operating System :: POSIX',
         'Operating System :: Unix'
     ],
-    'packages'           : find_packages('src'),
+    'packages'           : find_namespace_packages('src', include=['radical.*']),
     'package_dir'        : {'': 'src'},
     'scripts'            : ['bin/radical-entk-version'],
     'package_data'       : {'': ['*.txt', '*.sh', '*.json', '*.gz', '*.c',
-                                 'VERSION', 'CHANGES.md', 'SDIST', sdist_name]},
+                                 '*.md', 'VERSION', 'SDIST', sdist_name]},
   # 'setup_requires'     : ['pytest-runner'],
     'install_requires'   : ['radical.utils',
                             'radical.pilot',
                             'pika==0.13.0',
                             'sphinx'
                            ],
     'tests_require'      : ['pytest',
@@ -229,21 +227,35 @@
                             'flake8',
                             'coverage',
                             'hypothesis',
                             'timeout_decorator'
                            ],
     'test_suite'         : '%s.tests' % name,
     'zip_safe'           : False,
+  # 'build_sphinx'       : {
+  #     'source-dir'     : 'docs/',
+  #     'build-dir'      : 'docs/build',
+  #     'all_files'      : 1,
+  # },
+  # 'upload_sphinx'      : {
+  #     'upload-dir'     : 'docs/build/html',
+  # },
+    # This copies the contents of the examples/ dir under
+    # sys.prefix/share/$name
+    # It needs the MANIFEST.in entries to work.
     'data_files'         : df,
     'cmdclass'           : {'upload': RunTwine},
 }
 
 
 # ------------------------------------------------------------------------------
 #
 setup(**setup_args)
 
 os.system('rm -rf src/%s.egg-info' % name)
+# os.system('rm -rf %s/VERSION'      % path)
+# os.system('rm -rf %s/VERSION.git'  % path)
+# os.system('rm -rf %s/SDIST'        % path)
 
 
 # ------------------------------------------------------------------------------
```

### Comparing `radical.entk-1.8.0/src/radical/entk/__init__.py` & `radical.entk-1.9.0/src/radical/entk/__init__.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/appman/appmanager.py` & `radical.entk-1.9.0/src/radical/entk/appman/appmanager.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 __license__   = 'MIT'
 
 import os
 import json
 import pika
 import time
 
-import threading     as mt
+import threading       as mt
+import multiprocessing as mp
 
-import radical.utils as ru
+import radical.utils   as ru
 
 from ..           import exceptions as ree
 from ..           import states
 
 from ..pipeline   import Pipeline
 from ..task       import Task
 from ..utils      import write_session_description
@@ -123,14 +124,15 @@
         self._shared_data     = list()
         self._outputs         = None
         self._wfp             = None
         self._sync_thread     = None
         self._terminate_sync  = mt.Event()
         self._resubmit_failed = False
         self._port            = int(self._port)
+        self._term            = mp.Event()
 
         # Setup rabbitmq queues
         self._setup_mqs()
 
         self._rmq_ping_interval = int(os.getenv('RMQ_PING_INTERVAL', "10"))
 
         self._logger.info('Application Manager initialized')
@@ -482,14 +484,16 @@
 
     # --------------------------------------------------------------------------
     #
     def terminate(self):
 
         self._prof.prof('term_start', uid=self._uid)
 
+        self._term.set()
+
         # Terminate threads in following order: wfp, helper, synchronizer
         if self._wfp:
             self._logger.info('Terminating WFprocessor')
             self._wfp.terminate_processor()
 
         if self._task_manager:
             self._logger.info('Terminating task manager process')
@@ -730,14 +734,17 @@
         # We wait till all pipelines of the workflow are marked
         # complete
         # incomplete = self._wfp.workflow_incomplete()
         rts_final_states = self._rmgr.get_completed_states()
 
         while active_pipe_count and self._cur_attempt <= self._reattempts:
 
+            if self._term.is_set():
+                break
+
             for pipe in self._workflow:
 
                 with pipe.lock:
 
                     if pipe.completed and \
                        pipe.uid not in finished_pipe_uids:
```

### Comparing `radical.entk-1.8.0/src/radical/entk/appman/wfprocessor.py` & `radical.entk-1.9.0/src/radical/entk/appman/wfprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 __license__   = "MIT"
 
 
 import os
 import json
 import pika
 import time
-import threading
+import threading     as mt
 
 import radical.utils as ru
 
 from ..           import states, Task
 from ..exceptions import EnTKError
 
 
@@ -509,14 +509,15 @@
 
         finally:
             try:
                 mq_connection.close()
             except Exception as ex:
                 self._logger.warning('mq_connection close failed, %s' % ex)
             self._logger.debug('closed mq_connection')
+            self.terminate_processor()
 
 
     # --------------------------------------------------------------------------
     #
     # Public Methods
     #
     def start_processor(self):
@@ -527,27 +528,27 @@
         """
 
         try:
 
             self._logger.info('Starting WFprocessor')
             self._prof.prof('wfp_start', uid=self._uid)
 
-            self._enqueue_thread_terminate = threading.Event()
-            self._dequeue_thread_terminate = threading.Event()
+            self._enqueue_thread_terminate = mt.Event()
+            self._dequeue_thread_terminate = mt.Event()
 
             # Start dequeue thread
-            self._dequeue_thread = threading.Thread(target=self._dequeue,
-                                                    name='dequeue-thread')
+            self._dequeue_thread = mt.Thread(target=self._dequeue,
+                                             name='dequeue-thread')
             self._logger.info('Starting dequeue-thread')
             self._prof.prof('starting dequeue-thread', uid=self._uid)
             self._dequeue_thread.start()
 
             # Start enqueue thread
-            self._enqueue_thread = threading.Thread(target=self._enqueue,
-                                                    name='enqueue-thread')
+            self._enqueue_thread = mt.Thread(target=self._enqueue,
+                                             name='enqueue-thread')
             self._logger.info('Starting enqueue-thread')
             self._prof.prof('starting enqueue-thread', uid=self._uid)
             self._enqueue_thread.start()
 
             self._logger.info('WFprocessor started')
             self._prof.prof('wfp_started', uid=self._uid)
 
@@ -564,28 +565,32 @@
         """
         **Purpose**: Method to terminate the wfp process. This method is
         blocking as it waits for the wfp process to terminate (aka join).
         """
 
         try:
 
+            tid = mt.current_thread().ident
+
             if self._enqueue_thread:
 
                 if not self._enqueue_thread_terminate.is_set():
                     self._logger.info('Terminating enqueue-thread')
                     self._enqueue_thread_terminate.set()
-                    self._enqueue_thread.join()
+                    if tid != self._enqueue_thread.ident:
+                        self._enqueue_thread.join()
                     self._enqueue_thread = None
 
             if self._dequeue_thread:
 
                 if not self._dequeue_thread_terminate.is_set():
                     self._logger.info('Terminating dequeue-thread')
                     self._dequeue_thread_terminate.set()
-                    self._dequeue_thread.join()
+                    if tid != self._dequeue_thread.ident:
+                      self._dequeue_thread.join()
                     self._dequeue_thread = None
 
             self._logger.info('WFprocessor terminated')
             self._prof.prof('wfp_stop', uid=self._uid)
             self._prof.close()
 
         except Exception as ex:
```

### Comparing `radical.entk-1.8.0/src/radical/entk/exceptions.py` & `radical.entk-1.9.0/src/radical/entk/exceptions.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/execman/base/resource_manager.py` & `radical.entk-1.9.0/src/radical/entk/execman/base/resource_manager.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/execman/base/task_manager.py` & `radical.entk-1.9.0/src/radical/entk/execman/base/task_manager.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/execman/mock/resource_manager.py` & `radical.entk-1.9.0/src/radical/entk/execman/mock/resource_manager.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/execman/mock/task_manager.py` & `radical.entk-1.9.0/src/radical/entk/execman/mock/task_manager.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/execman/rp/resource_manager.py` & `radical.entk-1.9.0/src/radical/entk/execman/rp/resource_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,19 +180,22 @@
             if self._shared_data:
                 shared_data = []
                 for data in self._shared_data:
                     data = data.split('>')
                     if len(data) > 1:
                         shared_data.append({'source': data[0].strip(),
                                             'target': data[1].strip(),
-                                            'action': rp.TRANSFER})
+                                            'action': rp.TRANSFER,
+                                            'flags' : rp.RECURSIVE})
                     else:
+                        data[0] = data[0].rstrip('/')
                         shared_data.append({'source': data[0].strip(),
-                                            'target': data[0].split('/')[-1].strip(),
-                                            'action': rp.TRANSFER})
+                                            'target': os.path.basename(data[0]),
+                                            'action': rp.TRANSFER,
+                                            'flags' : rp.RECURSIVE})
                 self._pilot.stage_in(shared_data)
             self._prof.prof('rreq submitted', uid=self._uid)
 
             self._logger.info('Resource request submission successful, waiting'
                               'for pilot to become Active')
 
             # Wait for pilot to go active or final state
```

### Comparing `radical.entk-1.8.0/src/radical/entk/execman/rp/task_manager.py` & `radical.entk-1.9.0/src/radical/entk/execman/rp/task_manager.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/execman/rp/task_processor.py` & `radical.entk-1.9.0/src/radical/entk/execman/rp/task_processor.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/pipeline.py` & `radical.entk-1.9.0/src/radical/entk/pipeline.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/stage.py` & `radical.entk-1.9.0/src/radical/entk/stage.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/states.py` & `radical.entk-1.9.0/src/radical/entk/states.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/task.py` & `radical.entk-1.9.0/src/radical/entk/task.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical/entk/utils/prof_utils.py` & `radical.entk-1.9.0/src/radical/entk/utils/prof_utils.py`

 * *Files identical despite different names*

### Comparing `radical.entk-1.8.0/src/radical.entk.egg-info/PKG-INFO` & `radical.entk-1.9.0/src/radical.entk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: radical.entk
-Version: 1.8.0
+Version: 1.9.0
 Summary: Radical Ensemble Toolkit.
 Home-page: https://www.github.com/radical-cybertools/radical.entk/
 Author: RADICAL Group at Rutgers University
 Author-email: radical@rutgers.edu
 Maintainer: The RADICAL Group
 Maintainer-email: radical@rutgers.edu
 License: MIT
-Description: UNKNOWN
 Keywords: ensemble workflow execution
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -20,7 +19,12 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Utilities
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
+Requires-Python: >=3.6
+License-File: LICENSE.md
+
+UNKNOWN
+
```

### Comparing `radical.entk-1.8.0/src/radical.entk.egg-info/SOURCES.txt` & `radical.entk-1.9.0/src/radical.entk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,23 @@
 examples/analytics/get_durations.py
 examples/analytics/get_timestamps.py
 examples/misc/async_repex.py
 examples/misc/lfs_tagging_dd.py
 examples/misc/suspend_pipelines.py
 examples/simple/eop.py
 examples/simple/poe.py
-examples/simple/radical.entk.task_processor.log
 examples/simple/sow.py
 examples/user_guide/add_data.py
 examples/user_guide/add_pipelines.py
 examples/user_guide/add_shared_data.py
 examples/user_guide/add_stages.py
 examples/user_guide/add_tasks.py
 examples/user_guide/change_target.py
 examples/user_guide/get_started.py
 examples/user_guide/profiling.py
-src/radical/__init__.py
 src/radical.entk.egg-info/PKG-INFO
 src/radical.entk.egg-info/SOURCES.txt
 src/radical.entk.egg-info/dependency_links.txt
 src/radical.entk.egg-info/namespace_packages.txt
 src/radical.entk.egg-info/not-zip-safe
 src/radical.entk.egg-info/requires.txt
 src/radical.entk.egg-info/top_level.txt
```

