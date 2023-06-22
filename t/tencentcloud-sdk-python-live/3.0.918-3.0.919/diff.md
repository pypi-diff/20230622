# Comparing `tmp/tencentcloud-sdk-python-live-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.918.tar", last modified: Tue Jun 20 02:43:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.919.tar", last modified: Wed Jun 21 00:31:29 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.918.tar` & `tencentcloud-sdk-python-live-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   480059 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)   153149 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    19977 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1008 2023-06-20 02:43:37.000000 tencentcloud-sdk-python-live-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   483583 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)   154127 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    19977 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-21 00:31:29.000000 tencentcloud-sdk-python-live-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-live-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5393,14 +5393,61 @@
     def _deserialize(self, params):
         if params.get("PlayAuthKeyInfo") is not None:
             self.PlayAuthKeyInfo = PlayAuthKeyInfo()
             self.PlayAuthKeyInfo._deserialize(params.get("PlayAuthKeyInfo"))
         self.RequestId = params.get("RequestId")
 
 
+class DescribeLivePullStreamTaskStatusRequest(AbstractModel):
+    """DescribeLivePullStreamTaskStatus请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskId: 任务 ID。
+        :type TaskId: str
+        """
+        self.TaskId = None
+
+
+    def _deserialize(self, params):
+        self.TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeLivePullStreamTaskStatusResponse(AbstractModel):
+    """DescribeLivePullStreamTaskStatus返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param TaskStatusInfo: 任务状态信息。
+        :type TaskStatusInfo: :class:`tencentcloud.live.v20180801.models.TaskStatusInfo`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.TaskStatusInfo = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("TaskStatusInfo") is not None:
+            self.TaskStatusInfo = TaskStatusInfo()
+            self.TaskStatusInfo._deserialize(params.get("TaskStatusInfo"))
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeLivePullStreamTasksRequest(AbstractModel):
     """DescribeLivePullStreamTasks请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -12933,31 +12980,90 @@
         :type StreamName: str
         :param PublishTimeList: 推流时间列表
         :type PublishTimeList: list of PublishTime
         :param AppName: 应用名称。
         :type AppName: str
         :param DomainName: 推流域名。
         :type DomainName: str
+        :param PushToDelay: 流是否推送到延播。
+0 - 无延播，
+1 - 有延播。
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PushToDelay: int
         """
         self.StreamName = None
         self.PublishTimeList = None
         self.AppName = None
         self.DomainName = None
+        self.PushToDelay = None
 
 
     def _deserialize(self, params):
         self.StreamName = params.get("StreamName")
         if params.get("PublishTimeList") is not None:
             self.PublishTimeList = []
             for item in params.get("PublishTimeList"):
                 obj = PublishTime()
                 obj._deserialize(item)
                 self.PublishTimeList.append(obj)
         self.AppName = params.get("AppName")
         self.DomainName = params.get("DomainName")
+        self.PushToDelay = params.get("PushToDelay")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class TaskStatusInfo(AbstractModel):
+    """直播拉流任务状态信息。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FileUrl: 当前使用的源 URL。
+        :type FileUrl: str
+        :param LoopedTimes: 点播源任务的轮播次数。
+        :type LoopedTimes: int
+        :param OffsetTime: 点播源的播放偏移，单位：秒。
+        :type OffsetTime: int
+        :param ReportTime: 最新心跳上报时间。UTC时间，例如：
+2022-02-11T10:00:00Z。
+注意：UTC时间与北京时间相差八小时。
+        :type ReportTime: str
+        :param RunStatus: 实际运行状态：
+active - 活跃，
+inactive - 不活跃。
+        :type RunStatus: str
+        :param FileDuration: 点播源的文件时长，单位：秒。
+        :type FileDuration: int
+        :param NextFileUrl: 下一进度点播文件 URL。
+        :type NextFileUrl: str
+        """
+        self.FileUrl = None
+        self.LoopedTimes = None
+        self.OffsetTime = None
+        self.ReportTime = None
+        self.RunStatus = None
+        self.FileDuration = None
+        self.NextFileUrl = None
+
+
+    def _deserialize(self, params):
+        self.FileUrl = params.get("FileUrl")
+        self.LoopedTimes = params.get("LoopedTimes")
+        self.OffsetTime = params.get("OffsetTime")
+        self.ReportTime = params.get("ReportTime")
+        self.RunStatus = params.get("RunStatus")
+        self.FileDuration = params.get("FileDuration")
+        self.NextFileUrl = params.get("NextFileUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/live_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1743,14 +1743,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeLivePullStreamTaskStatus(self, request):
+        """查询直播拉流任务状态信息。
+
+        :param request: Request instance for DescribeLivePullStreamTaskStatus.
+        :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePullStreamTaskStatusRequest`
+        :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLivePullStreamTaskStatusResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeLivePullStreamTaskStatus", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeLivePullStreamTaskStatusResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeLivePullStreamTasks(self, request):
         """查询使用 CreateLivePullStreamTask 接口创建的直播拉流任务。
         排序方式：默认按更新时间 倒序排列。
 
         :param request: Request instance for DescribeLivePullStreamTasks.
         :type request: :class:`tencentcloud.live.v20180801.models.DescribeLivePullStreamTasksRequest`
         :rtype: :class:`tencentcloud.live.v20180801.models.DescribeLivePullStreamTasksResponse`
```

### Comparing `tencentcloud-sdk-python-live-3.0.918/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.919/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.918/README.rst` & `tencentcloud-sdk-python-live-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.919/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.918/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.919/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.918/setup.py` & `tencentcloud-sdk-python-live-3.0.919/setup.py`

 * *Files identical despite different names*

