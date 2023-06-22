# Comparing `tmp/th2_grpc_common-4.2.0.dev4476477365.tar.gz` & `tmp/th2_grpc_common-4.3.0.dev5346500753.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_grpc_common-4.2.0.dev4476477365.tar", last modified: Tue Mar 21 07:20:00 2023, max compression
+gzip compressed data, was "dist/th2_grpc_common-4.3.0.dev5346500753.tar", last modified: Thu Jun 22 14:04:40 2023, max compression
```

## Comparing `th2_grpc_common-4.2.0.dev4476477365.tar` & `th2_grpc_common-4.3.0.dev5346500753.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/
--rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4816 2023-03-21 07:19:01.000000 th2_grpc_common-4.2.0.dev4476477365/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-03-21 07:19:05.000000 th2_grpc_common-4.2.0.dev4476477365/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-03-21 07:19:01.000000 th2_grpc_common-4.2.0.dev4476477365/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8561 2023-03-21 07:19:01.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/common.proto
--rw-r--r--   0 runner    (1001) docker     (122)    31313 2023-03-21 07:19:59.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (122)    43947 2023-03-21 07:19:59.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      159 2023-03-21 07:19:59.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     6167 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      408 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-03-21 07:20:00.000000 th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/
+-rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4966 2023-06-22 14:03:30.000000 th2_grpc_common-4.3.0.dev5346500753/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-22 14:03:30.000000 th2_grpc_common-4.3.0.dev5346500753/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4491 2023-06-22 14:03:30.000000 th2_grpc_common-4.3.0.dev5346500753/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8561 2023-06-22 14:03:30.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/common.proto
+-rw-r--r--   0 runner    (1001) docker     (122)    14747 2023-06-22 14:04:39.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45617 2023-06-22 14:04:39.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-06-22 14:04:39.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6525 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      408 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-22 14:04:40.000000 th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common.egg-info/top_level.txt
```

### Comparing `th2_grpc_common-4.2.0.dev4476477365/PKG-INFO` & `th2_grpc_common-4.3.0.dev5346500753/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 Metadata-Version: 2.1
 Name: th2_grpc_common
-Version: 4.2.0.dev4476477365
+Version: 4.3.0.dev5346500753
 Summary: th2_grpc_common
 Home-page: https://github.com/th2-net/th2-grpc-common
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC common library (4.2.0)
+Description: # th2 gRPC common library (4.3.0)
         
-        
-        This library contains common proto messages that are used in all th2 components. See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto") file for details. <br>
-        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
+        This library contains common proto messages that are used in all th2 components.
+        See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto")
+        file for details. <br>
+        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
+        repositories.
         
         ## How to maintain a project
+        
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
         3. Update the package version of Python in `package_info.json` file.
         4. Commit everything.
         
         ### Java
+        
         If you wish to manually create and publish a package for Java, run the following command:
+        
         ```
         gradle --no-daemon clean build publish artifactoryPublish \
                -Purl=${URL} \ 
                -Puser=${USER} \
                -Ppassword=${PASSWORD}
         ```
+        
         `URL`, `USER` and `PASSWORD` are parameters for publishing.
         
         ### Python
+        
         If you wish to manually create and publish a package for Python:
+        
         1. Generate services with `Gradle`:
             ```
                gradle --no-daemon clean generateProto
             ```
            You can find the generated files by following path: `src/gen/main/services/python`
         2. Generate code from `.proto` files and publish everything using `twine`:
             ```
             pip install -r requirements.txt
             pip install twine
             python setup.py generate
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
-            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
+           `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.3.0
+        
+        + Updated bom:4.4.0
+        + Updated grpc-service-generator:3.4.0
+        + Updated grpcio-tools:1.54.2
+        + Updated mypy-protobuf:3.4
+        
         ### 4.2.0
         
         + Added vulnerability check
         + Updated bom:4.2.0
         + Updated protoc:3.21.7
         + Updated grpc-service-generator:3.3.1
         + Downgraded grpc version from 1.50.2 to 1.48.1 according to bom
@@ -58,70 +73,81 @@
         ### 4.1.1
         
         + Added script for publishing dev-release for maven artefacts
         + Migrated to bom:4.2.0
         
         ### 4.1.0
         
-        + Added event / message batch metadata with the external_user_queue field. This field can be used to send MQ message to direct queue instead of schema routing in some cases.
+        + Added event / message batch metadata with the external_user_queue field. This field can be used to send MQ message to
+          direct queue instead of schema routing in some cases.
         
         ### 4.0.0
+        
         + Marked deprecated fields as `reserved`
         + Moved `timestamp` from `MessageMetadata`/`RawMessageMetadata` to `MessageID`
         + Moved `start_timestamp` from `Event` to `EventID`
         + Added `book_name` to `MessageID` and `EventID`
         + Added `scope` to `EventID`
-        + Added `map<string, SessionAliasToDirectionCheckpoint>` to `Checkpoint`. It describes book to session alias to direction.
+        + Added `map<string, SessionAliasToDirectionCheckpoint>` to `Checkpoint`. It describes book to session alias to
+          direction.
         + Added `EventBatchMetadata` and `MessageGroupBatchMetadata` with `external_queue` property
         
         ### 3.13.0
+        
         + Update `th2-bom` version from '3.0.0' to '4.1.0'
         
         ### 3.12.0
         
-        + Update `grpcio-tools` Python dependency version from `1.38.1` to `1.50.0` 
+        + Update `grpcio-tools` Python dependency version from `1.38.1` to `1.50.0`
         + Update `grpc` Java dependency version from `1.32.1` to `1.50.2`
         
         ### 3.11.1
         
-        + Update `mypy-protobuf` Python dependency version from `2.5` to `3.2` 
+        + Update `mypy-protobuf` Python dependency version from `2.5` to `3.2`
         
         ### 3.11.0
         
         + Added `session_group` parameter to `ConnectionID`
         
         ### 3.10.0
         
         + Updated grpc-service-generator (added support for gRPC pins filters).
         
         ### 3.9.0
         
         + Added `null_value` in `ValueFilter`. Should be used only with EQUAL and NOT_EQUAL operations.
         
         ### 3.8.0
+        
         + Added `time_precision` and `decimal_precision` parameters to `RootComparisonSettings`
-        + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operation, witch filter a field by comparing values(`date/time` in ISO format and `numeric` types) with the precision. The timestamps will be compared with the protobuf duration format. Numbers use string format, for example _0.0001_, _0.125_, _125E-3_
+        + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operation, witch filter a field by comparing
+          values(`date/time` in ISO format and `numeric` types) with the precision. The timestamps will be compared with the
+          protobuf duration format. Numbers use string format, for example _0.0001_, _0.125_, _125E-3_
         
         ### 3.7.0
+        
         + Added `check_repeating_group_order` parameter to `RootComparisonSettings`
         
         ### 3.6.0
+        
         + Added `description` parameter to `RootMessageFilter`.
         
         ### 3.5.0
-        + Added SimpleList parameter to SimpleFilter. 
+        
+        + Added SimpleList parameter to SimpleFilter.
         
         ### 3.4.0
         
         + Added `IN` and `NOT_IN` filter operation, which filter a field by value from list of `String`.
         + Added `LIKE` and `NOT_LIKE` filter operation, which filter a field by `String` regEx expression.
-        + Added `MORE`, `LESS`, `NOT_MORE`, `NOT_LESS` filter operations, which filter a field by comparing values(`numeric` types and `date/time` in ISO format).
-        + Added `WILDCARD` and `NOT_WILDCARD`  filter operations, which filter a field by `String` specified wildcard expression.
-        The wildcard matcher uses the characters `?` and `*` to represent a single or multiple (zero or more) wildcard characters.
-        This is the same as often found on Dos/Unix command lines.
+        + Added `MORE`, `LESS`, `NOT_MORE`, `NOT_LESS` filter operations, which filter a field by comparing values(`numeric`
+          types and `date/time` in ISO format).
+        + Added `WILDCARD` and `NOT_WILDCARD`  filter operations, which filter a field by `String` specified wildcard
+          expression. The wildcard matcher uses the characters `?` and `*` to represent a single or multiple (zero or more)
+          wildcard characters. This is the same as often found on Dos/Unix command lines.
         + "abc-123", "*-123"     --&gt; true
         + "abc-123", "*-xyz"     --&gt; false
         + "abc-123", "ab*"       --&gt; true
         + "abc-123", "*-???"     --&gt; true
         + "abc-123", "*-????"    --&gt; false
         
         N.B. the sequence `*?` does not work properly at present in match strings.
