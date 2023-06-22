# Comparing `tmp/streamline-1.1.0.tar.gz` & `tmp/streamline-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamline-1.1.0.tar", last modified: Tue Apr 25 09:17:14 2023, max compression
+gzip compressed data, was "streamline-1.1.1.tar", last modified: Thu Jun 22 14:28:01 2023, max compression
```

## Comparing `streamline-1.1.0.tar` & `streamline-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.103753 streamline-1.1.0/
--rw-r--r--   0 kj         (501) staff       (20)     9975 2023-04-25 09:17:14.103521 streamline-1.1.0/PKG-INFO
--rw-r--r--   0 kj         (501) staff       (20)     9548 2023-04-25 08:36:21.000000 streamline-1.1.0/README.md
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.101410 streamline-1.1.0/bin/
--rwxr-xr-x   0 kj         (501) staff       (20)      146 2023-04-25 08:36:21.000000 streamline-1.1.0/bin/streamline
--rw-r--r--   0 kj         (501) staff       (20)       38 2023-04-25 09:17:14.103804 streamline-1.1.0/setup.cfg
--rw-r--r--   0 kj         (501) staff       (20)      722 2023-04-25 08:36:31.000000 streamline-1.1.0/setup.py
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.102640 streamline-1.1.0/streamline/
--rw-r--r--   0 kj         (501) staff       (20)        1 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/__init__.py
--rw-r--r--   0 kj         (501) staff       (20)    11164 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/cli.py
--rw-r--r--   0 kj         (501) staff       (20)     5110 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/consumers.py
--rw-r--r--   0 kj         (501) staff       (20)     1421 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/core.py
--rw-r--r--   0 kj         (501) staff       (20)     1846 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/entries.py
--rw-r--r--   0 kj         (501) staff       (20)    16679 2023-04-25 09:08:43.000000 streamline-1.1.0/streamline/executors.py
--rw-r--r--   0 kj         (501) staff       (20)     2256 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/extractor.py
--rw-r--r--   0 kj         (501) staff       (20)     4404 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/generators.py
--rw-r--r--   0 kj         (501) staff       (20)    25990 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/streamers.py
--rw-r--r--   0 kj         (501) staff       (20)     2320 2023-04-25 08:36:21.000000 streamline-1.1.0/streamline/utils.py
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-04-25 09:17:14.103258 streamline-1.1.0/streamline.egg-info/
--rw-r--r--   0 kj         (501) staff       (20)     9975 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/PKG-INFO
--rw-r--r--   0 kj         (501) staff       (20)      425 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/SOURCES.txt
--rw-r--r--   0 kj         (501) staff       (20)        1 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/dependency_links.txt
--rw-r--r--   0 kj         (501) staff       (20)        7 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/requires.txt
--rw-r--r--   0 kj         (501) staff       (20)       11 2023-04-25 09:17:14.000000 streamline-1.1.0/streamline.egg-info/top_level.txt
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-06-22 14:28:01.036231 streamline-1.1.1/
+-rw-r--r--   0 kj         (501) staff       (20)     9975 2023-06-22 14:28:01.036097 streamline-1.1.1/PKG-INFO
+-rw-r--r--   0 kj         (501) staff       (20)     9548 2023-04-25 08:36:21.000000 streamline-1.1.1/README.md
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-06-22 14:28:01.033874 streamline-1.1.1/bin/
+-rwxr-xr-x   0 kj         (501) staff       (20)      146 2023-04-25 08:36:21.000000 streamline-1.1.1/bin/streamline
+-rw-r--r--   0 kj         (501) staff       (20)       38 2023-06-22 14:28:01.036265 streamline-1.1.1/setup.cfg
+-rw-r--r--   0 kj         (501) staff       (20)      722 2023-06-22 14:27:29.000000 streamline-1.1.1/setup.py
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-06-22 14:28:01.035331 streamline-1.1.1/streamline/
+-rw-r--r--   0 kj         (501) staff       (20)        1 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/__init__.py
+-rw-r--r--   0 kj         (501) staff       (20)    11164 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/cli.py
+-rw-r--r--   0 kj         (501) staff       (20)     5110 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/consumers.py
+-rw-r--r--   0 kj         (501) staff       (20)     1421 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/core.py
+-rw-r--r--   0 kj         (501) staff       (20)     1846 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/entries.py
+-rw-r--r--   0 kj         (501) staff       (20)    16816 2023-06-22 14:25:50.000000 streamline-1.1.1/streamline/executors.py
+-rw-r--r--   0 kj         (501) staff       (20)     2256 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/extractor.py
+-rw-r--r--   0 kj         (501) staff       (20)     4404 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/generators.py
+-rw-r--r--   0 kj         (501) staff       (20)    25990 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/streamers.py
+-rw-r--r--   0 kj         (501) staff       (20)     2320 2023-04-25 08:36:21.000000 streamline-1.1.1/streamline/utils.py
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-06-22 14:28:01.035911 streamline-1.1.1/streamline.egg-info/
+-rw-r--r--   0 kj         (501) staff       (20)     9975 2023-06-22 14:28:01.000000 streamline-1.1.1/streamline.egg-info/PKG-INFO
+-rw-r--r--   0 kj         (501) staff       (20)      425 2023-06-22 14:28:01.000000 streamline-1.1.1/streamline.egg-info/SOURCES.txt
+-rw-r--r--   0 kj         (501) staff       (20)        1 2023-06-22 14:28:01.000000 streamline-1.1.1/streamline.egg-info/dependency_links.txt
+-rw-r--r--   0 kj         (501) staff       (20)        7 2023-06-22 14:28:01.000000 streamline-1.1.1/streamline.egg-info/requires.txt
+-rw-r--r--   0 kj         (501) staff       (20)       11 2023-06-22 14:28:01.000000 streamline-1.1.1/streamline.egg-info/top_level.txt
```

### Comparing `streamline-1.1.0/PKG-INFO` & `streamline-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamline
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLI tool for doing async tasks and transformations
 Home-page: https://github.com/jdotpy/streamline
 Author: KJ
 Author-email: jdotpy@users.noreply.github.com
 License: UNKNOWN
 Download-URL: https://github.com/jdotpy/streamline/tarball/master
 Keywords: tools
