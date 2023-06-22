# Comparing `tmp/flask_pydantic_api-0.9.5-py3-none-any.whl.zip` & `tmp/flask_pydantic_api-0.9.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12862 bytes, number of entries: 12
+Zip file size: 12899 bytes, number of entries: 12
 -rw-r--r--  2.0 unx       98 b- defN 23-Apr-06 01:39 flask_pydantic_api/__init__.py
--rw-r--r--  2.0 unx     7145 b- defN 23-May-21 00:54 flask_pydantic_api/api_wrapper.py
+-rw-r--r--  2.0 unx     7285 b- defN 23-Jun-22 05:00 flask_pydantic_api/api_wrapper.py
 -rw-r--r--  2.0 unx      819 b- defN 23-Mar-18 20:39 flask_pydantic_api/apidocs_views.py
--rw-r--r--  2.0 unx     7733 b- defN 23-May-17 21:59 flask_pydantic_api/openapi.py
+-rw-r--r--  2.0 unx     7733 b- defN 23-Jun-22 06:26 flask_pydantic_api/openapi.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Mar-19 03:04 flask_pydantic_api/py.typed
--rw-r--r--  2.0 unx     2342 b- defN 23-Apr-06 02:14 flask_pydantic_api/utils.py
+-rw-r--r--  2.0 unx     2342 b- defN 23-May-30 22:54 flask_pydantic_api/utils.py
 -rw-r--r--  2.0 unx      447 b- defN 23-Mar-18 20:21 flask_pydantic_api/templates/rapidoc.html
--rw-r--r--  2.0 unx     1073 b- defN 23-May-30 22:37 flask_pydantic_api-0.9.5.dist-info/LICENSE
--rw-r--r--  2.0 unx    12093 b- defN 23-May-30 22:37 flask_pydantic_api-0.9.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-30 22:37 flask_pydantic_api-0.9.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-30 22:37 flask_pydantic_api-0.9.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1056 b- defN 23-May-30 22:37 flask_pydantic_api-0.9.5.dist-info/RECORD
-12 files, 32917 bytes uncompressed, 11056 bytes compressed:  66.4%
+-rw-r--r--  2.0 unx     1073 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12093 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1056 b- defN 23-Jun-22 06:30 flask_pydantic_api-0.9.6.dist-info/RECORD
+12 files, 33057 bytes uncompressed, 11093 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: flask_pydantic_api/utils.py
 Comment: 
 
 Filename: flask_pydantic_api/templates/rapidoc.html
 Comment: 
 
-Filename: flask_pydantic_api-0.9.5.dist-info/LICENSE
+Filename: flask_pydantic_api-0.9.6.dist-info/LICENSE
 Comment: 
 
-Filename: flask_pydantic_api-0.9.5.dist-info/METADATA
+Filename: flask_pydantic_api-0.9.6.dist-info/METADATA
 Comment: 
 
-Filename: flask_pydantic_api-0.9.5.dist-info/WHEEL
+Filename: flask_pydantic_api-0.9.6.dist-info/WHEEL
 Comment: 
 
-Filename: flask_pydantic_api-0.9.5.dist-info/top_level.txt
+Filename: flask_pydantic_api-0.9.6.dist-info/top_level.txt
 Comment: 
 
-Filename: flask_pydantic_api-0.9.5.dist-info/RECORD
+Filename: flask_pydantic_api-0.9.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## flask_pydantic_api/api_wrapper.py

```diff
@@ -156,19 +156,22 @@
                     result = view_func(*args, **kwargs)
 
                 if response_models and isinstance(result, dict):
                     result = response_models[0](**result)
 
                 if isinstance(result, BaseModel):
                     if render_fieldset_model:
-                        result_data = async_to_sync(render_fieldset_model)(
-                            model=result,
-                            fieldsets=fieldsets,
-                            maximum_expansion_depth=maximum_expansion_depth,
-                            raise_error_on_expansion_not_found=False,
+                        loop = asyncio.get_event_loop()
+                        result_data = loop.run_until_complete(
+                            render_fieldset_model(
+                                model=result,
+                                fieldsets=fieldsets,
+                                maximum_expansion_depth=maximum_expansion_depth,
+                                raise_error_on_expansion_not_found=False,
+                            )
                         )
                     else:
                         result_data = result.dict()
 
                     result = make_response(result_data, success_status_code)
 
             except ValidationError as e:
```

## Comparing `flask_pydantic_api-0.9.5.dist-info/LICENSE` & `flask_pydantic_api-0.9.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `flask_pydantic_api-0.9.5.dist-info/METADATA` & `flask_pydantic_api-0.9.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-pydantic-api
-Version: 0.9.5
+Version: 0.9.6
 Summary: Pydantic based API support for Flask
 Home-page: https://github.com/adamsussman/flask-pydantic-api
 Author: Adam Sussman
 Author-email: adam.sussman@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic
```

## Comparing `flask_pydantic_api-0.9.5.dist-info/RECORD` & `flask_pydantic_api-0.9.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 flask_pydantic_api/__init__.py,sha256=KICwgGx_FRhKuNBAcoy1GHBo9C4Jn0QUEwChlmdGS18,98
-flask_pydantic_api/api_wrapper.py,sha256=-d1ie9YKIQwQZfsmRcAXHN2p5dumkgr2XjHOXz2ISEg,7145
+flask_pydantic_api/api_wrapper.py,sha256=Iy61agmROlazyFcrUo4WacVGM1zativTF8GdoMwACq4,7285
 flask_pydantic_api/apidocs_views.py,sha256=sSsr1zVE35UtVPHH0on6HRoZO1vYO1xXRMETq4Fcp1U,819
 flask_pydantic_api/openapi.py,sha256=7kTBYCDQ10F-wwggoiZQtTKEs3vEXudXkZOeDMxamO8,7733
 flask_pydantic_api/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 flask_pydantic_api/utils.py,sha256=mQ-33XUZ_VOHjSgxv2hCyAIIeOCZnCeemRsyDW6D-ng,2342
 flask_pydantic_api/templates/rapidoc.html,sha256=VLYAdPmRJ7dVQmpLmykMUA8KsVEF77tP-Xo2mbBHbBw,447
-flask_pydantic_api-0.9.5.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
-flask_pydantic_api-0.9.5.dist-info/METADATA,sha256=wHaBoxa8GTRKtqNapYFzKQUEvPOLkFBf9S7vTh6-1Fc,12093
-flask_pydantic_api-0.9.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-flask_pydantic_api-0.9.5.dist-info/top_level.txt,sha256=lFmuWAb1KRWKxzT1wPHWpS8eUwnDY1WPWAzqkUDVlU4,19
-flask_pydantic_api-0.9.5.dist-info/RECORD,,
+flask_pydantic_api-0.9.6.dist-info/LICENSE,sha256=INaSDKc7Y-fYndT1E_X93xe_8Ez3nkemMNtk3TaFH9c,1073
+flask_pydantic_api-0.9.6.dist-info/METADATA,sha256=jHoW-THbI8uWqNooikzE-Ph9fsURfBiACFinHOd_wxM,12093
+flask_pydantic_api-0.9.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+flask_pydantic_api-0.9.6.dist-info/top_level.txt,sha256=lFmuWAb1KRWKxzT1wPHWpS8eUwnDY1WPWAzqkUDVlU4,19
+flask_pydantic_api-0.9.6.dist-info/RECORD,,
```