```

### Comparing `th2_grpc_common-4.2.0.dev4476477365/README.md` & `th2_grpc_common-4.3.0.dev5346500753/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,63 @@
-# th2 gRPC common library (4.2.0)
+# th2 gRPC common library (4.3.0)
 
-
-This library contains common proto messages that are used in all th2 components. See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto") file for details. <br>
-Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
+This library contains common proto messages that are used in all th2 components.
+See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto")
+file for details. <br>
+Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
+repositories.
 
 ## How to maintain a project
+
 1. Perform the necessary changes.
 2. Update the package version of Java in `gradle.properties` file.
 3. Update the package version of Python in `package_info.json` file.
 4. Commit everything.
 
 ### Java
+
 If you wish to manually create and publish a package for Java, run the following command:
+
 ```
 gradle --no-daemon clean build publish artifactoryPublish \
        -Purl=${URL} \ 
        -Puser=${USER} \
        -Ppassword=${PASSWORD}
 ```
+
 `URL`, `USER` and `PASSWORD` are parameters for publishing.
 
 ### Python
+
 If you wish to manually create and publish a package for Python:
+
 1. Generate services with `Gradle`:
     ```
        gradle --no-daemon clean generateProto
     ```
    You can find the generated files by following path: `src/gen/main/services/python`
 2. Generate code from `.proto` files and publish everything using `twine`:
     ```
     pip install -r requirements.txt
     pip install twine
     python setup.py generate
     python setup.py sdist
     twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
     ```
-    `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
+   `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
 
 ## Release notes
 
+### 4.3.0
+
++ Updated bom:4.4.0
++ Updated grpc-service-generator:3.4.0
++ Updated grpcio-tools:1.54.2
++ Updated mypy-protobuf:3.4
+
 ### 4.2.0
 
 + Added vulnerability check
 + Updated bom:4.2.0
 + Updated protoc:3.21.7
 + Updated grpc-service-generator:3.3.1
 + Downgraded grpc version from 1.50.2 to 1.48.1 according to bom
@@ -50,70 +65,81 @@
 ### 4.1.1
 
 + Added script for publishing dev-release for maven artefacts
 + Migrated to bom:4.2.0
 
 ### 4.1.0
 
-+ Added event / message batch metadata with the external_user_queue field. This field can be used to send MQ message to direct queue instead of schema routing in some cases.
++ Added event / message batch metadata with the external_user_queue field. This field can be used to send MQ message to
+  direct queue instead of schema routing in some cases.
 
 ### 4.0.0
+
 + Marked deprecated fields as `reserved`
 + Moved `timestamp` from `MessageMetadata`/`RawMessageMetadata` to `MessageID`
 + Moved `start_timestamp` from `Event` to `EventID`
 + Added `book_name` to `MessageID` and `EventID`
 + Added `scope` to `EventID`
-+ Added `map<string, SessionAliasToDirectionCheckpoint>` to `Checkpoint`. It describes book to session alias to direction.
++ Added `map<string, SessionAliasToDirectionCheckpoint>` to `Checkpoint`. It describes book to session alias to
+  direction.
 + Added `EventBatchMetadata` and `MessageGroupBatchMetadata` with `external_queue` property
 
 ### 3.13.0
+
 + Update `th2-bom` version from '3.0.0' to '4.1.0'
 
 ### 3.12.0
 
-+ Update `grpcio-tools` Python dependency version from `1.38.1` to `1.50.0` 
++ Update `grpcio-tools` Python dependency version from `1.38.1` to `1.50.0`
 + Update `grpc` Java dependency version from `1.32.1` to `1.50.2`
 
 ### 3.11.1
 
-+ Update `mypy-protobuf` Python dependency version from `2.5` to `3.2` 
++ Update `mypy-protobuf` Python dependency version from `2.5` to `3.2`
 
 ### 3.11.0
 
 + Added `session_group` parameter to `ConnectionID`
 
 ### 3.10.0
 
 + Updated grpc-service-generator (added support for gRPC pins filters).
 
 ### 3.9.0
 
 + Added `null_value` in `ValueFilter`. Should be used only with EQUAL and NOT_EQUAL operations.
 
 ### 3.8.0
+
 + Added `time_precision` and `decimal_precision` parameters to `RootComparisonSettings`
-+ Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operation, witch filter a field by comparing values(`date/time` in ISO format and `numeric` types) with the precision. The timestamps will be compared with the protobuf duration format. Numbers use string format, for example _0.0001_, _0.125_, _125E-3_
++ Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operation, witch filter a field by comparing
+  values(`date/time` in ISO format and `numeric` types) with the precision. The timestamps will be compared with the
+  protobuf duration format. Numbers use string format, for example _0.0001_, _0.125_, _125E-3_
 
 ### 3.7.0
+
 + Added `check_repeating_group_order` parameter to `RootComparisonSettings`
 
 ### 3.6.0
+
 + Added `description` parameter to `RootMessageFilter`.
 
 ### 3.5.0
-+ Added SimpleList parameter to SimpleFilter. 
+
++ Added SimpleList parameter to SimpleFilter.
 
 ### 3.4.0
 
 + Added `IN` and `NOT_IN` filter operation, which filter a field by value from list of `String`.
 + Added `LIKE` and `NOT_LIKE` filter operation, which filter a field by `String` regEx expression.
-+ Added `MORE`, `LESS`, `NOT_MORE`, `NOT_LESS` filter operations, which filter a field by comparing values(`numeric` types and `date/time` in ISO format).
-+ Added `WILDCARD` and `NOT_WILDCARD`  filter operations, which filter a field by `String` specified wildcard expression.
-The wildcard matcher uses the characters `?` and `*` to represent a single or multiple (zero or more) wildcard characters.
-This is the same as often found on Dos/Unix command lines.
++ Added `MORE`, `LESS`, `NOT_MORE`, `NOT_LESS` filter operations, which filter a field by comparing values(`numeric`
+  types and `date/time` in ISO format).
++ Added `WILDCARD` and `NOT_WILDCARD`  filter operations, which filter a field by `String` specified wildcard
+  expression. The wildcard matcher uses the characters `?` and `*` to represent a single or multiple (zero or more)
+  wildcard characters. This is the same as often found on Dos/Unix command lines.
 + "abc-123", "*-123"     --&gt; true
 + "abc-123", "*-xyz"     --&gt; false
 + "abc-123", "ab*"       --&gt; true
 + "abc-123", "*-???"     --&gt; true
 + "abc-123", "*-????"    --&gt; false
 
 N.B. the sequence `*?` does not work properly at present in match strings.
```

### Comparing `th2_grpc_common-4.2.0.dev4476477365/setup.py` & `th2_grpc_common-4.3.0.dev5346500753/setup.py`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/common.proto` & `th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/common.proto`

 * *Files identical despite different names*

### Comparing `th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common/common_pb2.pyi` & `th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common/common_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,96 +1,105 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
+
+Copyright 2020-2022 Exactpro (Exactpro Systems Limited)
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
 """
 import builtins
+import collections.abc
 import google.protobuf.descriptor
 import google.protobuf.duration_pb2
 import google.protobuf.internal.containers
 import google.protobuf.internal.enum_type_wrapper
 import google.protobuf.message
 import google.protobuf.timestamp_pb2
 import google.protobuf.wrappers_pb2
+import sys
 import typing
-import typing_extensions
+
+if sys.version_info >= (3, 10):
+    import typing as typing_extensions
+else:
+    import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class _Direction:
-    ValueType = typing.NewType('ValueType', builtins.int)
+    ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
+
 class _DirectionEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_Direction.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     FIRST: _Direction.ValueType  # 0
     """Incoming message for connectivity"""
-
     SECOND: _Direction.ValueType  # 1
     """Outgoing message for connectivity"""
 
-class Direction(_Direction, metaclass=_DirectionEnumTypeWrapper):
-    pass
+class Direction(_Direction, metaclass=_DirectionEnumTypeWrapper): ...
 
 FIRST: Direction.ValueType  # 0
 """Incoming message for connectivity"""
-
 SECOND: Direction.ValueType  # 1
 """Outgoing message for connectivity"""
-
 global___Direction = Direction
 
-
 class _NullValue:
-    ValueType = typing.NewType('ValueType', builtins.int)
+    ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
+
 class _NullValueEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_NullValue.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     NULL_VALUE: _NullValue.ValueType  # 0
-class NullValue(_NullValue, metaclass=_NullValueEnumTypeWrapper):
-    """--// Message body structure //--//
 
-    """
-    pass
+class NullValue(_NullValue, metaclass=_NullValueEnumTypeWrapper):
+    """--// Message body structure //--//"""
 
 NULL_VALUE: NullValue.ValueType  # 0
 global___NullValue = NullValue
 
-
 class _FailUnexpected:
