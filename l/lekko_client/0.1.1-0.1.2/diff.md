# Comparing `tmp/lekko_client-0.1.1.tar.gz` & `tmp/lekko_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lekko_client-0.1.1.tar", last modified: Tue Jun 13 19:53:15 2023, max compression
+gzip compressed data, was "lekko_client-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lekko_client-0.1.1.tar` & `lekko_client-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1127 2023-05-03 23:03:04.216499 lekko_client-0.1.1/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     3078 2023-04-21 20:20:24.420901 lekko_client-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2023-04-21 20:20:24.421086 lekko_client-0.1.1/LICENSE
--rw-r--r--   0        0        0      607 2023-05-03 23:03:04.216872 lekko_client-0.1.1/Makefile
--rw-r--r--   0        0        0       12 2023-04-21 20:20:24.421180 lekko_client-0.1.1/README.md
--rw-r--r--   0        0        0      233 2023-05-03 18:55:48.352789 lekko_client-0.1.1/buf.gen.yaml
--rw-r--r--   0        0        0     2368 2023-05-28 18:43:00.488488 lekko_client-0.1.1/example.py
--rw-r--r--   0        0        0      245 2023-06-13 19:52:16.322836 lekko_client-0.1.1/lekko_client/__init__.py
--rw-r--r--   0        0        0     7353 2023-05-03 22:29:42.588741 lekko_client-0.1.1/lekko_client/client.py
--rw-r--r--   0        0        0      279 2023-05-03 18:55:48.354020 lekko_client-0.1.1/lekko_client/exceptions.py
--rw-r--r--   0        0        0     9857 2023-05-03 21:16:43.938055 lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py
--rw-r--r--   0        0        0    18544 2023-05-03 20:42:34.599769 lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi
--rw-r--r--   0        0        0    16283 2023-05-03 21:16:43.938327 lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py
--rw-r--r--   0        0        0     1761 2023-05-31 18:07:52.219437 lekko_client-0.1.1/lekko_client/helpers.py
--rw-r--r--   0        0        0      753 2023-05-28 18:42:56.475381 lekko_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       61 2023-04-26 23:47:06.221249 lekko_client-0.1.1/requirements.txt
--rw-r--r--   0        0        0     2086 2023-05-28 18:50:58.132098 lekko_client-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1888 2023-05-03 18:55:48.355229 lekko_client-0.1.1/tests/mock_server.py
--rw-r--r--   0        0        0       40 2023-05-03 18:55:48.355400 lekko_client-0.1.1/tests/requirements.txt
--rw-r--r--   0        0        0     2456 2023-05-31 18:07:52.219638 lekko_client-0.1.1/tests/test_client.py
--rw-r--r--   0        0        0      913 2023-05-03 23:03:04.217147 lekko_client-0.1.1/tox.ini
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 lekko_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1194 2023-06-22 00:22:58.664693 lekko_client-0.1.2/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     3078 2023-05-05 21:12:44.881820 lekko_client-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2023-05-05 21:12:44.881972 lekko_client-0.1.2/LICENSE
+-rw-r--r--   0        0        0      644 2023-06-21 18:36:15.400750 lekko_client-0.1.2/Makefile
+-rw-r--r--   0        0        0      147 2023-06-21 18:36:15.400875 lekko_client-0.1.2/README.md
+-rw-r--r--   0        0        0      233 2023-05-05 21:12:44.882244 lekko_client-0.1.2/buf.gen.yaml
+-rw-r--r--   0        0        0     2368 2023-06-09 21:08:10.443431 lekko_client-0.1.2/example.py
+-rw-r--r--   0        0        0      245 2023-06-22 20:34:21.499893 lekko_client-0.1.2/lekko_client/__init__.py
+-rw-r--r--   0        0        0     8129 2023-06-22 00:22:58.665259 lekko_client-0.1.2/lekko_client/client.py
+-rw-r--r--   0        0        0      279 2023-05-05 21:12:44.882685 lekko_client-0.1.2/lekko_client/exceptions.py
+-rw-r--r--   0        0        0    10136 2023-06-22 00:22:58.665633 lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py
+-rw-r--r--   0        0        0    19270 2023-06-22 00:22:58.665913 lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi
+-rw-r--r--   0        0        0    16283 2023-06-21 18:37:43.929549 lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1761 2023-06-09 21:40:27.116943 lekko_client-0.1.2/lekko_client/helpers.py
+-rw-r--r--   0        0        0      753 2023-05-05 21:12:44.883532 lekko_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-05-05 21:12:44.883614 lekko_client-0.1.2/requirements.txt
+-rw-r--r--   0        0        0     3397 2023-06-21 18:36:15.401775 lekko_client-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     1888 2023-05-05 21:12:44.883843 lekko_client-0.1.2/tests/mock_server.py
+-rw-r--r--   0        0        0       40 2023-05-05 21:12:44.883918 lekko_client-0.1.2/tests/requirements.txt
+-rw-r--r--   0        0        0     8323 2023-06-22 00:22:58.666197 lekko_client-0.1.2/tests/test_client.py
+-rw-r--r--   0        0        0     1546 2023-06-21 18:36:15.402106 lekko_client-0.1.2/tox.ini
+-rw-r--r--   0        0        0      635 1970-01-01 00:00:00.000000 lekko_client-0.1.2/PKG-INFO
```

### Comparing `lekko_client-0.1.1/.github/workflows/ci.yaml` & `lekko_client-0.1.2/.github/workflows/ci.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     branches:
       - main
 
 jobs:
   lint:
     name: Lint
     runs-on: ubuntu-latest
