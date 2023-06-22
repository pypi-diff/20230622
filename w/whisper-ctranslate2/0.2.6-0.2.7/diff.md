# Comparing `tmp/whisper-ctranslate2-0.2.6.tar.gz` & `tmp/whisper-ctranslate2-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.2.6.tar", last modified: Tue Jun  6 05:27:30 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.2.7.tar", last modified: Thu Jun 22 10:37:17 2023, max compression
```

## Comparing `whisper-ctranslate2-0.2.6.tar` & `whisper-ctranslate2-0.2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5232 2023-06-06 05:24:38.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     6324 2023-06-06 05:24:38.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-05-27 11:37:32.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    17517 2023-06-06 05:24:38.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    10359 2023-05-27 10:54:49.000000 whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-06 05:27:30.020632 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-06-06 05:27:29.000000 whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-22 10:37:17.105853 whisper-ctranslate2-0.2.7/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.7/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-06-22 10:37:17.105853 whisper-ctranslate2-0.2.7/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4990 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.7/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-06-22 10:37:17.105853 whisper-ctranslate2-0.2.7/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1501 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.7/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-22 10:37:17.105853 whisper-ctranslate2-0.2.7/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-22 10:37:17.105853 whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-05-22 19:00:07.000000 whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5250 2023-06-22 07:28:46.000000 whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6324 2023-06-22 07:28:04.000000 whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-06-06 05:29:36.000000 whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    17517 2023-06-22 05:48:32.000000 whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    10359 2023-05-27 10:54:49.000000 whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-06-22 10:37:17.105853 whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5623 2023-06-22 10:37:17.000000 whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      520 2023-06-22 10:37:17.000000 whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-06-22 10:37:17.000000 whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       89 2023-06-22 10:37:17.000000 whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      100 2023-06-22 10:37:17.000000 whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-06-22 10:37:17.000000 whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.2.6/LICENSE` & `whisper-ctranslate2-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.6/PKG-INFO` & `whisper-ctranslate2-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.6
+Version: 0.2.7
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `whisper-ctranslate2-0.2.6/README.md` & `whisper-ctranslate2-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.6/setup.py` & `whisper-ctranslate2-0.2.7/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/live.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
                     self.compute_type,
                     self.threads,
                     self.cache_directory,
                     self.local_files_only,
                 )
 
             result = self.transcribe.inference(
-                audio=_buffer.flatten(),
+                audio=_buffer.flatten().astype("float32"),
                 task=self.task,
                 language=self.language,
                 verbose=self.verbose,
                 live=True,
                 options=self.options,
             )
             print(f"\033[1A\033[2K\033[0G{result['text']}")
```

### Comparing `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/transcribe.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.6/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.2.7/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.2.6
+Version: 0.2.7
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/Softcatala/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `whisper-ctranslate2-0.2.6/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.2.7/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

