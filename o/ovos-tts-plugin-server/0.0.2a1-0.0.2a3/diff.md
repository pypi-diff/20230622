# Comparing `tmp/ovos-tts-plugin-server-0.0.2a1.tar.gz` & `tmp/ovos-tts-plugin-server-0.0.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-plugin-server-0.0.2a1.tar", last modified: Thu Sep 29 16:09:01 2022, max compression
+gzip compressed data, was "ovos-tts-plugin-server-0.0.2a3.tar", last modified: Thu Jun 22 01:55:16 2023, max compression
```

## Comparing `ovos-tts-plugin-server-0.0.2a1.tar` & `ovos-tts-plugin-server-0.0.2a3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 16:09:01.397000 ovos-tts-plugin-server-0.0.2a1/
--rw-rw-r--   0 user      (1000) user      (1000)      995 2022-09-29 16:09:01.396000 ovos-tts-plugin-server-0.0.2a1/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 16:09:01.396000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server/
--rwxrwxr-x   0 user      (1000) user      (1000)     1618 2022-09-29 16:07:54.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-29 16:09:01.396000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      995 2022-09-29 16:09:01.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      362 2022-09-29 16:09:01.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-29 16:09:01.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      187 2022-09-29 16:09:01.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       27 2022-09-29 16:09:01.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       23 2022-09-29 16:09:01.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-29 16:09:01.000000 ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server.egg-info/zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-09-29 16:09:01.397000 ovos-tts-plugin-server-0.0.2a1/setup.cfg
--rwxrwxr-x   0 user      (1000) user      (1000)     1549 2022-09-29 16:07:54.000000 ovos-tts-plugin-server-0.0.2a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1706 2023-06-22 01:55:11.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-22 01:55:11.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:55:16.000000 ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:55:16.212165 ovos-tts-plugin-server-0.0.2a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3279 2023-06-22 01:55:11.000000 ovos-tts-plugin-server-0.0.2a3/setup.py
```

### Comparing `ovos-tts-plugin-server-0.0.2a1/ovos_tts_plugin_server/__init__.py` & `ovos-tts-plugin-server-0.0.2a3/ovos_tts_plugin_server/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,22 +32,25 @@
         return OVOSServerTTS
 
 
 OVOSServerTTSConfig = {}
 
 # jarbas public demo instances
 jarbas_hosted = {
-    "S.A.M.": ("https://sam.jarbasai.online", "male"),
-    "PicoTTS": ("https://pico.jarbasai.online", "female"),
-    "Glados": ("https://glados.jarbasai.online", "female"),
-    "Alan Pope [Mimic 1]": ("https://mimic.jarbasai.online", "male"),
-    "R2D2": ("https://r2d2.jarbasai.online", "neutral")
+    "S.A.M.": ("https://sam.jarbasai.online", "male", 100),
+    "PicoTTS": ("https://pico.jarbasai.online", "female", 90),
+    "Glados": ("https://glados.jarbasai.online", "female", 60),
+    "Alan Pope [Mimic 1]": ("https://mimic.jarbasai.online", "male", 80),
+    "R2D2": ("https://r2d2.jarbasai.online", "neutral", 95)
 }
 
 OVOSServerTTSConfig["en-us"] = [
     {"lang": "en-us",
      "url": url,
-     "gender": gender,
-     "display_name": f"{display_name} (jarbasai.online)",
-     "offline": False}
-    for display_name, (url, gender) in jarbas_hosted.items()
+     "meta": {
+         "gender": gender,
+         "priority": prio,
+         "display_name": f"{display_name} (jarbasai.online)",
+         "offline": False}
+     }
+    for display_name, (url, gender, prio) in jarbas_hosted.items()
 ]
```

