# Comparing `tmp/ovos-PHAL-plugin-system-0.0.4a6.tar.gz` & `tmp/ovos-PHAL-plugin-system-0.0.4a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a6.tar", last modified: Wed Jun 21 19:41:45 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-system-0.0.4a7.tar", last modified: Wed Jun 21 22:46:20 2023, max compression
```

## Comparing `ovos-PHAL-plugin-system-0.0.4a6.tar` & `ovos-PHAL-plugin-system-0.0.4a7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.810620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/
--rw-r--r--   0 runner    (1001) docker     (123)    12605 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Reboot.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Restart.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Shutdown.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Status.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/loading.json
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-fail.json
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-success.json
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:41:45.000000 ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:41:45.814620 ovos-PHAL-plugin-system-0.0.4a6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-06-21 19:41:38.000000 ovos-PHAL-plugin-system-0.0.4a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.721002 ovos-PHAL-plugin-system-0.0.4a7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 22:46:20.721002 ovos-PHAL-plugin-system-0.0.4a7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Reboot.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Restart.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Shutdown.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Status.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/loading.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-fail.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-success.json
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:46:20.717002 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:46:20.000000 ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:46:20.721002 ovos-PHAL-plugin-system-0.0.4a7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-06-21 22:46:16.000000 ovos-PHAL-plugin-system-0.0.4a7/setup.py
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a6
+Version: 0.0.4a7
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/__init__.py` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ovos_config.locations import OLD_USER_CONFIG, USER_CONFIG, WEB_CONFIG_CACHE
 from ovos_config.meta import get_xdg_base
 
 from ovos_plugin_manager.phal import PHALPlugin
 from ovos_utils import classproperty
 from ovos_utils.gui import GUIInterface
 from ovos_utils.process_utils import RuntimeRequirements
-from ovos_utils.system import system_reboot, ssh_enable,\
+from ovos_utils.system import system_reboot, system_shutdown, ssh_enable,\
     ssh_disable, ntp_sync, restart_service, is_process_running, \
     check_service_active
 from ovos_utils.xdg_utils import xdg_state_home, xdg_cache_home, xdg_data_home
 from ovos_utils.log import LOG
 
 
 class SystemEventsValidator:
@@ -44,15 +44,16 @@
         self.bus.on("system.ssh.status", self.handle_ssh_status)
         self.bus.on("system.ssh.enable", self.handle_ssh_enable_request)
         self.bus.on("system.ssh.disable", self.handle_ssh_disable_request)
         self.bus.on("system.reboot", self.handle_reboot_request)
         self.bus.on("system.shutdown", self.handle_shutdown_request)
         self.bus.on("system.factory.reset", self.handle_factory_reset_request)
         self.bus.on("system.factory.reset.register", self.handle_reset_register)
-        self.bus.on("system.configure.language", self.handle_configure_language_request)
+        self.bus.on("system.configure.language",
+                    self.handle_configure_language_request)
         self.bus.on("system.mycroft.service.restart",
                     self.handle_mycroft_restart_request)
         self.service_name = config.get("core_service") or "mycroft.service"
         # In Debian, ssh stays active, but sshd is removed when ssh is disabled
         self.ssh_service = config.get("ssh_service") or "sshd.service"
         self.use_root = config.get("sudo", True)
 
@@ -171,20 +172,23 @@
 
         script = message.data.get("script", True)
         if script:
             script = os.path.expanduser(self.config.get("reset_script", ""))
             LOG.debug(f"Running reset script: {script}")
             if os.path.isfile(script):
                 if self.use_external_factory_reset:
-                    self.bus.emit(Message("ovos.shell.exec.factory.reset", {"script": script}))
-                    # OVOS shell will handle all external operations here to exec script
-                    # including sending complete event to whoever is listening
+                    self.bus.emit(Message("ovos.shell.exec.factory.reset",
+                                          {"script": script}))
+                    # OVOS shell will handle all external operations here to
+                    # exec script including sending complete event to whoever
+                    # is listening
                 else:
                     subprocess.call(script, shell=True)
-                    self.bus.emit(message.forward("system.factory.reset.complete"))
+                    self.bus.emit(
+                        message.forward("system.factory.reset.complete"))
 
         reboot = message.data.get("reboot", True)
         if reboot:
             self.bus.emit(message.forward("system.reboot"))
 
     def handle_ssh_enable_request(self, message):
         ssh_enable()
@@ -203,67 +207,75 @@
             self.gui["status"] = "Disabled"
             self.gui["label"] = "SSH Disabled"
             self.gui.show_page(page)
 
     def handle_ntp_sync_request(self, message):
         ntp_sync()
         # NOTE: this one defaults to False
-        # it is usually part of other groups of actions that may provide their own UI
+        # it is usually part of other groups of actions that may
+        # provide their own UI
         if message.data.get("display", False):
             page = join(dirname(__file__), "ui", "Status.qml")
             self.gui["status"] = "Enabled"
             self.gui["label"] = "Clock updated"
             self.gui.show_page(page)
         self.bus.emit(message.reply('system.ntp.sync.complete'))
 
     def handle_reboot_request(self, message):
         if message.data.get("display", True):
             page = join(dirname(__file__), "ui", "Reboot.qml")
-            self.gui.show_page(page, override_animations=True, override_idle=True)
+            self.gui.show_page(page, override_animations=True,
+                               override_idle=True)
 
-        script = os.path.expanduser(self.config.get("reboot_script"))
+        script = os.path.expanduser(self.config.get("reboot_script") or "")
+        LOG.info(f"Reboot requested. script={script}")
         if script and os.path.isfile(script):
             subprocess.call(script, shell=True)
         else:
             system_reboot()
 
     def handle_shutdown_request(self, message):
         if message.data.get("display", True):
             page = join(dirname(__file__), "ui", "Shutdown.qml")
-            self.gui.show_page(page, override_animations=True, override_idle=True)
-        script = os.path.expanduser(self.config.get("shutdown_script"))
+            self.gui.show_page(page, override_animations=True,
+                               override_idle=True)
+        script = os.path.expanduser(self.config.get("shutdown_script") or "")
+        LOG.info(f"Shutdown requested. script={script}")
         if script and os.path.isfile(script):
             subprocess.call(script, shell=True)
         else:
-            system_reboot()
+            system_shutdown()
 
     def handle_configure_language_request(self, message):
         language_code = message.data.get('language_code', "en_US")
-        with open(f"{os.environ['HOME']}/.bash_profile", "w") as bash_profile_file:
+        with open(f"{os.environ['HOME']}/.bash_profile",
+                  "w") as bash_profile_file:
             bash_profile_file.write(f"export LANG={language_code}\n")
 
         language_code = language_code.lower().replace("_", "-")
         set_default_lang(language_code)
         update_mycroft_config({"lang": language_code}, bus=self.bus)
 
         # NOTE: this one defaults to False
-        # it is usually part of other groups of actions that may provide their own UI
+        # it is usually part of other groups of actions that may
+        # provide their own UI
         if message.data.get("display", False):
             page = join(dirname(__file__), "ui", "Status.qml")
             self.gui["status"] = "Enabled"
             self.gui["label"] = f"Language changed to {language_code}"
             self.gui.show_page(page)
 
         self.bus.emit(Message('system.configure.language.complete',
                               {"lang": language_code}))
 
     def handle_mycroft_restart_request(self, message):
         if message.data.get("display", True):
             page = join(dirname(__file__), "ui", "Restart.qml")
-            self.gui.show_page(page, override_animations=True, override_idle=True)
+            self.gui.show_page(page, override_animations=True,
+                               override_idle=True)
         restart_service(self.service_name, sudo=self.use_root)
 
     def handle_ssh_status(self, message):
         """
         Check SSH service status and emit a response
         """
         enabled = check_service_active(self.ssh_service)
@@ -271,12 +283,16 @@
 
     def shutdown(self):
         self.bus.remove("system.ntp.sync", self.handle_ntp_sync_request)
         self.bus.remove("system.ssh.enable", self.handle_ssh_enable_request)
         self.bus.remove("system.ssh.disable", self.handle_ssh_disable_request)
         self.bus.remove("system.reboot", self.handle_reboot_request)
         self.bus.remove("system.shutdown", self.handle_shutdown_request)
-        self.bus.remove("system.factory.reset", self.handle_factory_reset_request)
-        self.bus.remove("system.factory.reset.register", self.handle_reset_register)
-        self.bus.remove("system.configure.language", self.handle_configure_language_request)
-        self.bus.remove("system.mycroft.service.restart", self.handle_mycroft_restart_request)
+        self.bus.remove("system.factory.reset",
+                        self.handle_factory_reset_request)
+        self.bus.remove("system.factory.reset.register",
+                        self.handle_reset_register)
+        self.bus.remove("system.configure.language",
+                        self.handle_configure_language_request)
+        self.bus.remove("system.mycroft.service.restart",
+                        self.handle_mycroft_restart_request)
         super().shutdown()
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Reboot.qml` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Reboot.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Restart.qml` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Restart.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Shutdown.qml` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Shutdown.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/Status.qml` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/Status.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/loading.json` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/loading.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-fail.json` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-fail.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system/ui/animations/status-success.json` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system/ui/animations/status-success.json`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/PKG-INFO` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-system
-Version: 0.0.4a6
+Version: 0.0.4a7
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-system
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/ovos_PHAL_plugin_system.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-system-0.0.4a7/ovos_PHAL_plugin_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-system-0.0.4a6/setup.py` & `ovos-PHAL-plugin-system-0.0.4a7/setup.py`

 * *Files identical despite different names*

