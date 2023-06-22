# Comparing `tmp/sarufi-0.1.5-py3-none-any.whl.zip` & `tmp/sarufi-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 13228 bytes, number of entries: 6
--rw-rw-r--  2.0 unx    32473 b- defN 23-Jun-22 15:59 sarufi/__init__.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     6286 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      457 b- defN 23-Jun-22 16:00 sarufi-0.1.5.dist-info/RECORD
-6 files, 50672 bytes uncompressed, 12406 bytes compressed:  75.5%
+Zip file size: 13205 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx    32457 b- defN 23-Jun-22 16:10 sarufi/__init__.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     6286 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      457 b- defN 23-Jun-22 16:11 sarufi-0.1.6.dist-info/RECORD
+6 files, 50656 bytes uncompressed, 12383 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: sarufi/__init__.py
 Comment: 
 
-Filename: sarufi-0.1.5.dist-info/LICENSE
+Filename: sarufi-0.1.6.dist-info/LICENSE
 Comment: 
 
-Filename: sarufi-0.1.5.dist-info/METADATA
+Filename: sarufi-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: sarufi-0.1.5.dist-info/WHEEL
+Filename: sarufi-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: sarufi-0.1.5.dist-info/top_level.txt
+Filename: sarufi-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: sarufi-0.1.5.dist-info/RECORD
+Filename: sarufi-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sarufi/__init__.py

```diff
@@ -16,29 +16,28 @@
 from typing import Dict, Any, List, Union, Optional
 from yaml import safe_load
 import requests
 
 # Create logger instance
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
+logger_formatter = logging.Formatter(
+    "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
+)
+logger_handler = logging.StreamHandler()
+logger_handler.setFormatter(logger_formatter)
+logger.addHandler(logger_handler)
 
-# Set up logging handler for lazy reloading
-handler = WatchedFileHandler("sarufi.log")
-handler.setFormatter(logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s"))
-logger.addHandler(handler)
 
 class Sarufi(object):
     """Sarufi Class"""
 
     _BASE_URL: str = "https://developers.sarufi.io/"
 
-    def __init__(
-        self,
-        api_key:str 
-    ) -> None:
+    def __init__(self, api_key: str) -> None:
         """Initialize the Sarufi class with API Key
 
 
         Args:
             api_key (str): API Key for the Sarufi account
 
         Examples:
@@ -65,15 +64,14 @@
     @staticmethod
     def __strip_of_nones(data: Dict[str, str]):
         if isinstance(data, dict):
             return {k: v for k, v in data.items() if v is not None}
         error_message = f"{data} should be dict not {type(data)}"
         logging.error(error_message)
 
-
     @staticmethod
     def _read_file(_file: Union[Path, str]) -> Dict[Any, Any]:
         """_read_file
             Reads a file and returns the contents as a dict
         Args:
             _file (Union[Path, str]): File to read(path or filename) | (intents, flows)
 
@@ -85,30 +83,30 @@
         """
         # Get full path of file
         _file = os.path.realpath(_file)
         if os.path.exists(_file):
             try:
                 if any([_file.endswith(ext) for ext in [".yaml", ".yml"]]):
                     logger.info(f"Reading {_file} as YAML")
-                    return safe_load(open(_file, encoding='utf-8'))
+                    return safe_load(open(_file, encoding="utf-8"))
                 elif _file.endswith(".json"):
                     logger.info(f"Reading {_file} as JSON")
-                    return json.load(open(_file, encoding='utf-8'))
+                    return json.load(open(_file, encoding="utf-8"))
                 else:
                     raise FileNotFoundError(f"{_file} is not a valid file")
             except Exception as error:
                 logging.error(error)
                 logging.error("Could not read file")
                 return None
         raise FileNotFoundError(f"File {_file} not found")
 
     @property
     def headers(self):
         """headers
-            Creates a header with the Bearer token using the token property
+        Creates a header with the Bearer token using the token property
         """
         return {
             "Authorization": "Bearer " + self.token,
             "Content-Type": "application/json",
         }
 
     def _get_req(
@@ -202,15 +200,15 @@
             _headers (Dict[str, str], optional): Request headers. Defaults to None.
 
         Returns:
             Union[type[Bot], Dict[Any, Any]]: Bot object if request is successful otherwise dict with error message
         """
 
         _headers = _headers or self.headers
-        response = requests.delete(url, headers=_headers,timeout=120)
+        response = requests.delete(url, headers=_headers, timeout=120)
         if response.status_code == 200:
             return response
         elif response.status_code == 400:
             logger.debug(response.json())
         return response
 
     def create_bot(
```

## Comparing `sarufi-0.1.5.dist-info/LICENSE` & `sarufi-0.1.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sarufi-0.1.5.dist-info/METADATA` & `sarufi-0.1.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sarufi
-Version: 0.1.5
+Version: 0.1.6
 Summary: Opensource python wrapper to Sarufi Conversation API
 Home-page: https://github.com/Neurotech-HQ/sarufi-python-sdk
 Author: Jordan Kalebu
 Author-email: isaackeinstein@gmail.com
 License: MIT
 Download-URL: https://github.com/Neurotech-HQ/sarufi-python-sdk/archive/refs/tags/v0.0.2.tar.gz
 Keywords: sarufi,Sarufi Python SDK,Conversation API python,Swahili Conversational API,Conversational platform Python
```

