# Comparing `tmp/tencentcloud-sdk-python-iotcloud-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-iotcloud-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.918.tar", last modified: Tue Jun 20 02:42:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-iotcloud-3.0.919.tar", last modified: Wed Jun 21 00:30:25 2023, max compression
```

## Comparing `tencentcloud-sdk-python-iotcloud-3.0.918.tar` & `tencentcloud-sdk-python-iotcloud-3.0.919.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud_sdk_python_iotcloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)   174274 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)    66885 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)    12818 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/__init__.py
--rw-r--r--   0 root         (0) root         (0)   175690 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/models.py
--rw-r--r--   0 root         (0) root         (0)    64286 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)    12668 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-20 02:42:37.000000 tencentcloud-sdk-python-iotcloud-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud_sdk_python_iotcloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud_sdk_python_iotcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud_sdk_python_iotcloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   174274 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)    66885 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)    12818 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   175690 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/models.py
+-rw-r--r--   0 root         (0) root         (0)    64286 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-21 00:30:25.000000 tencentcloud-sdk-python-iotcloud-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud_sdk_python_iotcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud_sdk_python_iotcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20210408/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/models.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/iotcloud_client.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/tencentcloud/iotcloud/v20180614/errorcodes.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/tencentcloud/iotcloud/v20180614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/README.rst` & `tencentcloud-sdk-python-iotcloud-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-iotcloud-3.0.919/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-iotcloud
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Iotcloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-iotcloud-3.0.918/setup.py` & `tencentcloud-sdk-python-iotcloud-3.0.919/setup.py`

 * *Files identical despite different names*

