# Comparing `tmp/ovos-tts-server-0.0.3a6.tar.gz` & `tmp/ovos-tts-server-0.0.3a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-server-0.0.3a6.tar", last modified: Tue May 30 18:08:34 2023, max compression
+gzip compressed data, was "ovos-tts-server-0.0.3a7.tar", last modified: Thu Jun 22 03:33:43 2023, max compression
```

## Comparing `ovos-tts-server-0.0.3a6.tar` & `ovos-tts-server-0.0.3a7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/ovos_tts_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/ovos_tts_server/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/examples/rainbow.json
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/gradio_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:33:43.963886 ovos-tts-server-0.0.3a7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 03:33:43.963886 ovos-tts-server-0.0.3a7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:33:43.963886 ovos-tts-server-0.0.3a7/ovos_tts_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:33:43.963886 ovos-tts-server-0.0.3a7/ovos_tts_server/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server/examples/rainbow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:33:43.963886 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:33:43.963886 ovos-tts-server-0.0.3a7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-06-22 03:33:43.000000 ovos-tts-server-0.0.3a7/setup.py
```

### Comparing `ovos-tts-server-0.0.3a6/LICENSE.md` & `ovos-tts-server-0.0.3a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a6/PKG-INFO` & `ovos-tts-server-0.0.3a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.3a6
+Version: 0.0.3a7
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-tts-server-0.0.3a6/ovos_tts_server/__init__.py` & `ovos-tts-server-0.0.3a7/ovos_tts_server/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from fastapi import FastAPI
 from fastapi.responses import FileResponse
 from ovos_plugin_manager.tts import load_tts_plugin
 from ovos_utils.log import LOG
+from ovos_config import Configuration
 from starlette.requests import Request
 
 TTS = None
 
 
 def create_app(tts_plugin):
     app = FastAPI()
@@ -37,14 +38,16 @@
 
 def start_tts_server(tts_plugin, cache=False):
     global TTS
 
     # load ovos TTS plugin
     engine = load_tts_plugin(tts_plugin)
 
-    TTS = engine(config={"persist_cache": cache})  # this will cache every synth even across reboots
+    config = Configuration().get("tts", {}).get(tts_plugin, {})
+    config["persist_cache"] = cache  # this will cache every synth even across reboots
+    TTS = engine(config=config)
     TTS.log_timestamps = True  # enable logging
 
     app = create_app(tts_plugin)
     return app, TTS
```

### Comparing `ovos-tts-server-0.0.3a6/ovos_tts_server/__main__.py` & `ovos-tts-server-0.0.3a7/ovos_tts_server/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a6/ovos_tts_server/examples/rainbow.json` & `ovos-tts-server-0.0.3a7/ovos_tts_server/examples/rainbow.json`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a6/ovos_tts_server/gradio_app.py` & `ovos-tts-server-0.0.3a7/ovos_tts_server/gradio_app.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/PKG-INFO` & `ovos-tts-server-0.0.3a7/ovos_tts_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.3a6
+Version: 0.0.3a7
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
```

### Comparing `ovos-tts-server-0.0.3a6/setup.py` & `ovos-tts-server-0.0.3a7/setup.py`

 * *Files identical despite different names*

