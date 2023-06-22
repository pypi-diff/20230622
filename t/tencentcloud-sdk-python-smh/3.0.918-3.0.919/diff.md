# Comparing `tmp/tencentcloud-sdk-python-smh-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-smh-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-smh-3.0.918.tar", last modified: Tue Jun 20 02:46:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-smh-3.0.919.tar", last modified: Wed Jun 21 00:34:49 2023, max compression
```

## Comparing `tencentcloud-sdk-python-smh-3.0.918.tar` & `tencentcloud-sdk-python-smh-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud_sdk_python_smh.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud_sdk_python_smh.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud_sdk_python_smh.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud_sdk_python_smh.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud_sdk_python_smh.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9872 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/smh_client.py
--rw-r--r--   0 root         (0) root         (0)    35676 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/models.py
--rw-r--r--   0 root         (0) root         (0)     3535 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:46:52.000000 tencentcloud-sdk-python-smh-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:46:51.000000 tencentcloud-sdk-python-smh-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud_sdk_python_smh.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud_sdk_python_smh.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud_sdk_python_smh.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud_sdk_python_smh.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud_sdk_python_smh.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9872 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/smh_client.py
+-rw-r--r--   0 root         (0) root         (0)    35778 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/models.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-21 00:34:49.000000 tencentcloud-sdk-python-smh-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-smh-3.0.918/tencentcloud_sdk_python_smh.egg-info/PKG-INFO` & `tencentcloud-sdk-python-smh-3.0.919/tencentcloud_sdk_python_smh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-smh
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Smh SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-smh-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-smh-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/smh_client.py` & `tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/smh_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/models.py` & `tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,38 +23,38 @@
 
     """
 
     def __init__(self):
         r"""
         :param Name: 媒体库名称，最多 50 个字符
         :type Name: str
-        :param BucketName: 存储桶全名，新建后不可更改
+        :param Remark: 备注，最多 250 个字符
+        :type Remark: str
+        :param BucketName: 存储桶全名，新建后不可更改。当前版本不再支持指定存储桶。
         :type BucketName: str
-        :param BucketRegion: 存储桶所在地域，新建后不可更改
+        :param BucketRegion: 存储桶所在地域，新建后不可更改。当前版本不再支持指定存储桶所在地域。
         :type BucketRegion: str
         :param LibraryExtension: 媒体库配置项，部分参数新建后不可更改
         :type LibraryExtension: :class:`tencentcloud.smh.v20210712.models.LibraryExtension`
-        :param Remark: 备注，最多 250 个字符
-        :type Remark: str
         """
         self.Name = None
+        self.Remark = None
         self.BucketName = None
         self.BucketRegion = None
         self.LibraryExtension = None
-        self.Remark = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
+        self.Remark = params.get("Remark")
         self.BucketName = params.get("BucketName")
         self.BucketRegion = params.get("BucketRegion")
         if params.get("LibraryExtension") is not None:
             self.LibraryExtension = LibraryExtension()
             self.LibraryExtension._deserialize(params.get("LibraryExtension"))
-        self.Remark = params.get("Remark")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-smh-3.0.918/tencentcloud/smh/v20210712/errorcodes.py` & `tencentcloud-sdk-python-smh-3.0.919/tencentcloud/smh/v20210712/errorcodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,29 @@
 
 # 内部错误。
 INTERNALERROR = 'InternalError'
 
 # 发送短信验证码时发生错误。
 INTERNALERROR_SENDSMS = 'InternalError.SendSms'
 
+# 参数取值错误。
+INVALIDPARAMETERVALUE = 'InvalidParameterValue'
+
 # 存储桶名称无效。
 INVALIDPARAMETERVALUE_BUCKETNAMEINVALID = 'InvalidParameterValue.BucketNameInvalid'
 
 # 存储桶名称不属于当前主账号。
 INVALIDPARAMETERVALUE_BUCKETNAMENOTBELONGYOU = 'InvalidParameterValue.BucketNameNotBelongYou'
 
 # 存储桶不存在或不在指定地域。
 INVALIDPARAMETERVALUE_BUCKETNOTFOUND = 'InvalidParameterValue.BucketNotFound'
 
+# 服务已不支持自选桶
+INVALIDPARAMETERVALUE_BUCKETNOTSUPPORT = 'InvalidParameterValue.BucketNotSupport'
+
 # 存储桶所在地域无效。
 INVALIDPARAMETERVALUE_BUCKETREGIONINVALID = 'InvalidParameterValue.BucketRegionInvalid'
 
 # 指定的存储类型无效。
 INVALIDPARAMETERVALUE_COSSTORAGECLASS = 'InvalidParameterValue.CosStorageClass'
 
 # 指定的存储桶未开启智能分层存储，请先开通存储桶的智能分层存储功能。
@@ -64,17 +70,14 @@
 
 # 媒体库不存在或不属于当前账号。
 RESOURCENOTFOUND_LIBRARY = 'ResourceNotFound.Library'
 
 # 官方云盘实例不存在或不属于当前账号。
 RESOURCENOTFOUND_OFFICIALINSTANCE = 'ResourceNotFound.OfficialInstance'
 
-# 尚未开通 COS 数据处理（数据万象）服务。
-UNAUTHORIZEDOPERATION_CREATEMEDIABUCKET = 'UnauthorizedOperation.CreateMediaBucket'
-
 # 未授予 cam:PassRole 权限。
 UNAUTHORIZEDOPERATION_PASSROLE = 'UnauthorizedOperation.PassRole'
 
 # 未授予 SMH 服务相关角色。
 UNAUTHORIZEDOPERATION_SERVICELINKEDROLE = 'UnauthorizedOperation.ServiceLinkedRole'
 
 # 短信验证码错误或已过期。
```

### Comparing `tencentcloud-sdk-python-smh-3.0.918/README.rst` & `tencentcloud-sdk-python-smh-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-smh-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-smh-3.0.919/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-smh
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Smh SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-smh-3.0.918/setup.py` & `tencentcloud-sdk-python-smh-3.0.919/setup.py`

 * *Files identical despite different names*

