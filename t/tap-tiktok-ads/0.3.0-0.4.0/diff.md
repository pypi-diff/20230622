# Comparing `tmp/tap-tiktok-ads-0.3.0.tar.gz` & `tmp/tap-tiktok-ads-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap-tiktok-ads-0.3.0.tar", last modified: Fri Jun  9 07:47:42 2023, max compression
+gzip compressed data, was "tap-tiktok-ads-0.4.0.tar", last modified: Thu Jun 22 08:31:04 2023, max compression
```

## Comparing `tap-tiktok-ads-0.3.0.tar` & `tap-tiktok-ads-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/LICENSE
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7970 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/README.md
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/setup.cfg
--rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.121490 tap-tiktok-ads-0.3.0/tap_tiktok_ads/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1798 2023-05-24 06:51:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7638 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/discover.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_country.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10070 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/adgroups.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3802 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ads.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2095 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/advertisers.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/campaigns.json
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1009 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16979 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/streams.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1630 2023-05-26 18:02:58.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads/sync.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.121490 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      965 2023-06-09 07:47:42.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/entry_points.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-06-09 07:47:41.000000 tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/top_level.txt
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-09 07:47:42.125490 tap-tiktok-ads-0.3.0/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4633 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_all_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2269 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_automatic_fields.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8049 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_bookmarks.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6083 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_discovery.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9068 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/tests/test_interrupted_sync.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.3.0/tests/test_pagination.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7075 2023-06-09 06:51:29.000000 tap-tiktok-ads-0.3.0/tests/test_start_date.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32387 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       54 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7970 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/setup.cfg
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)      790 2023-06-22 08:24:58.000000 tap-tiktok-ads-0.4.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.397244 tap-tiktok-ads-0.4.0/tap_tiktok_ads/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1798 2023-05-24 06:51:41.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7638 2023-06-21 21:32:34.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/discover.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3153 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3082 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_country.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3078 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10070 2023-06-21 21:32:34.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/adgroups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3802 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2095 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/advertisers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1531 2023-06-21 21:32:34.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1009 2022-09-02 08:09:40.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17030 2023-06-22 08:24:58.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1630 2023-05-26 18:02:58.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads/sync.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.397244 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      263 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      965 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       55 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       15 2023-06-22 08:31:04.000000 tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 08:31:04.401244 tap-tiktok-ads-0.4.0/tests/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4633 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_all_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2269 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_automatic_fields.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8049 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_bookmarks.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6083 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_discovery.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9068 2023-06-20 05:59:29.000000 tap-tiktok-ads-0.4.0/tests/test_interrupted_sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3174 2023-05-16 05:53:52.000000 tap-tiktok-ads-0.4.0/tests/test_pagination.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6996 2023-06-22 08:24:58.000000 tap-tiktok-ads-0.4.0/tests/test_start_date.py
```

### Comparing `tap-tiktok-ads-0.3.0/LICENSE` & `tap-tiktok-ads-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/README.md` & `tap-tiktok-ads-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/setup.py` & `tap-tiktok-ads-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="tap-tiktok-ads",
-    version="0.3.0",
+    version="0.4.0",
     description="Singer.io tap for extracting data",
     author="Stitch",
     url="http://singer.io",
     classifiers=["Programming Language :: Python :: 3 :: Only"],
     py_modules=["tap_tiktok_ads"],
     install_requires=[
         "singer-python==5.13.0",
```

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/__init__.py` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/client.py` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/client.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/discover.py` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/discover.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_age_and_gender.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_country.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_country.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ad_insights_by_platform.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/adgroups.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/adgroups.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/ads.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/advertisers.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/advertisers.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas/campaigns.json` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/schemas.py` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/schemas.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/streams.py` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,27 +185,27 @@
             transformed_records.append(record)
         else:
             if bookmark_value is not None and record['create_time'] > parse(bookmark_value):
                 transformed_records.append(record)
     return transformed_records
 
 
-def get_bookmark_value(stream_name, bookmark_data, advertiser_id):
+def get_bookmark_value(stream_name, bookmark_data, advertiser_id, start_date):
     '''
     Returns bookmark value for any stream based on stream category(normal or stream with advertiser_id). Return None in 
     case of `advertisers` stream if bookmark is not present. For other streams return bookmark for each advertiser_id
     '''
     if stream_name in ENDPOINT_ADVERTISERS:
         if bookmark_data:
             return bookmark_data
-        return None
+        return start_date
     elif (stream_name in ENDPOINT_INSIGHTS or stream_name in ENDPOINT_AD_MANAGEMENT) and advertiser_id in bookmark_data:
         return bookmark_data[advertiser_id]
     else:
-        return None
+        return start_date
 
 
 class Stream():
 
     tap_stream_id = None
     key_properties = None
     replication_keys = None
@@ -264,15 +264,15 @@
 
     def process_batch(self, stream, records, advertiser_id):
         """
             Process records for the stream by transforming it to the desired format, writing it to output, and bookmark writing
         """
         bookmark_column = self.replication_keys[0] # pylint: disable=unsubscriptable-object
         bookmark_data = self.get_bookmark(stream.tap_stream_id)
-        bookmark_value = get_bookmark_value(stream.tap_stream_id, bookmark_data, advertiser_id)
+        bookmark_value = get_bookmark_value(stream.tap_stream_id, bookmark_data, advertiser_id, self.config['start_date'])
         transformed_records = pre_transform(stream.tap_stream_id, records, bookmark_value)
         sorted_records = sorted(transformed_records, key=lambda x: x[bookmark_column])
         for record in sorted_records:
             with Transformer(integer_datetime_fmt=UNIX_MILLISECONDS_INTEGER_DATETIME_PARSING) as transformer:
                 # for 'insights' stream, 'advertiser_id' is not getting populated and it is one for the Primary Keys
                 record['advertiser_id'] = advertiser_id
                 transformed_record = transformer.transform(record, stream.schema.to_dict(),
```

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads/sync.py` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads/sync.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tap_tiktok_ads.egg-info/SOURCES.txt` & `tap-tiktok-ads-0.4.0/tap_tiktok_ads.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tests/test_all_fields.py` & `tap-tiktok-ads-0.4.0/tests/test_all_fields.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tests/test_automatic_fields.py` & `tap-tiktok-ads-0.4.0/tests/test_automatic_fields.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tests/test_bookmarks.py` & `tap-tiktok-ads-0.4.0/tests/test_bookmarks.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tests/test_discovery.py` & `tap-tiktok-ads-0.4.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tests/test_interrupted_sync.py` & `tap-tiktok-ads-0.4.0/tests/test_interrupted_sync.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tests/test_pagination.py` & `tap-tiktok-ads-0.4.0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `tap-tiktok-ads-0.3.0/tests/test_start_date.py` & `tap-tiktok-ads-0.4.0/tests/test_start_date.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
             - Verify minimum bookmark sent to the target for incremental streams >= start date for both syncs.
             - Verify by primary key values, that all records in the 2nd sync are included in the 1st sync since 2nd sync has a later start date.
         - FULL TABLE
             - Verify that the 2nd sync includes the same number of records as the 1st sync.
             - Verify by primary key values, that the 2nd sync and 1st sync replicated the same records.
         """
 
-        self.first_start_date = "2020-12-01T00:00:00Z"
-        self.second_start_date = "2020-12-20T00:00:00Z"
+        self.first_start_date = "2022-04-18T00:00:00Z"
+        self.second_start_date = "2022-04-21T00:00:00Z"
         start_date_1_epoch = self.dt_to_ts(self.first_start_date)
         start_date_2_epoch = self.dt_to_ts(self.second_start_date)
 
         ##########################################################################
         ### Update Start Date for 1st sync
         ##########################################################################
 
@@ -105,18 +105,17 @@
                         self.assertGreaterEqual(self.dt_to_ts(start_date_key_value_parsed), start_date_1_epoch)
 
                     # Verify bookmark key values are greater than or equal to start date of sync 2
                     for start_date_key_value in start_date_key_sync_2:
                         start_date_key_value_parsed = parse(start_date_key_value).strftime("%Y-%m-%dT%H:%M:%SZ")
                         self.assertGreaterEqual(self.dt_to_ts(start_date_key_value_parsed), start_date_2_epoch)
 
-                    # ticket - https://jira.talendforge.org/browse/TDL-23225
                     # Verify the number of records replicated in sync 1 is greater than the number
                     # of records replicated in sync 2 for stream
-                    # self.assertGreater(record_count_sync_1, record_count_sync_2)
+                    self.assertGreater(record_count_sync_1, record_count_sync_2)
 
                     # Verify the records replicated in sync 2 were also replicated in sync 1
                     self.assertTrue(primary_keys_sync_2.issubset(primary_keys_sync_1))
 
                 else:
                     # Verify that the 2nd sync with a later start date replicates the same number of
                     # records as the 1st sync.
```