```

### Comparing `streamline-1.1.0/README.md` & `streamline-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/setup.py` & `streamline-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = 'streamline',
     scripts=['bin/streamline'],
     packages=['streamline'],
-    version = '1.1.0',
+    version = '1.1.1',
     description = 'CLI tool for doing async tasks and transformations',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author = 'KJ',
     author_email = 'jdotpy@users.noreply.github.com',
     url = 'https://github.com/jdotpy/streamline',
     download_url = 'https://github.com/jdotpy/streamline/tarball/master',
```

### Comparing `streamline-1.1.0/streamline/cli.py` & `streamline-1.1.1/streamline/cli.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline/consumers.py` & `streamline-1.1.1/streamline/consumers.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline/core.py` & `streamline-1.1.1/streamline/core.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline/entries.py` & `streamline-1.1.1/streamline/entries.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline/executors.py` & `streamline-1.1.1/streamline/executors.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import shlex
 import uuid
 import sys
 import os
 
 from .utils import import_obj, inject_module, arg_help
 
+SSH_CONNECTION_TIMEOUT = int(os.environ.get('STREAMLINE_SSH_CONNECTION_TIMEOUT', 10))
 
 def _silence_urllib_warnings():
     import urllib3
     urllib3.disable_warnings()
 
 def parse_vars(args):
     env_vars = {}
@@ -55,14 +56,15 @@
 
 class BaseAsyncSSHHandler():
     async_handler = True
     connection_options = {
         'known_hosts': None,
         'keepalive_interval': 30,
         'keepalive_count_max': sys.maxsize,
+        'connect_timeout': SSH_CONNECTION_TIMEOUT,
     }
 
     def __init__(self, **options):
         inject_module('asyncssh', globals())
         if not hasattr(asyncssh.connection, '_DEFAULT_KEEPALIVE_INTERVAL'):
             print('asyncssh>1.16 required')
             sys.exit(10)
```

### Comparing `streamline-1.1.0/streamline/extractor.py` & `streamline-1.1.1/streamline/extractor.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline/generators.py` & `streamline-1.1.1/streamline/generators.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline/streamers.py` & `streamline-1.1.1/streamline/streamers.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline/utils.py` & `streamline-1.1.1/streamline/utils.py`

 * *Files identical despite different names*

### Comparing `streamline-1.1.0/streamline.egg-info/PKG-INFO` & `streamline-1.1.1/streamline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamline
-Version: 1.1.0
+Version: 1.1.1
 Summary: CLI tool for doing async tasks and transformations
 Home-page: https://github.com/jdotpy/streamline
 Author: KJ
 Author-email: jdotpy@users.noreply.github.com
 License: UNKNOWN
 Download-URL: https://github.com/jdotpy/streamline/tarball/master
 Keywords: tools
```

