# Comparing `tmp/uaDevice-1.0.8.tar.gz` & `tmp/uaDevice-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uaDevice-1.0.8.tar", last modified: Fri Jul 29 09:46:11 2022, max compression
+gzip compressed data, was "uaDevice-1.0.9.tar", last modified: Thu Jun 22 02:29:07 2023, max compression
```

## Comparing `uaDevice-1.0.8.tar` & `uaDevice-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2022-07-29 09:46:11.426484 uaDevice-1.0.8/
--rw-r--r--   0 wukaifang   (502) staff       (20)     4090 2022-07-29 09:46:11.426164 uaDevice-1.0.8/PKG-INFO
--rwxrwxrwx   0 wukaifang   (502) staff       (20)     3245 2020-03-05 11:20:50.000000 uaDevice-1.0.8/README.md
--rw-r--r--   0 wukaifang   (502) staff       (20)       38 2022-07-29 09:46:11.426613 uaDevice-1.0.8/setup.cfg
--rwxr-xr-x   0 wukaifang   (502) staff       (20)     1409 2022-07-29 09:45:43.000000 uaDevice-1.0.8/setup.py
-drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2022-07-29 09:46:11.421656 uaDevice-1.0.8/test/
--rwxrwxrwx   0 wukaifang   (502) staff       (20)     3727 2020-05-31 16:06:47.000000 uaDevice-1.0.8/test/test.py
-drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2022-07-29 09:46:11.423711 uaDevice-1.0.8/uaDevice/
--rwxrwxrwx   0 wukaifang   (502) staff       (20)       28 2020-05-25 08:22:26.000000 uaDevice-1.0.8/uaDevice/__init__.py
--rwxrwxrwx   0 wukaifang   (502) staff       (20)   109310 2022-07-29 09:23:20.000000 uaDevice-1.0.8/uaDevice/models.py
--rwxrwxrwx   0 wukaifang   (502) staff       (20)     7120 2018-12-17 11:01:58.000000 uaDevice-1.0.8/uaDevice/regs.py
--rwxrwxrwx   0 wukaifang   (502) staff       (20)    43024 2022-07-29 09:23:09.000000 uaDevice-1.0.8/uaDevice/uaDevice.py
--rwxrwxrwx   0 wukaifang   (502) staff       (20)   103571 2020-05-31 16:03:09.000000 uaDevice-1.0.8/uaDevice/useragentBase.py
-drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2022-07-29 09:46:11.425674 uaDevice-1.0.8/uaDevice.egg-info/
--rwxrwxrwx   0 wukaifang   (502) staff       (20)     4090 2022-07-29 09:46:11.000000 uaDevice-1.0.8/uaDevice.egg-info/PKG-INFO
--rwxrwxrwx   0 wukaifang   (502) staff       (20)      263 2022-07-29 09:46:11.000000 uaDevice-1.0.8/uaDevice.egg-info/SOURCES.txt
--rwxrwxrwx   0 wukaifang   (502) staff       (20)        1 2022-07-29 09:46:11.000000 uaDevice-1.0.8/uaDevice.egg-info/dependency_links.txt
--rwxrwxrwx   0 wukaifang   (502) staff       (20)        9 2022-07-29 09:46:11.000000 uaDevice-1.0.8/uaDevice.egg-info/top_level.txt
+drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2023-06-22 02:29:07.660509 uaDevice-1.0.9/
+-rw-r--r--   0 wukaifang   (502) staff       (20)     4090 2023-06-22 02:29:07.660126 uaDevice-1.0.9/PKG-INFO
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)     3245 2020-03-05 11:20:50.000000 uaDevice-1.0.9/README.md
+-rw-r--r--   0 wukaifang   (502) staff       (20)       38 2023-06-22 02:29:07.660656 uaDevice-1.0.9/setup.cfg
+-rwxr-xr-x   0 wukaifang   (502) staff       (20)     1465 2023-06-22 02:29:01.000000 uaDevice-1.0.9/setup.py
+drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2023-06-22 02:29:07.650722 uaDevice-1.0.9/test/
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)     3727 2023-06-22 02:05:15.000000 uaDevice-1.0.9/test/test.py
+drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2023-06-22 02:29:07.655863 uaDevice-1.0.9/uaDevice/
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)       28 2020-05-25 08:22:26.000000 uaDevice-1.0.9/uaDevice/__init__.py
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)   109310 2022-07-29 09:23:20.000000 uaDevice-1.0.9/uaDevice/models.py
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)       15 2023-06-22 02:05:44.000000 uaDevice-1.0.9/uaDevice/regs.py
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)    42912 2023-06-22 02:19:07.000000 uaDevice-1.0.9/uaDevice/uaDevice.py
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)   102736 2023-06-22 02:19:56.000000 uaDevice-1.0.9/uaDevice/useragentBase.py
+drwxr-xr-x   0 wukaifang   (502) staff       (20)        0 2023-06-22 02:29:07.659142 uaDevice-1.0.9/uaDevice.egg-info/
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)     4090 2023-06-22 02:29:07.000000 uaDevice-1.0.9/uaDevice.egg-info/PKG-INFO
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)      263 2023-06-22 02:29:07.000000 uaDevice-1.0.9/uaDevice.egg-info/SOURCES.txt
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)        1 2023-06-22 02:29:07.000000 uaDevice-1.0.9/uaDevice.egg-info/dependency_links.txt
+-rwxrwxrwx   0 wukaifang   (502) staff       (20)        9 2023-06-22 02:29:07.000000 uaDevice-1.0.9/uaDevice.egg-info/top_level.txt
```

### Comparing `uaDevice-1.0.8/PKG-INFO` & `uaDevice-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uaDevice
-Version: 1.0.8
+Version: 1.0.9
 Summary: User Agent parser, More accurate
 Home-page: https://github.com/kaivean/python-ua-device
 Author: kaivean
 Author-email: kaivean@outlook.com
 License: MIT Licence
 Description: # ua-device [![Build Status](https://travis-ci.com/kaivean/python-ua-device.svg?branch=master)](https://travis-ci.com/kaivean/python-ua-device)
         解析user-agent的python包，可以获取到系统、浏览器内核、浏览器、设备信息，其特点：
