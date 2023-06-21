# Comparing `tmp/databricks_sql_connector-2.6.2.tar.gz` & `tmp/databricks_sql_connector-2.6.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databricks_sql_connector-2.6.2.tar", max compression
+gzip compressed data, was "databricks_sql_connector-2.6.3.dev1.tar", max compression
```

## Comparing `databricks_sql_connector-2.6.2.tar` & `databricks_sql_connector-2.6.3.dev1.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     4496 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/CHANGELOG.md
--rw-r--r--   0        0        0    11346 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/LICENSE
--rw-r--r--   0        0        0     2723 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/README.md
--rw-r--r--   0        0        0     1417 2023-06-14 23:41:53.878201 databricks_sql_connector-2.6.2/pyproject.toml
--rw-r--r--   0        0        0      295 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/__init__.py
--rw-r--r--   0        0        0     1269 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/auth/__init__.py
--rw-r--r--   0        0        0     3894 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/auth/auth.py
--rw-r--r--   0        0        0     5493 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/auth/authenticators.py
--rw-r--r--   0        0        0     9717 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/auth/oauth.py
--rw-r--r--   0        0        0     1201 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/auth/oauth_http_handler.py
--rw-r--r--   0        0        0     5949 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/auth/thrift_http_client.py
--rw-r--r--   0        0        0    36862 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/client.py
--rw-r--r--   0        0        0     2423 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/exc.py
--rw-r--r--   0        0        0        0 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/experimental/__init__.py
--rw-r--r--   0        0        0     2236 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/experimental/oauth_persistence.py
--rwxr-xr-x   0        0        0     8062 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
--rw-r--r--   0        0        0   136849 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
--rw-r--r--   0        0        0       49 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/__init__.py
--rw-r--r--   0        0        0     1307 2023-06-14 23:41:27.745801 databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/constants.py
--rw-r--r--   0        0        0  2077276 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/ttypes.py
--rw-r--r--   0        0        0        0 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/__init__.py
--rw-r--r--   0        0        0    41924 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sql/thrift_backend.py
--rw-r--r--   0        0        0     6771 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sql/types.py
--rw-r--r--   0        0        0     6646 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sql/utils.py
--rw-r--r--   0        0        0       60 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     9761 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sqlalchemy/dialect/__init__.py
--rw-r--r--   0        0        0      494 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sqlalchemy/dialect/base.py
--rw-r--r--   0        0        0      792 2023-06-14 23:41:27.753801 databricks_sql_connector-2.6.2/src/databricks/sqlalchemy/dialect/compiler.py
--rw-r--r--   0        0        0     4107 1970-01-01 00:00:00.000000 databricks_sql_connector-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0     4585 2023-06-21 21:04:46.601915 databricks_sql_connector-2.6.3.dev1/CHANGELOG.md
+-rw-r--r--   0        0        0    11346 2023-06-14 20:24:08.166793 databricks_sql_connector-2.6.3.dev1/LICENSE
+-rw-r--r--   0        0        0     2723 2023-06-14 20:24:08.167012 databricks_sql_connector-2.6.3.dev1/README.md
+-rw-r--r--   0        0        0     1421 2023-06-21 22:01:35.095661 databricks_sql_connector-2.6.3.dev1/pyproject.toml
+-rw-r--r--   0        0        0      295 2023-06-14 20:24:08.170343 databricks_sql_connector-2.6.3.dev1/src/databricks/__init__.py
+-rw-r--r--   0        0        0     1273 2023-06-21 22:01:46.449876 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.170890 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/__init__.py
+-rw-r--r--   0        0        0     4421 2023-06-21 18:47:10.955827 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/auth.py
+-rw-r--r--   0        0        0     6192 2023-06-21 18:47:10.956342 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/authenticators.py
+-rw-r--r--   0        0        0     3790 2023-06-21 18:47:10.956670 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/endpoint.py
+-rw-r--r--   0        0        0     9499 2023-06-21 18:47:10.957158 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth.py
+-rw-r--r--   0        0        0     1201 2023-06-14 20:24:08.171709 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth_http_handler.py
+-rw-r--r--   0        0        0     5949 2023-06-14 20:24:08.171906 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/thrift_http_client.py
+-rw-r--r--   0        0        0    36862 2023-06-14 20:24:08.172377 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/client.py
+-rw-r--r--   0        0        0     2423 2023-06-14 20:24:08.172576 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/exc.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.172808 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/experimental/__init__.py
+-rw-r--r--   0        0        0     2543 2023-06-21 18:47:10.957602 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/experimental/oauth_persistence.py
+-rwxr-xr-x   0        0        0     8062 2023-06-14 20:24:08.173439 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote
+-rw-r--r--   0        0        0   136849 2023-06-14 20:24:08.175895 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py
+-rw-r--r--   0        0        0       49 2023-06-14 20:24:08.176090 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/__init__.py
+-rw-r--r--   0        0        0     1307 2023-06-14 20:24:08.176221 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py
+-rw-r--r--   0        0        0  2077276 2023-06-14 20:24:08.177855 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py
+-rw-r--r--   0        0        0        0 2023-06-14 20:24:08.178096 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/__init__.py
+-rw-r--r--   0        0        0    42976 2023-06-21 21:48:18.641419 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_backend.py
+-rw-r--r--   0        0        0     6771 2023-06-14 20:24:08.178634 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/types.py
+-rw-r--r--   0        0        0     6646 2023-06-14 20:24:08.178813 databricks_sql_connector-2.6.3.dev1/src/databricks/sql/utils.py
+-rw-r--r--   0        0        0       60 2023-06-14 20:24:08.179003 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     9761 2023-06-14 20:24:08.179220 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-14 20:24:08.179360 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/base.py
+-rw-r--r--   0        0        0      792 2023-06-14 20:24:08.179497 databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/compiler.py
+-rw-r--r--   0        0        0     4112 1970-01-01 00:00:00.000000 databricks_sql_connector-2.6.3.dev1/PKG-INFO
```

### Comparing `databricks_sql_connector-2.6.2/CHANGELOG.md` & `databricks_sql_connector-2.6.3.dev1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Release History
 
 ## 2.6.x (Unreleased)
 
