# Comparing `tmp/commonX-0.4.7.tar.gz` & `tmp/commonX-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\commonX-0.4.7.tar", last modified: Mon Jun  5 14:10:45 2023, max compression
+gzip compressed data, was "dist\commonX-0.4.8.tar", last modified: Thu Jun 22 17:04:59 2023, max compression
```

## Comparing `commonX-0.4.7.tar` & `commonX-0.4.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 14:10:45.000000 commonX-0.4.7/
--rw-rw-rw-   0        0        0      714 2023-06-05 14:10:45.000000 commonX-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0       77 2023-06-05 14:09:40.000000 commonX-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/
--rw-rw-rw-   0        0        0       86 2023-06-05 14:09:40.000000 commonX-0.4.7/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/base/
--rw-rw-rw-   0        0        0      622 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/__init__.py
--rw-rw-rw-   0        0        0     1894 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/entity.py
--rw-rw-rw-   0        0        0      359 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/factory.py
--rw-rw-rw-   0        0        0     2927 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/genor.py
--rw-rw-rw-   0        0        0     2916 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/hook.py
--rw-rw-rw-   0        0        0     4135 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/logger.py
--rw-rw-rw-   0        0        0     5710 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/mapper.py
--rw-rw-rw-   0        0        0     8399 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/multi_task.py
--rw-rw-rw-   0        0        0     5194 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/packer.py
--rw-rw-rw-   0        0        0     1968 2023-06-05 14:09:40.000000 commonX-0.4.7/common/base/registry.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/ext/
--rw-rw-rw-   0        0        0      187 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/__init__.py
--rw-rw-rw-   0        0        0     2174 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/cookie_parser.py
--rw-rw-rw-   0        0        0     3845 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/iphone_client.py
--rw-rw-rw-   0        0        0      220 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/ocr_support.py
--rw-rw-rw-   0        0        0     1862 2023-06-05 14:09:40.000000 commonX-0.4.7/common/ext/qq_email.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/common/postman/
--rw-rw-rw-   0        0        0       87 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/__init__.py
--rw-rw-rw-   0        0        0     5045 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/postman_api.py
--rw-rw-rw-   0        0        0     4438 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/postman_impl.py
--rw-rw-rw-   0        0        0     4782 2023-06-05 14:09:40.000000 commonX-0.4.7/common/postman/postman_proxy.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:10:45.000000 commonX-0.4.7/common/util/
--rw-rw-rw-   0        0        0      304 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/__init__.py
--rw-rw-rw-   0        0        0      791 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/args_util.py
--rw-rw-rw-   0        0        0     2176 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/assert_util.py
--rw-rw-rw-   0        0        0     3273 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/decorator_util.py
--rw-rw-rw-   0        0        0     2725 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/exception_utll.py
--rw-rw-rw-   0        0        0     7244 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/file_util.py
--rw-rw-rw-   0        0        0     2935 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/image_util.py
--rw-rw-rw-   0        0        0     2921 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/json_util.py
--rw-rw-rw-   0        0        0     6928 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/requests_util.py
--rw-rw-rw-   0        0        0     4616 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/sys_util.py
--rw-rw-rw-   0        0        0      898 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/time_util.py
--rw-rw-rw-   0        0        0      715 2023-06-05 14:09:40.000000 commonX-0.4.7/common/util/typing_util.py
-drwxrwxrwx   0        0        0        0 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/
--rw-rw-rw-   0        0        0      714 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 14:10:44.000000 commonX-0.4.7/commonX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 14:10:45.000000 commonX-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1089 2023-06-05 14:09:40.000000 commonX-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/
+-rw-rw-rw-   0        0        0      760 2023-06-22 17:04:59.000000 commonX-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0       77 2023-06-22 17:01:37.000000 commonX-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/
+-rw-rw-rw-   0        0        0      107 2023-06-22 17:01:37.000000 commonX-0.4.8/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/base/
+-rw-rw-rw-   0        0        0      622 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/__init__.py
+-rw-rw-rw-   0        0        0     1894 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/entity.py
+-rw-rw-rw-   0        0        0      359 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/factory.py
+-rw-rw-rw-   0        0        0     2927 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/genor.py
+-rw-rw-rw-   0        0        0     2916 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/hook.py
+-rw-rw-rw-   0        0        0     4135 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/logger.py
+-rw-rw-rw-   0        0        0     5710 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/mapper.py
+-rw-rw-rw-   0        0        0     8399 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/multi_task.py
+-rw-rw-rw-   0        0        0     5194 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/packer.py
+-rw-rw-rw-   0        0        0     1968 2023-06-22 17:01:37.000000 commonX-0.4.8/common/base/registry.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/ext/
+-rw-rw-rw-   0        0        0      187 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/__init__.py
+-rw-rw-rw-   0        0        0     2174 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/cookie_parser.py
+-rw-rw-rw-   0        0        0     3845 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/iphone_client.py
+-rw-rw-rw-   0        0        0      220 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/ocr_support.py
+-rw-rw-rw-   0        0        0     1862 2023-06-22 17:01:37.000000 commonX-0.4.8/common/ext/qq_email.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/postman/
+-rw-rw-rw-   0        0        0       87 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/__init__.py
+-rw-rw-rw-   0        0        0     5045 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/postman_api.py
+-rw-rw-rw-   0        0        0     5201 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/postman_impl.py
+-rw-rw-rw-   0        0        0     4782 2023-06-22 17:01:37.000000 commonX-0.4.8/common/postman/postman_proxy.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/common/util/
+-rw-rw-rw-   0        0        0      304 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/__init__.py
+-rw-rw-rw-   0        0        0      791 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/args_util.py
+-rw-rw-rw-   0        0        0     2176 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/assert_util.py
+-rw-rw-rw-   0        0        0     3273 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/decorator_util.py
+-rw-rw-rw-   0        0        0     2725 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/exception_utll.py
+-rw-rw-rw-   0        0        0     7244 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/file_util.py
+-rw-rw-rw-   0        0        0     2935 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/image_util.py
+-rw-rw-rw-   0        0        0     2921 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/json_util.py
+-rw-rw-rw-   0        0        0     7041 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/requests_util.py
+-rw-rw-rw-   0        0        0     4611 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/sys_util.py
+-rw-rw-rw-   0        0        0      898 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/time_util.py
+-rw-rw-rw-   0        0        0      715 2023-06-22 17:01:37.000000 commonX-0.4.8/common/util/typing_util.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 17:04:59.000000 commonX-0.4.8/commonX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 17:04:59.000000 commonX-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1410 2023-06-22 17:01:37.000000 commonX-0.4.8/setup.py
```

### Comparing `commonX-0.4.7/PKG-INFO` & `commonX-0.4.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.7
+Version: 0.4.8
 Summary: python common toolkit
+Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Unix
```

### Comparing `commonX-0.4.7/common/base/__init__.py` & `commonX-0.4.8/common/base/__init__.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/entity.py` & `commonX-0.4.8/common/base/entity.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/genor.py` & `commonX-0.4.8/common/base/genor.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/hook.py` & `commonX-0.4.8/common/base/hook.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/logger.py` & `commonX-0.4.8/common/base/logger.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/mapper.py` & `commonX-0.4.8/common/base/mapper.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/multi_task.py` & `commonX-0.4.8/common/base/multi_task.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/packer.py` & `commonX-0.4.8/common/base/packer.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/base/registry.py` & `commonX-0.4.8/common/base/registry.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/ext/cookie_parser.py` & `commonX-0.4.8/common/ext/cookie_parser.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/ext/iphone_client.py` & `commonX-0.4.8/common/ext/iphone_client.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/ext/qq_email.py` & `commonX-0.4.8/common/ext/qq_email.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/postman/postman_api.py` & `commonX-0.4.8/common/postman/postman_api.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/postman/postman_impl.py` & `commonX-0.4.8/common/postman/postman_impl.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,29 +50,29 @@
     def fix_meta_data(self, meta_data):
         for k, v in self.tls_client_rename_kwargs.items():
             if k in meta_data:
                 meta_data[v] = meta_data.pop(k)
         return meta_data
 
 
