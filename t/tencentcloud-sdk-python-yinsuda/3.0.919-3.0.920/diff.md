# Comparing `tmp/tencentcloud-sdk-python-yinsuda-3.0.919.tar.gz` & `tmp/tencentcloud-sdk-python-yinsuda-3.0.920.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.919.tar", last modified: Wed Jun 21 00:41:10 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-yinsuda-3.0.920.tar", last modified: Thu Jun 22 00:39:53 2023, max compression
```

## Comparing `tencentcloud-sdk-python-yinsuda-3.0.919.tar` & `tencentcloud-sdk-python-yinsuda-3.0.920.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72966 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/models.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15889 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/yinsuda_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud_sdk_python_yinsuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/README.rst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-21 00:41:10.000000 tencentcloud-sdk-python-yinsuda-3.0.919/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77103 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/models.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    16900 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/yinsuda_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud_sdk_python_yinsuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud_sdk_python_yinsuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud_sdk_python_yinsuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud_sdk_python_yinsuda.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-22 00:39:53.000000 tencentcloud-sdk-python-yinsuda-3.0.920/setup.py
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/__init__.py` & `tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/models.py` & `tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -355,14 +355,111 @@
             for item in params.get("NotMatchRuleSet"):
                 obj = KTVMatchRule()
                 obj._deserialize(item)
                 self.NotMatchRuleSet.append(obj)
         self.RequestId = params.get("RequestId")
 
 
+class DescribeKTVMusicAccompanySegmentUrlRequest(AbstractModel):
+    """DescribeKTVMusicAccompanySegmentUrl请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param AppName: 应用名称。
+        :type AppName: str
+        :param UserId: 用户标识。
+        :type UserId: str
+        :param MusicId: 歌曲 Id 。
+        :type MusicId: str
+        :param PlayScene: 播放场景。默认为Chat
+<li>Live：直播</li><li>Chat：语聊</li>
+        :type PlayScene: str
+        :param RoomId: 房间Id
+        :type RoomId: str
+        """
+        self.AppName = None
+        self.UserId = None
+        self.MusicId = None
+        self.PlayScene = None
+        self.RoomId = None
+
+
+    def _deserialize(self, params):
+        self.AppName = params.get("AppName")
+        self.UserId = params.get("UserId")
+        self.MusicId = params.get("MusicId")
+        self.PlayScene = params.get("PlayScene")
+        self.RoomId = params.get("RoomId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeKTVMusicAccompanySegmentUrlResponse(AbstractModel):
+    """DescribeKTVMusicAccompanySegmentUrl返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Status: 歌曲状态。
+0：可用
+1：下线
+2：没权限
+3：没伴奏
+当返回2时，其他参数有可能全部为空
+        :type Status: int
+        :param Url: 伴奏链接
+        :type Url: str
+        :param ExtName: 伴奏类型，如mkv，mp3等
+        :type ExtName: str
+        :param SegmentBegin: 高潮开始时间
+        :type SegmentBegin: int
+        :param SegmentEnd: 高潮结束时间
+        :type SegmentEnd: int
+        :param FileSize: 链接文件大小 单位 字节
+        :type FileSize: int
+        :param OtherSegments: 其它片段时间（可用于抢唱）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OtherSegments: list of KTVOtherSegments
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Status = None
+        self.Url = None
+        self.ExtName = None
+        self.SegmentBegin = None
+        self.SegmentEnd = None
+        self.FileSize = None
+        self.OtherSegments = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.Status = params.get("Status")
+        self.Url = params.get("Url")
+        self.ExtName = params.get("ExtName")
+        self.SegmentBegin = params.get("SegmentBegin")
+        self.SegmentEnd = params.get("SegmentEnd")
+        self.FileSize = params.get("FileSize")
+        if params.get("OtherSegments") is not None:
+            self.OtherSegments = []
+            for item in params.get("OtherSegments"):
+                obj = KTVOtherSegments()
+                obj._deserialize(item)
+                self.OtherSegments.append(obj)
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeKTVMusicsByTagRequest(AbstractModel):
     """DescribeKTVMusicsByTag请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1252,14 +1349,44 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class KTVOtherSegments(AbstractModel):
+    """其它片段时间（可用于抢唱）
+
+    """
+
+    def __init__(self):
+        r"""
+        :param SegmentBegin: 片段开始时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SegmentBegin: int
+        :param SegmentEnd: 片段结束时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SegmentEnd: int
+        """
+        self.SegmentBegin = None
+        self.SegmentEnd = None
+
+
+    def _deserialize(self, params):
+        self.SegmentBegin = params.get("SegmentBegin")
+        self.SegmentEnd = params.get("SegmentEnd")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class KTVPlaylistBaseInfo(AbstractModel):
     """歌单基础信息。
 
     """
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/errorcodes.py` & `tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud/yinsuda/v20220527/yinsuda_client.py` & `tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud/yinsuda/v20220527/yinsuda_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeKTVMusicAccompanySegmentUrl(self, request):
+        """获取歌曲伴奏片段链接，可用于抢唱
+
+        :param request: Request instance for DescribeKTVMusicAccompanySegmentUrl.
+        :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVMusicAccompanySegmentUrlRequest`
+        :rtype: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVMusicAccompanySegmentUrlResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeKTVMusicAccompanySegmentUrl", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeKTVMusicAccompanySegmentUrlResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeKTVMusicsByTag(self, request):
         """通过标签过滤歌曲列表。
 
         :param request: Request instance for DescribeKTVMusicsByTag.
         :type request: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVMusicsByTagRequest`
         :rtype: :class:`tencentcloud.yinsuda.v20220527.models.DescribeKTVMusicsByTagResponse`
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.920/tencentcloud_sdk_python_yinsuda.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.919
+Version: 3.0.920
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/README.rst` & `tencentcloud-sdk-python-yinsuda-3.0.920/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/PKG-INFO` & `tencentcloud-sdk-python-yinsuda-3.0.920/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-yinsuda
-Version: 3.0.919
+Version: 3.0.920
 Summary: Tencent Cloud Yinsuda SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-yinsuda-3.0.919/setup.py` & `tencentcloud-sdk-python-yinsuda-3.0.920/setup.py`

 * *Files identical despite different names*

