# Comparing `tmp/CosmoTech-SupplyChain-4.1.2.tar.gz` & `tmp/CosmoTech-SupplyChain-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CosmoTech-SupplyChain-4.1.2.tar", last modified: Tue Jun 13 08:32:09 2023, max compression
+gzip compressed data, was "CosmoTech-SupplyChain-5.0.0.tar", last modified: Thu Jun 22 09:59:37 2023, max compression
```

## Comparing `CosmoTech-SupplyChain-4.1.2.tar` & `CosmoTech-SupplyChain-5.0.0.tar`

### file list

```diff
@@ -1,69 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.719530 CosmoTech-SupplyChain-4.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.711530 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2203 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-13 08:32:09.000000 CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.711530 CosmoTech-SupplyChain-4.1.2/Supplychain/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.711530 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adt_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_and_file_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/cosmo_api_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/duration.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_reader.py
--rw-r--r--   0 runner    (1001) docker     (122)      780 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/memory_folder_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/simulator_io.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/storage_queue_writer.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/cmaes_optimization_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/default_transformation.py
--rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/multiprocessing_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/objective_functions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/cmaes_optimization.py
--rw-r--r--   0 runner    (1001) docker     (122)    31357 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/local_sensitivity_analysis_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation_comets.py
--rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis.py
--rw-r--r--   0 runner    (1001) docker     (122)    33487 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis_comets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/adt_column_description.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/default_values.py
--rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/simulator_files_description.py
--rw-r--r--   0 runner    (1001) docker     (122)    20522 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/validation_schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/complete_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_table.py
--rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict_old.py
--rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/patch_dict_with_parameters.py
--rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/production_route.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/validate_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:09.715530 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/simulator.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:32:00.000000 CosmoTech-SupplyChain-4.1.2/Supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-13 08:32:09.719530 CosmoTech-SupplyChain-4.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      852 2023-06-13 08:32:01.000000 CosmoTech-SupplyChain-4.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2332 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-06-22 09:59:37.000000 CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1195 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      323 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3447 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/Supplychain/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adt_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1488 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_and_file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6620 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4451 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/cosmo_api_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3385 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/duration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1710 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1287 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1460 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)      780 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/memory_folder_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      679 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/simulator_io.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/storage_queue_writer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.608733 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1101 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/cmaes_optimization_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/default_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/multiprocessing_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)      761 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/objective_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2044 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5391 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/cmaes_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3232 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/consumers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31357 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/local_sensitivity_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1025 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20372 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/stochastic_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7760 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23910 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis_comets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22140 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis_helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6223 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/adt_column_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5318 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/default_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3149 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/simulator_files_description.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23192 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/validation_schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6539 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/complete_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39924 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11669 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6822 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52415 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict_old.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15303 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/patch_dict_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3058 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/production_route.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.612733 CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21965 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/validate_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1646 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18535 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/Supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 09:59:37.616733 CosmoTech-SupplyChain-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      851 2023-06-22 09:59:27.000000 CosmoTech-SupplyChain-5.0.0/setup.py
```

### Comparing `CosmoTech-SupplyChain-4.1.2/CosmoTech_SupplyChain.egg-info/SOURCES.txt` & `CosmoTech-SupplyChain-5.0.0/CosmoTech_SupplyChain.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,22 @@
 Supplychain/Protocol/cmaes_optimization_algorithm.py
 Supplychain/Protocol/default_transformation.py
 Supplychain/Protocol/multiprocessing_optimization.py
 Supplychain/Protocol/objective_functions.py
 Supplychain/Protocol/protocol.py
 Supplychain/Run/__init__.py
 Supplychain/Run/cmaes_optimization.py
+Supplychain/Run/consumers.py
 Supplychain/Run/local_sensitivity_analysis_comets.py
 Supplychain/Run/simulation.py
 Supplychain/Run/simulation_comets.py
+Supplychain/Run/stochastic_optimization.py
 Supplychain/Run/uncertainty_analysis.py
 Supplychain/Run/uncertainty_analysis_comets.py
+Supplychain/Run/uncertainty_analysis_helper_functions.py
 Supplychain/Schema/__init__.py
 Supplychain/Schema/adt_column_description.py
 Supplychain/Schema/default_values.py
 Supplychain/Schema/simulator_files_description.py
 Supplychain/Schema/validation_schemas.py
 Supplychain/Transform/__init__.py
 Supplychain/Transform/complete_dict.py
```

### Comparing `CosmoTech-SupplyChain-4.1.2/LICENSE` & `CosmoTech-SupplyChain-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/README.md` & `CosmoTech-SupplyChain-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adt_writer.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adt_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_and_file_writer.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_and_file_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/adx_wrapper.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/adx_wrapper.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/cosmo_api_parameters.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/cosmo_api_parameters.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_reader.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/csv_folder_writer.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/csv_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/duration.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/duration.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_reader.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/excel_folder_writer.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/excel_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/folder_io.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_reader.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_reader.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/json_folder_writer.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/json_folder_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/memory_folder_io.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/memory_folder_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/simulator_io.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/simulator_io.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/storage_queue_writer.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/storage_queue_writer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Generic/timer.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Generic/timer.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/cmaes_optimization_algorithm.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/cmaes_optimization_algorithm.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/default_transformation.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/default_transformation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/multiprocessing_optimization.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/multiprocessing_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/objective_functions.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/objective_functions.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Protocol/protocol.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/cmaes_optimization.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/cmaes_optimization.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/local_sensitivity_analysis_comets.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/local_sensitivity_analysis_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/simulation_comets.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/simulation_comets.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Run/uncertainty_analysis_comets.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Run/uncertainty_analysis_comets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,167 +1,272 @@
 import multiprocessing
 from typing import Union
 from copy import deepcopy
+
 import pandas
+import comets as co
+
 from Supplychain.Wrappers.simulator import CosmoEngine
 from Supplychain.Generic.adx_and_file_writer import ADXAndFileWriter
 from Supplychain.Generic.timer import Timer
-from Supplychain.Wrappers.environment_variables import EnvironmentVariables
 from Supplychain.Run.simulation import run_simple_simulation
-import comets as co
+from Supplychain.Run.consumers import (
+    StockConsumer,
+    PerformanceConsumer,
+    StocksFinalConsumer,
+)
+from Supplychain.Run.uncertainty_analysis_helper_functions import (
+    get_max_time_step,
+    get_attribute,
+    get_stocks,
+    get_transports,
+    collect_transport_information,
+    extend_dic,
+    add_tag_to_parameterset,
+    collect_simulated_stock_final_output,
+    collect_simulated_stock_output,
+    collect_simulated_transport_output,
+    transform_transport_data,
+    transform_stock_data,
+    transform_stocksfinal_data,
+    create_transport_distribution_sampling,
+    create_demand_generator,
+)
+
+
+class UncertaintyAnalyzer:
+    """
+    Object in charge of performing the different steps of the uncertainty analysis.
+    Its main method is "execute".
+
+    Args:
+        simulation_name (str): Name of simulation, used by the probes
+        simulation_path (str): Name of the simulation file (typically Simulation)
+        sample_size (int): Number of simulations runs by the uncertainty analysis
+        batch_size (int): Number of simulations runs that are run in a same batch by the uncertainty analysis
+        amqp_consumer_adress (Union[str, None], optional): Adress of consumer to send probe results to. Defaults to None.
+        consumers (list, optional): Which consumers are activated. Defaults to ["Stocks", "Transport", "Performances", "StocksFinal", "PerformanceAMQP"].
+        validation_folder (str, optional): Local folder to which results are written to, used by the tests. Defaults to None.
+        cold_inputs (dict, optional): Parameters that are passed to the simulator at each simulation and don't change during the analysis. Defaults to {}.
+        timer (Timer object, optional): Timer object that can be used for logs and counting time. Defaults to None.
+    """
+
+    def __init__(
+        self,
+        simulation_name,
+        simulation_path,
+        sample_size,
+        batch_size,
+        amqp_consumer_adress=None,
+        consumers=["Stocks", "Transport", "Performances", "StocksFinal"],
+        validation_folder=None,
+        cold_inputs={},
+        timer=None,
+        n_jobs=-1,
+    ):
+        if timer is None:
+            self.t = Timer("[Run Uncertainty]")
+        else:
+            self.t = timer
+        self.simulation_name = simulation_name
+        self.simulation_path = simulation_path
+        self.amqp_consumer_adress = amqp_consumer_adress
+        self.sample_size = sample_size
+        self.batch_size = batch_size
+        self.validation_folder = validation_folder
+        self.consumers = consumers
+        self.cold_inputs = cold_inputs
 
