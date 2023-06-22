# Comparing `tmp/lisflood-model-4.1.2.tar.gz` & `tmp/lisflood-model-4.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lisflood-model-4.1.2.tar", last modified: Wed Mar 22 09:18:23 2023, max compression
+gzip compressed data, was "dist/lisflood-model-4.1.3.tar", last modified: Thu Jun 22 12:04:02 2023, max compression
```

## Comparing `lisflood-model-4.1.2.tar` & `lisflood-model-4.1.3.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    13760 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/LICENSE
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      131 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/MANIFEST.in
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8729 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7528 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/README.md
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-03-22 09:15:43.000000 lisflood-model-4.1.2/VERSION
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/bin/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1623 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/bin/lisflood
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      633 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/requirements.txt
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)       38 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/setup.cfg
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     6821 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/setup.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/src/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1428 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisf1.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/src/lisflood/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     2424 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/Lisflood_EnKF.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11316 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/Lisflood_dynamic.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    17724 2023-02-23 11:44:06.000000 lisflood-model-4.1.2/src/lisflood/Lisflood_initial.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1450 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/Lisflood_monteCarlo.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      682 2023-03-22 09:15:43.000000 lisflood-model-4.1.2/src/lisflood/__init__.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/src/lisflood/global_modules/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/global_modules/__init__.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    37628 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/global_modules/add1.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     4396 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/global_modules/checkers.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3027 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/global_modules/decorators.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)   131101 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/global_modules/default_options.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1554 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/global_modules/errors.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    20485 2023-03-22 09:15:43.000000 lisflood-model-4.1.2/src/lisflood/global_modules/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    17563 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/global_modules/output.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    30488 2023-03-22 09:15:43.000000 lisflood-model-4.1.2/src/lisflood/global_modules/settings.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     6153 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/global_modules/stateVar.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    17146 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/global_modules/zusatz.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     2739 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/__init__.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1130 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/compile_kinematic_wave_parallel_tools.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7696 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/evapowater.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4460 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/frost.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8170 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/groundwater.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    16483 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/indicatorcalc.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     6044 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/inflow.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    11427 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/kinematic_wave_parallel.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)   901029 2022-11-18 10:21:29.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.c
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     8133 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    15667 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/lakes.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    10358 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/landusechange.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4128 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/leafarea.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7709 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/miscInitial.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3335 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/opensealed.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7610 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/polder.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3996 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/readmeteo.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    19690 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/reservoir.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    10610 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/riceirrigation.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    41378 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/routing.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     9644 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/snow.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    30635 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/soil.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    50345 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/soilloop.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     2946 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/structures.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    13122 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/surface_routing.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3763 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/transmission.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    57847 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/waterabstraction.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)    17140 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/waterbalance.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3334 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/waterlevel.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1620 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/hydrological_modules/wateruse.py
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)     8277 2022-10-04 12:24:33.000000 lisflood-model-4.1.2/src/lisflood/main.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)   143665 2023-03-21 11:20:34.000000 lisflood-model-4.1.2/src/lisfloodSettings_reference.xml
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/src/lisflood_model.egg-info/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8729 2023-03-22 09:18:22.000000 lisflood-model-4.1.2/src/lisflood_model.egg-info/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2497 2023-03-22 09:18:23.000000 lisflood-model-4.1.2/src/lisflood_model.egg-info/SOURCES.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-03-22 09:18:22.000000 lisflood-model-4.1.2/src/lisflood_model.egg-info/dependency_links.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      644 2023-03-22 09:18:22.000000 lisflood-model-4.1.2/src/lisflood_model.egg-info/requires.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       15 2023-03-22 09:18:22.000000 lisflood-model-4.1.2/src/lisflood_model.egg-info/top_level.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2022-10-04 10:05:22.000000 lisflood-model-4.1.2/src/lisflood_model.egg-info/zip-safe
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    13760 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/LICENSE
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      131 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/MANIFEST.in
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8729 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7528 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/README.md
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/VERSION
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/bin/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1623 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/bin/lisflood
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      628 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/requirements.txt
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)       38 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/setup.cfg
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     6821 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/setup.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1428 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisf1.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     2424 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/Lisflood_EnKF.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11348 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/src/lisflood/Lisflood_dynamic.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    17756 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/src/lisflood/Lisflood_initial.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1450 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/Lisflood_monteCarlo.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      682 2023-06-22 12:01:40.000000 lisflood-model-4.1.3/src/lisflood/__init__.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood/global_modules/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/global_modules/__init__.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    37709 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/src/lisflood/global_modules/add1.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     4396 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/global_modules/checkers.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3027 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/global_modules/decorators.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)   131047 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/src/lisflood/global_modules/default_options.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1554 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/global_modules/errors.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    23273 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/src/lisflood/global_modules/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    17563 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/global_modules/output.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    30562 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/src/lisflood/global_modules/settings.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     6153 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/global_modules/stateVar.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    17146 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/global_modules/zusatz.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     2739 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/__init__.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1130 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/compile_kinematic_wave_parallel_tools.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7696 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/evapowater.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4460 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/frost.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8170 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/groundwater.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    16483 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/indicatorcalc.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     6044 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/inflow.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    11427 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/kinematic_wave_parallel.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)   882792 2023-05-17 13:08:31.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.c
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     8133 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    15667 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/lakes.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    10358 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/landusechange.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4128 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/leafarea.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7709 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/miscInitial.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3335 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/opensealed.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     7610 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/polder.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3996 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/readmeteo.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    19690 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/reservoir.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    10610 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/riceirrigation.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    41378 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/routing.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     9644 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/snow.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    30635 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/soil.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    50345 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/soilloop.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     2946 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/structures.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    13122 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/surface_routing.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3763 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/transmission.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    57847 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/waterabstraction.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)    17140 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/waterbalance.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     3334 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/waterlevel.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     1620 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisflood/hydrological_modules/wateruse.py
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)     8475 2023-06-22 11:42:12.000000 lisflood-model-4.1.3/src/lisflood/main.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)   143665 2023-04-26 16:22:09.000000 lisflood-model-4.1.3/src/lisfloodSettings_reference.xml
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood_model.egg-info/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8729 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood_model.egg-info/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2497 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood_model.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood_model.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      639 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood_model.egg-info/requires.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       15 2023-06-22 12:04:02.000000 lisflood-model-4.1.3/src/lisflood_model.egg-info/top_level.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-06-22 11:43:42.000000 lisflood-model-4.1.3/src/lisflood_model.egg-info/zip-safe
```

### Comparing `lisflood-model-4.1.2/LICENSE` & `lisflood-model-4.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/PKG-INFO` & `lisflood-model-4.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lisflood-model
-Version: 4.1.2
+Version: 4.1.3
 Summary: LISFLOOD model python module
 Home-page: https://github.com/ec-jrc/lisflood-code
-Download-URL: https://github.com/ec-jrc/lisflood-code/archive/4.1.2.tar.gz
+Download-URL: https://github.com/ec-jrc/lisflood-code/archive/4.1.3.tar.gz
 Author: Ad de Roo, Emiliano Gelati, Peter Burek, Johan van der Knijff, Niko Wanders
 Author-email: carlo.russo@ext.ec.europa.eu
 License: EUPL 1.2
 Keywords: lisflood,lisvap,efas,glofas,copernicus,ecmwf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `lisflood-model-4.1.2/README.md` & `lisflood-model-4.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/bin/lisflood` & `lisflood-model-4.1.3/bin/lisflood`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/requirements.txt` & `lisflood-model-4.1.3/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 more-itertools>=7.2.0
 netCDF4>=1.5.3
 nine>=1.0.0
 numba>=0.54.0
 numexpr>=2.7.0
 numpy>=1.21.0
 packaging>=19.2
-pandas>=0.25.1
+pandas>=1
 pathlib2>=2.3.5
 pkginfo>=1.5.0.1
 pluggy>=0.13.0
 py>=1.10.0
 pyparsing>=2.4.2
 pyproj>=2.4.0
 pytest>=6.2.5
```

### Comparing `lisflood-model-4.1.2/setup.py` & `lisflood-model-4.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisf1.py` & `lisflood-model-4.1.3/src/lisf1.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/Lisflood_EnKF.py` & `lisflood-model-4.1.3/src/lisflood/Lisflood_EnKF.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/Lisflood_dynamic.py` & `lisflood-model-4.1.3/src/lisflood/Lisflood_dynamic.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         # debug 
         # Print value of variables after computation (from state files)
         if flags['debug']:
             nomefile = 'Debug_out_'+str(self.currentStep)+'.txt'
             ftemp1 = open(nomefile, 'w+')
             nelements = len(self.ChanM3)
             for i in range(0,nelements-1):
-                if  hasattr(self,'CrossSection2Area'):
+                if  hasattr(self,'CrossSection2Area') and not(option['InitLisflood']):
                     print(i, self.TotalCrossSectionArea[i], self.CrossSection2Area[i], self.ChanM3[i], \
                     self.Chan2M3Kin[i], file=ftemp1)
                 else:
                     print(i, self.TotalCrossSectionArea[i], self.ChanM3[i], file=ftemp1)
             ftemp1.close()
 
         ### Report states if EnKF is used and filter moment
```

### Comparing `lisflood-model-4.1.2/src/lisflood/Lisflood_initial.py` & `lisflood-model-4.1.3/src/lisflood/Lisflood_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         # debug start
         if flags['debug']:
             # Print value of variables after initialization (from state files)
             nomefile = 'Debug_init_' + str(self.currentStep + 1) + '.txt'
             ftemp1 = open(nomefile, 'w+')
             nelements = len(self.ChanM3)
             for i in range(0, nelements - 1):
-                if hasattr(self, 'CrossSection2Area'):
+                if hasattr(self, 'CrossSection2Area') and not(option['InitLisflood']):
                     print(i, self.TotalCrossSectionArea[i], self.CrossSection2Area[i], self.ChanM3[i], self.Chan2M3Kin[i], file=ftemp1)
                 else:
                     print(i, self.TotalCrossSectionArea[i], self.ChanM3[i], file=ftemp1)
 
             ftemp1.close()
 
 # ====== INITIAL ================================
```

### Comparing `lisflood-model-4.1.2/src/lisflood/Lisflood_monteCarlo.py` & `lisflood-model-4.1.3/src/lisflood/Lisflood_monteCarlo.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/__init__.py` & `lisflood-model-4.1.3/src/lisflood/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,11 +6,11 @@
     version_file = os.path.join(current_dir, '../../../../VERSION')
 
 with open(version_file, 'r') as f:
     version = f.read().strip()
 
 __version__ = version
 __authors__ = "Ad de Roo, Emiliano Gelati, Peter Burek, Johan van der Knijff, Niko Wanders"
-__date__ = "22/03/2023"
+__date__ = "22/06/2023"
 __copyright__ = "Copyright 2019-2023, European Commission - Joint Research Centre"
 __maintainer__ = "Stefania Grimaldi, Cinzia Mazzetti, Carlo Russo, Damien Decremer, Corentin Carton De Wiart, Valerio Lorini, Ad de Roo"
 __status__ = "Operation"
```

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/add1.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/add1.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,29 +200,30 @@
         except Exception as e:
             # FIXME manage exceptions and print type of error
             # print(str(e))
             # print(type(e))
             # try to read a netcdf file
             filename = os.path.splitext(binding[name])[0] + '.nc'
             nf1 = iterOpenNetcdf(filename, "", "r")
-            value = listitems(nf1.variables)[-1][0]  # get the last variable name
-            nr_rows, nr_cols = nf1.variables[value].shape  # just use shape to know rows and cols...
+            num_dims = 3 if 'time' in nf1.variables else 2
+            varname = [v for v in nf1.variables if len(nf1.variables[v].dimensions) == num_dims][0]
+            nr_rows, nr_cols = nf1.variables[varname].shape  # just use shape to know rows and cols...
             if 'x' in nf1.variables:
                 x1 = nf1.variables['x'][0]
                 x2 = nf1.variables['x'][-1]
                 y1 = nf1.variables['y'][0]
             else:
                 x1 = nf1.variables['lon'][0]
                 x2 = nf1.variables['lon'][-1]
                 y1 = nf1.variables['lat'][0]
 
             cell_size = np.abs(x2 - x1)/(nr_cols - 1)
             x = x1 - cell_size / 2
             y = y1 + cell_size / 2
-            mapnp = np.array(nf1.variables[value][0:nr_rows, 0:nr_cols])
+            mapnp = np.array(nf1.variables[varname][0:nr_rows, 0:nr_cols])
             nf1.close()
             # setclone  row col cellsize xupleft yupleft
             setclone(nr_rows, nr_cols, cell_size, x, y)
             map_out = numpy2pcr(Boolean, mapnp, 0)
             flagmap = True
 
         if flags['checkfiles']:
```

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/checkers.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/checkers.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/decorators.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/decorators.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/default_options.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/default_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -893,134 +893,134 @@
                                                    yearly=False),                                                   
                        'TaMaps': ReportedMap(name='TaMaps', output_var='TaPixel', unit='mm', end=[],
                                              steps=[], all=['repE2O1','repTaMaps'], restrictoption=['nonInit'],
                                              monthly=False, yearly=False),
                        'TavgMapsOut': ReportedMap(name='TavgMapsOut', output_var='Tavg', unit='degree',
                                                   end=[], steps=[], all=['repTavgMaps'],
                                                   restrictoption=[], monthly=False, yearly=False),
