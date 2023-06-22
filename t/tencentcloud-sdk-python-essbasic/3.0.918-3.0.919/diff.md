# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.918.tar", last modified: Tue Jun 20 02:40:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.919.tar", last modified: Wed Jun 21 00:27:09 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.918.tar` & `tencentcloud-sdk-python-essbasic-3.0.919.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   234871 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)    51715 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)    16662 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-20 02:40:35.000000 tencentcloud-sdk-python-essbasic-3.0.918/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:40:36.000000 tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   242551 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)    52742 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)    16662 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:27:09.000000 tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1789,14 +1789,71 @@
                 self.Employees.append(obj)
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class ChannelDescribeFlowComponentsRequest(AbstractModel):
+    """ChannelDescribeFlowComponents请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Agent: 应用相关信息
+        :type Agent: :class:`tencentcloud.essbasic.v20210526.models.Agent`
+        :param FlowId: 电子签流程的Id
+        :type FlowId: str
+        """
+        self.Agent = None
+        self.FlowId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Agent") is not None:
+            self.Agent = Agent()
+            self.Agent._deserialize(params.get("Agent"))
+        self.FlowId = params.get("FlowId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ChannelDescribeFlowComponentsResponse(AbstractModel):
+    """ChannelDescribeFlowComponents返回参数结构体
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
 class ChannelDescribeOrganizationSealsRequest(AbstractModel):
     """ChannelDescribeOrganizationSeals请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -2393,15 +2450,46 @@
         :type ComponentHeight: float
         :param ComponentPage: 参数控件所在页码，从1开始
         :type ComponentPage: int
         :param ComponentPosX: 参数控件X位置，单位px
         :type ComponentPosX: float
         :param ComponentPosY: 参数控件Y位置，单位px
         :type ComponentPosY: float
-        :param ComponentExtra: 参数控件样式，json格式表述
+        :param ComponentExtra: 扩展参数：
+为JSON格式。
+
+ComponentType为FILL_IMAGE时，支持以下参数：
+NotMakeImageCenter：bool。是否设置图片居中。false：居中（默认）。 true: 不居中
+FillMethod: int. 填充方式。0-铺满（默认）；1-等比例缩放
+
+ComponentType为SIGN_SIGNATURE类型可以控制签署方式
+{“ComponentTypeLimit”: [“xxx”]}
+xxx可以为：
+HANDWRITE – 手写签名
+OCR_ESIGN -- AI智能识别手写签名
+ESIGN -- 个人印章类型
+SYSTEM_ESIGN -- 系统签名（该类型可以在用户签署时根据用户姓名一键生成一个签名来进行签署）
+如：{“ComponentTypeLimit”: [“SYSTEM_ESIGN”]}
+
+ComponentType为SIGN_DATE时，支持以下参数：
+1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
+2 FontSize： 数字类型，范围6-72，默认值为12
+3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
+4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
+5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
+如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
+特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
+参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
+
+ComponentType为SIGN_SEAL类型时，支持以下参数：
+1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
+参数样例： "ComponentExtra":"{\"PageRanges\":[\"PageRange\":{\"BeginPage\":1,\"EndPage\":-1}]}"
+
+
+参数控件样式，json格式表述
 
 不同类型的控件会有部分非通用参数
 
 TEXT/MULTI_LINE_TEXT控件可以指定
 1 Font：目前只支持黑体、宋体
 2 FontSize： 范围12-72
 3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
@@ -2425,15 +2513,19 @@
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙钟的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
-参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}",
+参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
+
+ComponentType为SIGN_SEAL类型时，支持以下参数：
+1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
+参数样例： "ComponentExtra":"{\"PageRanges\":[\"PageRange\":{\"BeginPage\":1,\"EndPage\":-1}]}"
         :type ComponentExtra: str
         :param ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
 CHECK_BOX - true/false
 FILL_IMAGE、ATTACHMENT - 附件的FileId，需要通过UploadFiles接口上传获取
 SELECTOR - 选项值
@@ -3661,14 +3753,59 @@
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
+        :param ImageUrl: 图片填充控件下载链接，如果是图片填充控件时，这里返回图片的下载链接。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ImageUrl: str
+        """
+        self.ComponentId = None
+        self.ComponentName = None
+        self.ComponentFillStatus = None
+        self.ComponentValue = None
+        self.ImageUrl = None
+
+
+    def _deserialize(self, params):
+        self.ComponentId = params.get("ComponentId")
+        self.ComponentName = params.get("ComponentName")
+        self.ComponentFillStatus = params.get("ComponentFillStatus")
+        self.ComponentValue = params.get("ComponentValue")
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
     """此结构体 (Filter) 用于描述查询过滤条件。
 
     """
 
     def __init__(self):
         r"""
@@ -4969,14 +5106,59 @@
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
 
 
 class ReleasedApprover(AbstractModel):
     """解除协议的签署人，如不指定，默认使用待解除流程（即原流程）中的签署人。
     注意：不支持更换C端（个人身份类型）签署人，如果原流程中含有C端签署人，默认使用原流程中的该签署人。
 
     如果需要指定B端（机构身份类型）签署人，其中ReleasedApprover需要传递的参数如下：
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,14 +523,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ChannelDescribeFlowComponents(self, request):
+        """查询流程填写控件内容，可以根据流程Id查询该流程相关联的填写控件信息
+
+        :param request: Request instance for ChannelDescribeFlowComponents.
+        :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeFlowComponentsRequest`
+        :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeFlowComponentsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ChannelDescribeFlowComponents", params, headers=headers)
+            response = json.loads(body)
+            model = models.ChannelDescribeFlowComponentsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ChannelDescribeOrganizationSeals(self, request):
         """查询子客企业电子印章，需要操作者具有管理印章权限
         客户指定需要获取的印章数量和偏移量，数量最多100，超过100按100处理；入参InfoType控制印章是否携带授权人信息，为1则携带，为0则返回的授权人信息为空数组。接口调用成功返回印章的信息列表还有企业印章的总数。
 
         :param request: Request instance for ChannelDescribeOrganizationSeals.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeOrganizationSealsRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelDescribeOrganizationSealsResponse`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.919/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.919/setup.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.918/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.919/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

