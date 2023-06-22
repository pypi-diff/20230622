# Comparing `tmp/tencentcloud-sdk-python-dnspod-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-dnspod-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.918.tar", last modified: Tue Jun 20 02:39:14 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dnspod-3.0.919.tar", last modified: Wed Jun 21 00:23:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dnspod-3.0.918.tar` & `tencentcloud-sdk-python-dnspod-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   209672 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    59836 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)    23664 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud_sdk_python_dnspod.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:39:14.000000 tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-20 02:39:13.000000 tencentcloud-sdk-python-dnspod-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   209870 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    59836 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)    23664 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud_sdk_python_dnspod.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud_sdk_python_dnspod.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud_sdk_python_dnspod.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud_sdk_python_dnspod.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-21 00:23:29.000000 tencentcloud-sdk-python-dnspod-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,28 +119,32 @@
         :type Enabled: int
         :param MX: 记录的MX权重
 注意：此字段可能返回 null，表示取不到有效值。
         :type MX: int
         :param Weight: 记录权重
 注意：此字段可能返回 null，表示取不到有效值。
         :type Weight: int
+        :param Remark: 备注信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Remark: str
         """
         self.RecordId = None
         self.SubDomain = None
         self.RecordType = None
         self.RecordLine = None
         self.Value = None
         self.TTL = None
         self.Status = None
         self.Operation = None
         self.ErrMsg = None
         self.Id = None
         self.Enabled = None
         self.MX = None
         self.Weight = None
+        self.Remark = None
 
 
     def _deserialize(self, params):
         self.RecordId = params.get("RecordId")
         self.SubDomain = params.get("SubDomain")
         self.RecordType = params.get("RecordType")
         self.RecordLine = params.get("RecordLine")
@@ -149,14 +153,15 @@
         self.Status = params.get("Status")
         self.Operation = params.get("Operation")
         self.ErrMsg = params.get("ErrMsg")
         self.Id = params.get("Id")
         self.Enabled = params.get("Enabled")
         self.MX = params.get("MX")
         self.Weight = params.get("Weight")
+        self.Remark = params.get("Remark")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/README.rst` & `tencentcloud-sdk-python-dnspod-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.919/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dnspod-3.0.919/tencentcloud_sdk_python_dnspod.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dnspod
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Dnspod SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dnspod-3.0.918/setup.py` & `tencentcloud-sdk-python-dnspod-3.0.919/setup.py`

 * *Files identical despite different names*

