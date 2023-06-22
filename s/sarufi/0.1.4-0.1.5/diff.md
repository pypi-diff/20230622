# Comparing `tmp/sarufi-0.1.4-py3-none-any.whl.zip` & `tmp/sarufi-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 13228 bytes, number of entries: 6
--rw-rw-rw-  2.0 unx    32469 b- defN 23-Apr-25 23:46 sarufi/__init__.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/LICENSE
--rw-rw-rw-  2.0 unx     6288 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/METADATA
--rw-rw-rw-  2.0 unx       92 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      457 b- defN 23-Apr-26 00:02 sarufi-0.1.4.dist-info/RECORD
-6 files, 50670 bytes uncompressed, 12406 bytes compressed:  75.5%
+-rw-rw-r--  2.0 unx    32473 b- defN 23-Jun-22 15:59 sarufi/__init__.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6286 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      457 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/RECORD
+6 files, 50672 bytes uncompressed, 12406 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sarufi/__init__.py
 Comment: 
 
-Filename: sarufi-0.1.4.dist-info/LICENSE
+Filename: sarufi-0.1.5.dist-info/LICENSE
 Comment: 
 
-Filename: sarufi-0.1.4.dist-info/METADATA
+Filename: sarufi-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: sarufi-0.1.4.dist-info/WHEEL
+Filename: sarufi-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: sarufi-0.1.4.dist-info/top_level.txt
+Filename: sarufi-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: sarufi-0.1.4.dist-info/RECORD
+Filename: sarufi-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sarufi/__init__.py

```diff
@@ -121,15 +121,15 @@
         Simplifies making get requests
 
         Args:
             url (str): _description_
             _headers (Dict[str, str], optional): Authenticated header with Bearer token. Defaults to None.
         """
 
-        response = requests.get(url, headers=_headers or self.headers, timeout=10)
+        response = requests.get(url, headers=_headers or self.headers, timeout=120)
         if response.status_code == 200:
             return response
         elif response.status_code == 400:
             logger.debug(response.json())
         return response
 
     def _post_req(
@@ -149,15 +149,15 @@
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Bot object if request is successful otherwise dict with error message
         """
 
         _data = json.dumps(self.__strip_of_nones(body))  # remove None values
         _headers = _headers or self.headers
-        response = requests.post(url, data=_data, headers=_headers, timeout=10)
+        response = requests.post(url, data=_data, headers=_headers, timeout=120)
         if response.status_code == 200:
             return response
         elif response.status_code == 400:
             logger.debug(response.json())
         return response
 
     def _put_req(
@@ -177,15 +177,15 @@
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Bot object if request is successful otherwise dict with error message
         """
 
         _data = json.dumps(self.__strip_of_nones(body))
         _headers = _headers or self.headers
-        response = requests.put(url, data=_data, headers=_headers, timeout=10)
+        response = requests.put(url, data=_data, headers=_headers, timeout=120)
         if response.status_code == 200:
             return response
         elif response.status_code == 400:
             logger.debug(response.json())
         return response
 
     def _delete_req(
@@ -202,15 +202,15 @@
             _headers (Dict[str, str], optional): Request headers. Defaults to None.
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Bot object if request is successful otherwise dict with error message
         """
 
         _headers = _headers or self.headers
-        response = requests.delete(url, headers=_headers,timeout=10)
+        response = requests.delete(url, headers=_headers,timeout=120)
         if response.status_code == 200:
             return response
         elif response.status_code == 400:
             logger.debug(response.json())
         return response
 
     def create_bot(
```

## Comparing `sarufi-0.1.4.dist-info/LICENSE` & `sarufi-0.1.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sarufi-0.1.4.dist-info/METADATA` & `sarufi-0.1.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 Metadata-Version: 2.1
 Name: sarufi
-Version: 0.1.4
+Version: 0.1.5
 Summary: Opensource python wrapper to Sarufi Conversation API
 Home-page: https://github.com/Neurotech-HQ/sarufi-python-sdk
-Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Author: Jordan Kalebu
 Author-email: isaackeinstein@gmail.com
 License: MIT
+Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Keywords: sarufi,Sarufi Python SDK,Conversation API python,Swahili Conversational API,Conversational platform Python
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pyyaml
 Requires-Dist: python-telegram-bot
 
 <samp>
 
 # sarufi-python-sdk
@@ -208,7 +208,9 @@
 Are you facing any issue with the usage of the package, please raise one
 
 ## Contributors
 
 1. [kalebu](https://github.com/kalebu/)
 2. [Anthony Mipawa](https://github.com/Tonyloyt)
 </samp>
+
+
```

