# Comparing `tmp/grpcio-channelz-1.56.0.tar.gz` & `tmp/grpcio-channelz-1.56.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-channelz-1.56.0.tar", last modified: Wed Jun 14 20:38:20 2023, max compression
+gzip compressed data, was "grpcio-channelz-1.56.0rc2.tar", last modified: Mon Jun  5 20:57:23 2023, max compression
```

## Comparing `grpcio-channelz-1.56.0.tar` & `grpcio-channelz-1.56.0rc2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.908834 grpcio-channelz-1.56.0/
--rw-r--r--   0 root         (0) root         (0)    29687 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      104 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1159 2023-06-14 20:38:20.908834 grpcio-channelz-1.56.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      281 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.904834 grpcio-channelz-1.56.0/grpc_channelz/
--rw-r--r--   0 root         (0) root         (0)      580 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/grpc_channelz/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.908834 grpcio-channelz-1.56.0/grpc_channelz/v1/
--rw-r--r--   0 root         (0) root         (0)      580 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/grpc_channelz/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/grpc_channelz/v1/_async.py
--rw-r--r--   0 root         (0) root         (0)     4469 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/grpc_channelz/v1/_servicer.py
--rw-r--r--   0 root         (0) root         (0)     2419 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/grpc_channelz/v1/channelz.py
--rw-r--r--   0 root         (0) root         (0)    16425 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpc_channelz/v1/channelz_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24126 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpc_channelz/v1/channelz_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    13199 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpc_channelz/v1/channelz_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.908834 grpcio-channelz-1.56.0/grpcio_channelz.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1159 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpcio_channelz.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      721 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpcio_channelz.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpcio_channelz.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpcio_channelz.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-14 20:38:20.000000 grpcio-channelz-1.56.0/grpcio_channelz.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 20:38:20.908834 grpcio-channelz-1.56.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3250 2023-06-14 20:30:35.000000 grpcio-channelz-1.56.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:23.336161 grpcio-channelz-1.56.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    29687 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      104 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-06-05 20:57:23.336161 grpcio-channelz-1.56.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      281 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:23.332161 grpcio-channelz-1.56.0rc2/grpc_channelz/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:23.336161 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/
+-rw-r--r--   0 root         (0) root         (0)      580 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/_async.py
+-rw-r--r--   0 root         (0) root         (0)     4469 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/_servicer.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz.py
+-rw-r--r--   0 root         (0) root         (0)    16425 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24126 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    13199 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:23.336161 grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1162 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      721 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-05 20:57:23.000000 grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 20:57:23.336161 grpcio-channelz-1.56.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3250 2023-06-05 20:49:43.000000 grpcio-channelz-1.56.0rc2/setup.py
```

### Comparing `grpcio-channelz-1.56.0/LICENSE` & `grpcio-channelz-1.56.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/PKG-INFO` & `grpcio-channelz-1.56.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.56.0
+Version: 1.56.0rc2
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/__init__.py` & `grpcio-channelz-1.56.0rc2/grpc_channelz/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/v1/__init__.py` & `grpcio-channelz-1.56.0rc2/grpc_channelz/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/v1/_async.py` & `grpcio-channelz-1.56.0rc2/grpc_channelz/v1/_async.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/v1/_servicer.py` & `grpcio-channelz-1.56.0rc2/grpc_channelz/v1/_servicer.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/v1/channelz.py` & `grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/v1/channelz_pb2.py` & `grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz_pb2.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/v1/channelz_pb2.pyi` & `grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz_pb2.pyi`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_channelz/v1/channelz_pb2_grpc.py` & `grpcio-channelz-1.56.0rc2/grpc_channelz/v1/channelz_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/grpc_version.py` & `grpcio-channelz-1.56.0rc2/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_channelz/grpc_version.py.template`!!!
 
-VERSION = '1.56.0'
+VERSION = '1.56.0rc2'
```

### Comparing `grpcio-channelz-1.56.0/grpcio_channelz.egg-info/PKG-INFO` & `grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-channelz
-Version: 1.56.0
+Version: 1.56.0rc2
 Summary: Channel Level Live Debug Information Service for gRPC
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-channelz-1.56.0/grpcio_channelz.egg-info/SOURCES.txt` & `grpcio-channelz-1.56.0rc2/grpcio_channelz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-channelz-1.56.0/setup.py` & `grpcio-channelz-1.56.0rc2/setup.py`

 * *Files identical despite different names*