+        if self.batch_size > self.sample_size:
+            self.batch_size = self.sample_size
 
-def uncertainty_analysis(
-    simulation_name: str,
-    simulation_path: str = "Simulation",
-    amqp_consumer_adress: Union[str, None] = None,
-    sample_size: int = 1000,
-    batch_size: int = 100,
-    adx_writer: Union[ADXAndFileWriter, None] = None,
-    validation_folder: Union[str, None] = None,
-):
-
-    with Timer("[Run Uncertainty]") as t:
-        if batch_size > sample_size:
-            batch_size = sample_size
-
-        processes_size = min(multiprocessing.cpu_count(), batch_size)
-
-        used_probes = ["PerformanceIndicators", "Stocks"]
-        used_consumers = ["PerformanceIndicatorsAMQP"]
-
-        class StockConsumer:
-            def __init__(self):
-                self.memory = list()
-
-            def Consume(self, p_data):
-                probe_output = self.engine.StocksProbeOutput.Cast(p_data)
-                f = probe_output.GetFacts()
-                timestep = int(
-                    probe_output.GetProbeRunDimension().GetProbeOutputCounter()
-                )
-                for data in f:
-                    fact = [
-                        str(data.GetAttributeAsString("ID")),
-                        timestep,
-                        float(data.GetAttributeAsFloat64("Demand")),
-                        float(data.GetAttributeAsFloat64("RemainingQuantity")),
-                        float(data.GetAttributeAsFloat64("ServedQuantity")),
-                        float(data.GetAttributeAsFloat64("UnservedQuantity")),
-                    ]
-                    self.memory.append(fact)
+        if n_jobs == -1:
+            self.processes_size = min(multiprocessing.cpu_count(), self.batch_size)
+        else:
+            self.processes_size = n_jobs
 
-        class PerformanceConsumer:
-            """
-            Python Consumer for performance indicators.
-            Currently not used by the solution (results are also sent directly to ADX through the PerformanceIndicatorsAMQP consumer),
-            but available for the future and for local computation of performance indicators statistics.
-            """
+    def execute(self):
+        """Setup and run the uncertainty analysis
 
-            def __init__(self):
-                self.memory = list()
+        Returns:
+            dict: dictionary with keys among ["Stock", "Transport", "Performances", "StocksFinal"]
+                containing the output tables. Which table is available depends on the specified
+                consumers of the UncertaintyAnalyzer.
+        """
+        self.t.split("Initialize uncertainty analysis")
+        self.initialize_simulator_interface()
+        self.collect_simulation_parameters()
+        self.create_encoder()
+        self.create_get_outcomes()
+        self.create_sampling()
+        self.create_task(self.cold_inputs)
+        self.t.split(
+            "Ended uncertainty analysis initialization : {time_since_last_split}"
+        )
 
-            def Consume(self, p_data):
-                probe_output = self.engine.PerformanceIndicatorsProbeOutput.Cast(p_data)
-                f = probe_output.GetFacts()
-                for data in f:
-                    fact = {
-                        "OPEX": float(data.GetAttributeAsFloat64("OPEX")),
-                        "Profit": float(data.GetAttributeAsFloat64("Profit")),
-                        "AverageStockValue": float(
-                            data.GetAttributeAsFloat64("AverageStockValue")
-                        ),
-                        "ServiceLevelIndicator": float(
-                            data.GetAttributeAsFloat64("ServiceLevelIndicator")
-                        ),
-                        "CO2Emissions": float(
-                            data.GetAttributeAsFloat64("CO2Emissions")
-                        ),
-                        "TotalDemand": float(data.GetAttributeAsFloat64("TotalDemand")),
-                        "TotalServedQuantity": float(
-                            data.GetAttributeAsFloat64("TotalServedQuantity")
-                        ),
-                    }
-                    self.memory.append(fact)
+        self.t.display_message("Run uncertainty analysis")
+        self.run_experiment()
+        self.t.split("Ended uncertainty analysis run : {time_since_last_split}")
+
+        self.t.display_message("Reformat uncertainty analysis results")
+        self.reformat_results()
+        if self.validation_folder:
+            self.write_results_locally()
+        self.t.split(
+            "Ended uncertainty analysis reformatting : {time_since_last_split}"
+        )
 
-        size_of_performance_consumer = 7  # Number of KPIs in PerformanceConsumer
+        return self.results
 
-        simulator_interface = co.CosmoInterface(
-            simulator_path=simulation_path,
-            custom_sim_engine=CosmoEngine,
-            simulation_name=simulation_name,
-            amqp_consumer_address=amqp_consumer_adress,
-            used_consumers=used_consumers,
-            used_probes=used_probes,
-            custom_consumers=[
-                (StockConsumer, "LocalConsumer", "Stocks"),
+    def initialize_simulator_interface(self):
+        used_probes = []
+        used_consumers = []
+        custom_consumers = []
+
+        if "Stocks" in self.consumers:
+            used_probes.append("Stocks")
+            custom_consumers.append((StockConsumer, "LocalConsumer", "Stocks"))
+        if "StocksFinal" in self.consumers:
+            used_probes.append("StocksFinal")
+            custom_consumers.append(
+                (StocksFinalConsumer, "StocksFinalConsumer", "StocksFinal")
+            )
+        if "Performances" in self.consumers:
+            used_probes.append("PerformanceIndicators")
+            custom_consumers.append(
                 (
                     PerformanceConsumer,
                     "LocalPerformanceConsumer",
                     "PerformanceIndicators",
-                ),
-            ],
+                )
+            )
+        if "PerformanceAMQP" in self.consumers:
+            used_consumers.append("PerformanceIndicatorsAMQP")
+
+        self.simulator_interface = co.CosmoInterface(
+            simulator_path=self.simulation_path,
+            custom_sim_engine=CosmoEngine,
+            simulation_name=self.simulation_name,
+            amqp_consumer_address=self.amqp_consumer_adress,
+            used_consumers=used_consumers,
+            used_probes=used_probes,
+            custom_consumers=custom_consumers,
         )
 
+    def collect_simulation_parameters(self):
+        """
+        Collect values of attributes of the model
+        Used to retrieve the probability distribution parameters, the theoretical transport duration, etc...
+        """
         # Load simulator to be able to access attributes of the model
