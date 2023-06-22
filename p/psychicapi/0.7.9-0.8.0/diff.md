# Comparing `tmp/psychicapi-0.7.9.tar.gz` & `tmp/psychicapi-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psychicapi-0.7.9.tar", last modified: Thu Jun 22 21:05:52 2023, max compression
+gzip compressed data, was "dist/psychicapi-0.8.0.tar", last modified: Thu Jun 22 21:23:36 2023, max compression
```

## Comparing `psychicapi-0.7.9.tar` & `psychicapi-0.8.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:05:52.000000 psychicapi-0.7.9/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 21:05:52.000000 psychicapi-0.7.9/PKG-INFO
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:05:52.000000 psychicapi-0.7.9/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.7.9/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     7709 2023-06-22 21:05:27.000000 psychicapi-0.7.9/psychicapi/psychic.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3726 2023-06-17 23:03:51.000000 psychicapi-0.7.9/README.md
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-22 21:05:34.000000 psychicapi-0.7.9/setup.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:05:52.000000 psychicapi-0.7.9/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 21:05:52.000000 psychicapi-0.7.9/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-22 21:05:52.000000 psychicapi-0.7.9/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-22 21:05:52.000000 psychicapi-0.7.9/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-22 21:05:52.000000 psychicapi-0.7.9/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-22 21:05:52.000000 psychicapi-0.7.9/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-22 21:05:52.000000 psychicapi-0.7.9/setup.cfg
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:23:36.000000 psychicapi-0.8.0/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 21:23:36.000000 psychicapi-0.8.0/PKG-INFO
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.8.0/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     7858 2023-06-22 21:16:22.000000 psychicapi-0.8.0/psychicapi/psychic.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3726 2023-06-17 23:03:51.000000 psychicapi-0.8.0/README.md
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-22 21:22:03.000000 psychicapi-0.8.0/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-22 21:23:36.000000 psychicapi-0.8.0/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-22 21:23:36.000000 psychicapi-0.8.0/setup.cfg
```

### Comparing `psychicapi-0.7.9/PKG-INFO` & `psychicapi-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.9
+Version: 0.8.0
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
```

### Comparing `psychicapi-0.7.9/psychicapi/psychic.py` & `psychicapi-0.8.0/psychicapi/psychic.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,16 +73,20 @@
     def __init__(self, secret_key: str):
         self.api_url = "https://api.psychic.dev/"
         self.secret_key = secret_key
 
     def handle_http_error(self, response: requests.Response):
         if response.status_code == 401 or response.status_code == 403:
             raise Exception("Unauthorized: Invalid or missing secret key")
-        data = response.json()
-        raise Exception(f"HTTP error {response.status_code}: {data.get('detail', 'No additional information')}")
+        try:
+            data = response.json()
+            message = data.get('detail', 'No additional information')
+        except requests.exceptions.JSONDecodeError:
+            message = 'No additional information'
+        raise Exception(f"HTTP error {response.status_code}: {message}")
 
     def get_documents(self, 
                       *, 
                       account_id: str, 
                       connector_id: Optional[ConnectorId] = None, 
                       section_filter_id: Optional[str] = None, 
                       uris: Optional[List[str]] = None,
```

### Comparing `psychicapi-0.7.9/README.md` & `psychicapi-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `psychicapi-0.7.9/setup.py` & `psychicapi-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.7.9',
+    version='0.8.0',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

### Comparing `psychicapi-0.7.9/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.8.0/psychicapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.9
+Version: 0.8.0
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
```

