# Comparing `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a3.tar.gz` & `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a3.tar", last modified: Wed Jun 21 15:46:07 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a4.tar", last modified: Wed Jun 21 23:28:22 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a3.tar` & `ovos-PHAL-plugin-wifi-setup-1.1.1a4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/
--rw-r--r--   0 runner    (1001) docker     (123)    23664 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 15:46:00.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)    23664 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 23:28:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 23:28:22.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 23:28:22.419860 ovos-PHAL-plugin-wifi-setup-1.1.1a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-21 23:28:11.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a4/setup.py
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a3/LICENSE` & `ovos-PHAL-plugin-wifi-setup-1.1.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a3/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.1a3
+Version: 1.1.1a4
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a3/README.md` & `ovos-PHAL-plugin-wifi-setup-1.1.1a4/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/__init__.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a4/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.1a3
+Version: 1.1.1a4
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a3/setup.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a4/setup.py`

 * *Files identical despite different names*

