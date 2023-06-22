# Comparing `tmp/tencentcloud-sdk-python-ckafka-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-ckafka-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.918.tar", last modified: Tue Jun 20 02:36:38 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ckafka-3.0.919.tar", last modified: Wed Jun 21 00:20:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ckafka-3.0.918.tar` & `tencentcloud-sdk-python-ckafka-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   475057 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)    70499 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/ckafka_client.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud_sdk_python_ckafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      475 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1674 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1012 2023-06-20 02:36:38.000000 tencentcloud-sdk-python-ckafka-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   477031 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)    70499 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/ckafka_client.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud_sdk_python_ckafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud_sdk_python_ckafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      475 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud_sdk_python_ckafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud_sdk_python_ckafka.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1012 2023-06-21 00:20:54.000000 tencentcloud-sdk-python-ckafka-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -746,14 +746,49 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class BrokerTopicData(AbstractModel):
+    """主题占用Broker磁盘大小
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TopicName: 主题名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TopicName: str
+        :param TopicId: 主题ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TopicId: str
+        :param DataSize: 主题占用Broker 容量大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DataSize: int
+        """
+        self.TopicName = None
+        self.TopicId = None
+        self.DataSize = None
+
+
+    def _deserialize(self, params):
+        self.TopicName = params.get("TopicName")
+        self.TopicId = params.get("TopicId")
+        self.DataSize = params.get("DataSize")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class CancelAuthorizationTokenRequest(AbstractModel):
     """CancelAuthorizationToken请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6085,26 +6120,30 @@
         :type InstanceId: str
         :param RankingType: 排行类别(PRO-Topic生产流量/CON-Topic消费流量)
         :type RankingType: str
         :param BeginDate: 排行起始日期
         :type BeginDate: str
         :param EndDate: 排行结束日期
         :type EndDate: str
+        :param BrokerIp: Broker IP 地址
+        :type BrokerIp: str
         """
         self.InstanceId = None
         self.RankingType = None
         self.BeginDate = None
         self.EndDate = None
+        self.BrokerIp = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.RankingType = params.get("RankingType")
         self.BeginDate = params.get("BeginDate")
         self.EndDate = params.get("EndDate")
+        self.BrokerIp = params.get("BrokerIp")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -12068,18 +12107,26 @@
         :param TopicFlow: Topic 流量数组
         :type TopicFlow: list of TopicFlowRanking
         :param ConsumeSpeed: 消费者组消费速度排行速度
         :type ConsumeSpeed: list of ConsumerGroupSpeed
         :param TopicMessageHeap: Topic 消息堆积/占用磁盘排行
 注意：此字段可能返回 null，表示取不到有效值。
         :type TopicMessageHeap: list of TopicMessageHeapRanking
+        :param BrokerIp: Broker Ip 列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BrokerIp: list of str
+        :param BrokerTopicData: 单个broker 节点 Topic占用的数据大小
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BrokerTopicData: list of BrokerTopicData
         """
         self.TopicFlow = None
         self.ConsumeSpeed = None
         self.TopicMessageHeap = None
+        self.BrokerIp = None
+        self.BrokerTopicData = None
 
 
     def _deserialize(self, params):
         if params.get("TopicFlow") is not None:
             self.TopicFlow = []
             for item in params.get("TopicFlow"):
                 obj = TopicFlowRanking()
@@ -12093,14 +12140,21 @@
                 self.ConsumeSpeed.append(obj)
         if params.get("TopicMessageHeap") is not None:
             self.TopicMessageHeap = []
             for item in params.get("TopicMessageHeap"):
                 obj = TopicMessageHeapRanking()
                 obj._deserialize(item)
                 self.TopicMessageHeap.append(obj)
+        self.BrokerIp = params.get("BrokerIp")
+        if params.get("BrokerTopicData") is not None:
+            self.BrokerTopicData = []
+            for item in params.get("BrokerTopicData"):
+                obj = BrokerTopicData()
+                obj._deserialize(item)
+                self.BrokerTopicData.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/README.rst` & `tencentcloud-sdk-python-ckafka-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.919/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ckafka-3.0.919/tencentcloud_sdk_python_ckafka.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ckafka
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Ckafka SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ckafka-3.0.918/setup.py` & `tencentcloud-sdk-python-ckafka-3.0.919/setup.py`

 * *Files identical despite different names*

