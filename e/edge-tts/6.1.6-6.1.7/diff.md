# Comparing `tmp/edge-tts-6.1.6.tar.gz` & `tmp/edge-tts-6.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-tts-6.1.6.tar", last modified: Fri Jun  2 17:06:26 2023, max compression
+gzip compressed data, was "edge-tts-6.1.7.tar", last modified: Thu Jun 22 15:11:03 2023, max compression
```

## Comparing `edge-tts-6.1.6.tar` & `edge-tts-6.1.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.119232 edge-tts-6.1.6/.github/
--rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.6/.github/dependabot.yml
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/.github/workflows/
--rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.6/.github/workflows/code-quality.yml
--rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.6/.github/workflows/codeql-analysis.yml
--rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.6/.gitignore
--rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.6/.isort.cfg
--rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.6/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-06-02 17:06:26.123232 edge-tts-6.1.6/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3477 2023-04-30 20:56:25.000000 edge-tts-6.1.6/README.md
--rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.6/build_and_publish.sh
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/examples/
--rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-02 17:04:37.000000 edge-tts-6.1.6/examples/basic_audio_streaming.py
--rw-rw-r--   0 user      (1000) user      (1000)      492 2023-06-02 17:04:44.000000 edge-tts-6.1.6/examples/basic_generation.py
--rw-rw-r--   0 user      (1000) user      (1000)      754 2023-06-02 17:04:50.000000 edge-tts-6.1.6/examples/dynamic_voice_selection.py
--rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-06-02 17:04:56.000000 edge-tts-6.1.6/examples/streaming_with_subtitles.py
--rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.6/format.sh
--rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.6/lint.sh
--rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.6/mypy.ini
--rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-04-30 20:48:15.000000 edge-tts-6.1.6/pylintrc
--rw-rw-r--   0 user      (1000) user      (1000)      834 2023-06-02 17:06:26.123232 edge-tts-6.1.6/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.6/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.119232 edge-tts-6.1.6/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/src/edge_playback/
--rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.6/src/edge_playback/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-01-10 14:38:06.000000 edge-tts-6.1.6/src/edge_playback/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.6/src/edge_playback/py.typed
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/src/edge_tts/
--rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.6/src/edge_tts/__init__.py
--rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.6/src/edge_tts/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)    16836 2023-05-03 19:21:45.000000 edge-tts-6.1.6/src/edge_tts/communicate.py
--rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.6/src/edge_tts/constants.py
--rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.6/src/edge_tts/exceptions.py
--rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.6/src/edge_tts/list_voices.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.6/src/edge_tts/py.typed
--rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.6/src/edge_tts/submaker.py
--rw-rw-r--   0 user      (1000) user      (1000)     4385 2023-06-02 17:05:35.000000 edge-tts-6.1.6/src/edge_tts/util.py
--rw-rw-r--   0 user      (1000) user      (1000)      128 2023-06-02 17:06:07.000000 edge-tts-6.1.6/src/edge_tts/version.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 17:06:26.123232 edge-tts-6.1.6/src/edge_tts.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      903 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       98 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       46 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       23 2023-06-02 17:06:26.000000 edge-tts-6.1.6/src/edge_tts.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.805001 edge-tts-6.1.7/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.801001 edge-tts-6.1.7/.github/
+-rw-rw-r--   0 user      (1000) user      (1000)      106 2022-09-27 09:16:55.000000 edge-tts-6.1.7/.github/dependabot.yml
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.805001 edge-tts-6.1.7/.github/workflows/
+-rw-rw-r--   0 user      (1000) user      (1000)      585 2023-01-05 05:52:51.000000 edge-tts-6.1.7/.github/workflows/code-quality.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     2277 2022-09-27 09:17:01.000000 edge-tts-6.1.7/.github/workflows/codeql-analysis.yml
+-rw-rw-r--   0 user      (1000) user      (1000)     3078 2023-01-05 05:54:43.000000 edge-tts-6.1.7/.gitignore
+-rw-rw-r--   0 user      (1000) user      (1000)      161 2023-01-04 23:46:51.000000 edge-tts-6.1.7/.isort.cfg
+-rw-------   0 user      (1000) user      (1000)    35149 2021-12-03 12:08:58.000000 edge-tts-6.1.7/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-06-22 15:11:03.805001 edge-tts-6.1.7/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     3477 2023-04-30 20:56:25.000000 edge-tts-6.1.7/README.md
+-rwx------   0 user      (1000) user      (1000)      136 2023-01-05 05:59:23.000000 edge-tts-6.1.7/build_and_publish.sh
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.805001 edge-tts-6.1.7/examples/
+-rw-rw-r--   0 user      (1000) user      (1000)     1005 2023-06-02 17:04:37.000000 edge-tts-6.1.7/examples/basic_audio_streaming.py
+-rw-rw-r--   0 user      (1000) user      (1000)      492 2023-06-02 17:04:44.000000 edge-tts-6.1.7/examples/basic_generation.py
+-rw-rw-r--   0 user      (1000) user      (1000)      754 2023-06-02 17:04:50.000000 edge-tts-6.1.7/examples/dynamic_voice_selection.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1070 2023-06-02 17:04:56.000000 edge-tts-6.1.7/examples/streaming_with_subtitles.py
+-rwxrwxr-x   0 user      (1000) user      (1000)       99 2023-01-04 23:47:18.000000 edge-tts-6.1.7/format.sh
+-rwxrwxr-x   0 user      (1000) user      (1000)      108 2023-01-20 00:45:15.000000 edge-tts-6.1.7/lint.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      561 2023-01-04 23:38:10.000000 edge-tts-6.1.7/mypy.ini
+-rw-rw-r--   0 user      (1000) user      (1000)    20395 2023-04-30 20:48:15.000000 edge-tts-6.1.7/pylintrc
+-rw-rw-r--   0 user      (1000) user      (1000)      834 2023-06-22 15:11:03.805001 edge-tts-6.1.7/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      192 2023-01-04 23:17:58.000000 edge-tts-6.1.7/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.801001 edge-tts-6.1.7/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.805001 edge-tts-6.1.7/src/edge_playback/
+-rw-rw-r--   0 user      (1000) user      (1000)      109 2023-01-05 05:52:51.000000 edge-tts-6.1.7/src/edge_playback/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2053 2023-06-18 15:33:31.000000 edge-tts-6.1.7/src/edge_playback/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-04 23:17:58.000000 edge-tts-6.1.7/src/edge_playback/py.typed
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.805001 edge-tts-6.1.7/src/edge_tts/
+-rw-rw-r--   0 user      (1000) user      (1000)      317 2023-01-09 19:17:13.000000 edge-tts-6.1.7/src/edge_tts/__init__.py
+-rw-------   0 user      (1000) user      (1000)       94 2021-12-07 19:17:40.000000 edge-tts-6.1.7/src/edge_tts/__main__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    16863 2023-06-22 15:09:58.000000 edge-tts-6.1.7/src/edge_tts/communicate.py
+-rw-rw-r--   0 user      (1000) user      (1000)      416 2023-01-05 05:52:51.000000 edge-tts-6.1.7/src/edge_tts/constants.py
+-rw-rw-r--   0 user      (1000) user      (1000)      558 2023-04-05 13:39:33.000000 edge-tts-6.1.7/src/edge_tts/exceptions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2587 2023-01-09 16:29:31.000000 edge-tts-6.1.7/src/edge_tts/list_voices.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-05 04:26:59.000000 edge-tts-6.1.7/src/edge_tts/py.typed
+-rw-rw-r--   0 user      (1000) user      (1000)     3823 2023-04-05 14:00:08.000000 edge-tts-6.1.7/src/edge_tts/submaker.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4385 2023-06-02 17:05:35.000000 edge-tts-6.1.7/src/edge_tts/util.py
+-rw-rw-r--   0 user      (1000) user      (1000)      128 2023-06-22 15:10:15.000000 edge-tts-6.1.7/src/edge_tts/version.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-22 15:11:03.805001 edge-tts-6.1.7/src/edge_tts.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     4031 2023-06-22 15:11:03.000000 edge-tts-6.1.7/src/edge_tts.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      903 2023-06-22 15:11:03.000000 edge-tts-6.1.7/src/edge_tts.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-22 15:11:03.000000 edge-tts-6.1.7/src/edge_tts.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       98 2023-06-22 15:11:03.000000 edge-tts-6.1.7/src/edge_tts.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2023-06-22 15:11:03.000000 edge-tts-6.1.7/src/edge_tts.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       23 2023-06-22 15:11:03.000000 edge-tts-6.1.7/src/edge_tts.egg-info/top_level.txt
```

### Comparing `edge-tts-6.1.6/.github/workflows/code-quality.yml` & `edge-tts-6.1.7/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/.github/workflows/codeql-analysis.yml` & `edge-tts-6.1.7/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/.gitignore` & `edge-tts-6.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/LICENSE` & `edge-tts-6.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/PKG-INFO` & `edge-tts-6.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.6
+Version: 6.1.7
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
```

### Comparing `edge-tts-6.1.6/README.md` & `edge-tts-6.1.7/README.md`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/examples/basic_audio_streaming.py` & `edge-tts-6.1.7/examples/basic_audio_streaming.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/examples/dynamic_voice_selection.py` & `edge-tts-6.1.7/examples/dynamic_voice_selection.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/examples/streaming_with_subtitles.py` & `edge-tts-6.1.7/examples/streaming_with_subtitles.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/mypy.ini` & `edge-tts-6.1.7/mypy.ini`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/pylintrc` & `edge-tts-6.1.7/pylintrc`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/setup.cfg` & `edge-tts-6.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/src/edge_playback/__main__.py` & `edge-tts-6.1.7/src/edge_playback/__main__.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/src/edge_tts/communicate.py` & `edge-tts-6.1.7/src/edge_tts/communicate.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,19 +244,20 @@
         if not isinstance(text, str):
             raise TypeError("text must be str")
         self.text: str = text
 
         # Possible values for voice are:
         # - Microsoft Server Speech Text to Speech Voice (cy-GB, NiaNeural)
         # - cy-GB-NiaNeural
+	# - fil-PH-AngeloNeural
         # Always send the first variant as that is what Microsoft Edge does.
         if not isinstance(voice, str):
             raise TypeError("voice must be str")
         self.voice: str = voice
-        match = re.match(r"^([a-z]{2})-([A-Z]{2})-(.+Neural)$", voice)
+        match = re.match(r"^([a-z]{2,})-([A-Z]{2,})-(.+Neural)$", voice)
         if match is not None:
             lang = match.group(1)
             region = match.group(2)
             name = match.group(3)
             if name.find("-") != -1:
                 region = region + "-" + name[: name.find("-")]
                 name = name[name.find("-") + 1 :]
```

### Comparing `edge-tts-6.1.6/src/edge_tts/exceptions.py` & `edge-tts-6.1.7/src/edge_tts/exceptions.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/src/edge_tts/list_voices.py` & `edge-tts-6.1.7/src/edge_tts/list_voices.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/src/edge_tts/submaker.py` & `edge-tts-6.1.7/src/edge_tts/submaker.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/src/edge_tts/util.py` & `edge-tts-6.1.7/src/edge_tts/util.py`

 * *Files identical despite different names*

### Comparing `edge-tts-6.1.6/src/edge_tts.egg-info/PKG-INFO` & `edge-tts-6.1.7/src/edge_tts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-tts
-Version: 6.1.6
+Version: 6.1.7
 Summary: Microsoft Edge's TTS
 Home-page: https://github.com/rany2/edge-tts
 Author: rany
 Author-email: ranygh@riseup.net
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/rany2/edge-tts/issues
 Platform: UNKNOWN
```

### Comparing `edge-tts-6.1.6/src/edge_tts.egg-info/SOURCES.txt` & `edge-tts-6.1.7/src/edge_tts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

