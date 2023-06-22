# Comparing `tmp/reversinglabs-sdk-py3-2.1.2.tar.gz` & `tmp/reversinglabs-sdk-py3-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversinglabs-sdk-py3-2.1.2.tar", last modified: Mon May 15 12:49:20 2023, max compression
+gzip compressed data, was "reversinglabs-sdk-py3-2.2.0.tar", last modified: Thu Jun 22 05:29:44 2023, max compression
```

## Comparing `reversinglabs-sdk-py3-2.1.2.tar` & `reversinglabs-sdk-py3-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.209660 reversinglabs-sdk-py3-2.1.2/
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     5969 2023-05-15 12:14:56.000000 reversinglabs-sdk-py3-2.1.2/CHANGELOG.md
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1056 2023-01-01 19:35:25.000000 reversinglabs-sdk-py3-2.1.2/LICENSE
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       53 2022-10-18 22:24:54.000000 reversinglabs-sdk-py3-2.1.2/MANIFEST.in
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    37303 2023-05-15 12:49:20.210660 reversinglabs-sdk-py3-2.1.2/PKG-INFO
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    36051 2023-05-15 12:44:26.000000 reversinglabs-sdk-py3-2.1.2/README.md
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.207660 reversinglabs-sdk-py3-2.1.2/ReversingLabs/
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.209660 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/__init__.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   110651 2023-05-15 12:44:26.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/a1000.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    19593 2023-02-27 14:28:49.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/clouddeepscan.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     4776 2023-03-30 13:23:32.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/helper.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   171456 2023-04-05 12:27:16.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/ticloud.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    16840 2023-04-05 21:30:12.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/tiscale.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.2/ReversingLabs/__init__.py
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    41623 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.1.2/logo.jpg
-drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-05-15 12:49:20.209660 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    37303 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/PKG-INFO
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)      542 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/dependency_links.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/not-zip-safe
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       34 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/requires.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       14 2023-05-15 12:49:20.000000 reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/top_level.txt
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       74 2023-05-15 12:49:20.210660 reversinglabs-sdk-py3-2.1.2/setup.cfg
--rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1645 2023-05-15 12:00:53.000000 reversinglabs-sdk-py3-2.1.2/setup.py
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-06-22 05:29:44.793698 reversinglabs-sdk-py3-2.2.0/
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     6109 2023-06-22 05:28:33.000000 reversinglabs-sdk-py3-2.2.0/CHANGELOG.md
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1056 2023-01-01 19:35:25.000000 reversinglabs-sdk-py3-2.2.0/LICENSE
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       53 2022-10-18 22:24:54.000000 reversinglabs-sdk-py3-2.2.0/MANIFEST.in
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    37713 2023-06-22 05:29:44.793698 reversinglabs-sdk-py3-2.2.0/PKG-INFO
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    36461 2023-06-22 05:28:33.000000 reversinglabs-sdk-py3-2.2.0/README.md
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-06-22 05:29:44.791698 reversinglabs-sdk-py3-2.2.0/ReversingLabs/
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-06-22 05:29:44.792698 reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/__init__.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   110651 2023-05-15 12:44:26.000000 reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/a1000.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    19593 2023-02-27 14:28:49.000000 reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/clouddeepscan.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     4776 2023-03-30 13:23:32.000000 reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/helper.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)   177294 2023-06-22 05:28:22.000000 reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/ticloud.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    16840 2023-04-05 21:30:12.000000 reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/tiscale.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.2.0/ReversingLabs/__init__.py
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    41623 2022-06-24 11:40:25.000000 reversinglabs-sdk-py3-2.2.0/logo.jpg
+drwxr-xr-x   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        0 2023-06-22 05:29:44.793698 reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)    37713 2023-06-22 05:29:44.000000 reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/PKG-INFO
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)      542 2023-06-22 05:29:44.000000 reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-06-22 05:29:44.000000 reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)        1 2023-06-22 05:29:44.000000 reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/not-zip-safe
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       34 2023-06-22 05:29:44.000000 reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/requires.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       14 2023-06-22 05:29:44.000000 reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/top_level.txt
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)       74 2023-06-22 05:29:44.793698 reversinglabs-sdk-py3-2.2.0/setup.cfg
+-rw-r--r--   0 msever@reversinglabs.lan (1816802225) domain users@reversinglabs.lan (1816800513)     1645 2023-06-22 05:23:19.000000 reversinglabs-sdk-py3-2.2.0/setup.py
```

### Comparing `reversinglabs-sdk-py3-2.1.2/CHANGELOG.md` & `reversinglabs-sdk-py3-2.2.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,12 +113,24 @@
 - **a1000** module:
   - Added paging parameters to the Network Threat Intelligence methods: `network_ip_to_domain`, `network_urls_from_ip` and `network_files_from_ip`
   - Added auto paging versions of the same methods: `network_ip_to_domain_aggregated`, `network_urls_from_ip_aggregated` and `network_files_from_ip_aggregated`
 
 ---
 
 