+- Redact logged thrift responses by default
+- Add support for OAuth on Databricks Azure
+
 ## 2.6.2 (2023-06-14)
 
 - Fix: Retry GetOperationStatus requests for http errors
 
 ## 2.6.1 (2023-06-08)
 
 - Fix: http.client would raise a BadStatusLine exception in some cases
```

### Comparing `databricks_sql_connector-2.6.2/LICENSE` & `databricks_sql_connector-2.6.3.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/README.md` & `databricks_sql_connector-2.6.3.dev1/README.md`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/pyproject.toml` & `databricks_sql_connector-2.6.3.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "databricks-sql-connector"
-version = "2.6.2"
+version = "2.6.3dev1"
 description = "Databricks SQL Connector for Python"
 authors = ["Databricks <databricks-sql-connector-maintainers@databricks.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "databricks", from = "src"}]
 include = ["CHANGELOG.md"]
```

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/__init__.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 NUMBER = DBAPITypeObject(
     "boolean", "tinyint", "smallint", "int", "bigint", "float", "double", "decimal"
 )
 DATETIME = DBAPITypeObject("timestamp")
 DATE = DBAPITypeObject("date")
 ROWID = DBAPITypeObject()
 
-__version__ = "2.6.2"
+__version__ = "2.6.3dev1"
 USER_AGENT_NAME = "PyDatabricksSqlConnector"
 
 # These two functions are pyhive legacy
 Date = datetime.date
 Timestamp = datetime.datetime
