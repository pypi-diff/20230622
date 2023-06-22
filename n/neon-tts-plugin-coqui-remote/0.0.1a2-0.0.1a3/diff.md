# Comparing `tmp/neon-tts-plugin-coqui-remote-0.0.1a2.tar.gz` & `tmp/neon-tts-plugin-coqui-remote-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.1a2.tar", last modified: Thu Jun 22 01:02:26 2023, max compression
+gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.1a3.tar", last modified: Thu Jun 22 01:16:29 2023, max compression
```

## Comparing `neon-tts-plugin-coqui-remote-0.0.1a2.tar` & `neon-tts-plugin-coqui-remote-0.0.1a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:16:29.245917 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:16:29.000000 neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:16:29.249917 neon-tts-plugin-coqui-remote-0.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-22 01:16:22.000000 neon-tts-plugin-coqui-remote-0.0.1a3/setup.py
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a2/LICENSE.md` & `neon-tts-plugin-coqui-remote-0.0.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a2/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/__init__.py` & `neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,54 +26,73 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import requests
 
 from urllib.parse import quote
 from typing import Optional
-from ovos_plugin_manager.templates.tts import RemoteTTS, TTSValidator
+from ovos_plugin_manager.templates.tts import RemoteTTS, TTSValidator, RemoteTTSException
 
 from .configs import languages
 
 
 class CoquiRemoteTTS(RemoteTTS):
     # TODO: Update to query remote API
     langs = languages
+    public_servers = ['https://coqui.2021.us']
 
-    def __init__(self, lang: str = "en", config: dict = None, api_path: str = '/synthesize'):
-        default_url = 'https://coqui.2021.us'
+    def __init__(self, lang: str = "en", config: dict = None,
+                 api_path: str = '/synthesize'):
         config = config or dict()
-        super(CoquiRemoteTTS, self).__init__(lang, config, default_url, api_path, CoquiRemoteTTSValidator(self))
+        RemoteTTS.__init__(self, lang, config, url="", api_path=api_path,
+                           validator=CoquiRemoteTTSValidator(self))
 
     def get_tts(self, sentence: str, output_file: str,
-                speaker: Optional[dict] = None, lang: Optional[str] = None) -> (str, Optional[str]):
+                speaker: Optional[dict] = None,
+                lang: Optional[str] = None) -> (str, Optional[str]):
         """
         Get Synthesized audio
         Args:
             sentence: string to synthesize
             output_file: path to output audio file
             speaker: optional dict speaker data
             lang: optional lang override
         Returns:
             tuple wav_file, optional phonemes
         """
         speaker = speaker or dict()
         lang = lang or speaker.get('language') or self.lang
 
-        resp = requests.get(f'{self.url}{self.api_path}/{quote(sentence)}', params={'lang': lang})
-        if resp.status_code != 200:
-            return None
+        if not self.url:
+            resp = self._get_from_public_servers(lang, sentence)
+        else:
+            resp = requests.get(f'{self.url}{self.api_path}/{quote(sentence)}',
+                                params={'lang': lang})
+            if not resp.ok:
+                raise RemoteTTSException(resp.text)
         with open(output_file, 'wb') as f:
             f.write(resp.content)
         return output_file, None
 
     @property
     def available_languages(self):
         return set(self.langs.keys())
 
+    def _get_from_public_servers(self, lang, sentence):
+        for url in self.public_servers:
+            try:
+                r = requests.get(f'{url}{self.api_path}/{quote(sentence)}',
+                                 params={'lang': lang})
+                if r.ok:
+                    return r
+            except:
+                continue
+        raise RemoteTTSException(f"All Coqui public servers are down, "
+                                 f"please self host Coqui")
+
 
 class CoquiRemoteTTSValidator(TTSValidator):
     def __init__(self, tts):
         super(CoquiRemoteTTSValidator, self).__init__(tts)
 
     def validate_lang(self):
         if self.tts.lang.split('-')[0] not in CoquiRemoteTTS.langs:
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/configs.py` & `neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote/configs.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.1a3/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a2/setup.py` & `neon-tts-plugin-coqui-remote-0.0.1a3/setup.py`

 * *Files identical despite different names*

