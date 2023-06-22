# Comparing `tmp/dvadmin-sms-1.0.6.tar.gz` & `tmp/dvadmin-sms-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvadmin-sms-1.0.6.tar", last modified: Thu Jun 22 09:40:32 2023, max compression
+gzip compressed data, was "dvadmin-sms-1.0.7.tar", last modified: Thu Jun 22 10:13:37 2023, max compression
```

## Comparing `dvadmin-sms-1.0.6.tar` & `dvadmin-sms-1.0.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.105230 dvadmin-sms-1.0.6/
--rw-r--r--   0 liqiang    (501) staff       (20)     1072 2023-03-28 22:21:13.000000 dvadmin-sms-1.0.6/LICENSE
--rw-r--r--   0 liqiang    (501) staff       (20)       36 2023-06-22 09:39:55.000000 dvadmin-sms-1.0.6/MANIFEST.in
--rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-22 09:40:32.104843 dvadmin-sms-1.0.6/PKG-INFO
--rw-r--r--   0 liqiang    (501) staff       (20)     2036 2023-04-05 15:36:58.000000 dvadmin-sms-1.0.6/README.md
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.097267 dvadmin-sms-1.0.6/dvadmin_sms/
--rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/__init__.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.100581 dvadmin-sms-1.0.6/dvadmin_sms/api/
--rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/api/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)     1902 2023-06-12 03:50:27.000000 dvadmin-sms-1.0.6/dvadmin_sms/api/alibabacloud.py
--rw-r--r--   0 liqiang    (501) staff       (20)     2424 2023-03-29 07:31:38.000000 dvadmin-sms-1.0.6/dvadmin_sms/api/tencent_cloud.py
--rw-r--r--   0 liqiang    (501) staff       (20)      184 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.6/dvadmin_sms/apps.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.102871 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/
--rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)      703 2023-03-28 22:58:05.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_dictionary.json
--rw-r--r--   0 liqiang    (501) staff       (20)        4 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_menu.json
--rw-r--r--   0 liqiang    (501) staff       (20)     7592 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_systemconfig.json
--rw-r--r--   0 liqiang    (501) staff       (20)     1139 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/initialize.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.103356 dvadmin-sms-1.0.6/dvadmin_sms/migrations/
--rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-21 07:15:07.000000 dvadmin-sms-1.0.6/dvadmin_sms/migrations/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/models.py
--rw-r--r--   0 liqiang    (501) staff       (20)      741 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.6/dvadmin_sms/settings.py
--rw-r--r--   0 liqiang    (501) staff       (20)      287 2023-03-28 23:45:43.000000 dvadmin-sms-1.0.6/dvadmin_sms/urls.py
--rw-r--r--   0 liqiang    (501) staff       (20)     2441 2023-03-29 08:20:32.000000 dvadmin-sms-1.0.6/dvadmin_sms/utils.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.104345 dvadmin-sms-1.0.6/dvadmin_sms/views/
--rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/views/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)     1934 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.6/dvadmin_sms/views/send_sms.py
--rw-r--r--   0 liqiang    (501) staff       (20)     1792 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/wechat.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.099372 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/
--rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/PKG-INFO
--rw-r--r--   0 liqiang    (501) staff       (20)      758 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/SOURCES.txt
--rw-r--r--   0 liqiang    (501) staff       (20)        1 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/dependency_links.txt
--rw-r--r--   0 liqiang    (501) staff       (20)       71 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/requires.txt
--rw-r--r--   0 liqiang    (501) staff       (20)       12 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/top_level.txt
--rw-r--r--   0 liqiang    (501) staff       (20)      104 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/pyproject.toml
--rw-r--r--   0 liqiang    (501) staff       (20)       38 2023-06-22 09:40:32.105352 dvadmin-sms-1.0.6/setup.cfg
--rw-r--r--   0 liqiang    (501) staff       (20)      971 2023-06-22 09:40:30.000000 dvadmin-sms-1.0.6/setup.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 10:13:37.485743 dvadmin-sms-1.0.7/
+-rw-r--r--   0 liqiang    (501) staff       (20)     1072 2023-03-28 22:21:13.000000 dvadmin-sms-1.0.7/LICENSE
+-rw-r--r--   0 liqiang    (501) staff       (20)       36 2023-06-22 09:48:44.000000 dvadmin-sms-1.0.7/MANIFEST.in
+-rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-22 10:13:37.485324 dvadmin-sms-1.0.7/PKG-INFO
+-rw-r--r--   0 liqiang    (501) staff       (20)     2036 2023-04-05 15:36:58.000000 dvadmin-sms-1.0.7/README.md
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 10:13:37.475117 dvadmin-sms-1.0.7/dvadmin_sms/
+-rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/__init__.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 10:13:37.479190 dvadmin-sms-1.0.7/dvadmin_sms/api/
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/api/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1902 2023-06-22 10:13:19.000000 dvadmin-sms-1.0.7/dvadmin_sms/api/alibabacloud.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     2424 2023-03-29 07:31:38.000000 dvadmin-sms-1.0.7/dvadmin_sms/api/tencent_cloud.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      184 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.7/dvadmin_sms/apps.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 10:13:37.482300 dvadmin-sms-1.0.7/dvadmin_sms/fixtures/
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/fixtures/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      703 2023-03-28 22:58:05.000000 dvadmin-sms-1.0.7/dvadmin_sms/fixtures/init_dictionary.json
+-rw-r--r--   0 liqiang    (501) staff       (20)        4 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/fixtures/init_menu.json
+-rw-r--r--   0 liqiang    (501) staff       (20)     7592 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.7/dvadmin_sms/fixtures/init_systemconfig.json
+-rw-r--r--   0 liqiang    (501) staff       (20)     1139 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/fixtures/initialize.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 10:13:37.482972 dvadmin-sms-1.0.7/dvadmin_sms/migrations/
+-rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-21 07:15:07.000000 dvadmin-sms-1.0.7/dvadmin_sms/migrations/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/models.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      741 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.7/dvadmin_sms/settings.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      287 2023-03-28 23:45:43.000000 dvadmin-sms-1.0.7/dvadmin_sms/urls.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     2441 2023-03-29 08:20:32.000000 dvadmin-sms-1.0.7/dvadmin_sms/utils.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 10:13:37.484535 dvadmin-sms-1.0.7/dvadmin_sms/views/
+-rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/views/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1934 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.7/dvadmin_sms/views/send_sms.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1792 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/dvadmin_sms/wechat.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 10:13:37.477843 dvadmin-sms-1.0.7/dvadmin_sms.egg-info/
+-rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-22 10:13:37.000000 dvadmin-sms-1.0.7/dvadmin_sms.egg-info/PKG-INFO
+-rw-r--r--   0 liqiang    (501) staff       (20)      758 2023-06-22 10:13:37.000000 dvadmin-sms-1.0.7/dvadmin_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)        1 2023-06-22 10:13:37.000000 dvadmin-sms-1.0.7/dvadmin_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)       71 2023-06-22 10:13:37.000000 dvadmin-sms-1.0.7/dvadmin_sms.egg-info/requires.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)       12 2023-06-22 10:13:37.000000 dvadmin-sms-1.0.7/dvadmin_sms.egg-info/top_level.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)      104 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.7/pyproject.toml
+-rw-r--r--   0 liqiang    (501) staff       (20)       38 2023-06-22 10:13:37.485865 dvadmin-sms-1.0.7/setup.cfg
+-rw-r--r--   0 liqiang    (501) staff       (20)      970 2023-06-22 10:13:36.000000 dvadmin-sms-1.0.7/setup.py
```

### Comparing `dvadmin-sms-1.0.6/LICENSE` & `dvadmin-sms-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/PKG-INFO` & `dvadmin-sms-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvadmin-sms
-Version: 1.0.6
+Version: 1.0.7
 Summary: 一款适用于django-vue-admin基于阿里云、腾讯云、华为云等官方短信服务开发的短信发送插件，快速整合各端的短信服务插件。
 Home-page: https://gitee.com/huge-dream/dvadmin-sms
 Author: DVAdmin
 Author-email: liqiang@django-vue-admin.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvadmin-sms-1.0.6/README.md` & `dvadmin-sms-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/api/alibabacloud.py` & `dvadmin-sms-1.0.7/dvadmin_sms/api/alibabacloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,13 +34,13 @@
             template_param=template_param
         )
         runtime = util_models.RuntimeOptions()
         try:
             # 复制代码运行请自行打印 API 的返回值
             res = client.send_sms_with_options(send_sms_request, runtime)
             if res.body.code == "OK":
