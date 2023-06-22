# Comparing `tmp/iterable_etl-0.1.3.tar.gz` & `tmp/iterable_etl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.1.3.tar", last modified: Wed Jun 21 21:57:23 2023, max compression
+gzip compressed data, was "iterable_etl-0.2.0.tar", last modified: Thu Jun 22 19:09:55 2023, max compression
```

## Comparing `iterable_etl-0.1.3.tar` & `iterable_etl-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 21:57:23.367015 iterable_etl-0.1.3/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      307 2023-06-09 16:43:58.000000 iterable_etl-0.1.3/MANIFEST.in
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 21:57:23.367015 iterable_etl-0.1.3/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1519 2023-06-21 16:51:38.000000 iterable_etl-0.1.3/README_PUBLIC.md
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 21:57:23.363015 iterable_etl-0.1.3/iterable_etl/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       22 2023-06-21 21:57:04.000000 iterable_etl-0.1.3/iterable_etl/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      155 2023-06-21 16:51:38.000000 iterable_etl-0.1.3/iterable_etl/__main__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1006 2023-06-21 21:57:04.000000 iterable_etl-0.1.3/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 21:57:23.363015 iterable_etl-0.1.3/iterable_etl/libs/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.3/iterable_etl/libs/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      667 2023-06-21 21:57:04.000000 iterable_etl-0.1.3/iterable_etl/libs/cnst.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1629 2023-06-21 16:51:38.000000 iterable_etl-0.1.3/iterable_etl/libs/dbg.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1086 2023-06-21 17:16:40.000000 iterable_etl-0.1.3/iterable_etl/libs/network.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1403 2023-06-21 21:57:04.000000 iterable_etl-0.1.3/iterable_etl/libs/spark.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      928 2023-06-21 16:51:38.000000 iterable_etl-0.1.3/iterable_etl/libs/transform.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 21:57:23.363015 iterable_etl-0.1.3/iterable_etl/tables/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.3/iterable_etl/tables/__init__.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      843 2023-06-21 17:33:07.000000 iterable_etl-0.1.3/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1370 2023-06-21 16:51:38.000000 iterable_etl-0.1.3/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1723 2023-06-21 16:51:38.000000 iterable_etl-0.1.3/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      769 2023-06-21 16:51:38.000000 iterable_etl-0.1.3/iterable_etl/tables/list.py
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2230 2023-06-21 21:57:04.000000 iterable_etl-0.1.3/iterable_etl/tables/list_user_history.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 21:57:23.363015 iterable_etl-0.1.3/iterable_etl.egg-info/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-21 21:57:23.000000 iterable_etl-0.1.3/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      717 2023-06-21 21:57:23.000000 iterable_etl-0.1.3/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-21 21:57:23.000000 iterable_etl-0.1.3/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       75 2023-06-21 21:57:23.000000 iterable_etl-0.1.3/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       13 2023-06-21 21:57:23.000000 iterable_etl-0.1.3/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      426 2023-06-21 21:57:23.367015 iterable_etl-0.1.3/setup.cfg
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1050 2023-06-21 21:57:04.000000 iterable_etl-0.1.3/setup.py
-drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-21 21:57:23.363015 iterable_etl-0.1.3/tests/
--rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.1.3/tests/__init__.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      307 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/MANIFEST.in
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1519 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/README_PUBLIC.md
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       22 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      155 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/__main__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1006 2023-06-21 21:57:04.000000 iterable_etl-0.2.0/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl/libs/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      667 2023-06-21 21:57:04.000000 iterable_etl-0.2.0/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1900 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1047 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/libs/network.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1403 2023-06-21 21:57:04.000000 iterable_etl-0.2.0/iterable_etl/libs/spark.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      928 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/libs/transform.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl/tables/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      843 2023-06-21 17:33:07.000000 iterable_etl-0.2.0/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1370 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1723 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      769 2023-06-21 16:51:38.000000 iterable_etl-0.2.0/iterable_etl/tables/list.py
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2279 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/iterable_etl/tables/list_user_history.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/iterable_etl.egg-info/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     2027 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      717 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        1 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       75 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)       13 2023-06-22 19:09:55.000000 iterable_etl-0.2.0/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)      426 2023-06-22 19:09:55.189529 iterable_etl-0.2.0/setup.cfg
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)     1050 2023-06-22 19:08:51.000000 iterable_etl-0.2.0/setup.py
+drwxrwxr-x   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-22 19:09:55.185529 iterable_etl-0.2.0/tests/
+-rw-rw-r--   0 andrewmoss  (1000) andrewmoss  (1000)        0 2023-06-09 16:43:58.000000 iterable_etl-0.2.0/tests/__init__.py
```

### Comparing `iterable_etl-0.1.3/PKG-INFO` & `iterable_etl-0.2.0/iterable_etl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iterable_etl
-Version: 0.1.3
+Name: iterable-etl
+Version: 0.2.0
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.1.3/README_PUBLIC.md` & `iterable_etl-0.2.0/README_PUBLIC.md`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/iterable_etl.py` & `iterable_etl-0.2.0/iterable_etl/iterable_etl.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/libs/cnst.py` & `iterable_etl-0.2.0/iterable_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/libs/dbg.py` & `iterable_etl-0.2.0/iterable_etl/libs/dbg.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 
 def dbg(__message: str, *args: Any, **kwargs: Any) -> None:
     """dbg"""
     if os.environ.get("APP_ENV") == "development":
         logger.debug(__message, *args, **kwargs)
 
 
+def error_handler_decorator(func: Callable[..., T]) -> Callable[..., T]:
+    def wrapper(*args: Any, **kwargs: Any):
+        try:
+            return func(*args, **kwargs)
+        except Exception as e:
+            dbg(f"An exception occurred: {e}")
+
+    return wrapper
+
+
 def print_dataframe_head(func: Callable[..., T]) -> Callable[..., T]:
     def wrapper(*args: Any, **kwargs: Any) -> T:
         result = func(*args, **kwargs)
         if os.environ.get("APP_ENV") == "development":
             if isinstance(result, pd.DataFrame):
                 dbg(func.__name__)
                 dbg(result.head(10))
```