+    timeout-minutes: 10
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python 3
         uses: actions/setup-python@v4
         with:
           python-version: "3.11"
           cache: 'pip'
@@ -25,27 +26,28 @@
       - name: lint
         run: make lint
       - name: typecheck
         run: make typecheck
 
   test:
     runs-on: ubuntu-latest
-    strategy:
-      matrix:
-        python-version: ['3.9', '3.10', '3.11']
-
+    timeout-minutes: 10
     steps:
       - uses: actions/checkout@v3
-      - name: Set up Python ${{ matrix.python-version }}
+      - name: Set up Python 3.x
         uses: actions/setup-python@v4
         with:
-          python-version: ${{ matrix.python-version }}
+          python-version: "3.x"
           cache: 'pip'
           cache-dependency-path: |
             pyproject.toml
             tox.ini
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
-          python -m pip install tox tox-gh-actions
+          python -m pip install tox
       - name: Test with tox
-        run: tox
+        run:  PYTHONPATH=. tox -p auto
+      - name: Upload coverage report
+        uses: codecov/codecov-action@v3
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `lekko_client-0.1.1/.gitignore` & `lekko_client-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.1/LICENSE` & `lekko_client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.1/Makefile` & `lekko_client-0.1.2/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 venv/bin/touchfile: pyproject.toml
 	@test -d venv || ${PYTHON} -m venv venv
 	. venv/bin/activate; pip install .[dev]
 	@touch venv/bin/touchfile
 
 .PHONY: test
 test: venv
-	venv/bin/tox -p auto
+	PYTHONPATH=. venv/bin/tox -p auto
+	venv/bin/tox -e report
 
 .PHONY: lint
 lint: venv
 	venv/bin/tox -e lint
 
 .PHONY: typecheck
 typecheck: venv
```

### Comparing `lekko_client-0.1.1/example.py` & `lekko_client-0.1.2/example.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.1/lekko_client/client.py` & `lekko_client-0.1.2/lekko_client/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,48 +48,48 @@
         self.namespace = namespace
         self.context = context or {}
 
         self.api_key = api_key or os.environ.get("LEKKO_API_KEY")
 
     @abstractmethod
     def get_bool(self, key: str, context: Dict[str, Any]) -> bool:
-        raise NotImplementedError
+        ...
 
     @abstractmethod
     def get_int(self, key: str, context: Dict[str, Any]) -> int:
-        raise NotImplementedError
+        ...
 
     @abstractmethod
     def get_float(self, key: str, context: Dict[str, Any]) -> float:
-        raise NotImplementedError
+        ...
 
     @abstractmethod
     def get_string(self, key: str, context: Dict[str, Any]) -> str:
-        raise NotImplementedError
+        ...
 
     @abstractmethod
     def get_json(self, key: str, context: Dict[str, Any]) -> dict:
-        pass
+        ...
 
     @abstractmethod
     def get_proto(
         self,
         key: str,
         context: Dict[str, Any],
     ) -> ProtoMessage:
-        pass
+        ...
 
     @abstractmethod
     def get_proto_by_type(
         self,
         key: str,
         context: Dict[str, Any],
         proto_message_type: Type[ProtoType],
     ) -> ProtoType:
-        pass
+        ...
 
 
 class GRPCClient(Client):
     _channels: Dict[Tuple[str, str], grpc.Channel] = {}
 
     class JsonBytes(bytes):
         pass
@@ -148,15 +148,15 @@
         return self._get(key, context, str)
 
     def get_json(self, key: str, context: Dict[str, Any]) -> dict:
         json_bytes = self._get(key, context, GRPCClient.JsonBytes)
         return json.loads(json_bytes.decode("utf-8"))
 
     def get_proto(self, key: str, context: Dict[str, Any]) -> ProtoMessage:
-        val = self._get(key, context, AnyProto)
+        val = self._get_proto(key, context)
         db = proto_symbol_database.SymbolDatabase(pool=proto_descriptor_pool.Default())
         try:
             ret_val = db.GetSymbol(val.type_url.split("/")[1])()
             if val.Unpack(ret_val):
                 return ret_val
         except (KeyError, IndexError):
             pass
@@ -164,15 +164,15 @@
 
     def get_proto_by_type(
         self,
         key: str,
         context: Dict[str, Any],
         proto_message_type: Type[Client.ProtoType],
     ) -> Client.ProtoType:
-        val = self._get(key, context, AnyProto)
+        val = self._get_proto(key, context)
         ret_val = proto_message_type()
         if val.Unpack(ret_val):
             return ret_val
 
         raise MismatchedProtoType(f"Error unpacking from {val.type_url} to {proto_message_type.DESCRIPTOR.name}")
 
     def _get(self, key: str, context: Dict[str, Any], typ: Type[ReturnType]) -> ReturnType:
@@ -184,19 +184,41 @@
                 context=convert_context(ctx),
                 namespace=self.namespace,
                 repo_key=self.repository,
             )
             response = getattr(self._client, fn_name)(req)
             return response.value
         except grpc.RpcError as e:
+            if e.code() == grpc.StatusCode.NOT_FOUND:
+                raise FeatureNotFound(e.details()) from e
+            if e.code() == grpc.StatusCode.INVALID_ARGUMENT:
+                raise MismatchedType(e.details()) from e
+            raise
+
+    def _get_proto(self, key: str, context: Dict[str, Any]) -> AnyProto:
+        ctx = self.context | context
+        try:
+            req = GetProtoValueRequest(
+                key=key,
+                context=convert_context(ctx),
+                namespace=self.namespace,
+                repo_key=self.repository,
+            )
+            response = self._client.GetProtoValue(req)
+            if response.value_v2.IsInitialized() and response.value_v2.type_url:
+                return AnyProto(
+                    type_url=response.value_v2.type_url,
+                    value=response.value_v2.value,
+                )
+            return response.value
+        except grpc.RpcError as e:
+            if e.code() == grpc.StatusCode.NOT_FOUND:
+                raise FeatureNotFound(e.details()) from e
             if e.code() == grpc.StatusCode.INVALID_ARGUMENT:
-                if "type mismatch" in (e.details() or ""):
-                    raise MismatchedType(e.details()) from e
-                elif "not found" in (e.details() or ""):
-                    raise FeatureNotFound(e.details()) from e
+                raise MismatchedType(e.details()) from e
             raise
 
 
 class SidecarClient(GRPCClient):
     def __init__(
         self,
         owner_name: str,
```

### Comparing `lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py` & `lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: lekko/client/v1beta1/configuration_service.proto
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0lekko/client/v1beta1/configuration_service.proto\x12\x14lekko.client.v1beta1\x1a\x19google/protobuf/any.proto\"K\n\rRepositoryKey\x12\x1d\n\nowner_name\x18\x01 \x01(\tR\townerName\x12\x1b\n\trepo_name\x18\x02 \x01(\tR\x08repoName\"\xb0\x02\n\x13GetBoolValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x36.lekko.client.v1beta1.GetBoolValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\",\n\x14GetBoolValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x08R\x05value\"\xae\x02\n\x12GetIntValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12O\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x35.lekko.client.v1beta1.GetIntValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\"+\n\x13GetIntValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x03R\x05value\"\xb2\x02\n\x14GetFloatValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12Q\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x37.lekko.client.v1beta1.GetFloatValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\"-\n\x15GetFloatValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x01R\x05value\"\xb4\x02\n\x15GetStringValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12R\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x38.lekko.client.v1beta1.GetStringValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\".\n\x16GetStringValueResponse\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\"\xb2\x02\n\x14GetProtoValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12Q\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x37.lekko.client.v1beta1.GetProtoValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\"C\n\x15GetProtoValueResponse\x12*\n\x05value\x18\x01 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05value\"\xb0\x02\n\x13GetJSONValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x36.lekko.client.v1beta1.GetJSONValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\",\n\x14GetJSONValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x0cR\x05value\"\x99\x01\n\x05Value\x12\x1f\n\nbool_value\x18\x01 \x01(\x08H\x00R\tboolValue\x12\x1d\n\tint_value\x18\x02 \x01(\x03H\x00R\x08intValue\x12#\n\x0c\x64ouble_value\x18\x03 \x01(\x01H\x00R\x0b\x64oubleValue\x12#\n\x0cstring_value\x18\x04 \x01(\tH\x00R\x0bstringValueB\x06\n\x04kind\"x\n\x0fRegisterRequest\x12>\n\x08repo_key\x18\x01 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x12%\n\x0enamespace_list\x18\x02 \x03(\tR\rnamespaceList\"\x12\n\x10RegisterResponse\"\x13\n\x11\x44\x65registerRequest\"\x14\n\x12\x44\x65registerResponse2\xd5\x06\n\x14\x43onfigurationService\x12g\n\x0cGetBoolValue\x12).lekko.client.v1beta1.GetBoolValueRequest\x1a*.lekko.client.v1beta1.GetBoolValueResponse\"\x00\x12\x64\n\x0bGetIntValue\x12(.lekko.client.v1beta1.GetIntValueRequest\x1a).lekko.client.v1beta1.GetIntValueResponse\"\x00\x12j\n\rGetFloatValue\x12*.lekko.client.v1beta1.GetFloatValueRequest\x1a+.lekko.client.v1beta1.GetFloatValueResponse\"\x00\x12m\n\x0eGetStringValue\x12+.lekko.client.v1beta1.GetStringValueRequest\x1a,.lekko.client.v1beta1.GetStringValueResponse\"\x00\x12j\n\rGetProtoValue\x12*.lekko.client.v1beta1.GetProtoValueRequest\x1a+.lekko.client.v1beta1.GetProtoValueResponse\"\x00\x12g\n\x0cGetJSONValue\x12).lekko.client.v1beta1.GetJSONValueRequest\x1a*.lekko.client.v1beta1.GetJSONValueResponse\"\x00\x12[\n\x08Register\x12%.lekko.client.v1beta1.RegisterRequest\x1a&.lekko.client.v1beta1.RegisterResponse\"\x00\x12\x61\n\nDeregister\x12\'.lekko.client.v1beta1.DeregisterRequest\x1a(.lekko.client.v1beta1.DeregisterResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n0lekko/client/v1beta1/configuration_service.proto\x12\x14lekko.client.v1beta1\x1a\x19google/protobuf/any.proto\"K\n\rRepositoryKey\x12\x1d\n\nowner_name\x18\x01 \x01(\tR\townerName\x12\x1b\n\trepo_name\x18\x02 \x01(\tR\x08repoName\"\xb0\x02\n\x13GetBoolValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x36.lekko.client.v1beta1.GetBoolValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\",\n\x14GetBoolValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x08R\x05value\"\xae\x02\n\x12GetIntValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12O\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x35.lekko.client.v1beta1.GetIntValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\"+\n\x13GetIntValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x03R\x05value\"\xb2\x02\n\x14GetFloatValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12Q\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x37.lekko.client.v1beta1.GetFloatValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\"-\n\x15GetFloatValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x01R\x05value\"\xb4\x02\n\x15GetStringValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12R\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x38.lekko.client.v1beta1.GetStringValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\".\n\x16GetStringValueResponse\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\"\xb2\x02\n\x14GetProtoValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12Q\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x37.lekko.client.v1beta1.GetProtoValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\"y\n\x15GetProtoValueResponse\x12*\n\x05value\x18\x01 \x01(\x0b\x32\x14.google.protobuf.AnyR\x05value\x12\x34\n\x08value_v2\x18\x02 \x01(\x0b\x32\x19.lekko.client.v1beta1.AnyR\x07valueV2\"6\n\x03\x41ny\x12\x19\n\x08type_url\x18\x01 \x01(\tR\x07typeUrl\x12\x14\n\x05value\x18\x02 \x01(\x0cR\x05value\"\xb0\x02\n\x13GetJSONValueRequest\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12P\n\x07\x63ontext\x18\x02 \x03(\x0b\x32\x36.lekko.client.v1beta1.GetJSONValueRequest.ContextEntryR\x07\x63ontext\x12\x1c\n\tnamespace\x18\x03 \x01(\tR\tnamespace\x12>\n\x08repo_key\x18\x04 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x1aW\n\x0c\x43ontextEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x31\n\x05value\x18\x02 \x01(\x0b\x32\x1b.lekko.client.v1beta1.ValueR\x05value:\x02\x38\x01\",\n\x14GetJSONValueResponse\x12\x14\n\x05value\x18\x01 \x01(\x0cR\x05value\"\x99\x01\n\x05Value\x12\x1f\n\nbool_value\x18\x01 \x01(\x08H\x00R\tboolValue\x12\x1d\n\tint_value\x18\x02 \x01(\x03H\x00R\x08intValue\x12#\n\x0c\x64ouble_value\x18\x03 \x01(\x01H\x00R\x0b\x64oubleValue\x12#\n\x0cstring_value\x18\x04 \x01(\tH\x00R\x0bstringValueB\x06\n\x04kind\"x\n\x0fRegisterRequest\x12>\n\x08repo_key\x18\x01 \x01(\x0b\x32#.lekko.client.v1beta1.RepositoryKeyR\x07repoKey\x12%\n\x0enamespace_list\x18\x02 \x03(\tR\rnamespaceList\"\x12\n\x10RegisterResponse\"\x13\n\x11\x44\x65registerRequest\"\x14\n\x12\x44\x65registerResponse2\xd5\x06\n\x14\x43onfigurationService\x12g\n\x0cGetBoolValue\x12).lekko.client.v1beta1.GetBoolValueRequest\x1a*.lekko.client.v1beta1.GetBoolValueResponse\"\x00\x12\x64\n\x0bGetIntValue\x12(.lekko.client.v1beta1.GetIntValueRequest\x1a).lekko.client.v1beta1.GetIntValueResponse\"\x00\x12j\n\rGetFloatValue\x12*.lekko.client.v1beta1.GetFloatValueRequest\x1a+.lekko.client.v1beta1.GetFloatValueResponse\"\x00\x12m\n\x0eGetStringValue\x12+.lekko.client.v1beta1.GetStringValueRequest\x1a,.lekko.client.v1beta1.GetStringValueResponse\"\x00\x12j\n\rGetProtoValue\x12*.lekko.client.v1beta1.GetProtoValueRequest\x1a+.lekko.client.v1beta1.GetProtoValueResponse\"\x00\x12g\n\x0cGetJSONValue\x12).lekko.client.v1beta1.GetJSONValueRequest\x1a*.lekko.client.v1beta1.GetJSONValueResponse\"\x00\x12[\n\x08Register\x12%.lekko.client.v1beta1.RegisterRequest\x1a&.lekko.client.v1beta1.RegisterResponse\"\x00\x12\x61\n\nDeregister\x12\'.lekko.client.v1beta1.DeregisterRequest\x1a(.lekko.client.v1beta1.DeregisterResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'lekko.client.v1beta1.configuration_service_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -61,27 +61,29 @@
   _globals['_GETSTRINGVALUERESPONSE']._serialized_start=1548
   _globals['_GETSTRINGVALUERESPONSE']._serialized_end=1594
   _globals['_GETPROTOVALUEREQUEST']._serialized_start=1597
   _globals['_GETPROTOVALUEREQUEST']._serialized_end=1903
   _globals['_GETPROTOVALUEREQUEST_CONTEXTENTRY']._serialized_start=396
   _globals['_GETPROTOVALUEREQUEST_CONTEXTENTRY']._serialized_end=483
   _globals['_GETPROTOVALUERESPONSE']._serialized_start=1905
-  _globals['_GETPROTOVALUERESPONSE']._serialized_end=1972
-  _globals['_GETJSONVALUEREQUEST']._serialized_start=1975
-  _globals['_GETJSONVALUEREQUEST']._serialized_end=2279
+  _globals['_GETPROTOVALUERESPONSE']._serialized_end=2026
+  _globals['_ANY']._serialized_start=2028
+  _globals['_ANY']._serialized_end=2082
+  _globals['_GETJSONVALUEREQUEST']._serialized_start=2085
+  _globals['_GETJSONVALUEREQUEST']._serialized_end=2389
   _globals['_GETJSONVALUEREQUEST_CONTEXTENTRY']._serialized_start=396
   _globals['_GETJSONVALUEREQUEST_CONTEXTENTRY']._serialized_end=483
-  _globals['_GETJSONVALUERESPONSE']._serialized_start=2281
-  _globals['_GETJSONVALUERESPONSE']._serialized_end=2325
-  _globals['_VALUE']._serialized_start=2328
-  _globals['_VALUE']._serialized_end=2481
-  _globals['_REGISTERREQUEST']._serialized_start=2483
-  _globals['_REGISTERREQUEST']._serialized_end=2603
-  _globals['_REGISTERRESPONSE']._serialized_start=2605
-  _globals['_REGISTERRESPONSE']._serialized_end=2623
-  _globals['_DEREGISTERREQUEST']._serialized_start=2625
-  _globals['_DEREGISTERREQUEST']._serialized_end=2644
-  _globals['_DEREGISTERRESPONSE']._serialized_start=2646
-  _globals['_DEREGISTERRESPONSE']._serialized_end=2666
-  _globals['_CONFIGURATIONSERVICE']._serialized_start=2669
-  _globals['_CONFIGURATIONSERVICE']._serialized_end=3522
+  _globals['_GETJSONVALUERESPONSE']._serialized_start=2391
+  _globals['_GETJSONVALUERESPONSE']._serialized_end=2435
+  _globals['_VALUE']._serialized_start=2438
+  _globals['_VALUE']._serialized_end=2591
+  _globals['_REGISTERREQUEST']._serialized_start=2593
+  _globals['_REGISTERREQUEST']._serialized_end=2713
+  _globals['_REGISTERRESPONSE']._serialized_start=2715
+  _globals['_REGISTERRESPONSE']._serialized_end=2733
+  _globals['_DEREGISTERREQUEST']._serialized_start=2735
+  _globals['_DEREGISTERREQUEST']._serialized_end=2754
+  _globals['_DEREGISTERRESPONSE']._serialized_start=2756
+  _globals['_DEREGISTERRESPONSE']._serialized_end=2776
+  _globals['_CONFIGURATIONSERVICE']._serialized_start=2779
+  _globals['_CONFIGURATIONSERVICE']._serialized_end=3632
 # @@protoc_insertion_point(module_scope)
```

### Comparing `lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi` & `lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -334,27 +334,49 @@
 global___GetProtoValueRequest = GetProtoValueRequest
 
 @typing_extensions.final
 class GetProtoValueResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     VALUE_FIELD_NUMBER: builtins.int
+    VALUE_V2_FIELD_NUMBER: builtins.int
     @property
     def value(self) -> google.protobuf.any_pb2.Any: ...
+    @property
+    def value_v2(self) -> global___Any: ...
     def __init__(
         self,
         *,
         value: google.protobuf.any_pb2.Any | None = ...,
+        value_v2: global___Any | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["value", b"value"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["value", b"value", "value_v2", b"value_v2"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["value", b"value", "value_v2", b"value_v2"]) -> None: ...
 
 global___GetProtoValueResponse = GetProtoValueResponse
 
 @typing_extensions.final
+class Any(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    TYPE_URL_FIELD_NUMBER: builtins.int
+    VALUE_FIELD_NUMBER: builtins.int
+    type_url: builtins.str
+    value: builtins.bytes
+    def __init__(
+        self,
+        *,
+        type_url: builtins.str = ...,
+        value: builtins.bytes = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["type_url", b"type_url", "value", b"value"]) -> None: ...
+
+global___Any = Any
+
+@typing_extensions.final
 class GetJSONValueRequest(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class ContextEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
```

### Comparing `lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py` & `lekko_client-0.1.2/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.1/lekko_client/helpers.py` & `lekko_client-0.1.2/lekko_client/helpers.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.1/pyproject.toml` & `lekko_client-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1.1/tests/mock_server.py` & `lekko_client-0.1.2/tests/mock_server.py`

 * *Files identical despite different names*

