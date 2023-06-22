# Comparing `tmp/neon-tts-plugin-coqui-remote-0.0.1a0.tar.gz` & `tmp/neon-tts-plugin-coqui-remote-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.1a0.tar", last modified: Fri Nov 11 20:47:30 2022, max compression
+gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.1a1.tar", last modified: Thu Jun 22 00:49:37 2023, max compression
```

## Comparing `neon-tts-plugin-coqui-remote-0.0.1a0.tar` & `neon-tts-plugin-coqui-remote-0.0.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 20:47:30.171869 neon-tts-plugin-coqui-remote-0.0.1a0/
--rw-r--r--   0 runner    (1001) docker     (121)     1634 2022-11-11 20:47:25.000000 neon-tts-plugin-coqui-remote-0.0.1a0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-11-11 20:47:30.167869 neon-tts-plugin-coqui-remote-0.0.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-11 20:47:25.000000 neon-tts-plugin-coqui-remote-0.0.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 20:47:30.167869 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote/
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-11-11 20:47:25.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14191 2022-11-11 20:47:25.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 20:47:30.167869 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-11-11 20:47:30.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-11-11 20:47:30.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 20:47:30.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-11 20:47:30.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-11 20:47:30.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-11-11 20:47:30.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 20:47:30.000000 neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 20:47:30.171869 neon-tts-plugin-coqui-remote-0.0.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4051 2022-11-11 20:47:25.000000 neon-tts-plugin-coqui-remote-0.0.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:49:37.002257 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 00:49:37.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/setup.py
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a0/LICENSE.md` & `neon-tts-plugin-coqui-remote-0.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a0/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.1a1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
-Description: # NeonAI Coqui AI Remote TTS Plugin
-        [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
-        TTS Plugin for Remote Coqui AI Text-to-Speech. This plugin connects to a remote Coqui TTS server for TTS processing
-        
-        ## Configuration
-        ```yaml
-        TTS:
-          module: neon-tts-plugin-coqui-remote
-        ```
-        ## Language Support
-        See the [neon-tts-plugin-coqui](https://github.com/NeonGeckoCom/neon-tts-plugin-coqui) plugin for updated language
-        support info.
 Keywords: mycroft plugin tts
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# NeonAI Coqui AI Remote TTS Plugin
+[Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
+TTS Plugin for Remote Coqui AI Text-to-Speech. This plugin connects to a remote Coqui TTS server for TTS processing
+
+## Configuration
+```yaml
+TTS:
+  module: neon-tts-plugin-coqui-remote
+```
+## Language Support
+See the [neon-tts-plugin-coqui](https://github.com/NeonGeckoCom/neon-tts-plugin-coqui) plugin for updated language
+support info.
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote/__init__.py` & `neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote/configs.py` & `neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/configs.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a0/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
-Description: # NeonAI Coqui AI Remote TTS Plugin
-        [Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
-        TTS Plugin for Remote Coqui AI Text-to-Speech. This plugin connects to a remote Coqui TTS server for TTS processing
-        
-        ## Configuration
-        ```yaml
-        TTS:
-          module: neon-tts-plugin-coqui-remote
-        ```
-        ## Language Support
-        See the [neon-tts-plugin-coqui](https://github.com/NeonGeckoCom/neon-tts-plugin-coqui) plugin for updated language
-        support info.
 Keywords: mycroft plugin tts
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# NeonAI Coqui AI Remote TTS Plugin
+[Mycroft](https://mycroft-ai.gitbook.io/docs/mycroft-technologies/mycroft-core/plugins) compatible
+TTS Plugin for Remote Coqui AI Text-to-Speech. This plugin connects to a remote Coqui TTS server for TTS processing
+
+## Configuration
+```yaml
+TTS:
+  module: neon-tts-plugin-coqui-remote
+```
+## Language Support
+See the [neon-tts-plugin-coqui](https://github.com/NeonGeckoCom/neon-tts-plugin-coqui) plugin for updated language
+support info.
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a0/setup.py` & `neon-tts-plugin-coqui-remote-0.0.1a1/setup.py`

 * *Files identical despite different names*

