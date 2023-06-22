# Comparing `tmp/zigpy-0.56.0.tar.gz` & `tmp/zigpy-0.56.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zigpy-0.56.0.tar", last modified: Mon Jun  5 20:35:02 2023, max compression
+gzip compressed data, was "zigpy-0.56.1.tar", last modified: Thu Jun 22 21:09:27 2023, max compression
```

## Comparing `zigpy-0.56.0.tar` & `zigpy-0.56.1.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-05 20:34:59.000000 zigpy-0.56.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-05 20:34:59.000000 zigpy-0.56.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-05 20:35:02.334019 zigpy-0.56.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-05 20:34:59.000000 zigpy-0.56.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-05 20:35:02.338019 zigpy-0.56.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-05 20:34:59.000000 zigpy-0.56.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.326019 zigpy-0.56.0/zigpy/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/appdb_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v0.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v1.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v11.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v12.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v2.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v3.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v4.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v5.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v6.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v8.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/appdb_schemas/schema_v9.sql
--rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/application.py
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/backups.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/config/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/listeners.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/ota/
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/ota/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/zgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/zha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/profiles/zll.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.330019 zigpy-0.56.0/zigpy/quirks/
--rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/quirks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/quirks/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/types/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/named.py
--rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/types/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/zcl/
--rw-r--r--   0 runner    (1001) docker     (123)    35495 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/zcl/clusters/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/closures.py
--rw-r--r--   0 runner    (1001) docker     (123)    90858 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/homeautomation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/hvac.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/lighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/lightlink.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/manufacturer_specific.py
--rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16606 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/clusters/smartenergy.py
--rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zcl/foundation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.334019 zigpy-0.56.0/zigpy/zdo/
--rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zdo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-06-05 20:34:59.000000 zigpy-0.56.0/zigpy/zdo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 20:35:02.326019 zigpy-0.56.0/zigpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 20:35:02.000000 zigpy-0.56.0/zigpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 21:09:23.000000 zigpy-0.56.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-22 21:09:23.000000 zigpy-0.56.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-22 21:09:27.416668 zigpy-0.56.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7600 2023-06-22 21:09:23.000000 zigpy-0.56.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-22 21:09:27.420668 zigpy-0.56.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-22 21:09:23.000000 zigpy-0.56.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.408668 zigpy-0.56.1/zigpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/appdb_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v0.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v1.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v12.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v2.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v3.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v4.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v5.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v6.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v8.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4961 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/appdb_schemas/schema_v9.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    43976 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/backups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/config/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/config/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16826 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/listeners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/ota/
+-rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/ota/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.412668 zigpy-0.56.1/zigpy/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/zgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/zha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/profiles/zll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/quirks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11954 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/quirks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5946 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/quirks/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11443 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8527 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/topology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18607 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/named.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12200 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/types/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/zcl/
+-rw-r--r--   0 runner    (1001) docker     (123)    35495 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/zcl/clusters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28452 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/closures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90858 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26113 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/homeautomation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/hvac.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/lighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/lightlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/manufacturer_specific.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20097 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16606 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15042 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18998 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/clusters/smartenergy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zcl/foundation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.416668 zigpy-0.56.1/zigpy/zdo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7628 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zdo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24087 2023-06-22 21:09:23.000000 zigpy-0.56.1/zigpy/zdo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:09:27.408668 zigpy-0.56.1/zigpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 21:09:27.000000 zigpy-0.56.1/zigpy.egg-info/top_level.txt
```

### Comparing `zigpy-0.56.0/COPYING` & `zigpy-0.56.1/COPYING`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/LICENSE` & `zigpy-0.56.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/PKG-INFO` & `zigpy-0.56.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.56.0
+Version: 0.56.1
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.56.0/README.md` & `zigpy-0.56.1/README.md`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/setup.cfg` & `zigpy-0.56.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/setup.py` & `zigpy-0.56.1/setup.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb.py` & `zigpy-0.56.1/zigpy/appdb.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v0.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v0.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v1.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v1.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v10.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v10.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v11.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v11.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v12.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v12.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v2.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v2.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v3.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v3.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v4.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v4.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v5.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v5.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v6.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v6.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v7.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v7.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v8.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v8.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/appdb_schemas/schema_v9.sql` & `zigpy-0.56.1/zigpy/appdb_schemas/schema_v9.sql`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/application.py` & `zigpy-0.56.1/zigpy/application.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/backups.py` & `zigpy-0.56.1/zigpy/backups.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/config/__init__.py` & `zigpy-0.56.1/zigpy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/config/defaults.py` & `zigpy-0.56.1/zigpy/config/defaults.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/config/validators.py` & `zigpy-0.56.1/zigpy/config/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/const.py` & `zigpy-0.56.1/zigpy/const.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/device.py` & `zigpy-0.56.1/zigpy/device.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/endpoint.py` & `zigpy-0.56.1/zigpy/endpoint.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/exceptions.py` & `zigpy-0.56.1/zigpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/group.py` & `zigpy-0.56.1/zigpy/group.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/listeners.py` & `zigpy-0.56.1/zigpy/listeners.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/ota/__init__.py` & `zigpy-0.56.1/zigpy/ota/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/ota/image.py` & `zigpy-0.56.1/zigpy/ota/image.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/ota/provider.py` & `zigpy-0.56.1/zigpy/ota/provider.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/ota/validators.py` & `zigpy-0.56.1/zigpy/ota/validators.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/profiles/zgp.py` & `zigpy-0.56.1/zigpy/profiles/zgp.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/profiles/zha.py` & `zigpy-0.56.1/zigpy/profiles/zha.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/profiles/zll.py` & `zigpy-0.56.1/zigpy/profiles/zll.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/quirks/__init__.py` & `zigpy-0.56.1/zigpy/quirks/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/quirks/registry.py` & `zigpy-0.56.1/zigpy/quirks/registry.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/serial.py` & `zigpy-0.56.1/zigpy/serial.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/state.py` & `zigpy-0.56.1/zigpy/state.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/topology.py` & `zigpy-0.56.1/zigpy/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 LOGGER = logging.getLogger(__name__)
 REQUEST_DELAY = (1.0, 1.5)
 
 if typing.TYPE_CHECKING:
     import zigpy.application
 
 
+RETRY_SLOW = zigpy.util.retryable_request(tries=3, delay=1)
+
+
 class ScanNotSupported(Exception):
     pass
 
 
 INVALID_NEIGHBOR_IEEES = {
     t.EUI64.convert("00:00:00:00:00:00:00:00"),
     t.EUI64.convert("ff:ff:ff:ff:ff:ff:ff:ff"),
@@ -97,15 +100,15 @@
     ) -> list[typing.Any]:
         """Scan a device table by sending ZDO requests."""
 
         index = 0
         table = []
 
         while True:
-            status, rsp = await scan_request(index, tries=3, delay=1)
+            status, rsp = await RETRY_SLOW(scan_request)(index)
 
             if status != zdo_t.Status.SUCCESS:
                 raise ScanNotSupported()
 
             entries = getattr(rsp, entries_attr)
 
             table.extend(entries)
```