```

### Comparing `uaDevice-1.0.8/README.md` & `uaDevice-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `uaDevice-1.0.8/setup.py` & `uaDevice-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 
 #############################################
 # File Name: setup.py
 # Author: kaivean
 # Mail: kaivean@outlook.com
-# usage test: rm -fr dist && python3 setup.py sdist  && twine upload --repository-url https://test.pypi.org/legacy/ dist/uaDevice-*.tar.gz
-# usage: rm -fr dist && python3 setup.py sdist  && twine upload dist/uaDevice-*.tar.gz
+# 1: modify following version
+# 2. build and upload
+#   usage test: rm -fr dist && python3 setup.py sdist  && twine upload --repository-url https://test.pypi.org/legacy/ dist/uaDevice-*.tar.gz
+#   usage: rm -fr dist && python3 setup.py sdist  && twine upload dist/uaDevice-*.tar.gz
 #############################################
 
 import os
 from setuptools import setup, find_packages
 ROOT = os.path.dirname(os.path.realpath(__file__))
 
 import sys
@@ -21,15 +23,15 @@
 if sys.version_info < (3, 0):
     desc = open(os.path.join(ROOT, 'README.md')).read()
 else:
     desc = open(os.path.join(ROOT, 'README.md'), encoding='UTF-8').read()
 
 setup(
     name = "uaDevice",
-    version = "1.0.8",
+    version = "1.0.9",
     keywords = ("ua", "user-agent", "User Agent", "parser", "device", "os", "browser", "engine", "data analysis", "china", "中国", "国内"),
     description = "User Agent parser, More accurate",
     long_description = desc,
     long_description_content_type="text/markdown",
     license = "MIT Licence",
 
     url = "https://github.com/kaivean/python-ua-device",
```

### Comparing `uaDevice-1.0.8/test/test.py` & `uaDevice-1.0.9/test/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 if sys.version_info < (3, 0):
     sys.setdefaultencoding('utf-8')
 
 sys.path.append('uaDevice')
 import uaDevice
 
 if __name__ == '__main__':
