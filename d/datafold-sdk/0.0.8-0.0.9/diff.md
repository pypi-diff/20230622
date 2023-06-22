# Comparing `tmp/datafold_sdk-0.0.8-py3-none-any.whl.zip` & `tmp/datafold_sdk-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 11350 bytes, number of entries: 18
+Zip file size: 11357 bytes, number of entries: 18
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-02 20:37 datafold_sdk/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 22-Jan-19 20:40 datafold_sdk/version.py
+-rw-r--r--  2.0 unx       22 b- defN 22-Jan-20 12:24 datafold_sdk/version.py
 -rw-r--r--  2.0 unx     1326 b- defN 22-Jan-19 20:28 datafold_sdk/cli/__init__.py
--rw-r--r--  2.0 unx     2120 b- defN 22-Jan-19 20:28 datafold_sdk/cli/alerts.py
+-rw-r--r--  2.0 unx     2120 b- defN 22-Jan-20 12:23 datafold_sdk/cli/alerts.py
 -rw-r--r--  2.0 unx      166 b- defN 21-Nov-02 20:17 datafold_sdk/cli/context.py
 -rw-r--r--  2.0 unx       47 b- defN 21-Nov-02 20:17 datafold_sdk/cli/exceptions.py
 -rw-r--r--  2.0 unx     4152 b- defN 21-Nov-02 20:17 datafold_sdk/cli/dbt/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 21-Nov-02 20:17 datafold_sdk/sdk/__init__.py
 -rw-r--r--  2.0 unx       48 b- defN 21-Nov-02 20:17 datafold_sdk/sdk/exceptions.py
--rw-r--r--  2.0 unx     1809 b- defN 22-Jan-19 20:28 datafold_sdk/sdk/utils.py
+-rw-r--r--  2.0 unx     1841 b- defN 22-Jan-20 12:23 datafold_sdk/sdk/utils.py
 -rw-r--r--  2.0 unx     1845 b- defN 21-Nov-02 20:17 datafold_sdk/sdk/ci/__init__.py
 -rw-r--r--  2.0 unx     6125 b- defN 22-Jan-19 20:28 datafold_sdk/sdk/dbt/__init__.py
--rw-r--r--  2.0 unx     1061 b- defN 22-Jan-19 20:40 datafold_sdk-0.0.8.dist-info/LICENSE
--rw-r--r--  2.0 unx     2091 b- defN 22-Jan-19 20:40 datafold_sdk-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jan-19 20:40 datafold_sdk-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 22-Jan-19 20:40 datafold_sdk-0.0.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 22-Jan-19 20:40 datafold_sdk-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1518 b- defN 22-Jan-19 20:40 datafold_sdk-0.0.8.dist-info/RECORD
-18 files, 22508 bytes uncompressed, 8830 bytes compressed:  60.8%
+-rw-r--r--  2.0 unx     1061 b- defN 22-Jan-20 12:24 datafold_sdk-0.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2091 b- defN 22-Jan-20 12:24 datafold_sdk-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 22-Jan-20 12:24 datafold_sdk-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 22-Jan-20 12:24 datafold_sdk-0.0.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 22-Jan-20 12:24 datafold_sdk-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1518 b- defN 22-Jan-20 12:24 datafold_sdk-0.0.9.dist-info/RECORD
+18 files, 22540 bytes uncompressed, 8837 bytes compressed:  60.8%
```

## zipnote {}

```diff
@@ -30,26 +30,26 @@
 
 Filename: datafold_sdk/sdk/ci/__init__.py
 Comment: 
 
 Filename: datafold_sdk/sdk/dbt/__init__.py
 Comment: 
 
-Filename: datafold_sdk-0.0.8.dist-info/LICENSE
+Filename: datafold_sdk-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: datafold_sdk-0.0.8.dist-info/METADATA
+Filename: datafold_sdk-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: datafold_sdk-0.0.8.dist-info/WHEEL
+Filename: datafold_sdk-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: datafold_sdk-0.0.8.dist-info/entry_points.txt
+Filename: datafold_sdk-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: datafold_sdk-0.0.8.dist-info/top_level.txt
+Filename: datafold_sdk-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: datafold_sdk-0.0.8.dist-info/RECORD
+Filename: datafold_sdk-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datafold_sdk/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
```

## datafold_sdk/cli/alerts.py

```diff
@@ -23,15 +23,15 @@
 @click.pass_context
 def run(ctx: click.Context, query_id: int, wait: Optional[int], interval: int):
     """ Run the query, trigger the alerts. """
     headers = prepare_headers(ctx.obj.api_key)
 
     api_segment = f"api/v1/alerts/{query_id}/checks"
     url = prepare_api_url(ctx.obj.host, api_segment)
-    resp = post_data(url, data={}, headers=headers)
+    resp = post_data(url, json={}, headers=headers)
     data = resp.json()
     result_id = data['id']
     logger.debug(f"API response={data!r}")
 
     started = time.monotonic()
     last_status: Optional[str] = None
     while wait and time.monotonic() < started + wait:
```

## datafold_sdk/sdk/utils.py

```diff
@@ -28,17 +28,17 @@
     except subprocess.CalledProcessError as exception:
         logger.error("The process failed")
         logger.error(exception.stderr)
         logger.error(exception.stdout)
         raise exception
 
 
-def post_data(url, data, headers, files=None):
+def post_data(url, data=None, json=None, headers=None, files=None):
     try:
-        res = requests.post(url, files=files, json=data, headers=headers)
+        res = requests.post(url, files=files, data=data, json=json, headers=headers)
         check_requests_result(res)
         return res
     except requests.exceptions.ConnectionError as exception:
         parsed_uri = urlparse(url)
         logger.error(f"The host {parsed_uri.netloc} could not be reached")
         raise exception
```

## Comparing `datafold_sdk-0.0.8.dist-info/LICENSE` & `datafold_sdk-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `datafold_sdk-0.0.8.dist-info/METADATA` & `datafold_sdk-0.0.9.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datafold-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: The datafold SDK
 Home-page: https://pypi.org/project/datafold-sdk
 Author: Datafold
 Author-email: hello@datafold.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `datafold_sdk-0.0.8.dist-info/RECORD` & `datafold_sdk-0.0.9.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 datafold_sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-datafold_sdk/version.py,sha256=wOJN3HxAgnSon5vWYU3Txm2UZ_7tBHDKXUKZIH-mXX8,22
+datafold_sdk/version.py,sha256=46Yjk3fz9o8aTN8E95McnzpJcjGzVJmHmQqUZ5mXzfc,22
 datafold_sdk/cli/__init__.py,sha256=4ojuRK8chnW1jUv1QzcDeBo50J4ZethpGNzC29tZsqk,1326
-datafold_sdk/cli/alerts.py,sha256=nmffsvLZvXWGur6ugU0g6Fn-oyjQhLVO_WTTQyCUli0,2120
+datafold_sdk/cli/alerts.py,sha256=SCD1CQGvji5LyYZ5RNHrajnH8TrtbZzvM3zgtbQbgcw,2120
 datafold_sdk/cli/context.py,sha256=Qyyd215w-4NfhIXbbmFOeguxlSzqp5y3uNPH2GRk4Do,166
 datafold_sdk/cli/exceptions.py,sha256=rkSGCedWYfmYew_sIDSTXfQ47-HFChfhlPVIRNDGgMw,47
 datafold_sdk/cli/dbt/__init__.py,sha256=obvOqazH8K3TUucHAPBM4g74SazzRwsCG8AoeUZsHNo,4152
 datafold_sdk/sdk/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 datafold_sdk/sdk/exceptions.py,sha256=-8ag2TRJO0F5iMBK_numgyYw8Att6rsiHgUM_J-zfx0,48
-datafold_sdk/sdk/utils.py,sha256=4NwgYDHp8DhEBZPtCU1NRw8vWqnL6RpZ2bH028iDspk,1809
+datafold_sdk/sdk/utils.py,sha256=rv71RQ5qa8L2iEPVYqqBng6RIcqIU_EqL3ayEOqLtmY,1841
 datafold_sdk/sdk/ci/__init__.py,sha256=nLs2mKAZbDvBT-FZ1qdhgOOcH4hFbXiWMXvMmjIR7k8,1845
 datafold_sdk/sdk/dbt/__init__.py,sha256=qyzH2KjqVR8hCsy4U_fAMDy6Jq-3WCwMVXoxrgXNYoY,6125
-datafold_sdk-0.0.8.dist-info/LICENSE,sha256=iHzgYnei-dnBU7MZvlWDsrVRoxAyNRNjpN4Qenk8FhY,1061
-datafold_sdk-0.0.8.dist-info/METADATA,sha256=0WjlfGfv27qGGzku1FEl3VU-O1N3vFKH2UYZ0MEP4G8,2091
-datafold_sdk-0.0.8.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-datafold_sdk-0.0.8.dist-info/entry_points.txt,sha256=aTqKYM2a6XEqH_KDzzxwugevQH7exM5whQgP7TI59jk,73
-datafold_sdk-0.0.8.dist-info/top_level.txt,sha256=Y5EO_5iRh3lsg3EEOm1LC3D3wjojY-OFlmu_tSyEqDo,13
-datafold_sdk-0.0.8.dist-info/RECORD,,
+datafold_sdk-0.0.9.dist-info/LICENSE,sha256=iHzgYnei-dnBU7MZvlWDsrVRoxAyNRNjpN4Qenk8FhY,1061
+datafold_sdk-0.0.9.dist-info/METADATA,sha256=yzh8gpKvJG7ZXS15pPQHvg6vqQhdvNw4bqmEk3kDpMA,2091
+datafold_sdk-0.0.9.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+datafold_sdk-0.0.9.dist-info/entry_points.txt,sha256=aTqKYM2a6XEqH_KDzzxwugevQH7exM5whQgP7TI59jk,73
+datafold_sdk-0.0.9.dist-info/top_level.txt,sha256=Y5EO_5iRh3lsg3EEOm1LC3D3wjojY-OFlmu_tSyEqDo,13
+datafold_sdk-0.0.9.dist-info/RECORD,,
```