+
+v2.2.0 (2023-06-23)
+-------------------
+
+#### Improvements
+
+- **ticloud** module:
+  - Added the `NewMalwarePlatformFiltered` class.
+
+---
+
+
 ### Scheduled removals
 - **June 2023.**:
   - `a1000.A1000.get_results`, `a1000.A1000.upload_sample_and_get_results`, `a1000.A1000.get_classification`, `a1000.A1000.reanalyze_samples`, `a1000.A1000.get_extracted_files`, `a1000.A1000.advanced_search`, `a1000.A1000.advanced_search_aggregated`
 - **September 2023.**:
   - `ticloud.ReanalyzeFile.ranalyze_samples`
```

### Comparing `reversinglabs-sdk-py3-2.1.2/LICENSE` & `reversinglabs-sdk-py3-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.2/PKG-INFO` & `reversinglabs-sdk-py3-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python SDK for using ReversingLabs services - Python 3 version.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -619,14 +619,26 @@
 - `set_start_time`
   - Sets the starting point for the DataChangeSubscription.pull_from_feed method.
 - `pull_from_feed`
   - Returns a recordset with samples to which the user is subscribed. The starting point for this action is set using the DataChangeSubscription.set_start_time method. If the starting point is not set, this method will return records starting with the current timestamp. Every subsequent request will continue from the timestamp where the previous request ended.
 - `continuous_data_change_feed`
   - Returns a recordset with samples to which the user is subscribed from the timestamp stated in the request onwards. To fetch the next recordset, use the last_timestamp value from the response and submit it in a new request as the time_value parameter.
 
+#### Class:
+```python
+class NewMalwarePlatformFiltered(TiCloudAPI)
+````
+#### Methods:
+- `feed_query`
+    - Returns a list of malware samples optionally filtered by platform since the requested timestamp.
+- `start_query`
+    - Sets the starting timestamp for the pull_query.
+- `pull_query`
+    - Returns the list of malware samples optionally filtered by platform since a point in time set by the start_query.
+
 
 ***
 
 ## Module: tiscale
 A Python module representing the ReversingLabs TitaniumScale malware analysis appliance.
 #### Class:
 ```python
```

### Comparing `reversinglabs-sdk-py3-2.1.2/README.md` & `reversinglabs-sdk-py3-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -591,14 +591,26 @@
 - `set_start_time`
   - Sets the starting point for the DataChangeSubscription.pull_from_feed method.
 - `pull_from_feed`
   - Returns a recordset with samples to which the user is subscribed. The starting point for this action is set using the DataChangeSubscription.set_start_time method. If the starting point is not set, this method will return records starting with the current timestamp. Every subsequent request will continue from the timestamp where the previous request ended.
 - `continuous_data_change_feed`
   - Returns a recordset with samples to which the user is subscribed from the timestamp stated in the request onwards. To fetch the next recordset, use the last_timestamp value from the response and submit it in a new request as the time_value parameter.
 
+#### Class:
+```python
+class NewMalwarePlatformFiltered(TiCloudAPI)
+````
+#### Methods:
+- `feed_query`
+    - Returns a list of malware samples optionally filtered by platform since the requested timestamp.
+- `start_query`
+    - Sets the starting timestamp for the pull_query.
+- `pull_query`
+    - Returns the list of malware samples optionally filtered by platform since a point in time set by the start_query.
+
 
 ***
 
 ## Module: tiscale
 A Python module representing the ReversingLabs TitaniumScale malware analysis appliance.
 #### Class:
 ```python
