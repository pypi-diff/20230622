# Comparing `tmp/tabulario-0.3.1.tar.gz` & `tmp/tabulario-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabulario-0.3.1.tar", max compression
+gzip compressed data, was "tabulario-0.3.2.tar", max compression
```

## Comparing `tabulario-0.3.1.tar` & `tabulario-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11358 2023-06-13 07:58:34.858905 tabulario-0.3.1/LICENSE
--rw-r--r--   0        0        0     5831 2023-06-13 07:58:34.858905 tabulario-0.3.1/README.md
--rw-r--r--   0        0        0     2487 2023-06-13 07:58:51.099009 tabulario-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      785 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/__init__.py
--rw-r--r--   0        0        0     3716 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/cli.py
--rw-r--r--   0        0        0      871 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/exceptions.py
--rw-r--r--   0        0        0     5045 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/oauth.py
--rw-r--r--   0        0        0     1004 2023-06-13 07:58:34.858905 tabulario-0.3.1/tab/util.py
--rw-r--r--   0        0        0        0 2023-06-13 07:58:34.858905 tabulario-0.3.1/tabular/__init__.py
--rw-r--r--   0        0        0     4955 2023-06-13 07:58:34.858905 tabulario-0.3.1/tabular/loader.py
--rw-r--r--   0        0        0     6642 1970-01-01 00:00:00.000000 tabulario-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-22 18:14:34.670083 tabulario-0.3.2/LICENSE
+-rw-r--r--   0        0        0     6701 2023-06-22 18:14:34.670083 tabulario-0.3.2/README.md
+-rw-r--r--   0        0        0     2487 2023-06-22 18:14:45.582204 tabulario-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      785 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/__init__.py
+-rw-r--r--   0        0        0     4146 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/cli.py
+-rw-r--r--   0        0        0      871 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/exceptions.py
+-rw-r--r--   0        0        0     5024 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/oauth.py
+-rw-r--r--   0        0        0     1004 2023-06-22 18:14:34.670083 tabulario-0.3.2/tab/util.py
+-rw-r--r--   0        0        0      836 2023-06-22 18:14:34.670083 tabulario-0.3.2/tabular/__init__.py
+-rw-r--r--   0        0        0     4955 2023-06-22 18:14:34.670083 tabulario-0.3.2/tabular/loader.py
+-rw-r--r--   0        0        0     2016 2023-06-22 18:14:34.670083 tabulario-0.3.2/tabular/tabular.py
+-rw-r--r--   0        0        0     7512 1970-01-01 00:00:00.000000 tabulario-0.3.2/PKG-INFO
```

### Comparing `tabulario-0.3.1/LICENSE` & `tabulario-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.1/README.md` & `tabulario-0.3.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -84,7 +84,49 @@
     "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzUxMiJ9.eyJjcmVkc0tleSI6InQtR2RDWkdqNU9wb1EiLCJzdWJJZCI6ImViMzc2NTQ4LTIwNmItNDBiYS1hN2E1LWVkYmUzZjg4YWVlZCIsInN1YiI6ImZva2tvQHRhYnVsYXIuaW8iLCJ3YXJlaG91c2VJZCI6IjhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZSIsImlzcyI6InRhYnVsYXIuaW8iLCJsb2NhdGlvbiI6InMzOi8vdGFidWxhci13aC11cy13ZXN0LTItZGV2LzhiY2IwODM4LTUwZmMtNDcyZC05ZGRiLThmZWI4OWVmNWYxZS8iLCJ0eXBlIjoiV0FSRUhPVVNFIiwicmVnaW9uIjoidXMtd2VzdC0yIiwiZXhwIjoxNjY1NzU1NDM5LCJpYXQiOjE2NjU2NjkwMzksImp0aSI6IjZhNzljNzU1LTYzNGEtNDJlNC04YmVlLTEzZjgxOWFlYTYyNCIsIm9yZ0lkIjoiMWM1MmU4MzItMjY2Yy00OTYxLTk3YWYtMTE1ZDFiNzJmY2UwIn0.DBmmCfyj4hNaP0eVwzyv6R5aoSLrwWwHbHKePs2lEphA8zzilVreN1BPligIjezLPsn57S8FiOHqsCAwkeNWPthxxCI_gBkeZuCDhqbP90GsIuKwsFIaECZjn2_sO7UAhT3oSLgSeSB289QsQck6qIPPLLXM95jKrfzClKIF3Me4lKPmsRdLNRwCEDAOIgiR9sjBEUbSxgSkRvwxPQNDu75T25pn8O18EMlhmOUROSYva8VPRCc9PIFJL0PfcD_D7wlKZfiug8v58-q-1RAfB57IF0p-o9G_5RNeDrbEDA35OM8jTZEFDpL8Q-WlzT_6EZTvsIx_b7HxNW6kxf6WsQ",
     "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
     "token_type": "Bearer",
     "expires_in": 86400,
     "scope": null
 }
 ```
+
+### Listing all the warehouses
+
+```bash
+➜ tab warehouses --help
+Usage: tab warehouses [OPTIONS]
+
+Fetches all the warehouses
+
+Options:
+-c, --credential TEXT
+-t, --token TEXT
+--help                 Show this message and exit.
+```
+
+Example:
+
+```bash
+➜ tab warehouses --credential t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI | jq
+[
+  {
+    "id": "6efbcaf4-21ae-499d-b340-3bc1a7003f52",
+    "name": "sandbox",
+    "region": "us-east-1"
+  },
+  {
+    "id": "c70f668c-4746-414f-8a74-b1e4f1f0de60",
+    "name": "Fokko",
+    "region": "us-west-2"
+  }
+]
+```
+
+```python
+>> from tabular import Tabular
+>>> t = Tabular("t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI")
+>>> t.list_warehouses()
+[
+    Warehouse(id='6efbcaf4-21ae-499d-b340-3bc1a7003f52', name='sandbox', region='us-east-1'),
+    Warehouse(id='c70f668c-4746-414f-8a74-b1e4f1f0de60', name='Fokko', region='us-west-2')
+]
+```
```