-    ValueType = typing.NewType('ValueType', builtins.int)
+    ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
+
 class _FailUnexpectedEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_FailUnexpected.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     NO: _FailUnexpected.ValueType  # 0
     """comparison won't fail in case of unexpected fields or messages"""
-
     FIELDS: _FailUnexpected.ValueType  # 1
     """comparison will fail in case of unexpected fields only"""
-
     FIELDS_AND_MESSAGES: _FailUnexpected.ValueType  # 2
     """comparison will fail in case of unexpected fields or messages"""
 
 class FailUnexpected(_FailUnexpected, metaclass=_FailUnexpectedEnumTypeWrapper):
     """--// Settings //--//"""
-    pass
 
 NO: FailUnexpected.ValueType  # 0
 """comparison won't fail in case of unexpected fields or messages"""
-
 FIELDS: FailUnexpected.ValueType  # 1
 """comparison will fail in case of unexpected fields only"""
-
 FIELDS_AND_MESSAGES: FailUnexpected.ValueType  # 2
 """comparison will fail in case of unexpected fields or messages"""
-
 global___FailUnexpected = FailUnexpected
 
-
 class _FilterOperation:
-    ValueType = typing.NewType('ValueType', builtins.int)
+    ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
+
 class _FilterOperationEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_FilterOperation.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     EQUAL: _FilterOperation.ValueType  # 0
     NOT_EQUAL: _FilterOperation.ValueType  # 1
     EMPTY: _FilterOperation.ValueType  # 2
     NOT_EMPTY: _FilterOperation.ValueType  # 3
     IN: _FilterOperation.ValueType  # 4
@@ -101,19 +110,17 @@
     NOT_MORE: _FilterOperation.ValueType  # 9
     LESS: _FilterOperation.ValueType  # 10
     NOT_LESS: _FilterOperation.ValueType  # 11
     WILDCARD: _FilterOperation.ValueType  # 12
     NOT_WILDCARD: _FilterOperation.ValueType  # 13
     EQ_TIME_PRECISION: _FilterOperation.ValueType  # 14
     EQ_DECIMAL_PRECISION: _FilterOperation.ValueType  # 15
-class FilterOperation(_FilterOperation, metaclass=_FilterOperationEnumTypeWrapper):
-    """--// Message filter //--//
 
-    """
-    pass
+class FilterOperation(_FilterOperation, metaclass=_FilterOperationEnumTypeWrapper):
+    """--// Message filter //--//"""
 
 EQUAL: FilterOperation.ValueType  # 0
 NOT_EQUAL: FilterOperation.ValueType  # 1
 EMPTY: FilterOperation.ValueType  # 2
 NOT_EMPTY: FilterOperation.ValueType  # 3
 IN: FilterOperation.ValueType  # 4
 NOT_IN: FilterOperation.ValueType  # 5
@@ -125,824 +132,934 @@
 NOT_LESS: FilterOperation.ValueType  # 11
 WILDCARD: FilterOperation.ValueType  # 12
 NOT_WILDCARD: FilterOperation.ValueType  # 13
 EQ_TIME_PRECISION: FilterOperation.ValueType  # 14
 EQ_DECIMAL_PRECISION: FilterOperation.ValueType  # 15
 global___FilterOperation = FilterOperation
 
-
 class _EventStatus:
-    ValueType = typing.NewType('ValueType', builtins.int)
+    ValueType = typing.NewType("ValueType", builtins.int)
     V: typing_extensions.TypeAlias = ValueType
+
 class _EventStatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[_EventStatus.ValueType], builtins.type):
     DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
     SUCCESS: _EventStatus.ValueType  # 0
     FAILED: _EventStatus.ValueType  # 1
+
 class EventStatus(_EventStatus, metaclass=_EventStatusEnumTypeWrapper):
     """--// Event //--//"""
-    pass
 
 SUCCESS: EventStatus.ValueType  # 0
 FAILED: EventStatus.ValueType  # 1
 global___EventStatus = EventStatus
 
-
+@typing_extensions.final
 class ConnectionID(google.protobuf.message.Message):
-    """--// Metadata structures //--//
+    """--// Metadata structures //--//"""
 
