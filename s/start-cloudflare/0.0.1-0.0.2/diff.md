# Comparing `tmp/start_cloudflare-0.0.1.tar.gz` & `tmp/start_cloudflare-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_cloudflare-0.0.1.tar", max compression
+gzip compressed data, was "start_cloudflare-0.0.2.tar", max compression
```

## Comparing `start_cloudflare-0.0.1.tar` & `start_cloudflare-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      262 2023-05-15 12:44:07.730544 start_cloudflare-0.0.1/README.md
--rw-r--r--   0        0        0     1312 2023-05-15 12:45:04.227140 start_cloudflare-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       66 2023-05-15 12:12:42.183999 start_cloudflare-0.0.1/start_cloudflare/__init__.py
--rw-r--r--   0        0        0     5471 2023-05-15 12:47:05.837088 start_cloudflare-0.0.1/start_cloudflare/main.py
--rw-r--r--   0        0        0     1097 1970-01-01 00:00:00.000000 start_cloudflare-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      262 2023-06-22 02:15:00.368655 start_cloudflare-0.0.2/README.md
+-rw-r--r--   0        0        0     1431 2023-06-22 02:54:49.599510 start_cloudflare-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-06-22 02:54:49.600033 start_cloudflare-0.0.2/start_cloudflare/__init__.py
+-rw-r--r--   0        0        0     5846 2023-06-22 02:54:49.600527 start_cloudflare-0.0.2/start_cloudflare/main.py
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 start_cloudflare-0.0.2/PKG-INFO
```

### Comparing `start_cloudflare-0.0.1/pyproject.toml` & `start_cloudflare-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 [tool.poetry]
 name = "start-cloudflare"
 description = "A Pydantic BaseSettings class intended to be extended by other Cloudflare services."
-version = "0.0.1"
-authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
+version = "0.0.2"
+authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-cloudflare"
-documentation = "https://mv3.dev/start-cloudflare"
+documentation = "https://justmars.github.io/start-cloudflare"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 python-dotenv = "^1.0"
-pydantic = "^1.10.7"
+pydantic-settings = {version = "^2.0b1", allow-prereleases = true}
+pydantic = {version = "^2.0b3", allow-prereleases = true}
 email-validator = "^2.0.0.post2"
 
 [tool.poetry.group.dev.dependencies]
-rich = "^13.3"
-pytest = "^7.2"
-pytest-datadir = "^1.4"
-pytest-cov = "^2.12"
-pre-commit = "^2.21"
-mkdocs = "^1.4"
-mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.1"
+pytest = "^7.3"
+pytest-env = "^0.8.1"
+pytest-cov = "^4.1"
+pre-commit = "^3.3"
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material = "^9.1.16"
+ipykernel = "^6.23"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --cov --doctest-modules"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
```

### Comparing `start_cloudflare-0.0.1/start_cloudflare/main.py` & `start_cloudflare-0.0.2/start_cloudflare/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from enum import Enum
 from typing import Final
 
-from pydantic import BaseSettings, EmailStr, Field
+from pydantic import EmailStr, Field
+from pydantic_settings import BaseSettings
+from pydantic_settings.main import SettingsConfigDict
 
 CF_API_URL: Final = "https://api.cloudflare.com"
 MIME_TYPE: dict[str, str] = {"Content-Type": "application/json"}
 
 
 class CFSecurityKey(Enum):
     EMAIL = "X-Auth-Email"
@@ -59,51 +61,50 @@
         >>> cf.account_id
         '<ACCT_ID> from https://dash.cloudflare.com/<ACCT_ID>/'
         >>> CF_API_URL
         'https://api.cloudflare.com'
 
     """  # noqa: E501
 
+    model_config = SettingsConfigDict(env_file=".env", env_file_encoding="utf-8")  # type: ignore # noqa: E501
     account_id: str | None = Field(
         default="ACCT",
         repr=False,
-        env="CF_ACCT_ID",
+        validation_alias="CF_ACCT_ID",
     )
     version: int = Field(
         default=4,
         repr=True,
-        env="CF_API_VERSION",
+        validation_alias="CF_API_VERSION",
     )
     email: EmailStr | None = Field(
         default=None,
         repr=True,
-        env="CF_ACCT_EMAIL",
+        validation_alias="CF_ACCT_EMAIL",
     )
     global_api_key: str | None = Field(
         default=None,
         repr=False,
-        env="CF_GLOBAL_API_KEY",
+        validation_alias="CF_GLOBAL_API_KEY",
     )
     origin_ca_key: str | None = Field(
         default=None,
         repr=False,
-        env="CF_ORIGIN_CA_KEY",
+        validation_alias="CF_ORIGIN_CA_KEY",
     )
 
-    class Config:
-        env_file = ".env"
-        env_file_encoding = "utf-8"
-
     @property
     def head_email(self) -> dict[str, str]:
         """Get partial header involving 'X-Auth-Email' key, provided the
         'CF_ACCT_EMAIL' is set.
 
         Examples:
-            >>> cf = CF(email='brightness@long.ago')
+            >>> import os
+            >>> os.environ['CF_ACCT_EMAIL'] = 'brightness@long.ago'
+            >>> cf = CF()
             >>> cf.head_email
             {'X-Auth-Email': 'brightness@long.ago'}
 
         Returns:
             dict[str, str]: Partial header
         """
         if self.email:
@@ -112,15 +113,17 @@
 
     @property
     def head_auth_key(self) -> dict:
         """Get partial header involving the 'X-Auth-Email' key, provided the
         'X-Auth-Key' is set.
 
         Examples:
-            >>> cf = CF(global_api_key='mytoken')
+            >>> import os
+            >>> os.environ['CF_GLOBAL_API_KEY'] = 'mytoken'
+            >>> cf = CF()
             >>> cf.head_auth_key
             {'X-Auth-Key': 'mytoken'}
 
         Returns:
             dict[str, str]: Partial header
         """
         if self.global_api_key:
@@ -145,15 +148,17 @@
     def base(self) -> str:
         """Create the base url for the Cloudflare API with version 4 as default
 
         Examples:
             >>> cf = CF()
             >>> cf.base
             'https://api.cloudflare.com/client/v4'
-            >>> cf = CF(version=5)
+            >>> import os
+            >>> os.environ['CF_API_VERSION'] = '5'
+            >>> cf = CF()
             >>> cf.base
             'https://api.cloudflare.com/client/v5'
 
         Returns:
             str: Partial URL
         """
```

### Comparing `start_cloudflare-0.0.1/PKG-INFO` & `start_cloudflare-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: start-cloudflare
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Pydantic BaseSettings class intended to be extended by other Cloudflare services.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
-Author-email: mars@veloso.one
+Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: email-validator (>=2.0.0.post2,<3.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pydantic (>=2.0b3,<3.0)
+Requires-Dist: pydantic-settings (>=2.0b1,<3.0)
 Requires-Dist: python-dotenv (>=1.0,<2.0)
-Project-URL: Documentation, https://mv3.dev/start-cloudflare
+Project-URL: Documentation, https://justmars.github.io/start-cloudflare
 Project-URL: Repository, https://github.com/justmars/start-cloudflare
 Description-Content-Type: text/markdown
 
 # start-cloudflare
 
 ![Github CI](https://github.com/justmars/start-cloudflare/actions/workflows/main.yml/badge.svg)
```

