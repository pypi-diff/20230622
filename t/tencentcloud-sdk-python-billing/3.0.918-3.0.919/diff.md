# Comparing `tmp/tencentcloud-sdk-python-billing-3.0.918.tar.gz` & `tmp/tencentcloud-sdk-python-billing-3.0.919.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.918.tar", last modified: Tue Jun 20 02:33:36 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-billing-3.0.919.tar", last modified: Wed Jun 21 00:18:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-billing-3.0.918.tar` & `tencentcloud-sdk-python-billing-3.0.919.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/
--rw-r--r--   0 root         (0) root         (0)       88 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud_sdk_python_billing.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud_sdk_python_billing.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   167054 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)     2904 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    21124 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/billing_client.py
--rw-r--r--   0 root         (0) root         (0)      749 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/README.rst
--rw-r--r--   0 root         (0) root         (0)     1679 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1014 2023-06-20 02:33:36.000000 tencentcloud-sdk-python-billing-3.0.918/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud_sdk_python_billing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud_sdk_python_billing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud_sdk_python_billing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud_sdk_python_billing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud_sdk_python_billing.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   167451 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)     2904 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    21124 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/billing_client.py
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-21 00:18:01.000000 tencentcloud-sdk-python-billing-3.0.919/setup.py
```

### Comparing `tencentcloud-sdk-python-billing-3.0.918/tencentcloud_sdk_python_billing.egg-info/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.919/tencentcloud_sdk_python_billing.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.918/tencentcloud/__init__.py` & `tencentcloud-sdk-python-billing-3.0.919/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1876,45 +1876,49 @@
         :type PayMode: str
         :param ResourceId: 查询指定资源信息
         :type ResourceId: str
         :param ActionType: 查询交易类型（请使用交易类型名称入参），入参示例枚举如下：
 包年包月新购
 包年包月续费
 包年包月配置变更
-包年包月退款
-按量计费扣费
-按量计费小时结
-按量计费日结
-按量计费月结
-线下项目扣费
-线下产品扣费
-调账扣费
-调账补偿
-竞价实例小时结
-线下项目调账补偿
-线下产品调账补偿
-优惠扣费
-优惠补偿
-按量计费迁入资源
-按量计费迁出资源
-包年包月迁入资源
-包年包月迁出资源
-预付费用
-小时费用
-预留实例退款
-按量计费冲正
-包年包月转按量
+包年包月退款 
+按量计费扣费 
+线下项目扣费 
+线下产品扣费 
+调账扣费 
+调账补偿 
+按量计费小时结 
+按量计费日结 
+按量计费月结 
+竞价实例小时结 
+线下项目调账补偿 
+线下产品调账补偿 
+优惠扣费 
+优惠补偿 
+按量计费迁入资源 
+按量计费迁出资源 
+包年包月迁入资源 
+包年包月迁出资源 
+预付费用 
+小时费用 
+预留实例退款 
+按量计费冲正 
+包年包月转按量 
+保底扣款 
+节省计划小时费用
         :type ActionType: str
         :param ProjectId: 项目ID:资源所属项目ID
         :type ProjectId: int
         :param BusinessCode: 产品名称代码
 备注：如需获取当月使用过的BusinessCode，请调用API：<a href="https://cloud.tencent.com/document/product/555/35761">获取产品汇总费用分布</a>
         :type BusinessCode: str
         :param Context: 上一次请求返回的上下文信息，翻页查询Month>=2023-05的月份的数据可加快查询速度，数据量10万级别以上的用户建议使用，查询速度可提升2~10倍
         :type Context: str
+        :param PayerUin: 支付者的账号 ID（账号 ID 是用户在腾讯云的唯一账号标识），默认查询本账号账单，如集团管理账号需查询成员账号自付的账单，该字段需入参成员账号UIN
+        :type PayerUin: str
         """
         self.Offset = None
         self.Limit = None
         self.PeriodType = None
         self.Month = None
         self.BeginTime = None
         self.EndTime = None
@@ -1922,14 +1926,15 @@
         self.ProductCode = None
         self.PayMode = None
         self.ResourceId = None
         self.ActionType = None
         self.ProjectId = None
         self.BusinessCode = None
         self.Context = None
+        self.PayerUin = None
 
 
     def _deserialize(self, params):
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
         self.PeriodType = params.get("PeriodType")
         self.Month = params.get("Month")
@@ -1939,14 +1944,15 @@
         self.ProductCode = params.get("ProductCode")
         self.PayMode = params.get("PayMode")
         self.ResourceId = params.get("ResourceId")
         self.ActionType = params.get("ActionType")
         self.ProjectId = params.get("ProjectId")
         self.BusinessCode = params.get("BusinessCode")
         self.Context = params.get("Context")
+        self.PayerUin = params.get("PayerUin")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.918/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-billing-3.0.919/tencentcloud/billing/v20180709/billing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.918/README.rst` & `tencentcloud-sdk-python-billing-3.0.919/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-billing-3.0.918/PKG-INFO` & `tencentcloud-sdk-python-billing-3.0.919/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-billing
-Version: 3.0.918
+Version: 3.0.919
 Summary: Tencent Cloud Billing SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-billing-3.0.918/setup.py` & `tencentcloud-sdk-python-billing-3.0.919/setup.py`

 * *Files identical despite different names*