```

### Comparing `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/a1000.py` & `reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/clouddeepscan.py` & `reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/clouddeepscan.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/helper.py` & `reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/ticloud.py` & `reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/ticloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -4101,14 +4101,150 @@
         response = self._get_request(url=url)
 
         self._raise_on_error(response)
 
         return response
 
 
+class NewMalwarePlatformFiltered(TiCloudAPI):
+    """TCF-0102-0106"""
+
+    __FEED_ENDPOINT = "/api/feed/malware/detection/platform/v1/query/{time_format}/{time_value}"
+    __START_ENDPOINT = "/api/feed/malware/detection/platform/v1/query/start/{time_format}/{time_value}"
+    __PULL_ENDPOINT = "/api/feed/malware/detection/platform/v1/query/pull"
+
+    def __init__(self, host, username, password, verify=True, proxies=None, user_agent=DEFAULT_USER_AGENT,
+                 allow_none_return=False):
+        super(NewMalwarePlatformFiltered, self).__init__(host, username, password, verify, proxies,
+                                                         user_agent=user_agent, allow_none_return=allow_none_return)
+
+        self._url = "{host}{{endpoint}}".format(host=self._host)
+
+    def feed_query(self, time_format, time_value, platforms=None, sample_available=False, limit=1000):
+        """Returns a list of malware samples optionally filtered by platform since the requested
+        timestamp.
+            :param time_format: possible values: 'utc' or 'timestamp'
+            :type time_format: str
+            :param time_value: results will be retrieved from the specified time up until the current moment;
+            accepted formats are Unix timestamp string and 'YYYY-MM-DDThh:mm:ss'
+            :type time_value: str
+            :param platforms: filter the samples by their detected platform value; check the API documentation for
+            allowed values; the platforms should be passed as list of strings
+            :type platforms: list[str] or None
+            :param sample_available: return only samples available for download
+            :type sample_available: bool
+            :param limit: number of records to return in the response
+            :type limit: int
+            :return: response
+            :rtype: requests.Response
+        """
+        if time_format not in ("utc", "timestamp"):
+            raise WrongInputError("time_format parameter must be one of the following values: 'utc', 'timestamp'")
+
+        if not isinstance(time_value, str):
+            raise WrongInputError("time_value parameter must be string.")
+
+        if not isinstance(sample_available, bool):
+            raise WrongInputError("sample_available parameter must be boolean.")
+
+        if not isinstance(limit, int):
+            raise WrongInputError("limit parameter must be integer.")
+
+        base = self.__FEED_ENDPOINT.format(
+            time_format=time_format,
+            time_value=time_value
+        )
+
+        query_params = "?sample_available={sample_available}&limit={limit}&format=json".format(
+            sample_available=str(sample_available).lower(),
+            limit=limit
+        )
+
+        if platforms:
+            for platform in platforms:
+                query_params = query_params + "&platform={platform}".format(platform=platform)
+
+        endpoint = "{base}{query_params}".format(base=base, query_params=query_params)
+
+        url = self._url.format(endpoint=endpoint)
+
+        response = self._get_request(url=url)
+
+        self._raise_on_error(response)
+
+        return response
+
+    def start_query(self, time_format, time_value):
+        """Sets the starting timestamp for the pull_query.
+            :param time_format: possible values: 'utc' or 'timestamp'
+            :type time_format: str
+            :param time_value: results will be retrieved from the specified time up until the current moment;
+            accepted formats are Unix timestamp string and 'YYYY-MM-DDThh:mm:ss'
+            :type time_value: str
+            :return: response
+            :rtype: requests.Response
+        """
+        if time_format not in ("utc", "timestamp"):
+            raise WrongInputError("time_format parameter must be one of the following values: 'utc', 'timestamp'")
+
+        if not isinstance(time_value, str):
+            raise WrongInputError("time_value parameter must be string.")
+
+        endpoint = self.__START_ENDPOINT.format(
+            time_format=time_format,
+            time_value=time_value
+        )
+
+        url = self._url.format(endpoint=endpoint)
+
+        response = self._put_request(url=url)
+
+        self._raise_on_error(response)
+
+        return response
+
+    def pull_query(self, platforms=None, sample_available=False, limit=1000):
+        """Returns the list of malware samples optionally filtered by platform
+        since a point in time set by the start_query.
+            :param platforms: filter the samples by their detected platform value; check the API documentation for
+            allowed values; the platforms should be passed as list of strings
+            :type platforms: list[str] or None
+            :param sample_available: return only samples available for download
+            :type sample_available: bool
+            :param limit: number of records to return in the response
+            :type limit: int
+            :return: response
+            :rtype: requests.Response
+        """
+        if not isinstance(sample_available, bool):
+            raise WrongInputError("sample_available parameter must be boolean.")
+
+        if not isinstance(limit, int):
+            raise WrongInputError("limit parameter must be integer.")
+
+        query_params = "?sample_available={sample_available}&limit={limit}&format=json".format(
+            sample_available=str(sample_available).lower(),
+            limit=limit
+        )
+
+        if platforms:
+            for platform in platforms:
+                query_params = query_params + "&platform={platform}".format(platform=platform)
+
+        endpoint = "{base}{query_params}".format(base=self.__PULL_ENDPOINT, query_params=query_params)
+
+        url = self._url.format(endpoint=endpoint)
+
+        response = self._get_request(url=url)
+
+        self._raise_on_error(response)
+
+        return response
+
+
 def _update_hash_object(input_source, hash_object):
     """Accepts a string or an opened file in 'rb' mode and a created hashlib hash object and
     returns an updated hashlib hash object.
         :param input_source: open file in "rb" mode or string
         :type input_source: str or file or BinaryIO
         :param hash_object: hash object
         :type hash_object: _hashlib._HASH
```

### Comparing `reversinglabs-sdk-py3-2.1.2/ReversingLabs/SDK/tiscale.py` & `reversinglabs-sdk-py3-2.2.0/ReversingLabs/SDK/tiscale.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.2/logo.jpg` & `reversinglabs-sdk-py3-2.2.0/logo.jpg`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/PKG-INFO` & `reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.1.2
+Version: 2.2.0
 Summary: Python SDK for using ReversingLabs services - Python 3 version.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -619,14 +619,26 @@
 - `set_start_time`
   - Sets the starting point for the DataChangeSubscription.pull_from_feed method.
 - `pull_from_feed`
   - Returns a recordset with samples to which the user is subscribed. The starting point for this action is set using the DataChangeSubscription.set_start_time method. If the starting point is not set, this method will return records starting with the current timestamp. Every subsequent request will continue from the timestamp where the previous request ended.
 - `continuous_data_change_feed`
   - Returns a recordset with samples to which the user is subscribed from the timestamp stated in the request onwards. To fetch the next recordset, use the last_timestamp value from the response and submit it in a new request as the time_value parameter.
 
+#### Class:
+```python
+class NewMalwarePlatformFiltered(TiCloudAPI)
+````
+#### Methods:
+- `feed_query`
+    - Returns a list of malware samples optionally filtered by platform since the requested timestamp.
+- `start_query`
+    - Sets the starting timestamp for the pull_query.
+- `pull_query`
+    - Returns the list of malware samples optionally filtered by platform since a point in time set by the start_query.
+
 
 ***
 
 ## Module: tiscale
 A Python module representing the ReversingLabs TitaniumScale malware analysis appliance.
 #### Class:
 ```python
```

### Comparing `reversinglabs-sdk-py3-2.1.2/reversinglabs_sdk_py3.egg-info/SOURCES.txt` & `reversinglabs-sdk-py3-2.2.0/reversinglabs_sdk_py3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.1.2/setup.py` & `reversinglabs-sdk-py3-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             "ReversingLabs.SDK"]
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="reversinglabs-sdk-py3",
-    version="2.1.2",
+    version="2.2.0",
     description="Python SDK for using ReversingLabs services - Python 3 version.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ReversingLabs",
     author_email="support@reversinglabs.com",
     url="https://github.com/reversinglabs/reversinglabs-sdk-py3",
     packages=packages,
```

