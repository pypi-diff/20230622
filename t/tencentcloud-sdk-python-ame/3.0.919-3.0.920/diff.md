# Comparing `tmp/tencentcloud-sdk-python-ame-3.0.919.tar.gz` & `tmp/tencentcloud-sdk-python-ame-3.0.920.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ame-3.0.919.tar", last modified: Wed Jun 21 00:16:32 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ame-3.0.920.tar", last modified: Thu Jun 22 00:15:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ame-3.0.919.tar` & `tencentcloud-sdk-python-ame-3.0.920.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud_sdk_python_ame.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud_sdk_python_ame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud_sdk_python_ame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud_sdk_python_ame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud_sdk_python_ame.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   126602 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/models.py
--rw-r--r--   0 root         (0) root         (0)    29455 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/ame_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-21 00:16:32.000000 tencentcloud-sdk-python-ame-3.0.919/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud_sdk_python_ame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud_sdk_python_ame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud_sdk_python_ame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud_sdk_python_ame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud_sdk_python_ame.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   126602 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/models.py
+-rw-r--r--   0 root         (0) root         (0)    29455 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/ame_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-22 00:15:38.000000 tencentcloud-sdk-python-ame-3.0.920/setup.py
```

### Comparing `tencentcloud-sdk-python-ame-3.0.919/tencentcloud_sdk_python_ame.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ame-3.0.920/tencentcloud_sdk_python_ame.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ame
-Version: 3.0.919
+Version: 3.0.920
 Summary: Tencent Cloud Ame SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ame-3.0.919/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ame-3.0.920/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.919'
+__version__ = '3.0.920'
```

### Comparing `tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/models.py` & `tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/ame_client.py` & `tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/ame_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.919/tencentcloud/ame/v20190916/errorcodes.py` & `tencentcloud-sdk-python-ame-3.0.920/tencentcloud/ame/v20190916/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.919/README.rst` & `tencentcloud-sdk-python-ame-3.0.920/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ame-3.0.919/PKG-INFO` & `tencentcloud-sdk-python-ame-3.0.920/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ame
-Version: 3.0.919
+Version: 3.0.920
 Summary: Tencent Cloud Ame SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ame-3.0.919/setup.py` & `tencentcloud-sdk-python-ame-3.0.920/setup.py`

 * *Files identical despite different names*
