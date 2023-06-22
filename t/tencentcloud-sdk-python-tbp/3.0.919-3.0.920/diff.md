# Comparing `tmp/tencentcloud-sdk-python-tbp-3.0.919.tar.gz` & `tmp/tencentcloud-sdk-python-tbp-3.0.920.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.919.tar", last modified: Wed Jun 21 00:36:39 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tbp-3.0.920.tar", last modified: Thu Jun 22 00:35:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tbp-3.0.919.tar` & `tencentcloud-sdk-python-tbp-3.0.920.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud_sdk_python_tbp.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13728 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/models.py
--rw-r--r--   0 root         (0) root         (0)     2682 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/tbp_client.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17397 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/models.py
--rw-r--r--   0 root         (0) root         (0)     4420 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/tbp_client.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:36:39.000000 tencentcloud-sdk-python-tbp-3.0.919/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-21 00:36:38.000000 tencentcloud-sdk-python-tbp-3.0.919/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud_sdk_python_tbp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud_sdk_python_tbp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud_sdk_python_tbp.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13728 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/models.py
+-rw-r--r--   0 root         (0) root         (0)     2682 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/tbp_client.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17453 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/models.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/tbp_client.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-22 00:35:29.000000 tencentcloud-sdk-python-tbp-3.0.920/setup.py
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud_sdk_python_tbp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud_sdk_python_tbp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.919
+Version: 3.0.920
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/models.py` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190627/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/models.py` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,23 +212,26 @@
 
     """
 
     def __init__(self):
         r"""
         :param GroupList: 消息组列表。	
 注意：此字段可能返回 null，表示取不到有效值。
-        :type GroupList: :class:`tencentcloud.tbp.v20190311.models.Group`
+        :type GroupList: list of Group
         """
         self.GroupList = None
 
 
     def _deserialize(self, params):
         if params.get("GroupList") is not None:
-            self.GroupList = Group()
-            self.GroupList._deserialize(params.get("GroupList"))
+            self.GroupList = []
+            for item in params.get("GroupList"):
+                obj = Group()
+                obj._deserialize(item)
+                self.GroupList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -328,32 +331,32 @@
         :type InputText: str
         :param SessionAttributes: 透传字段，由用户自定义的WebService服务返回。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SessionAttributes: str
         :param ResponseText: 机器人对话的应答文本。
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResponseText: str
-        :param ResponseMessage: 机器人应答。	
-注意：此字段可能返回 null，表示取不到有效值。
-        :type ResponseMessage: :class:`tencentcloud.tbp.v20190311.models.ResponseMessage`
         :param ResultType: 结果类型 {中间逻辑出错:0; 任务型机器人:1; 问答型机器人:2; 闲聊型机器人:3; 未匹配上，返回预设兜底话术:5; 未匹配上，返回相似问题列表:6}。	
 注意：此字段可能返回 null，表示取不到有效值。
         :type ResultType: str
+        :param ResponseMessage: 机器人应答。	
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResponseMessage: :class:`tencentcloud.tbp.v20190311.models.ResponseMessage`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.DialogStatus = None
         self.BotName = None
         self.IntentName = None
         self.SlotInfoList = None
         self.InputText = None
         self.SessionAttributes = None
         self.ResponseText = None
-        self.ResponseMessage = None
         self.ResultType = None
+        self.ResponseMessage = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.DialogStatus = params.get("DialogStatus")
         self.BotName = params.get("BotName")
         self.IntentName = params.get("IntentName")
@@ -362,18 +365,18 @@
             for item in params.get("SlotInfoList"):
                 obj = SlotInfo()
                 obj._deserialize(item)
                 self.SlotInfoList.append(obj)
         self.InputText = params.get("InputText")
         self.SessionAttributes = params.get("SessionAttributes")
         self.ResponseText = params.get("ResponseText")
+        self.ResultType = params.get("ResultType")
         if params.get("ResponseMessage") is not None:
             self.ResponseMessage = ResponseMessage()
             self.ResponseMessage._deserialize(params.get("ResponseMessage"))
-        self.ResultType = params.get("ResultType")
         self.RequestId = params.get("RequestId")
 
 
 class TextResetRequest(AbstractModel):
     """TextReset请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/tbp_client.py` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/tencentcloud/tbp/v20190311/errorcodes.py` & `tencentcloud-sdk-python-tbp-3.0.920/tencentcloud/tbp/v20190311/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/README.rst` & `tencentcloud-sdk-python-tbp-3.0.920/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/PKG-INFO` & `tencentcloud-sdk-python-tbp-3.0.920/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tbp
-Version: 3.0.919
+Version: 3.0.920
 Summary: Tencent Cloud Tbp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tbp-3.0.919/setup.py` & `tencentcloud-sdk-python-tbp-3.0.920/setup.py`

 * *Files identical despite different names*

