# Comparing `tmp/grpcio-csds-1.56.0.tar.gz` & `tmp/grpcio-csds-1.56.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-csds-1.56.0.tar", last modified: Wed Jun 14 20:38:25 2023, max compression
+gzip compressed data, was "grpcio-csds-1.56.0rc2.tar", last modified: Mon Jun  5 20:57:28 2023, max compression
```

## Comparing `grpcio-csds-1.56.0.tar` & `grpcio-csds-1.56.0rc2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:25.457269 grpcio-csds-1.56.0/
--rw-r--r--   0 root         (0) root         (0)       94 2023-06-14 20:30:35.000000 grpcio-csds-1.56.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-14 20:38:25.457269 grpcio-csds-1.56.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      511 2023-06-14 20:30:35.000000 grpcio-csds-1.56.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:25.457269 grpcio-csds-1.56.0/grpc_csds/
--rw-r--r--   0 root         (0) root         (0)     2149 2023-06-14 20:30:35.000000 grpcio-csds-1.56.0/grpc_csds/__init__.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-14 20:30:35.000000 grpcio-csds-1.56.0/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:25.457269 grpcio-csds-1.56.0/grpcio_csds.egg-info/
--rw-r--r--   0 root         (0) root         (0)      960 2023-06-14 20:38:25.000000 grpcio-csds-1.56.0/grpcio_csds.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      267 2023-06-14 20:38:25.000000 grpcio-csds-1.56.0/grpcio_csds.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 20:38:25.000000 grpcio-csds-1.56.0/grpcio_csds.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-14 20:38:25.000000 grpcio-csds-1.56.0/grpcio_csds.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-14 20:38:25.000000 grpcio-csds-1.56.0/grpcio_csds.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 20:38:25.457269 grpcio-csds-1.56.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2120 2023-06-14 20:30:35.000000 grpcio-csds-1.56.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:28.384153 grpcio-csds-1.56.0rc2/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-05 20:49:43.000000 grpcio-csds-1.56.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      963 2023-06-05 20:57:28.384153 grpcio-csds-1.56.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-05 20:49:43.000000 grpcio-csds-1.56.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:28.380154 grpcio-csds-1.56.0rc2/grpc_csds/
+-rw-r--r--   0 root         (0) root         (0)     2149 2023-06-05 20:49:43.000000 grpcio-csds-1.56.0rc2/grpc_csds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-06-05 20:49:43.000000 grpcio-csds-1.56.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:28.384153 grpcio-csds-1.56.0rc2/grpcio_csds.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      963 2023-06-05 20:57:28.000000 grpcio-csds-1.56.0rc2/grpcio_csds.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      267 2023-06-05 20:57:28.000000 grpcio-csds-1.56.0rc2/grpcio_csds.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:57:28.000000 grpcio-csds-1.56.0rc2/grpcio_csds.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-05 20:57:28.000000 grpcio-csds-1.56.0rc2/grpcio_csds.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-05 20:57:28.000000 grpcio-csds-1.56.0rc2/grpcio_csds.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 20:57:28.384153 grpcio-csds-1.56.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-06-05 20:49:43.000000 grpcio-csds-1.56.0rc2/setup.py
```

### Comparing `grpcio-csds-1.56.0/PKG-INFO` & `grpcio-csds-1.56.0rc2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.56.0
+Version: 1.56.0rc2
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-csds-1.56.0/grpc_csds/__init__.py` & `grpcio-csds-1.56.0rc2/grpc_csds/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-csds-1.56.0/grpc_version.py` & `grpcio-csds-1.56.0rc2/grpc_version.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_csds/grpc_version.py.template`!!!
 
-VERSION = '1.56.0'
+VERSION = '1.56.0rc2'
```

### Comparing `grpcio-csds-1.56.0/grpcio_csds.egg-info/PKG-INFO` & `grpcio-csds-1.56.0rc2/grpcio_csds.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpcio-csds
-Version: 1.56.0
+Version: 1.56.0rc2
 Summary: xDS configuration dump library
 Home-page: https://grpc.io
 Author: The gRPC Authors
 Author-email: grpc-io@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `grpcio-csds-1.56.0/setup.py` & `grpcio-csds-1.56.0rc2/setup.py`

 * *Files identical despite different names*

