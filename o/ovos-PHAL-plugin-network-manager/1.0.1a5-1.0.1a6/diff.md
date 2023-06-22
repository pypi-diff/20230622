# Comparing `tmp/ovos-PHAL-plugin-network-manager-1.0.1a5.tar.gz` & `tmp/ovos-PHAL-plugin-network-manager-1.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-network-manager-1.0.1a5.tar", last modified: Wed Jun 21 19:37:14 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-network-manager-1.0.1a6.tar", last modified: Wed Jun 21 23:36:14 2023, max compression
```

## Comparing `ovos-PHAL-plugin-network-manager-1.0.1a5.tar` & `ovos-PHAL-plugin-network-manager-1.0.1a6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:14.555043 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:37:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:37:14.559043 ovos-PHAL-plugin-network-manager-1.0.1a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3241 2023-06-21 19:37:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:36:14.653446 ovos-PHAL-plugin-network-manager-1.0.1a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 23:36:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 23:36:14.653446 ovos-PHAL-plugin-network-manager-1.0.1a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-21 23:36:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:36:14.653446 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    17870 2023-06-21 23:36:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 23:36:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:36:14.653446 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 23:36:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-21 23:36:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:36:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-21 23:36:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 23:36:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 23:36:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:36:14.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:36:14.653446 ovos-PHAL-plugin-network-manager-1.0.1a6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3241 2023-06-21 23:36:10.000000 ovos-PHAL-plugin-network-manager-1.0.1a6/setup.py
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a5/LICENSE` & `ovos-PHAL-plugin-network-manager-1.0.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a5/PKG-INFO` & `ovos-PHAL-plugin-network-manager-1.0.1a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-network-manager
-Version: 1.0.1a5
+Version: 1.0.1a6
 Summary: Network Manager plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-network-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a5/README.md` & `ovos-PHAL-plugin-network-manager-1.0.1a6/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager/__init__.py` & `ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a5/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO` & `ovos-PHAL-plugin-network-manager-1.0.1a6/ovos_PHAL_plugin_network_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-network-manager
-Version: 1.0.1a5
+Version: 1.0.1a6
 Summary: Network Manager plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-network-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-network-manager-1.0.1a5/setup.py` & `ovos-PHAL-plugin-network-manager-1.0.1a6/setup.py`

 * *Files identical despite different names*