-class CffiPostman(AbstractPostman):
+class CurlCffiPostman(AbstractPostman):
 
     def __init__(self, kwargs) -> None:
         super().__init__(kwargs)
 
     def __get__(self):
         from curl_cffi import requests
         return requests.get
 
     def __post__(self):
         from curl_cffi import requests
         return requests.post
 
 
-class CffiSessionPostman(AbstractSessionPostman):
+class CurlCffiSessionPostman(AbstractSessionPostman):
 
     def create_session(self, kwargs):
         return self.new_cffi_session(kwargs)
 
     # noinspection PyMethodMayBeStatic
     def new_cffi_session(self, kwargs: dict):
         from curl_cffi import requests
@@ -80,35 +80,45 @@
 
     def before_request(self, kwargs):
         return kwargs
 
 
 # help typing
 PostmanImplClazz = Union[
-    Type[CffiPostman],
-    Type[CffiSessionPostman],
+    Type[CurlCffiPostman],
+    Type[CurlCffiSessionPostman],
     Type[RequestsPostman],
     Type[RequestsSessionPostman],
     Type[TslClientSessionPostman],
 ]
 
 
 class Postmans:
     postman_impl_class_dict: Dict[str, PostmanImplClazz] = {
         'requests': RequestsPostman,
         'requests_Session': RequestsSessionPostman,
-        'cffi': CffiPostman,
-        'cffi_Session': CffiSessionPostman,
+        'cffi': CurlCffiPostman,
+        'cffi_Session': CurlCffiSessionPostman,
+        'curl_cffi': CurlCffiPostman,
+        'curl_cffi_Session': CurlCffiSessionPostman,
     }
 
     @classmethod
     def get_impl_clazz(cls, key='requests') -> PostmanImplClazz:
         return cls.postman_impl_class_dict[key]
 
     @classmethod
+    def new_session(cls, **kwargs):
+        return cls.get_impl_clazz('curl_cffi_Session').create(**kwargs)
+
+    @classmethod
+    def new_postman(cls, **kwargs):
+        return cls.get_impl_clazz('curl_cffi').create(**kwargs)
+
+    @classmethod
     def create(cls,
                filepath='./postman.yml',
                data=None,
                ) -> Postman:
         if data is None:
             from common import PackerUtil
             data = PackerUtil.unpack(filepath)[0]
@@ -135,17 +145,27 @@
 
             # 无代理，或代理已配置好好的
             if proxies is None or isinstance(proxies, dict):
                 return
 
             meta_data[key] = ProxyBuilder.build_by_str(proxies)
 
-        def impltype_handler(self, data: dict, key='type'):
-            impl_clazz = Postmans.get_impl_clazz(data.get(key, 'requests'))
-            return impl_clazz(data.get('meta_data', {}))
+        def impltype_handler(self,
+                             dsl_data: dict,
+                             __default_cname__='requests',
+                             ):
+            meta_data = dsl_data.setdefault('meta_data', {})
+            impl_type = dsl_data.get('type', __default_cname__)
+
+            # fix wrong config, but not a good solution
+            if impl_type.startswith(__default_cname__) and 'impersonate' in meta_data:
+                meta_data.pop('impersonate')
+
+            clazz = Postmans.get_impl_clazz(impl_type)
+            return clazz(meta_data)
 
         def build_postman(self, data):
             for handler in self.dsl_handler_list:
                 postman = handler(data)
                 if postman is not None:
                     return postman
