# Comparing `tmp/tencentcloud-sdk-python-ims-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-ims-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ims-3.0.918.tar", last modified: Tue Jun 20 02:42:26 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ims-3.0.919.tar", last modified: Wed Jun 21 00:30:12 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ims-3.0.918.tar` & `tencentcloud-sdk-python-ims-3.0.919.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8549 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/ims_client.py
--rw-r--r--   0 root         (0) root         (0)    47385 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3224 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/ims_client.py
--rw-r--r--   0 root         (0) root         (0)    30860 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/models.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud_sdk_python_ims.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud_sdk_python_ims.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud_sdk_python_ims.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:42:26.000000 tencentcloud-sdk-python-ims-3.0.918/tencentcloud_sdk_python_ims.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8549 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/ims_client.py
+-rw-r--r--   0 root         (0) root         (0)    47385 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/ims_client.py
+-rw-r--r--   0 root         (0) root         (0)    30860 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/models.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-21 00:30:11.000000 tencentcloud-sdk-python-ims-3.0.919/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud_sdk_python_ims.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud_sdk_python_ims.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud_sdk_python_ims.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:30:12.000000 tencentcloud-sdk-python-ims-3.0.919/tencentcloud_sdk_python_ims.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/ims_client.py` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/ims_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/models.py` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20201229/errorcodes.py` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/ims_client.py` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/ims_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/models.py` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud/ims/v20200713/errorcodes.py` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud/ims/v20200713/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ims-3.0.918/README.rst` & `tencentcloud-sdk-python-ims-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-ims-3.0.919/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ims
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Ims SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ims-3.0.918/setup.py` & `tencentcloud-sdk-python-ims-3.0.919/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud_sdk_python_ims.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ims-3.0.918/tencentcloud_sdk_python_ims.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ims-3.0.919/tencentcloud_sdk_python_ims.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ims
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Ims SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