-    """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     SESSION_ALIAS_FIELD_NUMBER: builtins.int
     SESSION_GROUP_FIELD_NUMBER: builtins.int
-    session_alias: typing.Text
+    session_alias: builtins.str
     """Session identifier depends on protocol, target / sender"""
-
-    session_group: typing.Text
+    session_group: builtins.str
     """Session group"""
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        session_alias: typing.Text = ...,
-        session_group: typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["session_alias",b"session_alias","session_group",b"session_group"]) -> None: ...
+        session_alias: builtins.str = ...,
+        session_group: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["session_alias", b"session_alias", "session_group", b"session_group"]) -> None: ...
+
 global___ConnectionID = ConnectionID
 
+@typing_extensions.final
 class MessageID(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     CONNECTION_ID_FIELD_NUMBER: builtins.int
     DIRECTION_FIELD_NUMBER: builtins.int
     SEQUENCE_FIELD_NUMBER: builtins.int
     SUBSEQUENCE_FIELD_NUMBER: builtins.int
     BOOK_NAME_FIELD_NUMBER: builtins.int
     TIMESTAMP_FIELD_NUMBER: builtins.int
     @property
     def connection_id(self) -> global___ConnectionID: ...
     direction: global___Direction.ValueType
     """Transport direction."""
-
     sequence: builtins.int
     """Unique sequence number in session"""
-
     @property
     def subsequence(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]:
         """List of nested sequences in addition to the main one"""
-        pass
-    book_name: typing.Text
+    book_name: builtins.str
     @property
     def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
         """Message creation timestamp"""
-        pass
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        connection_id: typing.Optional[global___ConnectionID] = ...,
+        connection_id: global___ConnectionID | None = ...,
         direction: global___Direction.ValueType = ...,
         sequence: builtins.int = ...,
-        subsequence: typing.Optional[typing.Iterable[builtins.int]] = ...,
-        book_name: typing.Text = ...,
-        timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["connection_id",b"connection_id","timestamp",b"timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_name",b"book_name","connection_id",b"connection_id","direction",b"direction","sequence",b"sequence","subsequence",b"subsequence","timestamp",b"timestamp"]) -> None: ...
+        subsequence: collections.abc.Iterable[builtins.int] | None = ...,
+        book_name: builtins.str = ...,
+        timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["connection_id", b"connection_id", "timestamp", b"timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["book_name", b"book_name", "connection_id", b"connection_id", "direction", b"direction", "sequence", b"sequence", "subsequence", b"subsequence", "timestamp", b"timestamp"]) -> None: ...
+
 global___MessageID = MessageID
 
+@typing_extensions.final
 class EventBatchMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     EXTERNAL_QUEUE_FIELD_NUMBER: builtins.int
-    external_queue: typing.Text
+    external_queue: builtins.str
     """External user queue can be used for routing by internal box logic."""
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        external_queue: typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["external_queue",b"external_queue"]) -> None: ...
+        external_queue: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["external_queue", b"external_queue"]) -> None: ...
+
 global___EventBatchMetadata = EventBatchMetadata
 
+@typing_extensions.final
 class MessageGroupBatchMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     EXTERNAL_QUEUE_FIELD_NUMBER: builtins.int
-    external_queue: typing.Text
+    external_queue: builtins.str
     """External user queue can be used for routing by internal box logic."""
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        external_queue: typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["external_queue",b"external_queue"]) -> None: ...
+        external_queue: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["external_queue", b"external_queue"]) -> None: ...
+
 global___MessageGroupBatchMetadata = MessageGroupBatchMetadata
 
+@typing_extensions.final
 class MessageMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
-        value: typing.Text
-        def __init__(self,
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
             *,
-            key: typing.Text = ...,
-            value: typing.Text = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     ID_FIELD_NUMBER: builtins.int
     MESSAGE_TYPE_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     PROTOCOL_FIELD_NUMBER: builtins.int
     @property
     def id(self) -> global___MessageID:
         """Message id should be unique in session"""
-        pass
-    message_type: typing.Text
+    message_type: builtins.str
     """Message type by dictionary"""
-
     @property
-    def properties(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]:
+    def properties(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Additional properties for the message"""
-        pass
-    protocol: typing.Text
+    protocol: builtins.str
     """Protocol to be used when encoding the message"""
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        id: typing.Optional[global___MessageID] = ...,
-        message_type: typing.Text = ...,
-        properties: typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
-        protocol: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["id",b"id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id",b"id","message_type",b"message_type","properties",b"properties","protocol",b"protocol"]) -> None: ...
+        id: global___MessageID | None = ...,
+        message_type: builtins.str = ...,
+        properties: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        protocol: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["id", b"id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "message_type", b"message_type", "properties", b"properties", "protocol", b"protocol"]) -> None: ...
+
 global___MessageMetadata = MessageMetadata
 
+@typing_extensions.final
 class RawMessageMetadata(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class PropertiesEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
-        value: typing.Text
-        def __init__(self,
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
             *,
-            key: typing.Text = ...,
-            value: typing.Text = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     ID_FIELD_NUMBER: builtins.int
     PROPERTIES_FIELD_NUMBER: builtins.int
     PROTOCOL_FIELD_NUMBER: builtins.int
     @property
     def id(self) -> global___MessageID:
         """Message id should be unique in session"""
-        pass
     @property
-    def properties(self) -> google.protobuf.internal.containers.ScalarMap[typing.Text, typing.Text]:
+    def properties(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]:
         """Additional properties for the raw message"""
-        pass
-    protocol: typing.Text
+    protocol: builtins.str
     """Protocol to be used when decoding the message"""
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        id: typing.Optional[global___MessageID] = ...,
-        properties: typing.Optional[typing.Mapping[typing.Text, typing.Text]] = ...,
-        protocol: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["id",b"id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id",b"id","properties",b"properties","protocol",b"protocol"]) -> None: ...
+        id: global___MessageID | None = ...,
+        properties: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        protocol: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["id", b"id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "properties", b"properties", "protocol", b"protocol"]) -> None: ...
+
 global___RawMessageMetadata = RawMessageMetadata
 
+@typing_extensions.final
 class Value(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     NULL_VALUE_FIELD_NUMBER: builtins.int
     SIMPLE_VALUE_FIELD_NUMBER: builtins.int
     MESSAGE_VALUE_FIELD_NUMBER: builtins.int
     LIST_VALUE_FIELD_NUMBER: builtins.int
     null_value: global___NullValue.ValueType
-    simple_value: typing.Text
+    simple_value: builtins.str
     @property
     def message_value(self) -> global___Message: ...
     @property
     def list_value(self) -> global___ListValue: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
         null_value: global___NullValue.ValueType = ...,
-        simple_value: typing.Text = ...,
-        message_value: typing.Optional[global___Message] = ...,
-        list_value: typing.Optional[global___ListValue] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["kind",b"kind","list_value",b"list_value","message_value",b"message_value","null_value",b"null_value","simple_value",b"simple_value"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kind",b"kind","list_value",b"list_value","message_value",b"message_value","null_value",b"null_value","simple_value",b"simple_value"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind",b"kind"]) -> typing.Optional[typing_extensions.Literal["null_value","simple_value","message_value","list_value"]]: ...
+        simple_value: builtins.str = ...,
+        message_value: global___Message | None = ...,
+        list_value: global___ListValue | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["kind", b"kind", "list_value", b"list_value", "message_value", b"message_value", "null_value", b"null_value", "simple_value", b"simple_value"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["kind", b"kind", "list_value", b"list_value", "message_value", b"message_value", "null_value", b"null_value", "simple_value", b"simple_value"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["null_value", "simple_value", "message_value", "list_value"] | None: ...
+
 global___Value = Value
 
+@typing_extensions.final
 class ListValue(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     VALUES_FIELD_NUMBER: builtins.int
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Value]: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        values: typing.Optional[typing.Iterable[global___Value]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["values",b"values"]) -> None: ...
+        values: collections.abc.Iterable[global___Value] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["values", b"values"]) -> None: ...
+
 global___ListValue = ListValue
 
+@typing_extensions.final
 class Message(google.protobuf.message.Message):
-    """--// Message / Raw structures //--//
+    """--// Message / Raw structures //--//"""
 
-    """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class FieldsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
+        key: builtins.str
         @property
         def value(self) -> global___Value: ...
-        def __init__(self,
+        def __init__(
+            self,
             *,
-            key: typing.Text = ...,
-            value: typing.Optional[global___Value] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+            key: builtins.str = ...,
+            value: global___Value | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     FIELDS_FIELD_NUMBER: builtins.int
     @property
     def parent_event_id(self) -> global___EventID:
         """It maybe used to store event related to message life cycle"""
-        pass
     @property
     def metadata(self) -> global___MessageMetadata: ...
     @property
-    def fields(self) -> google.protobuf.internal.containers.MessageMap[typing.Text, global___Value]: ...
-    def __init__(self,
-        *,
-        parent_event_id: typing.Optional[global___EventID] = ...,
-        metadata: typing.Optional[global___MessageMetadata] = ...,
-        fields: typing.Optional[typing.Mapping[typing.Text, global___Value]] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["metadata",b"metadata","parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fields",b"fields","metadata",b"metadata","parent_event_id",b"parent_event_id"]) -> None: ...
+    def fields(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___Value]: ...
+    def __init__(
+        self,
+        *,
+        parent_event_id: global___EventID | None = ...,
+        metadata: global___MessageMetadata | None = ...,
+        fields: collections.abc.Mapping[builtins.str, global___Value] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata", "parent_event_id", b"parent_event_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["fields", b"fields", "metadata", b"metadata", "parent_event_id", b"parent_event_id"]) -> None: ...
+
 global___Message = Message
 
+@typing_extensions.final
 class RawMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     METADATA_FIELD_NUMBER: builtins.int
     BODY_FIELD_NUMBER: builtins.int
     @property
     def parent_event_id(self) -> global___EventID:
         """It maybe used to store event related to message life cycle"""
-        pass
     @property
     def metadata(self) -> global___RawMessageMetadata: ...
     body: builtins.bytes
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        parent_event_id: typing.Optional[global___EventID] = ...,
-        metadata: typing.Optional[global___RawMessageMetadata] = ...,
+        parent_event_id: global___EventID | None = ...,
+        metadata: global___RawMessageMetadata | None = ...,
         body: builtins.bytes = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["metadata",b"metadata","parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["body",b"body","metadata",b"metadata","parent_event_id",b"parent_event_id"]) -> None: ...
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata", "parent_event_id", b"parent_event_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["body", b"body", "metadata", b"metadata", "parent_event_id", b"parent_event_id"]) -> None: ...
+
 global___RawMessage = RawMessage
 
+@typing_extensions.final
 class AnyMessage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MESSAGE_FIELD_NUMBER: builtins.int
     RAW_MESSAGE_FIELD_NUMBER: builtins.int
     @property
     def message(self) -> global___Message: ...
     @property
     def raw_message(self) -> global___RawMessage: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        message: typing.Optional[global___Message] = ...,
-        raw_message: typing.Optional[global___RawMessage] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["kind",b"kind","message",b"message","raw_message",b"raw_message"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kind",b"kind","message",b"message","raw_message",b"raw_message"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind",b"kind"]) -> typing.Optional[typing_extensions.Literal["message","raw_message"]]: ...
+        message: global___Message | None = ...,
+        raw_message: global___RawMessage | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["kind", b"kind", "message", b"message", "raw_message", b"raw_message"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["kind", b"kind", "message", b"message", "raw_message", b"raw_message"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["message", "raw_message"] | None: ...
+
 global___AnyMessage = AnyMessage
 
+@typing_extensions.final
 class MessageGroup(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MESSAGES_FIELD_NUMBER: builtins.int
     @property
     def messages(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___AnyMessage]: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        messages: typing.Optional[typing.Iterable[global___AnyMessage]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["messages",b"messages"]) -> None: ...
+        messages: collections.abc.Iterable[global___AnyMessage] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["messages", b"messages"]) -> None: ...
+
 global___MessageGroup = MessageGroup
 
+@typing_extensions.final
 class MessageBatch(google.protobuf.message.Message):
-    """--// Message batch //--//
+    """--// Message batch //--//"""
 
-    """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MESSAGES_FIELD_NUMBER: builtins.int
     @property
     def messages(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Message]: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        messages: typing.Optional[typing.Iterable[global___Message]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["messages",b"messages"]) -> None: ...
+        messages: collections.abc.Iterable[global___Message] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["messages", b"messages"]) -> None: ...
+
 global___MessageBatch = MessageBatch
 
+@typing_extensions.final
 class RawMessageBatch(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MESSAGES_FIELD_NUMBER: builtins.int
     @property
     def messages(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___RawMessage]: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        messages: typing.Optional[typing.Iterable[global___RawMessage]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["messages",b"messages"]) -> None: ...
+        messages: collections.abc.Iterable[global___RawMessage] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["messages", b"messages"]) -> None: ...
+
 global___RawMessageBatch = RawMessageBatch
 
+@typing_extensions.final
 class MessageGroupBatch(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     METADATA_FIELD_NUMBER: builtins.int
     GROUPS_FIELD_NUMBER: builtins.int
     @property
     def metadata(self) -> global___MessageGroupBatchMetadata: ...
     @property
     def groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MessageGroup]: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        metadata: typing.Optional[global___MessageGroupBatchMetadata] = ...,
-        groups: typing.Optional[typing.Iterable[global___MessageGroup]] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["metadata",b"metadata"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["groups",b"groups","metadata",b"metadata"]) -> None: ...
+        metadata: global___MessageGroupBatchMetadata | None = ...,
+        groups: collections.abc.Iterable[global___MessageGroup] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["groups", b"groups", "metadata", b"metadata"]) -> None: ...
+
 global___MessageGroupBatch = MessageGroupBatch
 
+@typing_extensions.final
 class RequestStatus(google.protobuf.message.Message):
-    """--// RPC call response //--//
+    """--// RPC call response //--//"""
 
-    """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     class _Status:
-        ValueType = typing.NewType('ValueType', builtins.int)
+        ValueType = typing.NewType("ValueType", builtins.int)
         V: typing_extensions.TypeAlias = ValueType
-    class _StatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[RequestStatus._Status.ValueType], builtins.type):
+
+    class _StatusEnumTypeWrapper(google.protobuf.internal.enum_type_wrapper._EnumTypeWrapper[RequestStatus._Status.ValueType], builtins.type):  # noqa: F821
         DESCRIPTOR: google.protobuf.descriptor.EnumDescriptor
         SUCCESS: RequestStatus._Status.ValueType  # 0
         ERROR: RequestStatus._Status.ValueType  # 1
-    class Status(_Status, metaclass=_StatusEnumTypeWrapper):
-        pass
 
+    class Status(_Status, metaclass=_StatusEnumTypeWrapper): ...
     SUCCESS: RequestStatus.Status.ValueType  # 0
     ERROR: RequestStatus.Status.ValueType  # 1
 
     STATUS_FIELD_NUMBER: builtins.int
     MESSAGE_FIELD_NUMBER: builtins.int
     status: global___RequestStatus.Status.ValueType
-    message: typing.Text
-    def __init__(self,
+    message: builtins.str
+    def __init__(
+        self,
         *,
         status: global___RequestStatus.Status.ValueType = ...,
-        message: typing.Text = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["message",b"message","status",b"status"]) -> None: ...
+        message: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["message", b"message", "status", b"status"]) -> None: ...
+
 global___RequestStatus = RequestStatus
 
+@typing_extensions.final
 class ComparisonSettings(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     FAIL_UNEXPECTED_FIELD_NUMBER: builtins.int
     fail_unexpected: global___FailUnexpected.ValueType
-    def __init__(self,
+    def __init__(
+        self,
         *,
         fail_unexpected: global___FailUnexpected.ValueType = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fail_unexpected",b"fail_unexpected"]) -> None: ...
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["fail_unexpected", b"fail_unexpected"]) -> None: ...
+
 global___ComparisonSettings = ComparisonSettings
 
+@typing_extensions.final
 class RootComparisonSettings(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     IGNORE_FIELDS_FIELD_NUMBER: builtins.int
     CHECK_REPEATING_GROUP_ORDER_FIELD_NUMBER: builtins.int
     TIME_PRECISION_FIELD_NUMBER: builtins.int
     DECIMAL_PRECISION_FIELD_NUMBER: builtins.int
     @property
-    def ignore_fields(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text]:
+    def ignore_fields(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]:
         """
         These fields will not be considered during comparison. It concerns fields with simple or collection types.
         Comparison result will have the NA status for them.
         """
-        pass
     check_repeating_group_order: builtins.bool
     """
     Enables order verification in repeating groups according to defined filters.
     """
-
     @property
     def time_precision(self) -> google.protobuf.duration_pb2.Duration:
         """
         Time precision format for comparing timestamps
         """
-        pass
-    decimal_precision: typing.Text
+    decimal_precision: builtins.str
     """
     Decimal precision format for comparing numbers. E.g. 0.0001, 0.125, 125E-3 could be supported
     """
-
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        ignore_fields: typing.Optional[typing.Iterable[typing.Text]] = ...,
+        ignore_fields: collections.abc.Iterable[builtins.str] | None = ...,
         check_repeating_group_order: builtins.bool = ...,
-        time_precision: typing.Optional[google.protobuf.duration_pb2.Duration] = ...,
-        decimal_precision: typing.Text = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["time_precision",b"time_precision"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["check_repeating_group_order",b"check_repeating_group_order","decimal_precision",b"decimal_precision","ignore_fields",b"ignore_fields","time_precision",b"time_precision"]) -> None: ...
+        time_precision: google.protobuf.duration_pb2.Duration | None = ...,
+        decimal_precision: builtins.str = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["time_precision", b"time_precision"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["check_repeating_group_order", b"check_repeating_group_order", "decimal_precision", b"decimal_precision", "ignore_fields", b"ignore_fields", "time_precision", b"time_precision"]) -> None: ...
+
 global___RootComparisonSettings = RootComparisonSettings
 
+@typing_extensions.final
 class ValueFilter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     OPERATION_FIELD_NUMBER: builtins.int
     KEY_FIELD_NUMBER: builtins.int
     SIMPLE_FILTER_FIELD_NUMBER: builtins.int
     MESSAGE_FILTER_FIELD_NUMBER: builtins.int
     LIST_FILTER_FIELD_NUMBER: builtins.int
     SIMPLE_LIST_FIELD_NUMBER: builtins.int
     NULL_VALUE_FIELD_NUMBER: builtins.int
     operation: global___FilterOperation.ValueType
     key: builtins.bool
-    simple_filter: typing.Text
+    simple_filter: builtins.str
     @property
     def message_filter(self) -> global___MessageFilter: ...
     @property
     def list_filter(self) -> global___ListValueFilter: ...
     @property
     def simple_list(self) -> global___SimpleList: ...
     null_value: global___NullValue.ValueType
-    def __init__(self,
+    def __init__(
+        self,
         *,
         operation: global___FilterOperation.ValueType = ...,
         key: builtins.bool = ...,
-        simple_filter: typing.Text = ...,
-        message_filter: typing.Optional[global___MessageFilter] = ...,
-        list_filter: typing.Optional[global___ListValueFilter] = ...,
-        simple_list: typing.Optional[global___SimpleList] = ...,
+        simple_filter: builtins.str = ...,
+        message_filter: global___MessageFilter | None = ...,
+        list_filter: global___ListValueFilter | None = ...,
+        simple_list: global___SimpleList | None = ...,
         null_value: global___NullValue.ValueType = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["kind",b"kind","list_filter",b"list_filter","message_filter",b"message_filter","null_value",b"null_value","simple_filter",b"simple_filter","simple_list",b"simple_list"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["key",b"key","kind",b"kind","list_filter",b"list_filter","message_filter",b"message_filter","null_value",b"null_value","operation",b"operation","simple_filter",b"simple_filter","simple_list",b"simple_list"]) -> None: ...
-    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind",b"kind"]) -> typing.Optional[typing_extensions.Literal["simple_filter","message_filter","list_filter","simple_list","null_value"]]: ...
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["kind", b"kind", "list_filter", b"list_filter", "message_filter", b"message_filter", "null_value", b"null_value", "simple_filter", b"simple_filter", "simple_list", b"simple_list"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "kind", b"kind", "list_filter", b"list_filter", "message_filter", b"message_filter", "null_value", b"null_value", "operation", b"operation", "simple_filter", b"simple_filter", "simple_list", b"simple_list"]) -> None: ...
+    def WhichOneof(self, oneof_group: typing_extensions.Literal["kind", b"kind"]) -> typing_extensions.Literal["simple_filter", "message_filter", "list_filter", "simple_list", "null_value"] | None: ...
+
 global___ValueFilter = ValueFilter
 
+@typing_extensions.final
 class ListValueFilter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     VALUES_FIELD_NUMBER: builtins.int
     @property
     def values(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ValueFilter]: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        values: typing.Optional[typing.Iterable[global___ValueFilter]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["values",b"values"]) -> None: ...
+        values: collections.abc.Iterable[global___ValueFilter] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["values", b"values"]) -> None: ...
+
 global___ListValueFilter = ListValueFilter
 
+@typing_extensions.final
 class SimpleList(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     SIMPLE_VALUES_FIELD_NUMBER: builtins.int
     @property
-    def simple_values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text]: ...
-    def __init__(self,
-        *,
-        simple_values: typing.Optional[typing.Iterable[typing.Text]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["simple_values",b"simple_values"]) -> None: ...
+    def simple_values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    def __init__(
+        self,
+        *,
+        simple_values: collections.abc.Iterable[builtins.str] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["simple_values", b"simple_values"]) -> None: ...
+
 global___SimpleList = SimpleList
 
+@typing_extensions.final
 class MessageFilter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class FieldsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
+        key: builtins.str
         @property
         def value(self) -> global___ValueFilter: ...
-        def __init__(self,
+        def __init__(
+            self,
             *,
-            key: typing.Text = ...,
-            value: typing.Optional[global___ValueFilter] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+            key: builtins.str = ...,
+            value: global___ValueFilter | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     FIELDS_FIELD_NUMBER: builtins.int
     COMPARISON_SETTINGS_FIELD_NUMBER: builtins.int
     @property
-    def fields(self) -> google.protobuf.internal.containers.MessageMap[typing.Text, global___ValueFilter]: ...
+    def fields(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___ValueFilter]: ...
     @property
     def comparison_settings(self) -> global___ComparisonSettings: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        fields: typing.Optional[typing.Mapping[typing.Text, global___ValueFilter]] = ...,
-        comparison_settings: typing.Optional[global___ComparisonSettings] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["comparison_settings",b"comparison_settings"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["comparison_settings",b"comparison_settings","fields",b"fields"]) -> None: ...
+        fields: collections.abc.Mapping[builtins.str, global___ValueFilter] | None = ...,
+        comparison_settings: global___ComparisonSettings | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["comparison_settings", b"comparison_settings"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["comparison_settings", b"comparison_settings", "fields", b"fields"]) -> None: ...
+
 global___MessageFilter = MessageFilter
 
+@typing_extensions.final
 class MetadataFilter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class SimpleFilter(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         OPERATION_FIELD_NUMBER: builtins.int
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         SIMPLE_LIST_FIELD_NUMBER: builtins.int
         operation: global___FilterOperation.ValueType
         key: builtins.bool
-        value: typing.Text
+        value: builtins.str
         @property
         def simple_list(self) -> global___SimpleList: ...
-        def __init__(self,
+        def __init__(
+            self,
             *,
             operation: global___FilterOperation.ValueType = ...,
             key: builtins.bool = ...,
-            value: typing.Text = ...,
-            simple_list: typing.Optional[global___SimpleList] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["filter_value",b"filter_value","simple_list",b"simple_list","value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["filter_value",b"filter_value","key",b"key","operation",b"operation","simple_list",b"simple_list","value",b"value"]) -> None: ...
-        def WhichOneof(self, oneof_group: typing_extensions.Literal["filter_value",b"filter_value"]) -> typing.Optional[typing_extensions.Literal["value","simple_list"]]: ...
+            value: builtins.str = ...,
+            simple_list: global___SimpleList | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["filter_value", b"filter_value", "simple_list", b"simple_list", "value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["filter_value", b"filter_value", "key", b"key", "operation", b"operation", "simple_list", b"simple_list", "value", b"value"]) -> None: ...
+        def WhichOneof(self, oneof_group: typing_extensions.Literal["filter_value", b"filter_value"]) -> typing_extensions.Literal["value", "simple_list"] | None: ...
 
+    @typing_extensions.final
     class PropertyFiltersEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
+        key: builtins.str
         @property
         def value(self) -> global___MetadataFilter.SimpleFilter: ...
-        def __init__(self,
+        def __init__(
+            self,
             *,
-            key: typing.Text = ...,
-            value: typing.Optional[global___MetadataFilter.SimpleFilter] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+            key: builtins.str = ...,
+            value: global___MetadataFilter.SimpleFilter | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
     PROPERTY_FILTERS_FIELD_NUMBER: builtins.int
     @property
-    def property_filters(self) -> google.protobuf.internal.containers.MessageMap[typing.Text, global___MetadataFilter.SimpleFilter]: ...
-    def __init__(self,
-        *,
-        property_filters: typing.Optional[typing.Mapping[typing.Text, global___MetadataFilter.SimpleFilter]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["property_filters",b"property_filters"]) -> None: ...
+    def property_filters(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___MetadataFilter.SimpleFilter]: ...
+    def __init__(
+        self,
+        *,
+        property_filters: collections.abc.Mapping[builtins.str, global___MetadataFilter.SimpleFilter] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["property_filters", b"property_filters"]) -> None: ...
+
 global___MetadataFilter = MetadataFilter
 
+@typing_extensions.final
 class RootMessageFilter(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     MESSAGETYPE_FIELD_NUMBER: builtins.int
     MESSAGE_FILTER_FIELD_NUMBER: builtins.int
     METADATA_FILTER_FIELD_NUMBER: builtins.int
     COMPARISON_SETTINGS_FIELD_NUMBER: builtins.int
     DESCRIPTION_FIELD_NUMBER: builtins.int
-    messageType: typing.Text
+    messageType: builtins.str
     """
     The message type to match
     """
-
     @property
     def message_filter(self) -> global___MessageFilter:
         """
         The filter to match message's content
         """
-        pass
     @property
     def metadata_filter(self) -> global___MetadataFilter:
         """
         The filter to match message's metadata content
         """
-        pass
     @property
     def comparison_settings(self) -> global___RootComparisonSettings:
         """
         Settings that will be used for comparing both filters (MessageFilter and MetadataFilter)
         """
-        pass
     @property
     def description(self) -> google.protobuf.wrappers_pb2.StringValue:
         """
         Description that may contain some information about the RootMessageFilter
         """
-        pass
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        messageType: typing.Text = ...,
-        message_filter: typing.Optional[global___MessageFilter] = ...,
-        metadata_filter: typing.Optional[global___MetadataFilter] = ...,
-        comparison_settings: typing.Optional[global___RootComparisonSettings] = ...,
-        description: typing.Optional[google.protobuf.wrappers_pb2.StringValue] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["comparison_settings",b"comparison_settings","description",b"description","message_filter",b"message_filter","metadata_filter",b"metadata_filter"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["comparison_settings",b"comparison_settings","description",b"description","messageType",b"messageType","message_filter",b"message_filter","metadata_filter",b"metadata_filter"]) -> None: ...
+        messageType: builtins.str = ...,
+        message_filter: global___MessageFilter | None = ...,
+        metadata_filter: global___MetadataFilter | None = ...,
+        comparison_settings: global___RootComparisonSettings | None = ...,
+        description: google.protobuf.wrappers_pb2.StringValue | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["comparison_settings", b"comparison_settings", "description", b"description", "message_filter", b"message_filter", "metadata_filter", b"metadata_filter"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["comparison_settings", b"comparison_settings", "description", b"description", "messageType", b"messageType", "message_filter", b"message_filter", "metadata_filter", b"metadata_filter"]) -> None: ...
+
 global___RootMessageFilter = RootMessageFilter
 
+@typing_extensions.final
 class Checkpoint(google.protobuf.message.Message):
-    """--// Checkpoint //--//
+    """--// Checkpoint //--//"""
 
-    """
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    @typing_extensions.final
     class BookNameToSessionAliasToDirectionCheckpointEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
-        key: typing.Text
+        key: builtins.str
         @property
         def value(self) -> global___Checkpoint.SessionAliasToDirectionCheckpoint: ...
-        def __init__(self,
+        def __init__(
+            self,
             *,
-            key: typing.Text = ...,
-            value: typing.Optional[global___Checkpoint.SessionAliasToDirectionCheckpoint] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+            key: builtins.str = ...,
+            value: global___Checkpoint.SessionAliasToDirectionCheckpoint | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
+    @typing_extensions.final
     class SessionAliasToDirectionCheckpoint(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        @typing_extensions.final
         class SessionAliasToDirectionCheckpointEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
-            key: typing.Text
+            key: builtins.str
             @property
             def value(self) -> global___Checkpoint.DirectionCheckpoint: ...
-            def __init__(self,
+            def __init__(
+                self,
                 *,
-                key: typing.Text = ...,
-                value: typing.Optional[global___Checkpoint.DirectionCheckpoint] = ...,
-                ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+                key: builtins.str = ...,
+                value: global___Checkpoint.DirectionCheckpoint | None = ...,
+            ) -> None: ...
+            def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
         SESSION_ALIAS_TO_DIRECTION_CHECKPOINT_FIELD_NUMBER: builtins.int
         @property
-        def session_alias_to_direction_checkpoint(self) -> google.protobuf.internal.containers.MessageMap[typing.Text, global___Checkpoint.DirectionCheckpoint]: ...
-        def __init__(self,
+        def session_alias_to_direction_checkpoint(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___Checkpoint.DirectionCheckpoint]: ...
+        def __init__(
+            self,
             *,
-            session_alias_to_direction_checkpoint: typing.Optional[typing.Mapping[typing.Text, global___Checkpoint.DirectionCheckpoint]] = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["session_alias_to_direction_checkpoint",b"session_alias_to_direction_checkpoint"]) -> None: ...
+            session_alias_to_direction_checkpoint: collections.abc.Mapping[builtins.str, global___Checkpoint.DirectionCheckpoint] | None = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["session_alias_to_direction_checkpoint", b"session_alias_to_direction_checkpoint"]) -> None: ...
 
+    @typing_extensions.final
     class DirectionCheckpoint(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        @typing_extensions.final
         class DirectionToCheckpointDataEntry(google.protobuf.message.Message):
             DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
             KEY_FIELD_NUMBER: builtins.int
             VALUE_FIELD_NUMBER: builtins.int
             key: builtins.int
             @property
             def value(self) -> global___Checkpoint.CheckpointData: ...
-            def __init__(self,
+            def __init__(
+                self,
                 *,
                 key: builtins.int = ...,
-                value: typing.Optional[global___Checkpoint.CheckpointData] = ...,
-                ) -> None: ...
-            def HasField(self, field_name: typing_extensions.Literal["value",b"value"]) -> builtins.bool: ...
-            def ClearField(self, field_name: typing_extensions.Literal["key",b"key","value",b"value"]) -> None: ...
+                value: global___Checkpoint.CheckpointData | None = ...,
+            ) -> None: ...
+            def HasField(self, field_name: typing_extensions.Literal["value", b"value"]) -> builtins.bool: ...
+            def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
         DIRECTION_TO_CHECKPOINT_DATA_FIELD_NUMBER: builtins.int
         @property
         def direction_to_checkpoint_data(self) -> google.protobuf.internal.containers.MessageMap[builtins.int, global___Checkpoint.CheckpointData]: ...
-        def __init__(self,
+        def __init__(
+            self,
             *,
-            direction_to_checkpoint_data: typing.Optional[typing.Mapping[builtins.int, global___Checkpoint.CheckpointData]] = ...,
-            ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["direction_to_checkpoint_data",b"direction_to_checkpoint_data"]) -> None: ...
+            direction_to_checkpoint_data: collections.abc.Mapping[builtins.int, global___Checkpoint.CheckpointData] | None = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["direction_to_checkpoint_data", b"direction_to_checkpoint_data"]) -> None: ...
 
+    @typing_extensions.final
     class CheckpointData(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
         SEQUENCE_FIELD_NUMBER: builtins.int
         TIMESTAMP_FIELD_NUMBER: builtins.int
         sequence: builtins.int
         """Message sequence number in session"""
-
         @property
         def timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp:
             """Message creation timestamp"""
-            pass
-        def __init__(self,
+        def __init__(
+            self,
             *,
             sequence: builtins.int = ...,
-            timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-            ) -> None: ...
-        def HasField(self, field_name: typing_extensions.Literal["timestamp",b"timestamp"]) -> builtins.bool: ...
-        def ClearField(self, field_name: typing_extensions.Literal["sequence",b"sequence","timestamp",b"timestamp"]) -> None: ...
+            timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+        ) -> None: ...
+        def HasField(self, field_name: typing_extensions.Literal["timestamp", b"timestamp"]) -> builtins.bool: ...
+        def ClearField(self, field_name: typing_extensions.Literal["sequence", b"sequence", "timestamp", b"timestamp"]) -> None: ...
 
     ID_FIELD_NUMBER: builtins.int
     BOOK_NAME_TO_SESSION_ALIAS_TO_DIRECTION_CHECKPOINT_FIELD_NUMBER: builtins.int
-    id: typing.Text
+    id: builtins.str
     @property
-    def book_name_to_session_alias_to_direction_checkpoint(self) -> google.protobuf.internal.containers.MessageMap[typing.Text, global___Checkpoint.SessionAliasToDirectionCheckpoint]: ...
-    def __init__(self,
-        *,
-        id: typing.Text = ...,
-        book_name_to_session_alias_to_direction_checkpoint: typing.Optional[typing.Mapping[typing.Text, global___Checkpoint.SessionAliasToDirectionCheckpoint]] = ...,
-        ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_name_to_session_alias_to_direction_checkpoint",b"book_name_to_session_alias_to_direction_checkpoint","id",b"id"]) -> None: ...
+    def book_name_to_session_alias_to_direction_checkpoint(self) -> google.protobuf.internal.containers.MessageMap[builtins.str, global___Checkpoint.SessionAliasToDirectionCheckpoint]: ...
+    def __init__(
+        self,
+        *,
+        id: builtins.str = ...,
+        book_name_to_session_alias_to_direction_checkpoint: collections.abc.Mapping[builtins.str, global___Checkpoint.SessionAliasToDirectionCheckpoint] | None = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["book_name_to_session_alias_to_direction_checkpoint", b"book_name_to_session_alias_to_direction_checkpoint", "id", b"id"]) -> None: ...
+
 global___Checkpoint = Checkpoint
 
+@typing_extensions.final
 class EventID(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     ID_FIELD_NUMBER: builtins.int
     BOOK_NAME_FIELD_NUMBER: builtins.int
     SCOPE_FIELD_NUMBER: builtins.int
     START_TIMESTAMP_FIELD_NUMBER: builtins.int
-    id: typing.Text
+    id: builtins.str
     """Unique event id in TH2 deploy"""
-
-    book_name: typing.Text
-    scope: typing.Text
+    book_name: builtins.str
+    scope: builtins.str
     @property
     def start_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        id: typing.Text = ...,
-        book_name: typing.Text = ...,
-        scope: typing.Text = ...,
-        start_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["start_timestamp",b"start_timestamp"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["book_name",b"book_name","id",b"id","scope",b"scope","start_timestamp",b"start_timestamp"]) -> None: ...
+        id: builtins.str = ...,
+        book_name: builtins.str = ...,
+        scope: builtins.str = ...,
+        start_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["start_timestamp", b"start_timestamp"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["book_name", b"book_name", "id", b"id", "scope", b"scope", "start_timestamp", b"start_timestamp"]) -> None: ...
+
 global___EventID = EventID
 
+@typing_extensions.final
 class Event(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     ID_FIELD_NUMBER: builtins.int
     PARENT_ID_FIELD_NUMBER: builtins.int
     END_TIMESTAMP_FIELD_NUMBER: builtins.int
     STATUS_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
     TYPE_FIELD_NUMBER: builtins.int
     BODY_FIELD_NUMBER: builtins.int
     ATTACHED_MESSAGE_IDS_FIELD_NUMBER: builtins.int
     @property
     def id(self) -> global___EventID: ...
     @property
     def parent_id(self) -> global___EventID:
         """Event id of parent event. It is null for root event"""
-        pass
     @property
     def end_timestamp(self) -> google.protobuf.timestamp_pb2.Timestamp: ...
     status: global___EventStatus.ValueType
     """Aggregated status of current and children events which sync written."""
-
-    name: typing.Text
-    type: typing.Text
+    name: builtins.str
+    type: builtins.str
     body: builtins.bytes
     @property
     def attached_message_ids(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___MessageID]: ...
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        id: typing.Optional[global___EventID] = ...,
-        parent_id: typing.Optional[global___EventID] = ...,
-        end_timestamp: typing.Optional[google.protobuf.timestamp_pb2.Timestamp] = ...,
+        id: global___EventID | None = ...,
+        parent_id: global___EventID | None = ...,
+        end_timestamp: google.protobuf.timestamp_pb2.Timestamp | None = ...,
         status: global___EventStatus.ValueType = ...,
-        name: typing.Text = ...,
-        type: typing.Text = ...,
+        name: builtins.str = ...,
+        type: builtins.str = ...,
         body: builtins.bytes = ...,
-        attached_message_ids: typing.Optional[typing.Iterable[global___MessageID]] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["end_timestamp",b"end_timestamp","id",b"id","parent_id",b"parent_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["attached_message_ids",b"attached_message_ids","body",b"body","end_timestamp",b"end_timestamp","id",b"id","name",b"name","parent_id",b"parent_id","status",b"status","type",b"type"]) -> None: ...
+        attached_message_ids: collections.abc.Iterable[global___MessageID] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["end_timestamp", b"end_timestamp", "id", b"id", "parent_id", b"parent_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["attached_message_ids", b"attached_message_ids", "body", b"body", "end_timestamp", b"end_timestamp", "id", b"id", "name", b"name", "parent_id", b"parent_id", "status", b"status", "type", b"type"]) -> None: ...
+
 global___Event = Event
 
+@typing_extensions.final
 class EventBatch(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
     METADATA_FIELD_NUMBER: builtins.int
     PARENT_EVENT_ID_FIELD_NUMBER: builtins.int
     EVENTS_FIELD_NUMBER: builtins.int
     @property
     def metadata(self) -> global___EventBatchMetadata: ...
     @property
     def parent_event_id(self) -> global___EventID: ...
     @property
     def events(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___Event]:
         """Events optional related to between themselves. No events outside this batch should refer to the events in this batch."""
-        pass
-    def __init__(self,
+    def __init__(
+        self,
         *,
-        metadata: typing.Optional[global___EventBatchMetadata] = ...,
-        parent_event_id: typing.Optional[global___EventID] = ...,
-        events: typing.Optional[typing.Iterable[global___Event]] = ...,
-        ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["metadata",b"metadata","parent_event_id",b"parent_event_id"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["events",b"events","metadata",b"metadata","parent_event_id",b"parent_event_id"]) -> None: ...
+        metadata: global___EventBatchMetadata | None = ...,
+        parent_event_id: global___EventID | None = ...,
+        events: collections.abc.Iterable[global___Event] | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["metadata", b"metadata", "parent_event_id", b"parent_event_id"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["events", b"events", "metadata", b"metadata", "parent_event_id", b"parent_event_id"]) -> None: ...
+
 global___EventBatch = EventBatch
```

### Comparing `th2_grpc_common-4.2.0.dev4476477365/th2_grpc_common.egg-info/PKG-INFO` & `th2_grpc_common-4.3.0.dev5346500753/th2_grpc_common.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,71 @@
 Metadata-Version: 2.1
 Name: th2-grpc-common
-Version: 4.2.0.dev4476477365
+Version: 4.3.0.dev5346500753
 Summary: th2_grpc_common
 Home-page: https://github.com/th2-net/th2-grpc-common
 Author: TH2-devs
 Author-email: th2-devs@exactprosystems.com
 License: Apache License 2.0
-Description: # th2 gRPC common library (4.2.0)
+Description: # th2 gRPC common library (4.3.0)
         
-        
-        This library contains common proto messages that are used in all th2 components. See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto") file for details. <br>
-        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified repositories.
+        This library contains common proto messages that are used in all th2 components.
+        See [common.proto](https://github.com/th2-net/th2-grpc-common/blob/master/src/main/proto/th2_grpc_common/common.proto "common.proto")
+        file for details. <br>
+        Tool generates code from `.proto` files and uploads built packages (`.proto` files and generated code) to specified
+        repositories.
         
         ## How to maintain a project
+        
         1. Perform the necessary changes.
         2. Update the package version of Java in `gradle.properties` file.
         3. Update the package version of Python in `package_info.json` file.
         4. Commit everything.
         
         ### Java
+        
         If you wish to manually create and publish a package for Java, run the following command:
+        
         ```
         gradle --no-daemon clean build publish artifactoryPublish \
                -Purl=${URL} \ 
                -Puser=${USER} \
                -Ppassword=${PASSWORD}
         ```
+        
         `URL`, `USER` and `PASSWORD` are parameters for publishing.
         
         ### Python
+        
         If you wish to manually create and publish a package for Python:
+        
         1. Generate services with `Gradle`:
             ```
                gradle --no-daemon clean generateProto
             ```
            You can find the generated files by following path: `src/gen/main/services/python`
         2. Generate code from `.proto` files and publish everything using `twine`:
             ```
             pip install -r requirements.txt
             pip install twine
             python setup.py generate
             python setup.py sdist
             twine upload --repository-url ${PYPI_REPOSITORY_URL} --username ${PYPI_USER} --password ${PYPI_PASSWORD} dist/*
             ```
-            `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
+           `PYPI_REPOSITORY_URL`, `PYPI_USER` and `PYPI_PASSWORD` are parameters for publishing.
         
         ## Release notes
         
+        ### 4.3.0
+        
+        + Updated bom:4.4.0
+        + Updated grpc-service-generator:3.4.0
+        + Updated grpcio-tools:1.54.2
+        + Updated mypy-protobuf:3.4
+        
         ### 4.2.0
         
         + Added vulnerability check
         + Updated bom:4.2.0
         + Updated protoc:3.21.7
         + Updated grpc-service-generator:3.3.1
         + Downgraded grpc version from 1.50.2 to 1.48.1 according to bom
@@ -58,70 +73,81 @@
         ### 4.1.1
         
         + Added script for publishing dev-release for maven artefacts
         + Migrated to bom:4.2.0
         
         ### 4.1.0
         
-        + Added event / message batch metadata with the external_user_queue field. This field can be used to send MQ message to direct queue instead of schema routing in some cases.
+        + Added event / message batch metadata with the external_user_queue field. This field can be used to send MQ message to
+          direct queue instead of schema routing in some cases.
         
         ### 4.0.0
+        
         + Marked deprecated fields as `reserved`
         + Moved `timestamp` from `MessageMetadata`/`RawMessageMetadata` to `MessageID`
         + Moved `start_timestamp` from `Event` to `EventID`
         + Added `book_name` to `MessageID` and `EventID`
         + Added `scope` to `EventID`
-        + Added `map<string, SessionAliasToDirectionCheckpoint>` to `Checkpoint`. It describes book to session alias to direction.
+        + Added `map<string, SessionAliasToDirectionCheckpoint>` to `Checkpoint`. It describes book to session alias to
+          direction.
         + Added `EventBatchMetadata` and `MessageGroupBatchMetadata` with `external_queue` property
         
         ### 3.13.0
+        
         + Update `th2-bom` version from '3.0.0' to '4.1.0'
         
         ### 3.12.0
         
-        + Update `grpcio-tools` Python dependency version from `1.38.1` to `1.50.0` 
+        + Update `grpcio-tools` Python dependency version from `1.38.1` to `1.50.0`
         + Update `grpc` Java dependency version from `1.32.1` to `1.50.2`
         
         ### 3.11.1
         
-        + Update `mypy-protobuf` Python dependency version from `2.5` to `3.2` 
+        + Update `mypy-protobuf` Python dependency version from `2.5` to `3.2`
         
         ### 3.11.0
         
         + Added `session_group` parameter to `ConnectionID`
         
         ### 3.10.0
         
         + Updated grpc-service-generator (added support for gRPC pins filters).
         
         ### 3.9.0
         
         + Added `null_value` in `ValueFilter`. Should be used only with EQUAL and NOT_EQUAL operations.
         
         ### 3.8.0
+        
         + Added `time_precision` and `decimal_precision` parameters to `RootComparisonSettings`
-        + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operation, witch filter a field by comparing values(`date/time` in ISO format and `numeric` types) with the precision. The timestamps will be compared with the protobuf duration format. Numbers use string format, for example _0.0001_, _0.125_, _125E-3_
+        + Added `EQ_TIME_PRECISION` and `EQ_DECIMAL_PRECISION` filter operation, witch filter a field by comparing
+          values(`date/time` in ISO format and `numeric` types) with the precision. The timestamps will be compared with the
+          protobuf duration format. Numbers use string format, for example _0.0001_, _0.125_, _125E-3_
         
         ### 3.7.0
+        
         + Added `check_repeating_group_order` parameter to `RootComparisonSettings`
         
         ### 3.6.0
+        
         + Added `description` parameter to `RootMessageFilter`.
         
         ### 3.5.0
-        + Added SimpleList parameter to SimpleFilter. 
+        
+        + Added SimpleList parameter to SimpleFilter.
         
         ### 3.4.0
         
         + Added `IN` and `NOT_IN` filter operation, which filter a field by value from list of `String`.
         + Added `LIKE` and `NOT_LIKE` filter operation, which filter a field by `String` regEx expression.
-        + Added `MORE`, `LESS`, `NOT_MORE`, `NOT_LESS` filter operations, which filter a field by comparing values(`numeric` types and `date/time` in ISO format).
-        + Added `WILDCARD` and `NOT_WILDCARD`  filter operations, which filter a field by `String` specified wildcard expression.
-        The wildcard matcher uses the characters `?` and `*` to represent a single or multiple (zero or more) wildcard characters.
-        This is the same as often found on Dos/Unix command lines.
+        + Added `MORE`, `LESS`, `NOT_MORE`, `NOT_LESS` filter operations, which filter a field by comparing values(`numeric`
+          types and `date/time` in ISO format).
+        + Added `WILDCARD` and `NOT_WILDCARD`  filter operations, which filter a field by `String` specified wildcard
+          expression. The wildcard matcher uses the characters `?` and `*` to represent a single or multiple (zero or more)
+          wildcard characters. This is the same as often found on Dos/Unix command lines.
         + "abc-123", "*-123"     --&gt; true
         + "abc-123", "*-xyz"     --&gt; false
         + "abc-123", "ab*"       --&gt; true
         + "abc-123", "*-???"     --&gt; true
         + "abc-123", "*-????"    --&gt; false
         
         N.B. the sequence `*?` does not work properly at present in match strings.
```