-                       'Theta1End': ReportedMap(name='Theta1End', output_var='Theta1a[0]', unit='mm',
+                       'Theta1End': ReportedMap(name='Theta1End', output_var='Theta1a[0]', unit='',
                                                 end=['repEndMaps'], steps=[], all=[],
                                                 restrictoption=[], monthly=False, yearly=False),
                        'Theta1ForestEnd': ReportedMap(name='Theta1ForestEnd', output_var='Theta1a[1]',
-                                                      unit='mm', end=['repEndMaps'], steps=[],
+                                                      unit='', end=['repEndMaps'], steps=[],
                                                       all=[], restrictoption=[],
                                                       monthly=False, yearly=False),
                        'Theta1ForestMaps': ReportedMap(name='Theta1ForestMaps', output_var='Theta1a[1]',
-                                                       unit='mm', end=[], steps=[],
+                                                       unit='', end=[], steps=[],
                                                        all=['repThetaForestMaps','repThetaMaps'],
                                                        restrictoption=['nonInit'], monthly=False,
                                                        yearly=False),
                        'Theta1ForestState': ReportedMap(name='Theta1ForestState',
-                                                        output_var='Theta1a[1]', unit='mm', end=[],
+                                                        output_var='Theta1a[1]', unit='', end=[],
                                                         steps=['repStateMaps'], all=[],
                                                         restrictoption=['nonInit'], monthly=False,
                                                         yearly=False),
                        'Theta1IrrigationEnd': ReportedMap(name='Theta1IrrigationEnd',
-                                                          output_var='Theta1a[2]', unit='mm',
+                                                          output_var='Theta1a[2]', unit='',
                                                           end=['repEndMaps'], steps=[], all=[],
                                                           restrictoption=[], monthly=False,
                                                           yearly=False),
                        'Theta1IrrigationMaps': ReportedMap(name='Theta1IrrigationMaps',
-                                                           output_var='Theta1a[2]', unit='mm',
+                                                           output_var='Theta1a[2]', unit='',
                                                            end=[], steps=[],
                                                            all=['repThetaIrrigationMaps','repThetaMaps'],
                                                            restrictoption=['nonInit'], monthly=False,
                                                            yearly=False),
                        'Theta1IrrigationState': ReportedMap(name='Theta1IrrigationState',
-                                                            output_var='Theta1a[2]', unit='mm',
+                                                            output_var='Theta1a[2]', unit='',
                                                             end=[], steps=['repStateMaps'], all=[],
                                                             restrictoption=['nonInit'], monthly=False,
                                                             yearly=False),
-                       'Theta1Maps': ReportedMap(name='Theta1Maps', output_var='Theta1a[0]', unit='mm',
+                       'Theta1Maps': ReportedMap(name='Theta1Maps', output_var='Theta1a[0]', unit='',
                                                  end=[], steps=[], all=['repThetaMaps','repE2O2'],
                                                  restrictoption=['nonInit'], monthly=False,
                                                  yearly=False),
                        'Theta1State': ReportedMap(name='Theta1State', output_var='Theta1a[0]',
-                                                  unit='mm', end=[], steps=['repStateMaps'],
+                                                  unit='', end=[], steps=['repStateMaps'],
                                                   all=[], restrictoption=['nonInit'], monthly=False,
                                                   yearly=False),
-                       'Theta2End': ReportedMap(name='Theta2End', output_var='Theta1b[0]', unit='mm',
+                       'Theta2End': ReportedMap(name='Theta2End', output_var='Theta1b[0]', unit='',
                                                 end=['repEndMaps'], steps=[], all=[],
                                                 restrictoption=[], monthly=False, yearly=False),
                        'Theta2ForestEnd': ReportedMap(name='Theta2ForestEnd', output_var='Theta1b[1]',
-                                                      unit='mm', end=['repEndMaps'], steps=[],
+                                                      unit='', end=['repEndMaps'], steps=[],
                                                       all=[], restrictoption=[],
                                                       monthly=False, yearly=False),
                        'Theta2ForestMaps': ReportedMap(name='Theta2ForestMaps', output_var='Theta1b[1]',
-                                                       unit='mm', end=[], steps=[],
+                                                       unit='', end=[], steps=[],
                                                        all=['repThetaForestMaps','repThetaMaps'],
                                                        restrictoption=['nonInit'], monthly=False,
                                                        yearly=False),
                        'Theta2ForestState': ReportedMap(name='Theta2ForestState',
-                                                        output_var='Theta1b[1]', unit='mm', end=[],
+                                                        output_var='Theta1b[1]', unit='', end=[],
                                                         steps=['repStateMaps'], all=[],
                                                         restrictoption=['nonInit'], monthly=False,
                                                         yearly=False),
                        'Theta2IrrigationEnd': ReportedMap(name='Theta2IrrigationEnd',
-                                                          output_var='Theta1b[2]', unit='mm',
+                                                          output_var='Theta1b[2]', unit='',
                                                           end=['repEndMaps'], steps=[], all=[],
                                                           restrictoption=[], monthly=False,
                                                           yearly=False),
                        'Theta2IrrigationMaps': ReportedMap(name='Theta2IrrigationMaps',
-                                                           output_var='Theta1b[2]', unit='mm',
+                                                           output_var='Theta1b[2]', unit='',
                                                            end=[], steps=[],
                                                            all=['repThetaIrrigationMaps','repThetaMaps'],
                                                            restrictoption=['nonInit'], monthly=False,
                                                            yearly=False),
                        'Theta2IrrigationState': ReportedMap(name='Theta2IrrigationState',
-                                                            output_var='Theta1b[2]', unit='mm',
+                                                            output_var='Theta1b[2]', unit='',
                                                             end=[], steps=['repStateMaps'], all=[],
                                                             restrictoption=['nonInit'], monthly=False,
                                                             yearly=False),
-                       'Theta2Maps': ReportedMap(name='Theta2Maps', output_var='Theta1b[0]', unit='mm',
+                       'Theta2Maps': ReportedMap(name='Theta2Maps', output_var='Theta1b[0]', unit='',
                                                  end=[], steps=[], all=['repThetaMaps','repE2O2'],
                                                  restrictoption=['nonInit'], monthly=False,
                                                  yearly=False),
                        'Theta2State': ReportedMap(name='Theta2State', output_var='Theta1b[0]',
-                                                  unit='mm', end=[], steps=['repStateMaps'],
+                                                  unit='', end=[], steps=['repStateMaps'],
                                                   all=[], restrictoption=['nonInit'], monthly=False,
                                                   yearly=False),
-                       'Theta3End': ReportedMap(name='Theta3End', output_var='Theta2[0]', unit='mm',
+                       'Theta3End': ReportedMap(name='Theta3End', output_var='Theta2[0]', unit='',
                                                 end=['repEndMaps'], steps=[], all=[],
                                                 restrictoption=[], monthly=False, yearly=False),
                        'Theta3ForestEnd': ReportedMap(name='Theta3ForestEnd', output_var='Theta2[1]',
-                                                      unit='mm', end=['repEndMaps'], steps=[],
+                                                      unit='', end=['repEndMaps'], steps=[],
                                                       all=[], restrictoption=[],
                                                       monthly=False, yearly=False),
                        'Theta3ForestMaps': ReportedMap(name='Theta3ForestMaps', output_var='Theta2[1]',
-                                                       unit='mm', end=[], steps=[],
+                                                       unit='', end=[], steps=[],
                                                        all=['repThetaForestMaps','repThetaMaps'],
                                                        restrictoption=['nonInit'], monthly=False,
                                                        yearly=False),
                        'Theta3ForestState': ReportedMap(name='Theta3ForestState',
-                                                        output_var='Theta2[1]', unit='mm', end=[],
+                                                        output_var='Theta2[1]', unit='', end=[],
                                                         steps=['repStateMaps'], all=[],
                                                         restrictoption=['nonInit'], monthly=False,
                                                         yearly=False),
                        'Theta3IrrigationEnd': ReportedMap(name='Theta3IrrigationEnd',
-                                                          output_var='Theta2[2]', unit='mm',
+                                                          output_var='Theta2[2]', unit='',
                                                           end=['repEndMaps'], steps=[], all=[],
                                                           restrictoption=[], monthly=False,
                                                           yearly=False),
                        'Theta3IrrigationMaps': ReportedMap(name='Theta3IrrigationMaps',
-                                                           output_var='Theta2[2]', unit='mm', end=[],
+                                                           output_var='Theta2[2]', unit='', end=[],
                                                            steps=[], all=['repThetaIrrigationMaps','repThetaMaps'],
                                                            restrictoption=['nonInit'], monthly=False,
                                                            yearly=False),
                        'Theta3IrrigationState': ReportedMap(name='Theta3IrrigationState',
-                                                            output_var='Theta2[2]', unit='mm',
+                                                            output_var='Theta2[2]', unit='',
                                                             end=[], steps=['repStateMaps'], all=[],
                                                             restrictoption=['nonInit'], monthly=False,
                                                             yearly=False),
-                       'Theta3Maps': ReportedMap(name='Theta3Maps', output_var='Theta2[0]', unit='mm',
+                       'Theta3Maps': ReportedMap(name='Theta3Maps', output_var='Theta2[0]', unit='',
                                                  end=[], steps=[], all=['repThetaMaps','repE2O2'],
                                                  restrictoption=['nonInit'], monthly=False,
                                                  yearly=False),
                        'Theta3State': ReportedMap(name='Theta3State', output_var='Theta2[0]',
-                                                  unit='mm', end=[], steps=['repStateMaps'],
+                                                  unit='', end=[], steps=['repStateMaps'],
                                                   all=[], restrictoption=['nonInit'], monthly=False,
                                                   yearly=False),
                        'TotalAbsGroundwater': ReportedMap(name='TotalAbsGroundwater',
                                                           output_var='abstraction_GW_actual_M3*self.var.M3toMM',
                                                           unit='mm', end=[], steps=['repTotalAbs'],
                                                           all=[],
                                                           restrictoption=['nonInit', 'wateruse'],
```

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/errors.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/errors.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/netcdf.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/netcdf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import glob
+import warnings
 import xarray as xr
 import numpy as np
 import datetime
 import pcraster
 from netCDF4 import num2date, date2num
 import time as xtime
 from nine import range
@@ -12,38 +13,53 @@
 from .settings import (calendar_inconsistency_warning, get_calendar_type, calendar, MaskAttrs, CutMap, NetCDFMetadata,
                        get_core_dims, LisSettings, MaskInfo)
 from .errors import LisfloodWarning, LisfloodError
 from .decorators import Cache, cached
 from .zusatz import iterOpenNetcdf
 # from .add1 import *
 from .add1 import nanCheckMap, decompress
+from netCDF4 import default_fillvals
 
 
-def mask_array_np(data, mask, crop):
+def mask_array_np(data, mask, crop, name, valid_min, valid_max):
     data_cut = data[:, crop[2]:crop[3], crop[0]:crop[1]]
+    if (valid_min is not None):
+        if (data_cut < valid_min).sum() > 0:
+            warnings.warn(LisfloodWarning('Data in var "{}" contains values out of valid range (valid_min)'.format(name)))
+            if np.issubdtype(data.dtype, np.floating):
+                data_cut[(data_cut < valid_min)] = np.nan
+            else:
+                data_cut[(data_cut < valid_min)] = default_fillvals[data_cut.dtype.str[1:]]
+    if (valid_max is not None):
+        if (data_cut > valid_max).sum() > 0:
+            warnings.warn(LisfloodWarning('Data in var "{}" contains values out of valid range (valid_max)'.format(name)))
+            if np.issubdtype(data.dtype, np.floating):
+                data_cut[(data_cut > valid_max)] = np.nan
+            else:
+                data_cut[(data_cut > valid_max)] = default_fillvals[data_cut.dtype.str[1:]]
     return data_cut[:, mask]
 
 
 
-def mask_array(data, mask, crop, core_dims):
+def mask_array(data, mask, crop, core_dims, name, valid_min, valid_max):
     n_data = int(mask.sum())
     masked_data = xr.apply_ufunc(mask_array_np, data,
                                  dask='parallelized',
                                  input_core_dims=[core_dims],
                                  exclude_dims=set(core_dims),
                                  output_dtypes=[data.dtype],
                                  output_core_dims=[['z']],
                                  dask_gufunc_kwargs = dict(output_sizes={'z': n_data}),
-                                 kwargs={'mask': mask, 'crop': crop})
+                                 kwargs={'mask': mask, 'crop': crop, 'name': name, 'valid_min': valid_min, 'valid_max': valid_max})
     return masked_data
 
 
-def compress_xarray(mask, crop, data):
+def compress_xarray(mask, crop, data, name, valid_min, valid_max):
     core_dims = get_core_dims(data.dims)
-    masked_data = mask_array(data, mask, crop, core_dims=core_dims)
+    masked_data = mask_array(data, mask, crop, core_dims=core_dims, name=name, valid_min=valid_min, valid_max=valid_max)
     return masked_data
 
 
 def uncompress_array(masked_data):
     maskinfo = MaskInfo.instance()
     data = maskinfo.info.maskall.copy()
     data[~maskinfo.info.maskflat] = masked_data[:]
@@ -150,15 +166,16 @@
 
     def __init__(self, data_path, time_chunk, dates, indexer=None, climatology=False):
 
         # load dataset using xarray
         if time_chunk != 'auto' and time_chunk is not None:
             time_chunk = int(time_chunk)
         data_path = data_path + ".nc" if not data_path.endswith('.nc') else data_path
-        ds = xr.open_mfdataset(data_path, engine='netcdf4', chunks={'time': time_chunk}, combine='by_coords')
+        ds = xr.open_mfdataset(data_path, engine='netcdf4', chunks={'time': time_chunk}, combine='by_coords',
+                               mask_and_scale=True)
 
         # check calendar type
         check_dataset_calendar_type(ds, data_path)
 
         # extract main variable
         var_name = find_main_var(ds, data_path)
         da = ds[var_name]
@@ -170,15 +187,26 @@
         self.index_map = map_dates_index(dates, da.time, indexer, climatology)
 
         # compress dataset (remove missing values and flatten the array)
         maskinfo = MaskInfo.instance()
         mask = np.logical_not(maskinfo.info.mask)
         cutmap = CutMap.instance()
         crop = cutmap.cuts
-        self.dataset = compress_xarray(mask, crop, da) # final dataset to store
+
+        # in case the dataset contains valid_min and valid_max set, store here the scaled adn offset values of them
+        scale_factor=da.encoding['scale_factor'] if 'scale_factor' in da.encoding else 1
+        add_offset=da.encoding['add_offset'] if 'add_offset' in da.encoding else 0
+        valid_min_scaled = None
+        valid_max_scaled = None
+        settings = LisSettings.instance()
+        flags = settings.flags
+        if not flags['skipvalreplace']:
+            valid_min_scaled = (da.attrs['valid_min']*scale_factor+add_offset) if 'valid_min' in da.attrs else None
+            valid_max_scaled = (da.attrs['valid_max']*scale_factor+add_offset) if 'valid_max' in da.attrs else None
+        self.dataset = compress_xarray(mask, crop, da, var_name, valid_min_scaled, valid_max_scaled) # final dataset to store
 
         # initialise class variables and load first chunk
         self.init_chunks(self.dataset, time_chunk)
 
     def init_chunks(self, dataset, time_chunk):
         # compute chunks indexes in dataset
         chunks = self.dataset.chunks[0]  # list of chunks indexes in dataset
@@ -209,17 +237,26 @@
         if dataset_index == self.chunk_indexes[self.ichunk+1]:
             self.load_next_chunk()
 
         local_index = dataset_index - self.chunk_indexes[self.ichunk]
 
         if local_index < 0:
             msg = 'local step cannot be negative! step: {}, chunk: {} - {}', local_index, self.chunk_index[self.ichunk], self.chunk_index[self.ichunk+1]
-            LisfloodError(msg)
+            raise LisfloodError(msg)
 
         data = self.dataset_chunk.values[local_index]
+        if np.issubdtype(data.dtype, np.floating):
+            if (np.isnan(data).any()):
+                #warnings.warn(LisfloodWarning('Data in var "{}" contains NaN values or values out of valid range inside mask map for step: {}'.format(self.dataset.name,local_index)))
+                raise LisfloodError('Data in var "{}" contains NaN values or values out of valid range inside mask map for step: {}'.format(self.dataset.name,local_index))
+        else:
+            if (data==default_fillvals[data.dtype.str[1:]]).any():
+                #warnings.warn(LisfloodWarning('Data in var "{}" contains NaN values or values out of valid range inside mask map for step: {}'.format(self.dataset.name,local_index)))
+                raise LisfloodError('Data in var "{}" contains missing values or values out of valid range inside mask map for step: {}'.format(self.dataset.name,local_index))
+
         return data
 
 
 @Cache
 class XarrayCached(XarrayChunked):
 
     def __init__(self, data_path, dates, indexer=None, climatology=False):
```

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/output.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/output.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/settings.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from collections import namedtuple
 import multiprocessing
 import cftime
 import threading
 import xml.dom.minidom
 import pcraster
 from netCDF4 import Dataset, date2num, num2date
-from pandas.core.tools.datetimes import parsing
+from pandas import to_datetime
 import numpy as np
 
 from .errors import LisfloodError, LisfloodWarning, LisfloodFileError
 from .decorators import cached
 from .default_options import default_options
 
 
@@ -193,15 +193,15 @@
 def get_core_dims(dims):
     if 'x' in dims and 'y' in dims:
         core_dims = ('y', 'x')
     elif 'lat' in dims and 'lon' in dims:
         core_dims = ('lat', 'lon')
     else:
         msg = 'Core dimension in netcdf file not recognised! Expecting (y, x) or (lat, lon), have '+str(dims)
-        LisfloodError(msg)
+        raise LisfloodError(msg)
     return core_dims
 
 
 @nine
 class NetCDFMetadata(with_metaclass(Singleton)):
     def __init__(self, uid):
         from .zusatz import iterOpenNetcdf
@@ -327,15 +327,15 @@
         return enkf_set, mc_set
 
     def _check_timestep_init(self):
         try:
             float(self.timestep_init)
         except ValueError:
             try:
-                parsing.parse_time_string(self.timestep_init, dayfirst=True)
+                to_datetime(self.timestep_init, dayfirst=True).to_pydatetime()
             except ValueError:
                 raise LisfloodError('Option timestepInit was not parsable. Must be integer or date string: {}'.format(self.timestep_init))
             else:
                 return True
         else:
             return True
 
@@ -407,30 +407,31 @@
         # CM: output folder
         return pathout
 
     @staticmethod
     def _flags(sys_args):
         flags = OrderedDict([('quiet', False), ('veryquiet', False), ('loud', False),
                              ('checkfiles', False), ('noheader', False), ('printtime', False),
-                             ('debug', False), ('nancheck', False), ('initonly', False)])
+                             ('debug', False), ('nancheck', False), ('initonly', False),
+                             ('skipvalreplace', False)])
 
         @cached
         def _flags(argz):
             try:
-                opts, arguments = getopt.getopt(argz, 'qvlchtdni', list(flags.keys()))
+                opts, arguments = getopt.getopt(argz, 'qvlchtdnis', list(flags.keys()))
             except getopt.GetoptError:
                 from ..main import usage
                 usage()
             else:
                 for o, a in opts:
                     for opt in (('-q', '--quiet'), ('-v', '--veryquiet'),
                                 ('-l', '--loud'), ('-c', '--checkfiles'),
                                 ('-h', '--noheader'), ('-t', '--printtime'),
                                 ('-d', '--debug'), ('-n', '--nancheck'),
-                                ('-i', '--initonly')):
+                                ('-i', '--initonly'), ('-s', '--skipvalreplace')):
                         if o in opt:
                             flags[opt[1].lstrip('--')] = True
                             break
             return flags
 
         return _flags(sys_args)
 
@@ -612,15 +613,15 @@
     try:
         # try reading step number from number or string
         return float(date_in)
     except ValueError:
         # try reading a date in one of available formats
         try:
             _t_units = "hours since 1970-01-01 00:00:00"  # units used for date type conversion (datetime.datetime -> calendar-specific if needed)
-            date = parsing.parse_time_string(date_in, dayfirst=True)[0]  # datetime.datetime type
+            date = to_datetime(date_in, dayfirst=True).to_pydatetime() # datetime.datetime type
             step = date2num(date, _t_units, calendar_type)  # float type
             return num2date(step, _t_units, calendar_type)  # calendar-dependent type from netCDF4.netcdftime._netcdftime module
         except:
             # if cannot read input then stop
             msg = "Wrong step or date format in XML settings file\n Input {}".format(date_in)
             raise LisfloodError(msg)
```

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/stateVar.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/stateVar.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/global_modules/zusatz.py` & `lisflood-model-4.1.3/src/lisflood/global_modules/zusatz.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/__init__.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/compile_kinematic_wave_parallel_tools.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/compile_kinematic_wave_parallel_tools.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/evapowater.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/evapowater.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/frost.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/frost.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/groundwater.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/groundwater.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/indicatorcalc.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/indicatorcalc.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/inflow.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/inflow.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/kinematic_wave_parallel.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/kinematic_wave_parallel.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.c` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.30 */
+/* Generated by Cython 0.29.14 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-O3",
@@ -17,25 +17,23 @@
             "src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx"
         ]
     },
     "module_name": "lisflood.hydrological_modules.kinematic_wave_parallel_tools"
 }
 END: Cython Metadata */
 
-#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
-#endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_30"
-#define CYTHON_HEX_VERSION 0x001D1EF0
+#define CYTHON_ABI "0_29_14"
+#define CYTHON_HEX_VERSION 0x001D0EF0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,17 +100,14 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
-  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
@@ -146,17 +141,14 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
@@ -180,64 +172,53 @@
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
+  #if PY_VERSION_HEX < 0x030300F0
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_FAST_THREAD_STATE
-    #define CYTHON_FAST_THREAD_STATE 0
-  #elif !defined(CYTHON_FAST_THREAD_STATE)
+  #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
+    #define CYTHON_FAST_PYCALL 1
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #if PY_VERSION_HEX >= 0x030B00A4
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
+  #ifndef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
-  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_MAJOR_VERSION < 3
-    #include "longintrepr.h"
-  #endif
+  #include "longintrepr.h"
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -346,76 +327,17 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-  #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
-                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
-                                                    PyObject *fv, PyObject *cell, PyObject* fn,
-                                                    PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject* co=NULL;
-        PyObject *type, *value, *traceback;
-        PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
-        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
-        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
-        Py_XDECREF((PyObject*)co);
-        co = (PyCodeObject*)call_result;
-        call_result = NULL;
-        if (0) {
-            cleanup_code_too:
-            Py_XDECREF((PyObject*)co);
-            co = NULL;
-        }
-        end:
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(call_result);
-        Py_XDECREF(empty);
-        if (type) {
-            PyErr_Restore(type, value, traceback);
-        }
-        return co;
-    }
+#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -521,36 +443,24 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
   #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
                                               0 : _PyUnicode_Ready((PyObject *)(op)))
-  #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
-  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
-  #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
@@ -591,35 +501,26 @@
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBaseString_Type            PyUnicode_Type
   #define PyStringObject               PyUnicodeObject
   #define PyString_Type                PyUnicode_Type
   #define PyString_Check               PyUnicode_Check
   #define PyString_CheckExact          PyUnicode_CheckExact
-#ifndef PyObject_Unicode
   #define PyObject_Unicode             PyObject_Str
 #endif
-#endif
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
 #ifndef PySet_CheckExact
   #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
-#if PY_VERSION_HEX >= 0x030900A4
-  #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
-  #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
-#else
-  #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
-  #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
-#endif
 #if CYTHON_ASSUME_SAFE_MACROS
   #define __Pyx_PySequence_SIZE(seq)  Py_SIZE(seq)
 #else
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
@@ -645,21 +546,21 @@
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
 #endif
 #if PY_MAJOR_VERSION >= 3
-  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? PyMethod_New(func, self) : (Py_INCREF(func), func))
 #else
   #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
@@ -673,18 +574,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -694,18 +593,19 @@
 #endif
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
-#define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+
 #define __PYX_ERR(f_index, lineno, Ln_error) \
-    { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
+{ \
+  __pyx_filename = __pyx_f[f_index]; __pyx_lineno = lineno; __pyx_clineno = __LINE__; goto Ln_error; \
+}
 
 #ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
@@ -812,15 +712,14 @@
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
@@ -1341,29 +1240,21 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
-#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
@@ -1444,15 +1335,15 @@
 /* StrEquals.proto */
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
 #else
 #define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
 #endif
 
-/* DivInt[Py_ssize_t].proto */
+/* None.proto */
 static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t, Py_ssize_t);
 
 /* UnaryNegOverflows.proto */
 #define UNARY_NEG_WOULD_OVERFLOW(x)\
         (((x) < 0) & ((unsigned long)(x) == 0-(unsigned long)(x)))
 
 static CYTHON_UNUSED int __pyx_array_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
@@ -1585,15 +1476,15 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len)) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
+        Py_SIZE(list) = len+1;
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
@@ -1623,35 +1514,29 @@
 #if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
 static CYTHON_INLINE int __Pyx_PyList_Append(PyObject* list, PyObject* x) {
     PyListObject* L = (PyListObject*) list;
     Py_ssize_t len = Py_SIZE(list);
     if (likely(L->allocated > len) & likely(len > (L->allocated >> 1))) {
         Py_INCREF(x);
         PyList_SET_ITEM(list, len, x);
-        __Pyx_SET_SIZE(list, len + 1);
+        Py_SIZE(list) = len+1;
         return 0;
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
-/* DivInt[long].proto */
+/* None.proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
-
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
 /* PyObject_GenericGetAttrNoDict.proto */
@@ -1667,17 +1552,14 @@
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
 static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
@@ -1765,28 +1647,29 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_long(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_long(PyObject *, int writable_flag);
 
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_unsigned_char(PyObject *, int writable_flag);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_long(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_long(const char *itemp, PyObject *obj);
 
-/* ObjectToMemviewSlice.proto */
-static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_int(PyObject *, int writable_flag);
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value);
+
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_char(unsigned char value);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj);
 
 /* MemviewSliceCopyTemplate.proto */
 static __Pyx_memviewslice
@@ -1794,32 +1677,26 @@
                                  const char *mode, int ndim,
                                  size_t sizeof_dtype, int contig_flag,
                                  int dtype_is_object);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value);
