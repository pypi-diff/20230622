# Comparing `tmp/robotframework_openapi_libcore-1.9.0.tar.gz` & `tmp/robotframework_openapi_libcore-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework_openapi_libcore-1.9.0.tar", max compression
+gzip compressed data, was "robotframework_openapi_libcore-1.9.1.tar", max compression
```

## Comparing `robotframework_openapi_libcore-1.9.0.tar` & `robotframework_openapi_libcore-1.9.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     4748 2023-06-09 13:40:52.874546 robotframework_openapi_libcore-1.9.0/docs/README.md
--rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.9.0/LICENSE
--rw-r--r--   0        0        0     2374 2023-06-09 13:15:10.704523 robotframework_openapi_libcore-1.9.0/pyproject.toml
--rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/__init__.py
--rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_base.py
--rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_utils.py
--rw-r--r--   0        0        0      163 2023-04-20 07:55:08.986947 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/oas_cache.py
--rw-r--r--   0        0        0    28654 2023-06-09 13:40:52.807168 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.libspec
--rw-r--r--   0        0        0    60706 2023-06-09 13:40:49.228395 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.py
--rw-r--r--   0        0        0    14791 2023-06-01 13:47:32.926184 robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/value_utils.py
--rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.9.0/setup.py
--rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4748 2023-06-22 08:04:12.949122 robotframework_openapi_libcore-1.9.1/docs/README.md
+-rw-r--r--   0        0        0    11558 2021-12-13 14:33:13.481598 robotframework_openapi_libcore-1.9.1/LICENSE
+-rw-r--r--   0        0        0     2374 2023-06-22 07:37:34.833744 robotframework_openapi_libcore-1.9.1/pyproject.toml
+-rw-r--r--   0        0        0     1297 2021-12-28 14:18:06.991167 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/__init__.py
+-rw-r--r--   0        0        0     8014 2023-02-17 14:58:53.541795 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/dto_base.py
+-rw-r--r--   0        0        0     2659 2023-02-17 14:58:53.542831 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/dto_utils.py
+-rw-r--r--   0        0        0      163 2023-04-20 07:55:08.986947 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/oas_cache.py
+-rw-r--r--   0        0        0    28654 2023-06-22 08:04:12.825416 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/openapi_libcore.libspec
+-rw-r--r--   0        0        0    60765 2023-06-22 08:04:06.150201 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/openapi_libcore.py
+-rw-r--r--   0        0        0        0 2023-06-12 07:47:27.960875 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/py.typed
+-rw-r--r--   0        0        0    14791 2023-06-01 13:47:32.926184 robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/value_utils.py
+-rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.9.1/setup.py
+-rw-r--r--   0        0        0     5926 1970-01-01 00:00:00.000000 robotframework_openapi_libcore-1.9.1/PKG-INFO
```

### Comparing `robotframework_openapi_libcore-1.9.0/docs/README.md` & `robotframework_openapi_libcore-1.9.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.9.0/LICENSE` & `robotframework_openapi_libcore-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.9.0/pyproject.toml` & `robotframework_openapi_libcore-1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="robotframework-openapi-libcore"
-version = "1.9.0"
+version = "1.9.1"
 description = "A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs."
 license = "Apache-2.0"
 authors = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 maintainers = ["Robin Mackaij <r.a.mackaij@gmail.com>"]
 readme =  "./docs/README.md"
 homepage = "https://github.com/MarketSquare/robotframework-openapi-libcore"
 classifiers = [
```

### Comparing `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/__init__.py` & `robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_base.py` & `robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/dto_base.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/dto_utils.py` & `robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/dto_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/openapi_libcore.libspec`

 * *Files 0% similar despite different names*

#### Comparing `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.libspec` & `robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/openapi_libcore.libspec`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-06-09T13:40:53+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="379">
-  <version>1.9.0</version>
+<keywordspec name="OpenApiLibCore" type="LIBRARY" format="HTML" scope="SUITE" generated="2023-06-22T08:04:13+00:00" specversion="4" source="C:\GitHub\robotframework-openapi-libcore\src\OpenApiLibCore\openapi_libcore.py" lineno="379">
+  <version>1.9.1</version>
   <doc>&lt;p&gt;Main class providing the keywords and core logic to interact with an OpenAPI server.&lt;/p&gt;
 &lt;p&gt;Visit the &lt;a href=&quot;https://github.com/MarketSquare/robotframework-openapi-libcore&quot;&gt;library page&lt;/a&gt; for an introduction.&lt;/p&gt;</doc>
   <tags/>
   <inits>
     <init name="__init__" lineno="387">
       <arguments repr="source: str, origin: str = , base_path: str = , mappings_path: str | Path = , invalid_property_default_response: int = 422, default_id_property_name: str = id, faker_locale: str | List[str] | None = None, recursion_limit: int = 1, recursion_default: Any = {}, username: str = , password: str = , security_token: str = , auth: AuthBase | None = None, cert: str | Tuple[str, str] | None = None, verify_tls: bool | str | None = True, extra_headers: Dict[str, str] | None = None, cookies: Dict[str, str] | RequestsCookieJar | None = None, proxies: Dict[str, str] | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="source: str">
@@ -151,15 +151,15 @@
 &lt;p&gt;A dictionary or &lt;a href=&quot;https://docs.python.org/3/library/http.cookiejar.html#http.cookiejar.CookieJar&quot;&gt;CookieJar object&lt;/a&gt; to send with all requests.&lt;/p&gt;
 &lt;h4&gt;proxies&lt;/h4&gt;
 &lt;p&gt;A dictionary of 'protocol': 'proxy url' to use for all requests.&lt;/p&gt;</doc>
       <shortdoc>== Base parameters ==</shortdoc>
     </init>
   </inits>
   <keywords>
-    <kw name="Authorized Request" lineno="1395">
+    <kw name="Authorized Request" lineno="1397">
       <arguments repr="url: str, method: str, params: Dict[str, Any] | None = None, headers: Dict[str, str] | None = None, json_data: Dict[str, Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | List[Dict[str, ForwardRef('JSON')] | List[ForwardRef('JSON')] | str | int | float | bool | None] | str | int | float | bool | None = None">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -189,39 +189,39 @@
           <default>None</default>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a request using the security token or authentication set in the library.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: provided username / password or auth objects take precedence over token based security&lt;/p&gt;</doc>
       <shortdoc>Perform a request using the security token or authentication set in the library.</shortdoc>
     </kw>
-    <kw name="Ensure In Use" lineno="1299">
+    <kw name="Ensure In Use" lineno="1301">
       <arguments repr="url: str, resource_relation: IdReference">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="resource_relation: IdReference">
           <name>resource_relation</name>
           <type>IdReference</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Ensure that the (right-most) &lt;span class=&quot;name&quot;&gt;id&lt;/span&gt; of the resource referenced by the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; is used by the resource defined by the &lt;span class=&quot;name&quot;&gt;resource_relation&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Ensure that the (right-most) `id` of the resource referenced by the `url` is used by the resource defined by the `resource_relation`.</shortdoc>
     </kw>
-    <kw name="Get Ids From Url" lineno="734">
+    <kw name="Get Ids From Url" lineno="736">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Perform a GET request on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt; and return the list of resource &lt;span class=&quot;name&quot;&gt;ids&lt;/span&gt; from the response.&lt;/p&gt;</doc>
       <shortdoc>Perform a GET request on the `url` and return the list of resource `ids` from the response.</shortdoc>
     </kw>
-    <kw name="Get Invalid Json Data" lineno="1078">
+    <kw name="Get Invalid Json Data" lineno="1080">
       <arguments repr="url: str, method: str, status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -236,40 +236,40 @@
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; on the &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that will cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt; for the &lt;span class=&quot;name&quot;&gt;method&lt;/span&gt; operation on the &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;
 &lt;p&gt;&amp;gt; Note: applicable UniquePropertyValueConstraint and IdReference Relations are considered before changes to &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; are made.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `dto` on the `request_data` that will cause the provided `status_code` for the `method` operation on the `url`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Parameters" lineno="1126">
+    <kw name="Get Invalidated Parameters" lineno="1128">
       <arguments repr="status_code: int, request_data: RequestData">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="status_code: int">
           <name>status_code</name>
           <type typedoc="integer">int</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="request_data: RequestData">
           <name>request_data</name>
           <type>RequestData</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Returns a version of &lt;span class=&quot;name&quot;&gt;params, headers&lt;/span&gt; as present on &lt;span class=&quot;name&quot;&gt;request_data&lt;/span&gt; that has been modified to cause the provided &lt;span class=&quot;name&quot;&gt;status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Returns a version of `params, headers` as present on `request_data` that has been modified to cause the provided `status_code`.</shortdoc>
     </kw>
-    <kw name="Get Invalidated Url" lineno="1044">
+    <kw name="Get Invalidated Url" lineno="1046">
       <arguments repr="valid_url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="valid_url: str">
           <name>valid_url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return an url with all the path parameters in the &lt;span class=&quot;name&quot;&gt;valid_url&lt;/span&gt; replaced by a random UUID.&lt;/p&gt;
 &lt;p&gt;Raises ValueError if the valid_url cannot be invalidated.&lt;/p&gt;</doc>
       <shortdoc>Return an url with all the path parameters in the `valid_url` replaced by a random UUID.</shortdoc>
     </kw>
-    <kw name="Get Json Data For Dto Class" lineno="954">
+    <kw name="Get Json Data For Dto Class" lineno="956">
       <arguments repr="schema: Dict[str, Any], dto_class: Dto | Type[Dto], operation_id: str = ">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="schema: Dict[str, Any]">
           <name>schema</name>
           <type typedoc="dictionary">Dict[str, Any]</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="dto_class: Dto | Type[Dto]">
           <name>dto_class</name>
@@ -281,15 +281,15 @@
           <type typedoc="string">str</type>
           <default/>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Generate a valid (json-compatible) dict for all the &lt;span class=&quot;name&quot;&gt;dto_class&lt;/span&gt; properties.&lt;/p&gt;</doc>
       <shortdoc>Generate a valid (json-compatible) dict for all the `dto_class` properties.</shortdoc>
     </kw>
-    <kw name="Get Json Data With Conflict" lineno="1343">
+    <kw name="Get Json Data With Conflict" lineno="1345">
       <arguments repr="url: str, method: str, dto: Dto, conflict_status_code: int">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
@@ -303,25 +303,25 @@
           <name>conflict_status_code</name>
           <type typedoc="integer">int</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return &lt;span class=&quot;name&quot;&gt;json_data&lt;/span&gt; based on the &lt;span class=&quot;name&quot;&gt;UniquePropertyValueConstraint&lt;/span&gt; that must be returned by the &lt;span class=&quot;name&quot;&gt;get_relations&lt;/span&gt; implementation on the &lt;span class=&quot;name&quot;&gt;dto&lt;/span&gt; for the given &lt;span class=&quot;name&quot;&gt;conflict_status_code&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return `json_data` based on the `UniquePropertyValueConstraint` that must be returned by the `get_relations` implementation on the `dto` for the given `conflict_status_code`.</shortdoc>
     </kw>
-    <kw name="Get Parameterized Endpoint From Url" lineno="1066">
+    <kw name="Get Parameterized Endpoint From Url" lineno="1068">
       <arguments repr="url: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="url: str">
           <name>url</name>
           <type typedoc="string">str</type>
         </arg>
       </arguments>
       <doc>&lt;p&gt;Return the endpoint as found in the &lt;span class=&quot;name&quot;&gt;paths&lt;/span&gt; section based on the given &lt;span class=&quot;name&quot;&gt;url&lt;/span&gt;.&lt;/p&gt;</doc>
       <shortdoc>Return the endpoint as found in the `paths` section based on the given `url`.</shortdoc>
     </kw>
-    <kw name="Get Request Data" lineno="774">
+    <kw name="Get Request Data" lineno="776">
       <arguments repr="endpoint: str, method: str">
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="endpoint: str">
           <name>endpoint</name>
           <type typedoc="string">str</type>
         </arg>
         <arg kind="POSITIONAL_OR_NAMED" required="true" repr="method: str">
           <name>method</name>
```

### Comparing `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/openapi_libcore.py` & `robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/openapi_libcore.py`

 * *Files 1% similar despite different names*

```diff
@@ -630,24 +630,26 @@
             url = f"{self.base_url}{choice(paths)}"
             return url
         endpoint_parts = list(endpoint.split("/"))
         for index, part in enumerate(endpoint_parts):
             if part.startswith("{") and part.endswith("}"):
                 type_endpoint_parts = endpoint_parts[slice(index)]
                 type_endpoint = "/".join(type_endpoint_parts)
-                existing_id: str = run_keyword(
+                existing_id: Union[str, int, float] = run_keyword(
                     "get_valid_id_for_endpoint", type_endpoint, method
                 )
-                endpoint_parts[index] = existing_id
+                endpoint_parts[index] = str(existing_id)
         resolved_endpoint = "/".join(endpoint_parts)
         url = f"{self.base_url}{resolved_endpoint}"
         return url
 
     @keyword
-    def get_valid_id_for_endpoint(self, endpoint: str, method: str) -> str:
+    def get_valid_id_for_endpoint(
+        self, endpoint: str, method: str
+    ) -> Union[str, int, float]:
         """
         Support keyword that returns the `id` for an existing resource at `endpoint`.
 
         To prevent resource conflicts with other test cases, a new resource is created
         (POST) if possible.
         """
         method = method.lower()
```

### Comparing `robotframework_openapi_libcore-1.9.0/src/OpenApiLibCore/value_utils.py` & `robotframework_openapi_libcore-1.9.1/src/OpenApiLibCore/value_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework_openapi_libcore-1.9.0/setup.py` & `robotframework_openapi_libcore-1.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prance[cli]>=0.22,<0.23',
  'requests>=2.27,<3.0',
  'robotframework>=4',
  'rstr>=3,<4']
 
 setup_kwargs = {
     'name': 'robotframework-openapi-libcore',
-    'version': '1.9.0',
+    'version': '1.9.1',
     'description': 'A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.',
     'long_description': '---\n---\n\n# OpenApiLibCore for Robot Framework\n\nThe OpenApiLibCore library is a utility library that is meant to simplify creation\nof other Robot Framework libraries for API testing based on the information in\nan OpenAPI document (also known as Swagger document).\nThis document explains how to use the OpenApiLibCore library.\n\nMy RoboCon 2022 talk about OpenApiDriver and OpenApiLibCore can be found\n[here](https://www.youtube.com/watch?v=7YWZEHxk9Ps)\n\nFor more information about Robot Framework, see http://robotframework.org.\n\n---\n\n> Note: OpenApiLibCore is still being developed so there are currently\nrestrictions / limitations that you may encounter when using this library to run\ntests against an API. See [Limitations](#limitations) for details.\n\n---\n\n## Installation\n\nIf you already have Python >= 3.8 with pip installed, you can simply run:\n\n`pip install --upgrade robotframework-openapi-libcore`\n\n---\n\n## OpenAPI (aka Swagger)\n\nThe OpenAPI Specification (OAS) defines a standard, language-agnostic interface\nto RESTful APIs, see https://swagger.io/specification/\n\nThe OpenApiLibCore implements a number of Robot Framework keywords that make it\neasy to interact with an OpenAPI implementation by using the information in the\nopenapi document (Swagger file), for examply by automatic generation of valid values\nfor requests based on the schema information in the document.\n\n> Note: OpenApiLibCore is designed for APIs based on the OAS v3\nThe library has not been tested for APIs based on the OAS v2.\n\n---\n\n## Getting started\n\nBefore trying to use the keywords exposed by OpenApiLibCore on the target API\nit\'s recommended to first ensure that the openapi document for the API is valid\nunder the OpenAPI Specification.\n\nThis can be done using the command line interface of a package that is installed as\na prerequisite for OpenApiLibCore.\nBoth a local openapi.json or openapi.yaml file or one hosted by the API server\ncan be checked using the `prance validate <reference_to_file>` shell command:\n\n```shell\nprance validate --backend=openapi-spec-validator http://localhost:8000/openapi.json\nProcessing "http://localhost:8000/openapi.json"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n\nprance validate --backend=openapi-spec-validator /tests/files/petstore_openapi.yaml\nProcessing "/tests/files/petstore_openapi.yaml"...\n -> Resolving external references.\nValidates OK as OpenAPI 3.0.2!\n```\n\nYou\'ll have to change the url or file reference to the location of the openapi\ndocument for your API.\n\n> Note: Although recursion is technically allowed under the OAS, tool support is limited\nand changing the OAS to not use recursion is recommended.\nOpenApiLibCore has limited support for parsing OpenAPI documents with\nrecursion in them. See the `recursion_limit` and `recursion_default` parameters.\n\nIf the openapi document passes this validation, the next step is trying to do a test\nrun with a minimal test suite.\nThe example below can be used, with `source`, `origin` and \'endpoint\' altered to\nfit your situation.\n\n``` robotframework\n*** Settings ***\nLibrary            OpenApiLibCore\n...                    source=http://localhost:8000/openapi.json\n...                    origin=http://localhost:8000\n\n*** Test Cases ***\nGetting Started\n    ${url}=    Get Valid Url    endpoint=/employees/{employee_id}   method=get\n\n```\n\nRunning the above suite for the first time may result in an error / failed test.\nYou should look at the Robot Framework `log.html` to determine the reasons\nfor the failing tests.\nDepending on the reasons for the failures, different solutions are possible.\n\nDetails about the OpenApiLibCore library parameters and keywords that you may need can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/openapi_libcore.html).\n\nThe OpenApiLibCore also support handling of relations between resources within the scope\nof the API being validated as well as handling dependencies on resources outside the\nscope of the API. In addition there is support for handling restrictions on the values\nof parameters and properties.\n\nDetails about the `mappings_path` variable usage can be found\n[here](https://marketsquare.github.io/robotframework-openapi-libcore/advanced_use.html).\n\n---\n\n## Limitations\n\nThere are currently a number of limitations to supported API structures, supported\ndata types and properties. The following list details the most important ones:\n- Only JSON request and response bodies are supported.\n- No support for per-endpoint authorization levels.\n- Parsing of OAS 3.1 documents is supported by the parsing tools, but runtime behavior is untested.\n\n',
     'author': 'Robin Mackaij',
     'author_email': 'r.a.mackaij@gmail.com',
     'maintainer': 'Robin Mackaij',
     'maintainer_email': 'r.a.mackaij@gmail.com',
     'url': 'https://github.com/MarketSquare/robotframework-openapi-libcore',
```

### Comparing `robotframework_openapi_libcore-1.9.0/PKG-INFO` & `robotframework_openapi_libcore-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-openapi-libcore
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Robot Framework library to facilitate library development for OpenAPI / Swagger APIs.
 Home-page: https://github.com/MarketSquare/robotframework-openapi-libcore
 License: Apache-2.0
 Author: Robin Mackaij
 Author-email: r.a.mackaij@gmail.com
 Maintainer: Robin Mackaij
 Maintainer-email: r.a.mackaij@gmail.com
```

