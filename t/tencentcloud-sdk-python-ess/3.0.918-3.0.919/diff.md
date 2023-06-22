# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.918.tar", last modified: Tue Jun 20 02:40:29 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.919.tar", last modified: Wed Jun 21 00:27:02 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.918.tar` & `tencentcloud-sdk-python-ess-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252397 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)    58476 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24640 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-06-20 02:40:29.000000 tencentcloud-sdk-python-ess-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   258617 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)    59451 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24640 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-21 00:27:02.000000 tencentcloud-sdk-python-ess-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-ess-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -724,15 +724,19 @@
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
-参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}",
+参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
+
+ComponentType为SIGN_SEAL类型时，支持以下参数：
+1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
+参数样例： "ComponentExtra":"{\"PageRanges\":[\"PageRange\":{\"BeginPage\":1,\"EndPage\":-1}]}"
         :type ComponentExtra: str
         :param IsFormType: 是否是表单域类型，默认不false-不是
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsFormType: bool
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
@@ -3299,14 +3303,77 @@
             for item in params.get("FlowBriefs"):
                 obj = FlowBrief()
                 obj._deserialize(item)
                 self.FlowBriefs.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeFlowComponentsRequest(AbstractModel):
+    """DescribeFlowComponents请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Operator: 操作者信息
+        :type Operator: :class:`tencentcloud.ess.v20201111.models.UserInfo`
+        :param FlowId: 电子签流程的Id
+        :type FlowId: str
+        :param Agent: 应用相关信息
+        :type Agent: :class:`tencentcloud.ess.v20201111.models.Agent`
+        """
+        self.Operator = None
+        self.FlowId = None
+        self.Agent = None
+
+
+    def _deserialize(self, params):
+        if params.get("Operator") is not None:
+            self.Operator = UserInfo()
+            self.Operator._deserialize(params.get("Operator"))
+        self.FlowId = params.get("FlowId")
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeFlowComponentsResponse(AbstractModel):
+    """DescribeFlowComponents返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RecipientComponentInfos: 流程关联的填写控件信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecipientComponentInfos: list of RecipientComponentInfo
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RecipientComponentInfos = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("RecipientComponentInfos") is not None:
+            self.RecipientComponentInfos = []
+            for item in params.get("RecipientComponentInfos"):
+                obj = RecipientComponentInfo()
+                obj._deserialize(item)
+                self.RecipientComponentInfos.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeFlowEvidenceReportRequest(AbstractModel):
     """DescribeFlowEvidenceReport请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -4459,14 +4526,64 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class FilledComponent(AbstractModel):
+    """文档内的填充控件返回结构体，返回控件的基本信息和填写内容值
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ComponentId: 控件Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ComponentId: str
+        :param ComponentName: 控件名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ComponentName: str
+        :param ComponentFillStatus: 控件填写状态；0-未填写；1-已填写
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ComponentFillStatus: str
+        :param ComponentValue: 控件填写内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ComponentValue: str
+        :param ComponentRecipientId: 控件所属参与方Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ComponentRecipientId: str
+        :param ImageUrl: 图片填充控件下载链接，如果是图片填充控件时，这里返回图片的下载链接。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageUrl: str
+        """
+        self.ComponentId = None
+        self.ComponentName = None
+        self.ComponentFillStatus = None
+        self.ComponentValue = None
+        self.ComponentRecipientId = None
+        self.ImageUrl = None
+
+
+    def _deserialize(self, params):
+        self.ComponentId = params.get("ComponentId")
+        self.ComponentName = params.get("ComponentName")
+        self.ComponentFillStatus = params.get("ComponentFillStatus")
+        self.ComponentValue = params.get("ComponentValue")
+        self.ComponentRecipientId = params.get("ComponentRecipientId")
+        self.ImageUrl = params.get("ImageUrl")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class Filter(AbstractModel):
     """查询过滤条件
 
     """
 
     def __init__(self):
         r"""
@@ -5735,14 +5852,59 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class RecipientComponentInfo(AbstractModel):
+    """参与方填写控件信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RecipientId: 参与方Id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecipientId: str
+        :param RecipientFillStatus: 参与方填写状态
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RecipientFillStatus: str
+        :param IsPromoter: 是否发起方
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsPromoter: bool
+        :param Components: 填写控件内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Components: list of FilledComponent
+        """
+        self.RecipientId = None
+        self.RecipientFillStatus = None
+        self.IsPromoter = None
+        self.Components = None
+
+
+    def _deserialize(self, params):
+        self.RecipientId = params.get("RecipientId")
+        self.RecipientFillStatus = params.get("RecipientFillStatus")
+        self.IsPromoter = params.get("IsPromoter")
+        if params.get("Components") is not None:
+            self.Components = []
+            for item in params.get("Components"):
+                obj = FilledComponent()
+                obj._deserialize(item)
+                self.Components.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class RegisterInfo(AbstractModel):
     """发起流程快速注册相关信息
 
     """
```

### Comparing `tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -832,14 +832,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeFlowComponents(self, request):
+        """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息
+
+        :param request: Request instance for DescribeFlowComponents.
+        :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowComponentsRequest`
+        :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowComponentsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeFlowComponents", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeFlowComponentsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeFlowEvidenceReport(self, request):
         """查询出证报告，返回报告 URL。
 
         :param request: Request instance for DescribeFlowEvidenceReport.
         :type request: :class:`tencentcloud.ess.v20201111.models.DescribeFlowEvidenceReportRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.DescribeFlowEvidenceReportResponse`
```

### Comparing `tencentcloud-sdk-python-ess-3.0.918/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.919/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.918/README.rst` & `tencentcloud-sdk-python-ess-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.919/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.918/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.919/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.918/setup.py` & `tencentcloud-sdk-python-ess-3.0.919/setup.py`

 * *Files identical despite different names*

