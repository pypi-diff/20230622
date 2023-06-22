# Comparing `tmp/psychicapi-0.7.6.tar.gz` & `tmp/psychicapi-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/psychicapi-0.7.6.tar", last modified: Sat Jun 17 23:04:05 2023, max compression
+gzip compressed data, was "dist/psychicapi-0.7.7.tar", last modified: Thu Jun 22 20:51:02 2023, max compression
```

## Comparing `psychicapi-0.7.6.tar` & `psychicapi-0.7.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 23:04:05.000000 psychicapi-0.7.6/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-17 23:04:05.000000 psychicapi-0.7.6/PKG-INFO
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.7.6/psychicapi/__init__.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     7272 2023-06-17 22:29:02.000000 psychicapi-0.7.6/psychicapi/psychic.py
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3726 2023-06-17 23:03:51.000000 psychicapi-0.7.6/README.md
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-17 23:03:36.000000 psychicapi-0.7.6/setup.py
-drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/PKG-INFO
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/SOURCES.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/requires.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/top_level.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-17 23:04:05.000000 psychicapi-0.7.6/psychicapi.egg-info/dependency_links.txt
--rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-17 23:04:05.000000 psychicapi-0.7.6/setup.cfg
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 20:51:02.000000 psychicapi-0.7.7/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 20:51:02.000000 psychicapi-0.7.7/PKG-INFO
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 20:51:02.000000 psychicapi-0.7.7/psychicapi/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       65 2023-06-12 16:34:35.000000 psychicapi-0.7.7/psychicapi/__init__.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     7679 2023-06-22 20:48:22.000000 psychicapi-0.7.7/psychicapi/psychic.py
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     3726 2023-06-17 23:03:51.000000 psychicapi-0.7.7/README.md
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      648 2023-06-22 20:50:39.000000 psychicapi-0.7.7/setup.py
+drwxr-xr-x   0 ayanbandyopadhyay   (501) staff       (20)        0 2023-06-22 20:51:02.000000 psychicapi-0.7.7/psychicapi.egg-info/
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)     4819 2023-06-22 20:51:02.000000 psychicapi-0.7.7/psychicapi.egg-info/PKG-INFO
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)      232 2023-06-22 20:51:02.000000 psychicapi-0.7.7/psychicapi.egg-info/SOURCES.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        9 2023-06-22 20:51:02.000000 psychicapi-0.7.7/psychicapi.egg-info/requires.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       11 2023-06-22 20:51:02.000000 psychicapi-0.7.7/psychicapi.egg-info/top_level.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)        1 2023-06-22 20:51:02.000000 psychicapi-0.7.7/psychicapi.egg-info/dependency_links.txt
+-rw-r--r--   0 ayanbandyopadhyay   (501) staff       (20)       38 2023-06-22 20:51:02.000000 psychicapi-0.7.7/setup.cfg
```

### Comparing `psychicapi-0.7.6/PKG-INFO` & `psychicapi-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.6
+Version: 0.7.7
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
```

### Comparing `psychicapi-0.7.6/psychicapi/psychic.py` & `psychicapi-0.7.7/psychicapi/psychic.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,20 @@
     max_chunk_size: Optional[int] = None
 
 class Psychic:
     def __init__(self, secret_key: str):
         self.api_url = "https://api.psychic.dev/"
         self.secret_key = secret_key
 
+    def handle_http_error(self, response: requests.Response):
+        if response.status_code == 401:
+            raise Exception("Unauthorized: Invalid or missing secret key")
+        data = response.json()
+        raise Exception(f"HTTP error {response.status_code}: {data.get('message', 'No additional information')}")
+
     def get_documents(self, 
                       *, 
                       account_id: str, 
                       connector_id: Optional[ConnectorId] = None, 
                       section_filter_id: Optional[str] = None, 
                       uris: Optional[List[str]] = None, 
                       chunked: Optional[bool] = False, 
@@ -106,15 +112,15 @@
         )
         if response.status_code == 200:
             data = response.json()
             documents = data["documents"]
             next_page_cursor = data["next_page_cursor"]
             return GetDocumentsResponse(documents=documents, next_page_cursor=next_page_cursor)
         else:
-            return None
+            self.handle_http_error(response)
         
     def get_connections(self, *, connector_id: Optional[ConnectorId] = None, account_id: Optional[str] = None):
         filter = {
             "connector_id": connector_id.value if connector_id is not None else None,
             "account_id": account_id
         }
 
@@ -140,15 +146,15 @@
                         sections = [Section(**section) for section in section_filter["sections"]]
                         id = section_filter["id"]
                         typed_section_filters.append(SectionFilter(id=id, sections=sections))
                     connection["section_filters"] = typed_section_filters
 
             return [Connection(**connection) for connection in connections]
         else:
-            return None
+            self.handle_http_error(response)
         
     def add_section_filter(self, *, connector_id: ConnectorId, account_id: str, section_filter: SectionFilter):
         body = {
             "connector_id": connector_id.value,
             "account_id": account_id,
             "section_filter": {
                 "id": section_filter.id,
@@ -171,15 +177,15 @@
             }
         )
         if response.status_code == 200:
             filter = response.json()["section_filter"]
             filter = SectionFilter(id=filter["id"], sections=[Section(**section) for section in filter["sections"]])
             return filter
         else:
-            return None
+            self.handle_http_error(response)
 
         
     def get_conversations(self, *, account_id: str, connector_id: ConnectorId, oldest_timestamp: Optional[int] = None):
         body = {
             "connector_id": connector_id.value,
             "account_id": account_id,
         }
@@ -194,8 +200,8 @@
                 'Accept': 'application/json'
             }
         )
         if response.status_code == 200:
             messages = response.json()["messages"]
             return messages
         else:
-            return None
+            self.handle_http_error(response)
```

### Comparing `psychicapi-0.7.6/README.md` & `psychicapi-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `psychicapi-0.7.6/setup.py` & `psychicapi-0.7.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md')) as f:
     long_description = f.read()
 
 setup(
     name='psychicapi',
-    version='0.7.6',
+    version='0.7.7',
     description='Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ayan Bandyopadhyay',
     author_email='ayan@psychic.dev',
     packages=['psychicapi'],
     install_requires=[
```

### Comparing `psychicapi-0.7.6/psychicapi.egg-info/PKG-INFO` & `psychicapi-0.7.7/psychicapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychicapi
-Version: 0.7.6
+Version: 0.7.7
 Summary: Psychic.dev is an open-source data integration platform for LLMs. This is the Python client for Psychic
 Home-page: UNKNOWN
 Author: Ayan Bandyopadhyay
 Author-email: ayan@psychic.dev
 License: UNKNOWN
 Description: # Psychic
```

