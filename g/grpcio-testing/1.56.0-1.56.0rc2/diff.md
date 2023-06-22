# Comparing `tmp/grpcio-testing-1.56.0.tar.gz` & `tmp/grpcio-testing-1.56.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-testing-1.56.0.tar", last modified: Wed Jun 14 20:38:20 2023, max compression
+gzip compressed data, was "grpcio-testing-1.56.0rc2.tar", last modified: Mon Jun  5 20:57:22 2023, max compression
```

## Comparing `grpcio-testing-1.56.0.tar` & `grpcio-testing-1.56.0rc2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.164763 grpcio-testing-1.56.0/
--rw-r--r--   0 root         (0) root         (0)    29687 2023-06-14 20:38:20.000000 grpcio-testing-1.56.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-14 20:38:20.164763 grpcio-testing-1.56.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.156762 grpcio-testing-1.56.0/grpc_testing/
--rw-r--r--   0 root         (0) root         (0)    22851 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.160763 grpcio-testing-1.56.0/grpc_testing/_channel/
--rw-r--r--   0 root         (0) root         (0)      887 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_channel/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_channel/_channel.py
--rw-r--r--   0 root         (0) root         (0)     3948 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_channel/_channel_rpc.py
--rw-r--r--   0 root         (0) root         (0)     1752 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_channel/_channel_state.py
--rw-r--r--   0 root         (0) root         (0)     8042 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_channel/_invocation.py
--rw-r--r--   0 root         (0) root         (0)     4781 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_channel/_multi_callable.py
--rw-r--r--   0 root         (0) root         (0)     7232 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_channel/_rpc_state.py
--rw-r--r--   0 root         (0) root         (0)     4373 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.160763 grpcio-testing-1.56.0/grpc_testing/_server/
--rw-r--r--   0 root         (0) root         (0)      823 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7405 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_server/_handler.py
--rw-r--r--   0 root         (0) root         (0)     5233 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_server/_rpc.py
--rw-r--r--   0 root         (0) root         (0)     6302 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_server/_server.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_server/_server_rpc.py
--rw-r--r--   0 root         (0) root         (0)     2860 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_server/_service.py
--rw-r--r--   0 root         (0) root         (0)     2601 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_server/_servicer_context.py
--rw-r--r--   0 root         (0) root         (0)     7209 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_testing/_time.py
--rw-r--r--   0 root         (0) root         (0)      697 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/grpc_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-14 20:38:20.164763 grpcio-testing-1.56.0/grpcio_testing.egg-info/
--rw-r--r--   0 root         (0) root         (0)      488 2023-06-14 20:38:20.000000 grpcio-testing-1.56.0/grpcio_testing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1416 2023-06-14 20:38:20.000000 grpcio-testing-1.56.0/grpcio_testing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-14 20:38:20.000000 grpcio-testing-1.56.0/grpcio_testing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-14 20:38:20.000000 grpcio-testing-1.56.0/grpcio_testing.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-14 20:38:20.000000 grpcio-testing-1.56.0/grpcio_testing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-14 20:38:20.164763 grpcio-testing-1.56.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2456 2023-06-14 20:30:35.000000 grpcio-testing-1.56.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:22.420162 grpcio-testing-1.56.0rc2/
+-rw-r--r--   0 root         (0) root         (0)    29687 2023-06-05 20:57:22.000000 grpcio-testing-1.56.0rc2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      491 2023-06-05 20:57:22.420162 grpcio-testing-1.56.0rc2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:22.416162 grpcio-testing-1.56.0rc2/grpc_testing/
+-rw-r--r--   0 root         (0) root         (0)    22851 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:22.416162 grpcio-testing-1.56.0rc2/grpc_testing/_channel/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_channel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_channel/_channel.py
+-rw-r--r--   0 root         (0) root         (0)     3948 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_channel/_channel_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     1752 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_channel/_channel_state.py
+-rw-r--r--   0 root         (0) root         (0)     8042 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_channel/_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     4781 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_channel/_multi_callable.py
+-rw-r--r--   0 root         (0) root         (0)     7232 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_channel/_rpc_state.py
+-rw-r--r--   0 root         (0) root         (0)     4373 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:22.420162 grpcio-testing-1.56.0rc2/grpc_testing/_server/
+-rw-r--r--   0 root         (0) root         (0)      823 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7405 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_server/_handler.py
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_server/_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     6302 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_server/_server.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_server/_server_rpc.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_server/_service.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_server/_servicer_context.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_testing/_time.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/grpc_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 20:57:22.420162 grpcio-testing-1.56.0rc2/grpcio_testing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      491 2023-06-05 20:57:22.000000 grpcio-testing-1.56.0rc2/grpcio_testing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-06-05 20:57:22.000000 grpcio-testing-1.56.0rc2/grpcio_testing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 20:57:22.000000 grpcio-testing-1.56.0rc2/grpcio_testing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-05 20:57:22.000000 grpcio-testing-1.56.0rc2/grpcio_testing.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-05 20:57:22.000000 grpcio-testing-1.56.0rc2/grpcio_testing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-05 20:57:22.420162 grpcio-testing-1.56.0rc2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2456 2023-06-05 20:49:43.000000 grpcio-testing-1.56.0rc2/setup.py
```

### Comparing `grpcio-testing-1.56.0/LICENSE` & `grpcio-testing-1.56.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/__init__.py` & `grpcio-testing-1.56.0rc2/grpc_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_channel/__init__.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_channel/_channel.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_channel/_channel.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_channel/_channel_rpc.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_channel/_channel_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_channel/_channel_state.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_channel/_channel_state.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_channel/_invocation.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_channel/_invocation.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_channel/_multi_callable.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_channel/_multi_callable.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_channel/_rpc_state.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_channel/_rpc_state.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_common.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_common.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_server/__init__.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_server/__init__.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_server/_handler.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_server/_handler.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_server/_rpc.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_server/_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_server/_server.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_server/_server.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_server/_server_rpc.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_server/_server_rpc.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_server/_service.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_server/_service.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_server/_servicer_context.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_server/_servicer_context.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_testing/_time.py` & `grpcio-testing-1.56.0rc2/grpc_testing/_time.py`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/grpc_version.py` & `grpcio-testing-1.56.0rc2/grpc_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # AUTO-GENERATED FROM `$REPO_ROOT/templates/src/python/grpcio_testing/grpc_version.py.template`!!!
 
-VERSION = '1.56.0'
+VERSION = '1.56.0rc2'
```

### Comparing `grpcio-testing-1.56.0/grpcio_testing.egg-info/SOURCES.txt` & `grpcio-testing-1.56.0rc2/grpcio_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grpcio-testing-1.56.0/setup.py` & `grpcio-testing-1.56.0rc2/setup.py`

 * *Files identical despite different names*

