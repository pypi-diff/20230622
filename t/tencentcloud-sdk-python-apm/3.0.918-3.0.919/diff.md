# Comparing `tmp/tencentcloud-sdk-python-apm-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-apm-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.918.tar", last modified: Tue Jun 20 02:32:51 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-apm-3.0.919.tar", last modified: Wed Jun 21 00:17:13 2023, max compression
```

## Comparing `tencentcloud-sdk-python-apm-3.0.918.tar` & `tencentcloud-sdk-python-apm-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43549 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)     8295 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/apm_client.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud_sdk_python_apm.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:32:51.000000 tencentcloud-sdk-python-apm-3.0.918/tencentcloud_sdk_python_apm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43736 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)     8295 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/apm_client.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud_sdk_python_apm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud_sdk_python_apm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud_sdk_python_apm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud_sdk_python_apm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:17:13.000000 tencentcloud-sdk-python-apm-3.0.919/tencentcloud_sdk_python_apm.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-apm-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-apm-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/models.py` & `tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -548,31 +548,35 @@
         :type Tags: list of ApmTag
         :param InstanceName: 搜索实例名
         :type InstanceName: str
         :param InstanceIds: 过滤实例ID
         :type InstanceIds: list of str
         :param DemoInstanceFlag: 是否查询官方demo实例
         :type DemoInstanceFlag: int
+        :param AllRegionsFlag: 是否查询全地域实例
+        :type AllRegionsFlag: int
         """
         self.Tags = None
         self.InstanceName = None
         self.InstanceIds = None
         self.DemoInstanceFlag = None
+        self.AllRegionsFlag = None
 
 
     def _deserialize(self, params):
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = ApmTag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
         self.InstanceName = params.get("InstanceName")
         self.InstanceIds = params.get("InstanceIds")
         self.DemoInstanceFlag = params.get("DemoInstanceFlag")
+        self.AllRegionsFlag = params.get("AllRegionsFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/apm_client.py` & `tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/apm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.918/tencentcloud/apm/v20210622/errorcodes.py` & `tencentcloud-sdk-python-apm-3.0.919/tencentcloud/apm/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.918/README.rst` & `tencentcloud-sdk-python-apm-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.919/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-apm-3.0.918/setup.py` & `tencentcloud-sdk-python-apm-3.0.919/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-apm-3.0.918/tencentcloud_sdk_python_apm.egg-info/PKG-INFO` & `tencentcloud-sdk-python-apm-3.0.919/tencentcloud_sdk_python_apm.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-apm
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Apm SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