-
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_char(unsigned char value);
-
-/* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_int(PyObject *, int writable_flag);
+
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
@@ -2034,15 +1911,15 @@
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_Copyright_2019_European_Union_L[] = "\n\nCopyright 2019 European Union\n\nLicensed under the EUPL, Version 1.2 or as soon they will be approved by the European Commission  subsequent versions of the EUPL (the \"Licence\");\n\nYou may not use this work except in compliance with the Licence.\nYou may obtain a copy of the Licence at:\n\nhttps://joinup.ec.europa.eu/sites/default/files/inline-files/EUPL%20v1_2%20EN(1).txt\n\nUnless required by applicable law or agreed to in writing, software distributed under the Licence is distributed on an \"AS IS\" basis,\nWITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.\nSee the Licence for the specific language governing permissions and limitations under the Licence.\n\nCollection of functions called by the Python module kinematic_wave_parallel.py. These functions are\nimplemented in Cython to achieve compiled-code performance when executing loops over numpy arrays.\nTo compile this Cython module to enable OpenMP multithreading, execute:\n$ python compile_kinematic_wave_parallel_tools.py build_ext --inplace\nImportant: the module has to be compiled on the machine where the model is run - the resulting binary is not portable.\n";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
 static const char __pyx_k_Empty_shape_tuple_for_cython_arr[] = "Empty shape tuple for cython.array";
-static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))";
+static const char __pyx_k_Incompatible_checksums_s_vs_0xb0[] = "Incompatible checksums (%s vs 0xb068931 = (name))";
 static const char __pyx_k_Indirect_dimensions_not_supporte[] = "Indirect dimensions not supported";
 static const char __pyx_k_Invalid_mode_expected_c_or_fortr[] = "Invalid mode, expected 'c' or 'fortran', got %s";
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_lisflood_hydrological_modules_ki[] = "lisflood.hydrological_modules.kinematic_wave_parallel_tools";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
@@ -2055,15 +1932,15 @@
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Emiliano_Gelati;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
-static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
+static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xb0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
@@ -2244,16 +2121,14 @@
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_8;
-static PyObject *__pyx_int_112105877;
-static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
@@ -2267,29 +2142,28 @@
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
 static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_tuple__33;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
-static PyObject *__pyx_codeobj__27;
-static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
+static PyObject *__pyx_codeobj__33;
 /* Late includes */
 
 /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":45
  * @boundscheck(False)
  * @wraparound(False)
  * def kinematicRouting(double[::1] discharge, double[::1] lateral_inflow, double[::1] constant, long[:,::1] upstream_lookup,\             # <<<<<<<<<<<<<<
  *                      long[::1] num_upstream_pixels, long[::1] ordered_pixels, long[:,::1] start_stop, double beta, double inv_beta,\
@@ -2309,17 +2183,14 @@
   __Pyx_memviewslice __pyx_v_start_stop = { 0, 0, { 0 }, { 0 }, { 0 } };
   double __pyx_v_beta;
   double __pyx_v_inv_beta;
   double __pyx_v_b_minus_1;
   __Pyx_memviewslice __pyx_v_a_dx_div_dt = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_b_a_dx_div_dt = { 0, 0, { 0 }, { 0 }, { 0 } };
   CYTHON_UNUSED long __pyx_v_num_threads;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("kinematicRouting (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_discharge,&__pyx_n_s_lateral_inflow,&__pyx_n_s_constant,&__pyx_n_s_upstream_lookup,&__pyx_n_s_num_upstream_pixels,&__pyx_n_s_ordered_pixels,&__pyx_n_s_start_stop,&__pyx_n_s_beta,&__pyx_n_s_inv_beta,&__pyx_n_s_b_minus_1,&__pyx_n_s_a_dx_div_dt,&__pyx_n_s_b_a_dx_div_dt,&__pyx_n_s_num_threads,0};
     PyObject* values[13] = {0,0,0,0,0,0,0,0,0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -2491,18 +2362,21 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   long __pyx_t_1;
   long __pyx_t_2;
   long __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   Py_ssize_t __pyx_t_5;
-  long __pyx_t_6;
-  long __pyx_t_7;
+  Py_ssize_t __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
   long __pyx_t_8;
   long __pyx_t_9;
+  long __pyx_t_10;
+  long __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
   __Pyx_RefNannySetupContext("kinematicRouting", 0);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":50
  *     """"""
  *     cdef:
  *         long order, index, first, last, num_orders = start_stop.shape[0]             # <<<<<<<<<<<<<<
  *     # Iterate through routing orders (sets of pixels for which the kinemativc wave can be solved independently and thus in parallel)
@@ -2536,17 +2410,17 @@
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":54
  *     for order in range(num_orders):
  *         first = start_stop[order,0]
  *         last = start_stop[order,1]             # <<<<<<<<<<<<<<
  *         for index in prange(first, last, nogil=True, schedule="dynamic", num_threads=num_threads):
  *             solve1Pixel(ordered_pixels[index], discharge, lateral_inflow, constant, upstream_lookup,\
  */
-    __pyx_t_5 = __pyx_v_order;
-    __pyx_t_4 = 1;
-    __pyx_v_last = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_start_stop.data + __pyx_t_5 * __pyx_v_start_stop.strides[0]) )) + __pyx_t_4)) )));
+    __pyx_t_6 = __pyx_v_order;
+    __pyx_t_7 = 1;
+    __pyx_v_last = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_start_stop.data + __pyx_t_6 * __pyx_v_start_stop.strides[0]) )) + __pyx_t_7)) )));
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":55
  *         first = start_stop[order,0]
  *         last = start_stop[order,1]
  *         for index in prange(first, last, nogil=True, schedule="dynamic", num_threads=num_threads):             # <<<<<<<<<<<<<<
  *             solve1Pixel(ordered_pixels[index], discharge, lateral_inflow, constant, upstream_lookup,\
  *                         num_upstream_pixels, a_dx_div_dt, b_a_dx_div_dt, beta, inv_beta, b_minus_1)
@@ -2554,55 +2428,55 @@
     {
         #ifdef WITH_THREAD
         PyThreadState *_save;
         Py_UNBLOCK_THREADS
         __Pyx_FastGIL_Remember();
         #endif
         /*try:*/ {
-          __pyx_t_6 = __pyx_v_first;
-          __pyx_t_7 = __pyx_v_last;
-          if ((1 == 0)) abort();
+          __pyx_t_8 = __pyx_v_first;
+          __pyx_t_9 = __pyx_v_last;
+          if (1 == 0) abort();
           {
               #if ((defined(__APPLE__) || defined(__OSX__)) && (defined(__GNUC__) && (__GNUC__ > 2 || (__GNUC__ == 2 && (__GNUC_MINOR__ > 95)))))
                   #undef likely
                   #undef unlikely
                   #define likely(x)   (x)
                   #define unlikely(x) (x)
               #endif
-              __pyx_t_9 = (__pyx_t_7 - __pyx_t_6 + 1 - 1/abs(1)) / 1;
-              if (__pyx_t_9 > 0)
+              __pyx_t_11 = (__pyx_t_9 - __pyx_t_8 + 1 - 1/abs(1)) / 1;
+              if (__pyx_t_11 > 0)
               {
                   #ifdef _OPENMP
-                  #pragma omp parallel num_threads(__pyx_v_num_threads) private(__pyx_t_4)
+                  #pragma omp parallel num_threads(__pyx_v_num_threads) private(__pyx_t_12)
                   #endif /* _OPENMP */
                   {
                       #ifdef _OPENMP
                       #pragma omp for firstprivate(__pyx_v_index) lastprivate(__pyx_v_index) schedule(dynamic)
                       #endif /* _OPENMP */
-                      for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_9; __pyx_t_8++){
+                      for (__pyx_t_10 = 0; __pyx_t_10 < __pyx_t_11; __pyx_t_10++){
                           {
-                              __pyx_v_index = (long)(__pyx_t_6 + 1 * __pyx_t_8);
+                              __pyx_v_index = (long)(__pyx_t_8 + 1 * __pyx_t_10);
 
                               /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":56
  *         last = start_stop[order,1]
  *         for index in prange(first, last, nogil=True, schedule="dynamic", num_threads=num_threads):
  *             solve1Pixel(ordered_pixels[index], discharge, lateral_inflow, constant, upstream_lookup,\             # <<<<<<<<<<<<<<
  *                         num_upstream_pixels, a_dx_div_dt, b_a_dx_div_dt, beta, inv_beta, b_minus_1)
  * 
  */
-                              __pyx_t_4 = __pyx_v_index;
+                              __pyx_t_12 = __pyx_v_index;
 
                               /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":57
  *         for index in prange(first, last, nogil=True, schedule="dynamic", num_threads=num_threads):
  *             solve1Pixel(ordered_pixels[index], discharge, lateral_inflow, constant, upstream_lookup,\
  *                         num_upstream_pixels, a_dx_div_dt, b_a_dx_div_dt, beta, inv_beta, b_minus_1)             # <<<<<<<<<<<<<<
  * 
  * @boundscheck(False)
  */
-                              __pyx_f_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_solve1Pixel((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ordered_pixels.data) + __pyx_t_4)) ))), __pyx_v_discharge, __pyx_v_lateral_inflow, __pyx_v_constant, __pyx_v_upstream_lookup, __pyx_v_num_upstream_pixels, __pyx_v_a_dx_div_dt, __pyx_v_b_a_dx_div_dt, __pyx_v_beta, __pyx_v_inv_beta, __pyx_v_b_minus_1);
+                              __pyx_f_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_solve1Pixel((*((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_ordered_pixels.data) + __pyx_t_12)) ))), __pyx_v_discharge, __pyx_v_lateral_inflow, __pyx_v_constant, __pyx_v_upstream_lookup, __pyx_v_num_upstream_pixels, __pyx_v_a_dx_div_dt, __pyx_v_b_a_dx_div_dt, __pyx_v_beta, __pyx_v_inv_beta, __pyx_v_b_minus_1);
                           }
                       }
                   }
               }
           }
           #if ((defined(__APPLE__) || defined(__OSX__)) && (defined(__GNUC__) && (__GNUC__ > 2 || (__GNUC__ == 2 && (__GNUC_MINOR__ > 95)))))
               #undef likely
@@ -2676,16 +2550,35 @@
   double __pyx_v_upstream_inflow;
   Py_ssize_t __pyx_t_1;
   long __pyx_t_2;
   long __pyx_t_3;
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
-  int __pyx_t_7;
-  int __pyx_t_8;
+  Py_ssize_t __pyx_t_7;
+  Py_ssize_t __pyx_t_8;
+  int __pyx_t_9;
+  Py_ssize_t __pyx_t_10;
+  Py_ssize_t __pyx_t_11;
+  Py_ssize_t __pyx_t_12;
+  Py_ssize_t __pyx_t_13;
+  Py_ssize_t __pyx_t_14;
+  Py_ssize_t __pyx_t_15;
+  int __pyx_t_16;
+  Py_ssize_t __pyx_t_17;
+  Py_ssize_t __pyx_t_18;
+  Py_ssize_t __pyx_t_19;
+  Py_ssize_t __pyx_t_20;
+  Py_ssize_t __pyx_t_21;
+  Py_ssize_t __pyx_t_22;
+  Py_ssize_t __pyx_t_23;
+  Py_ssize_t __pyx_t_24;
+  Py_ssize_t __pyx_t_25;
+  Py_ssize_t __pyx_t_26;
+  Py_ssize_t __pyx_t_27;
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":67
  *     """"""
  *     cdef:
  *         long ups_ix, count = 0             # <<<<<<<<<<<<<<
  *         double error, const_plus_ups_infl, a_cpui_pow_b_m_1, secant_bound, other_bound, previous_estimate = -1., upstream_inflow = 0.
  *     # Inflow from upstream pixels
@@ -2718,49 +2611,49 @@
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":71
  *     # Inflow from upstream pixels
  *     for ups_ix in range(num_upstream_pixels[pix]):
  *         upstream_inflow += discharge[upstream_lookup[pix,ups_ix]]             # <<<<<<<<<<<<<<
  *     const_plus_ups_infl = upstream_inflow + constant[pix] # upstream_inflow + alpha*dx/dt*Qold**beta + dx*specific_lateral_inflow
  *     # If old discharge, upstream inflow and lateral inflow are below accuracy: set discharge to 0 and exit
  */
-    __pyx_t_1 = __pyx_v_pix;
-    __pyx_t_5 = __pyx_v_ups_ix;
-    __pyx_t_6 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_1 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_5)) )));
-    __pyx_v_upstream_inflow = (__pyx_v_upstream_inflow + (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_6)) ))));
+    __pyx_t_5 = __pyx_v_pix;
+    __pyx_t_6 = __pyx_v_ups_ix;
+    __pyx_t_7 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_5 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_6)) )));
+    __pyx_v_upstream_inflow = (__pyx_v_upstream_inflow + (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_7)) ))));
   }
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":72
  *     for ups_ix in range(num_upstream_pixels[pix]):
  *         upstream_inflow += discharge[upstream_lookup[pix,ups_ix]]
  *     const_plus_ups_infl = upstream_inflow + constant[pix] # upstream_inflow + alpha*dx/dt*Qold**beta + dx*specific_lateral_inflow             # <<<<<<<<<<<<<<
  *     # If old discharge, upstream inflow and lateral inflow are below accuracy: set discharge to 0 and exit
  *     if const_plus_ups_infl <= NEWTON_TOL:
  */
-  __pyx_t_5 = __pyx_v_pix;
-  __pyx_v_const_plus_ups_infl = (__pyx_v_upstream_inflow + (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_constant.data) + __pyx_t_5)) ))));
+  __pyx_t_8 = __pyx_v_pix;
+  __pyx_v_const_plus_ups_infl = (__pyx_v_upstream_inflow + (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_constant.data) + __pyx_t_8)) ))));
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":74
  *     const_plus_ups_infl = upstream_inflow + constant[pix] # upstream_inflow + alpha*dx/dt*Qold**beta + dx*specific_lateral_inflow
  *     # If old discharge, upstream inflow and lateral inflow are below accuracy: set discharge to 0 and exit
  *     if const_plus_ups_infl <= NEWTON_TOL:             # <<<<<<<<<<<<<<
  *         discharge[pix] = 0
  *         return
  */
-  __pyx_t_7 = ((__pyx_v_const_plus_ups_infl <= __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL) != 0);
-  if (__pyx_t_7) {
+  __pyx_t_9 = ((__pyx_v_const_plus_ups_infl <= __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL) != 0);
+  if (__pyx_t_9) {
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":75
  *     # If old discharge, upstream inflow and lateral inflow are below accuracy: set discharge to 0 and exit
  *     if const_plus_ups_infl <= NEWTON_TOL:
  *         discharge[pix] = 0             # <<<<<<<<<<<<<<
  *         return
  *     # Initial discharge guess using analytically derived boundary values
  */
-    __pyx_t_5 = __pyx_v_pix;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_5)) )) = 0.0;
+    __pyx_t_10 = __pyx_v_pix;
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_10)) )) = 0.0;
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":76
  *     if const_plus_ups_infl <= NEWTON_TOL:
  *         discharge[pix] = 0
  *         return             # <<<<<<<<<<<<<<
  *     # Initial discharge guess using analytically derived boundary values
  *     a_cpui_pow_b_m_1 = b_a_dx_div_dt[pix] * const_plus_ups_infl**b_minus_1
@@ -2779,26 +2672,26 @@
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":78
  *         return
  *     # Initial discharge guess using analytically derived boundary values
  *     a_cpui_pow_b_m_1 = b_a_dx_div_dt[pix] * const_plus_ups_infl**b_minus_1             # <<<<<<<<<<<<<<
  *     if a_cpui_pow_b_m_1 <= 1:
  *         secant_bound = const_plus_ups_infl / (1 + a_cpui_pow_b_m_1)
  */
-  __pyx_t_5 = __pyx_v_pix;
-  __pyx_v_a_cpui_pow_b_m_1 = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_b_a_dx_div_dt.data) + __pyx_t_5)) ))) * pow(__pyx_v_const_plus_ups_infl, __pyx_v_b_minus_1));
+  __pyx_t_11 = __pyx_v_pix;
+  __pyx_v_a_cpui_pow_b_m_1 = ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_b_a_dx_div_dt.data) + __pyx_t_11)) ))) * pow(__pyx_v_const_plus_ups_infl, __pyx_v_b_minus_1));
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":79
  *     # Initial discharge guess using analytically derived boundary values
  *     a_cpui_pow_b_m_1 = b_a_dx_div_dt[pix] * const_plus_ups_infl**b_minus_1
  *     if a_cpui_pow_b_m_1 <= 1:             # <<<<<<<<<<<<<<
  *         secant_bound = const_plus_ups_infl / (1 + a_cpui_pow_b_m_1)
  *     else:
  */
-  __pyx_t_7 = ((__pyx_v_a_cpui_pow_b_m_1 <= 1.0) != 0);
-  if (__pyx_t_7) {
+  __pyx_t_9 = ((__pyx_v_a_cpui_pow_b_m_1 <= 1.0) != 0);
+  if (__pyx_t_9) {
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":80
  *     a_cpui_pow_b_m_1 = b_a_dx_div_dt[pix] * const_plus_ups_infl**b_minus_1
  *     if a_cpui_pow_b_m_1 <= 1:
  *         secant_bound = const_plus_ups_infl / (1 + a_cpui_pow_b_m_1)             # <<<<<<<<<<<<<<
  *     else:
  *         secant_bound = const_plus_ups_infl / (1 + a_cpui_pow_b_m_1**inv_beta)
@@ -2830,107 +2723,107 @@
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":83
  *     else:
  *         secant_bound = const_plus_ups_infl / (1 + a_cpui_pow_b_m_1**inv_beta)
  *     other_bound = ((const_plus_ups_infl - secant_bound) / a_dx_div_dt[pix])**inv_beta             # <<<<<<<<<<<<<<
  *     discharge[pix] = (secant_bound + other_bound) / 2
  *     error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)
  */
-  __pyx_t_5 = __pyx_v_pix;
-  __pyx_v_other_bound = pow(((__pyx_v_const_plus_ups_infl - __pyx_v_secant_bound) / (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_a_dx_div_dt.data) + __pyx_t_5)) )))), __pyx_v_inv_beta);
+  __pyx_t_12 = __pyx_v_pix;
+  __pyx_v_other_bound = pow(((__pyx_v_const_plus_ups_infl - __pyx_v_secant_bound) / (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_a_dx_div_dt.data) + __pyx_t_12)) )))), __pyx_v_inv_beta);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":84
  *         secant_bound = const_plus_ups_infl / (1 + a_cpui_pow_b_m_1**inv_beta)
  *     other_bound = ((const_plus_ups_infl - secant_bound) / a_dx_div_dt[pix])**inv_beta
  *     discharge[pix] = (secant_bound + other_bound) / 2             # <<<<<<<<<<<<<<
  *     error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)
  *     # Iterations
  */