-                return False, ""
-            return True, res.body.message
+                return True, ""
+            return False, res.body.message
         except Exception as error:
             # 如有需要，请打印 error
             print(error)
             return False, UtilClient.assert_as_string(error)
```

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/api/tencent_cloud.py` & `dvadmin-sms-1.0.7/dvadmin_sms/api/tencent_cloud.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_dictionary.json` & `dvadmin-sms-1.0.7/dvadmin_sms/fixtures/init_dictionary.json`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_systemconfig.json` & `dvadmin-sms-1.0.7/dvadmin_sms/fixtures/init_systemconfig.json`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/fixtures/initialize.py` & `dvadmin-sms-1.0.7/dvadmin_sms/fixtures/initialize.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/settings.py` & `dvadmin-sms-1.0.7/dvadmin_sms/settings.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/utils.py` & `dvadmin-sms-1.0.7/dvadmin_sms/utils.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/views/send_sms.py` & `dvadmin-sms-1.0.7/dvadmin_sms/views/send_sms.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms/wechat.py` & `dvadmin-sms-1.0.7/dvadmin_sms/wechat.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms.egg-info/PKG-INFO` & `dvadmin-sms-1.0.7/dvadmin_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvadmin-sms
-Version: 1.0.6
+Version: 1.0.7
 Summary: 一款适用于django-vue-admin基于阿里云、腾讯云、华为云等官方短信服务开发的短信发送插件，快速整合各端的短信服务插件。
 Home-page: https://gitee.com/huge-dream/dvadmin-sms
 Author: DVAdmin
 Author-email: liqiang@django-vue-admin.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvadmin-sms-1.0.6/dvadmin_sms.egg-info/SOURCES.txt` & `dvadmin-sms-1.0.7/dvadmin_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.6/setup.py` & `dvadmin-sms-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dvadmin-sms",
-    version="1.0.6",
+    version="1.0.7",
     author="DVAdmin",
     author_email="liqiang@django-vue-admin.com",
     description="一款适用于django-vue-admin基于阿里云、腾讯云、华为云等官方短信服务开发的短信发送插件，快速整合各端的短信服务插件。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/huge-dream/dvadmin-sms",
     packages=setuptools.find_packages(),
@@ -19,9 +19,9 @@
         "tencentcloud-sdk-python>=3.0.911",  # 腾讯云
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    include_package_data=True,
+    include_package_data=True
 )
```