```

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/auth/auth.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from databricks.sql.auth.authenticators import (
     AuthProvider,
     AccessTokenAuthProvider,
     BasicAuthProvider,
     ExternalAuthProvider,
     DatabricksOAuthProvider,
 )
+from databricks.sql.auth.endpoint import infer_cloud_from_host, CloudType
 from databricks.sql.experimental.oauth_persistence import OAuthPersistence
 
 
 class AuthType(Enum):
     DATABRICKS_OAUTH = "databricks-oauth"
     # other supported types (access_token, user/pass) can be inferred
     # we can add more types as needed later
@@ -71,34 +72,45 @@
         return AuthProvider()
     else:
         raise RuntimeError("No valid authentication settings!")
 
 
 PYSQL_OAUTH_SCOPES = ["sql", "offline_access"]
 PYSQL_OAUTH_CLIENT_ID = "databricks-sql-python"
+PYSQL_OAUTH_AZURE_CLIENT_ID = "96eecda7-19ea-49cc-abb5-240097d554f5"
 PYSQL_OAUTH_REDIRECT_PORT_RANGE = list(range(8020, 8025))
+PYSQL_OAUTH_AZURE_REDIRECT_PORT_RANGE = [8030]
 
 
 def normalize_host_name(hostname: str):
     maybe_scheme = "https://" if not hostname.startswith("https://") else ""
     maybe_trailing_slash = "/" if not hostname.endswith("/") else ""
     return f"{maybe_scheme}{hostname}{maybe_trailing_slash}"
 
 
+def get_client_id_and_redirect_port(hostname: str):
+    return (
+        (PYSQL_OAUTH_CLIENT_ID, PYSQL_OAUTH_REDIRECT_PORT_RANGE)
+        if infer_cloud_from_host(hostname) == CloudType.AWS
+        else (PYSQL_OAUTH_AZURE_CLIENT_ID, PYSQL_OAUTH_AZURE_REDIRECT_PORT_RANGE)
+    )
+
+
 def get_python_sql_connector_auth_provider(hostname: str, **kwargs):
+    (client_id, redirect_port_range) = get_client_id_and_redirect_port(hostname)
     cfg = ClientContext(
         hostname=normalize_host_name(hostname),
         auth_type=kwargs.get("auth_type"),
         access_token=kwargs.get("access_token"),
         username=kwargs.get("_username"),
         password=kwargs.get("_password"),
         use_cert_as_auth=kwargs.get("_use_cert_as_auth"),
         tls_client_cert_file=kwargs.get("_tls_client_cert_file"),
         oauth_scopes=PYSQL_OAUTH_SCOPES,
-        oauth_client_id=kwargs.get("oauth_client_id") or PYSQL_OAUTH_CLIENT_ID,
+        oauth_client_id=kwargs.get("oauth_client_id") or client_id,
         oauth_redirect_port_range=[kwargs["oauth_redirect_port"]]
         if kwargs.get("oauth_client_id") and kwargs.get("oauth_redirect_port")
-        else PYSQL_OAUTH_REDIRECT_PORT_RANGE,
+        else redirect_port_range,
         oauth_persistence=kwargs.get("experimental_oauth_persistence"),
         credentials_provider=kwargs.get("credentials_provider"),
     )
     return get_auth_provider(cfg)
```

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/auth/authenticators.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/authenticators.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import base64
 import logging
 from typing import Callable, Dict, List
 
 from databricks.sql.auth.oauth import OAuthManager
+from databricks.sql.auth.endpoint import get_oauth_endpoints, infer_cloud_from_host
 
 # Private API: this is an evolving interface and it will change in the future.
 # Please must not depend on it in your applications.
 from databricks.sql.experimental.oauth_persistence import OAuthToken, OAuthPersistence
 
 
 class AuthProvider:
@@ -66,19 +67,34 @@
         hostname: str,
         oauth_persistence: OAuthPersistence,
         redirect_port_range: List[int],
         client_id: str,
         scopes: List[str],
     ):
         try:
+            cloud_type = infer_cloud_from_host(hostname)
+            if not cloud_type:
+                raise NotImplementedError("Cannot infer the cloud type from hostname")
+
+            idp_endpoint = get_oauth_endpoints(cloud_type)
+            if not idp_endpoint:
+                raise NotImplementedError(
+                    f"OAuth is not supported for cloud ${cloud_type.value}"
+                )
+
+            # Convert to the corresponding scopes in the corresponding IdP
+            cloud_scopes = idp_endpoint.get_scopes_mapping(scopes)
+
             self.oauth_manager = OAuthManager(
-                port_range=redirect_port_range, client_id=client_id
+                port_range=redirect_port_range,
+                client_id=client_id,
+                idp_endpoint=idp_endpoint,
             )
             self._hostname = hostname
-            self._scopes_as_str = DatabricksOAuthProvider.SCOPE_DELIM.join(scopes)
+            self._scopes_as_str = DatabricksOAuthProvider.SCOPE_DELIM.join(cloud_scopes)
             self._oauth_persistence = oauth_persistence
             self._client_id = client_id
             self._access_token = None
             self._refresh_token = None
             self._initial_get_token()
         except Exception as e:
             logging.error(f"unexpected error", e, exc_info=True)