-        simulator_interface.initialize()
+        self.simulator_interface.initialize()
+
+        # Retrieving model information
+        self.max_time_step = get_max_time_step(self.simulator_interface)
+        self.ActivateCorrelatedDemandUncertainties = get_attribute(
+            self.simulator_interface, "Model::@ActivateCorrelatedDemandUncertainties"
+        )
+        self.DemandCorrelations = get_attribute(
+            self.simulator_interface, "Model::@DemandCorrelations"
+        )
+        self.transport_distribution = get_attribute(
+            self.simulator_interface,
+            "Model::@TransportUncertaintiesProbabilityDistribution",
+        )
+        self.ActivateUncertainties = get_attribute(
+            self.simulator_interface,
+            "Model::@ActivateUncertainties",
+        )
+
+        # Getting the name of all the stocks with uncertain demand
+        if self.ActivateCorrelatedDemandUncertainties:
+            self.uncertain_stocks = get_stocks(self.simulator_interface)
+        else:
+            self.uncertain_stocks = []
 
         # Getting the name of all the transport operations
-        all_transports = get_transports(simulator_interface.sim)
+        self.all_transports = get_transports(self.simulator_interface)
 
-        # Retrieving model information
+        # Collect information about transports:
+        # which transport have uncertain durations, what are the schedule for the theoretical transport duration
+        # and for the parameters of the probability distribution
         (
-            max_time_step,
-            distribution,
-            actual_duration_schedule,
-            list_of_transports,
+            self.transports_with_uncertain_duration,
+            self.actual_duration_schedule,
             uncertainty_param_1,
             uncertainty_param_2,
             uncertainty_param_3,
             uncertainty_param_4,
-            demands,
-            ActivateCorrelatedDemandUncertainties,
-            DemandCorrelations,
-            uncertain_stocks,
-        ) = model_info(simulator_interface, simulation_path, all_transports)
-
-        simulator_interface.terminate()
-
-        distribution_params = get_distribution_parameter(distribution)
-
-        # Extending the dictionaries above (scheduled attributes)
-        extended_actual_duration = extend_dic(actual_duration_schedule, max_time_step)
-        extended_param_1 = extend_dic(uncertainty_param_1, max_time_step)
-        extended_param_2 = extend_dic(uncertainty_param_2, max_time_step)
-        extended_param_3 = extend_dic(uncertainty_param_3, max_time_step)
-        extended_param_4 = extend_dic(uncertainty_param_4, max_time_step)
-        extended_demands = extend_dic(demands, max_time_step)
+        ) = collect_transport_information(self.simulator_interface, self.all_transports)
 
-        def encoder(parameters):
+        # Collect model information about demands of each stock
+        demands = {}
+        for stock in self.uncertain_stocks:
+            demands[stock] = get_attribute(
+                self.simulator_interface,
+                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{stock}::@Demand",
+            )
+
+        self.simulator_interface.terminate()
+        self.transport_distribution_params = co.DistributionRegistry.information[
+            str(self.transport_distribution)
+        ]["parameters"]
+
+        # Extending the dictionaries above for scheduled attributes so that all time steps are present
+        self.extended_actual_duration = extend_dic(
+            self.actual_duration_schedule, self.max_time_step
+        )
+        self.extended_param_1 = extend_dic(uncertainty_param_1, self.max_time_step)
+        self.extended_param_2 = extend_dic(uncertainty_param_2, self.max_time_step)
+        self.extended_param_3 = extend_dic(uncertainty_param_3, self.max_time_step)
+        self.extended_param_4 = extend_dic(uncertainty_param_4, self.max_time_step)
+        self.extended_demands = extend_dic(demands, self.max_time_step)
+
+        if not self.ActivateUncertainties:
+            # Remove uncertain transports and stocks if ActivateUncertainties is false
+            self.transports_with_uncertain_duration = []
+            self.uncertain_stocks = []
+
+    def create_encoder(self):
+        """Create encoder of the task"""
+
+        def encoder(
+            parameters,
+            extended_demands=self.extended_demands,
+            transports_with_uncertain_duration=self.transports_with_uncertain_duration,
+            extended_actual_duration=self.extended_actual_duration,
+            uncertain_stocks=self.uncertain_stocks,
+            max_time_step=self.max_time_step,
+        ):
             """
             The encoder takes a parameterset containing the input parameters that are changing at each simulation.
             It has the following format :
-            {'{Model} [..] Seed': 3251851028, 'T_@_0': 1.7504164949122698, 'T_@_1': 3.05256524351985, [...], 'T_@_10': 3.2371899035525793, 'StockA':[1.1, 2., ..., 3.4]}
+            {'{Model} [..] Seed': 3251851028, 'T_@_0': 1.7504164949122698, 'T_@_1': 3.05256524351985, [...],
+            'T_@_10': 3.2371899035525793, 'StockA':[1.1, 2., ..., 3.4]}
             The parameters correspond either to:
             - the Seed datapath and its value
             - transport_name +_@_ + time_step, and the duration of this transport at this time step
             - stock_name, and a list of demands for this stock
-
             It returns a parameterset where the keys are datapaths in the model.
             The values for each transport's duration is transformed in one dictionary {TimeStep: value} and updated as follows:
-            new_transport_duration = max(0, round(old_transport_duration + sample input drawn from the distribution))
-            The values for each stock's demand is set to its ExternalDemand in the attribute Demand, which is a dictionary {TimeStep: Composite attribute}.
-            {'Model [..] T::@ActualDurationSchedule': {'0': 5, '1': 6, [..] '10': 44}, '{Model}Model::{Attribute}Seed': 3209521878, ...}
+            new_transport_duration = max(0, round(old_transport_duration +
+                sample input drawn from the distribution))
+            The values for each stock's demand is set to its ExternalDemand in the attribute Demand, which is a dictionary
+            {TimeStep: Composite attribute}.
+            {'Model [..] T::@ActualDurationSchedule': {'0': 5, '1': 6, [..] '10': 44},
+                '{Model}Model::{Attribute}Seed': 3209521878, ...}
             """
