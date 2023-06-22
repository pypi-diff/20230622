# Comparing `tmp/tencentcloud-sdk-python-kms-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-kms-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.918.tar", last modified: Tue Jun 20 02:43:21 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-kms-3.0.919.tar", last modified: Wed Jun 21 00:31:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-kms-3.0.918.tar` & `tencentcloud-sdk-python-kms-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104577 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)     5342 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50843 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/kms_client.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud_sdk_python_kms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/tencentcloud_sdk_python_kms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:43:21.000000 tencentcloud-sdk-python-kms-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104577 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50843 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/kms_client.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud_sdk_python_kms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud_sdk_python_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud_sdk_python_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud_sdk_python_kms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/tencentcloud_sdk_python_kms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-21 00:31:12.000000 tencentcloud-sdk-python-kms-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-kms-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-kms-3.0.919/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.918'
+__version__ = '3.0.919'
```

### Comparing `tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/models.py` & `tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/errorcodes.py` & `tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.918/tencentcloud/kms/v20190118/kms_client.py` & `tencentcloud-sdk-python-kms-3.0.919/tencentcloud/kms/v20190118/kms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.918/README.rst` & `tencentcloud-sdk-python-kms-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-kms-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.919/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.918/tencentcloud_sdk_python_kms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-kms-3.0.919/tencentcloud_sdk_python_kms.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-kms
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Kms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-kms-3.0.918/setup.py` & `tencentcloud-sdk-python-kms-3.0.919/setup.py`

 * *Files identical despite different names*

