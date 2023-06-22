# Comparing `tmp/tencentcloud-sdk-python-mariadb-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-mariadb-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.918.tar", last modified: Tue Jun 20 02:43:54 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-mariadb-3.0.919.tar", last modified: Wed Jun 21 00:31:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-mariadb-3.0.918.tar` & `tencentcloud-sdk-python-mariadb-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   218209 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    14932 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    70805 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/mariadb_client.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud_sdk_python_mariadb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:43:54.000000 tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223448 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    14932 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    71772 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/mariadb_client.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-21 00:31:43.000000 tencentcloud-sdk-python-mariadb-3.0.919/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud_sdk_python_mariadb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud_sdk_python_mariadb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud_sdk_python_mariadb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:31:44.000000 tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud_sdk_python_mariadb.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/models.py` & `tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2864,14 +2864,64 @@
         self.LockTimeSum = params.get("LockTimeSum")
         self.QueryCount = params.get("QueryCount")
         self.Total = params.get("Total")
         self.QueryTimeSum = params.get("QueryTimeSum")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDBTmpInstancesRequest(AbstractModel):
+    """DescribeDBTmpInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例ID
+        :type InstanceId: str
+        """
+        self.InstanceId = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDBTmpInstancesResponse(AbstractModel):
+    """DescribeDBTmpInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TmpInstances: 临时实例
+        :type TmpInstances: list of TmpInstance
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TmpInstances = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("TmpInstances") is not None:
+            self.TmpInstances = []
+            for item in params.get("TmpInstances"):
+                obj = TmpInstance()
+                obj._deserialize(item)
+                self.TmpInstances.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDatabaseObjectsRequest(AbstractModel):
     """DescribeDatabaseObjects请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6113,14 +6163,109 @@
 
 
     def _deserialize(self, params):
         self.FlowId = params.get("FlowId")
         self.RequestId = params.get("RequestId")
 
 
+class TmpInstance(AbstractModel):
+    """临时实例
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AppId: 应用ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppId: int
+        :param CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param InstanceRemark: 实例备注
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceRemark: str
+        :param TempType: 0:非临时实例 ,1:无效临时实例, 2:回档成功的有效临时实例
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TempType: int
+        :param Status: 实例状态,0:待初始化,1:流程处理中,2:有效状态,-1:已隔离，-2：已下线
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Status: int
+        :param InstanceId: 实例 ID，形如：tdsql-ow728lmc。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InstanceId: str
+        :param Vip: 实例虚IP
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Vip: str
+        :param Vport: 实例虚端口
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Vport: int
+        :param PeriodEndTime: 有效期结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PeriodEndTime: str
+        :param SrcInstanceId: 源实例 ID，形如：tdsql-ow728lmc。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SrcInstanceId: str
+        :param StatusDesc: 实例状态描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StatusDesc: str
+        :param Region: 实例所在地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Region: str
+        :param Zone: 实例所在可用区
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Zone: str
+        :param Vipv6: 实例虚IPv6
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Vipv6: str
+        :param Ipv6Flag: 实例IPv6标志
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Ipv6Flag: int
+        """
+        self.AppId = None
+        self.CreateTime = None
+        self.InstanceRemark = None
+        self.TempType = None
+        self.Status = None
+        self.InstanceId = None
+        self.Vip = None
+        self.Vport = None
+        self.PeriodEndTime = None
+        self.SrcInstanceId = None
+        self.StatusDesc = None
+        self.Region = None
+        self.Zone = None
+        self.Vipv6 = None
+        self.Ipv6Flag = None
+
+
+    def _deserialize(self, params):
+        self.AppId = params.get("AppId")
+        self.CreateTime = params.get("CreateTime")
+        self.InstanceRemark = params.get("InstanceRemark")
+        self.TempType = params.get("TempType")
+        self.Status = params.get("Status")
+        self.InstanceId = params.get("InstanceId")
+        self.Vip = params.get("Vip")
+        self.Vport = params.get("Vport")
+        self.PeriodEndTime = params.get("PeriodEndTime")
+        self.SrcInstanceId = params.get("SrcInstanceId")
+        self.StatusDesc = params.get("StatusDesc")
+        self.Region = params.get("Region")
+        self.Zone = params.get("Zone")
+        self.Vipv6 = params.get("Vipv6")
+        self.Ipv6Flag = params.get("Ipv6Flag")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class UpgradeDBInstanceRequest(AbstractModel):
     """UpgradeDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/errorcodes.py` & `tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud/mariadb/v20170312/mariadb_client.py` & `tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud/mariadb/v20170312/mariadb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -577,14 +577,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeDBTmpInstances(self, request):
+        """本接口（DescribeDBTmpInstances）用于获取实例回档生成的临时实例
+
+        :param request: Request instance for DescribeDBTmpInstances.
+        :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBTmpInstancesRequest`
+        :rtype: :class:`tencentcloud.mariadb.v20170312.models.DescribeDBTmpInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDBTmpInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDBTmpInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDatabaseObjects(self, request):
         """本接口（DescribeDatabaseObjects）用于查询云数据库实例的数据库中的对象列表，包含表、存储过程、视图和函数。
 
         :param request: Request instance for DescribeDatabaseObjects.
         :type request: :class:`tencentcloud.mariadb.v20170312.models.DescribeDatabaseObjectsRequest`
         :rtype: :class:`tencentcloud.mariadb.v20170312.models.DescribeDatabaseObjectsResponse`
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/README.rst` & `tencentcloud-sdk-python-mariadb-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.919/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/setup.py` & `tencentcloud-sdk-python-mariadb-3.0.919/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-mariadb-3.0.918/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-mariadb-3.0.919/tencentcloud_sdk_python_mariadb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-mariadb
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Mariadb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

