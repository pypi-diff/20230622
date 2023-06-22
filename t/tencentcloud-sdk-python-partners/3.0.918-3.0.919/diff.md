# Comparing `tmp/tencentcloud-sdk-python-partners-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-partners-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.918.tar", last modified: Tue Jun 20 02:45:42 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-partners-3.0.919.tar", last modified: Wed Jun 21 00:33:27 2023, max compression
```

## Comparing `tencentcloud-sdk-python-partners-3.0.918.tar` & `tencentcloud-sdk-python-partners-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65298 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)    19334 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/partners_client.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud_sdk_python_partners.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/tencentcloud_sdk_python_partners.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1684 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-06-20 02:45:42.000000 tencentcloud-sdk-python-partners-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65525 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)    19334 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/partners_client.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud_sdk_python_partners.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud_sdk_python_partners.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud_sdk_python_partners.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud_sdk_python_partners.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/tencentcloud_sdk_python_partners.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-06-21 00:33:27.000000 tencentcloud-sdk-python-partners-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-partners-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-partners-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/models.py` & `tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,14 +330,17 @@
         :type ProductInfo: list of ProductInfoElem
         :param PaymentMethod: 付款方式
 注意：此字段可能返回 null，表示取不到有效值。
         :type PaymentMethod: str
         :param UpdateTime: 订单更新时间
 注意：此字段可能返回 null，表示取不到有效值。
         :type UpdateTime: str
+        :param ResourceIds: 资源id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ResourceIds: list of str
         """
         self.DealId = None
         self.DealName = None
         self.GoodsCategoryId = None
         self.OwnerUin = None
         self.AppId = None
         self.GoodsNum = None
@@ -359,14 +362,15 @@
         self.SalesUin = None
         self.PayerMode = None
         self.ActivityId = None
         self.OverdueTime = None
         self.ProductInfo = None
         self.PaymentMethod = None
         self.UpdateTime = None
+        self.ResourceIds = None
 
 
     def _deserialize(self, params):
         self.DealId = params.get("DealId")
         self.DealName = params.get("DealName")
         self.GoodsCategoryId = params.get("GoodsCategoryId")
         self.OwnerUin = params.get("OwnerUin")
@@ -397,14 +401,15 @@
             self.ProductInfo = []
             for item in params.get("ProductInfo"):
                 obj = ProductInfoElem()
                 obj._deserialize(item)
                 self.ProductInfo.append(obj)
         self.PaymentMethod = params.get("PaymentMethod")
         self.UpdateTime = params.get("UpdateTime")
+        self.ResourceIds = params.get("ResourceIds")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/partners_client.py` & `tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/partners_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.918/tencentcloud/partners/v20180321/errorcodes.py` & `tencentcloud-sdk-python-partners-3.0.919/tencentcloud/partners/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.918/tencentcloud_sdk_python_partners.egg-info/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.919/tencentcloud_sdk_python_partners.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.918/README.rst` & `tencentcloud-sdk-python-partners-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-partners-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-partners-3.0.919/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-partners
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Partners SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-partners-3.0.918/setup.py` & `tencentcloud-sdk-python-partners-3.0.919/setup.py`

 * *Files identical despite different names*
