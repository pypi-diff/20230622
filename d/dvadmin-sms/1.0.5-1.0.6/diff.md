# Comparing `tmp/dvadmin-sms-1.0.5.tar.gz` & `tmp/dvadmin-sms-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvadmin-sms-1.0.5.tar", last modified: Mon Jun 12 03:51:07 2023, max compression
+gzip compressed data, was "dvadmin-sms-1.0.6.tar", last modified: Thu Jun 22 09:40:32 2023, max compression
```

## Comparing `dvadmin-sms-1.0.5.tar` & `dvadmin-sms-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:51:07.580664 dvadmin-sms-1.0.5/
--rw-r--r--   0 liqiang    (501) staff       (20)     1072 2023-03-28 22:21:13.000000 dvadmin-sms-1.0.5/LICENSE
--rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-12 03:51:07.580181 dvadmin-sms-1.0.5/PKG-INFO
--rw-r--r--   0 liqiang    (501) staff       (20)     2036 2023-04-05 15:36:58.000000 dvadmin-sms-1.0.5/README.md
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:51:07.574010 dvadmin-sms-1.0.5/dvadmin_sms/
--rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/__init__.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:51:07.577765 dvadmin-sms-1.0.5/dvadmin_sms/api/
--rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/api/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)     1902 2023-06-12 03:50:27.000000 dvadmin-sms-1.0.5/dvadmin_sms/api/alibabacloud.py
--rw-r--r--   0 liqiang    (501) staff       (20)     2424 2023-03-29 07:31:38.000000 dvadmin-sms-1.0.5/dvadmin_sms/api/tencent_cloud.py
--rw-r--r--   0 liqiang    (501) staff       (20)      184 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.5/dvadmin_sms/apps.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:51:07.578309 dvadmin-sms-1.0.5/dvadmin_sms/fixtures/
--rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/fixtures/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)      703 2023-03-28 22:58:05.000000 dvadmin-sms-1.0.5/dvadmin_sms/fixtures/init_dictionary.json
--rw-r--r--   0 liqiang    (501) staff       (20)        4 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/fixtures/init_menu.json
--rw-r--r--   0 liqiang    (501) staff       (20)     7592 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.5/dvadmin_sms/fixtures/init_systemconfig.json
--rw-r--r--   0 liqiang    (501) staff       (20)     1139 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/fixtures/initialize.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:51:07.578846 dvadmin-sms-1.0.5/dvadmin_sms/migrations/
--rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-21 07:15:07.000000 dvadmin-sms-1.0.5/dvadmin_sms/migrations/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/models.py
--rw-r--r--   0 liqiang    (501) staff       (20)      741 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.5/dvadmin_sms/settings.py
--rw-r--r--   0 liqiang    (501) staff       (20)      287 2023-03-28 23:45:43.000000 dvadmin-sms-1.0.5/dvadmin_sms/urls.py
--rw-r--r--   0 liqiang    (501) staff       (20)     2441 2023-03-29 08:20:32.000000 dvadmin-sms-1.0.5/dvadmin_sms/utils.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:51:07.579668 dvadmin-sms-1.0.5/dvadmin_sms/views/
--rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/views/__init__.py
--rw-r--r--   0 liqiang    (501) staff       (20)     1934 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.5/dvadmin_sms/views/send_sms.py
--rw-r--r--   0 liqiang    (501) staff       (20)     1792 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/dvadmin_sms/wechat.py
-drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-12 03:51:07.576620 dvadmin-sms-1.0.5/dvadmin_sms.egg-info/
--rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-12 03:51:07.000000 dvadmin-sms-1.0.5/dvadmin_sms.egg-info/PKG-INFO
--rw-r--r--   0 liqiang    (501) staff       (20)      752 2023-06-12 03:51:07.000000 dvadmin-sms-1.0.5/dvadmin_sms.egg-info/SOURCES.txt
--rw-r--r--   0 liqiang    (501) staff       (20)        1 2023-06-12 03:51:07.000000 dvadmin-sms-1.0.5/dvadmin_sms.egg-info/dependency_links.txt
--rw-r--r--   0 liqiang    (501) staff       (20)       71 2023-06-12 03:51:07.000000 dvadmin-sms-1.0.5/dvadmin_sms.egg-info/requires.txt
--rw-r--r--   0 liqiang    (501) staff       (20)       12 2023-06-12 03:51:07.000000 dvadmin-sms-1.0.5/dvadmin_sms.egg-info/top_level.txt
--rw-r--r--   0 liqiang    (501) staff       (20)      104 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.5/pyproject.toml
--rw-r--r--   0 liqiang    (501) staff       (20)       38 2023-06-12 03:51:07.580778 dvadmin-sms-1.0.5/setup.cfg
--rw-r--r--   0 liqiang    (501) staff       (20)     1193 2023-06-12 03:50:47.000000 dvadmin-sms-1.0.5/setup.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.105230 dvadmin-sms-1.0.6/
+-rw-r--r--   0 liqiang    (501) staff       (20)     1072 2023-03-28 22:21:13.000000 dvadmin-sms-1.0.6/LICENSE
+-rw-r--r--   0 liqiang    (501) staff       (20)       36 2023-06-22 09:39:55.000000 dvadmin-sms-1.0.6/MANIFEST.in
+-rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-22 09:40:32.104843 dvadmin-sms-1.0.6/PKG-INFO
+-rw-r--r--   0 liqiang    (501) staff       (20)     2036 2023-04-05 15:36:58.000000 dvadmin-sms-1.0.6/README.md
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.097267 dvadmin-sms-1.0.6/dvadmin_sms/
+-rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/__init__.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.100581 dvadmin-sms-1.0.6/dvadmin_sms/api/
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/api/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1902 2023-06-12 03:50:27.000000 dvadmin-sms-1.0.6/dvadmin_sms/api/alibabacloud.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     2424 2023-03-29 07:31:38.000000 dvadmin-sms-1.0.6/dvadmin_sms/api/tencent_cloud.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      184 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.6/dvadmin_sms/apps.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.102871 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      703 2023-03-28 22:58:05.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_dictionary.json
+-rw-r--r--   0 liqiang    (501) staff       (20)        4 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_menu.json
+-rw-r--r--   0 liqiang    (501) staff       (20)     7592 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_systemconfig.json
+-rw-r--r--   0 liqiang    (501) staff       (20)     1139 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/fixtures/initialize.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.103356 dvadmin-sms-1.0.6/dvadmin_sms/migrations/
+-rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-21 07:15:07.000000 dvadmin-sms-1.0.6/dvadmin_sms/migrations/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)        0 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/models.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      741 2023-03-28 23:02:04.000000 dvadmin-sms-1.0.6/dvadmin_sms/settings.py
+-rw-r--r--   0 liqiang    (501) staff       (20)      287 2023-03-28 23:45:43.000000 dvadmin-sms-1.0.6/dvadmin_sms/urls.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     2441 2023-03-29 08:20:32.000000 dvadmin-sms-1.0.6/dvadmin_sms/utils.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.104345 dvadmin-sms-1.0.6/dvadmin_sms/views/
+-rw-r--r--   0 liqiang    (501) staff       (20)       24 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/views/__init__.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1934 2023-03-29 13:52:19.000000 dvadmin-sms-1.0.6/dvadmin_sms/views/send_sms.py
+-rw-r--r--   0 liqiang    (501) staff       (20)     1792 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/dvadmin_sms/wechat.py
+drwxr-xr-x   0 liqiang    (501) staff       (20)        0 2023-06-22 09:40:32.099372 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/
+-rw-r--r--   0 liqiang    (501) staff       (20)     2611 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/PKG-INFO
+-rw-r--r--   0 liqiang    (501) staff       (20)      758 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)        1 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)       71 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/requires.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)       12 2023-06-22 09:40:32.000000 dvadmin-sms-1.0.6/dvadmin_sms.egg-info/top_level.txt
+-rw-r--r--   0 liqiang    (501) staff       (20)      104 2023-03-28 15:25:40.000000 dvadmin-sms-1.0.6/pyproject.toml
+-rw-r--r--   0 liqiang    (501) staff       (20)       38 2023-06-22 09:40:32.105352 dvadmin-sms-1.0.6/setup.cfg
+-rw-r--r--   0 liqiang    (501) staff       (20)      971 2023-06-22 09:40:30.000000 dvadmin-sms-1.0.6/setup.py
```

### Comparing `dvadmin-sms-1.0.5/LICENSE` & `dvadmin-sms-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/PKG-INFO` & `dvadmin-sms-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvadmin-sms
-Version: 1.0.5
+Version: 1.0.6
 Summary: 一款适用于django-vue-admin基于阿里云、腾讯云、华为云等官方短信服务开发的短信发送插件，快速整合各端的短信服务插件。
 Home-page: https://gitee.com/huge-dream/dvadmin-sms
 Author: DVAdmin
 Author-email: liqiang@django-vue-admin.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvadmin-sms-1.0.5/README.md` & `dvadmin-sms-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/api/alibabacloud.py` & `dvadmin-sms-1.0.6/dvadmin_sms/api/alibabacloud.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/api/tencent_cloud.py` & `dvadmin-sms-1.0.6/dvadmin_sms/api/tencent_cloud.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/fixtures/init_dictionary.json` & `dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_dictionary.json`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/fixtures/init_systemconfig.json` & `dvadmin-sms-1.0.6/dvadmin_sms/fixtures/init_systemconfig.json`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/fixtures/initialize.py` & `dvadmin-sms-1.0.6/dvadmin_sms/fixtures/initialize.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/settings.py` & `dvadmin-sms-1.0.6/dvadmin_sms/settings.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/utils.py` & `dvadmin-sms-1.0.6/dvadmin_sms/utils.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/views/send_sms.py` & `dvadmin-sms-1.0.6/dvadmin_sms/views/send_sms.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms/wechat.py` & `dvadmin-sms-1.0.6/dvadmin_sms/wechat.py`

 * *Files identical despite different names*

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms.egg-info/PKG-INFO` & `dvadmin-sms-1.0.6/dvadmin_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvadmin-sms
-Version: 1.0.5
+Version: 1.0.6
 Summary: 一款适用于django-vue-admin基于阿里云、腾讯云、华为云等官方短信服务开发的短信发送插件，快速整合各端的短信服务插件。
 Home-page: https://gitee.com/huge-dream/dvadmin-sms
 Author: DVAdmin
 Author-email: liqiang@django-vue-admin.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dvadmin-sms-1.0.5/dvadmin_sms.egg-info/SOURCES.txt` & `dvadmin-sms-1.0.6/dvadmin_sms.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 setup.py
-./dvadmin_sms/fixtures/init_dictionary.json
-./dvadmin_sms/fixtures/init_menu.json
-./dvadmin_sms/fixtures/init_systemconfig.json
 dvadmin_sms/__init__.py
 dvadmin_sms/apps.py
 dvadmin_sms/models.py
 dvadmin_sms/settings.py
 dvadmin_sms/urls.py
 dvadmin_sms/utils.py
 dvadmin_sms/wechat.py
@@ -17,11 +15,14 @@
 dvadmin_sms.egg-info/dependency_links.txt
 dvadmin_sms.egg-info/requires.txt
 dvadmin_sms.egg-info/top_level.txt
 dvadmin_sms/api/__init__.py
 dvadmin_sms/api/alibabacloud.py
 dvadmin_sms/api/tencent_cloud.py
 dvadmin_sms/fixtures/__init__.py
+dvadmin_sms/fixtures/init_dictionary.json
+dvadmin_sms/fixtures/init_menu.json
+dvadmin_sms/fixtures/init_systemconfig.json
 dvadmin_sms/fixtures/initialize.py
 dvadmin_sms/migrations/__init__.py
 dvadmin_sms/views/__init__.py
 dvadmin_sms/views/send_sms.py
```

### Comparing `dvadmin-sms-1.0.5/setup.py` & `dvadmin-sms-1.0.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dvadmin-sms",
-    version="1.0.5",
+    version="1.0.6",
     author="DVAdmin",
     author_email="liqiang@django-vue-admin.com",
     description="一款适用于django-vue-admin基于阿里云、腾讯云、华为云等官方短信服务开发的短信发送插件，快速整合各端的短信服务插件。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/huge-dream/dvadmin-sms",
     packages=setuptools.find_packages(),
@@ -19,16 +19,9 @@
         "tencentcloud-sdk-python>=3.0.911",  # 腾讯云
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    data_files=[
-        ('', [
-            './dvadmin_sms/fixtures/init_menu.json',
-            './dvadmin_sms/fixtures/init_systemconfig.json',
-            './dvadmin_sms/fixtures/init_dictionary.json'
-        ])
-    ],
     include_package_data=True,
 )
```