```

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/auth/oauth.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,72 +10,71 @@
 
 import oauthlib.oauth2
 import requests
 from oauthlib.oauth2.rfc6749.errors import OAuth2Error
 from requests.exceptions import RequestException
 
 from databricks.sql.auth.oauth_http_handler import OAuthHttpSingleRequestHandler
+from databricks.sql.auth.endpoint import OAuthEndpointCollection
 
 logger = logging.getLogger(__name__)
 
 
 class OAuthManager:
-    OIDC_REDIRECTOR_PATH = "oidc"
-
-    def __init__(self, port_range: List[int], client_id: str):
+    def __init__(
+        self,
+        port_range: List[int],
+        client_id: str,
+        idp_endpoint: OAuthEndpointCollection,
+    ):
         self.port_range = port_range
         self.client_id = client_id
         self.redirect_port = None
+        self.idp_endpoint = idp_endpoint
 
     @staticmethod
     def __token_urlsafe(nbytes=32):
         return secrets.token_urlsafe(nbytes)
 
     @staticmethod
     def __get_redirect_url(redirect_port: int):
         return f"http://localhost:{redirect_port}"
 
-    @staticmethod
-    def __fetch_well_known_config(idp_url: str):
-        known_config_url = f"{idp_url}/.well-known/oauth-authorization-server"
+    def __fetch_well_known_config(self, hostname: str):
+        known_config_url = self.idp_endpoint.get_openid_config_url(hostname)
+
         try:
             response = requests.get(url=known_config_url)
         except RequestException as e:
             logger.error(
-                f"Unable to fetch OAuth configuration from {idp_url}.\n"
+                f"Unable to fetch OAuth configuration from {known_config_url}.\n"
                 "Verify it is a valid workspace URL and that OAuth is "
                 "enabled on this account."
             )
             raise e
 
         if response.status_code != 200:
             msg = (
                 f"Received status {response.status_code} OAuth configuration from "
-                f"{idp_url}.\n Verify it is a valid workspace URL and "
+                f"{known_config_url}.\n Verify it is a valid workspace URL and "
                 "that OAuth is enabled on this account."
             )
             logger.error(msg)
             raise RuntimeError(msg)
         try:
             return response.json()
         except requests.exceptions.JSONDecodeError as e:
             logger.error(
-                f"Unable to decode OAuth configuration from {idp_url}.\n"
+                f"Unable to decode OAuth configuration from {known_config_url}.\n"
                 "Verify it is a valid workspace URL and that OAuth is "
                 "enabled on this account."
             )
             raise e
 
     @staticmethod
-    def __get_idp_url(host: str):
-        maybe_scheme = "https://" if not host.startswith("https://") else ""
-        maybe_trailing_slash = "/" if not host.endswith("/") else ""
-        return f"{maybe_scheme}{host}{maybe_trailing_slash}{OAuthManager.OIDC_REDIRECTOR_PATH}"
-
-    @staticmethod
     def __get_challenge():
         verifier_string = OAuthManager.__token_urlsafe(32)
         digest = hashlib.sha256(verifier_string.encode("UTF-8")).digest()
         challenge_string = (
             base64.urlsafe_b64encode(digest).decode("UTF-8").replace("=", "")
         )
         return verifier_string, challenge_string
@@ -150,16 +149,15 @@
             "Accept": "application/json",
             "Content-Type": "application/x-www-form-urlencoded",
         }
         response = requests.post(url=token_request_url, data=data, headers=headers)
         return response.json()
 
     def __send_refresh_token_request(self, hostname, refresh_token):
-        idp_url = OAuthManager.__get_idp_url(hostname)
-        oauth_config = OAuthManager.__fetch_well_known_config(idp_url)
+        oauth_config = self.__fetch_well_known_config(hostname)
         token_request_url = oauth_config["token_endpoint"]
         client = oauthlib.oauth2.WebApplicationClient(self.client_id)
         token_request_body = client.prepare_refresh_body(
             refresh_token=refresh_token, client_id=client.client_id
         )
         return OAuthManager.__send_token_request(token_request_url, token_request_body)
 
@@ -211,22 +209,23 @@
         oauth_response = self.__send_refresh_token_request(hostname, refresh_token)
         fresh_access_token, fresh_refresh_token = self.__get_tokens_from_response(
             oauth_response
         )
         return fresh_access_token, fresh_refresh_token, True
 
     def get_tokens(self, hostname: str, scope=None):
-        idp_url = self.__get_idp_url(hostname)
-        oauth_config = self.__fetch_well_known_config(idp_url)
+        oauth_config = self.__fetch_well_known_config(hostname)
         # We are going to override oauth_config["authorization_endpoint"] use the
         # /oidc redirector on the hostname, which may inject additional parameters.
-        auth_url = f"{hostname}oidc/v1/authorize"
+        auth_url = self.idp_endpoint.get_authorization_url(hostname)
+
         state = OAuthManager.__token_urlsafe(16)
         (verifier, challenge) = OAuthManager.__get_challenge()
         client = oauthlib.oauth2.WebApplicationClient(self.client_id)
+
         try:
             auth_response = self.__get_authorization_code(
                 client, auth_url, scope, state, challenge
             )
         except OAuth2Error as e:
             msg = f"OAuth Authorization Error: {e.description}"
             logger.error(msg)
```

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/auth/oauth_http_handler.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/oauth_http_handler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/auth/thrift_http_client.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/auth/thrift_http_client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/client.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/client.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/exc.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/exc.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/experimental/oauth_persistence.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/experimental/oauth_persistence.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,25 @@
     def persist(self, hostname: str, oauth_token: OAuthToken):
         pass
 
     def read(self, hostname: str) -> Optional[OAuthToken]:
         pass
 
 