### Comparing `iterable_etl-0.1.3/iterable_etl/libs/network.py` & `iterable_etl-0.2.0/iterable_etl/libs/network.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 
 import requests
 from requests import Response
 
 from iterable_etl.libs.dbg import dbg
 
 
-def remove_query_params(url):
-    """shorten url for printing"""
-    parsed_url = urlparse(url)
-    new_url = parsed_url._replace(query=None)
-    cleaned_url = urlunparse(new_url)
-    return cleaned_url
+def trim_string(string: str):
+    if len(string) > 150:
+        trimmed_string = string[:150].strip() + "..."
+        return trimmed_string
+    else:
+        return string
 
 
 def get_data(api_url: str, headers: Dict[str, str]) -> Response:
     """Make a GET request to the Iterable API and return the data."""
-    dbg_url = remove_query_params(api_url)
+    dbg_url = trim_string(api_url)
     dbg("Making request to {api_url}", api_url=dbg_url)
     response = requests.get(api_url, headers=headers, timeout=60)
     dbg("{api_url} response code {code}", api_url=dbg_url, code=response.status_code)
     response.raise_for_status()
     return response
```

### Comparing `iterable_etl-0.1.3/iterable_etl/libs/spark.py` & `iterable_etl-0.2.0/iterable_etl/libs/spark.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/libs/transform.py` & `iterable_etl-0.2.0/iterable_etl/libs/transform.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.2.0/iterable_etl/tables/campaign_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.2.0/iterable_etl/tables/campaign_list_history.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/tables/campaign_metrics.py` & `iterable_etl-0.2.0/iterable_etl/tables/campaign_metrics.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/tables/list.py` & `iterable_etl-0.2.0/iterable_etl/tables/list.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/iterable_etl/tables/list_user_history.py` & `iterable_etl-0.2.0/iterable_etl/tables/list_user_history.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,22 @@
 import time
 from typing import Any, Dict, List
 
 import pandas as pd
 from pandas import DataFrame as PandasDF
 
 from iterable_etl.libs.cnst import get_headers, urls
-from iterable_etl.libs.dbg import dbg, print_dataframe_head, write_dataframe_to_csv
+from iterable_etl.libs.dbg import (
+    dbg,
+    error_handler_decorator,
+    print_dataframe_head,
+    write_dataframe_to_csv,
+)
 from iterable_etl.libs.network import get_data_json, get_data_text
-from iterable_etl.libs.transform import clean_column_headers, csv_to_dataframe
+from iterable_etl.libs.transform import csv_to_dataframe
 
 
 def get_list_ids(api_url: str, headers: Dict[str, str]) -> List[Any]:
     """Make a GET request to the Iterable API and return a dictionary of list data."""
     data = get_data_json(api_url, headers)
     list_ids = [_list["id"] for _list in data["lists"]]
     list_ids.sort()
@@ -24,14 +29,15 @@
 
 
 # spark: SparkSession, pandas_df: PandasDF, target_schema_table_name: str
 
 
 @write_dataframe_to_csv("list_user_history")
 @print_dataframe_head
+@error_handler_decorator
 def list_user_history_df(
     spark=None, target_schema_table_name=None, diff_writer=None
 ) -> PandasDF:
     """
     list_user_history dataframe
 
     This will take ~12 hours to run. It should be setup as an individual job.
```

### Comparing `iterable_etl-0.1.3/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iterable-etl
-Version: 0.1.3
+Name: iterable_etl
+Version: 0.2.0
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `iterable_etl-0.1.3/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.2.0/iterable_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.1.3/setup.py` & `iterable_etl-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.1.3",
+    version="0.2.0",
     description="Replicate iterable data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
```