-  __pyx_t_5 = __pyx_v_pix;
-  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_5)) )) = ((__pyx_v_secant_bound + __pyx_v_other_bound) / 2.0);
+  __pyx_t_13 = __pyx_v_pix;
+  *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_13)) )) = ((__pyx_v_secant_bound + __pyx_v_other_bound) / 2.0);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":85
  *     other_bound = ((const_plus_ups_infl - secant_bound) / a_dx_div_dt[pix])**inv_beta
  *     discharge[pix] = (secant_bound + other_bound) / 2
  *     error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)             # <<<<<<<<<<<<<<
  *     # Iterations
  *     while fabs(error) > NEWTON_TOL and discharge[pix] != previous_estimate and count < MAX_ITERS: # is previous_estimate useful?
  */
-  __pyx_t_5 = __pyx_v_pix;
-  __pyx_t_1 = __pyx_v_pix;
-  __pyx_v_error = __pyx_f_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_closureError((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_5)) ))), __pyx_v_const_plus_ups_infl, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_a_dx_div_dt.data) + __pyx_t_1)) ))), __pyx_v_beta);
+  __pyx_t_14 = __pyx_v_pix;
+  __pyx_t_15 = __pyx_v_pix;
+  __pyx_v_error = __pyx_f_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_closureError((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_14)) ))), __pyx_v_const_plus_ups_infl, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_a_dx_div_dt.data) + __pyx_t_15)) ))), __pyx_v_beta);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":87
  *     error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)
  *     # Iterations
  *     while fabs(error) > NEWTON_TOL and discharge[pix] != previous_estimate and count < MAX_ITERS: # is previous_estimate useful?             # <<<<<<<<<<<<<<
  *         previous_estimate = discharge[pix]
  *         discharge[pix] -= error / (1 + b_a_dx_div_dt[pix] * discharge[pix]**b_minus_1)
  */
   while (1) {
-    __pyx_t_8 = ((fabs(__pyx_v_error) > __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL) != 0);
-    if (__pyx_t_8) {
+    __pyx_t_16 = ((fabs(__pyx_v_error) > __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL) != 0);
+    if (__pyx_t_16) {
     } else {
-      __pyx_t_7 = __pyx_t_8;
+      __pyx_t_9 = __pyx_t_16;
       goto __pyx_L9_bool_binop_done;
     }
-    __pyx_t_1 = __pyx_v_pix;
-    __pyx_t_8 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_1)) ))) != __pyx_v_previous_estimate) != 0);
-    if (__pyx_t_8) {
+    __pyx_t_17 = __pyx_v_pix;
+    __pyx_t_16 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_17)) ))) != __pyx_v_previous_estimate) != 0);
+    if (__pyx_t_16) {
     } else {
-      __pyx_t_7 = __pyx_t_8;
+      __pyx_t_9 = __pyx_t_16;
       goto __pyx_L9_bool_binop_done;
     }
-    __pyx_t_8 = ((__pyx_v_count < __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_MAX_ITERS) != 0);
-    __pyx_t_7 = __pyx_t_8;
+    __pyx_t_16 = ((__pyx_v_count < __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_MAX_ITERS) != 0);
+    __pyx_t_9 = __pyx_t_16;
     __pyx_L9_bool_binop_done:;
-    if (!__pyx_t_7) break;
+    if (!__pyx_t_9) break;
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":88
  *     # Iterations
  *     while fabs(error) > NEWTON_TOL and discharge[pix] != previous_estimate and count < MAX_ITERS: # is previous_estimate useful?
  *         previous_estimate = discharge[pix]             # <<<<<<<<<<<<<<
  *         discharge[pix] -= error / (1 + b_a_dx_div_dt[pix] * discharge[pix]**b_minus_1)
  *         discharge[pix] = fmax(discharge[pix], NEWTON_TOL)
  */
-    __pyx_t_1 = __pyx_v_pix;
-    __pyx_v_previous_estimate = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_1)) )));
+    __pyx_t_18 = __pyx_v_pix;
+    __pyx_v_previous_estimate = (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_18)) )));
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":89
  *     while fabs(error) > NEWTON_TOL and discharge[pix] != previous_estimate and count < MAX_ITERS: # is previous_estimate useful?
  *         previous_estimate = discharge[pix]
  *         discharge[pix] -= error / (1 + b_a_dx_div_dt[pix] * discharge[pix]**b_minus_1)             # <<<<<<<<<<<<<<
  *         discharge[pix] = fmax(discharge[pix], NEWTON_TOL)
  *         error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)
  */
-    __pyx_t_1 = __pyx_v_pix;
-    __pyx_t_5 = __pyx_v_pix;
-    __pyx_t_6 = __pyx_v_pix;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_6)) )) -= (__pyx_v_error / (1.0 + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_b_a_dx_div_dt.data) + __pyx_t_1)) ))) * pow((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_5)) ))), __pyx_v_b_minus_1))));
+    __pyx_t_19 = __pyx_v_pix;
+    __pyx_t_20 = __pyx_v_pix;
+    __pyx_t_21 = __pyx_v_pix;
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_21)) )) -= (__pyx_v_error / (1.0 + ((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_b_a_dx_div_dt.data) + __pyx_t_19)) ))) * pow((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_20)) ))), __pyx_v_b_minus_1))));
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":90
  *         previous_estimate = discharge[pix]
  *         discharge[pix] -= error / (1 + b_a_dx_div_dt[pix] * discharge[pix]**b_minus_1)
  *         discharge[pix] = fmax(discharge[pix], NEWTON_TOL)             # <<<<<<<<<<<<<<
  *         error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)
  *         count += 1
  */
-    __pyx_t_5 = __pyx_v_pix;
-    __pyx_t_1 = __pyx_v_pix;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_1)) )) = fmax((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_5)) ))), __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL);
+    __pyx_t_22 = __pyx_v_pix;
+    __pyx_t_23 = __pyx_v_pix;
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_23)) )) = fmax((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_22)) ))), __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL);
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":91
  *         discharge[pix] -= error / (1 + b_a_dx_div_dt[pix] * discharge[pix]**b_minus_1)
  *         discharge[pix] = fmax(discharge[pix], NEWTON_TOL)
  *         error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)             # <<<<<<<<<<<<<<
  *         count += 1
  *     # If iterations converge to NEWTON_TOL, set value to 0
  */
-    __pyx_t_5 = __pyx_v_pix;
-    __pyx_t_1 = __pyx_v_pix;
-    __pyx_v_error = __pyx_f_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_closureError((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_5)) ))), __pyx_v_const_plus_ups_infl, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_a_dx_div_dt.data) + __pyx_t_1)) ))), __pyx_v_beta);
+    __pyx_t_24 = __pyx_v_pix;
+    __pyx_t_25 = __pyx_v_pix;
+    __pyx_v_error = __pyx_f_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_closureError((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_24)) ))), __pyx_v_const_plus_ups_infl, (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_a_dx_div_dt.data) + __pyx_t_25)) ))), __pyx_v_beta);
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":92
  *         discharge[pix] = fmax(discharge[pix], NEWTON_TOL)
  *         error = closureError(discharge[pix], const_plus_ups_infl, a_dx_div_dt[pix], beta)
  *         count += 1             # <<<<<<<<<<<<<<
  *     # If iterations converge to NEWTON_TOL, set value to 0
  *     if discharge[pix] == NEWTON_TOL:
@@ -2941,27 +2834,27 @@
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":94
  *         count += 1
  *     # If iterations converge to NEWTON_TOL, set value to 0
  *     if discharge[pix] == NEWTON_TOL:             # <<<<<<<<<<<<<<
  *         discharge[pix] = 0
  * 
  */
-  __pyx_t_1 = __pyx_v_pix;
-  __pyx_t_7 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_1)) ))) == __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL) != 0);
-  if (__pyx_t_7) {
+  __pyx_t_26 = __pyx_v_pix;
+  __pyx_t_9 = (((*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_26)) ))) == __pyx_v_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_NEWTON_TOL) != 0);
+  if (__pyx_t_9) {
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":95
  *     # If iterations converge to NEWTON_TOL, set value to 0
  *     if discharge[pix] == NEWTON_TOL:
  *         discharge[pix] = 0             # <<<<<<<<<<<<<<
  * 
  * @boundscheck(False)
  */
-    __pyx_t_1 = __pyx_v_pix;
-    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_1)) )) = 0.0;
+    __pyx_t_27 = __pyx_v_pix;
+    *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_27)) )) = 0.0;
 
     /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":94
  *         count += 1
  *     # If iterations converge to NEWTON_TOL, set value to 0
  *     if discharge[pix] == NEWTON_TOL:             # <<<<<<<<<<<<<<
  *         discharge[pix] = 0
  * 
@@ -3027,17 +2920,14 @@
 static char __pyx_doc_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_2updateUpstreamRouted[] = "Called by kinematic_wave_parallel.orderKinematicRouting to implement greedy pixel ordering starting from headwaters.";
 static PyMethodDef __pyx_mdef_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_3updateUpstreamRouted = {"updateUpstreamRouted", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_3updateUpstreamRouted, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_2updateUpstreamRouted};
 static PyObject *__pyx_pw_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_3updateUpstreamRouted(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_pixels_routed = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_downstream_lookup = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_upstream_lookup = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_upstream_routed = { 0, 0, { 0 }, { 0 }, { 0 } };
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("updateUpstreamRouted (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pixels_routed,&__pyx_n_s_downstream_lookup,&__pyx_n_s_upstream_lookup,&__pyx_n_s_upstream_routed,0};
     PyObject* values[4] = {0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -3120,17 +3010,17 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   long __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+  Py_ssize_t __pyx_t_9;
+  Py_ssize_t __pyx_t_10;
+  Py_ssize_t __pyx_t_11;
   __Pyx_RefNannySetupContext("updateUpstreamRouted", 0);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":113
  *     cdef:
  *         long downs_pix, pix, ups_index
  *     for pix in pixels_routed:             # <<<<<<<<<<<<<<
  *         downs_pix = downstream_lookup[pix]
@@ -3216,19 +3106,19 @@
  *         if downs_pix != -1:
  *             ups_index = 0
  *             while upstream_lookup[downs_pix,ups_index] != pix:             # <<<<<<<<<<<<<<
  *                 ups_index += 1
  *             upstream_routed[downs_pix,ups_index] = True
  */
       while (1) {
-        __pyx_t_6 = __pyx_v_downs_pix;
-        __pyx_t_8 = __pyx_v_ups_index;
-        if (__pyx_t_6 < 0) __pyx_t_6 += __pyx_v_upstream_lookup.shape[0];
-        if (__pyx_t_8 < 0) __pyx_t_8 += __pyx_v_upstream_lookup.shape[1];
-        __pyx_t_7 = (((*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_6 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_8)) ))) != __pyx_v_pix) != 0);
+        __pyx_t_8 = __pyx_v_downs_pix;
+        __pyx_t_9 = __pyx_v_ups_index;
+        if (__pyx_t_8 < 0) __pyx_t_8 += __pyx_v_upstream_lookup.shape[0];
+        if (__pyx_t_9 < 0) __pyx_t_9 += __pyx_v_upstream_lookup.shape[1];
+        __pyx_t_7 = (((*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_8 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_9)) ))) != __pyx_v_pix) != 0);
         if (!__pyx_t_7) break;
 
         /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":118
  *             ups_index = 0
  *             while upstream_lookup[downs_pix,ups_index] != pix:
  *                 ups_index += 1             # <<<<<<<<<<<<<<
  *             upstream_routed[downs_pix,ups_index] = True
@@ -3240,19 +3130,19 @@
       /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":119
  *             while upstream_lookup[downs_pix,ups_index] != pix:
  *                 ups_index += 1
  *             upstream_routed[downs_pix,ups_index] = True             # <<<<<<<<<<<<<<
  * 
  * def upDownLookups(long[:,::1] flow_d8, unsigned char[:,::1] land_mask, long[:,::1] land_points, long num_pixs, long[:,::1] ix_adds):
  */
-      __pyx_t_8 = __pyx_v_downs_pix;
-      __pyx_t_6 = __pyx_v_ups_index;
-      if (__pyx_t_8 < 0) __pyx_t_8 += __pyx_v_upstream_routed.shape[0];
-      if (__pyx_t_6 < 0) __pyx_t_6 += __pyx_v_upstream_routed.shape[1];
-      *((unsigned char *) ( /* dim=1 */ ((char *) (((unsigned char *) ( /* dim=0 */ (__pyx_v_upstream_routed.data + __pyx_t_8 * __pyx_v_upstream_routed.strides[0]) )) + __pyx_t_6)) )) = 1;
+      __pyx_t_10 = __pyx_v_downs_pix;
+      __pyx_t_11 = __pyx_v_ups_index;
+      if (__pyx_t_10 < 0) __pyx_t_10 += __pyx_v_upstream_routed.shape[0];
+      if (__pyx_t_11 < 0) __pyx_t_11 += __pyx_v_upstream_routed.shape[1];
+      *((unsigned char *) ( /* dim=1 */ ((char *) (((unsigned char *) ( /* dim=0 */ (__pyx_v_upstream_routed.data + __pyx_t_10 * __pyx_v_upstream_routed.strides[0]) )) + __pyx_t_11)) )) = 1;
 
       /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":115
  *     for pix in pixels_routed:
  *         downs_pix = downstream_lookup[pix]
  *         if downs_pix != -1:             # <<<<<<<<<<<<<<
  *             ups_index = 0
  *             while upstream_lookup[downs_pix,ups_index] != pix:
@@ -3309,17 +3199,14 @@
 static PyMethodDef __pyx_mdef_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_5upDownLookups = {"upDownLookups", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_5upDownLookups, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_4upDownLookups};
 static PyObject *__pyx_pw_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_5upDownLookups(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_flow_d8 = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_land_mask = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_land_points = { 0, 0, { 0 }, { 0 }, { 0 } };
   long __pyx_v_num_pixs;
   __Pyx_memviewslice __pyx_v_ix_adds = { 0, 0, { 0 }, { 0 }, { 0 } };
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("upDownLookups (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_flow_d8,&__pyx_n_s_land_mask,&__pyx_n_s_land_points,&__pyx_n_s_num_pixs,&__pyx_n_s_ix_adds,0};
     PyObject* values[5] = {0,0,0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -3432,21 +3319,32 @@
   unsigned int __pyx_t_14;
   int __pyx_t_15;
   Py_ssize_t __pyx_t_16;
   Py_ssize_t __pyx_t_17;
   int __pyx_t_18;
   Py_ssize_t __pyx_t_19;
   Py_ssize_t __pyx_t_20;
-  int __pyx_t_21;
-  size_t __pyx_t_22;
-  size_t __pyx_t_23;
-  size_t __pyx_t_24;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+  Py_ssize_t __pyx_t_21;
+  Py_ssize_t __pyx_t_22;
+  Py_ssize_t __pyx_t_23;
+  Py_ssize_t __pyx_t_24;
+  Py_ssize_t __pyx_t_25;
+  Py_ssize_t __pyx_t_26;
+  int __pyx_t_27;
+  Py_ssize_t __pyx_t_28;
+  Py_ssize_t __pyx_t_29;
+  Py_ssize_t __pyx_t_30;
+  Py_ssize_t __pyx_t_31;
+  Py_ssize_t __pyx_t_32;
+  Py_ssize_t __pyx_t_33;
+  size_t __pyx_t_34;
+  size_t __pyx_t_35;
+  size_t __pyx_t_36;
+  size_t __pyx_t_37;
+  size_t __pyx_t_38;
   __Pyx_RefNannySetupContext("upDownLookups", 0);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":124
  *     '''Called by catchment.streamLookups'''
  *     cdef:
  *         long[::1] downstream_lookup = -np.ones(num_pixs, int)             # <<<<<<<<<<<<<<
  *         long[:,::1] upstream_lookup = -np.ones((num_pixs, 8), int)
@@ -3718,138 +3616,138 @@
         /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":132
  *         for src_col in range(num_col):
  *             if flow_d8[src_row,src_col] < 8:
  *                 dst_row = src_row + ix_adds[flow_d8[src_row,src_col],0]             # <<<<<<<<<<<<<<
  *                 dst_col = src_col + ix_adds[flow_d8[src_row,src_col],1]
  *                 if dst_row != -1 and dst_col != -1 and dst_row != num_row and dst_col != num_col and land_mask[dst_row,dst_col]:
  */
-        __pyx_t_17 = __pyx_v_src_row;
-        __pyx_t_16 = __pyx_v_src_col;
-        if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_v_flow_d8.shape[0];
-        if (__pyx_t_16 < 0) __pyx_t_16 += __pyx_v_flow_d8.shape[1];
-        __pyx_t_19 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_flow_d8.data + __pyx_t_17 * __pyx_v_flow_d8.strides[0]) )) + __pyx_t_16)) )));
-        __pyx_t_20 = 0;
-        if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_v_ix_adds.shape[0];
-        if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_v_ix_adds.shape[1];
-        __pyx_v_dst_row = (__pyx_v_src_row + (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_ix_adds.data + __pyx_t_19 * __pyx_v_ix_adds.strides[0]) )) + __pyx_t_20)) ))));
+        __pyx_t_19 = __pyx_v_src_row;
+        __pyx_t_20 = __pyx_v_src_col;
+        if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_v_flow_d8.shape[0];
+        if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_v_flow_d8.shape[1];
+        __pyx_t_21 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_flow_d8.data + __pyx_t_19 * __pyx_v_flow_d8.strides[0]) )) + __pyx_t_20)) )));
+        __pyx_t_22 = 0;
+        if (__pyx_t_21 < 0) __pyx_t_21 += __pyx_v_ix_adds.shape[0];
+        if (__pyx_t_22 < 0) __pyx_t_22 += __pyx_v_ix_adds.shape[1];
+        __pyx_v_dst_row = (__pyx_v_src_row + (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_ix_adds.data + __pyx_t_21 * __pyx_v_ix_adds.strides[0]) )) + __pyx_t_22)) ))));
 
         /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":133
  *             if flow_d8[src_row,src_col] < 8:
  *                 dst_row = src_row + ix_adds[flow_d8[src_row,src_col],0]
  *                 dst_col = src_col + ix_adds[flow_d8[src_row,src_col],1]             # <<<<<<<<<<<<<<
  *                 if dst_row != -1 and dst_col != -1 and dst_row != num_row and dst_col != num_col and land_mask[dst_row,dst_col]:
  *                     ups_p = land_points[src_row,src_col]
  */