```

### Comparing `commonX-0.4.7/common/postman/postman_proxy.py` & `commonX-0.4.8/common/postman/postman_proxy.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/args_util.py` & `commonX-0.4.8/common/util/args_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/assert_util.py` & `commonX-0.4.8/common/util/assert_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/decorator_util.py` & `commonX-0.4.8/common/util/decorator_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/exception_utll.py` & `commonX-0.4.8/common/util/exception_utll.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/file_util.py` & `commonX-0.4.8/common/util/file_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/image_util.py` & `commonX-0.4.8/common/util/image_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/json_util.py` & `commonX-0.4.8/common/util/json_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/requests_util.py` & `commonX-0.4.8/common/util/requests_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .typing_util import *
 from .json_util import DictModel
 
 
 class ProxyBuilder:
     proxy_protocols = ['https', 'http']
-    addr_f = 'http://{}:{}'
+    addr_f = '{}:{}'
 
     @classmethod
     def build_proxy(cls, address):
         proxies = {protocol: address for protocol in cls.proxy_protocols}
         return proxies
 
     @classmethod
@@ -21,15 +21,20 @@
 
     @classmethod
     def build_by_str(cls, text):
         """
         :param text: 127.0.0.1:1234 / clash / v2ray
         """
         proxy = getattr(cls, text + '_proxy', None)
-        return proxy() or cls.build_proxy(text)
+        if proxy is None:
+            # 127.0.0.1:1234
+            return cls.build_proxy(text)
+        else:
+            # clash_proxy
+            return proxy()
 
     v2Ray_proxy = v2ray_proxy
 
 
 def save_resp_content(resp, filepath: str):
     from .file_util import of_dir_path
     of_dir_path(filepath, mkdir=True)
```

### Comparing `commonX-0.4.7/common/util/sys_util.py` & `commonX-0.4.8/common/util/sys_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         return msgs if msgs is not None else []
 
 
 def print_sep(text='-', length=70):
     print(''.center(length, text))
 
 
-def print_eye_catching(text: str, need_to_confirm=False, surround='\n', multiple=1, key=None):
+def print_eye_catching(text, need_to_confirm=False, surround='\n', multiple=1, key=None):
     if need_to_confirm is True:
         ApplicationMessageCenter.append_msg(text, key)
     margin = surround * multiple
     print(f"{margin}{text}{margin}")
 
 
 def print_list(data: Iterable, sep='\n', **kwargs):
```

### Comparing `commonX-0.4.7/common/util/time_util.py` & `commonX-0.4.8/common/util/time_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/common/util/typing_util.py` & `commonX-0.4.8/common/util/typing_util.py`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/commonX.egg-info/PKG-INFO` & `commonX-0.4.8/commonX.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: commonX
-Version: 0.4.7
+Version: 0.4.8
 Summary: python common toolkit
+Home-page: https://github.com/hect0x7/common
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,toolkit,postman
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Unix
```

### Comparing `commonX-0.4.7/commonX.egg-info/SOURCES.txt` & `commonX-0.4.8/commonX.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commonX-0.4.7/setup.py` & `commonX-0.4.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,15 +3,25 @@
 
 from setuptools import setup, find_packages
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = "\n" + f.read()
 
-VERSION = '0.4.7'
+VERSION = None
+with open(os.path.join(here, './common/__init__.py')) as f:
+    for line in f:
+        if line.startswith("VERSION"):
+            VERSION = line[line.index("'") + 1: line.rindex("'")]
+            break
+
+if VERSION is None:
+    print('Set VERSION first!')
+    exit(1)
+
 DESCRIPTION = 'python common toolkit'
 
 setup(
     name='commonX',
     version=VERSION,
     description=DESCRIPTION,
     author='hect0x7',
@@ -31,8 +41,9 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3.7",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
     author_email='93357912+hect0x7@users.noreply.github.com',
+    url='https://github.com/hect0x7/common',
 )
```

