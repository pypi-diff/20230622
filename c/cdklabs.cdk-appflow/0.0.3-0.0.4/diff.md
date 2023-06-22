# Comparing `tmp/cdklabs.cdk-appflow-0.0.3.tar.gz` & `tmp/cdklabs.cdk-appflow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdklabs.cdk-appflow-0.0.3.tar", last modified: Thu Jun 22 00:34:40 2023, max compression
+gzip compressed data, was "cdklabs.cdk-appflow-0.0.4.tar", last modified: Thu Jun 22 09:33:04 2023, max compression
```

## Comparing `cdklabs.cdk-appflow-0.0.3.tar` & `cdklabs.cdk-appflow-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:40.785606 cdklabs.cdk-appflow-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-22 00:34:40.785606 cdklabs.cdk-appflow-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:34:40.785606 cdklabs.cdk-appflow-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:40.781606 cdklabs.cdk-appflow-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:40.781606 cdklabs.cdk-appflow-0.0.3/src/cdklabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:40.785606 cdklabs.cdk-appflow-0.0.3/src/cdklabs/cdk_appflow/
--rw-r--r--   0 runner    (1001) docker     (123)   463711 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs/cdk_appflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:40.785606 cdklabs.cdk-appflow-0.0.3/src/cdklabs/cdk_appflow/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs/cdk_appflow/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   173440 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:34:26.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs/cdk_appflow/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:34:40.785606 cdklabs.cdk-appflow-0.0.3/src/cdklabs.cdk_appflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-22 00:34:40.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 00:34:40.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:34:40.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 00:34:40.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs.cdk_appflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 00:34:40.000000 cdklabs.cdk-appflow-0.0.3/src/cdklabs.cdk_appflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:33:04.048744 cdklabs.cdk-appflow-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-22 09:33:04.048744 cdklabs.cdk-appflow-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9014 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:33:04.048744 cdklabs.cdk-appflow-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:33:04.044744 cdklabs.cdk-appflow-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:33:04.044744 cdklabs.cdk-appflow-0.0.4/src/cdklabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:33:04.044744 cdklabs.cdk-appflow-0.0.4/src/cdklabs/cdk_appflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   504284 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs/cdk_appflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:33:04.048744 cdklabs.cdk-appflow-0.0.4/src/cdklabs/cdk_appflow/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs/cdk_appflow/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   179741 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs/cdk_appflow/_jsii/cdk-appflow@0.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:32:46.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs/cdk_appflow/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:33:04.044744 cdklabs.cdk-appflow-0.0.4/src/cdklabs.cdk_appflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-06-22 09:33:03.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs.cdk_appflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 09:33:04.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs.cdk_appflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:33:03.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs.cdk_appflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-22 09:33:03.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs.cdk_appflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 09:33:03.000000 cdklabs.cdk-appflow-0.0.4/src/cdklabs.cdk_appflow.egg-info/top_level.txt
```

### Comparing `cdklabs.cdk-appflow-0.0.3/LICENSE` & `cdklabs.cdk-appflow-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.3/PKG-INFO` & `cdklabs.cdk-appflow-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.3
+Version: 0.0.4
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdklabs.cdk-appflow-0.0.3/README.md` & `cdklabs.cdk-appflow-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdklabs.cdk-appflow-0.0.3/setup.py` & `cdklabs.cdk-appflow-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdklabs.cdk-appflow",
-    "version": "0.0.3",
+    "version": "0.0.4",
     "description": "@cdklabs/cdk-appflow",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-appflow.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdklabs.cdk_appflow",
         "cdklabs.cdk_appflow._jsii"
     ],
     "package_data": {
         "cdklabs.cdk_appflow._jsii": [
-            "cdk-appflow@0.0.3.jsii.tgz"
+            "cdk-appflow@0.0.4.jsii.tgz"
         ],
         "cdklabs.cdk_appflow": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdklabs.cdk-appflow-0.0.3/src/cdklabs/cdk_appflow/__init__.py` & `cdklabs.cdk-appflow-0.0.4/src/cdklabs/cdk_appflow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4135,14 +4135,681 @@
     def __repr__(self) -> str:
         return "S3SourceProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataBasicAuthSettings",
+    jsii_struct_bases=[],
+    name_mapping={"password": "password", "username": "username"},
+)
+class SAPOdataBasicAuthSettings:
+    def __init__(self, *, password: builtins.str, username: builtins.str) -> None:
+        '''
+        :param password: 
+        :param username: 
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ce4c0b0b2383996eec6cecc0c36fb286975bc25afe5c2b0daf63e6f4df264179)
+            check_type(argname="argument password", value=password, expected_type=type_hints["password"])
+            check_type(argname="argument username", value=username, expected_type=type_hints["username"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "password": password,
+            "username": username,
+        }
+
+    @builtins.property
+    def password(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("password")
+        assert result is not None, "Required property 'password' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def username(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("username")
+        assert result is not None, "Required property 'username' is missing"
+        return typing.cast(builtins.str, result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataBasicAuthSettings(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataConnectorProfileProps",
+    jsii_struct_bases=[ConnectorProfileProps],
+    name_mapping={
+        "key": "key",
+        "name": "name",
+        "application_host_url": "applicationHostUrl",
+        "application_service_path": "applicationServicePath",
+        "client_number": "clientNumber",
+        "logon_language": "logonLanguage",
+        "basic_auth": "basicAuth",
+        "o_auth": "oAuth",
+        "port_number": "portNumber",
+    },
+)
+class SAPOdataConnectorProfileProps(ConnectorProfileProps):
+    def __init__(
+        self,
+        *,
+        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        name: typing.Optional[builtins.str] = None,
+        application_host_url: builtins.str,
+        application_service_path: builtins.str,
+        client_number: builtins.str,
+        logon_language: builtins.str,
+        basic_auth: typing.Optional[typing.Union[SAPOdataBasicAuthSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        o_auth: typing.Optional[typing.Union["SAPOdataOAuthSettings", typing.Dict[builtins.str, typing.Any]]] = None,
+        port_number: typing.Optional[jsii.Number] = None,
+    ) -> None:
+        '''
+        :param key: (experimental) TODO: think if this should be here as not all connector profiles have that.
+        :param name: 
+        :param application_host_url: 
+        :param application_service_path: 
+        :param client_number: 
+        :param logon_language: 
+        :param basic_auth: 
+        :param o_auth: 
+        :param port_number: 
+
+        :stability: experimental
+        '''
+        if isinstance(basic_auth, dict):
+            basic_auth = SAPOdataBasicAuthSettings(**basic_auth)
+        if isinstance(o_auth, dict):
+            o_auth = SAPOdataOAuthSettings(**o_auth)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c30df13ceca2f1ff215e11a4e86a5f6bd8a1245b181c59827c0daa29e8f90072)
+            check_type(argname="argument key", value=key, expected_type=type_hints["key"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+            check_type(argname="argument application_host_url", value=application_host_url, expected_type=type_hints["application_host_url"])
+            check_type(argname="argument application_service_path", value=application_service_path, expected_type=type_hints["application_service_path"])
+            check_type(argname="argument client_number", value=client_number, expected_type=type_hints["client_number"])
+            check_type(argname="argument logon_language", value=logon_language, expected_type=type_hints["logon_language"])
+            check_type(argname="argument basic_auth", value=basic_auth, expected_type=type_hints["basic_auth"])
+            check_type(argname="argument o_auth", value=o_auth, expected_type=type_hints["o_auth"])
+            check_type(argname="argument port_number", value=port_number, expected_type=type_hints["port_number"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "application_host_url": application_host_url,
+            "application_service_path": application_service_path,
+            "client_number": client_number,
+            "logon_language": logon_language,
+        }
+        if key is not None:
+            self._values["key"] = key
+        if name is not None:
+            self._values["name"] = name
+        if basic_auth is not None:
+            self._values["basic_auth"] = basic_auth
+        if o_auth is not None:
+            self._values["o_auth"] = o_auth
+        if port_number is not None:
+            self._values["port_number"] = port_number
+
+    @builtins.property
+    def key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+        '''(experimental) TODO: think if this should be here as not all connector profiles have that.
+
+        :stability: experimental
+        '''
+        result = self._values.get("key")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+
+    @builtins.property
+    def name(self) -> typing.Optional[builtins.str]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def application_host_url(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("application_host_url")
+        assert result is not None, "Required property 'application_host_url' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def application_service_path(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("application_service_path")
+        assert result is not None, "Required property 'application_service_path' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def client_number(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("client_number")
+        assert result is not None, "Required property 'client_number' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def logon_language(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("logon_language")
+        assert result is not None, "Required property 'logon_language' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def basic_auth(self) -> typing.Optional[SAPOdataBasicAuthSettings]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("basic_auth")
+        return typing.cast(typing.Optional[SAPOdataBasicAuthSettings], result)
+
+    @builtins.property
+    def o_auth(self) -> typing.Optional["SAPOdataOAuthSettings"]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("o_auth")
+        return typing.cast(typing.Optional["SAPOdataOAuthSettings"], result)
+
+    @builtins.property
+    def port_number(self) -> typing.Optional[jsii.Number]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("port_number")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataConnectorProfileProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataDestinationProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "object": "object",
+        "operation": "operation",
+        "profile": "profile",
+        "error_handling": "errorHandling",
+        "success_response_handling": "successResponseHandling",
+    },
+)
+class SAPOdataDestinationProps:
+    def __init__(
+        self,
+        *,
+        object: builtins.str,
+        operation: "WriteOperation",
+        profile: "SAPOdataConnectorProfile",
+        error_handling: typing.Optional[typing.Union[ErrorHandlingConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+        success_response_handling: typing.Optional[typing.Union["SAPOdataSuccessResponseHandlingConfiguration", typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param object: (experimental) The SAPOdata object for which the operation is to be set.
+        :param operation: 
+        :param profile: 
+        :param error_handling: (experimental) The settings that determine how Amazon AppFlow handles an error when placing data in the SAPOdata destination. For example, this setting would determine if the flow should fail after one insertion error, or continue and attempt to insert every record regardless of the initial failure.
+        :param success_response_handling: 
+
+        :stability: experimental
+        '''
+        if isinstance(error_handling, dict):
+            error_handling = ErrorHandlingConfiguration(**error_handling)
+        if isinstance(success_response_handling, dict):
+            success_response_handling = SAPOdataSuccessResponseHandlingConfiguration(**success_response_handling)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__d90d6697fd4914c63c12e96e1fa677de8b617deda9d68e06597a1162de72ff46)
+            check_type(argname="argument object", value=object, expected_type=type_hints["object"])
+            check_type(argname="argument operation", value=operation, expected_type=type_hints["operation"])
+            check_type(argname="argument profile", value=profile, expected_type=type_hints["profile"])
+            check_type(argname="argument error_handling", value=error_handling, expected_type=type_hints["error_handling"])
+            check_type(argname="argument success_response_handling", value=success_response_handling, expected_type=type_hints["success_response_handling"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "object": object,
+            "operation": operation,
+            "profile": profile,
+        }
+        if error_handling is not None:
+            self._values["error_handling"] = error_handling
+        if success_response_handling is not None:
+            self._values["success_response_handling"] = success_response_handling
+
+    @builtins.property
+    def object(self) -> builtins.str:
+        '''(experimental) The SAPOdata object for which the operation is to be set.
+
+        :stability: experimental
+        '''
+        result = self._values.get("object")
+        assert result is not None, "Required property 'object' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def operation(self) -> "WriteOperation":
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("operation")
+        assert result is not None, "Required property 'operation' is missing"
+        return typing.cast("WriteOperation", result)
+
+    @builtins.property
+    def profile(self) -> "SAPOdataConnectorProfile":
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("profile")
+        assert result is not None, "Required property 'profile' is missing"
+        return typing.cast("SAPOdataConnectorProfile", result)
+
+    @builtins.property
+    def error_handling(self) -> typing.Optional[ErrorHandlingConfiguration]:
+        '''(experimental) The settings that determine how Amazon AppFlow handles an error when placing data in the SAPOdata destination.
+
+        For example, this setting would determine if the flow should fail after one insertion error, or continue and attempt to insert every record regardless of the initial failure.
+
+        :stability: experimental
+        '''
+        result = self._values.get("error_handling")
+        return typing.cast(typing.Optional[ErrorHandlingConfiguration], result)
+
+    @builtins.property
+    def success_response_handling(
+        self,
+    ) -> typing.Optional["SAPOdataSuccessResponseHandlingConfiguration"]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("success_response_handling")
+        return typing.cast(typing.Optional["SAPOdataSuccessResponseHandlingConfiguration"], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataDestinationProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataOAuthEndpoints",
+    jsii_struct_bases=[],
+    name_mapping={"token": "token"},
+)
+class SAPOdataOAuthEndpoints:
+    def __init__(self, *, token: builtins.str) -> None:
+        '''
+        :param token: 
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__da515d0d4648ceb542f575c8c56866e2466cb923c70d677cbc3a707ef221ccf4)
+            check_type(argname="argument token", value=token, expected_type=type_hints["token"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "token": token,
+        }
+
+    @builtins.property
+    def token(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("token")
+        assert result is not None, "Required property 'token' is missing"
+        return typing.cast(builtins.str, result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataOAuthEndpoints(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataOAuthFlows",
+    jsii_struct_bases=[],
+    name_mapping={"refresh_token_grant": "refreshTokenGrant"},
+)
+class SAPOdataOAuthFlows:
+    def __init__(
+        self,
+        *,
+        refresh_token_grant: typing.Union["SAPOdataOAuthRefreshTokenGrantFlow", typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''
+        :param refresh_token_grant: 
+
+        :stability: experimental
+        '''
+        if isinstance(refresh_token_grant, dict):
+            refresh_token_grant = SAPOdataOAuthRefreshTokenGrantFlow(**refresh_token_grant)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__cefed30b945239087f3dbb8a1ddb5dabb6307d3d35e04ede5e4a6887f6d0d581)
+            check_type(argname="argument refresh_token_grant", value=refresh_token_grant, expected_type=type_hints["refresh_token_grant"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "refresh_token_grant": refresh_token_grant,
+        }
+
+    @builtins.property
+    def refresh_token_grant(self) -> "SAPOdataOAuthRefreshTokenGrantFlow":
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("refresh_token_grant")
+        assert result is not None, "Required property 'refresh_token_grant' is missing"
+        return typing.cast("SAPOdataOAuthRefreshTokenGrantFlow", result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataOAuthFlows(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataOAuthRefreshTokenGrantFlow",
+    jsii_struct_bases=[],
+    name_mapping={
+        "client_id": "clientId",
+        "client_secret": "clientSecret",
+        "refresh_token": "refreshToken",
+    },
+)
+class SAPOdataOAuthRefreshTokenGrantFlow:
+    def __init__(
+        self,
+        *,
+        client_id: builtins.str,
+        client_secret: builtins.str,
+        refresh_token: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param client_id: 
+        :param client_secret: 
+        :param refresh_token: 
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__fff92b1fecd8fb687b0fb4bdc1411cb80fac93d1dfb20791ff4b5c327fd3b240)
+            check_type(argname="argument client_id", value=client_id, expected_type=type_hints["client_id"])
+            check_type(argname="argument client_secret", value=client_secret, expected_type=type_hints["client_secret"])
+            check_type(argname="argument refresh_token", value=refresh_token, expected_type=type_hints["refresh_token"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "client_id": client_id,
+            "client_secret": client_secret,
+        }
+        if refresh_token is not None:
+            self._values["refresh_token"] = refresh_token
+
+    @builtins.property
+    def client_id(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("client_id")
+        assert result is not None, "Required property 'client_id' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def client_secret(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("client_secret")
+        assert result is not None, "Required property 'client_secret' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def refresh_token(self) -> typing.Optional[builtins.str]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("refresh_token")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataOAuthRefreshTokenGrantFlow(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataOAuthSettings",
+    jsii_struct_bases=[],
+    name_mapping={
+        "access_token": "accessToken",
+        "endpoints": "endpoints",
+        "flow": "flow",
+    },
+)
+class SAPOdataOAuthSettings:
+    def __init__(
+        self,
+        *,
+        access_token: typing.Optional[builtins.str] = None,
+        endpoints: typing.Optional[typing.Union[SAPOdataOAuthEndpoints, typing.Dict[builtins.str, typing.Any]]] = None,
+        flow: typing.Optional[typing.Union[SAPOdataOAuthFlows, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param access_token: 
+        :param endpoints: 
+        :param flow: 
+
+        :stability: experimental
+        '''
+        if isinstance(endpoints, dict):
+            endpoints = SAPOdataOAuthEndpoints(**endpoints)
+        if isinstance(flow, dict):
+            flow = SAPOdataOAuthFlows(**flow)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__e6c602c5338ef47ca8f8b846c7354c60a34e2b2a3c774b4e8c0581d482e6294f)
+            check_type(argname="argument access_token", value=access_token, expected_type=type_hints["access_token"])
+            check_type(argname="argument endpoints", value=endpoints, expected_type=type_hints["endpoints"])
+            check_type(argname="argument flow", value=flow, expected_type=type_hints["flow"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if access_token is not None:
+            self._values["access_token"] = access_token
+        if endpoints is not None:
+            self._values["endpoints"] = endpoints
+        if flow is not None:
+            self._values["flow"] = flow
+
+    @builtins.property
+    def access_token(self) -> typing.Optional[builtins.str]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("access_token")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def endpoints(self) -> typing.Optional[SAPOdataOAuthEndpoints]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("endpoints")
+        return typing.cast(typing.Optional[SAPOdataOAuthEndpoints], result)
+
+    @builtins.property
+    def flow(self) -> typing.Optional[SAPOdataOAuthFlows]:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("flow")
+        return typing.cast(typing.Optional[SAPOdataOAuthFlows], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataOAuthSettings(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataSourceProps",
+    jsii_struct_bases=[],
+    name_mapping={"object": "object", "profile": "profile"},
+)
+class SAPOdataSourceProps:
+    def __init__(
+        self,
+        *,
+        object: builtins.str,
+        profile: "SAPOdataConnectorProfile",
+    ) -> None:
+        '''
+        :param object: 
+        :param profile: 
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__46c8000b7de41ff27d29d18565fcd6f07d4e7be2d898c826689b0a5ee0cc9835)
+            check_type(argname="argument object", value=object, expected_type=type_hints["object"])
+            check_type(argname="argument profile", value=profile, expected_type=type_hints["profile"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "object": object,
+            "profile": profile,
+        }
+
+    @builtins.property
+    def object(self) -> builtins.str:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("object")
+        assert result is not None, "Required property 'object' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def profile(self) -> "SAPOdataConnectorProfile":
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("profile")
+        assert result is not None, "Required property 'profile' is missing"
+        return typing.cast("SAPOdataConnectorProfile", result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataSourceProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataSuccessResponseHandlingConfiguration",
+    jsii_struct_bases=[],
+    name_mapping={"location": "location"},
+)
+class SAPOdataSuccessResponseHandlingConfiguration:
+    def __init__(
+        self,
+        *,
+        location: typing.Union[S3Location, typing.Dict[builtins.str, typing.Any]],
+    ) -> None:
+        '''
+        :param location: 
+
+        :stability: experimental
+        '''
+        if isinstance(location, dict):
+            location = S3Location(**location)
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__81ed6c082cacef689ea56d955987bb16bb38ebfbc22ac5a9953c1609643d6ef5)
+            check_type(argname="argument location", value=location, expected_type=type_hints["location"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "location": location,
+        }
+
+    @builtins.property
+    def location(self) -> S3Location:
+        '''
+        :stability: experimental
+        '''
+        result = self._values.get("location")
+        assert result is not None, "Required property 'location' is missing"
+        return typing.cast(S3Location, result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "SAPOdataSuccessResponseHandlingConfiguration(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="@cdklabs/cdk-appflow.SalesforceConnectorProfileProps",
     jsii_struct_bases=[ConnectorProfileProps],
     name_mapping={
         "key": "key",
         "name": "name",
         "instance_url": "instanceUrl",
         "o_auth": "oAuth",
@@ -8984,14 +9651,262 @@
         '''(experimental) The AppFlow type of the connector that this source is implemented for.
 
         :stability: experimental
         '''
         return typing.cast(ConnectorType, jsii.get(self, "connectorType"))
 
 
+class SAPOdataConnectorProfile(
+    ConnectorProfileBase,
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataConnectorProfile",
+):
+    '''
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        application_host_url: builtins.str,
+        application_service_path: builtins.str,
+        client_number: builtins.str,
+        logon_language: builtins.str,
+        basic_auth: typing.Optional[typing.Union[SAPOdataBasicAuthSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        o_auth: typing.Optional[typing.Union[SAPOdataOAuthSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+        port_number: typing.Optional[jsii.Number] = None,
+        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        name: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param scope: -
+        :param id: -
+        :param application_host_url: 
+        :param application_service_path: 
+        :param client_number: 
+        :param logon_language: 
+        :param basic_auth: 
+        :param o_auth: 
+        :param port_number: 
+        :param key: (experimental) TODO: think if this should be here as not all connector profiles have that.
+        :param name: 
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__1456a6c00e75acdfb46d10ac9e74fd8a326dbbb53336209c40da1bf1772dc678)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = SAPOdataConnectorProfileProps(
+            application_host_url=application_host_url,
+            application_service_path=application_service_path,
+            client_number=client_number,
+            logon_language=logon_language,
+            basic_auth=basic_auth,
+            o_auth=o_auth,
+            port_number=port_number,
+            key=key,
+            name=name,
+        )
+
+        jsii.create(self.__class__, self, [scope, id, props])
+
+    @jsii.member(jsii_name="fromConnectionProfileArn")
+    @builtins.classmethod
+    def from_connection_profile_arn(
+        cls,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        arn: builtins.str,
+    ) -> "SAPOdataConnectorProfile":
+        '''
+        :param scope: -
+        :param id: -
+        :param arn: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__8a6386649257a15b140d1f567e872eeeee4f4afe56bbb09734eb8b164e005830)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument arn", value=arn, expected_type=type_hints["arn"])
+        return typing.cast("SAPOdataConnectorProfile", jsii.sinvoke(cls, "fromConnectionProfileArn", [scope, id, arn]))
+
+    @jsii.member(jsii_name="fromConnectionProfileName")
+    @builtins.classmethod
+    def from_connection_profile_name(
+        cls,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        name: builtins.str,
+    ) -> "SAPOdataConnectorProfile":
+        '''
+        :param scope: -
+        :param id: -
+        :param name: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__65d328d60d5002bf9c8a09117a27e9b1e946b48879e17ad76aba5c6fd23857c8)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+            check_type(argname="argument name", value=name, expected_type=type_hints["name"])
+        return typing.cast("SAPOdataConnectorProfile", jsii.sinvoke(cls, "fromConnectionProfileName", [scope, id, name]))
+
+    @jsii.member(jsii_name="buildConnectorProfileCredentials")
+    def _build_connector_profile_credentials(
+        self,
+        *,
+        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        name: typing.Optional[builtins.str] = None,
+    ) -> _aws_cdk_aws_appflow_ceddda9d.CfnConnectorProfile.ConnectorProfileCredentialsProperty:
+        '''
+        :param key: (experimental) TODO: think if this should be here as not all connector profiles have that.
+        :param name: 
+
+        :stability: experimental
+        '''
+        props = ConnectorProfileProps(key=key, name=name)
+
+        return typing.cast(_aws_cdk_aws_appflow_ceddda9d.CfnConnectorProfile.ConnectorProfileCredentialsProperty, jsii.invoke(self, "buildConnectorProfileCredentials", [props]))
+
+    @jsii.member(jsii_name="buildConnectorProfileProperties")
+    def _build_connector_profile_properties(
+        self,
+        *,
+        key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        name: typing.Optional[builtins.str] = None,
+    ) -> _aws_cdk_aws_appflow_ceddda9d.CfnConnectorProfile.ConnectorProfilePropertiesProperty:
+        '''
+        :param key: (experimental) TODO: think if this should be here as not all connector profiles have that.
+        :param name: 
+
+        :stability: experimental
+        '''
+        props = ConnectorProfileProps(key=key, name=name)
+
+        return typing.cast(_aws_cdk_aws_appflow_ceddda9d.CfnConnectorProfile.ConnectorProfilePropertiesProperty, jsii.invoke(self, "buildConnectorProfileProperties", [props]))
+
+
+@jsii.implements(IDestination)
+class SAPOdataDestination(
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataDestination",
+):
+    '''
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        *,
+        object: builtins.str,
+        operation: WriteOperation,
+        profile: SAPOdataConnectorProfile,
+        error_handling: typing.Optional[typing.Union[ErrorHandlingConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+        success_response_handling: typing.Optional[typing.Union[SAPOdataSuccessResponseHandlingConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+    ) -> None:
+        '''
+        :param object: (experimental) The SAPOdata object for which the operation is to be set.
+        :param operation: 
+        :param profile: 
+        :param error_handling: (experimental) The settings that determine how Amazon AppFlow handles an error when placing data in the SAPOdata destination. For example, this setting would determine if the flow should fail after one insertion error, or continue and attempt to insert every record regardless of the initial failure.
+        :param success_response_handling: 
+
+        :stability: experimental
+        '''
+        props = SAPOdataDestinationProps(
+            object=object,
+            operation=operation,
+            profile=profile,
+            error_handling=error_handling,
+            success_response_handling=success_response_handling,
+        )
+
+        jsii.create(self.__class__, self, [props])
+
+    @jsii.member(jsii_name="bind")
+    def bind(
+        self,
+        flow: IFlow,
+    ) -> _aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty:
+        '''
+        :param flow: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__be9c75208a53ebc4db44ac27cc9aaac34a0b9ac8e574e73ff8a4a30fa1b7b46c)
+            check_type(argname="argument flow", value=flow, expected_type=type_hints["flow"])
+        return typing.cast(_aws_cdk_aws_appflow_ceddda9d.CfnFlow.DestinationFlowConfigProperty, jsii.invoke(self, "bind", [flow]))
+
+    @builtins.property
+    @jsii.member(jsii_name="connectorType")
+    def connector_type(self) -> ConnectorType:
+        '''(experimental) The AppFlow type of the connector that this source is implemented for.
+
+        :stability: experimental
+        '''
+        return typing.cast(ConnectorType, jsii.get(self, "connectorType"))
+
+
+@jsii.implements(ISource)
+class SAPOdataSource(
+    metaclass=jsii.JSIIMeta,
+    jsii_type="@cdklabs/cdk-appflow.SAPOdataSource",
+):
+    '''
+    :stability: experimental
+    '''
+
+    def __init__(
+        self,
+        *,
+        object: builtins.str,
+        profile: SAPOdataConnectorProfile,
+    ) -> None:
+        '''
+        :param object: 
+        :param profile: 
+
+        :stability: experimental
+        '''
+        props = SAPOdataSourceProps(object=object, profile=profile)
+
+        jsii.create(self.__class__, self, [props])
+
+    @jsii.member(jsii_name="bind")
+    def bind(
+        self,
+        flow: IFlow,
+    ) -> _aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty:
+        '''
+        :param flow: -
+
+        :stability: experimental
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__0026fc92ed92f4c9cabaa7c920e2d283ecacf980920ee014d8bef28dfb74a01a)
+            check_type(argname="argument flow", value=flow, expected_type=type_hints["flow"])
+        return typing.cast(_aws_cdk_aws_appflow_ceddda9d.CfnFlow.SourceFlowConfigProperty, jsii.invoke(self, "bind", [flow]))
+
+    @builtins.property
+    @jsii.member(jsii_name="connectorType")
+    def connector_type(self) -> ConnectorType:
+        '''(experimental) The AppFlow type of the connector that this source is implemented for.
+
+        :stability: experimental
+        '''
+        return typing.cast(ConnectorType, jsii.get(self, "connectorType"))
+
+
 class SalesforceConnectorProfile(
     ConnectorProfileBase,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdklabs/cdk-appflow.SalesforceConnectorProfile",
 ):
     '''
     :stability: experimental
@@ -10494,14 +11409,26 @@
     "S3OutputFilePrefixFormat",
     "S3OutputFilePrefixHierarchy",
     "S3OutputFilePrefixType",
     "S3OutputFileType",
     "S3OutputFormatting",
     "S3Source",
     "S3SourceProps",
+    "SAPOdataBasicAuthSettings",
+    "SAPOdataConnectorProfile",
+    "SAPOdataConnectorProfileProps",
+    "SAPOdataDestination",
+    "SAPOdataDestinationProps",
+    "SAPOdataOAuthEndpoints",
+    "SAPOdataOAuthFlows",
+    "SAPOdataOAuthRefreshTokenGrantFlow",
+    "SAPOdataOAuthSettings",
+    "SAPOdataSource",
+    "SAPOdataSourceProps",
+    "SAPOdataSuccessResponseHandlingConfiguration",
     "SalesforceConnectorProfile",
     "SalesforceConnectorProfileProps",
     "SalesforceDataTransferApi",
     "SalesforceDestination",
     "SalesforceDestinationProps",
     "SalesforceMarketingCloudApiVersions",
     "SalesforceMarketingCloudConnectorProfile",
@@ -11086,14 +12013,95 @@
     bucket: _aws_cdk_aws_s3_ceddda9d.IBucket,
     prefix: builtins.str,
     format: typing.Optional[typing.Union[S3InputFormat, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__ce4c0b0b2383996eec6cecc0c36fb286975bc25afe5c2b0daf63e6f4df264179(
+    *,
+    password: builtins.str,
+    username: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c30df13ceca2f1ff215e11a4e86a5f6bd8a1245b181c59827c0daa29e8f90072(
+    *,
+    key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    name: typing.Optional[builtins.str] = None,
+    application_host_url: builtins.str,
+    application_service_path: builtins.str,
+    client_number: builtins.str,
+    logon_language: builtins.str,
+    basic_auth: typing.Optional[typing.Union[SAPOdataBasicAuthSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+    o_auth: typing.Optional[typing.Union[SAPOdataOAuthSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+    port_number: typing.Optional[jsii.Number] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__d90d6697fd4914c63c12e96e1fa677de8b617deda9d68e06597a1162de72ff46(
+    *,
+    object: builtins.str,
+    operation: WriteOperation,
+    profile: SAPOdataConnectorProfile,
+    error_handling: typing.Optional[typing.Union[ErrorHandlingConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+    success_response_handling: typing.Optional[typing.Union[SAPOdataSuccessResponseHandlingConfiguration, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__da515d0d4648ceb542f575c8c56866e2466cb923c70d677cbc3a707ef221ccf4(
+    *,
+    token: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cefed30b945239087f3dbb8a1ddb5dabb6307d3d35e04ede5e4a6887f6d0d581(
+    *,
+    refresh_token_grant: typing.Union[SAPOdataOAuthRefreshTokenGrantFlow, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__fff92b1fecd8fb687b0fb4bdc1411cb80fac93d1dfb20791ff4b5c327fd3b240(
+    *,
+    client_id: builtins.str,
+    client_secret: builtins.str,
+    refresh_token: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__e6c602c5338ef47ca8f8b846c7354c60a34e2b2a3c774b4e8c0581d482e6294f(
+    *,
+    access_token: typing.Optional[builtins.str] = None,
+    endpoints: typing.Optional[typing.Union[SAPOdataOAuthEndpoints, typing.Dict[builtins.str, typing.Any]]] = None,
+    flow: typing.Optional[typing.Union[SAPOdataOAuthFlows, typing.Dict[builtins.str, typing.Any]]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__46c8000b7de41ff27d29d18565fcd6f07d4e7be2d898c826689b0a5ee0cc9835(
+    *,
+    object: builtins.str,
+    profile: SAPOdataConnectorProfile,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__81ed6c082cacef689ea56d955987bb16bb38ebfbc22ac5a9953c1609643d6ef5(
+    *,
+    location: typing.Union[S3Location, typing.Dict[builtins.str, typing.Any]],
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__eb386fe4c6e6ec8ddee55dea0effc0a7bd692124b527bb2ffbb3554ffd2a04ee(
     *,
     key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
     name: typing.Optional[builtins.str] = None,
     instance_url: builtins.str,
     o_auth: typing.Union[SalesforceOAuthSettings, typing.Dict[builtins.str, typing.Any]],
     is_sandbox: typing.Optional[builtins.bool] = None,
@@ -11868,14 +12876,59 @@
 
 def _typecheckingstub__a1e09e5f5312a9f8751cf5ce9d37ff5134334869d46594888883266c8504ea46(
     scope: IFlow,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__1456a6c00e75acdfb46d10ac9e74fd8a326dbbb53336209c40da1bf1772dc678(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    application_host_url: builtins.str,
+    application_service_path: builtins.str,
+    client_number: builtins.str,
+    logon_language: builtins.str,
+    basic_auth: typing.Optional[typing.Union[SAPOdataBasicAuthSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+    o_auth: typing.Optional[typing.Union[SAPOdataOAuthSettings, typing.Dict[builtins.str, typing.Any]]] = None,
+    port_number: typing.Optional[jsii.Number] = None,
+    key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    name: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__8a6386649257a15b140d1f567e872eeeee4f4afe56bbb09734eb8b164e005830(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    arn: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__65d328d60d5002bf9c8a09117a27e9b1e946b48879e17ad76aba5c6fd23857c8(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    name: builtins.str,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__be9c75208a53ebc4db44ac27cc9aaac34a0b9ac8e574e73ff8a4a30fa1b7b46c(
+    flow: IFlow,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__0026fc92ed92f4c9cabaa7c920e2d283ecacf980920ee014d8bef28dfb74a01a(
+    flow: IFlow,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__971cdd11384ff73d58d6d421eac3224b366d50d8ce1505049b566c9100872982(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     instance_url: builtins.str,
     o_auth: typing.Union[SalesforceOAuthSettings, typing.Dict[builtins.str, typing.Any]],
     is_sandbox: typing.Optional[builtins.bool] = None,
```

### Comparing `cdklabs.cdk-appflow-0.0.3/src/cdklabs.cdk_appflow.egg-info/PKG-INFO` & `cdklabs.cdk-appflow-0.0.4/src/cdklabs.cdk_appflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdklabs.cdk-appflow
-Version: 0.0.3
+Version: 0.0.4
 Summary: @cdklabs/cdk-appflow
 Home-page: https://github.com/cdklabs/cdk-appflow.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-appflow.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