### Comparing `tabulario-0.3.1/pyproject.toml` & `tabulario-0.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 [tool.poetry]
 name = "tabulario"
-version = "0.3.1"
+version = "0.3.2"
 readme = "README.md"
 homepage = "https://tabular.io/"
 repository = "https://github.com/tabular-io/"
 description = "Utility library for Tabular.io"
 authors = ["Tabular Technologies, Inc. <fokko@tabular.io>"]
 license = "Apache License 2.0"
```

### Comparing `tabulario-0.3.1/tab/__init__.py` & `tabulario-0.3.2/tab/__init__.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.1/tab/cli.py` & `tabulario-0.3.2/tab/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,17 +23,18 @@
     Dict,
     List,
     Optional,
 )
 
 import click
 from click import Context
+from tabular import Tabular
 
 from tab.exceptions import InvalidInputError
-from tab.oauth import OAuthTokenResponse, TabularOAuth
+from tab.oauth import TabularOAuth
 from tab.util import EnhancedJSONEncoder
 
 
 @dataclass(frozen=True)
 class TabularContext:
     environment: str
 
@@ -53,15 +54,15 @@
                 return json.loads(raw_json)
         except JSONDecodeError as e:
             raise InvalidInputError("Invalid JSON") from e
 
     return None
 
 
-def _out(output: OAuthTokenResponse):
+def _out(output: Any) -> None:
     click.echo(json.dumps(output, cls=EnhancedJSONEncoder))
 
 
 @run.command()
 @click.pass_obj
 @click.argument("credential", required=False)
 @click.argument("scopes", required=False, nargs=-1)
@@ -112,7 +113,21 @@
     """Retrieves a fresh token based on an existing token"""
     args = _read_stdin()
     if not args:
         args = {"token": token, "token_type": token_type, "scopes": scopes}
 
     fresh_token = TabularOAuth(ctx.environment).refresh_token(**args)
     _out(fresh_token)
