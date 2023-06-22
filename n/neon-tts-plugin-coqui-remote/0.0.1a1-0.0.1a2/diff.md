# Comparing `tmp/neon-tts-plugin-coqui-remote-0.0.1a1.tar.gz` & `tmp/neon-tts-plugin-coqui-remote-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.1a1.tar", last modified: Thu Jun 22 00:49:37 2023, max compression
+gzip compressed data, was "neon-tts-plugin-coqui-remote-0.0.1a2.tar", last modified: Thu Jun 22 01:02:26 2023, max compression
```

## Comparing `neon-tts-plugin-coqui-remote-0.0.1a1.tar` & `neon-tts-plugin-coqui-remote-0.0.1a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:49:37.002257 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 00:49:37.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:49:36.000000 neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:49:37.006257 neon-tts-plugin-coqui-remote-0.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-06-22 00:49:28.000000 neon-tts-plugin-coqui-remote-0.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14191 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:02:26.000000 neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 01:02:26.864711 neon-tts-plugin-coqui-remote-0.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-22 01:02:21.000000 neon-tts-plugin-coqui-remote-0.0.1a2/setup.py
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a1/LICENSE.md` & `neon-tts-plugin-coqui-remote-0.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a1/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/__init__.py` & `neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote/configs.py` & `neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote/configs.py`

 * *Files identical despite different names*

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a1/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO` & `neon-tts-plugin-coqui-remote-0.0.1a2/neon_tts_plugin_coqui_remote.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-tts-plugin-coqui-remote
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: A Coqui AI Remote TTS plugin for Neon
 Home-page: https://github.com/NeonGeckoCom/neon-tts-plugin-coqui
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Keywords: mycroft plugin tts
 Classifier: Intended Audience :: Developers
```

### Comparing `neon-tts-plugin-coqui-remote-0.0.1a1/setup.py` & `neon-tts-plugin-coqui-remote-0.0.1a2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,49 +23,45 @@
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 from setuptools import setup, find_packages
-from os import path, getenv
+from os import path, environ
+
+BASE_PATH = path.abspath(path.dirname(__file__))
 
 
 def get_requirements(requirements_filename: str):
-    requirements_file = path.join(path.abspath(path.dirname(__file__)), "requirements", requirements_filename)
+    requirements_file = path.join(BASE_PATH, "requirements", requirements_filename)
     with open(requirements_file, 'r', encoding='utf-8') as r:
         requirements = r.readlines()
-    requirements = [r.strip() for r in requirements if r.strip() and not r.strip().startswith("#")]
-
-    for i in range(0, len(requirements)):
-        r = requirements[i]
-        if "@" in r:
-            parts = [p.lower() if p.strip().startswith("git+http") else p for p in r.split('@')]
-            r = "@".join(parts)
-            if getenv("GITHUB_TOKEN"):
-                if "github.com" in r:
-                    r = r.replace("github.com", f"{getenv('GITHUB_TOKEN')}@github.com")
-            requirements[i] = r
+    requirements = [r.strip() for r in requirements
+                    if r.strip() and not r.strip().startswith("#")]
+    if 'MYCROFT_LOOSE_REQUIREMENTS' in environ:
+        print('USING LOOSE REQUIREMENTS!')
+        requirements = [r.replace('==', '>=').replace('~=', '>=')
+                        for r in requirements]
     return requirements
 
 
-PLUGIN_ENTRY_POINT = 'neon-tts-plugin-coqui-remote = neon_tts_plugin_coqui_remote:CoquiRemoteTTS'
-CONFIG_ENTRY_POINT = 'neon-tts-plugin-coqui-remote.config = neon_tts_plugin_coqui.configs:tts_config'
-
-with open("README.md", "r") as f:
+with open(path.join(BASE_PATH, "README.md"), "r") as f:
     long_description = f.read()
 
-with open("./version.py", "r", encoding="utf-8") as v:
+with open(path.join(BASE_PATH, "version.py"), "r", encoding="utf-8") as v:
     for line in v.readlines():
         if line.startswith("__version__"):
             if '"' in line:
                 version = line.split('"')[1]
             else:
                 version = line.split("'")[1]
 
+PLUGIN_ENTRY_POINT = 'neon-tts-plugin-coqui-remote = neon_tts_plugin_coqui_remote:CoquiRemoteTTS'
+CONFIG_ENTRY_POINT = 'neon-tts-plugin-coqui-remote.config = neon_tts_plugin_coqui.configs:tts_config'
 setup(
     name='neon-tts-plugin-coqui-remote',
     version=version,
     description='A Coqui AI Remote TTS plugin for Neon',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NeonGeckoCom/neon-tts-plugin-coqui',
```

