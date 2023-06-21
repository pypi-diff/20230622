# Comparing `tmp/ovos-phal-plugin-connectivity-events-0.0.3a3.tar.gz` & `tmp/ovos-phal-plugin-connectivity-events-0.0.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.3a3.tar", last modified: Wed Jun 21 15:46:16 2023, max compression
+gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.3a4.tar", last modified: Wed Jun 21 18:40:55 2023, max compression
```

## Comparing `ovos-phal-plugin-connectivity-events-0.0.3a3.tar` & `ovos-phal-plugin-connectivity-events-0.0.3a4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-21 15:46:07.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 15:46:10.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 15:46:16.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:15.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-21 15:46:07.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:16.152659 ovos-phal-plugin-connectivity-events-0.0.3a3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-21 15:46:07.000000 ovos-phal-plugin-connectivity-events-0.0.3a3/test/test_connectivity_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:40:55.540333 ovos-phal-plugin-connectivity-events-0.0.3a4/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 18:40:55.540333 ovos-phal-plugin-connectivity-events-0.0.3a4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:40:55.540333 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-06-21 18:40:51.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 18:40:51.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:40:55.540333 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-21 18:40:55.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-21 18:40:55.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:40:55.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-21 18:40:55.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-21 18:40:55.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 18:40:55.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:40:55.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:40:55.540333 ovos-phal-plugin-connectivity-events-0.0.3a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-21 18:40:51.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:40:55.540333 ovos-phal-plugin-connectivity-events-0.0.3a4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-21 18:40:51.000000 ovos-phal-plugin-connectivity-events-0.0.3a4/test/test_connectivity_events.py
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a3/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.3a3
+Version: 0.0.3a4
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
-Description: # ovos-PHAL-plugin - Connectivity Events
-        
-        Monitors network state and exposes it via messagebus.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+
+# ovos-PHAL-plugin - Connectivity Events
+
+Monitors network state and exposes it via messagebus.
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events/__init__.py` & `ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.3a3
+Version: 0.0.3a4
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
-Description: # ovos-PHAL-plugin - Connectivity Events
-        
-        Monitors network state and exposes it via messagebus.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+
+# ovos-PHAL-plugin - Connectivity Events
+
+Monitors network state and exposes it via messagebus.
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a3/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt` & `ovos-phal-plugin-connectivity-events-0.0.3a4/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a3/setup.py` & `ovos-phal-plugin-connectivity-events-0.0.3a4/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a3/test/test_connectivity_events.py` & `ovos-phal-plugin-connectivity-events-0.0.3a4/test/test_connectivity_events.py`

 * *Files identical despite different names*