+
+
+@run.command()
+@click.pass_obj
+@click.option("-c", "--credential")
+@click.option("-t", "--token")
+def warehouses(ctx: TabularContext, credential: List[str], token: Optional[str]):
+    """Fetches all the warehouses"""
+    args = _read_stdin()
+    if not args:
+        args = {"token": token, "credential": credential}
+
+    all_warehouses = Tabular(environment=ctx.environment, **args).list_warehouses()
+    _out(all_warehouses)
```

### Comparing `tabulario-0.3.1/tab/exceptions.py` & `tabulario-0.3.2/tab/exceptions.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.1/tab/oauth.py` & `tabulario-0.3.2/tab/oauth.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,25 +90,25 @@
     except HTTPError as e:
         raise ValueError(f"Request failed {response.text}") from e
 
     return response_type(**{**{"scope": None, "expires_in": None}, **response.json()})
 
 
 ENVIRONMENT_URLS = {
-    "prod": "https://api.tabular.io/ws/v1/oauth/tokens",
-    "test": "https://api.test.tabular.io/ws/v1/oauth/tokens",
-    "dev": "https://api.dev.tabular.io/ws/v1/oauth/tokens",
+    "prod": "https://api.tabular.io/ws/v1",
+    "test": "https://api.test.tabular.io/ws/v1",
+    "dev": "https://api.dev.tabular.io/ws/v1",
 }
 
 
 class TabularOAuth:
     base_url: str
 
     def __init__(self, environment: str):
-        self.base_url = ENVIRONMENT_URLS[environment]
+        self.base_url = ENVIRONMENT_URLS[environment] + "/oauth/tokens"
 
     def request_token(self, credential: str, scopes: Optional[Any] = None) -> OAuthTokenResponse:
         if SEMICOLON in credential:
             client_id, client_secret = credential.split(SEMICOLON)
         else:
             client_id, client_secret = None, credential
```

### Comparing `tabulario-0.3.1/tab/util.py` & `tabulario-0.3.2/tab/util.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.1/tabular/loader.py` & `tabulario-0.3.2/tabular/loader.py`

 * *Files identical despite different names*

### Comparing `tabulario-0.3.1/PKG-INFO` & `tabulario-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabulario
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utility library for Tabular.io
 Home-page: https://tabular.io/
 License: Apache-2.0
 Author: Tabular Technologies, Inc.
 Author-email: fokko@tabular.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -107,7 +107,49 @@
     "issued_token_type": "urn:ietf:params:oauth:token-type:access_token",
     "token_type": "Bearer",
     "expires_in": 86400,
     "scope": null
 }
 ```
 
+### Listing all the warehouses
+
+```bash
+➜ tab warehouses --help
+Usage: tab warehouses [OPTIONS]
+
+Fetches all the warehouses
+
+Options:
+-c, --credential TEXT
+-t, --token TEXT
+--help                 Show this message and exit.
+```
+
+Example:
+
+```bash
+➜ tab warehouses --credential t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI | jq
+[
+  {
+    "id": "6efbcaf4-21ae-499d-b340-3bc1a7003f52",
+    "name": "sandbox",
+    "region": "us-east-1"
+  },
+  {
+    "id": "c70f668c-4746-414f-8a74-b1e4f1f0de60",
+    "name": "Fokko",
+    "region": "us-west-2"
+  }
+]
+```
+
+```python
+>> from tabular import Tabular
+>>> t = Tabular("t-GdCZGj5OpoQ:jIcDDITVeIOnqxo7FxWbI21Y3kI")
+>>> t.list_warehouses()
+[
+    Warehouse(id='6efbcaf4-21ae-499d-b340-3bc1a7003f52', name='sandbox', region='us-east-1'),
+    Warehouse(id='c70f668c-4746-414f-8a74-b1e4f1f0de60', name='Fokko', region='us-west-2')
+]
+```
+
```