-            encoded_parameterset = {
-                "{Model}Model::{Attribute}Seed": parameters[
-                    "{Model}Model::{Attribute}Seed"
-                ],
-            }
-            for transports in list_of_transports:
+            encoded_parameterset = {}
+            if "{Model}Model::{Attribute}Seed" in parameters:
+                encoded_parameterset = {
+                    "{Model}Model::{Attribute}Seed": parameters[
+                        "{Model}Model::{Attribute}Seed"
+                    ],
+                }
+            for transports in transports_with_uncertain_duration:
                 ActualDurationSchedule = {}
                 for i in range(len(extended_actual_duration[transports])):
                     ActualDurationSchedule[str(i)] = max(
                         0,
                         round(
                             extended_actual_duration[transports][i]
                             + parameters[f"{transports}_@_{i}"]
@@ -176,640 +281,279 @@
                 for i in range(max_time_step):
                     demand_attribute[i]["ExternalDemand"] = sample_demand[i]
                 encoded_parameterset[
                     f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{stock}::@Demand"
                 ] = demand_attribute
             return encoded_parameterset
 
-        def get_outcomes(modelinterface):
+        self.encoder = encoder
+
+    def create_get_outcomes(self):
+        """Create the get_outcomes function of the task"""
+
+        def get_outcomes(
+            modelinterface,
+            consumers=self.consumers,
+            all_transports=self.all_transports,
+            max_time_step=self.max_time_step,
+        ):
             """
             Returns a parameter set with all the model's output. More precisely, the parameter set is the
-            the result of the concatenation of three parameter sets.
-
+            the result of the concatenation of up to four parameter sets, depending on the consumers that have been chosen.
+            In front of the name of each parameter, we add a '1_', '2_', '3_' or '4_' to identify the 4 original parametersets.
             The first one looks like this:
-            {'U__&@&__0': 5, 'U__&@&__1': 5, [...], 'U__&@&__10': 6}. The keys correspond to transport_name + __&@&__ + time_step,
+            {'1_U__&@&__0': 5, '1_U__&@&__1': 5, [...], '1_U__&@&__10': 6}.
+            The keys correspond to transport_name + __&@&__ + time_step,
             and the value to the duration of the transport at this time step.
-
             The second parameter set looks like this:
-            {'A__&@&__ServedQuantity__&@&__0': 0.0, 'A__&@&__UnservedQuantity__&@&__0': 0.0}. The keys correspond to stock + __&@&__ + category + time_step
-
-            The third parameter set contains the performance indicators (OPEX, Profit, ...).
+            {'2_A__&@&__ServedQuantity__&@&__0': 0.0, '2_A__&@&__UnservedQuantity__&@&__0': 0.0}.
+            The keys correspond to stock + __&@&__ + category (Demand, ServedQuantity,...)  + __&@&__ +  time_step
+            The third parameter set contains the performance indicators {'3_OPEX': 0.0, '3_Profit': 1.0, ...}.
+            The fourth parameter set looks like:
+            {'4_A__&@&__TotalDemand': 1.0}.
+            The keys correspond to stock name + __&@&__ + category (TotalDemand, TotalServedQuantity, ServiceLevelSatisfaction)
             """
-            transport_duration = get_transport_duration(
-                all_transports, modelinterface, max_time_step
-            )
-            transports_and_consumer = {
-                **transport_duration,
-                **transform_consumer_memory(modelinterface.LocalConsumer.memory),
+
+            output_parameterset = {}
+            if "Transports" in consumers:
+                output_parameterset.update(
+                    add_tag_to_parameterset(
+                        "1_",
+                        collect_simulated_transport_output(
+                            all_transports, modelinterface, max_time_step
+                        ),
+                    )
+                )
+            if "Stocks" in consumers:
+                output_parameterset.update(
+                    add_tag_to_parameterset(
+                        "2_",
+                        collect_simulated_stock_output(
+                            modelinterface.LocalConsumer.memory
+                        ),
+                    )
+                )
+            if "Performances" in consumers:
+                output_parameterset.update(
+                    add_tag_to_parameterset(
+                        "3_", modelinterface.LocalPerformanceConsumer.memory[0]
+                    )
+                )
+            if "StocksFinal" in consumers:
+                output_parameterset.update(
+                    add_tag_to_parameterset(
+                        "4_",
+                        collect_simulated_stock_final_output(
+                            modelinterface.StocksFinalConsumer.memory
+                        ),
+                    )
+                )
+            return output_parameterset
+
+        self.get_outcomes = get_outcomes
+
+    def create_sampling(self):
+        """Create the sampling of the uncertainty analysis"""
+        # Creating the sampling on transport durations
+        self.sampling = create_transport_distribution_sampling(
+            self.transport_distribution,
+            self.extended_param_1,
+            self.extended_param_2,
+            self.extended_param_3,
+            self.extended_param_4,
+            self.transports_with_uncertain_duration,
+            self.transport_distribution_params,
+            self.max_time_step,
+        )
+        # Add the seed as an uncertain parameter
+        self.sampling.append(
+            {
+                "name": "{Model}Model::{Attribute}Seed",
+                "sampling": "seed_generator",
             }
-            performances = modelinterface.LocalPerformanceConsumer.memory[0]
-            transports_and_consumer.update(performances)
-            return transports_and_consumer
+        )
+
+        # Add the generator of samples on the demand
+        if self.ActivateCorrelatedDemandUncertainties:
+            self.sampling += create_demand_generator(
+                self.extended_demands, self.max_time_step, self.DemandCorrelations
+            )
+
+    def create_task(self, cold_inputs={}):
+        """Create the task on which the uncertainty analysis will be performed
 
+        Args:
+            cold_inputs (dict): ParameterSet containing parameters of the simulator
+                that will be applied to each evaluation of the task.
+                Allows to modify other attributes than those modified by the uncertainty analysis.
+        """
         if (
-            ActivateCorrelatedDemandUncertainties
+            self.ActivateCorrelatedDemandUncertainties
         ):  # Correlated demands are not compatible with demands drawn inside the model
             cold_input_parameter_set = {
                 "{Model}Model::{Attribute}ActivateUncertainties": 0
             }
         else:
             cold_input_parameter_set = {}
 
-        simulationtask = co.ModelTask(
-            modelinterface=simulator_interface,
-            encode=encoder,
-            get_outcomes=get_outcomes,
-            cold_input_parameter_set=cold_input_parameter_set,
-        )
+        cold_input_parameter_set.update(cold_inputs)
 
-        # Creating the uncertainty analysis sampling
-        sampling = creating_transport_distribution_space(
-            distribution,
-            extended_param_1,
-            extended_param_2,
-            extended_param_3,
-            extended_param_4,
-            list_of_transports,
-            distribution_params,
-            max_time_step,
-        )
-        # adding the seed as an uncertain parameter
-        sampling.append(
-            {
-                "name": "{Model}Model::{Attribute}Seed",
-                "sampling": "seed_generator",
-            }
+        self.simulationtask = co.ModelTask(
+            modelinterface=self.simulator_interface,
+            encode=self.encoder,
+            get_outcomes=self.get_outcomes,
+            cold_input_parameter_set=cold_input_parameter_set,
         )
 
-        # adding the generator of samples on the demand
-        if ActivateCorrelatedDemandUncertainties:
-            sampling += creating_demand_generator(
-                extended_demands, max_time_step, DemandCorrelations
-            )
-
-        if validation_folder is not None:
+    def run_experiment(self):
+        """Create and run the uncertainty analysis experiment"""
+        if self.validation_folder is not None:
             save_task_history = True
         else:
             save_task_history = False
 
-        experiment = co.UncertaintyAnalysis(
-            task=simulationtask,
-            sampling=sampling,
-            stop_criteria={"max_evaluations": sample_size},
+        self.experiment = co.UncertaintyAnalysis(
+            task=self.simulationtask,
+            sampling=self.sampling,
+            stop_criteria={"max_evaluations": self.sample_size},
             analyzer=["standard", "quantiles"],
-            n_jobs=processes_size,
+            n_jobs=self.processes_size,
             save_task_history=save_task_history,
         )
 
-        t.display_message("Starting simulations")
-        experiment.run()
-        t.split("Ended simulations : {time_since_start}")
-
-        # Separating the results data on the stock from the results data on transport's duration from the results data on performances
-        transport_limiter = len(all_transports) * max_time_step
-        df_transport_duration = experiment.results["statistics"].iloc[
-            0:transport_limiter, :
-        ]  # First transport_limiter rows are results about transport durations
-        df_probe_data = experiment.results["statistics"].iloc[
-            transport_limiter:-size_of_performance_consumer, :
-        ]  # Next are results about stocks levels
-        # Last rows are general performances, not sent to ADX since the performance indicators are also sent directly by the AMQP consumer
-        # This object is unused for now, but might be used in the future
-        performances = experiment.results["statistics"].iloc[
-            -size_of_performance_consumer:, :
-        ]  # noqa
-
-        df_probe_data.reset_index(inplace=True)
-        df_transport_duration.reset_index(inplace=True)
-
-        # Transforming the data on both the stock and the transport duration
-        df_stock_final = transform_stock_data(df_probe_data)
-        df_transport_final = transform_transport_data(df_transport_duration)
-
-        if validation_folder:
-            # Writing the results locally in csv files
-
-            # Get all demands directly from the experiment, before aggregation of statistics
-            demands = []
-            j = 0
-            for i in experiment.task_history["outputs"]:
-
-                for (k, v) in i.items():
-                    if "__&@&__Demand__&@&__" in k:
-                        demand_result_dict = {}
-                        demand_result_dict["Simulation"] = j
-                        demand_result_dict["Entity"] = k.split("__&@&__Demand__&@&__")[
-                            0
-                        ]
-                        demand_result_dict["TimeStep"] = k.split(
-                            "__&@&__Demand__&@&__"
-                        )[1]
-                        demand_result_dict["Demand"] = v
-
-                        demands.append(demand_result_dict)
-                j += 1
-            demand_df = pandas.DataFrame(demands)
-            demand_df.to_csv(
-                str(validation_folder) + "/df_all_demands.csv", index=False
-            )
-            df_stock_final.to_csv(str(validation_folder) + "/final_df_comets.csv")
-            df_transport_final.to_csv(str(validation_folder) + "/df_transport.csv")
-            performances.to_csv(str(validation_folder) + "/df_performances.csv")
+        self.experiment.run()
+
+    def reformat_results(self):
+        """Reformat results of the experiment so that they are compatible with the output tables"""
+        self.results = {}
+        # Separating the results data on the different types of outputs (stock, transport, performances, stocksfinal)
+        self.experiment.results["statistics"].reset_index(inplace=True)
+        self.experiment.results["statistics"]["OutputType"] = (
+            self.experiment.results["statistics"]["index"]
+            .str.split(pat="_", expand=False, n=1)
+            .str[0]
+        )
+        self.experiment.results["statistics"]["index"] = (
+            self.experiment.results["statistics"]["index"]
+            .str.split(pat="_", expand=False, n=1)
+            .str[1]
+        )
+        if "Transports" in self.consumers:
+            df_transport_duration = self.experiment.results["statistics"][
+                self.experiment.results["statistics"]["OutputType"] == "1"
+            ]
+            df_transport_duration = df_transport_duration.drop("OutputType", axis=1)
+            df_transport_final = transform_transport_data(df_transport_duration)
+            self.results["Transport"] = df_transport_final
+        if "Stocks" in self.consumers:
+            df_probe_data = self.experiment.results["statistics"][
+                self.experiment.results["statistics"]["OutputType"] == "2"
+            ]
+            df_probe_data = df_probe_data.drop("OutputType", axis=1)
+            df_stock_final = transform_stock_data(df_probe_data)
+            self.results["Stock"] = df_stock_final
+        if "Performances" in self.consumers:
+            performances = self.experiment.results["statistics"][
+                self.experiment.results["statistics"]["OutputType"] == "3"
+            ]
+            performances = performances.drop("OutputType", axis=1)
+            performances = performances.rename(columns={"index": "KPI"})
+            self.results["Performances"] = performances
+        if "StocksFinal" in self.consumers:
+            df_stocksfinalconsumer = self.experiment.results["statistics"][
+                self.experiment.results["statistics"]["OutputType"] == "4"
+            ]
+            df_stocksfinalconsumer = df_stocksfinalconsumer.drop("OutputType", axis=1)
+            df_stocksfinalconsumer = transform_stocksfinal_data(df_stocksfinalconsumer)
+            self.results["StocksFinal"] = df_stocksfinalconsumer
+
+    def write_results_locally(self):
+        """Write the results tables locally to csv files"""
+
+        # Get all demands directly from the experiment, before aggregation of statistics
+        demands = []
+        j = 0
+        for i in self.experiment.task_history["outputs"]:
+
+            for (k, v) in i.items():
+                if "__&@&__Demand__&@&__" in k:
+                    demand_result_dict = {}
+                    demand_result_dict["Simulation"] = j
+                    demand_result_dict["Entity"] = k.split("__&@&__Demand__&@&__")[
+                        0
+                    ].split("_", 1)[1]
+                    demand_result_dict["TimeStep"] = k.split("__&@&__Demand__&@&__")[1]
+                    demand_result_dict["Demand"] = v
+
+                    demands.append(demand_result_dict)
+            j += 1
+        demand_df = pandas.DataFrame(demands)
+        demand_df.to_csv(
+            str(self.validation_folder) + "/df_all_demands.csv", index=False
+        )
+        self.results["Stock"].to_csv(
+            str(self.validation_folder) + "/final_df_comets.csv"
+        )
+        self.results["Transport"].to_csv(
+            str(self.validation_folder) + "/df_transport.csv"
+        )
+        self.results["Performances"].to_csv(
+            str(self.validation_folder) + "/df_performances.csv"
+        )
+
+
+def uncertainty_analysis(
+    simulation_name: str,
+    simulation_path: str = "Simulation",
+    amqp_consumer_adress: Union[str, None] = None,
+    sample_size: int = 1000,
+    batch_size: int = 100,
+    n_jobs: int = -1,
+    adx_writer: Union[ADXAndFileWriter, None] = None,
+    validation_folder: Union[str, None] = None,
+    cold_inputs: dict = {},  # Additional parameters that might be passed to the simulator at each task evaluation
+):
+
+    with Timer("[Run Uncertainty Analysis]") as t:
+
+        ua = UncertaintyAnalyzer(
+            simulation_name=simulation_name,
+            simulation_path=simulation_path,
+            amqp_consumer_adress=amqp_consumer_adress,
+            sample_size=sample_size,
+            batch_size=batch_size,
+            n_jobs=n_jobs,
+            validation_folder=validation_folder,
+            consumers=["Transports", "Stocks", "Performances", "PerformanceAMQP"],
+            cold_inputs=cold_inputs,
+            timer=t,
+        )
+
+        results = ua.execute()
 
         if adx_writer is not None:
+            t.split("Sending stats to ADX")
             adx_writer.write_target_file(
-                df_stock_final.to_dict("records"), "StockUncertaintiesStatistics"
+                results["Stock"].to_dict("records"), "StockUncertaintiesStatistics"
             )
             adx_writer.write_target_file(
-                df_transport_final.to_dict("records"), "TransportUncertaintyStatistics"
+                results["Transport"].to_dict("records"),
+                "TransportUncertaintyStatistics",
             )
+
             t.split("Sent stats to ADX : {time_since_last_split}")
+
         t.display_message("Running simple simulation to fill ADX")
         # Put back log level to Info for final simulation
         # Reduce log level to Error during optimization
         logger = CosmoEngine.LoggerManager.GetInstance().GetLogger()
         logger.SetLogLevel(logger.eInfo)
 
         stop_uncertainty = {"Model::@ActivateUncertainties": "false"}
 
         run_simple_simulation(
             simulation_name=simulation_name,
             simulation_path=simulation_path,
             amqp_consumer_adress=amqp_consumer_adress,
             modifications=stop_uncertainty,
         )
-
-
-# Function to get the list of all the transports in the simulation
-def get_transports(temporary_simulator):
-    transports_list = []
-    transports = temporary_simulator.get_entities_names_by_type(
-        entity_type="TransportOperation"
-    )
-    for keys in transports:
-        transports_list.append(keys)
-    return transports_list
-
-
-# Function to get the list of all the stocks that have uncertain demand
-def get_stocks(temporary_simulator):
-    uncertain_stocks = []
-    for stock in temporary_simulator.get_entities_by_type("Stock"):
-        demands = CosmoEngine.DataTypeMapInterface.Cast(stock.GetAttribute("Demand"))
-        stock_name = stock.GetName()
-        for time_step in demands.GetKeys():
-            demand = demands.GetAt(time_step)
-            if demand.GetAttribute("DemandRelativeUncertainty").Get() > 0:
-                uncertain_stocks.append(stock_name)
-                break
-    return uncertain_stocks
-
-
-def get_distribution_parameter(my_distribution):
-    return co.DistributionRegistry.information[str(my_distribution)]["parameters"]
-
-
-# Function to get the model informations for each transports, such as the distribution used and
-# its parameters, and for each stock, such as which stocks have uncertain demand
-def model_info(my_simulator, simulation_path, transports_names):
-    actual_duration_schedule = {}
-    list_of_transports = transports_names.copy()
-    uncertainty_param_1 = {}
-    uncertainty_param_2 = {}
-    uncertainty_param_3 = {}
-    uncertainty_param_4 = {}
-    demands = {}
-
-    time_step_per_cycle = my_simulator.get_outputs(["Model::@TimeStepPerCycle"])[
-        "Model::@TimeStepPerCycle"
-    ]
-
-    number_of_cycle = my_simulator.get_outputs(["Model::@NumberOfCycle"])[
-        "Model::@NumberOfCycle"
-    ]
-
-    max_time_step = time_step_per_cycle * number_of_cycle
-
-    distribution = my_simulator.get_outputs(
-        ["Model::@TransportUncertaintiesProbabilityDistribution"]
-    )["Model::@TransportUncertaintiesProbabilityDistribution"]
-
-    ActivateCorrelatedDemandUncertainties = my_simulator.get_outputs(
-        ["Model::@ActivateCorrelatedDemandUncertainties"]
-    )["Model::@ActivateCorrelatedDemandUncertainties"]
-
-    if ActivateCorrelatedDemandUncertainties:
-        uncertain_stocks = get_stocks(my_simulator.sim)
-    else:
-        uncertain_stocks = []
-
-    DemandCorrelations = my_simulator.get_outputs(["Model::@DemandCorrelations"])[
-        "Model::@DemandCorrelations"
-    ]
-
-    for transport in transports_names:
-
-        # If their is no ActualDuration in the TransportSchedules column of the dataset,
-        # we use by default the attribute duration, in the Transport column of the dataset.
-        if (
-            my_simulator.get_outputs(
-                [
-                    f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-                ]
-            )[
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-            ]
-            == {}
-        ):
-            duration = my_simulator.get_outputs(
-                [
-                    f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@Duration"
-                ]
-            )[f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@Duration"]
-
-            # Use a dict format so that the function "extended_dict" defined below can be applied
-            actual_duration_schedule[transport] = {0: duration}
-        else:
-            actual_duration_schedule[transport] = my_simulator.get_outputs(
-                [
-                    f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-                ]
-            )[
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-            ]
-
-        uncertainty_param_1[transport] = my_simulator.get_outputs(
-            [
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter1"
-            ]
-        )[
-            f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter1"
-        ]
-        uncertainty_param_2[transport] = my_simulator.get_outputs(
-            [
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter2"
-            ]
-        )[
-            f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter2"
-        ]
-        uncertainty_param_3[transport] = my_simulator.get_outputs(
-            [
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter3"
-            ]
-        )[
-            f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter3"
-        ]
-        uncertainty_param_4[transport] = my_simulator.get_outputs(
-            [
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter4"
-            ]
-        )[
-            f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@TransportUncertaintiesParameter4"
-        ]
-        # If the transport has no parameters, its transport duration will not be part of the uncertainty analysis
-        if (
-            uncertainty_param_1[transport] == uncertainty_param_2[transport]
-            and uncertainty_param_1[transport] == {}
-        ):
-            list_of_transports.remove(transport)
-
-    for stock in uncertain_stocks:
-        demands[stock] = my_simulator.get_outputs(
-            [f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{stock}::@Demand"]
-        )[f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{stock}::@Demand"]
-
-    return (
-        max_time_step,
-        distribution,
-        actual_duration_schedule,
-        list_of_transports,
-        uncertainty_param_1,
-        uncertainty_param_2,
-        uncertainty_param_3,
-        uncertainty_param_4,
-        demands,
-        ActivateCorrelatedDemandUncertainties,
-        DemandCorrelations,
-        uncertain_stocks,
-    )
-
-
-# Function to extend dictionaries using transport schedules.
-# the following dic: {0: 3, 6: 4, 7: 3, 8: 2, 9: 8, 10: 40}
-# Becomes: {0: 3, 1: 3, 2: 3, 3: 3, 4: 3, 5: 3, 6: 4, 7: 3, 8: 2, 9: 8, 10: 40}
-def extend_simple_dic(my_dic, number_of_iterations):
-    if my_dic != {}:  # checking that the dic isn't empty
-        extended_dic = {
-            0: my_dic[0]
-        }  # We assume that the uncertainty starts at the first time step
-        for i in range(1, number_of_iterations):
-            if i in my_dic:
-                extended_dic[i] = deepcopy(my_dic[i])
-            else:
-                extended_dic[i] = deepcopy(extended_dic[i - 1])
-    else:
-        extended_dic = {}
-    return extended_dic
-
-
-# Function to extend dictionaries using schedules.
-# For each transports, the following dic: {"transport name" : {0: 3, 6: 4, 7: 3, 8: 2, 9: 8, 10: 40}}
-# Becomes: {"transport name" : {0: 3, 1: 3, 2: 3, 3: 3, 4: 3, 5: 3, 6: 4, 7: 3, 8: 2, 9: 8, 10: 40}}
-def extend_dic(my_dic, number_of_iterations):
-    extended_dic = {}
-    for entity in my_dic.keys():
-        extended_dic[entity] = extend_simple_dic(my_dic[entity], number_of_iterations)
-    return extended_dic
-
-
-# this function transforms supply chain's distribution parameters
-# that don't match CoMETS format
-def check_distrib_parameters(
-    my_distribution, param1, param2, param3, param4, transports_names
-):
-    # In CoMETS the upper bound of the discreteuniform distribution is excluded.
-    # However, in supply chain it is included. Therefore, we need to add 1 to the upper bound
-    # so it matches CoMETS
-    if my_distribution == "discreteuniform":
-        for transport in transports_names:
-            for keys in param2[transport].keys():
-                param2[transport][keys] += 1
-
-    # In CoMETS the two arguments of the uniform distribution are loc and scale
-    # and the interval of the distribution is the following:  [loc, loc+scale]
-    # However, in supply chain the two parameters of the uniform distribution are
-    # [lower, upper]. Therefor, upper needs to be mapped to scale
-    if my_distribution == "uniform":
-        for transport in transports_names:
-            for keys in param2[transport].keys():
-                param2[transport][keys] = (
-                    param2[transport][keys] - param1[transport][keys]
-                )
-
-    if my_distribution == "betabinom":
-        for transport in transports_names:
-            for keys in param1[transport].keys():
-                param1[transport][keys] = round(param1[transport][keys])
-
-    if my_distribution == "binomial":
-        for transport in transports_names:
-            for keys in param1[transport].keys():
-                param1[transport][keys] = round(param1[transport][keys])
-
-    if my_distribution == "hypergeom":
-        for transport in transports_names:
-            for keys in param1[transport].keys():
-                param1[transport][keys] = round(param1[transport][keys])
-                param2[transport][keys] = round(param2[transport][keys])
-                param3[transport][keys] = round(param3[transport][keys])
-
-    return [param1, param2, param3, param4]
-
-
-# Function to create the uncertainty analysis space according to CoMETS format
-# This function will create one variable for each time step of each transports
-# distribution: name of the distribution used for the ua
-# param1: values by transport by time step for the first parameter of the distribution
-# param2: values by transport by time step for the second parameter of the distribution
-# param3: values by transport by time step for the third parameter of the distribution
-# param4: values by transport by time step for the fourth parameter of the distribution
-# transports: list of all the uncertain transports names
-# distribution_parameters: list of the parameters names required by CoMETS sampler for the given distribution
-# number_of_time_steps: number of time step simulated
-def creating_transport_distribution_space(
-    distribution,
-    param1,
-    param2,
-    param3,
-    param4,
-    transports,
-    distribution_parameters,
-    number_of_time_steps,
-):
-    sampling = []
-    all_parameters = check_distrib_parameters(
-        distribution, param1, param2, param3, param4, transports
-    )
-    for transport in transports:
-        considered_parameters = [
-            (position, parameter)
-            for position, parameter in enumerate(distribution_parameters)
-            if all_parameters[position][transport]
-        ]
-        for t in range(number_of_time_steps):
-            parameters = {
-                parameter: all_parameters[position][transport][t]
-                for position, parameter in considered_parameters
-            }
-            sampling.append(
-                {
-                    "name": f"{transport}_@_{t}",
-                    "sampling": distribution,
-                    "parameters": parameters,
-                }
-            )
-    return sampling
-
-
-def creating_demand_generator(
-    extended_demands, number_of_time_steps, DemandCorrelations
-):
-    sampling = []
-    for stock, demand_attribute in extended_demands.items():
-        mean_demand = []
-        uncertainties = []
-        for t in range(number_of_time_steps):
-
-            demand = demand_attribute[t]["ExternalDemand"]
-            mean_demand.append(demand)
-            uncertainties.append(
-                demand * demand_attribute[t]["DemandRelativeUncertainty"]
-            )  # Uncertainty proportional to demand, DemandRelativeUncertainty*Demand is the standard deviation
-        sampling.append(
-            {
-                "name": f"{stock}",
-                "sampling": co.TimeSeriesSampler(
-                    correlation=DemandCorrelations,
-                    dimension=number_of_time_steps,
-                    forecast=mean_demand,
-                    uncertainties=uncertainties,
-                    minimum=0,
-                ),
-            }
-        )
-    return sampling
-
-
-# Function that returns a parameterset with the transport duration for each transport at the end of the simulation
-# The transport duration is separated for each time step. The output parameterset (for a simulation
-# with 1 TransportOperation: U) will have the following format:
-#    {Model[...]U::@ActualDurationSchedule__&@&__0': 10,
-#          [...],
-#     Model[...]U::@ActualDurationSchedule__&@&__10': 7}
-def get_transport_duration(transports_names, modelinterface, max_time_step):
-    transport_duration = {}
-    transport_duration_transformed = {}
-    for transport in transports_names:
-        if (
-            modelinterface.get_outputs(
-                [
-                    f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-                ]
-            )[
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-            ]
-            == {}
-        ):
-            duration = modelinterface.get_outputs(
-                [
-                    f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@Duration"
-                ]
-            )[f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@Duration"]
-            # Use a dict format so that the function "extended_dict" defined below can be applied
-            actual_duration_schedule = {0: duration}
-        else:
-            actual_duration_schedule = modelinterface.get_outputs(
-                [
-                    f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-                ]
-            )[
-                f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-            ]
-        transport_duration[
-            f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-        ] = extend_simple_dic(
-            actual_duration_schedule,
-            max_time_step,
-        )
-        time_step = 0
-        for value in transport_duration[
-            f"Model::{{Entity}}IndustrialNetwork::{{Entity}}{transport}::@ActualDurationSchedule"
-        ].values():
-            transport_duration_transformed[f"{transport}__&@&__{time_step}"] = value
-            time_step += 1
-    return transport_duration_transformed
-
-
-# This function transform the consumer memory from a list of list to a list of
-# ParameterSet. Note that each sublist in the initial format is transformed into
-# a parameterset of 4 parameters : Demand, RemainingQuantity, ServedQuantity,UnservedQuantity
-def transform_consumer_memory(transform_consumer_memory):
-    dic_of_parameterset = {}
-    for elements in transform_consumer_memory:
-        dic_of_parameterset[
-            str(elements[0] + "__&@&__" + "Demand" + "__&@&__" + str(elements[1]))
-        ] = elements[2]
-        dic_of_parameterset[
-            str(
-                elements[0]
-                + "__&@&__"
-                + "RemainingQuantity"
-                + "__&@&__"
-                + str(elements[1])
-            )
-        ] = elements[3]
-        dic_of_parameterset[
-            str(
-                elements[0]
-                + "__&@&__"
-                + "ServedQuantity"
-                + "__&@&__"
-                + str(elements[1])
-            )
-        ] = elements[4]
-        dic_of_parameterset[
-            str(
-                elements[0]
-                + "__&@&__"
-                + "UnservedQuantity"
-                + "__&@&__"
-                + str(elements[1])
-            )
-        ] = elements[5]
-    return dic_of_parameterset
-
-
-def transform_stock_data(data):
-    # Splitting the first columns into 3 columns: TimeStep, StockId, Category
-    # And adding the simulationRun
-    temporary_df = data.copy()
-    temporary_df.loc[:, "SimulationRun"] = EnvironmentVariables.simulation_id
-    temporary_df[["StockId", "Category", "TimeStep"]] = temporary_df["index"].str.split(
-        pat="__&@&__", expand=True
-    )
-
-    # Removing unused columns such as index, quantile 10 ...
-    temporary_df = temporary_df.iloc[:, [1, 3, 5, 9, 14, 19, 23, 24, 25, 26, 27]]
-
-    # Changing the columns' order and renaming them to match the adx table
-    df_final = temporary_df[
-        [
-            "TimeStep",
-            "SimulationRun",
-            "StockId",
-            "quantile 5%",
-            "quantile 25%",
-            "quantile 50%",
-            "quantile 75%",
-            "quantile 95%",
-            "mean",
-            "sem",
-            "Category",
-        ]
-    ]
-
-    df_final.rename(
-        columns={
-            "quantile 5%": "Percentile5",
-            "quantile 25%": "Percentile25",
-            "quantile 50%": "Percentile50",
-            "quantile 75%": "Percentile75",
-            "quantile 95%": "Percentile95",
-            "mean": "Mean",
-            "sem": "SE",
-        },
-        inplace=True,
-    )
-    return df_final
-
-
-def transform_transport_data(data):
-
-    # Adding the simulation run to the df
-    temporary_df = data.copy()
-    if not temporary_df.empty:
-        temporary_df.loc[:, "SimulationRun"] = EnvironmentVariables.simulation_id
-        # Splitting the first column into 2 columns: TransportOperation, TimeStep
-        temporary_df[["TransportOperation", "TimeStep"]] = temporary_df[
-            "index"
-        ].str.split(pat="__&@&__", expand=True)
-    else:
-        temporary_df[["TransportOperation", "TimeStep"]] = None
-    df_final = temporary_df.iloc[:, 1:]
-
-    df_final.rename(
-        columns={
-            "confidence interval of the mean at 95%": "ConfidenceIntervalOfTheMeanAt95",
-            "quantile 5%": "Percentile5",
-            "quantile 10%": "Percentile10",
-            "quantile 15%": "Percentile15",
-            "quantile 20%": "Percentile20",
-            "quantile 25%": "Percentile25",
-            "quantile 30%": "Percentile30",
-            "quantile 35%": "Percentile35",
-            "quantile 40%": "Percentile40",
-            "quantile 45%": "Percentile45",
-            "quantile 50%": "Percentile50",
-            "quantile 55%": "Percentile55",
-            "quantile 60%": "Percentile60",
-            "quantile 65%": "Percentile65",
-            "quantile 70%": "Percentile70",
-            "quantile 75%": "Percentile75",
-            "quantile 80%": "Percentile80",
-            "quantile 85%": "Percentile85",
-            "quantile 90%": "Percentile90",
-            "quantile 95%": "Percentile95",
-        },
-        inplace=True,
-    )
-
-    return df_final
+        t.split("Final simulation succeeded : {time_since_last_split}")
```

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/adt_column_description.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/adt_column_description.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,29 @@
                 "UncertaintiesProbabilityDistribution",
                 "IntermediaryStockDispatchPolicy",
                 "TransportUncertaintiesProbabilityDistribution",
                 "ActualizeShipments",
                 "ActivateCorrelatedDemandUncertainties",
                 "DemandCorrelations",
                 "CarbonTax",
+                "Kpi",
+                "OptimizationMode",
+                "Statistic",
+                "TargetedValue",
+                "DecisionVariable",
+                "DecisionVariableMin",
+                "DecisionVariableMax",
+                "OptimizationMaximalDuration",
+                "OptimizationAlgorithm",
+                "OptimizationBatchSize",
+                "SampleSizeUncertaintyAnalysis",
+                "FinalSampleSizeUncertaintyAnalysis",
+                "MaxIterationsForOptim",
+                "AutomaticParallelizationConfig",
+                "MaxNumberOfSimInParallel",
             ],
             "change": [],
             "event": {},
         },
         "contains": {
             "fixed": [
                 "source",
```

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/default_values.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/default_values.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,14 +70,29 @@
         "UncertaintiesProbabilityDistribution": "Uniform",
         "IntermediaryStockDispatchPolicy": "DispatchAll",
         "TransportUncertaintiesProbabilityDistribution": "discreteuniform",
         "ActualizeShipments": False,
         "ActivateCorrelatedDemandUncertainties": False,
         "DemandCorrelations": 0,
         "CarbonTax": 0,
+        "Kpi": "Profit",
+        "OptimizationMode": "maximize",
+        "Statistic": "mean",
+        "TargetedValue": 80,
+        "DecisionVariable": "Order quantity",
+        "DecisionVariableMin": 0,
+        "DecisionVariableMax": 2000,
+        "OptimizationMaximalDuration": 3600,
+        "OptimizationAlgorithm": "NGOpt",
+        "OptimizationBatchSize": 1,
+        "SampleSizeUncertaintyAnalysis": 25,
+        "FinalSampleSizeUncertaintyAnalysis": 1000,
+        "MaxIterationsForOptim": 250,
+        "AutomaticParallelizationConfig": True,
+        "MaxNumberOfSimInParallel": 1,
     },
     "contains": {
         #'source',
         #'target',
     },
     "output": {
         #'source',
```

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/simulator_files_description.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/simulator_files_description.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Schema/validation_schemas.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Schema/validation_schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -91,14 +91,74 @@
                 "IntermediaryStockDispatchPolicy": {
                     "type": "string",
                     "enum": ["DispatchAll", "AllowRetention"],
                 },
                 "ActualizeShipments": {"type": "boolean"},
                 "ActivateCorrelatedDemandUncertainties": {"type": "boolean"},
                 "DemandCorrelations": {"type": "number", "minimum": 0, "maximum": 1},
+                "Kpi": {
+                    "type": "string",
+                    "enum": [
+                        "Profit",
+                        "OPEX",
+                        "AverageStockValue",
+                        "ServiceLevelIndicator",
+                        "ServiceLevelSatisfaction",
+                        "CO2Emissions",
+                        "TotalServedQuantity",
+                        "IndividualServiceLevelSatisfaction",
+                    ],
+                },
+                "OptimizationMode": {
+                    "type": "string",
+                    "enum": [
+                        "maximize",
+                        "minimize",
+                        "target",
+                    ],
+                },
+                "Statistic": {
+                    "type": "string",
+                    "enum": [
+                        "mean",
+                        "std",
+                        "sem",
+                        "quantile 5%",
+                        "quantile 10%",
+                        "quantile 15%",
+                        "quantile 20%",
+                        "quantile 25%",
+                        "quantile 30%",
+                        "quantile 35%",
+                        "quantile 40%",
+                        "quantile 45%",
+                        "quantile 50%",
+                        "quantile 55%",
+                        "quantile 60%",
+                        "quantile 65%",
+                        "quantile 70%",
+                        "quantile 75%",
+                        "quantile 80%",
+                        "quantile 85%",
+                        "quantile 90%",
+                        "quantile 95%",
+                    ],
+                },
+                "TargetedValue": {"type": "number"},
+                "DecisionVariable": {"type": "string"},
+                "DecisionVariableMin": {"type": "number"},
+                "DecisionVariableMax": {"type": "number"},
+                "OptimizationMaximalDuration": {"type": "number"},
+                "OptimizationAlgorithm": {"type": "string"},
+                "OptimizationBatchSize": {"type": "integer", "minimum": 1},
+                "SampleSizeUncertaintyAnalysis": {"type": "integer"},
+                "FinalSampleSizeUncertaintyAnalysis": {"type": "integer"},
+                "MaxIterationsForOptim": {"type": "integer"},
+                "AutomaticParallelizationConfig": {"type": "boolean"},
+                "MaxNumberOfSimInParallel": {"type": "integer", "minimum": 1},
             },
         },
         "input": {
             "$schema": "http://json-schema.org/draft-07/schema#",
             "type": "object",
             "properties": {"InputQuantity": {"type": "number", "exclusiveMinimum": 0}},
         },
@@ -118,15 +178,17 @@
                         "^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}
                     },
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "CycleTimes": {
                     "type": "object",
-                    "patternProperties": {"^[0-9]+$": {"type": "number", "exclusiveMinimum": 0}},
+                    "patternProperties": {
+                        "^[0-9]+$": {"type": "number", "exclusiveMinimum": 0}
+                    },
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "RejectRates": {
                     "type": "object",
                     "patternProperties": {
                         "^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}
@@ -164,15 +226,17 @@
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "SourcingProportions": {
                     "type": "object",
-                    "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}},
+                    "patternProperties": {
+                        "^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}
+                    },
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "IsContractor": {"type": "boolean"},
                 "InvestmentCost": {
                     "type": "number",
                     "minimum": 0,
@@ -391,15 +455,17 @@
                     "type": "object",
                     "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0}},
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "SourcingProportions": {
                     "type": "object",
-                    "patternProperties": {"^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}},
+                    "patternProperties": {
+                        "^[0-9]+$": {"type": "number", "minimum": 0, "maximum": 1}
+                    },
                     "if": {"minProperties": 1},
                     "then": {"required": ["0"]},
                 },
                 "TransportUncertaintiesParameter1": {
                     "type": "object",
                     "patternProperties": {
                         "^[0-9]+$": {
```

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/complete_dict.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/complete_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_simulator.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_dict_to_table.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_dict_to_table.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/from_table_to_dict_old.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/from_table_to_dict_old.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Transform/production_route.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Transform/production_route.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Validate/validate_dict.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Validate/validate_dict.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/environment_variables.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/environment_variables.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/Supplychain/Wrappers/simulator.py` & `CosmoTech-SupplyChain-5.0.0/Supplychain/Wrappers/simulator.py`

 * *Files identical despite different names*

### Comparing `CosmoTech-SupplyChain-4.1.2/setup.py` & `CosmoTech-SupplyChain-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-VERSION = "v4.1.2"
+VERSION = "5.0.0"
 
 setuptools.setup(
     name='CosmoTech-SupplyChain',
     version=VERSION,
     author='Alexis Fossart',
     author_email='alexis.fossart@cosmotech.com',
     url='https://github.com/Cosmo-Tech/supplychain-python-library<',
```

