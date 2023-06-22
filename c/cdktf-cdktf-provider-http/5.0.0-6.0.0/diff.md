# Comparing `tmp/cdktf-cdktf-provider-http-5.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-http-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-http-5.0.0.tar", last modified: Thu Jun 15 11:28:08 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-http-6.0.0.tar", last modified: Thu Jun 22 03:12:48 2023, max compression
```

## Comparing `cdktf-cdktf-provider-http-5.0.0.tar` & `cdktf-cdktf-provider-http-6.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29273 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/_jsii/provider-http@5.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/data_http/
--rw-r--r--   0 runner    (1001) docker     (123)    45926 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.149111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:27:52.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 11:28:08.145111 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-15 11:28:08.000000 cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:12:48.645042 cdktf-cdktf-provider-http-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/_jsii/provider-http@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/data_http/
+-rw-r--r--   0 runner    (1001) docker     (123)    46130 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:12:37.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:12:48.649042 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-22 03:12:48.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-22 03:12:48.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:12:48.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-22 03:12:48.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 03:12:48.000000 cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-http-5.0.0/LICENSE` & `cdktf-cdktf-provider-http-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-5.0.0/PKG-INFO` & `cdktf-cdktf-provider-http-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-http-5.0.0/README.md` & `cdktf-cdktf-provider-http-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-5.0.0/setup.py` & `cdktf-cdktf-provider-http-6.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-http",
-    "version": "5.0.0",
+    "version": "6.0.0",
     "description": "Prebuilt http Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-http.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -24,15 +24,15 @@
         "cdktf_cdktf_provider_http",
         "cdktf_cdktf_provider_http._jsii",
         "cdktf_cdktf_provider_http.data_http",
         "cdktf_cdktf_provider_http.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_http._jsii": [
-            "provider-http@5.0.0.jsii.tgz"
+            "provider-http@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_http": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/__init__.py` & `cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py` & `cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_http`
 
-Refer to the Terraform Registory for docs: [`data_http`](https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http).
+Refer to the Terraform Registory for docs: [`data_http`](https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class DataHttp(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-http.dataHttp.DataHttp",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http http}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http http}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         url: builtins.str,
@@ -45,26 +45,26 @@
         count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http http} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http http} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#url DataHttp#url}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
-        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#insecure DataHttp#insecure}
-        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#method DataHttp#method}
-        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_body DataHttp#request_body}
-        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_headers DataHttp#request_headers}
-        :param request_timeout_ms: The request timeout in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
-        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#retry DataHttp#retry}
+        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#url DataHttp#url}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#insecure DataHttp#insecure}
+        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#method DataHttp#method}
+        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_body DataHttp#request_body}
+        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_headers DataHttp#request_headers}
+        :param request_timeout_ms: The request timeout in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
+        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#retry DataHttp#retry}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -98,17 +98,17 @@
         self,
         *,
         attempts: typing.Optional[jsii.Number] = None,
         max_delay_ms: typing.Optional[jsii.Number] = None,
         min_delay_ms: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param attempts: The number of times the request is to be retried. For example, if 2 is specified, the request will be tried a maximum of 3 times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#attempts DataHttp#attempts}
-        :param max_delay_ms: The maximum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
-        :param min_delay_ms: The minimum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
+        :param attempts: The number of times the request is to be retried. For example, if 2 is specified, the request will be tried a maximum of 3 times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#attempts DataHttp#attempts}
+        :param max_delay_ms: The maximum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
+        :param min_delay_ms: The minimum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
         '''
         value = DataHttpRetry(
             attempts=attempts, max_delay_ms=max_delay_ms, min_delay_ms=min_delay_ms
         )
 
         return typing.cast(None, jsii.invoke(self, "putRetry", [value]))
 
@@ -161,14 +161,19 @@
 
     @builtins.property
     @jsii.member(jsii_name="responseBody")
     def response_body(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "responseBody"))
 
     @builtins.property
+    @jsii.member(jsii_name="responseBodyBase64")
+    def response_body_base64(self) -> builtins.str:
+        return typing.cast(builtins.str, jsii.get(self, "responseBodyBase64"))
+
+    @builtins.property
     @jsii.member(jsii_name="responseHeaders")
     def response_headers(self) -> _cdktf_9a9027ec.StringMap:
         return typing.cast(_cdktf_9a9027ec.StringMap, jsii.get(self, "responseHeaders"))
 
     @builtins.property
     @jsii.member(jsii_name="retry")
     def retry(self) -> "DataHttpRetryOutputReference":
@@ -213,16 +218,16 @@
     def request_timeout_ms_input(self) -> typing.Optional[jsii.Number]:
         return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "requestTimeoutMsInput"))
 
     @builtins.property
     @jsii.member(jsii_name="retryInput")
     def retry_input(
         self,
-    ) -> typing.Optional[typing.Union["DataHttpRetry", _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union["DataHttpRetry", _cdktf_9a9027ec.IResolvable]], jsii.get(self, "retryInput"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, "DataHttpRetry"]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, "DataHttpRetry"]], jsii.get(self, "retryInput"))
 
     @builtins.property
     @jsii.member(jsii_name="urlInput")
     def url_input(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "urlInput"))
 
     @builtins.property
@@ -361,22 +366,22 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#url DataHttp#url}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
-        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#insecure DataHttp#insecure}
-        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#method DataHttp#method}
-        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_body DataHttp#request_body}
-        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_headers DataHttp#request_headers}
-        :param request_timeout_ms: The request timeout in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
-        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#retry DataHttp#retry}
+        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#url DataHttp#url}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#insecure DataHttp#insecure}
+        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#method DataHttp#method}
+        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_body DataHttp#request_body}
+        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_headers DataHttp#request_headers}
+        :param request_timeout_ms: The request timeout in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
+        :param retry: retry block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#retry DataHttp#retry}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(retry, dict):
             retry = DataHttpRetry(**retry)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ee2b6a3664a80e642a2ef1d255302a3f3dc3d391999cb8f3d6103cac8420d573)
@@ -491,85 +496,85 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def url(self) -> builtins.str:
         '''The URL for the request. Supported schemes are ``http`` and ``https``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#url DataHttp#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#url DataHttp#url}
         '''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ca_cert_pem(self) -> typing.Optional[builtins.str]:
         '''Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
         '''
         result = self._values.get("ca_cert_pem")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Disables verification of the server's certificate chain and hostname. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#insecure DataHttp#insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#insecure DataHttp#insecure}
         '''
         result = self._values.get("insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def method(self) -> typing.Optional[builtins.str]:
         '''The HTTP Method for the request.
 
         Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#method DataHttp#method}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#method DataHttp#method}
         '''
         result = self._values.get("method")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def request_body(self) -> typing.Optional[builtins.str]:
         '''The request body as a string.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_body DataHttp#request_body}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_body DataHttp#request_body}
         '''
         result = self._values.get("request_body")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def request_headers(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''A map of request header field names and values.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_headers DataHttp#request_headers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_headers DataHttp#request_headers}
         '''
         result = self._values.get("request_headers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def request_timeout_ms(self) -> typing.Optional[jsii.Number]:
         '''The request timeout in milliseconds.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#request_timeout_ms DataHttp#request_timeout_ms}
         '''
         result = self._values.get("request_timeout_ms")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def retry(self) -> typing.Optional["DataHttpRetry"]:
         '''retry block.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#retry DataHttp#retry}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#retry DataHttp#retry}
         '''
         result = self._values.get("retry")
         return typing.cast(typing.Optional["DataHttpRetry"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -596,17 +601,17 @@
         self,
         *,
         attempts: typing.Optional[jsii.Number] = None,
         max_delay_ms: typing.Optional[jsii.Number] = None,
         min_delay_ms: typing.Optional[jsii.Number] = None,
     ) -> None:
         '''
-        :param attempts: The number of times the request is to be retried. For example, if 2 is specified, the request will be tried a maximum of 3 times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#attempts DataHttp#attempts}
-        :param max_delay_ms: The maximum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
-        :param min_delay_ms: The minimum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
+        :param attempts: The number of times the request is to be retried. For example, if 2 is specified, the request will be tried a maximum of 3 times. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#attempts DataHttp#attempts}
+        :param max_delay_ms: The maximum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
+        :param min_delay_ms: The minimum delay between retry requests in milliseconds. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5db3ea948028eba5857abc78a333d807c1e084b83b50b80801b01c9a63f2d524)
             check_type(argname="argument attempts", value=attempts, expected_type=type_hints["attempts"])
             check_type(argname="argument max_delay_ms", value=max_delay_ms, expected_type=type_hints["max_delay_ms"])
             check_type(argname="argument min_delay_ms", value=min_delay_ms, expected_type=type_hints["min_delay_ms"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
@@ -619,33 +624,33 @@
 
     @builtins.property
     def attempts(self) -> typing.Optional[jsii.Number]:
         '''The number of times the request is to be retried.
 
         For example, if 2 is specified, the request will be tried a maximum of 3 times.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#attempts DataHttp#attempts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#attempts DataHttp#attempts}
         '''
         result = self._values.get("attempts")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def max_delay_ms(self) -> typing.Optional[jsii.Number]:
         '''The maximum delay between retry requests in milliseconds.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#max_delay_ms DataHttp#max_delay_ms}
         '''
         result = self._values.get("max_delay_ms")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def min_delay_ms(self) -> typing.Optional[jsii.Number]:
         '''The minimum delay between retry requests in milliseconds.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs/data-sources/http#min_delay_ms DataHttp#min_delay_ms}
         '''
         result = self._values.get("min_delay_ms")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -741,21 +746,21 @@
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "minDelayMs", value)
 
     @builtins.property
     @jsii.member(jsii_name="internalValue")
     def internal_value(
         self,
-    ) -> typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]]:
-        return typing.cast(typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]], jsii.get(self, "internalValue"))
+    ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, DataHttpRetry]]:
+        return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, DataHttpRetry]], jsii.get(self, "internalValue"))
 
     @internal_value.setter
     def internal_value(
         self,
-        value: typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]],
+        value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, DataHttpRetry]],
     ) -> None:
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__8a2d49cc40232891cff2e743c36c379a77b753843ddef54acaa1aa0c95341d88)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "internalValue", value)
 
 
@@ -885,11 +890,11 @@
 def _typecheckingstub__5d59f2427a3deeb5b67ceab4f858492ff5754a45bc2792465bae30603cbe442f(
     value: jsii.Number,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__8a2d49cc40232891cff2e743c36c379a77b753843ddef54acaa1aa0c95341d88(
-    value: typing.Optional[typing.Union[DataHttpRetry, _cdktf_9a9027ec.IResolvable]],
+    value: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, DataHttpRetry]],
 ) -> None:
     """Type checking stubs"""
     pass
```

### Comparing `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py` & `cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`http`](https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs).
+Refer to the Terraform Registory for docs: [`http`](https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class HttpProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-http.provider.HttpProvider",
 ):
-    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs http}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs http}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs http} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs http} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs#alias HttpProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs#alias HttpProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed4656733258f821890abe9b576315755fbb2c26c5225d063440932e3244ec0a)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HttpProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-http.provider.HttpProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class HttpProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs#alias HttpProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs#alias HttpProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c5e292f1b2ced23926cb25076c6e327c7591be5943163c3c72b898964467f963)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.3.0/docs#alias HttpProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.4.0/docs#alias HttpProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO` & `cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 5.0.0
+Version: 6.0.0
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-http-5.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-http-6.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/cdktf_cdktf_provider_http/py.typed
 src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_http.egg-info/requires.txt
 src/cdktf_cdktf_provider_http.egg-info/top_level.txt
 src/cdktf_cdktf_provider_http/_jsii/__init__.py
-src/cdktf_cdktf_provider_http/_jsii/provider-http@5.0.0.jsii.tgz
+src/cdktf_cdktf_provider_http/_jsii/provider-http@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_http/data_http/__init__.py
 src/cdktf_cdktf_provider_http/provider/__init__.py
```