-        __pyx_t_16 = __pyx_v_src_row;
-        __pyx_t_17 = __pyx_v_src_col;
-        if (__pyx_t_16 < 0) __pyx_t_16 += __pyx_v_flow_d8.shape[0];
-        if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_v_flow_d8.shape[1];
-        __pyx_t_20 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_flow_d8.data + __pyx_t_16 * __pyx_v_flow_d8.strides[0]) )) + __pyx_t_17)) )));
-        __pyx_t_19 = 1;
-        if (__pyx_t_20 < 0) __pyx_t_20 += __pyx_v_ix_adds.shape[0];
-        if (__pyx_t_19 < 0) __pyx_t_19 += __pyx_v_ix_adds.shape[1];
-        __pyx_v_dst_col = (__pyx_v_src_col + (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_ix_adds.data + __pyx_t_20 * __pyx_v_ix_adds.strides[0]) )) + __pyx_t_19)) ))));
+        __pyx_t_23 = __pyx_v_src_row;
+        __pyx_t_24 = __pyx_v_src_col;
+        if (__pyx_t_23 < 0) __pyx_t_23 += __pyx_v_flow_d8.shape[0];
+        if (__pyx_t_24 < 0) __pyx_t_24 += __pyx_v_flow_d8.shape[1];
+        __pyx_t_25 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_flow_d8.data + __pyx_t_23 * __pyx_v_flow_d8.strides[0]) )) + __pyx_t_24)) )));
+        __pyx_t_26 = 1;
+        if (__pyx_t_25 < 0) __pyx_t_25 += __pyx_v_ix_adds.shape[0];
+        if (__pyx_t_26 < 0) __pyx_t_26 += __pyx_v_ix_adds.shape[1];
+        __pyx_v_dst_col = (__pyx_v_src_col + (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_ix_adds.data + __pyx_t_25 * __pyx_v_ix_adds.strides[0]) )) + __pyx_t_26)) ))));
 
         /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":134
  *                 dst_row = src_row + ix_adds[flow_d8[src_row,src_col],0]
  *                 dst_col = src_col + ix_adds[flow_d8[src_row,src_col],1]
  *                 if dst_row != -1 and dst_col != -1 and dst_row != num_row and dst_col != num_col and land_mask[dst_row,dst_col]:             # <<<<<<<<<<<<<<
  *                     ups_p = land_points[src_row,src_col]
  *                     downs_p = land_points[dst_row,dst_col]
  */
-        __pyx_t_21 = ((__pyx_v_dst_row != -1L) != 0);
-        if (__pyx_t_21) {
+        __pyx_t_27 = ((__pyx_v_dst_row != -1L) != 0);
+        if (__pyx_t_27) {
         } else {
-          __pyx_t_18 = __pyx_t_21;
+          __pyx_t_18 = __pyx_t_27;
           goto __pyx_L9_bool_binop_done;
         }
-        __pyx_t_21 = ((__pyx_v_dst_col != -1L) != 0);
-        if (__pyx_t_21) {
+        __pyx_t_27 = ((__pyx_v_dst_col != -1L) != 0);
+        if (__pyx_t_27) {
         } else {
-          __pyx_t_18 = __pyx_t_21;
+          __pyx_t_18 = __pyx_t_27;
           goto __pyx_L9_bool_binop_done;
         }
-        __pyx_t_21 = ((__pyx_v_dst_row != __pyx_v_num_row) != 0);
-        if (__pyx_t_21) {
+        __pyx_t_27 = ((__pyx_v_dst_row != __pyx_v_num_row) != 0);
+        if (__pyx_t_27) {
         } else {
-          __pyx_t_18 = __pyx_t_21;
+          __pyx_t_18 = __pyx_t_27;
           goto __pyx_L9_bool_binop_done;
         }
-        __pyx_t_21 = ((__pyx_v_dst_col != __pyx_v_num_col) != 0);
-        if (__pyx_t_21) {
+        __pyx_t_27 = ((__pyx_v_dst_col != __pyx_v_num_col) != 0);
+        if (__pyx_t_27) {
         } else {
-          __pyx_t_18 = __pyx_t_21;
+          __pyx_t_18 = __pyx_t_27;
           goto __pyx_L9_bool_binop_done;
         }
-        __pyx_t_17 = __pyx_v_dst_row;
-        __pyx_t_16 = __pyx_v_dst_col;
-        if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_v_land_mask.shape[0];
-        if (__pyx_t_16 < 0) __pyx_t_16 += __pyx_v_land_mask.shape[1];
-        __pyx_t_21 = ((*((unsigned char *) ( /* dim=1 */ ((char *) (((unsigned char *) ( /* dim=0 */ (__pyx_v_land_mask.data + __pyx_t_17 * __pyx_v_land_mask.strides[0]) )) + __pyx_t_16)) ))) != 0);
-        __pyx_t_18 = __pyx_t_21;
+        __pyx_t_28 = __pyx_v_dst_row;
+        __pyx_t_29 = __pyx_v_dst_col;
+        if (__pyx_t_28 < 0) __pyx_t_28 += __pyx_v_land_mask.shape[0];
+        if (__pyx_t_29 < 0) __pyx_t_29 += __pyx_v_land_mask.shape[1];
+        __pyx_t_27 = ((*((unsigned char *) ( /* dim=1 */ ((char *) (((unsigned char *) ( /* dim=0 */ (__pyx_v_land_mask.data + __pyx_t_28 * __pyx_v_land_mask.strides[0]) )) + __pyx_t_29)) ))) != 0);
+        __pyx_t_18 = __pyx_t_27;
         __pyx_L9_bool_binop_done:;
         if (__pyx_t_18) {
 
           /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":135
  *                 dst_col = src_col + ix_adds[flow_d8[src_row,src_col],1]
  *                 if dst_row != -1 and dst_col != -1 and dst_row != num_row and dst_col != num_col and land_mask[dst_row,dst_col]:
  *                     ups_p = land_points[src_row,src_col]             # <<<<<<<<<<<<<<
  *                     downs_p = land_points[dst_row,dst_col]
  *                     downstream_lookup[ups_p] = downs_p
  */
-          __pyx_t_16 = __pyx_v_src_row;
-          __pyx_t_17 = __pyx_v_src_col;
-          if (__pyx_t_16 < 0) __pyx_t_16 += __pyx_v_land_points.shape[0];
-          if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_v_land_points.shape[1];
-          __pyx_v_ups_p = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_land_points.data + __pyx_t_16 * __pyx_v_land_points.strides[0]) )) + __pyx_t_17)) )));
+          __pyx_t_30 = __pyx_v_src_row;
+          __pyx_t_31 = __pyx_v_src_col;
+          if (__pyx_t_30 < 0) __pyx_t_30 += __pyx_v_land_points.shape[0];
+          if (__pyx_t_31 < 0) __pyx_t_31 += __pyx_v_land_points.shape[1];
+          __pyx_v_ups_p = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_land_points.data + __pyx_t_30 * __pyx_v_land_points.strides[0]) )) + __pyx_t_31)) )));
 
           /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":136
  *                 if dst_row != -1 and dst_col != -1 and dst_row != num_row and dst_col != num_col and land_mask[dst_row,dst_col]:
  *                     ups_p = land_points[src_row,src_col]
  *                     downs_p = land_points[dst_row,dst_col]             # <<<<<<<<<<<<<<
  *                     downstream_lookup[ups_p] = downs_p
  *                     upstream_lookup[downs_p,ups_count[downs_p]] = ups_p
  */
-          __pyx_t_17 = __pyx_v_dst_row;
-          __pyx_t_16 = __pyx_v_dst_col;
-          if (__pyx_t_17 < 0) __pyx_t_17 += __pyx_v_land_points.shape[0];
-          if (__pyx_t_16 < 0) __pyx_t_16 += __pyx_v_land_points.shape[1];
-          __pyx_v_downs_p = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_land_points.data + __pyx_t_17 * __pyx_v_land_points.strides[0]) )) + __pyx_t_16)) )));
+          __pyx_t_32 = __pyx_v_dst_row;
+          __pyx_t_33 = __pyx_v_dst_col;
+          if (__pyx_t_32 < 0) __pyx_t_32 += __pyx_v_land_points.shape[0];
+          if (__pyx_t_33 < 0) __pyx_t_33 += __pyx_v_land_points.shape[1];
+          __pyx_v_downs_p = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_land_points.data + __pyx_t_32 * __pyx_v_land_points.strides[0]) )) + __pyx_t_33)) )));
 
           /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":137
  *                     ups_p = land_points[src_row,src_col]
  *                     downs_p = land_points[dst_row,dst_col]
  *                     downstream_lookup[ups_p] = downs_p             # <<<<<<<<<<<<<<
  *                     upstream_lookup[downs_p,ups_count[downs_p]] = ups_p
  *                     ups_count[downs_p] += 1
  */
-          __pyx_t_22 = __pyx_v_ups_p;
-          *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_downstream_lookup.data) + __pyx_t_22)) )) = __pyx_v_downs_p;
+          __pyx_t_34 = __pyx_v_ups_p;
+          *((long *) ( /* dim=0 */ ((char *) (((long *) __pyx_v_downstream_lookup.data) + __pyx_t_34)) )) = __pyx_v_downs_p;
 
           /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":138
  *                     downs_p = land_points[dst_row,dst_col]
  *                     downstream_lookup[ups_p] = downs_p
  *                     upstream_lookup[downs_p,ups_count[downs_p]] = ups_p             # <<<<<<<<<<<<<<
  *                     ups_count[downs_p] += 1
  *     return np.asarray(downstream_lookup), np.asarray(upstream_lookup)
  */
-          __pyx_t_22 = __pyx_v_downs_p;
-          __pyx_t_23 = __pyx_v_downs_p;
-          __pyx_t_24 = (*((unsigned int *) ( /* dim=0 */ ((char *) (((unsigned int *) __pyx_v_ups_count.data) + __pyx_t_22)) )));
-          *((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_23 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_24)) )) = __pyx_v_ups_p;
+          __pyx_t_35 = __pyx_v_downs_p;
+          __pyx_t_36 = __pyx_v_downs_p;
+          __pyx_t_37 = (*((unsigned int *) ( /* dim=0 */ ((char *) (((unsigned int *) __pyx_v_ups_count.data) + __pyx_t_35)) )));
+          *((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_36 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_37)) )) = __pyx_v_ups_p;
 
           /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":139
  *                     downstream_lookup[ups_p] = downs_p
  *                     upstream_lookup[downs_p,ups_count[downs_p]] = ups_p
  *                     ups_count[downs_p] += 1             # <<<<<<<<<<<<<<
  *     return np.asarray(downstream_lookup), np.asarray(upstream_lookup)
  * 
  */
-          __pyx_t_22 = __pyx_v_downs_p;
-          *((unsigned int *) ( /* dim=0 */ ((char *) (((unsigned int *) __pyx_v_ups_count.data) + __pyx_t_22)) )) += 1;
+          __pyx_t_38 = __pyx_v_downs_p;
+          *((unsigned int *) ( /* dim=0 */ ((char *) (((unsigned int *) __pyx_v_ups_count.data) + __pyx_t_38)) )) += 1;
 
           /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":134
  *                 dst_row = src_row + ix_adds[flow_d8[src_row,src_col],0]
  *                 dst_col = src_col + ix_adds[flow_d8[src_row,src_col],1]
  *                 if dst_row != -1 and dst_col != -1 and dst_row != num_row and dst_col != num_col and land_mask[dst_row,dst_col]:             # <<<<<<<<<<<<<<
  *                     ups_p = land_points[src_row,src_col]
  *                     downs_p = land_points[dst_row,dst_col]
@@ -3978,17 +3876,14 @@
 /* Python wrapper */
 static PyObject *__pyx_pw_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_7immediateUpstreamInflow(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_7immediateUpstreamInflow = {"immediateUpstreamInflow", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_7immediateUpstreamInflow, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_8lisflood_20hydrological_modules_29kinematic_wave_parallel_tools_7immediateUpstreamInflow(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_discharge = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_upstream_lookup = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_num_upstream_pixels = { 0, 0, { 0 }, { 0 }, { 0 } };
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("immediateUpstreamInflow (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_discharge,&__pyx_n_s_upstream_lookup,&__pyx_n_s_num_upstream_pixels,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -4069,17 +3964,15 @@
   Py_ssize_t __pyx_t_9;
   long __pyx_t_10;
   long __pyx_t_11;
   long __pyx_t_12;
   Py_ssize_t __pyx_t_13;
   Py_ssize_t __pyx_t_14;
   Py_ssize_t __pyx_t_15;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+  Py_ssize_t __pyx_t_16;
   __Pyx_RefNannySetupContext("immediateUpstreamInflow", 0);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":150
  *     """"""
  *     cdef:
  *         long pix, ups_ix, num_pixels = discharge.size             # <<<<<<<<<<<<<<
  *         double [::1] inflow = np.zeros(num_pixels)
@@ -4158,23 +4051,23 @@
 
       /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":154
  *     for pix in range(num_pixels):
  *         for ups_ix in range(num_upstream_pixels[pix]):
  *             inflow[pix] += discharge[upstream_lookup[pix,ups_ix]]             # <<<<<<<<<<<<<<
  *     return np.asarray(inflow)
  */
-      __pyx_t_9 = __pyx_v_pix;
-      __pyx_t_13 = __pyx_v_ups_ix;
-      if (__pyx_t_9 < 0) __pyx_t_9 += __pyx_v_upstream_lookup.shape[0];
-      if (__pyx_t_13 < 0) __pyx_t_13 += __pyx_v_upstream_lookup.shape[1];
-      __pyx_t_14 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_9 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_13)) )));
-      if (__pyx_t_14 < 0) __pyx_t_14 += __pyx_v_discharge.shape[0];
-      __pyx_t_15 = __pyx_v_pix;
-      if (__pyx_t_15 < 0) __pyx_t_15 += __pyx_v_inflow.shape[0];
-      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_inflow.data) + __pyx_t_15)) )) += (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_14)) )));
+      __pyx_t_13 = __pyx_v_pix;
+      __pyx_t_14 = __pyx_v_ups_ix;
+      if (__pyx_t_13 < 0) __pyx_t_13 += __pyx_v_upstream_lookup.shape[0];
+      if (__pyx_t_14 < 0) __pyx_t_14 += __pyx_v_upstream_lookup.shape[1];
+      __pyx_t_15 = (*((long *) ( /* dim=1 */ ((char *) (((long *) ( /* dim=0 */ (__pyx_v_upstream_lookup.data + __pyx_t_13 * __pyx_v_upstream_lookup.strides[0]) )) + __pyx_t_14)) )));
+      if (__pyx_t_15 < 0) __pyx_t_15 += __pyx_v_discharge.shape[0];
+      __pyx_t_16 = __pyx_v_pix;
+      if (__pyx_t_16 < 0) __pyx_t_16 += __pyx_v_inflow.shape[0];
+      *((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_inflow.data) + __pyx_t_16)) )) += (*((double *) ( /* dim=0 */ ((char *) (((double *) __pyx_v_discharge.data) + __pyx_t_15)) )));
     }
   }
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":155
  *         for ups_ix in range(num_upstream_pixels[pix]):
  *             inflow[pix] += discharge[upstream_lookup[pix,ups_ix]]
  *     return np.asarray(inflow)             # <<<<<<<<<<<<<<
@@ -4246,17 +4139,14 @@
 static int __pyx_array___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_array___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_shape = 0;
   Py_ssize_t __pyx_v_itemsize;
   PyObject *__pyx_v_format = 0;
   PyObject *__pyx_v_mode = 0;
   int __pyx_v_allocate_buffer;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_shape,&__pyx_n_s_itemsize,&__pyx_n_s_format,&__pyx_n_s_mode,&__pyx_n_s_allocate_buffer,0};
     PyObject* values[5] = {0,0,0,0,0};
     values[3] = ((PyObject *)__pyx_n_s_c);
