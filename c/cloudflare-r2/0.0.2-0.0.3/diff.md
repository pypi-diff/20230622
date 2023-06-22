# Comparing `tmp/cloudflare_r2-0.0.2.tar.gz` & `tmp/cloudflare_r2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare_r2-0.0.2.tar", max compression
+gzip compressed data, was "cloudflare_r2-0.0.3.tar", max compression
```

## Comparing `cloudflare_r2-0.0.2.tar` & `cloudflare_r2-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-05-15 14:17:56.734231 cloudflare_r2-0.0.2/LICENSE
--rw-r--r--   0        0        0      253 2023-05-15 15:11:48.461211 cloudflare_r2-0.0.2/README.md
--rw-r--r--   0        0        0       73 2023-05-25 06:07:18.337332 cloudflare_r2-0.0.2/cloudflare_r2/__init__.py
--rw-r--r--   0        0        0     8124 2023-05-25 06:10:00.302571 cloudflare_r2-0.0.2/cloudflare_r2/main.py
--rw-r--r--   0        0        0     1333 2023-05-25 07:48:32.968616 cloudflare_r2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      999 1970-01-01 00:00:00.000000 cloudflare_r2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-06-14 11:00:13.758722 cloudflare_r2-0.0.3/LICENSE
+-rw-r--r--   0        0        0      253 2023-06-14 11:00:13.758802 cloudflare_r2-0.0.3/README.md
+-rw-r--r--   0        0        0       51 2023-06-22 03:03:18.531837 cloudflare_r2-0.0.3/cloudflare_r2/__init__.py
+-rw-r--r--   0        0        0     8191 2023-06-22 03:03:18.532194 cloudflare_r2-0.0.3/cloudflare_r2/main.py
+-rw-r--r--   0        0        0      824 2023-06-22 03:03:18.532406 cloudflare_r2-0.0.3/cloudflare_r2/nb.ipynb
+-rw-r--r--   0        0        0     1280 2023-06-22 03:03:18.532729 cloudflare_r2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 cloudflare_r2-0.0.3/PKG-INFO
```

### Comparing `cloudflare_r2-0.0.2/LICENSE` & `cloudflare_r2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare_r2-0.0.2/cloudflare_r2/main.py` & `cloudflare_r2-0.0.3/cloudflare_r2/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,18 +24,20 @@
         >>> os.environ['R2_SECRET_ACCESS_KEY'] = "XYZ"
         >>> r2 = CloudflareR2()
         >>> type(r2.resource)
         <class 'boto3.resources.factory.s3.ServiceResource'>
 
     """  # noqa: E501
 
-    region: str = Field(default="apac", repr=True, env="CF_R2_REGION")
-    access_key_id: str = Field(default="ABC", repr=False, env="R2_ACCESS_KEY_ID")
+    region: str = Field(default="apac", repr=True, validation_alias="CF_R2_REGION")
+    access_key_id: str = Field(
+        default="ABC", repr=False, validation_alias="R2_ACCESS_KEY_ID"
+    )  # noqa: E501
     secret_access_key: str = Field(
-        default="XYZ", repr=False, env="R2_SECRET_ACCESS_KEY"
+        default="XYZ", repr=False, validation_alias="R2_SECRET_ACCESS_KEY"
     )
 
     @property
     def endpoint_url(self):
         return f"https://{self.account_id}.r2.cloudflarestorage.com"
 
     @property
```

### Comparing `cloudflare_r2-0.0.2/pyproject.toml` & `cloudflare_r2-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 [tool.poetry]
 name = "cloudflare-r2"
 description = "Wrapper around commonly used boto3 functions in Cloudflare R2 API."
-version = "0.0.2"
-authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
+version = "0.0.3"
+authors = ["Marcelino G. Veloso III <contact@mv3.dev>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/cloudflare-r2"
-documentation = "https://mv3.dev/cloudflare-r2"
+documentation = "https://justmars.github.io/cloudflare-r2"
 classifiers = [
   "Programming Language :: Python :: 3.11",
   "Typing :: Typed",
   "Development Status :: 4 - Beta",
   "Framework :: Pytest",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
-python-dotenv = "^1.0"
+start-cloudflare = "^0.0.2"
 boto3 = "^1.26"
-start-cloudflare = "^0.0.1"
 
-[tool.poetry.group.dev.dependencies] # latest as of Jan. 2023
-rich = "^13.3"
-pytest = "^7.2"
-pytest-datadir = "^1.4.1"
+[tool.poetry.group.dev.dependencies] # latest as of June 2023
+pytest = "^7.3"
 pytest-cov = "^2.12.1"
-pre-commit = "^2.21"
-mkdocs = "^1.4.2"
-mkdocstrings = { extras = ["python"], version = "^0.20.0" }
-mkdocs-material = "^9.1"
-ipykernel = "^6.22.0"
+pre-commit = "^3.3"
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material = "^9.1.16"
+ipykernel = "^6.23.1"
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 addopts = "-ra -q --doctest-modules --cov"
 filterwarnings = [
   "ignore::DeprecationWarning", # DeprecationWarning: pkg_resources is deprecated as an API
 ]
```

### Comparing `cloudflare_r2-0.0.2/PKG-INFO` & `cloudflare_r2-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: cloudflare-r2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wrapper around commonly used boto3 functions in Cloudflare R2 API.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
-Author-email: mars@veloso.one
+Author-email: contact@mv3.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: boto3 (>=1.26,<2.0)
-Requires-Dist: python-dotenv (>=1.0,<2.0)
-Requires-Dist: start-cloudflare (>=0.0.1,<0.0.2)
-Project-URL: Documentation, https://mv3.dev/cloudflare-r2
+Requires-Dist: start-cloudflare (>=0.0.2,<0.0.3)
+Project-URL: Documentation, https://justmars.github.io/cloudflare-r2
 Project-URL: Repository, https://github.com/justmars/cloudflare-r2
 Description-Content-Type: text/markdown
 
 # cloudflare-r2
 
 ![Github CI](https://github.com/justmars/cloudflare-r2/actions/workflows/main.yml/badge.svg)
```

