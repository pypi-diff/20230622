# Comparing `tmp/ovos-PHAL-plugin-alsa-0.0.3a4.tar.gz` & `tmp/ovos-PHAL-plugin-alsa-0.0.3a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.3a4.tar", last modified: Wed Jun 21 18:38:46 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-alsa-0.0.3a5.tar", last modified: Wed Jun 21 19:09:20 2023, max compression
```

## Comparing `ovos-PHAL-plugin-alsa-0.0.3a4.tar` & `ovos-PHAL-plugin-alsa-0.0.3a5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.930738 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87676 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 18:38:46.000000 ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2990 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 18:38:46.934738 ovos-PHAL-plugin-alsa-0.0.3a4/test/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 18:38:43.000000 ovos-PHAL-plugin-alsa-0.0.3a4/test/test_alsa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:09:20.856306 ovos-PHAL-plugin-alsa-0.0.3a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 19:09:20.856306 ovos-PHAL-plugin-alsa-0.0.3a5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:09:20.856306 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa/
+-rw-r--r--   0 runner    (1001) docker     (123)     8452 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87676 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:09:20.856306 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-21 19:09:20.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-21 19:09:20.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:09:20.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 19:09:20.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-21 19:09:20.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-21 19:09:20.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 19:09:20.000000 ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 19:09:20.856306 ovos-PHAL-plugin-alsa-0.0.3a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2990 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 19:09:20.856306 ovos-PHAL-plugin-alsa-0.0.3a5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-21 19:09:16.000000 ovos-PHAL-plugin-alsa-0.0.3a5/test/test_alsa.py
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a4/LICENSE` & `ovos-PHAL-plugin-alsa-0.0.3a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a4/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.3a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/__init__.py` & `ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def validate(config=None):
         """ this method is called before loading the plugin.
         If it returns False the plugin is not loaded.
         This allows a plugin to run platform checks"""
         # any aliases we need here ?
         execs = ["pulseaudio"]
         is_pulse = any((find_executable(e) or is_process_running(e)
-                    for e in execs))
+                        for e in execs))
 
         # check if pulseaudio is installed in system
         # if missing load alsa
         if not is_pulse:
             return True
 
         # check if pulse plugin is installed
@@ -144,21 +144,14 @@
         super().shutdown()
 
 
 class AlsaControl:
     _mixer = None
 
     def __init__(self, control=None):
-        # TODO: Deprecate class in 0.1
-        LOG.warning(f"This class is deprecated! Controls moved to"
-                    f"ovos_phal_plugin_alsa.AlsaVolumeControlPlugin")
-        if alsaaudio is None:
-            LOG.error("pyalsaaudio not installed")
-            LOG.info("Run pip install pyalsaaudio==0.8.2")
-            raise ImportError
         if control is None:
             control = alsaaudio.mixers()[0]
         self.get_mixer(control)
 
     @property
     def mixer(self):
         return self._mixer
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav` & `ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa/blop-mark-diangelo.wav`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a4/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO` & `ovos-PHAL-plugin-alsa-0.0.3a5/ovos_PHAL_plugin_alsa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-PHAL-plugin-alsa
-Version: 0.0.3a4
+Version: 0.0.3a5
 Summary: A volume control plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-alsa
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a4/setup.py` & `ovos-PHAL-plugin-alsa-0.0.3a5/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-alsa-0.0.3a4/test/test_alsa.py` & `ovos-PHAL-plugin-alsa-0.0.3a5/test/test_alsa.py`

 * *Files identical despite different names*

