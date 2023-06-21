# Comparing `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a2.tar.gz` & `tmp/ovos-PHAL-plugin-wifi-setup-1.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a2.tar", last modified: Wed Jun 14 01:43:14 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wifi-setup-1.1.1a3.tar", last modified: Wed Jun 21 15:46:07 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a2.tar` & `ovos-PHAL-plugin-wifi-setup-1.1.1a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:43:14.804878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/
--rw-r--r--   0 runner    (1001) docker     (123)    23088 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-14 01:43:08.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 01:43:14.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 01:43:14.808878 ovos-PHAL-plugin-wifi-setup-1.1.1a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-14 01:43:05.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9015 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/
+-rw-r--r--   0 runner    (1001) docker     (123)    23664 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 15:46:00.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:46:07.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:46:07.452948 ovos-PHAL-plugin-wifi-setup-1.1.1a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-21 15:45:57.000000 ovos-PHAL-plugin-wifi-setup-1.1.1a3/setup.py
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a2/LICENSE` & `ovos-PHAL-plugin-wifi-setup-1.1.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a2/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.1a2
+Version: 1.1.1a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a2/README.md` & `ovos-PHAL-plugin-wifi-setup-1.1.1a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup/__init__.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 import random
 import uuid
 from os.path import dirname, join
 from time import sleep
 
 from ovos_bus_client.message import Message
 from ovos_plugin_manager.phal import PHALPlugin
+from ovos_utils import classproperty
 from ovos_utils import create_daemon
 from ovos_utils.device_input import can_use_touch_mouse
 from ovos_utils.enclosure.api import EnclosureAPI
 from ovos_utils.gui import (GUIInterface,
                             is_gui_running, is_gui_connected)
 from ovos_utils.log import LOG
 from ovos_utils.skills.settings import PrivateSettings
 from ovos_utils.network_utils import is_connected
+from ovos_utils.process_utils import RuntimeRequirements
+
 
 # Event Documentation
 # ===================
 # Registration:
 # ----------------
 # ovos.phal.wifi.plugin.register.client
 # type: Request
@@ -186,14 +189,23 @@
 
         # Check if internet is ready for mycroft_ready
         self.bus.on("mycroft.internet.is_ready", self.handle_ready_check)
 
         self.enclosure = EnclosureAPI(bus=self.bus, skill_id=self.name)
         self.start_internet_check()
 
+    @classproperty
+    def runtime_requirements(self):
+        return RuntimeRequirements(internet_before_load=False,
+                                   network_before_load=False,
+                                   requires_internet=False,
+                                   requires_network=False,
+                                   no_internet_fallback=True,
+                                   no_network_fallback=True)
+
     @property
     def first_boot(self):
         return self.settings.get("first_boot", True)
 
     @first_boot.setter
     def first_boot(self, val):
         self.settings["first_boot"] = bool(val)
@@ -226,19 +238,23 @@
         client_plugin_type = message.data.get("type", "")
         client_plugin_display_text = message.data.get("display_text", "")
         client_plugin_has_gui = message.data.get("has_gui", False)
         client_plugin_requires_input = message.data.get("requires_input", False)
 
         # Fist make sure the required parameters are present
         if not client_plugin_name or not client_plugin_type or not client_plugin_display_text:
-            self.bus.emit(Message("ovos.phal.wifi.plugin.client.registration.failure", {"error": "Missing required parameters"}))
+            self.bus.emit(
+                Message("ovos.phal.wifi.plugin.client.registration.failure",
+                        {"error": "Missing required parameters"}))
             return
 
         if not client_plugin_has_gui and not client_plugin_requires_input:
-            self.bus.emit(Message("ovos.phal.wifi.plugin.client.registration.failure", {"error": "Missing required parameters"}))
+            self.bus.emit(
+                Message("ovos.phal.wifi.plugin.client.registration.failure",
+                        {"error": "Missing required parameters"}))
             return
 
         # Use the client plugin id for activation and deactivation rather than depending on parameters in the message
         random_uuid = str(uuid.uuid4())
         client_plugin_id = client_plugin_name[-2:] + client_plugin_type[-2:] + str(
             random.randint(0, 9)) + str(random.randint(0, 9)) + random_uuid[-1:] + random_uuid[0]
 
@@ -359,15 +375,15 @@
         self.in_setup = True
         self.gui.clear()
         page = join(dirname(__file__), "ui", "WifiPluginClientLoader.qml")
         self.gui["page_type"] = "ModeChoose"
         self.gui["clients_model"] = self.registered_clients
         self.gui.show_page(page, override_idle=self.first_boot or None,
                            override_animations=True)
-        
+
     def handle_skip_setup(self, message=None):
         self.in_setup = False
         self.client_in_setup = False
         self.active_client = None
         self.active_client_id = None
 
         # Deactivate the running watchdog daemon
@@ -399,15 +415,15 @@
             Message("ovos.phal.wifi.plugin.fully_offline")
         self.bus.emit(message)
         self.gui.clear()
 
     def handle_user_activated(self, message=None):
         # enable the watchdog if user activated the service manually
         self.enable_watchdog = True
-        
+
         # first check the plugin setup mode
         if self.plugin_setup_mode == 1:
             self.plugin_setup_mode = 0
             self.start_internet_check()
         else:
             # Assume the user wants to run the setup process manually
             self.launch_networking_setup()
@@ -425,15 +441,15 @@
             if self.plugin_setup_mode == 0:
                 create_daemon(self._watchdog)
             else:
                 LOG.info("Internet check disabled by user")
         else:  # User selected offline mode
             self.plugin_setup_mode = 1  # Advertise internet is ready
             LOG.info("Internet check disabled by skip network setup")
-        
+
     def stop_internet_check(self):
         self.monitoring = False
 
     def _watchdog(self):
         try:
             self.monitoring = True
             LOG.info("Wifi watchdog started")
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a2/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO` & `ovos-PHAL-plugin-wifi-setup-1.1.1a3/ovos_PHAL_plugin_wifi_setup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wifi-setup
-Version: 1.1.1a2
+Version: 1.1.1a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wifi-setup
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wifi-setup-1.1.1a2/setup.py` & `ovos-PHAL-plugin-wifi-setup-1.1.1a3/setup.py`

 * *Files identical despite different names*