@@ -4387,17 +4277,14 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   char *__pyx_t_7;
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   Py_ssize_t __pyx_t_11;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_format);
 
   /* "View.MemoryView":129
  *         cdef PyObject **p
  * 
  *         self.ndim = <int> len(shape)             # <<<<<<<<<<<<<<
@@ -5013,17 +4900,14 @@
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   char *__pyx_t_4;
   Py_ssize_t __pyx_t_5;
   int __pyx_t_6;
   Py_ssize_t *__pyx_t_7;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   if (__pyx_v_info == NULL) {
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
@@ -5444,17 +5328,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":223
  *     @property
  *     def memview(self):
  *         return self.get_memview()             # <<<<<<<<<<<<<<
  * 
@@ -5497,17 +5378,14 @@
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self) {
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_memview", 0);
 
   /* "View.MemoryView":227
  *     @cname('get_memview')
  *     cdef get_memview(self):
  *         flags =  PyBUF_ANY_CONTIGUOUS|PyBUF_FORMAT|PyBUF_WRITABLE             # <<<<<<<<<<<<<<
  *         return  memoryview(self, flags, self.dtype_is_object)
@@ -5638,17 +5516,14 @@
 }
 
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getattr__", 0);
 
   /* "View.MemoryView":234
  * 
  *     def __getattr__(self, attr):
  *         return getattr(self.memview, attr)             # <<<<<<<<<<<<<<
  * 
@@ -5706,17 +5581,14 @@
 }
 
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
   /* "View.MemoryView":237
  * 
  *     def __getitem__(self, item):
  *         return self.memview[item]             # <<<<<<<<<<<<<<
  * 
@@ -5773,17 +5645,14 @@
   return __pyx_r;
 }
 
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_12__setitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
 
   /* "View.MemoryView":240
  * 
  *     def __setitem__(self, item, value):
  *         self.memview[item] = value             # <<<<<<<<<<<<<<
  * 
@@ -5833,17 +5702,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_array___reduce_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
@@ -5890,17 +5756,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_array_2__setstate_cython__(CYTHON_UNUSED struct __pyx_array_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
@@ -5940,17 +5803,14 @@
   struct __pyx_array_obj *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("array_cwrapper", 0);
 
   /* "View.MemoryView":248
  *     cdef array result
  * 
  *     if buf == NULL:             # <<<<<<<<<<<<<<
  *         result = array(shape, itemsize, format, mode.decode('ASCII'))
@@ -6110,17 +5970,14 @@
  *     def __repr__(self):
  */
 
 /* Python wrapper */
 static int __pyx_MemviewEnum___init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_MemviewEnum___init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_name,0};
     PyObject* values[1] = {0};
     if (unlikely(__pyx_kwds)) {
@@ -6274,17 +6131,14 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":5
  *     cdef object _dict
  *     cdef bint use_setstate
  *     state = (self.name,)             # <<<<<<<<<<<<<<
  *     _dict = getattr(self, '__dict__', None)
@@ -6502,17 +6356,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_MemviewEnum_2__setstate_cython__(struct __pyx_MemviewEnum_obj *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
@@ -6634,17 +6485,14 @@
 
 /* Python wrapper */
 static int __pyx_memoryview___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_memoryview___cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_obj = 0;
   int __pyx_v_flags;
   int __pyx_v_dtype_is_object;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__cinit__ (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_obj,&__pyx_n_s_flags,&__pyx_n_s_dtype_is_object,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -6717,17 +6565,14 @@
 static int __pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview___cinit__(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_obj, int __pyx_v_flags, int __pyx_v_dtype_is_object) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
   /* "View.MemoryView":346
  * 
  *     def __cinit__(memoryview self, object obj, int flags, bint dtype_is_object=False):
  *         self.obj = obj             # <<<<<<<<<<<<<<
  *         self.flags = flags
@@ -7251,17 +7096,14 @@
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   Py_ssize_t __pyx_t_6;
   char *__pyx_t_7;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_item_pointer", 0);
 
   /* "View.MemoryView":395
  *     cdef char *get_item_pointer(memoryview self, object index) except NULL:
  *         cdef Py_ssize_t dim
  *         cdef char *itemp = <char *> self.view.buf             # <<<<<<<<<<<<<<
  * 
@@ -7401,17 +7243,14 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   char *__pyx_t_6;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__getitem__", 0);
 
   /* "View.MemoryView":404
  * 
  *     def __getitem__(memoryview self, object index):
  *         if index is Ellipsis:             # <<<<<<<<<<<<<<
  *             return self
@@ -7587,17 +7426,14 @@
   PyObject *__pyx_v_obj = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setitem__", 0);
   __Pyx_INCREF(__pyx_v_index);
 
   /* "View.MemoryView":417
  * 
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:             # <<<<<<<<<<<<<<
@@ -7805,17 +7641,14 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_slice", 0);
   __Pyx_INCREF(__pyx_v_obj);
 
   /* "View.MemoryView":432
  * 
  *     cdef is_slice(self, obj):
  *         if not isinstance(obj, memoryview):             # <<<<<<<<<<<<<<
@@ -8014,17 +7847,14 @@
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   __Pyx_memviewslice *__pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assignment", 0);
 
   /* "View.MemoryView":445
  *         cdef __Pyx_memviewslice src_slice
  * 
  *         memoryview_copy_contents(get_slice_from_memview(src, &src_slice)[0],             # <<<<<<<<<<<<<<
  *                                  get_slice_from_memview(dst, &dst_slice)[0],
@@ -8113,17 +7943,14 @@
   char const *__pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   PyObject *__pyx_t_9 = NULL;
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   PyObject *__pyx_t_12 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_slice_assign_scalar", 0);
 
   /* "View.MemoryView":451
  *     cdef setitem_slice_assign_scalar(self, memoryview dst, value):
  *         cdef int array[128]
  *         cdef void *tmp = NULL             # <<<<<<<<<<<<<<
  *         cdef void *item
@@ -8389,17 +8216,14 @@
 
 static PyObject *__pyx_memoryview_setitem_indexed(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index, PyObject *__pyx_v_value) {
   char *__pyx_v_itemp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   char *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("setitem_indexed", 0);
 
   /* "View.MemoryView":482
  * 
  *     cdef setitem_indexed(self, index, value):
  *         cdef char *itemp = self.get_item_pointer(index)             # <<<<<<<<<<<<<<
  *         self.assign_item_from_object(itemp, value)
@@ -8461,17 +8285,14 @@
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   PyObject *__pyx_t_9 = NULL;
   size_t __pyx_t_10;
   int __pyx_t_11;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
   /* "View.MemoryView":488
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef bytes bytesitem
@@ -8742,17 +8563,14 @@
   PyObject *__pyx_t_8 = NULL;
   Py_ssize_t __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   char *__pyx_t_11;
   char *__pyx_t_12;
   char *__pyx_t_13;
   char *__pyx_t_14;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
   /* "View.MemoryView":504
  *         """Only used if instantiated manually by the user, or if Cython doesn't
  *         know how to convert the type"""
  *         import struct             # <<<<<<<<<<<<<<
  *         cdef char c
@@ -8984,17 +8802,14 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t *__pyx_t_4;
   char *__pyx_t_5;
   void *__pyx_t_6;
   int __pyx_t_7;
   Py_ssize_t __pyx_t_8;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   if (__pyx_v_info == NULL) {
     PyErr_SetString(PyExc_BufferError, "PyObject_GetBuffer: view==NULL argument is obsolete");
     return -1;
   }
   __Pyx_RefNannySetupContext("__getbuffer__", 0);
   __pyx_v_info->obj = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(__pyx_v_info->obj);
@@ -9323,17 +9138,14 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_1T___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   struct __pyx_memoryviewslice_obj *__pyx_v_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":554
  *     @property
  *     def T(self):
  *         cdef _memoryviewslice result = memoryview_copy(self)             # <<<<<<<<<<<<<<
  *         transpose_memslice(&result.from_slice)
@@ -9465,17 +9277,14 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":564
  *     @property
  *     def shape(self):
  *         return tuple([length for length in self.view.shape[:self.view.ndim]])             # <<<<<<<<<<<<<<
  * 
@@ -9547,17 +9356,14 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":568
  *     @property
  *     def strides(self):
  *         if self.view.strides == NULL:             # <<<<<<<<<<<<<<
  * 
@@ -9661,17 +9467,14 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   Py_ssize_t *__pyx_t_6;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":576
  *     @property
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:             # <<<<<<<<<<<<<<
  *             return (-1,) * self.view.ndim
@@ -9773,17 +9576,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_4ndim___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":583
  *     @property
  *     def ndim(self):
  *         return self.view.ndim             # <<<<<<<<<<<<<<
  * 
@@ -9836,17 +9636,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_8itemsize___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":587
  *     @property
  *     def itemsize(self):
  *         return self.view.itemsize             # <<<<<<<<<<<<<<
  * 
@@ -9901,17 +9698,14 @@
 
 static PyObject *__pyx_pf_15View_dot_MemoryView_10memoryview_6nbytes___get__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":591
  *     @property
  *     def nbytes(self):
  *         return self.size * self.view.itemsize             # <<<<<<<<<<<<<<
  * 
@@ -9979,17 +9773,14 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   Py_ssize_t *__pyx_t_4;
   Py_ssize_t *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
   /* "View.MemoryView":595
  *     @property
  *     def size(self):
  *         if self._size is None:             # <<<<<<<<<<<<<<
  *             result = 1
@@ -10195,17 +9986,14 @@
 
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_12__repr__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
   /* "View.MemoryView":612
  * 
  *     def __repr__(self):
  *         return "<MemoryView of %r at 0x%x>" % (self.base.__class__.__name__,             # <<<<<<<<<<<<<<
  *                                                id(self))
@@ -10296,17 +10084,14 @@
 }
 
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_14__str__(struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__str__", 0);
 
   /* "View.MemoryView":616
  * 
  *     def __str__(self):
  *         return "<MemoryView of %r object>" % (self.base.__class__.__name__,)             # <<<<<<<<<<<<<<
  * 
@@ -10377,17 +10162,14 @@
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_16is_c_contig(struct __pyx_memoryview_obj *__pyx_v_self) {
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_c_contig", 0);
 
   /* "View.MemoryView":622
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'C', self.view.ndim)
@@ -10453,17 +10235,14 @@
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_18is_f_contig(struct __pyx_memoryview_obj *__pyx_v_self) {
   __Pyx_memviewslice *__pyx_v_mslice;
   __Pyx_memviewslice __pyx_v_tmp;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_f_contig", 0);
 
   /* "View.MemoryView":628
  *         cdef __Pyx_memviewslice *mslice
  *         cdef __Pyx_memviewslice tmp
  *         mslice = get_slice_from_memview(self, &tmp)             # <<<<<<<<<<<<<<
  *         return slice_is_contig(mslice[0], 'F', self.view.ndim)
@@ -10529,17 +10308,14 @@
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_20copy(struct __pyx_memoryview_obj *__pyx_v_self) {
   __Pyx_memviewslice __pyx_v_mslice;
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy", 0);
 
   /* "View.MemoryView":633
  *     def copy(self):
  *         cdef __Pyx_memviewslice mslice
  *         cdef int flags = self.flags & ~PyBUF_F_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
@@ -10624,17 +10400,14 @@
   __Pyx_memviewslice __pyx_v_src;
   __Pyx_memviewslice __pyx_v_dst;
   int __pyx_v_flags;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_memviewslice __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("copy_fortran", 0);
 
   /* "View.MemoryView":645
  *     def copy_fortran(self):
  *         cdef __Pyx_memviewslice src, dst
  *         cdef int flags = self.flags & ~PyBUF_C_CONTIGUOUS             # <<<<<<<<<<<<<<
  * 
@@ -10713,17 +10486,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
@@ -10770,17 +10540,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
@@ -10818,17 +10585,14 @@
 static PyObject *__pyx_memoryview_new(PyObject *__pyx_v_o, int __pyx_v_flags, int __pyx_v_dtype_is_object, __Pyx_TypeInfo *__pyx_v_typeinfo) {
   struct __pyx_memoryview_obj *__pyx_v_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_cwrapper", 0);
 
   /* "View.MemoryView":658
  * @cname('__pyx_memoryview_new')
  * cdef memoryview_cwrapper(object o, int flags, bint dtype_is_object, __Pyx_TypeInfo *typeinfo):
  *     cdef memoryview result = memoryview(o, flags, dtype_is_object)             # <<<<<<<<<<<<<<
  *     result.typeinfo = typeinfo
@@ -10962,17 +10726,14 @@
   Py_ssize_t __pyx_t_5;
   PyObject *(*__pyx_t_6)(PyObject *);
   PyObject *__pyx_t_7 = NULL;
   Py_ssize_t __pyx_t_8;
   int __pyx_t_9;
   int __pyx_t_10;
   PyObject *__pyx_t_11 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_unellipsify", 0);
 
   /* "View.MemoryView":671
  *     full slices.
  *     """
  *     if not isinstance(index, tuple):             # <<<<<<<<<<<<<<
  *         tup = (index,)
@@ -11407,17 +11168,14 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t *__pyx_t_1;
   Py_ssize_t *__pyx_t_2;
   Py_ssize_t *__pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assert_direct_dimensions", 0);
 
   /* "View.MemoryView":701
  * 
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
  *     for suboffset in suboffsets[:ndim]:             # <<<<<<<<<<<<<<
  *         if suboffset >= 0:
@@ -11517,17 +11275,14 @@
   int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
   PyObject *(*__pyx_t_8)(PyObject *);
   PyObject *__pyx_t_9 = NULL;
   Py_ssize_t __pyx_t_10;
   int __pyx_t_11;
   Py_ssize_t __pyx_t_12;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memview_slice", 0);
 
   /* "View.MemoryView":711
  * @cname('__pyx_memview_slice')
  * cdef memoryview memview_slice(memoryview memview, object indices):
  *     cdef int new_ndim = 0, suboffset_dim = -1, dim             # <<<<<<<<<<<<<<
  *     cdef bint negative_step
@@ -12073,17 +11828,14 @@
 static int __pyx_memoryview_slice_memviewslice(__Pyx_memviewslice *__pyx_v_dst, Py_ssize_t __pyx_v_shape, Py_ssize_t __pyx_v_stride, Py_ssize_t __pyx_v_suboffset, int __pyx_v_dim, int __pyx_v_new_ndim, int *__pyx_v_suboffset_dim, Py_ssize_t __pyx_v_start, Py_ssize_t __pyx_v_stop, Py_ssize_t __pyx_v_step, int __pyx_v_have_start, int __pyx_v_have_stop, int __pyx_v_have_step, int __pyx_v_is_slice) {
   Py_ssize_t __pyx_v_new_shape;
   int __pyx_v_negative_step;
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
 
   /* "View.MemoryView":827
  *     cdef bint negative_step
  * 
  *     if not is_slice:             # <<<<<<<<<<<<<<
  * 
  *         if start < 0:
@@ -12862,17 +12614,14 @@
   char *__pyx_v_resultp;
   char *__pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("pybuffer_index", 0);
 
   /* "View.MemoryView":912
  * cdef char *pybuffer_index(Py_buffer *view, char *bufp, Py_ssize_t index,
  *                           Py_ssize_t dim) except NULL:
  *     cdef Py_ssize_t shape, stride, suboffset = -1             # <<<<<<<<<<<<<<
  *     cdef Py_ssize_t itemsize = view.itemsize
@@ -13175,17 +12924,14 @@
   long __pyx_t_3;
   long __pyx_t_4;
   Py_ssize_t __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
 
   /* "View.MemoryView":944
  * @cname('__pyx_memslice_transpose')
  * cdef int transpose_memslice(__Pyx_memviewslice *memslice) nogil except 0:
  *     cdef int ndim = memslice.memview.view.ndim             # <<<<<<<<<<<<<<
  * 
  *     cdef Py_ssize_t *shape = memslice.shape
@@ -13382,17 +13128,14 @@
  */
 
 static PyObject *__pyx_memoryviewslice_convert_item_to_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("convert_item_to_object", 0);
 
   /* "View.MemoryView":980
  * 
  *     cdef convert_item_to_object(self, char *itemp):
  *         if self.to_object_func != NULL:             # <<<<<<<<<<<<<<
  *             return self.to_object_func(itemp)
@@ -13469,17 +13212,14 @@
 
 static PyObject *__pyx_memoryviewslice_assign_item_from_object(struct __pyx_memoryviewslice_obj *__pyx_v_self, char *__pyx_v_itemp, PyObject *__pyx_v_value) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("assign_item_from_object", 0);
 
   /* "View.MemoryView":986
  * 
  *     cdef assign_item_from_object(self, char *itemp, object value):
  *         if self.to_dtype_func != NULL:             # <<<<<<<<<<<<<<
  *             self.to_dtype_func(itemp, value)
@@ -13614,17 +13354,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
@@ -13671,17 +13408,14 @@
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
@@ -13727,17 +13461,14 @@
   PyObject *__pyx_t_3 = NULL;
   __Pyx_TypeInfo *__pyx_t_4;
   Py_buffer __pyx_t_5;
   Py_ssize_t *__pyx_t_6;
   Py_ssize_t *__pyx_t_7;
   Py_ssize_t *__pyx_t_8;
   Py_ssize_t __pyx_t_9;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_fromslice", 0);
 
   /* "View.MemoryView":1007
  *     cdef _memoryviewslice result
  * 
  *     if <PyObject *> memviewslice.memview == Py_None:             # <<<<<<<<<<<<<<
  *         return None
@@ -14105,17 +13836,14 @@
 static __Pyx_memviewslice *__pyx_memoryview_get_slice_from_memoryview(struct __pyx_memoryview_obj *__pyx_v_memview, __Pyx_memviewslice *__pyx_v_mslice) {
   struct __pyx_memoryviewslice_obj *__pyx_v_obj = 0;
   __Pyx_memviewslice *__pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_slice_from_memview", 0);
 
   /* "View.MemoryView":1055
  *                                                    __Pyx_memviewslice *mslice) except NULL:
  *     cdef _memoryviewslice obj
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         obj = memview
@@ -14332,17 +14060,14 @@
  */
 
 static PyObject *__pyx_memoryview_copy_object(struct __pyx_memoryview_obj *__pyx_v_memview) {
   __Pyx_memviewslice __pyx_v_memviewslice;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy", 0);
 
   /* "View.MemoryView":1083
  *     "Create a new memoryview object"
  *     cdef __Pyx_memviewslice memviewslice
  *     slice_copy(memview, &memviewslice)             # <<<<<<<<<<<<<<
  *     return memoryview_copy_from_slice(memview, &memviewslice)
@@ -14397,17 +14122,14 @@
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *(*__pyx_t_3)(char *);
   int (*__pyx_t_4)(char *, PyObject *);
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("memoryview_copy_from_slice", 0);
 
   /* "View.MemoryView":1094
  *     cdef int (*to_dtype_func)(char *, object) except 0
  * 
  *     if isinstance(memview, _memoryviewslice):             # <<<<<<<<<<<<<<
  *         to_object_func = (<_memoryviewslice> memview).to_object_func
@@ -15242,17 +14964,14 @@
   void *__pyx_r;
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_t_3;
   struct __pyx_memoryview_obj *__pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
 
   /* "View.MemoryView":1219
  *     cdef void *result
  * 
  *     cdef size_t itemsize = src.memview.view.itemsize             # <<<<<<<<<<<<<<
  *     cdef size_t size = slice_get_size(src, ndim)
  * 
@@ -15492,17 +15211,14 @@
 static int __pyx_memoryview_err_extents(int __pyx_v_i, Py_ssize_t __pyx_v_extent1, Py_ssize_t __pyx_v_extent2) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_extents", 0);
 
   /* "View.MemoryView":1254
  *                              Py_ssize_t extent2) except -1 with gil:
@@ -15580,17 +15296,14 @@
 static int __pyx_memoryview_err_dim(PyObject *__pyx_v_error, char *__pyx_v_msg, int __pyx_v_dim) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err_dim", 0);
   __Pyx_INCREF(__pyx_v_error);
 
   /* "View.MemoryView":1258
@@ -15665,17 +15378,14 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_err", 0);
   __Pyx_INCREF(__pyx_v_error);
 
   /* "View.MemoryView":1262
@@ -15785,17 +15495,14 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   void *__pyx_t_7;
   int __pyx_t_8;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
 
   /* "View.MemoryView":1276
  *     Check for overlapping memory and verify the shapes.
  *     """
  *     cdef void *tmpdata = NULL             # <<<<<<<<<<<<<<
  *     cdef size_t itemsize = src.memview.view.itemsize
  *     cdef int i
@@ -16864,17 +16571,14 @@
 /* Python wrapper */
 static PyObject *__pyx_pw_15View_dot_MemoryView_1__pyx_unpickle_Enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static PyMethodDef __pyx_mdef_15View_dot_MemoryView_1__pyx_unpickle_Enum = {"__pyx_unpickle_Enum", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_15View_dot_MemoryView_1__pyx_unpickle_Enum, METH_VARARGS|METH_KEYWORDS, 0};
 static PyObject *__pyx_pw_15View_dot_MemoryView_1__pyx_unpickle_Enum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum (wrapper)", 0);
   {
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     PyObject* values[3] = {0,0,0};
     if (unlikely(__pyx_kwds)) {
@@ -16938,155 +16642,148 @@
 }
 
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
-  int __pyx_t_3;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  PyObject *__pyx_t_6 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+  int __pyx_t_6;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__19, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = (__pyx_t_2 != 0);
-  if (__pyx_t_3) {
+  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xb068931) != 0);
+  if (__pyx_t_1) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
+ *     if __pyx_checksum != 0xb068931:
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
-    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_t_1);
-    __pyx_v___pyx_PickleError = __pyx_t_1;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
+    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_v___pyx_PickleError = __pyx_t_2;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
+ *     if __pyx_checksum != 0xb068931:
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
-      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
-      if (likely(__pyx_t_6)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-        __Pyx_INCREF(__pyx_t_6);
+    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_5);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_1, function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
-    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xb068931:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
-    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
-    if (likely(__pyx_t_5)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
-      __Pyx_INCREF(__pyx_t_5);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_MemviewEnum_type), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_4 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
+    if (likely(__pyx_t_4)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+      __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_1, function);
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_4);
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_v___pyx_result = __pyx_t_4;
-  __pyx_t_4 = 0;
+  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v___pyx_result = __pyx_t_3;
+  __pyx_t_3 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_2 = (__pyx_t_3 != 0);
-  if (__pyx_t_2) {
+  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_6 = (__pyx_t_1 != 0);
+  if (__pyx_t_6) {
 
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
     if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_3 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xb068931 = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -17106,18 +16803,18 @@
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_AddTraceback("View.MemoryView.__pyx_unpickle_Enum", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
@@ -17139,17 +16836,14 @@
   int __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_Enum__set_state", 0);
 
   /* "(tree fragment)":12
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  *     __pyx_result.name = __pyx_state[0]             # <<<<<<<<<<<<<<
  *     if len(__pyx_state) > 1 and hasattr(__pyx_result, '__dict__'):
@@ -17283,17 +16977,17 @@
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
+    ++Py_REFCNT(o);
     __pyx_array___dealloc__(o);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
+    --Py_REFCNT(o);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->mode);
   Py_CLEAR(p->_format);
   (*Py_TYPE(o)->tp_free)(o);
 }
 static PyObject *__pyx_sq_item_array(PyObject *o, Py_ssize_t i) {
@@ -17433,23 +17127,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
@@ -17555,23 +17246,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -17600,17 +17288,17 @@
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
+    ++Py_REFCNT(o);
     __pyx_memoryview___dealloc__(o);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
+    --Py_REFCNT(o);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->obj);
   Py_CLEAR(p->_size);
   Py_CLEAR(p->_array_interface);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -17819,23 +17507,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
   PyObject *o = __pyx_tp_new_memoryview(t, a, k);
   if (unlikely(!o)) return 0;
@@ -17853,17 +17538,17 @@
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
+    ++Py_REFCNT(o);
     __pyx_memoryviewslice___dealloc__(o);
-    __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
+    --Py_REFCNT(o);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->from_object);
   PyObject_GC_Track(o);
   __pyx_tp_dealloc_memoryview(o);
 }
 
@@ -17968,23 +17653,20 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
-  0, /*tp_pypy_flags*/
-  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -18036,15 +17718,15 @@
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Emiliano_Gelati, __pyx_k_Emiliano_Gelati, sizeof(__pyx_k_Emiliano_Gelati), 0, 0, 1, 0},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
-  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xb0, __pyx_k_Incompatible_checksums_s_vs_0xb0, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xb0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
@@ -18383,151 +18065,146 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__18);
   __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_tuple__19 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":45
  * @boundscheck(False)
  * @wraparound(False)
  * def kinematicRouting(double[::1] discharge, double[::1] lateral_inflow, double[::1] constant, long[:,::1] upstream_lookup,\             # <<<<<<<<<<<<<<
  *                      long[::1] num_upstream_pixels, long[::1] ordered_pixels, long[:,::1] start_stop, double beta, double inv_beta,\
  *                      double b_minus_1, double[::1] a_dx_div_dt, double[::1] b_a_dx_div_dt, long num_threads):
  */
-  __pyx_tuple__20 = PyTuple_Pack(18, __pyx_n_s_discharge, __pyx_n_s_lateral_inflow, __pyx_n_s_constant, __pyx_n_s_upstream_lookup, __pyx_n_s_num_upstream_pixels, __pyx_n_s_ordered_pixels, __pyx_n_s_start_stop, __pyx_n_s_beta, __pyx_n_s_inv_beta, __pyx_n_s_b_minus_1, __pyx_n_s_a_dx_div_dt, __pyx_n_s_b_a_dx_div_dt, __pyx_n_s_num_threads, __pyx_n_s_order, __pyx_n_s_index, __pyx_n_s_first, __pyx_n_s_last, __pyx_n_s_num_orders); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 45, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(13, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_kinematicRouting, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(18, __pyx_n_s_discharge, __pyx_n_s_lateral_inflow, __pyx_n_s_constant, __pyx_n_s_upstream_lookup, __pyx_n_s_num_upstream_pixels, __pyx_n_s_ordered_pixels, __pyx_n_s_start_stop, __pyx_n_s_beta, __pyx_n_s_inv_beta, __pyx_n_s_b_minus_1, __pyx_n_s_a_dx_div_dt, __pyx_n_s_b_a_dx_div_dt, __pyx_n_s_num_threads, __pyx_n_s_order, __pyx_n_s_index, __pyx_n_s_first, __pyx_n_s_last, __pyx_n_s_num_orders); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(13, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_kinematicRouting, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 45, __pyx_L1_error)
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":108
  * # FLOW DIRECTION MATRIX PRE-PROCESSING FUNCTIONS
  * # -------------------------------------------------------------------------------------------------
  * def updateUpstreamRouted(long[::1] pixels_routed, long[::1] downstream_lookup,\             # <<<<<<<<<<<<<<
  *                          long[:,::1] upstream_lookup, unsigned char[:,::1] upstream_routed):
  *     """Called by kinematic_wave_parallel.orderKinematicRouting to implement greedy pixel ordering starting from headwaters."""
  */
-  __pyx_tuple__22 = PyTuple_Pack(7, __pyx_n_s_pixels_routed, __pyx_n_s_downstream_lookup, __pyx_n_s_upstream_lookup, __pyx_n_s_upstream_routed, __pyx_n_s_downs_pix, __pyx_n_s_pix, __pyx_n_s_ups_index); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 108, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_updateUpstreamRouted, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(7, __pyx_n_s_pixels_routed, __pyx_n_s_downstream_lookup, __pyx_n_s_upstream_lookup, __pyx_n_s_upstream_routed, __pyx_n_s_downs_pix, __pyx_n_s_pix, __pyx_n_s_ups_index); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 108, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(4, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_updateUpstreamRouted, 108, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 108, __pyx_L1_error)
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":121
  *             upstream_routed[downs_pix,ups_index] = True
  * 
  * def upDownLookups(long[:,::1] flow_d8, unsigned char[:,::1] land_mask, long[:,::1] land_points, long num_pixs, long[:,::1] ix_adds):             # <<<<<<<<<<<<<<
  *     '''Called by catchment.streamLookups'''
  *     cdef:
  */
-  __pyx_tuple__24 = PyTuple_Pack(16, __pyx_n_s_flow_d8, __pyx_n_s_land_mask, __pyx_n_s_land_points, __pyx_n_s_num_pixs, __pyx_n_s_ix_adds, __pyx_n_s_downstream_lookup, __pyx_n_s_upstream_lookup, __pyx_n_s_ups_count, __pyx_n_s_src_row, __pyx_n_s_src_col, __pyx_n_s_dst_row, __pyx_n_s_dst_col, __pyx_n_s_ups_p, __pyx_n_s_downs_p, __pyx_n_s_num_row, __pyx_n_s_num_col); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 121, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(5, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_upDownLookups, 121, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(16, __pyx_n_s_flow_d8, __pyx_n_s_land_mask, __pyx_n_s_land_points, __pyx_n_s_num_pixs, __pyx_n_s_ix_adds, __pyx_n_s_downstream_lookup, __pyx_n_s_upstream_lookup, __pyx_n_s_ups_count, __pyx_n_s_src_row, __pyx_n_s_src_col, __pyx_n_s_dst_row, __pyx_n_s_dst_col, __pyx_n_s_ups_p, __pyx_n_s_downs_p, __pyx_n_s_num_row, __pyx_n_s_num_col); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 121, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(5, 0, 16, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_upDownLookups, 121, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 121, __pyx_L1_error)
 
   /* "lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx":147
  * # MISCELLANOUS TOOLS
  * # -------------------------------------------------------------------------------------------------
  * def immediateUpstreamInflow(double[::1] discharge, long[:,::1] upstream_lookup, long[::1] num_upstream_pixels):             # <<<<<<<<<<<<<<
  *     """"""
  *     cdef:
  */
-  __pyx_tuple__26 = PyTuple_Pack(7, __pyx_n_s_discharge, __pyx_n_s_upstream_lookup, __pyx_n_s_num_upstream_pixels, __pyx_n_s_pix, __pyx_n_s_ups_ix, __pyx_n_s_num_pixels, __pyx_n_s_inflow); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 147, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_immediateUpstreamInflow, 147, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(7, __pyx_n_s_discharge, __pyx_n_s_upstream_lookup, __pyx_n_s_num_upstream_pixels, __pyx_n_s_pix, __pyx_n_s_ups_ix, __pyx_n_s_num_pixels, __pyx_n_s_inflow); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 147, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src_lisflood_hydrological_module, __pyx_n_s_immediateUpstreamInflow, 147, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 147, __pyx_L1_error)
 
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 286, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 286, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
 
   /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 291, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__33 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__32 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   /* InitThreads.init */
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
+  #ifdef WITH_THREAD
 PyEval_InitThreads();
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -18566,17 +18243,14 @@
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_array = &__pyx_vtable_array;
   __pyx_vtable_array.get_memview = (PyObject *(*)(struct __pyx_array_obj *))__pyx_array_get_memview;
   if (PyType_Ready(&__pyx_type___pyx_array) < 0) __PYX_ERR(1, 105, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
   __pyx_type___pyx_array.tp_print = 0;
@@ -18654,27 +18328,25 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#ifndef CYTHON_NO_PYINIT_EXPORT
-#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
-#elif PY_MAJOR_VERSION < 3
-#ifdef __cplusplus
-#define __Pyx_PyMODINIT_FUNC extern "C" void
-#else
+#if PY_MAJOR_VERSION < 3
+#ifdef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC void
-#endif
 #else
-#ifdef __cplusplus
-#define __Pyx_PyMODINIT_FUNC extern "C" PyObject *
+#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
+#endif
 #else
+#ifdef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyObject *
+#else
+#define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
 __Pyx_PyMODINIT_FUNC initkinematic_wave_parallel_tools(void) CYTHON_SMALL_CODE; /*proto*/
 __Pyx_PyMODINIT_FUNC initkinematic_wave_parallel_tools(void)
@@ -18749,17 +18421,14 @@
 
 static CYTHON_SMALL_CODE int __pyx_pymod_exec_kinematic_wave_parallel_tools(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
   PyObject *__pyx_t_1 = NULL;
   static PyThread_type_lock __pyx_t_2[8];
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
     PyErr_SetString(PyExc_RuntimeError, "Module 'kinematic_wave_parallel_tools' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
@@ -18799,17 +18468,19 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("kinematic_wave_parallel_tools", __pyx_methods, __pyx_k_Copyright_2019_European_Union_L, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -18838,22 +18509,22 @@
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
     if (!PyDict_GetItemString(modules, "lisflood.hydrological_modules.kinematic_wave_parallel_tools")) {
       if (unlikely(PyDict_SetItemString(modules, "lisflood.hydrological_modules.kinematic_wave_parallel_tools", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
-  if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedBuiltins() < 0) goto __pyx_L1_error;
   /*--- Constants init code ---*/
-  if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_InitCachedConstants() < 0) goto __pyx_L1_error;
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely(__Pyx_modinit_type_init_code() != 0)) goto __pyx_L1_error;
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
@@ -19007,71 +18678,71 @@
   /* "View.MemoryView":286
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 286, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 286, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":287
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":288
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":291
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 291, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 291, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":292
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "View.MemoryView":316
@@ -19272,15 +18943,15 @@
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
         #if PY_MAJOR_VERSION < 3
-        if (likely(PyString_Check(key))) {
+        if (likely(PyString_CheckExact(key)) || likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
@@ -19299,15 +18970,15 @@
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
                 int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                    (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                    (PyUnicode_GET_SIZE(**name) != PyUnicode_GET_SIZE(key)) ? 1 :
                 #endif
                     PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
@@ -19315,15 +18986,15 @@
             }
             if (*name) continue;
             else {
                 PyObject*** argname = argnames;
                 while (argname != first_kw_arg) {
                     int cmp = (**argname == key) ? 0 :
                     #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
-                        (__Pyx_PyUnicode_GET_LENGTH(**argname) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
+                        (PyUnicode_GET_SIZE(**argname) != PyUnicode_GET_SIZE(key)) ? 1 :
                     #endif
                         PyUnicode_Compare(**argname, key);
                     if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                     if (cmp == 0) goto arg_passed_twice;
                     argname++;
                 }
             }
@@ -19363,15 +19034,15 @@
                         __Pyx_memviewslice *memviewslice,
                         int memview_is_new_reference)
 {
     __Pyx_RefNannyDeclarations
     int i, retval=-1;
     Py_buffer *buf = &memview->view;
     __Pyx_RefNannySetupContext("init_memviewslice", 0);
-    if (unlikely(memviewslice->memview || memviewslice->data)) {
+    if (memviewslice->memview || memviewslice->data) {
         PyErr_SetString(PyExc_ValueError,
             "memviewslice is already initialized!");
         goto fail;
     }
     if (buf->strides) {
         for (i = 0; i < ndim; i++) {
             memviewslice->strides[i] = buf->strides[i];
@@ -19442,44 +19113,46 @@
     return result;
 }
 static CYTHON_INLINE void
 __Pyx_INC_MEMVIEW(__Pyx_memviewslice *memslice, int have_gil, int lineno)
 {
     int first_time;
     struct __pyx_memoryview_obj *memview = memslice->memview;
-    if (unlikely(!memview || (PyObject *) memview == Py_None))
+    if (!memview || (PyObject *) memview == Py_None)
         return;
-    if (unlikely(__pyx_get_slice_count(memview) < 0))
+    if (__pyx_get_slice_count(memview) < 0)
         __pyx_fatalerror("Acquisition count is %d (line %d)",
                          __pyx_get_slice_count(memview), lineno);
     first_time = __pyx_add_acquisition_count(memview) == 0;
-    if (unlikely(first_time)) {
+    if (first_time) {
         if (have_gil) {
             Py_INCREF((PyObject *) memview);
         } else {
             PyGILState_STATE _gilstate = PyGILState_Ensure();
             Py_INCREF((PyObject *) memview);
             PyGILState_Release(_gilstate);
         }
     }
 }
 static CYTHON_INLINE void __Pyx_XDEC_MEMVIEW(__Pyx_memviewslice *memslice,
                                              int have_gil, int lineno) {
     int last_time;
     struct __pyx_memoryview_obj *memview = memslice->memview;
-    if (unlikely(!memview || (PyObject *) memview == Py_None)) {
+    if (!memview ) {
+        return;
+    } else if ((PyObject *) memview == Py_None) {
         memslice->memview = NULL;
         return;
     }
-    if (unlikely(__pyx_get_slice_count(memview) <= 0))
+    if (__pyx_get_slice_count(memview) <= 0)
         __pyx_fatalerror("Acquisition count is %d (line %d)",
                          __pyx_get_slice_count(memview), lineno);
     last_time = __pyx_sub_acquisition_count(memview) == 1;
     memslice->data = NULL;
-    if (unlikely(last_time)) {
+    if (last_time) {
         if (have_gil) {
             Py_CLEAR(memslice->memview);
         } else {
             PyGILState_STATE _gilstate = PyGILState_Ensure();
             Py_CLEAR(memslice->memview);
             PyGILState_Release(_gilstate);
         }
@@ -19691,15 +19364,15 @@
 }
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -19778,15 +19451,15 @@
         return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
     if (likely(PyCFunction_Check(func))) {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
             return __Pyx_PyObject_CallMethO(func, arg);
 #if CYTHON_FAST_PYCCALL
-        } else if (__Pyx_PyFastCFunction_Check(func)) {
+        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
             return __Pyx_PyCFunction_FastCall(func, &arg, 1);
 #endif
         }
     }
     return __Pyx__PyObject_CallOneArg(func, arg);
 }
 #else
@@ -20020,15 +19693,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
+#if CYTHON_USE_UNICODE_INTERNALS
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -20149,15 +19822,15 @@
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(owned_ref);
     #endif
     return (equals == Py_NE);
 #endif
 }
 
-/* DivInt[Py_ssize_t] */
+/* None */
 static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t a, Py_ssize_t b) {
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
@@ -20308,17 +19981,17 @@
             start += length;
             if (start < 0)
                 start = 0;
         }
         if (stop < 0)
             stop += length;
     }
-    if (unlikely(stop <= start))
-        return __Pyx_NewRef(__pyx_empty_unicode);
     length = stop - start;
+    if (unlikely(length <= 0))
+        return PyUnicode_FromUnicode(NULL, 0);
     cstring += start;
     if (decode_func) {
         return decode_func(cstring, length, errors);
     } else {
         return PyUnicode_Decode(cstring, length, encoding, errors);
     }
 }
@@ -20585,15 +20258,15 @@
         goto bad;
     empty_dict = PyDict_New();
     if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
-            if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
+            if (strchr(__Pyx_MODULE_NAME, '.')) {
                 module = PyImport_ImportModuleLevelObject(
                     name, global_dict, empty_dict, list, 1);
                 if (!module) {
                     if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
@@ -20849,15 +20522,15 @@
 #endif
 
 /* None */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
     PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
 }
 
-/* DivInt[long] */
+/* None */
 static CYTHON_INLINE long __Pyx_div_long(long a, long b) {
     long q = a / b;
     long r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
@@ -20957,36 +20630,14 @@
     Py_DECREF(ob);
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
-/* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
 /* SetupReduce */
 static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
   name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name_2);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
@@ -20999,101 +20650,73 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
-    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
-    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
+    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto GOOD;
 #else
-    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
-    if (!getstate && PyErr_Occurred()) {
-        goto __PYX_BAD;
-    }
+    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto GOOD;
 #endif
-    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
 #else
-        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
-        if (!object_getstate && PyErr_Occurred()) {
-            goto __PYX_BAD;
-        }
+    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto BAD;
 #endif
-        if (object_getstate != getstate) {
-            goto __PYX_GOOD;
-        }
-    }
-#if CYTHON_USE_PYTYPE_LOOKUP
-    object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
-#else
-    object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
-#endif
-    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
+    reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto BAD;
     if (reduce_ex == object_reduce_ex) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+        object_reduce = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
 #else
-        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto __PYX_BAD;
+        object_reduce = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce); if (!object_reduce) goto BAD;
 #endif
-        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto __PYX_BAD;
+        reduce = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce); if (unlikely(!reduce)) goto BAD;
         if (reduce == object_reduce || __Pyx_setup_reduce_is_named(reduce, __pyx_n_s_reduce_cython)) {
-            reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
-            if (likely(reduce_cython)) {
-                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-            } else if (reduce == object_reduce || PyErr_Occurred()) {
-                goto __PYX_BAD;
-            }
+            reduce_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_cython); if (unlikely(!reduce_cython)) goto BAD;
+            ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto BAD;
+            ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto BAD;
             setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
-                setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
-                if (likely(setstate_cython)) {
-                    ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                    ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
-                } else if (!setstate || PyErr_Occurred()) {
-                    goto __PYX_BAD;
-                }
+                setstate_cython = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate_cython); if (unlikely(!setstate_cython)) goto BAD;
+                ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto BAD;
+                ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto BAD;
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
-    goto __PYX_GOOD;
-__PYX_BAD:
+    goto GOOD;
+BAD:
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
-__PYX_GOOD:
+GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
-    Py_XDECREF(object_getstate);
-    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -21115,15 +20738,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -21189,15 +20812,15 @@
         entries[pos].code_object = code_object;
         Py_DECREF(tmp);
         return;
     }
     if (__pyx_code_cache.count == __pyx_code_cache.max_count) {
         int new_max = __pyx_code_cache.max_count + 64;
         entries = (__Pyx_CodeObjectCacheEntry*)PyMem_Realloc(
-            __pyx_code_cache.entries, ((size_t)new_max) * sizeof(__Pyx_CodeObjectCacheEntry));
+            __pyx_code_cache.entries, (size_t)new_max*sizeof(__Pyx_CodeObjectCacheEntry));
         if (unlikely(!entries)) {
             return;
         }
         __pyx_code_cache.entries = entries;
         __pyx_code_cache.max_count = new_max;
     }
     for (i=__pyx_code_cache.count; i>pos; i--) {
@@ -21209,48 +20832,41 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = NULL;
-    PyObject *py_funcname = NULL;
+    PyCodeObject *py_code = 0;
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
     #if PY_MAJOR_VERSION < 3
-    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    if (!py_srcfile) goto bad;
+    #else
+    py_srcfile = PyUnicode_FromString(filename);
     #endif
+    if (!py_srcfile) goto bad;
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
-        funcname = PyUnicode_AsUTF8(py_funcname);
-        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        if (!py_funcname) goto bad;
+        #else
+        py_funcname = PyUnicode_FromString(funcname);
         #endif
     }
-    #if PY_MAJOR_VERSION < 3
+    if (!py_funcname) goto bad;
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -21261,49 +20877,34 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    #else
-    py_code = PyCode_NewEmpty(filename, funcname, py_line);
-    #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_DECREF(py_funcname);
     return py_code;
 bad:
-    Py_XDECREF(py_funcname);
-    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
-    #endif
+    Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -21743,23 +21344,24 @@
   ctx->is_complex = 0;
   return 0;
 }
 static PyObject *
 __pyx_buffmt_parse_array(__Pyx_BufFmt_Context* ctx, const char** tsp)
 {
     const char *ts = *tsp;
-    int i = 0, number, ndim;
+    int i = 0, number;
+    int ndim = ctx->head->field->type->ndim;
+;
     ++ts;
     if (ctx->new_count != 1) {
         PyErr_SetString(PyExc_ValueError,
                         "Cannot handle repeated arrays in format string");
         return NULL;
     }
     if (__Pyx_BufFmt_ProcessTypeChunk(ctx) == -1) return NULL;
-    ndim = ctx->head->field->type->ndim;
     while (*ts && *ts != ')') {
         switch (*ts) {
             case ' ': case '\f': case '\r': case '\n': case '\t': case '\v':  continue;
             default:  break;
         }
         number = __Pyx_BufFmt_ExpectNumber(&ts);
         if (number == -1) return NULL;
@@ -21881,16 +21483,16 @@
           return NULL;
         }
         CYTHON_FALLTHROUGH;
       case '?': case 'c': case 'b': case 'B': case 'h': case 'H': case 'i': case 'I':
       case 'l': case 'L': case 'q': case 'Q':
       case 'f': case 'd': case 'g':
       case 'O': case 'p':
-        if ((ctx->enc_type == *ts) && (got_Z == ctx->is_complex) &&
-            (ctx->enc_packmode == ctx->new_packmode) && (!ctx->is_valid_array)) {
+        if (ctx->enc_type == *ts && got_Z == ctx->is_complex &&
+            ctx->enc_packmode == ctx->new_packmode) {
           ctx->enc_count += ctx->new_count;
           ctx->new_count = 1;
           got_Z = 0;
           ++ts;
           break;
         }
         CYTHON_FALLTHROUGH;
@@ -21968,72 +21570,72 @@
 __pyx_check_strides(Py_buffer *buf, int dim, int ndim, int spec)
 {
     if (buf->shape[dim] <= 1)
         return 1;
     if (buf->strides) {
         if (spec & __Pyx_MEMVIEW_CONTIG) {
             if (spec & (__Pyx_MEMVIEW_PTR|__Pyx_MEMVIEW_FULL)) {
-                if (unlikely(buf->strides[dim] != sizeof(void *))) {
+                if (buf->strides[dim] != sizeof(void *)) {
                     PyErr_Format(PyExc_ValueError,
                                  "Buffer is not indirectly contiguous "
                                  "in dimension %d.", dim);
                     goto fail;
                 }
-            } else if (unlikely(buf->strides[dim] != buf->itemsize)) {
+            } else if (buf->strides[dim] != buf->itemsize) {
                 PyErr_SetString(PyExc_ValueError,
                                 "Buffer and memoryview are not contiguous "
                                 "in the same dimension.");
                 goto fail;
             }
         }
         if (spec & __Pyx_MEMVIEW_FOLLOW) {
             Py_ssize_t stride = buf->strides[dim];
             if (stride < 0)
                 stride = -stride;
-            if (unlikely(stride < buf->itemsize)) {
+            if (stride < buf->itemsize) {
                 PyErr_SetString(PyExc_ValueError,
                                 "Buffer and memoryview are not contiguous "
                                 "in the same dimension.");
                 goto fail;
             }
         }
     } else {
-        if (unlikely(spec & __Pyx_MEMVIEW_CONTIG && dim != ndim - 1)) {
+        if (spec & __Pyx_MEMVIEW_CONTIG && dim != ndim - 1) {
             PyErr_Format(PyExc_ValueError,
                          "C-contiguous buffer is not contiguous in "
                          "dimension %d", dim);
             goto fail;
-        } else if (unlikely(spec & (__Pyx_MEMVIEW_PTR))) {
+        } else if (spec & (__Pyx_MEMVIEW_PTR)) {
             PyErr_Format(PyExc_ValueError,
                          "C-contiguous buffer is not indirect in "
                          "dimension %d", dim);
             goto fail;
-        } else if (unlikely(buf->suboffsets)) {
+        } else if (buf->suboffsets) {
             PyErr_SetString(PyExc_ValueError,
                             "Buffer exposes suboffsets but no strides");
             goto fail;
         }
     }
     return 1;
 fail:
     return 0;
 }
 static int
 __pyx_check_suboffsets(Py_buffer *buf, int dim, CYTHON_UNUSED int ndim, int spec)
 {
     if (spec & __Pyx_MEMVIEW_DIRECT) {
-        if (unlikely(buf->suboffsets && buf->suboffsets[dim] >= 0)) {
+        if (buf->suboffsets && buf->suboffsets[dim] >= 0) {
             PyErr_Format(PyExc_ValueError,
                          "Buffer not compatible with direct access "
                          "in dimension %d.", dim);
             goto fail;
         }
     }
     if (spec & __Pyx_MEMVIEW_PTR) {
-        if (unlikely(!buf->suboffsets || (buf->suboffsets[dim] < 0))) {
+        if (!buf->suboffsets || (buf->suboffsets[dim] < 0)) {
             PyErr_Format(PyExc_ValueError,
                          "Buffer is not indirectly accessible "
                          "in dimension %d.", dim);
             goto fail;
         }
     }
     return 1;
@@ -22043,25 +21645,28 @@
 static int
 __pyx_verify_contig(Py_buffer *buf, int ndim, int c_or_f_flag)
 {
     int i;
     if (c_or_f_flag & __Pyx_IS_F_CONTIG) {
         Py_ssize_t stride = 1;
         for (i = 0; i < ndim; i++) {
-            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
+            if (stride * buf->itemsize != buf->strides[i] &&
+                    buf->shape[i] > 1)
+            {
                 PyErr_SetString(PyExc_ValueError,
                     "Buffer not fortran contiguous.");
                 goto fail;
             }
             stride = stride * buf->shape[i];
         }
     } else if (c_or_f_flag & __Pyx_IS_C_CONTIG) {
         Py_ssize_t stride = 1;
         for (i = ndim - 1; i >- 1; i--) {
-            if (unlikely(stride * buf->itemsize != buf->strides[i]  &&  buf->shape[i] > 1)) {
+            if (stride * buf->itemsize != buf->strides[i] &&
+                    buf->shape[i] > 1) {
                 PyErr_SetString(PyExc_ValueError,
                     "Buffer not C contiguous.");
                 goto fail;
             }
             stride = stride * buf->shape[i];
         }
     }
@@ -22094,46 +21699,44 @@
         memview = (struct __pyx_memoryview_obj *) __pyx_memoryview_new(
                                             original_obj, buf_flags, 0, dtype);
         new_memview = memview;
         if (unlikely(!memview))
             goto fail;
     }
     buf = &memview->view;
-    if (unlikely(buf->ndim != ndim)) {
+    if (buf->ndim != ndim) {
         PyErr_Format(PyExc_ValueError,
                 "Buffer has wrong number of dimensions (expected %d, got %d)",
                 ndim, buf->ndim);
         goto fail;
     }
     if (new_memview) {
         __Pyx_BufFmt_Init(&ctx, stack, dtype);
-        if (unlikely(!__Pyx_BufFmt_CheckString(&ctx, buf->format))) goto fail;
+        if (!__Pyx_BufFmt_CheckString(&ctx, buf->format)) goto fail;
     }
-    if (unlikely((unsigned) buf->itemsize != dtype->size)) {
+    if ((unsigned) buf->itemsize != dtype->size) {
         PyErr_Format(PyExc_ValueError,
                      "Item size of buffer (%" CYTHON_FORMAT_SSIZE_T "u byte%s) "
                      "does not match size of '%s' (%" CYTHON_FORMAT_SSIZE_T "u byte%s)",
                      buf->itemsize,
                      (buf->itemsize > 1) ? "s" : "",
                      dtype->name,
                      dtype->size,
                      (dtype->size > 1) ? "s" : "");
         goto fail;
     }
-    if (buf->len > 0) {
-        for (i = 0; i < ndim; i++) {
-            spec = axes_specs[i];
-            if (unlikely(!__pyx_check_strides(buf, i, ndim, spec)))
-                goto fail;
-            if (unlikely(!__pyx_check_suboffsets(buf, i, ndim, spec)))
-                goto fail;
-        }
-        if (unlikely(buf->strides && !__pyx_verify_contig(buf, ndim, c_or_f_flag)))
+    for (i = 0; i < ndim; i++) {
+        spec = axes_specs[i];
+        if (!__pyx_check_strides(buf, i, ndim, spec))
+            goto fail;
+        if (!__pyx_check_suboffsets(buf, i, ndim, spec))
             goto fail;
     }
+    if (buf->strides && !__pyx_verify_contig(buf, ndim, c_or_f_flag))
+        goto fail;
     if (unlikely(__Pyx_init_memviewslice(memview, ndim, memviewslice,
                                          new_memview != NULL) == -1)) {
         goto fail;
     }
     retval = 0;
     goto no_fail;
 fail:
@@ -22254,47 +21857,117 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(long) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(long) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(long),
+                                     little, !is_unsigned);
+    }
+}
+
 /* MemviewDtypeToObject */
   static CYTHON_INLINE PyObject *__pyx_memview_get_long(const char *itemp) {
     return (PyObject *) __Pyx_PyInt_From_long(*(long *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_long(const char *itemp, PyObject *obj) {
     long value = __Pyx_PyInt_As_long(obj);
     if ((value == (long)-1) && PyErr_Occurred())
         return 0;
     *(long *) itemp = value;
     return 1;
 }
 
-/* ObjectToMemviewSlice */
-  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_int(PyObject *obj, int writable_flag) {
-    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
-    __Pyx_BufFmt_StackElem stack[1];
-    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
-    int retcode;
-    if (obj == Py_None) {
-        result.memview = (struct __pyx_memoryview_obj *) Py_None;
-        return result;
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
+    const unsigned int neg_one = (unsigned int) ((unsigned int) 0 - (unsigned int) 1), const_zero = (unsigned int) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(unsigned int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(unsigned int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(unsigned int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(unsigned int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(unsigned int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
+                                     little, !is_unsigned);
+    }
+}
+
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_char(unsigned char value) {
+    const unsigned char neg_one = (unsigned char) ((unsigned char) 0 - (unsigned char) 1), const_zero = (unsigned char) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(unsigned char) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(unsigned char) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(unsigned char) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(unsigned char) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(unsigned char) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(unsigned char),
+                                     little, !is_unsigned);
     }
-    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
-                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 1,
-                                                 &__Pyx_TypeInfo_unsigned_int, stack,
-                                                 &result, obj);
-    if (unlikely(retcode == -1))
-        goto __pyx_fail;
-    return result;
-__pyx_fail:
-    result.memview = NULL;
-    result.data = NULL;
-    return result;
 }
 
 /* MemviewDtypeToObject */
   static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp) {
     return (PyObject *) PyFloat_FromDouble(*(double *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj) {
@@ -22319,15 +21992,15 @@
     Py_buffer *buf = &from_memview->view;
     PyObject *shape_tuple = NULL;
     PyObject *temp_int = NULL;
     struct __pyx_array_obj *array_obj = NULL;
     struct __pyx_memoryview_obj *memview_obj = NULL;
     __Pyx_RefNannySetupContext("__pyx_memoryview_copy_new_contig", 0);
     for (i = 0; i < ndim; i++) {
-        if (unlikely(from_mvs->suboffsets[i] >= 0)) {
+        if (from_mvs->suboffsets[i] >= 0) {
             PyErr_Format(PyExc_ValueError, "Cannot copy memoryview slice with "
                                            "indirect dimensions (axis %d)", i);
             goto fail;
         }
     }
     shape_tuple = PyTuple_New(ndim);
     if (unlikely(!shape_tuple)) {
@@ -22370,22 +22043,15 @@
     __Pyx_XDECREF(array_obj);
     __Pyx_RefNannyFinishContext();
     return new_mvs;
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -22564,62 +22230,17 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -22799,99 +22420,16 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_int(unsigned int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const unsigned int neg_one = (unsigned int) -1, const_zero = (unsigned int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(unsigned int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(unsigned int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(unsigned int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(unsigned int),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_unsigned_char(unsigned char value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const unsigned char neg_one = (unsigned char) -1, const_zero = (unsigned char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(unsigned char) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(unsigned char) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned char) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(unsigned char) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(unsigned char) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(unsigned char),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
         if (sizeof(int) < sizeof(long)) {
             return PyInt_FromLong((long) value);
         } else if (sizeof(int) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
@@ -22914,22 +22452,15 @@
         return _PyLong_FromByteArray(bytes, sizeof(int),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
   static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const char neg_one = (char) -1, const_zero = (char) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const char neg_one = (char) ((char) 0 - (char) 1), const_zero = (char) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
         if (sizeof(char) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(char, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
@@ -23108,43 +22639,44 @@
     return (char) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to char");
     return (char) -1;
 }
 
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_unsigned_int(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 1,
+                                                 &__Pyx_TypeInfo_unsigned_int, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -23394,31 +22926,14 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
-  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
-#if PY_MAJOR_VERSION < 3
-  } else if (likely(PyInt_CheckExact(o))) {
-    return PyInt_AS_LONG(o);
-#endif
-  } else {
-    Py_ssize_t ival;
-    PyObject *x;
-    x = PyNumber_Index(o);
-    if (!x) return -1;
-    ival = PyInt_AsLong(x);
-    Py_DECREF(x);
-    return ival;
-  }
-}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
```

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/kinematic_wave_parallel_tools.pyx`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/lakes.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/lakes.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/landusechange.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/landusechange.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/leafarea.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/leafarea.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/miscInitial.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/miscInitial.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/opensealed.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/opensealed.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/polder.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/polder.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/readmeteo.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/readmeteo.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/reservoir.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/reservoir.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/riceirrigation.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/riceirrigation.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/routing.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/routing.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/snow.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/snow.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/soil.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/soil.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/soilloop.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/soilloop.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/structures.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/structures.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/surface_routing.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/surface_routing.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/transmission.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/transmission.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/waterabstraction.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/waterabstraction.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/waterbalance.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/waterbalance.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/waterlevel.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/waterlevel.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/hydrological_modules/wateruse.py` & `lisflood-model-4.1.3/src/lisflood/hydrological_modules/wateruse.py`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood/main.py` & `lisflood-model-4.1.3/src/lisflood/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,21 +169,23 @@
     print('Version: ', __version__)
     print('Date: ', __date__)
     print('Status: ', __status__)
     print("""
     Arguments list:
     settings.xml     settings file
 
-    -q --quiet       output progression given as .
-    -v --veryquiet   no output progression is given
-    -l --loud        output progression given as time step, date and discharge
-    -c --check       input maps and stack maps are checked, output for each input map BUT no model run
-    -h --noheader    .tss file have no header and start immediately with the time series
-    -d --debug       debug outputs
-    -i --initonly    only run initialisation, not the dynamic loop
+    -q --quiet           output progression given as .
+    -v --veryquiet       no output progression is given
+    -l --loud            output progression given as time step, date and discharge
+    -c --checkfiles      input maps and stack maps are checked, output for each input map BUT no model run
+    -n --nancheck        check NaN values in output maps
+    -h --noheader        .tss file have no header and start immediately with the time series
+    -d --debug           debug outputs
+    -i --initonly        only run initialisation, not the dynamic loop
+    -s --skipvalreplace  skip replacement of invalid values in meteo input maps (ignore valid_min and valid_max)
     """)
     sys.exit(1)
 
 
 def headerinfo():
 
     print("LisfloodPy ", __version__, " ", __date__)
```

### Comparing `lisflood-model-4.1.2/src/lisfloodSettings_reference.xml` & `lisflood-model-4.1.3/src/lisfloodSettings_reference.xml`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood_model.egg-info/PKG-INFO` & `lisflood-model-4.1.3/src/lisflood_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lisflood-model
-Version: 4.1.2
+Version: 4.1.3
 Summary: LISFLOOD model python module
 Home-page: https://github.com/ec-jrc/lisflood-code
-Download-URL: https://github.com/ec-jrc/lisflood-code/archive/4.1.2.tar.gz
+Download-URL: https://github.com/ec-jrc/lisflood-code/archive/4.1.3.tar.gz
 Author: Ad de Roo, Emiliano Gelati, Peter Burek, Johan van der Knijff, Niko Wanders
 Author-email: carlo.russo@ext.ec.europa.eu
 License: EUPL 1.2
 Keywords: lisflood,lisvap,efas,glofas,copernicus,ecmwf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `lisflood-model-4.1.2/src/lisflood_model.egg-info/SOURCES.txt` & `lisflood-model-4.1.3/src/lisflood_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lisflood-model-4.1.2/src/lisflood_model.egg-info/requires.txt` & `lisflood-model-4.1.3/src/lisflood_model.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 more-itertools>=7.2.0
 netCDF4>=1.5.3
 nine>=1.0.0
 numba>=0.54.0
 numexpr>=2.7.0
 numpy>=1.21.0
 packaging>=19.2
-pandas>=0.25.1
+pandas>=1
 pathlib2>=2.3.5
 pkginfo>=1.5.0.1
 pluggy>=0.13.0
 py>=1.10.0
 pyparsing>=2.4.2
 pyproj>=2.4.0
 pytest>=6.2.5
@@ -34,8 +34,8 @@
 six>=1.12.0
 soupsieve>=1.9.5
 toml>=0.10.0
 tomli>=1.2.1
 toolz>=0.10.0
 xarray>=0.20.2
 zipp>=0.6.0
-GDAL==3.5.1
+GDAL==3.5.0
```

