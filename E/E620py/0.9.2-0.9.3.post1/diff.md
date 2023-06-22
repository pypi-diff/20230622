# Comparing `tmp/E620py-0.9.2.tar.gz` & `tmp/E620py-0.9.3.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E620py-0.9.2.tar", last modified: Wed Jun 21 17:54:52 2023, max compression
+gzip compressed data, was "E620py-0.9.3.post1.tar", last modified: Thu Jun 22 17:21:18 2023, max compression
```

## Comparing `E620py-0.9.2.tar` & `E620py-0.9.3.post1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-21 17:54:42.000000 E620py-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 17:54:52.263161 E620py-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-21 17:54:42.000000 E620py-0.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-21 17:54:42.000000 E620py-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 17:54:52.263161 E620py-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/src/E620py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-21 17:54:52.000000 E620py-0.9.2/src/E620py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:54:52.263161 E620py-0.9.2/src/e620py/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-06-21 17:54:42.000000 E620py-0.9.2/src/e620py/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:21:18.615897 E620py-0.9.3.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-22 17:21:18.615897 E620py-0.9.3.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 17:21:18.615897 E620py-0.9.3.post1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:21:18.611897 E620py-0.9.3.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:21:18.615897 E620py-0.9.3.post1/src/E620py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-22 17:21:18.000000 E620py-0.9.3.post1/src/E620py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-22 17:21:18.000000 E620py-0.9.3.post1/src/E620py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:21:18.000000 E620py-0.9.3.post1/src/E620py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 17:21:18.000000 E620py-0.9.3.post1/src/E620py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 17:21:18.000000 E620py-0.9.3.post1/src/E620py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:21:18.615897 E620py-0.9.3.post1/src/e620py/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19899 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-06-22 17:21:06.000000 E620py-0.9.3.post1/src/e620py/objects.py
```

### Comparing `E620py-0.9.2/LICENSE` & `E620py-0.9.3.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `E620py-0.9.2/PKG-INFO` & `E620py-0.9.3.post1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 0.9.2
+Version: 0.9.3.post1
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `E620py-0.9.2/README.md` & `E620py-0.9.3.post1/README.md`

 * *Files identical despite different names*

### Comparing `E620py-0.9.2/pyproject.toml` & `E620py-0.9.3.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `E620py-0.9.2/src/E620py.egg-info/PKG-INFO` & `E620py-0.9.3.post1/src/E620py.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 0.9.2
+Version: 0.9.3.post1
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `E620py-0.9.2/src/e620py/api.py` & `E620py-0.9.3.post1/src/e620py/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Contains classes and methods that directly interact with the e621 api (post fetching, up-voting, etc)
 """
 
 from . import objects as ob
 from . import exceptions, file_handling
-from .logging import main_log
+from . import main_log
 from .networking import ConnectionHandler
 
 default_session = ConnectionHandler()
 
 
 class E6Get:
     def __init__(self, session=default_session):
@@ -119,15 +119,15 @@
 
                 for post in loop_post_list:
                     if len(post_list) >= fetch_count:
                         break
 
                     post_list.append(post)
 
-            self.e6get_log.info(f"Loop done! Fetched {len(post_list)} posts")
+            self.e6get_log.info(f"Fetched {len(post_list)} posts")
             return post_list
 
         def fetch_loop_all(initial_fetch):
 
             post_list = initial_fetch
 
             while True:
@@ -141,15 +141,15 @@
                     get_options = override_get_options
 
                 try:
                     loop_post_list = self.__single_page_post_get(
                         tags, page_size, get_options, override_endpoint
                     )
                 except exceptions.NoResults:
-                    self.e6get_log.info(f"Loop done! Fetched {len(post_list)} posts")
+                    self.e6get_log.info(f"Fetched {len(post_list)} posts")
                     return post_list
 
                 for post in loop_post_list:
                     post_list.append(post)
 
         page_size = 320
         request = self.__single_page_post_get(
```

### Comparing `E620py-0.9.2/src/e620py/downloader.py` & `E620py-0.9.3.post1/src/e620py/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import httpx
 import os
 import logging
 import json
 from . import objects as ob
 from . import exceptions
-from .logging import main_log
+from . import main_log
 
 
 class Downloader:
     def __init__(self, download_path=None, metadata_path=None, keep_metadata=False, make_folders=True, check_for_updated_posts=False):
         self.download_log = main_log.getChild('downloader')
         self.init_path = os.getcwd()
         self.keep_metadata = keep_metadata
```

### Comparing `E620py-0.9.2/src/e620py/exceptions.py` & `E620py-0.9.3.post1/src/e620py/exceptions.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.2/src/e620py/file_handling.py` & `E620py-0.9.3.post1/src/e620py/file_handling.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #? i may need a module like this later on so im making the file now just in case
 
 import os
 import json
 import hashlib
 from . import exceptions as exceptions
 from . import objects as ob
-from .logging import main_log
+from . import main_log
 
 
 def calculate_md5(file):
     #* this is supposed to be used as a helper function for upload_post, 
     #* but as uploading direct files are not working, this is not needed
     
     md5 = hashlib.md5()
```

### Comparing `E620py-0.9.2/src/e620py/networking.py` & `E620py-0.9.3.post1/src/e620py/networking.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Handles the actual requests being made and checking the responses for errors
 """
 
 import httpx
 import json
 from . import objects as ob
 from . import __user_agent__, base_url, exceptions
-from .logging import main_log
+from . import main_log
 
 
 class ConnectionHandler:
     """
     Handles connecting to e621 and verifying if a request was actually successful or not and handling authentication
     """
     #? i may want to merge most of the networking functions into one as most of it is the same with slight modifications
```

### Comparing `E620py-0.9.2/src/e620py/objects.py` & `E620py-0.9.3.post1/src/e620py/objects.py`

 * *Files identical despite different names*