-    f = open('test/data.txt')
-    # f = open('test/data10000.txt')
+    # f = open('test/data.txt')
+    f = open('test/data10000.txt')
     data = f.read()
 
     uas = data.split('\n')
 
     stat = {
         'osName': [0, [], []],
         'osVersion': [0, [], []],
```

### Comparing `uaDevice-1.0.8/uaDevice/models.py` & `uaDevice-1.0.9/uaDevice/models.py`

 * *Files identical despite different names*

### Comparing `uaDevice-1.0.8/uaDevice/uaDevice.py` & `uaDevice-1.0.9/uaDevice/uaDevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -640,23 +640,22 @@
     # handle browser
     # if (!uaData['browser']['name']) {
     # ua = ua.toLowerCase();
     if uaData['device']['type'] == 'desktop':
 
         # 360 security Explorer
 
-        # if match = //i.exec(ua):
+        # user-agent: Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.5359.95 Safari/537.36 QIHU 360SE/14.1.1094.0
         if getMatch(ua, r'360se(?:[ \/]([\w.]+))?', True):
             match = getMatch()
             uaData['browser']['name'] = '360 security Explorer'
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
 
-
         # the world
 
         # elif match = //i.exec(ua):
         elif getMatch(ua, r'the world(?:[ \/]([\w.]+))?', True):
             match = getMatch()
             uaData['browser']['name'] = 'the world'
             uaData['browser']['version'] = {
@@ -682,119 +681,67 @@
             match = getMatch()
             uaData['browser']['name'] = 'LBBROWSER'
 
 
     elif uaData['device']['type'] == 'mobile' or uaData['device']['type'] == 'tablet':
 
         # BaiduHD
-
         if getMatch(ua, r'BaiduHD\s+([\w.]+)', True):
             match = getMatch()
             uaData['browser']['name'] = 'BaiduHD'
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
 
 
         # 360 Browser
-
         elif getMatch(ua, r'360.s*aphone\s*browser\s*\(version\s*([\w.]+)\)', True):
             match = getMatch()
-            uaData['browser']['name'] = '360 Browser'
-            uaData['browser']['version'] = {
-                'original': match.group(1)
-            }
-
-
-        # Baidu Browser
-
-        # elif match = /flyflow\/([\w.]+)/i.exec(ua):
-        elif getMatch(ua, r'flyflow\/([\w.]+)', True):
-            match = getMatch()
-            uaData['browser']['name'] = 'Baidu Browser'
-            uaData['browser']['version'] = {
-                'original': match.group(1)
-            }
-
-
-
-        # Baidu HD
-
-        # elif match = /baiduhd ([\w.]+)/i.exec(ua):
-        elif getMatch(ua, r'baiduhd ([\w.]+)', True):
-            match = getMatch()
-            uaData['browser']['name'] = 'Baidu HD'
+            uaData['browser']['name'] = '360 Mobile Browser'
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
 
 
-
-        # baidubrowser
-
-        # elif match = //i.exec(ua):
-        elif getMatch(ua, r'baidubrowser\/([\d\.]+)\s', True):
-            match = getMatch()
-            uaData['browser']['name'] = 'baidubrowser'
-            uaData['browser']['version'] = {
-                'original': match.group(1)
-            }
-
-
-
         # LieBaoFast
-
         # elif match = //i.exec(ua):
         elif getMatch(ua, r'LieBaoFast\/([\w.]+)', True):
             match = getMatch()
             uaData['browser']['name'] = 'LieBao Fast'
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
 
 
-
         # LieBao
-
-        # elif match = //i.exec(ua):
         elif getMatch(ua, r'LieBao\/([\w.]+)', True):
             match = getMatch()
             uaData['browser']['name'] = 'LieBao'
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
 
 
-
         # SOUGOU
-
-        # elif match = //i.exec(ua):
         elif getMatch(ua, r'Sogou\w+\/([0-9\.]+)', True):
             match = getMatch()
             uaData['browser']['name'] = 'SogouMobileBrowser'
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
 
-
-
         # 百度国际
-
-        # elif match = //i.exec(ua):
         elif getMatch(ua, r'bdbrowser\w+\/([0-9\.]+)', True):
             match = getMatch()
             uaData['browser']['name'] = '百度国际'
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
 
-
-
         # Android Chrome Browser
-
         elif uaData['os']['name'] == 'Android' and optimizedSearch(r'safari', ua, re.I) and getMatch(ua, r'chrome\/([0-9\.]+)', True):
             match = getMatch()
             tmpMatch = getMatch(ua, r'\s+(\w+Browser)\/?([\d\.]*)')
             if tmpMatch:
                 uaData['browser']['name'] = tmpMatch.group(1)
                 if tmpMatch.group(2):
                     uaData['browser']['version'] = {'original': tmpMatch.group(2)}
@@ -802,18 +749,15 @@
                     uaData['browser']['version'] = {'original': match.group(1)}
 
             else:
                 uaData['browser']['name'] = 'Android Chrome'
                 uaData['browser']['version'] = {'original': match.group(1)}
 
 
-
-
         # Android Google Browser
-
         elif uaData['os']['name'] == 'Android' and optimizedSearch(r'safari', ua, re.I) and getMatch(ua, r'version\/([0-9\.]+)', True):
             match = getMatch()
             tmpMatch = getMatch(ua, r'\s+(\w+Browser)\/?([\d\.]*)')
             if tmpMatch:
                 uaData['browser']['name'] = tmpMatch.group(1)
                 if tmpMatch.group(2):
                     uaData['browser']['version'] = {'original': tmpMatch.group(2)}
@@ -821,74 +765,87 @@
                     uaData['browser']['version'] = {'original': match.group(1)}
 
             else:
                 uaData['browser']['name'] = 'Android Browser'
                 uaData['browser']['version'] = {'original': match.group(1)}
 
 
-
-
         # 'Mozilla/5.0 (iPad; CPU OS 5_1_1 like Mac OS X) AppleWebKit/534.46 (KHTML, like Gecko) Mobile/9B206' belongs to Safari
-
         elif getMatch(ua, r'(ipad|iphone).* applewebkit\/.* mobile', True):
             match = getMatch()
             uaData['browser']['name'] = 'Safari'
 
 
     if getMatch(ua, r'baiduboxapp\/?([\d\.]*)', True):
         match = getMatch()
-        uaData['browser']['name'] = '百度框'
+        uaData['browser']['name'] = 'BaiduApp'
         if match.group(1):
             uaData['browser']['version'] = {
                 'original': match.group(1)
             }
-
-        # uaData['browser']['name'] = 'baidu box';
-
     elif getMatch(ua, r'BaiduLightAppRuntime', True):
         match = getMatch()
         uaData['browser']['name'] = '轻应用runtime'
-        # uaData['browser']['name'] = 'qing runtime';
-
+    elif getMatch(ua, r'baidubrowser\/([\d\.]+)\s', True):
+        match = getMatch()
+        uaData['browser']['name'] = 'BaiduBrowser'
+        uaData['browser']['version'] = {
+            'original': match.group(1)
+        }
+    elif getMatch(ua, r'SE 2.X MetaSr', True):
+        # match = getMatch()
+        uaData['browser']['name'] = 'SogouExplorer'
+        uaData['browser']['version'] = {
+            'original': ''
+        }
+    elif getMatch(ua, r'PhantomJS\/([0-9.]*)', True):
+        match = getMatch()
+        uaData['browser']['name'] = 'PhantomJS'
+        uaData['browser']['version'] = {
+            'original': match.group(1)
+        }
     elif getMatch(ua, r'Weibo', True):
         match = getMatch()
         uaData['browser']['name'] = '微博'
-        # uaData['browser']['name'] = 'weibo';
-
     elif getMatch(ua, r'MQQ', True):
         match = getMatch()
         uaData['browser']['name'] = '手机QQ'
-        # uaData['browser']['name'] = 'mobile qq';
-
     elif getMatch(ua, r'hao123', True):
         match = getMatch()
         uaData['browser']['name'] = 'hao123'
 
-    # }
+
     if getMatch(ua, r'MicroMessenger\/([\w.]+)', True):
         match = getMatch()
         uaData['browser']['name'] = '微信'
-        # optimizedSub(r'-+|_+|\s+', r' ', )
         tmpVersion = match.group(1).replace('_', '.')
         tmpMatch = getMatch(tmpVersion, r'(\d+\.\d+\.\d+\.\d+)')
-        # tmpMatch = //.exec(tmpVersion)
         if tmpMatch:
             tmpVersion = tmpMatch.group(1)
 
         uaData['browser']['version'] = {
             'original': tmpVersion
         }
 
     elif getMatch(ua, r'UCBrowser\/([\w.]+)', True):
         match = getMatch()
         uaData['browser']['name'] = 'UC Browser'
         uaData['browser']['version'] = {
             'original': match.group(1)
         }
 
+    # Lenovo
+    # Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/92.0.4515.131 Safari/537.36 SLBrowser/8.0.1.5162 SLBChan/10
+    elif getMatch(ua, r'SLBrowser\/([\w.]+)', True):
+        match = getMatch()
+        uaData['browser']['name'] = 'Lenovo'
+        uaData['browser']['version'] = {
+            'original': match.group(1)
+        }
+
     if getMatch(ua, r'OPR\/([\w.]+)', True):
         match = getMatch()
         uaData['browser']['name'] = 'Opera'
         uaData['browser']['version'] = {
             'original': match.group(1)
         }
     elif getMatch(ua, r'OPiOS\/([\w.]+)', True):
@@ -904,19 +861,20 @@
         uaData['browser']['name'] = 'Internet Explorer'
         uaData['browser']['version'] = {
             'major': '11',
             'original': '11'
         }
 
     # Microsoft Edge
-    elif getMatch(ua, r'Edge\/12', True) and getMatch(ua, r'Windows Phone|Windows NT', True):
+    # Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36 Edg/111.0.1661.62
+    elif getMatch(ua, r' (Edge|Edg)\/([\w.]+)', True):
+        match = getMatch()
         uaData['browser']['name'] = 'Microsoft Edge'
         uaData['browser']['version'] = {
-            'major': '12',
-            'original': '12'
+            'original': match.group(2)
         }
 
     # miui browser
     # elif match = //i.exec(ua):
     elif getMatch(ua, r'miuibrowser\/([\w.]+)', True):
         match = getMatch()
         uaData['browser']['name'] = 'miui browser'
```

### Comparing `uaDevice-1.0.8/uaDevice/useragentBase.py` & `uaDevice-1.0.9/uaDevice/useragentBase.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import json
 from imp import reload
 reload(sys)
 if sys.version_info < (3, 0):
     sys.setdefaultencoding('utf-8')
 sys.path.append('./')
 
-from regs import *
 from models import *
 
 regObj = {
 
 }
 
 def optimizedSearch(regStr, matchStr, flags=0):
@@ -2730,44 +2729,15 @@
 
 
             self.device['manufacturer'] = None
             self.device['model'] = None
             self.device['type'] = 'desktop'
 
 
-
-        # Others
-        #
-        # 移除browsers
-
-        for item in browsers:
-            # 大小写不敏感
-            if 'i' in item:
-                match = optimizedSearch(item['regexp'], ua, re.I)
-            else:
-                match = optimizedSearch(item['regexp'], ua)
-            if match:
-                self.browser['name'] = item['name']
-                self.browser['channel'] = ''
-                self.browser['stock'] = False
-
-                if len(match.groups()) > 0 and match.group(1):
-                    self.browser['version'] = Version({
-                        'value': match.group(1),
-                        'details': item['details'] if 'details' in item else None
-                    })
-                else:
-                    self.browser['version'] = None
-
-
-
-
-
         # WebKit
-        #
         match = optimizedSearch(r'WebKit\/([0-9.]*)', ua, re.I)
         if match:
             self.engine['name'] = 'Webkit'
             self.engine['version'] = Version({
                 'value': match.group(1)
             })
```

### Comparing `uaDevice-1.0.8/uaDevice.egg-info/PKG-INFO` & `uaDevice-1.0.9/uaDevice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uaDevice
-Version: 1.0.8
+Version: 1.0.9
 Summary: User Agent parser, More accurate
 Home-page: https://github.com/kaivean/python-ua-device
 Author: kaivean
 Author-email: kaivean@outlook.com
 License: MIT Licence
 Description: # ua-device [![Build Status](https://travis-ci.com/kaivean/python-ua-device.svg?branch=master)](https://travis-ci.com/kaivean/python-ua-device)
         解析user-agent的python包，可以获取到系统、浏览器内核、浏览器、设备信息，其特点：
```