+class OAuthPersistenceCache(OAuthPersistence):
+    def __init__(self):
+        self.tokens = {}
+
+    def persist(self, hostname: str, oauth_token: OAuthToken):
+        self.tokens[hostname] = oauth_token
+
+    def read(self, hostname: str) -> Optional[OAuthToken]:
+        return self.tokens.get(hostname)
+
+
 # Note this is only intended to be used for development
 class DevOnlyFilePersistence(OAuthPersistence):
     def __init__(self, file_path):
         self._file_path = file_path
 
     def persist(self, hostname: str, token: OAuthToken):
         logger.info(f"persisting token in {self._file_path}")
```

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService-remote`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/TCLIService.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/TCLIService.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/constants.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/constants.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/thrift_api/TCLIService/ttypes.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_api/TCLIService/ttypes.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/thrift_backend.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/thrift_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,24 @@
     _bound,
     RequestErrorInfo,
     NoRetryReason,
 )
 
 logger = logging.getLogger(__name__)
 
+unsafe_logger = logging.getLogger("databricks.sql.unsafe")
+unsafe_logger.setLevel(logging.DEBUG)
+
+# To capture these logs in client code, add a non-NullHandler.
+# See our e2e test suite for an example with logging.FileHandler
+unsafe_logger.addHandler(logging.NullHandler())
+
+# Disable propagation so that handlers for `databricks.sql` don't pick up these messages
+unsafe_logger.propagate = False
+
 THRIFT_ERROR_MESSAGE_HEADER = "x-thriftserver-error-message"
 DATABRICKS_ERROR_OR_REDIRECT_HEADER = "x-databricks-error-or-redirect-message"
 DATABRICKS_REASON_HEADER = "x-databricks-reason-phrase"
 
 TIMESTAMP_AS_STRING_CONFIG = "spark.thriftserver.arrowBasedRowSet.timestampAsString"
 DEFAULT_SOCKET_TIMEOUT = float(900)
 
@@ -314,21 +324,33 @@
             # returns tuple: (method_return, delay_fn(), error, error_message)
             # - non-None method_return -> success, return and be done
             # - non-None retry_delay -> sleep delay before retry
             # - error, error_message always set when available
 
             error, error_message, retry_delay = None, None, None
             try:
-                logger.debug("Sending request: {}".format(request))
+                # The MagicMocks in our unit tests have a `name` property instead of `__name__`.
+                logger.debug(
+                    "Sending request: {}(<REDACTED>)".format(
+                        getattr(
+                            method, "__name__", getattr(method, "name", "UnknownMethod")
+                        )
+                    )
+                )
+                unsafe_logger.debug("Sending request: {}".format(request))
                 response = method(request)
 
                 # Calling `close()` here releases the active HTTP connection back to the pool
                 self._transport.close()
 
-                logger.debug("Received response: {}".format(response))
+                # We need to call type(response) here because thrift doesn't implement __name__ attributes for thrift responses
+                logger.debug(
+                    "Received response: {}(<REDACTED>)".format(type(response).__name__)
+                )
+                unsafe_logger.debug("Received response: {}".format(response))
                 return response
 
             except urllib3.exceptions.HTTPError as err:
                 # retry on timeout. Happens a lot in Azure and it is safe as data has not been sent to server yet
 
                 gos_name = TCLIServiceClient.GetOperationStatus.__name__
                 if method.__name__ == gos_name:
```

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/types.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/types.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sql/utils.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sql/utils.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sqlalchemy/dialect/__init__.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/src/databricks/sqlalchemy/dialect/compiler.py` & `databricks_sql_connector-2.6.3.dev1/src/databricks/sqlalchemy/dialect/compiler.py`

 * *Files identical despite different names*

### Comparing `databricks_sql_connector-2.6.2/PKG-INFO` & `databricks_sql_connector-2.6.3.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databricks-sql-connector
-Version: 2.6.2
+Version: 2.6.3.dev1
 Summary: Databricks SQL Connector for Python
 License: Apache-2.0
 Author: Databricks
 Author-email: databricks-sql-connector-maintainers@databricks.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