### Comparing `zigpy-0.56.0/zigpy/types/basic.py` & `zigpy-0.56.1/zigpy/types/basic.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/types/named.py` & `zigpy-0.56.1/zigpy/types/named.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/types/struct.py` & `zigpy-0.56.1/zigpy/types/struct.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/typing.py` & `zigpy-0.56.1/zigpy/typing.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/util.py` & `zigpy-0.56.1/zigpy/util.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/__init__.py` & `zigpy-0.56.1/zigpy/zcl/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/__init__.py` & `zigpy-0.56.1/zigpy/zcl/clusters/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/closures.py` & `zigpy-0.56.1/zigpy/zcl/clusters/closures.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/general.py` & `zigpy-0.56.1/zigpy/zcl/clusters/general.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/homeautomation.py` & `zigpy-0.56.1/zigpy/zcl/clusters/homeautomation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/hvac.py` & `zigpy-0.56.1/zigpy/zcl/clusters/hvac.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/lighting.py` & `zigpy-0.56.1/zigpy/zcl/clusters/lighting.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/lightlink.py` & `zigpy-0.56.1/zigpy/zcl/clusters/lightlink.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/measurement.py` & `zigpy-0.56.1/zigpy/zcl/clusters/measurement.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/protocol.py` & `zigpy-0.56.1/zigpy/zcl/clusters/protocol.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/security.py` & `zigpy-0.56.1/zigpy/zcl/clusters/security.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/clusters/smartenergy.py` & `zigpy-0.56.1/zigpy/zcl/clusters/smartenergy.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zcl/foundation.py` & `zigpy-0.56.1/zigpy/zcl/foundation.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zdo/__init__.py` & `zigpy-0.56.1/zigpy/zdo/__init__.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy/zdo/types.py` & `zigpy-0.56.1/zigpy/zdo/types.py`

 * *Files identical despite different names*

### Comparing `zigpy-0.56.0/zigpy.egg-info/PKG-INFO` & `zigpy-0.56.1/zigpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zigpy
-Version: 0.56.0
+Version: 0.56.1
 Summary: Library implementing a ZigBee stack
 Home-page: https://github.com/zigpy/zigpy
 Author: Russell Cloran
 Author-email: rcloran@gmail.com
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `zigpy-0.56.0/zigpy.egg-info/SOURCES.txt` & `zigpy-0.56.1/zigpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

