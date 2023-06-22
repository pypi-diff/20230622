# Comparing `tmp/sh2d-0.9.tar.gz` & `tmp/sh2d-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sh2d-0.9.tar", last modified: Thu Mar  2 10:46:17 2023, max compression
+gzip compressed data, was "sh2d-1.1.tar", last modified: Thu Jun 22 14:05:17 2023, max compression
```

## Comparing `sh2d-0.9.tar` & `sh2d-1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-03-02 10:46:17.421703 sh2d-0.9/
--rw-rw-rw-   0        0        0      310 2023-03-02 10:46:17.421703 sh2d-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     1369 2022-12-08 10:44:15.000000 sh2d-0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-02 10:46:17.418703 sh2d-0.9/mylib/
--rw-rw-rw-   0        0        0        0 2022-03-08 10:41:00.000000 sh2d-0.9/mylib/__init__.py
--rw-rw-rw-   0        0        0     1875 2023-02-25 11:48:07.000000 sh2d-0.9/mylib/aiqicha_help.py
--rw-rw-rw-   0        0        0     6490 2022-12-07 05:14:10.000000 sh2d-0.9/mylib/aqfh_help.py
--rw-rw-rw-   0        0        0     5548 2022-10-22 05:26:41.000000 sh2d-0.9/mylib/awvs_help.py
--rw-rw-rw-   0        0        0     6679 2023-02-25 11:59:15.000000 sh2d-0.9/mylib/beian_help.py
--rw-rw-rw-   0        0        0     2132 2023-02-25 12:03:23.000000 sh2d-0.9/mylib/beianx_help.py
--rw-rw-rw-   0        0        0     5235 2023-02-25 11:51:27.000000 sh2d-0.9/mylib/chinaz_help.py
--rw-rw-rw-   0        0        0     3115 2022-11-18 10:06:59.000000 sh2d-0.9/mylib/chromedriver_help.py
--rw-rw-rw-   0        0        0     3309 2023-02-25 11:30:29.000000 sh2d-0.9/mylib/common_help.py
--rw-rw-rw-   0        0        0     1019 2023-03-02 10:44:38.000000 sh2d-0.9/mylib/configparser_help.py
--rw-rw-rw-   0        0        0     1626 2022-11-18 09:45:43.000000 sh2d-0.9/mylib/csv_help.py
--rw-rw-rw-   0        0        0      607 2022-12-07 05:17:00.000000 sh2d-0.9/mylib/des_help.py
--rw-rw-rw-   0        0        0     2626 2022-10-21 04:40:04.000000 sh2d-0.9/mylib/dingtalk_help.py
--rw-rw-rw-   0        0        0     1069 2023-02-25 11:33:55.000000 sh2d-0.9/mylib/dnspython_help.py
--rw-rw-rw-   0        0        0      741 2022-10-22 03:13:28.000000 sh2d-0.9/mylib/docxtpl_help.py
--rw-rw-rw-   0        0        0     1937 2023-02-25 10:45:25.000000 sh2d-0.9/mylib/fofa_help.py
--rw-rw-rw-   0        0        0     3404 2022-12-02 15:53:46.000000 sh2d-0.9/mylib/github_help.py
--rw-rw-rw-   0        0        0      650 2022-12-02 13:35:32.000000 sh2d-0.9/mylib/hashlib_help.py
--rw-rw-rw-   0        0        0     4184 2023-02-25 13:16:46.000000 sh2d-0.9/mylib/ipaddress_help.py
--rw-rw-rw-   0        0        0     2153 2022-06-17 03:27:52.000000 sh2d-0.9/mylib/logging_help.py
--rw-rw-rw-   0        0        0     2331 2022-03-14 08:52:50.000000 sh2d-0.9/mylib/nessus_help.py
--rw-rw-rw-   0        0        0     4829 2022-02-08 04:37:27.000000 sh2d-0.9/mylib/openpyxl_help.py
--rw-rw-rw-   0        0        0     3220 2022-11-18 09:41:22.000000 sh2d-0.9/mylib/paramiko_help.py
--rw-rw-rw-   0        0        0     1987 2022-11-18 10:26:14.000000 sh2d-0.9/mylib/pymysql_help.py
--rw-rw-rw-   0        0        0     3883 2022-12-07 05:23:10.000000 sh2d-0.9/mylib/re_help.py
--rw-rw-rw-   0        0        0    12619 2022-12-07 04:43:27.000000 sh2d-0.9/mylib/rsas_help.py
--rw-rw-rw-   0        0        0     6215 2023-02-25 11:30:39.000000 sh2d-0.9/mylib/rsas_xls_help.py
--rw-rw-rw-   0        0        0     2133 2023-02-25 12:25:09.000000 sh2d-0.9/mylib/sqlite_help.py
--rw-rw-rw-   0        0        0     2837 2023-02-25 12:53:54.000000 sh2d-0.9/mylib/tmpdb_help.py
--rw-rw-rw-   0        0        0      886 2023-02-25 10:50:58.000000 sh2d-0.9/mylib/webinfo_help.py
--rw-rw-rw-   0        0        0     2002 2023-01-31 07:57:16.000000 sh2d-0.9/mylib/weixin_help.py
--rw-rw-rw-   0        0        0     2710 2022-11-18 09:38:34.000000 sh2d-0.9/mylib/xlrd_help.py
--rw-rw-rw-   0        0        0     1283 2022-02-08 04:38:38.000000 sh2d-0.9/mylib/xlsxwriter_help.py
--rw-rw-rw-   0        0        0      561 2022-02-08 04:38:45.000000 sh2d-0.9/mylib/xlwt_help.py
--rw-rw-rw-   0        0        0      582 2022-12-08 10:42:58.000000 sh2d-0.9/mylib/yaml_help.py
--rw-rw-rw-   0        0        0     1465 2022-10-22 02:51:37.000000 sh2d-0.9/mylib/zipfile_help.py
--rw-rw-rw-   0        0        0      793 2022-10-22 07:07:56.000000 sh2d-0.9/mylib/zmail_help.py
--rw-rw-rw-   0        0        0       42 2023-03-02 10:46:17.421703 sh2d-0.9/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-02-27 06:17:41.000000 sh2d-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-02 10:46:17.420703 sh2d-0.9/sh2d.egg-info/
--rw-rw-rw-   0        0        0      310 2023-03-02 10:46:17.000000 sh2d-0.9/sh2d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      941 2023-03-02 10:46:17.000000 sh2d-0.9/sh2d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-02 10:46:17.000000 sh2d-0.9/sh2d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-03-02 10:46:17.000000 sh2d-0.9/sh2d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-02 10:46:17.000000 sh2d-0.9/sh2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:05:17.457500 sh2d-1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 14:05:17.457500 sh2d-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-22 14:05:05.000000 sh2d-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:05:17.453499 sh2d-1.1/mylib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/aiqicha_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/aqfh_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/awvs_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/beian_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/beianx_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/chinaz_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/chromedriver_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/common_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/configparser_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/csv_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/des_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/dingtalk_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/dnspython_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/docxtpl_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/fofa_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/github_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/hashlib_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/ipaddress_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/logging_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/nessus_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/openpyxl_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/paramiko_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/pymysql_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/re_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/rsas_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/rsas_xls_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/sqlite_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/tmpdb_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/webinfo_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/weixin_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/xlrd_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/xlsxwriter_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/xlwt_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/yaml_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/zipfile_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-22 14:05:05.000000 sh2d-1.1/mylib/zmail_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:05:17.457500 sh2d-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-22 14:05:05.000000 sh2d-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:05:17.457500 sh2d-1.1/sh2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 14:05:17.000000 sh2d-1.1/sh2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-22 14:05:17.000000 sh2d-1.1/sh2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:05:17.000000 sh2d-1.1/sh2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 14:05:17.000000 sh2d-1.1/sh2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 14:05:17.000000 sh2d-1.1/sh2d.egg-info/top_level.txt
```

### Comparing `sh2d-0.9/README.md` & `sh2d-1.1/README.md`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-# 更新日志
-- 2022/12/08 新增 yaml_help.py 版本号更新为 0.7
-- 2022/12/07 更新 版本号更新为 0.6
-- 2022/12/07 更新 tmpdb_help.py，添加IP查询支持
-- 2022/12/06 新增 aqfh_help.py，install_requires新增ddddocr
-
-# 模块介绍
-
-## aqfh 定级备案爬虫(仅获取数据，不做数据处理)
-
-## awvs AWVS接口调用(待完善)
-
-## chromedriver chromedriver自动更新
-
-## common 通用数据处理
-
-## configparser 配置文件读取、写入、转json
-
-## csv cvs文件读取、写入
-
-## des DES(ECB)加解密
-
-## dingtalk 钉钉群机器人接口调用
-
-## dnspython 解析域名到IP、CNAME
-
-## docxtpl 根据模板生成word
-
-## fofa fofa查询接口调用
-
-## github github查询搜索接口调用
-
-## hashlib 字符串、文件md5
-
-## ipaddress 网段、IP格式转化
-
-## logging 日志
-
-## nessus nessus接口调用
-
-## openpyxl xlsx精细化编辑
-
-## paramiko ssh操作类封装
-
-## pymysql mysql操作类封装
-
-## re 常用正则
-
-## rsas 绿盟扫描器接口封装(爬虫版)
-
-## rsas_xls 绿盟扫描结果处理
-
-## sqlite sqlite操作类封装
-
-## tmpdb 简易kv数据库操作
-
-## xlrd excel文件读取
-
-## xlsxwriter xlsx文件写入
-
-## xlwt xls文件写入
-
-## yaml yaml文件读取写入
-
-## zipfile zip解压、压缩
-
-## zmail 邮件发送
-
-
-
+# 更新日志
+- 2022/12/08 新增 yaml_help.py 版本号更新为 0.7
+- 2022/12/07 更新 版本号更新为 0.6
+- 2022/12/07 更新 tmpdb_help.py，添加IP查询支持
+- 2022/12/06 新增 aqfh_help.py，install_requires新增ddddocr
+
+# 模块介绍
+
+## aqfh 定级备案爬虫(仅获取数据，不做数据处理)
+
+## awvs AWVS接口调用(待完善)
+
+## chromedriver chromedriver自动更新
+
+## common 通用数据处理
+
+## configparser 配置文件读取、写入、转json
+
+## csv cvs文件读取、写入
+
+## des DES(ECB)加解密
+
+## dingtalk 钉钉群机器人接口调用
+
+## dnspython 解析域名到IP、CNAME
+
+## docxtpl 根据模板生成word
+
+## fofa fofa查询接口调用
+
+## github github查询搜索接口调用
+
+## hashlib 字符串、文件md5
+
+## ipaddress 网段、IP格式转化
+
+## logging 日志
+
+## nessus nessus接口调用
+
+## openpyxl xlsx精细化编辑
+
+## paramiko ssh操作类封装
+
+## pymysql mysql操作类封装
+
+## re 常用正则
+
+## rsas 绿盟扫描器接口封装(爬虫版)
+
+## rsas_xls 绿盟扫描结果处理
+
+## sqlite sqlite操作类封装
+
+## tmpdb 简易kv数据库操作
+
+## xlrd excel文件读取
+
+## xlsxwriter xlsx文件写入
+
+## xlwt xls文件写入
+
+## yaml yaml文件读取写入
+
+## zipfile zip解压、压缩
+
+## zmail 邮件发送
+
+
+
```

### Comparing `sh2d-0.9/mylib/aqfh_help.py` & `sh2d-1.1/mylib/aqfh_help.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,151 +1,151 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import time
-import base64
-import requests
-import ddddocr
-import hashlib
-import random
-from requests.adapters import HTTPAdapter
-requests.packages.urllib3.disable_warnings()
-# 添加自动重试
-requests = requests.Session()
-requests.mount('http://', HTTPAdapter(max_retries=3))
-requests.mount('https://', HTTPAdapter(max_retries=3))
-
-
-class AQFHClient:
-    def __init__(self, url, username, password):
-        self.url = url
-        self.username = username
-        self.password = password
-        self.headers = {
-            "Referer": url,
-            "Accept": "application/json, text/plain, */*",
-            "X-Requested-With": "XMLHttpRequest",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.38 (KHTML, like Gecko) Chrome/105.0.5195.54 Safari/537.36",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "zh-CN,zh;q=0.91"
-        }
-        self.data = {}
-
-    def connect(self, method, resource, data=None):
-        '''请求'''
-        r = getattr(requests, method.lower())('{0}{1}'.format(
-            self.url, resource), json=data, headers=self.headers, verify=False, allow_redirects=False)
-        r.encoding = r.apparent_encoding
-        time.sleep(random.randint(10, 30)/10)
-        print('[{}]'.format(r.status_code), method, resource)
-        if r.status_code == 200:
-            try:
-                return r.status_code, r.json()
-            except:
-                return r.status_code, r.text
-        else:
-            self.connect(method, resource, data)
-
-    def login(self):
-        '''自动登录'''
-        _, rj1 = self.connect('GET', '/api/api/code')
-        ocr = ddddocr.DdddOcr(show_ad=False)
-        code = ocr.classification(base64.b64decode(
-            rj1['data']['img'].replace('data:image/png;base64,', '')))
-        data = {"account": self.username, "password": hashlib.new('sha1', self.password.encode(
-            'utf-8')).hexdigest(), "code": code, "key": rj1['data']['key']}
-        _, rj2 = self.connect('POST', '/api/api/login', data)
-        if rj2['message'] == "Success":
-            self.headers['Authorization'] = 'Bearer {}'.format(
-                rj2['data']['access_token'])
-            print('[+] 登录成功')
-            return True
-        elif rj2['message'] == "验证码有误":
-            print('[*] 验证码有误,重试中')
-            self.login()
-        else:
-            print('[-] 登录失败,', rj2['message'])
-            return False
-
-    def getObjectList(self, name="", neteid="", rank=[], status=[], creator_name=""):
-        '''定级对象列表'''
-        page = 1
-        while True:
-            data = {"name": name, "neteid": neteid, "rank": rank, "status": status, "time": "", "reviewer_name": "", "review_status": "", "apply_back_status": "",
-                    "creator_name": creator_name, "company_name": "", "updated_at": "", "comment_time_start": "", "comment_time_end": "", "page": page, "companytype": "3"}
-            _, rj = self.connect('POST', '/api/api/getObjectList', data)
-            for item in rj['data']['data']:
-                _id = item['id']
-                self.data.setdefault('ObjectList', {})
-                self.data['ObjectList'][_id] = item
-            print('[+] 当前第{}页，系统数为：{}'.format(page, rj['data']['total']))
-            if page * 10 > rj['data']['total']:
-                break
-            page += 1
-
-    def getObjectInfo(self, _id):
-        '''定级对象信息'''
-        data = {"id": _id, "companytype": "3"}
-        _, rj = self.connect('POST', '/api/api/getObjectInfo', data)
-        self.data['ObjectList'][_id]['ObjectInfo'] = rj['data']
-
-    def getObjectAttachmentReviewProve(self, _id):
-        '''符合性评测'''
-        data = {"id": _id}
-        _, rj = self.connect(
-            'POST', '/api/api/getObjectAttachmentReviewProve', data)
-        self.data['ObjectList'][_id]['ObjectAttachmentReviewProve'] = rj['data']
-
-    def getTitleList(self, _id, nete_id):
-        '''符合性评测表'''
-        data = {"id": _id, "neteid": nete_id, "companytype": "3"}
-        _, rj = self.connect(
-            'POST', '/api/api/getTitleList', data)
-        self.data['ObjectList'][_id]['TitleList'] = rj['data']
-
-    def getObjectAttachmentRisk(self, _id):
-        '''风险评估'''
-        data = {"id": _id}
-        _, rj = self.connect(
-            'POST', '/api/api/reviewGetObjectAttachmentRisk', data)
-        self.data['ObjectList'][_id]['ObjectAttachmentRisk'] = rj['data']
-
-    def getIpList(self, _id):
-        '''IP列表'''
-        page = 1
-        while True:
-            data = {"id": _id, "current_page": 1, "per_page": 10}
-            _, rj = self.connect('POST', '/api/api/getIpList', data=data)
-            self.data['ObjectList'][_id].setdefault('IpList', [])
-            self.data['ObjectList'][_id]['IpList'] += rj['data']['data']
-            if page*10 > rj['data']['total']:
-                break
-            page += 1
-
-    def getAllAssistant(self):
-        '''用户id列表'''
-        _, rj = self.connect('POST', '/api/api/getAllAssistant')
-        self.data['AllAssistant'] = rj['data']
-
-    def getNetType(self):
-        '''网络id列表'''
-        _, rj = self.connect('GET', '/api/api/common/getNetType')
-        self.data['NetType'] = rj['data']
-
-    def getcountObject(self):
-        '''统计'''
-        _, rj = self.connect('POST', '/api/api/countObject')
-        self.data['countObject'] = rj['data']
-
-    def getexportObjectURL(self):
-        '''导出对象下载地址'''
-        data = {"apply_back_status": "", "comment_time_end": "", "comment_time_start": "", "company_name": "", "companytype": "3", "creator_name": "", "expire_status": "",
-                "name": "", "neteid": "", "page": 1, "public_ip": "", "rank": [], "review_status": [], "reviewer_name": "", "software_ip": "", "status": [], "time": "", "updated_at": ""}
-        _, rj = self.connect('POST', '/api/api/exportObjectList', data=data)
-        self.data['exportObjectURL'] = rj['data']['url']
-
-    def download(self, path, url):
-        '''下载文件'''
-        print('[+] download', path)
-        with open(path, 'wb') as f:
-            f.write(requests.get(url, headers=self.headers,
-                    verify=False, allow_redirects=False).content)
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import time
+import base64
+import requests
+import ddddocr
+import hashlib
+import random
+from requests.adapters import HTTPAdapter
+requests.packages.urllib3.disable_warnings()
+# 添加自动重试
+requests = requests.Session()
+requests.mount('http://', HTTPAdapter(max_retries=3))
+requests.mount('https://', HTTPAdapter(max_retries=3))
+
+
+class AQFHClient:
+    def __init__(self, url, username, password):
+        self.url = url
+        self.username = username
+        self.password = password
+        self.headers = {
+            "Referer": url,
+            "Accept": "application/json, text/plain, */*",
+            "X-Requested-With": "XMLHttpRequest",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.38 (KHTML, like Gecko) Chrome/105.0.5195.54 Safari/537.36",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "zh-CN,zh;q=0.91"
+        }
+        self.data = {}
+
+    def connect(self, method, resource, data=None):
+        '''请求'''
+        r = getattr(requests, method.lower())('{0}{1}'.format(
+            self.url, resource), json=data, headers=self.headers, verify=False, allow_redirects=False)
+        r.encoding = r.apparent_encoding
+        time.sleep(random.randint(10, 30)/10)
+        print('[{}]'.format(r.status_code), method, resource)
+        if r.status_code == 200:
+            try:
+                return r.status_code, r.json()
+            except:
+                return r.status_code, r.text
+        else:
+            self.connect(method, resource, data)
+
+    def login(self):
+        '''自动登录'''
+        _, rj1 = self.connect('GET', '/api/api/code')
+        ocr = ddddocr.DdddOcr(show_ad=False)
+        code = ocr.classification(base64.b64decode(
+            rj1['data']['img'].replace('data:image/png;base64,', '')))
+        data = {"account": self.username, "password": hashlib.new('sha1', self.password.encode(
+            'utf-8')).hexdigest(), "code": code, "key": rj1['data']['key']}
+        _, rj2 = self.connect('POST', '/api/api/login', data)
+        if rj2['message'] == "Success":
+            self.headers['Authorization'] = 'Bearer {}'.format(
+                rj2['data']['access_token'])
+            print('[+] 登录成功')
+            return True
+        elif rj2['message'] == "验证码有误":
+            print('[*] 验证码有误,重试中')
+            self.login()
+        else:
+            print('[-] 登录失败,', rj2['message'])
+            return False
+
+    def getObjectList(self, name="", neteid="", rank=[], status=[], creator_name=""):
+        '''定级对象列表'''
+        page = 1
+        while True:
+            data = {"name": name, "neteid": neteid, "rank": rank, "status": status, "time": "", "reviewer_name": "", "review_status": "", "apply_back_status": "",
+                    "creator_name": creator_name, "company_name": "", "updated_at": "", "comment_time_start": "", "comment_time_end": "", "page": page, "companytype": "3"}
+            _, rj = self.connect('POST', '/api/api/getObjectList', data)
+            for item in rj['data']['data']:
+                _id = item['id']
+                self.data.setdefault('ObjectList', {})
+                self.data['ObjectList'][_id] = item
+            print('[+] 当前第{}页，系统数为：{}'.format(page, rj['data']['total']))
+            if page * 10 > rj['data']['total']:
+                break
+            page += 1
+
+    def getObjectInfo(self, _id):
+        '''定级对象信息'''
+        data = {"id": _id, "companytype": "3"}
+        _, rj = self.connect('POST', '/api/api/getObjectInfo', data)
+        self.data['ObjectList'][_id]['ObjectInfo'] = rj['data']
+
+    def getObjectAttachmentReviewProve(self, _id):
+        '''符合性评测'''
+        data = {"id": _id}
+        _, rj = self.connect(
+            'POST', '/api/api/getObjectAttachmentReviewProve', data)
+        self.data['ObjectList'][_id]['ObjectAttachmentReviewProve'] = rj['data']
+
+    def getTitleList(self, _id, nete_id):
+        '''符合性评测表'''
+        data = {"id": _id, "neteid": nete_id, "companytype": "3"}
+        _, rj = self.connect(
+            'POST', '/api/api/getTitleList', data)
+        self.data['ObjectList'][_id]['TitleList'] = rj['data']
+
+    def getObjectAttachmentRisk(self, _id):
+        '''风险评估'''
+        data = {"id": _id}
+        _, rj = self.connect(
+            'POST', '/api/api/reviewGetObjectAttachmentRisk', data)
+        self.data['ObjectList'][_id]['ObjectAttachmentRisk'] = rj['data']
+
+    def getIpList(self, _id):
+        '''IP列表'''
+        page = 1
+        while True:
+            data = {"id": _id, "current_page": 1, "per_page": 10}
+            _, rj = self.connect('POST', '/api/api/getIpList', data=data)
+            self.data['ObjectList'][_id].setdefault('IpList', [])
+            self.data['ObjectList'][_id]['IpList'] += rj['data']['data']
+            if page*10 > rj['data']['total']:
+                break
+            page += 1
+
+    def getAllAssistant(self):
+        '''用户id列表'''
+        _, rj = self.connect('POST', '/api/api/getAllAssistant')
+        self.data['AllAssistant'] = rj['data']
+
+    def getNetType(self):
+        '''网络id列表'''
+        _, rj = self.connect('GET', '/api/api/common/getNetType')
+        self.data['NetType'] = rj['data']
+
+    def getcountObject(self):
+        '''统计'''
+        _, rj = self.connect('POST', '/api/api/countObject')
+        self.data['countObject'] = rj['data']
+
+    def getexportObjectURL(self):
+        '''导出对象下载地址'''
+        data = {"apply_back_status": "", "comment_time_end": "", "comment_time_start": "", "company_name": "", "companytype": "3", "creator_name": "", "expire_status": "",
+                "name": "", "neteid": "", "page": 1, "public_ip": "", "rank": [], "review_status": [], "reviewer_name": "", "software_ip": "", "status": [], "time": "", "updated_at": ""}
+        _, rj = self.connect('POST', '/api/api/exportObjectList', data=data)
+        self.data['exportObjectURL'] = rj['data']['url']
+
+    def download(self, path, url):
+        '''下载文件'''
+        print('[+] download', path)
+        with open(path, 'wb') as f:
+            f.write(requests.get(url, headers=self.headers,
+                    verify=False, allow_redirects=False).content)
```

### Comparing `sh2d-0.9/mylib/awvs_help.py` & `sh2d-1.1/mylib/awvs_help.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import json
-import requests
-from requests.adapters import HTTPAdapter
-requests.packages.urllib3.disable_warnings()
-# 添加自动重试
-requests = requests.Session()
-requests.mount('http://', HTTPAdapter(max_retries=3))
-requests.mount('https://', HTTPAdapter(max_retries=3))
-
-class AWVSClient:
-
-    def __init__(self, url, api_key):
-
-        self.url = url
-        self.headers = {'X-Auth': api_key, 'Content-Type': 'application/json'}
-
-    def connect(self, method, resource, data=None):
-        print('[{}] {}'.format(method,resource))
-        if data:
-            data = json.dumps(data)
-        r = getattr(requests, method.lower())('{0}{1}'.format(
-            self.url, resource), data=data, headers=self.headers, timeout=20, verify=False)
-        r.encoding = r.apparent_encoding
-        try:
-            return r.status_code, r.headers, r.json()
-        except:
-            if 'text' in r.headers.get('Content-Type', ''):
-                return r.status_code, r.headers, r.text
-            else:
-                return r.status_code, r.headers, r.content
-
-    def get_targets(self):
-        '''获取所有目标'''
-        c = 0
-        while True:
-            _, _, rs = self.connect(
-                'GET', '/api/v1/targets?c={}&l=100'.format(c*100))
-            c += 1
-            if not len(rs["targets"]):
-                break
-            for s in rs["targets"]:
-                yield s['target_id'], s['address']
-
-    def add_target(self, url):
-        '''添加目标'''
-        data = {"address": url, "description": url, "criticality": "10"}
-        _, _, rs = self.connect('POST', '/api/v1/targets', data)
-        return rs['target_id']
-
-    def del_target(self, target_id):
-        '''删除目标'''
-        rc, _, _ = self.connect(
-            'DELETE', '/api/v1/targets/{}'.format(target_id))
-        return True if rc == 204 else False
-
-    def add_scan(self, target_id, rule='full'):
-        '''添加扫描'''
-        rules = {
-            "full": "11111111-1111-1111-1111-111111111111",
-            "highrisk": "11111111-1111-1111-1111-111111111112",
-            "XSS": "11111111-1111-1111-1111-111111111116",
-            "SQL": "11111111-1111-1111-1111-111111111113",
-            "Weakpass": "11111111-1111-1111-1111-111111111115",
-            "crawlonly": "11111111-1111-1111-1111-111111111117"
-        }
-        data = {'target_id': target_id, 'profile_id': rules[rule], 'schedule': {
-            'disable': False, 'start_date': None, 'time_sensitive': False}}
-        rc, _, _ = self.connect('POST', '/api/v1/scans', data)
-        return True if rc == 201 else False
-
-    def get_scans(self):
-        '''获取所有扫描'''
-        c = 0
-        while True:
-            _, _, rs = self.connect(
-                'GET', '/api/v1/scans?c={}&l=100&q=threat:1,2,3;&s=target_address:desc'.format(c*100))
-            c += 1
-            if not len(rs["scans"]):
-                break
-            for s in rs["scans"]:
-                yield s['scan_id'], s['current_session']['scan_session_id'],s['current_session']['severity_counts'] 
-
-    def get_vulns(self, scan_id, scan_session_id):
-        '''获取漏洞id'''
-        c = 0
-        while True:
-            _, _, rs = self.connect(
-                'GET', '/api/v1/scans/{}/results/{}/vulnerabilities?c={}'.format(scan_id, scan_session_id, c*100))
-            c += 1
-            if not len(rs["vulnerabilities"]):
-                break
-            for s in rs["vulnerabilities"]:
-                yield s['vuln_id']
-
-    def get_vuln_details(self, scan_id, scan_session_id, vuln_id):
-        '''获取漏洞详情'''
-        vuln = {}
-        _, _, rs = self.connect(
-            'GET', '/api/v1/scans/{}/results/{}/vulnerabilities/{}'.format(scan_id, scan_session_id, vuln_id)) 
-        vuln['affects_url'] =rs.get('affects_url','')
-        vuln['target_description'] =rs.get('target_description','')
-        vuln['vt_name'] = rs.get('vt_name','') 
-        vuln['severity'] = rs.get('severity','') 
-        vuln['description'] = rs.get('description','') 
-        vuln['impact'] = rs.get('impact','') 
-        vuln['recommendation'] = rs.get('recommendation','') 
-        vuln['details'] = rs.get('details','') 
-        vuln['recommendation'] = rs.get('recommendation','') 
-        vuln['request'] = rs.get('request','') 
-        return vuln
-
-    def get_vuln_http_response(self, scan_id, scan_session_id, vuln_id):
-        '''获取漏洞详情'''
-        _, _, rs = self.connect(
-            'GET', '/api/v1/scans/{}/results/{}/vulnerabilities/{}/http_response'.format(scan_id, scan_session_id, vuln_id))
-        return rs
-
-if __name__ == '__main__':
-    url = 'https://127.0.0.1:3443'
-    api_key = '1986ad8c0a5b3df4d7028d5f3c06e936c09b72504c2714a7c934c1247cd7be59c'
-
-    awvs = AWVSClient(url, api_key)
-
-    # 导出漏洞清单
-    # vulns = []
-    # from mylib import jsonlist2xlsx
-    # for scan_id,scan_session_id,severity_counts in awvs.get_scans():
-    #     if sum([severity_counts[i] for i in ['high','medium','low','info']]) == 0:continue
-    #     for vuln_id in awvs.get_vulns(scan_id, scan_session_id):
-    #         vuln = awvs.get_vuln_details(scan_id, scan_session_id, vuln_id)
-    #         vuln['http_response'] = awvs.get_vuln_http_response(scan_id, scan_session_id, vuln_id)
-    #         vulns.append(vuln)
-    # jsonlist2xlsx('vuln.xlsx',vuln=vulns)
-
-    
-
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import json
+import requests
+from requests.adapters import HTTPAdapter
+requests.packages.urllib3.disable_warnings()
+# 添加自动重试
+requests = requests.Session()
+requests.mount('http://', HTTPAdapter(max_retries=3))
+requests.mount('https://', HTTPAdapter(max_retries=3))
+
+class AWVSClient:
+
+    def __init__(self, url, api_key):
+
+        self.url = url
+        self.headers = {'X-Auth': api_key, 'Content-Type': 'application/json'}
+
+    def connect(self, method, resource, data=None):
+        print('[{}] {}'.format(method,resource))
+        if data:
+            data = json.dumps(data)
+        r = getattr(requests, method.lower())('{0}{1}'.format(
+            self.url, resource), data=data, headers=self.headers, timeout=20, verify=False)
+        r.encoding = r.apparent_encoding
+        try:
+            return r.status_code, r.headers, r.json()
+        except:
+            if 'text' in r.headers.get('Content-Type', ''):
+                return r.status_code, r.headers, r.text
+            else:
+                return r.status_code, r.headers, r.content
+
+    def get_targets(self):
+        '''获取所有目标'''
+        c = 0
+        while True:
+            _, _, rs = self.connect(
+                'GET', '/api/v1/targets?c={}&l=100'.format(c*100))
+            c += 1
+            if not len(rs["targets"]):
+                break
+            for s in rs["targets"]:
+                yield s['target_id'], s['address']
+
+    def add_target(self, url):
+        '''添加目标'''
+        data = {"address": url, "description": url, "criticality": "10"}
+        _, _, rs = self.connect('POST', '/api/v1/targets', data)
+        return rs['target_id']
+
+    def del_target(self, target_id):
+        '''删除目标'''
+        rc, _, _ = self.connect(
+            'DELETE', '/api/v1/targets/{}'.format(target_id))
+        return True if rc == 204 else False
+
+    def add_scan(self, target_id, rule='full'):
+        '''添加扫描'''
+        rules = {
+            "full": "11111111-1111-1111-1111-111111111111",
+            "highrisk": "11111111-1111-1111-1111-111111111112",
+            "XSS": "11111111-1111-1111-1111-111111111116",
+            "SQL": "11111111-1111-1111-1111-111111111113",
+            "Weakpass": "11111111-1111-1111-1111-111111111115",
+            "crawlonly": "11111111-1111-1111-1111-111111111117"
+        }
+        data = {'target_id': target_id, 'profile_id': rules[rule], 'schedule': {
+            'disable': False, 'start_date': None, 'time_sensitive': False}}
+        rc, _, _ = self.connect('POST', '/api/v1/scans', data)
+        return True if rc == 201 else False
+
+    def get_scans(self):
+        '''获取所有扫描'''
+        c = 0
+        while True:
+            _, _, rs = self.connect(
+                'GET', '/api/v1/scans?c={}&l=100&q=threat:1,2,3;&s=target_address:desc'.format(c*100))
+            c += 1
+            if not len(rs["scans"]):
+                break
+            for s in rs["scans"]:
+                yield s['scan_id'], s['current_session']['scan_session_id'],s['current_session']['severity_counts'] 
+
+    def get_vulns(self, scan_id, scan_session_id):
+        '''获取漏洞id'''
+        c = 0
+        while True:
+            _, _, rs = self.connect(
+                'GET', '/api/v1/scans/{}/results/{}/vulnerabilities?c={}'.format(scan_id, scan_session_id, c*100))
+            c += 1
+            if not len(rs["vulnerabilities"]):
+                break
+            for s in rs["vulnerabilities"]:
+                yield s['vuln_id']
+
+    def get_vuln_details(self, scan_id, scan_session_id, vuln_id):
+        '''获取漏洞详情'''
+        vuln = {}
+        _, _, rs = self.connect(
+            'GET', '/api/v1/scans/{}/results/{}/vulnerabilities/{}'.format(scan_id, scan_session_id, vuln_id)) 
+        vuln['affects_url'] =rs.get('affects_url','')
+        vuln['target_description'] =rs.get('target_description','')
+        vuln['vt_name'] = rs.get('vt_name','') 
+        vuln['severity'] = rs.get('severity','') 
+        vuln['description'] = rs.get('description','') 
+        vuln['impact'] = rs.get('impact','') 
+        vuln['recommendation'] = rs.get('recommendation','') 
+        vuln['details'] = rs.get('details','') 
+        vuln['recommendation'] = rs.get('recommendation','') 
+        vuln['request'] = rs.get('request','') 
+        return vuln
+
+    def get_vuln_http_response(self, scan_id, scan_session_id, vuln_id):
+        '''获取漏洞详情'''
+        _, _, rs = self.connect(
+            'GET', '/api/v1/scans/{}/results/{}/vulnerabilities/{}/http_response'.format(scan_id, scan_session_id, vuln_id))
+        return rs
+
+if __name__ == '__main__':
+    url = 'https://127.0.0.1:3443'
+    api_key = '1986ad8c0a5b3df4d7028d5f3c06e936c09b72504c2714a7c934c1247cd7be59c'
+
+    awvs = AWVSClient(url, api_key)
+
+    # 导出漏洞清单
+    # vulns = []
+    # from mylib import jsonlist2xlsx
+    # for scan_id,scan_session_id,severity_counts in awvs.get_scans():
+    #     if sum([severity_counts[i] for i in ['high','medium','low','info']]) == 0:continue
+    #     for vuln_id in awvs.get_vulns(scan_id, scan_session_id):
+    #         vuln = awvs.get_vuln_details(scan_id, scan_session_id, vuln_id)
+    #         vuln['http_response'] = awvs.get_vuln_http_response(scan_id, scan_session_id, vuln_id)
+    #         vulns.append(vuln)
+    # jsonlist2xlsx('vuln.xlsx',vuln=vulns)
+
+    
+
```

### Comparing `sh2d-0.9/mylib/beian_help.py` & `sh2d-1.1/mylib/beian_help.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import os
-import time
-import cv2
-import base64
-import hashlib
-import requests
-
-requests.packages.urllib3.disable_warnings()
-
-def beian(name):
-    '''
-    :param name  支持公司标准名称、域名、备案号查询
-    :return [{'目标': '', '主办单位': ' ', '单位性质': '', '网站备案号': '', '审核日期': '', '是否限制接入': ''}]
-    '''
-    result = []
-    headers = {
-        'Connection': 'keep-alive',
-        'Content-Length': '0',
-        'sec-ch-ua': '" Not A;Brand";v="99", "Chromium";v="90", "Microsoft Edge";v="90"',
-        'Accept': 'application/json, text/plain, */*',
-        'DNT': '1',
-        'sec-ch-ua-mobile': '?0',
-        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36 Edg/90.0.818.46',
-        'Origin': 'https://beian.miit.gov.cn',
-        'Sec-Fetch-Site': 'same-site',
-        'Sec-Fetch-Mode': 'cors',
-        'Sec-Fetch-Dest': 'empty',
-        'Referer': 'https://beian.miit.gov.cn/',
-        'Accept-Encoding': 'gzip, deflate, br',
-        'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6'}
-    try:
-        # 获取 __jsluid_s
-        __jsluid_s = requests.utils.dict_from_cookiejar(requests.get(
-            'https://beian.miit.gov.cn/', headers=headers).cookies)['__jsluid_s']
-        # 获取token
-        timeStamp = int(round(time.time()*1000))
-        authSecret = 'testtest' + str(timeStamp)
-        authKey = hashlib.md5(authSecret.encode(encoding='UTF-8')).hexdigest()
-        rj1 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/auth', data={
-                            'authKey': authKey, 'timeStamp': timeStamp}, headers={**headers, **{'Cookie': '__jsluid_s='+__jsluid_s}}).json()
-        if rj1['success']:
-            token = rj1['params']['bussiness']
-            # 获取验证图像、UUID
-            rj2 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/image/getCheckImage',
-                                data='', headers={**headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token}}).json()
-            if rj2['success']:
-                p_uuid = rj2['params']['uuid']
-                big_image = rj2['params']['bigImage']
-                small_image = rj2['params']['smallImage']
-                # 解码图片，写入并计算图片缺口位置
-                with open('bigImage.jpg', 'wb') as f:
-                    f.write(base64.b64decode(big_image))
-                    f.close()
-                with open('smallImage.jpg', 'wb') as f:
-                    f.write(base64.b64decode(small_image))
-                    f.close()
-                background_image = cv2.imread(
-                    'bigImage.jpg', cv2.COLOR_GRAY2RGB)
-                fill_image = cv2.imread('smallImage.jpg', cv2.COLOR_GRAY2RGB)
-                position_match = cv2.matchTemplate(
-                    background_image, fill_image, cv2.TM_CCOEFF_NORMED)
-                _, _, _, max_loc = cv2.minMaxLoc(position_match)
-                mouse_length = max_loc[0]+1
-                # 通过拼图验证，获取sign
-                rj3 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/image/checkImage', json={'key': p_uuid, 'value': mouse_length}, headers={
-                                    **headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token, 'Content-Type': 'application/json'}}).json()
-                if rj3['success']:
-                    sign = rj3['params']
-                    # 获取备案信息
-                    rj4 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/icpAbbreviateInfo/queryByCondition', json={'pageNum': '', 'pageSize': '', 'unitName': name}, headers={
-                                        **headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token, 'sign': sign, 'uuid': p_uuid, 'Content-Type': 'application/json'}}).json()
-                    if rj4['success']:
-                        for item in rj4['params']['list']:
-                            info = {}
-                            info['域名'] = item['domain']
-                            info['主办单位'] = item['unitName']
-                            info['单位性质'] = item['natureName']
-                            info['网站备案号'] = item['serviceLicence']
-                            info['审核日期'] = item['updateRecordTime']
-                            info['是否限制接入'] = item['limitAccess']
-                            result.append(info)
-                        total_page = rj4['params']['pages']
-                        if total_page > 1:
-                            for i in range(1, total_page):
-                                rj5 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/icpAbbreviateInfo/queryByCondition', json={'pageNum': i+1, 'pageSize': 10, 'unitName': name}, headers={
-                                                    **headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token, 'sign': sign, 'uuid': p_uuid, 'Content-Type': 'application/json'}}).json()
-                                if rj5['success']:
-                                    for item in rj5['params']['list']:
-                                        info = {}
-                                        info['域名'] = item['domain']
-                                        info['主办单位'] = item['unitName']
-                                        info['单位性质'] = item['natureName']
-                                        info['网站备案号'] = item['serviceLicence']
-                                        info['审核日期'] = item['updateRecordTime']
-                                        info['是否限制接入'] = item['limitAccess']
-                                        result.append(info)
-                                else:
-                                    print('获取备案信息', i+1, rj5['msg'])
-                    else:
-                        print('获取备案信息', rj4['msg'])
-                else:
-                    print('通过拼图验证，获取sign', rj3['msg'])
-            else:
-                print('获取验证图像、UUID', rj2['msg'])
-        else:
-            print('获取token', rj1['msg'])
-    except:
-        pass
-
-    try:
-        os.remove('bigImage.jpg')
-        os.remove('smallImage.jpg')
-    except:
-        pass
-    return result
-
-if __name__ == '__main__':
-    name = '沪ICP备13033796号'
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import os
+import time
+import cv2
+import base64
+import hashlib
+import requests
+
+requests.packages.urllib3.disable_warnings()
+
+def beian(name):
+    '''
+    :param name  支持公司标准名称、域名、备案号查询
+    :return [{'目标': '', '主办单位': ' ', '单位性质': '', '网站备案号': '', '审核日期': '', '是否限制接入': ''}]
+    '''
+    result = []
+    headers = {
+        'Connection': 'keep-alive',
+        'Content-Length': '0',
+        'sec-ch-ua': '" Not A;Brand";v="99", "Chromium";v="90", "Microsoft Edge";v="90"',
+        'Accept': 'application/json, text/plain, */*',
+        'DNT': '1',
+        'sec-ch-ua-mobile': '?0',
+        'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/90.0.4430.85 Safari/537.36 Edg/90.0.818.46',
+        'Origin': 'https://beian.miit.gov.cn',
+        'Sec-Fetch-Site': 'same-site',
+        'Sec-Fetch-Mode': 'cors',
+        'Sec-Fetch-Dest': 'empty',
+        'Referer': 'https://beian.miit.gov.cn/',
+        'Accept-Encoding': 'gzip, deflate, br',
+        'Accept-Language': 'zh-CN,zh;q=0.9,en;q=0.8,en-GB;q=0.7,en-US;q=0.6'}
+    try:
+        # 获取 __jsluid_s
+        __jsluid_s = requests.utils.dict_from_cookiejar(requests.get(
+            'https://beian.miit.gov.cn/', headers=headers).cookies)['__jsluid_s']
+        # 获取token
+        timeStamp = int(round(time.time()*1000))
+        authSecret = 'testtest' + str(timeStamp)
+        authKey = hashlib.md5(authSecret.encode(encoding='UTF-8')).hexdigest()
+        rj1 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/auth', data={
+                            'authKey': authKey, 'timeStamp': timeStamp}, headers={**headers, **{'Cookie': '__jsluid_s='+__jsluid_s}}).json()
+        if rj1['success']:
+            token = rj1['params']['bussiness']
+            # 获取验证图像、UUID
+            rj2 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/image/getCheckImage',
+                                data='', headers={**headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token}}).json()
+            if rj2['success']:
+                p_uuid = rj2['params']['uuid']
+                big_image = rj2['params']['bigImage']
+                small_image = rj2['params']['smallImage']
+                # 解码图片，写入并计算图片缺口位置
+                with open('bigImage.jpg', 'wb') as f:
+                    f.write(base64.b64decode(big_image))
+                    f.close()
+                with open('smallImage.jpg', 'wb') as f:
+                    f.write(base64.b64decode(small_image))
+                    f.close()
+                background_image = cv2.imread(
+                    'bigImage.jpg', cv2.COLOR_GRAY2RGB)
+                fill_image = cv2.imread('smallImage.jpg', cv2.COLOR_GRAY2RGB)
+                position_match = cv2.matchTemplate(
+                    background_image, fill_image, cv2.TM_CCOEFF_NORMED)
+                _, _, _, max_loc = cv2.minMaxLoc(position_match)
+                mouse_length = max_loc[0]+1
+                # 通过拼图验证，获取sign
+                rj3 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/image/checkImage', json={'key': p_uuid, 'value': mouse_length}, headers={
+                                    **headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token, 'Content-Type': 'application/json'}}).json()
+                if rj3['success']:
+                    sign = rj3['params']
+                    # 获取备案信息
+                    rj4 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/icpAbbreviateInfo/queryByCondition', json={'pageNum': '', 'pageSize': '', 'unitName': name}, headers={
+                                        **headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token, 'sign': sign, 'uuid': p_uuid, 'Content-Type': 'application/json'}}).json()
+                    if rj4['success']:
+                        for item in rj4['params']['list']:
+                            info = {}
+                            info['域名'] = item['domain']
+                            info['主办单位'] = item['unitName']
+                            info['单位性质'] = item['natureName']
+                            info['网站备案号'] = item['serviceLicence']
+                            info['审核日期'] = item['updateRecordTime']
+                            info['是否限制接入'] = item['limitAccess']
+                            result.append(info)
+                        total_page = rj4['params']['pages']
+                        if total_page > 1:
+                            for i in range(1, total_page):
+                                rj5 = requests.post('https://hlwicpfwc.miit.gov.cn/icpproject_query/api/icpAbbreviateInfo/queryByCondition', json={'pageNum': i+1, 'pageSize': 10, 'unitName': name}, headers={
+                                                    **headers, **{'Cookie': '__jsluid_s='+__jsluid_s, 'token': token, 'sign': sign, 'uuid': p_uuid, 'Content-Type': 'application/json'}}).json()
+                                if rj5['success']:
+                                    for item in rj5['params']['list']:
+                                        info = {}
+                                        info['域名'] = item['domain']
+                                        info['主办单位'] = item['unitName']
+                                        info['单位性质'] = item['natureName']
+                                        info['网站备案号'] = item['serviceLicence']
+                                        info['审核日期'] = item['updateRecordTime']
+                                        info['是否限制接入'] = item['limitAccess']
+                                        result.append(info)
+                                else:
+                                    print('获取备案信息', i+1, rj5['msg'])
+                    else:
+                        print('获取备案信息', rj4['msg'])
+                else:
+                    print('通过拼图验证，获取sign', rj3['msg'])
+            else:
+                print('获取验证图像、UUID', rj2['msg'])
+        else:
+            print('获取token', rj1['msg'])
+    except:
+        pass
+
+    try:
+        os.remove('bigImage.jpg')
+        os.remove('smallImage.jpg')
+    except:
+        pass
+    return result
+
+if __name__ == '__main__':
+    name = '沪ICP备13033796号'
     print(beian(name))
```

### Comparing `sh2d-0.9/mylib/beianx_help.py` & `sh2d-1.1/mylib/beianx_help.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import requests
-from lxml import etree
-
-requests.packages.urllib3.disable_warnings()
-
-def beianx(name):
-    '''
-    :param name  支持公司名称、域名、备案号查询
-    :return [{'目标': '', '主办单位': ' ', '单位性质': '', '网站备案号': '', '网站名称': '', '网站首页': '', '审核日期': '', '是否限制接入': ''}]
-    '''
-    result = []
-    url = "https://www.beianx.cn/search/{}".format(name)
-    headers = {"Sec-Ch-Ua": "\"Chromium\";v=\"105\", \"Not)A;Brand\";v=\"8\"", "Sec-Ch-Ua-Mobile": "?0", "Sec-Ch-Ua-Platform": "\"Windows\"", "Upgrade-Insecure-Requests": "1",
-               "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.5195.54 Safari/537.36", "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9", "Sec-Fetch-Site": "none", "Sec-Fetch-Mode": "navigate", "Sec-Fetch-User": "?1", "Sec-Fetch-Dest": "document", "Accept-Encoding": "gzip, deflate", "Accept-Language": "zh-CN,zh;q=0.9", "Connection": "close"}
-    try:
-        r = requests.get(url, headers=headers, verify=False)
-        r.encoding = r.apparent_encoding
-        html = etree.HTML(r.text)
-        for tr in html.xpath('//tbody/tr'):
-            info = {}
-            info['主办单位'] = ''.join(tr.xpath('td[2]/a/text()')).strip()
-            info['单位性质'] = ''.join(tr.xpath('td[3]/text()')).strip()
-            info['网站备案号'] = ''.join(tr.xpath('td[4]/text()')).strip()
-            info['网站名称'] = ''.join(tr.xpath('td[5]/text()')).strip()
-            info['网站首页'] = ''.join(tr.xpath('td[6]/div/a/text()')).strip()
-            info['审核日期'] = ''.join(tr.xpath('td[7]/div/text()')).strip()
-            info['是否限制接入'] = ''.join(tr.xpath('td[8]/text()')).strip()
-            result.append(info)
-    except:
-        pass
-
-    return result
-
-if __name__ == '__main__':
-    name = '沪ICP备13033796号'
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import requests
+from lxml import etree
+
+requests.packages.urllib3.disable_warnings()
+
+def beianx(name):
+    '''
+    :param name  支持公司名称、域名、备案号查询
+    :return [{'目标': '', '主办单位': ' ', '单位性质': '', '网站备案号': '', '网站名称': '', '网站首页': '', '审核日期': '', '是否限制接入': ''}]
+    '''
+    result = []
+    url = "https://www.beianx.cn/search/{}".format(name)
+    headers = {"Sec-Ch-Ua": "\"Chromium\";v=\"105\", \"Not)A;Brand\";v=\"8\"", "Sec-Ch-Ua-Mobile": "?0", "Sec-Ch-Ua-Platform": "\"Windows\"", "Upgrade-Insecure-Requests": "1",
+               "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.5195.54 Safari/537.36", "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9", "Sec-Fetch-Site": "none", "Sec-Fetch-Mode": "navigate", "Sec-Fetch-User": "?1", "Sec-Fetch-Dest": "document", "Accept-Encoding": "gzip, deflate", "Accept-Language": "zh-CN,zh;q=0.9", "Connection": "close"}
+    try:
+        r = requests.get(url, headers=headers, verify=False)
+        r.encoding = r.apparent_encoding
+        html = etree.HTML(r.text)
+        for tr in html.xpath('//tbody/tr'):
+            info = {}
+            info['主办单位'] = ''.join(tr.xpath('td[2]/a/text()')).strip()
+            info['单位性质'] = ''.join(tr.xpath('td[3]/text()')).strip()
+            info['网站备案号'] = ''.join(tr.xpath('td[4]/text()')).strip()
+            info['网站名称'] = ''.join(tr.xpath('td[5]/text()')).strip()
+            info['网站首页'] = ''.join(tr.xpath('td[6]/div/a/text()')).strip()
+            info['审核日期'] = ''.join(tr.xpath('td[7]/div/text()')).strip()
+            info['是否限制接入'] = ''.join(tr.xpath('td[8]/text()')).strip()
+            result.append(info)
+    except:
+        pass
+
+    return result
+
+if __name__ == '__main__':
+    name = '沪ICP备13033796号'
     print(beianx(name))
```

### Comparing `sh2d-0.9/mylib/chinaz_help.py` & `sh2d-1.1/mylib/chinaz_help.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import requests
-from lxml import etree
-
-requests.packages.urllib3.disable_warnings()
-
-def whois(domain):
-    '''
-    :param domain  域名
-    :return [{'域名': '', '注册商': ' ', '联系人': '', '联系邮箱': '', '创建时间': '', '过期时间': ''}]
-    '''
-    result = []
-    info = {}
-    info['域名'] = domain
-    headers = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE'}
-    try:
-        r = requests.get(
-            f'https://whois.chinaz.com/{domain}', headers=headers, verify=False)
-        r.encoding = r.apparent_encoding
-        html = etree.HTML(r.text)
-        whois_info = html.xpath('//*[@id="whois_info"]')[0]
-        info['注册商'] = ''.join(whois_info.xpath(
-            '//div[text()="注册商"]/following-sibling::*[1]/div/span/text()'))
-        info['联系人'] = ''.join(whois_info.xpath(
-            '//div[text()="联系人"]/following-sibling::*[1]/span/text()'))
-        info['联系邮箱'] = ''.join(whois_info.xpath(
-            '//div[text()="联系邮箱"]/following-sibling::*[1]/span/text()'))
-        info['创建时间'] = ''.join(whois_info.xpath(
-            '//div[text()="创建时间"]/following-sibling::*[1]/span/text()'))
-        info['过期时间'] = ''.join(whois_info.xpath(
-            '//div[text()="过期时间"]/following-sibling::*[1]/span/text()'))
-    except:
-        pass
-    result.append(info)
-    return result
-
-def ipbatch(ips):
-    '''
-    :param ips  IP列表,单次限300
-    :return [{'域名/IP': '', '获取的IP地址': '', '数字地址': '', 'IP的物理位置': ''},]
-    '''
-    result = []
-    headers = {
-        'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE'}
-    try:
-        data = {'ips': '\r\n'.join(ips), 'submore': '查询'}
-        r = requests.post("https://ip.tool.chinaz.com/ipbatch",
-                          data=data, headers=headers, verify=False)
-        r.encoding = r.apparent_encoding
-        html = etree.HTML(r.text)
-        ipList = html.xpath('//*[@id="ipList"]')[0]
-        for tr in ipList.xpath('tr'):
-            info = {}
-            info['域名/IP'] = ''.join(tr.xpath('td[1]/text()')).strip()
-            info['获取的IP地址'] = ''.join(tr.xpath('td[2]/a/text()')).strip()
-            info['数字地址'] = ''.join(tr.xpath('td[3]/text()')).strip()
-            info['IP的物理位置'] = ''.join(tr.xpath('td[4]/text()')).strip()
-            result.append(info)
-    except:
-        pass
-
-    return result
-
-def icp(domains):
-    '''
-    :param domains  域名列表,单次限20
-    :return [{'域名': '', '主办单位': '', '单位性质': '', '备案号': '', '网站名称': '', '网站首页': '', '审核时间': '', '最近检测': ''},]
-    '''
-    result = []
-    try:
-        url = "https://micp.chinaz.com/Icp/BatchSearchs/"
-        headers = {"Cache-Control": "max-age=0", "Sec-Ch-Ua": "\"Chromium\";v=\"105\", \"Not)A;Brand\";v=\"8\"", "Sec-Ch-Ua-Mobile": "?0", "Sec-Ch-Ua-Platform": "\"Windows\"", "Upgrade-Insecure-Requests": "1", "Origin": "https://micp.chinaz.com", "Content-Type": "application/x-www-form-urlencoded", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.5195.54 Safari/537.36", "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9", "Sec-Fetch-Site": "same-origin", "Sec-Fetch-Mode": "navigate", "Sec-Fetch-User": "?1", "Sec-Fetch-Dest": "document", "Referer": "https://micp.chinaz.com/Icp/BatchSearchs/", "Accept-Encoding": "gzip, deflate", "Accept-Language": "zh-CN,zh;q=0.9"}
-        data = {"hosts": '\r\n'.join(domains)}
-        r = requests.post(url,
-                          data=data, headers=headers, verify=False)
-        r.encoding = r.apparent_encoding
-        html = etree.HTML(r.text)
-        for table in html.xpath('//table'):
-            info = {}
-            info['域名'] = ''.join(table.xpath('thead/tr/td/a/text()')).strip()
-            info['主办单位'] = ''.join(table.xpath('tbody/tr[1]/td[2]/text()')).strip()
-            info['单位性质'] = ''.join(table.xpath('tbody/tr[2]/td[2]/text()')).strip()
-            info['备案号'] = ''.join(table.xpath('tbody/tr[3]/td[2]/text()')).strip()
-            info['网站名称'] = ''.join(table.xpath('tbody/tr[4]/td[2]/text()')).strip()
-            info['网站首页'] = ''.join(table.xpath('tbody/tr[5]/td[2]/text()')).strip()
-            info['审核时间'] = ''.join(table.xpath('tbody/tr[6]/td[2]/text()')).strip()
-            info['最近检测'] = ''.join(table.xpath('tbody/tr[7]/td[2]/text()')).strip()
-            result.append(info)
-    except:
-        pass
-
-    return result
-
-
-
-if __name__ == '__main__':
-    domain = 'freebuf.com'
-    print(whois(domain))
-    ips = ['8.8.8.8','114.114.114.114']
-    print(ipbatch(ips))
-    domains = ['baidu.com','freebuf.com']
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import requests
+from lxml import etree
+
+requests.packages.urllib3.disable_warnings()
+
+def whois(domain):
+    '''
+    :param domain  域名
+    :return [{'域名': '', '注册商': ' ', '联系人': '', '联系邮箱': '', '创建时间': '', '过期时间': ''}]
+    '''
+    result = []
+    info = {}
+    info['域名'] = domain
+    headers = {
+        'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE'}
+    try:
+        r = requests.get(
+            f'https://whois.chinaz.com/{domain}', headers=headers, verify=False)
+        r.encoding = r.apparent_encoding
+        html = etree.HTML(r.text)
+        whois_info = html.xpath('//*[@id="whois_info"]')[0]
+        info['注册商'] = ''.join(whois_info.xpath(
+            '//div[text()="注册商"]/following-sibling::*[1]/div/span/text()'))
+        info['联系人'] = ''.join(whois_info.xpath(
+            '//div[text()="联系人"]/following-sibling::*[1]/span/text()'))
+        info['联系邮箱'] = ''.join(whois_info.xpath(
+            '//div[text()="联系邮箱"]/following-sibling::*[1]/span/text()'))
+        info['创建时间'] = ''.join(whois_info.xpath(
+            '//div[text()="创建时间"]/following-sibling::*[1]/span/text()'))
+        info['过期时间'] = ''.join(whois_info.xpath(
+            '//div[text()="过期时间"]/following-sibling::*[1]/span/text()'))
+    except:
+        pass
+    result.append(info)
+    return result
+
+def ipbatch(ips):
+    '''
+    :param ips  IP列表,单次限300
+    :return [{'域名/IP': '', '获取的IP地址': '', '数字地址': '', 'IP的物理位置': ''},]
+    '''
+    result = []
+    headers = {
+        'User-Agent': 'Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36 QIHU 360SE'}
+    try:
+        data = {'ips': '\r\n'.join(ips), 'submore': '查询'}
+        r = requests.post("https://ip.tool.chinaz.com/ipbatch",
+                          data=data, headers=headers, verify=False)
+        r.encoding = r.apparent_encoding
+        html = etree.HTML(r.text)
+        ipList = html.xpath('//*[@id="ipList"]')[0]
+        for tr in ipList.xpath('tr'):
+            info = {}
+            info['域名/IP'] = ''.join(tr.xpath('td[1]/text()')).strip()
+            info['获取的IP地址'] = ''.join(tr.xpath('td[2]/a/text()')).strip()
+            info['数字地址'] = ''.join(tr.xpath('td[3]/text()')).strip()
+            info['IP的物理位置'] = ''.join(tr.xpath('td[4]/text()')).strip()
+            result.append(info)
+    except:
+        pass
+
+    return result
+
+def icp(domains):
+    '''
+    :param domains  域名列表,单次限20
+    :return [{'域名': '', '主办单位': '', '单位性质': '', '备案号': '', '网站名称': '', '网站首页': '', '审核时间': '', '最近检测': ''},]
+    '''
+    result = []
+    try:
+        url = "https://micp.chinaz.com/Icp/BatchSearchs/"
+        headers = {"Cache-Control": "max-age=0", "Sec-Ch-Ua": "\"Chromium\";v=\"105\", \"Not)A;Brand\";v=\"8\"", "Sec-Ch-Ua-Mobile": "?0", "Sec-Ch-Ua-Platform": "\"Windows\"", "Upgrade-Insecure-Requests": "1", "Origin": "https://micp.chinaz.com", "Content-Type": "application/x-www-form-urlencoded", "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.5195.54 Safari/537.36", "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9", "Sec-Fetch-Site": "same-origin", "Sec-Fetch-Mode": "navigate", "Sec-Fetch-User": "?1", "Sec-Fetch-Dest": "document", "Referer": "https://micp.chinaz.com/Icp/BatchSearchs/", "Accept-Encoding": "gzip, deflate", "Accept-Language": "zh-CN,zh;q=0.9"}
+        data = {"hosts": '\r\n'.join(domains)}
+        r = requests.post(url,
+                          data=data, headers=headers, verify=False)
+        r.encoding = r.apparent_encoding
+        html = etree.HTML(r.text)
+        for table in html.xpath('//table'):
+            info = {}
+            info['域名'] = ''.join(table.xpath('thead/tr/td/a/text()')).strip()
+            info['主办单位'] = ''.join(table.xpath('tbody/tr[1]/td[2]/text()')).strip()
+            info['单位性质'] = ''.join(table.xpath('tbody/tr[2]/td[2]/text()')).strip()
+            info['备案号'] = ''.join(table.xpath('tbody/tr[3]/td[2]/text()')).strip()
+            info['网站名称'] = ''.join(table.xpath('tbody/tr[4]/td[2]/text()')).strip()
+            info['网站首页'] = ''.join(table.xpath('tbody/tr[5]/td[2]/text()')).strip()
+            info['审核时间'] = ''.join(table.xpath('tbody/tr[6]/td[2]/text()')).strip()
+            info['最近检测'] = ''.join(table.xpath('tbody/tr[7]/td[2]/text()')).strip()
+            result.append(info)
+    except:
+        pass
+
+    return result
+
+
+
+if __name__ == '__main__':
+    domain = 'freebuf.com'
+    print(whois(domain))
+    ips = ['8.8.8.8','114.114.114.114']
+    print(ipbatch(ips))
+    domains = ['baidu.com','freebuf.com']
     print(icp(domains))
```

### Comparing `sh2d-0.9/mylib/chromedriver_help.py` & `sh2d-1.1/mylib/chromedriver_help.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import os
-import requests
-import winreg
-import zipfile
-
-
-def get_chrome_version():
-    '''获取本地chrome版本'''
-    key = winreg.OpenKey(winreg.HKEY_CURRENT_USER,
-                         r'Software\Google\Chrome\BLBeacon')
-    version, types = winreg.QueryValueEx(key, 'version')
-    return version
-
-
-def get_server_chrome_versions():
-    '''获取chrome版本列表'''
-    versionList = []
-    url = "https://registry.npmmirror.com/-/binary/chromedriver/"
-    rep = requests.get(url).json()
-    for item in rep:
-        versionList.append(item["name"])
-    return versionList
-
-
-def download_driver(download_url):
-    '''下载chromedriver.zip文件'''
-    file = requests.get(download_url)
-    with open("chromedriver.zip", 'wb') as zip_file:  # 保存文件到脚本所在目录
-        zip_file.write(file.content)
-        print("[+] chromedriver下载成功")
-
-
-def get_version(file_path):
-    '''查询当前Chromedriver版本'''
-    outstd2 = os.popen(os.path.join(
-        file_path, "chromedriver.exe") + '  --version').read()
-    return outstd2.split(' ')[1]
-
-
-def unzip_driver(path):
-    '''解压Chromedriver压缩包到指定目录'''
-    f = zipfile.ZipFile("chromedriver.zip", 'r')
-    for file in f.namelist():
-        f.extract(file, path)
-
-
-def update_chromedriver(file_path):
-    '''检查并更新chromedriver版本'''
-    url = 'http://npm.taobao.org/mirrors/chromedriver/'
-    chromeVersion = get_chrome_version()
-    chrome_main_version = int(chromeVersion.split(".")[0])  # chrome主版本号
-    driver_main_version = ''
-    if os.path.exists(os.path.join(file_path, "chromedriver.exe")):
-        driverVersion = get_version(file_path)
-        driver_main_version = int(driverVersion.split(".")[
-                                  0])  # chromedriver主版本号
-    download_url = ""
-    if driver_main_version != chrome_main_version:
-        print("[+] chromedriver版本与chrome浏览器不兼容,更新中>>>")
-        versionList = get_server_chrome_versions()
-        if chromeVersion in versionList:
-            download_url = "{}{}/chromedriver_win32.zip".format(url,chromeVersion)
-        else:
-            for version in versionList:
-                if version.startswith(str(chrome_main_version)):
-                    download_url = "{}{}/chromedriver_win32.zip".format(url,version)
-                    break
-            if download_url == "":
-                print(
-                    "[-] 未找到兼容的chromedriver版本,请在http://npm.taobao.org/mirrors/chromedriver/ 核实。")
-
-        download_driver(download_url=download_url)
-        path = file_path
-        unzip_driver(path)
-        os.remove("chromedriver.zip")
-        print('[+] 更新后的Chromedriver版本为:', get_version(file_path))
-    else:
-        print("[+] chromedriver版本兼容,无需更新！")
-    return os.path.join(file_path, "chromedriver.exe")
-
-
-if __name__ == "__main__":
-    file_path = "D:\\Temp"
-    print(update_chromedriver(file_path))
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import os
+import requests
+import winreg
+import zipfile
+
+
+def get_chrome_version():
+    '''获取本地chrome版本'''
+    key = winreg.OpenKey(winreg.HKEY_CURRENT_USER,
+                         r'Software\Google\Chrome\BLBeacon')
+    version, types = winreg.QueryValueEx(key, 'version')
+    return version
+
+
+def get_server_chrome_versions():
+    '''获取chrome版本列表'''
+    versionList = []
+    url = "https://registry.npmmirror.com/-/binary/chromedriver/"
+    rep = requests.get(url).json()
+    for item in rep:
+        versionList.append(item["name"])
+    return versionList
+
+
+def download_driver(download_url):
+    '''下载chromedriver.zip文件'''
+    file = requests.get(download_url)
+    with open("chromedriver.zip", 'wb') as zip_file:  # 保存文件到脚本所在目录
+        zip_file.write(file.content)
+        print("[+] chromedriver下载成功")
+
+
+def get_version(file_path):
+    '''查询当前Chromedriver版本'''
+    outstd2 = os.popen(os.path.join(
+        file_path, "chromedriver.exe") + '  --version').read()
+    return outstd2.split(' ')[1]
+
+
+def unzip_driver(path):
+    '''解压Chromedriver压缩包到指定目录'''
+    f = zipfile.ZipFile("chromedriver.zip", 'r')
+    for file in f.namelist():
+        f.extract(file, path)
+
+
+def update_chromedriver(file_path):
+    '''检查并更新chromedriver版本'''
+    url = 'http://npm.taobao.org/mirrors/chromedriver/'
+    chromeVersion = get_chrome_version()
+    chrome_main_version = int(chromeVersion.split(".")[0])  # chrome主版本号
+    driver_main_version = ''
+    if os.path.exists(os.path.join(file_path, "chromedriver.exe")):
+        driverVersion = get_version(file_path)
+        driver_main_version = int(driverVersion.split(".")[
+                                  0])  # chromedriver主版本号
+    download_url = ""
+    if driver_main_version != chrome_main_version:
+        print("[+] chromedriver版本与chrome浏览器不兼容,更新中>>>")
+        versionList = get_server_chrome_versions()
+        if chromeVersion in versionList:
+            download_url = "{}{}/chromedriver_win32.zip".format(url,chromeVersion)
+        else:
+            for version in versionList:
+                if version.startswith(str(chrome_main_version)):
+                    download_url = "{}{}/chromedriver_win32.zip".format(url,version)
+                    break
+            if download_url == "":
+                print(
+                    "[-] 未找到兼容的chromedriver版本,请在http://npm.taobao.org/mirrors/chromedriver/ 核实。")
+
+        download_driver(download_url=download_url)
+        path = file_path
+        unzip_driver(path)
+        os.remove("chromedriver.zip")
+        print('[+] 更新后的Chromedriver版本为:', get_version(file_path))
+    else:
+        print("[+] chromedriver版本兼容,无需更新！")
+    return os.path.join(file_path, "chromedriver.exe")
+
+
+if __name__ == "__main__":
+    file_path = "D:\\Temp"
+    print(update_chromedriver(file_path))
```

### Comparing `sh2d-0.9/mylib/common_help.py` & `sh2d-1.1/mylib/common_help.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-from itertools import groupby
-
-
-def mask2num(mask):
-    """
-    掩码转数字
-    :param mask: 255.255.255.255
-    :return 32
-    """
-    def count_bit(bin_str): return len([i for i in bin_str if i == '1'])
-    mask_splited = mask.split('.')
-    mask_count = [count_bit(bin(int(i))) for i in mask_splited]
-    return sum(mask_count)
-
-
-def num2mask(mask_int):
-    """
-    数字转掩码
-    :param mask_int: 32
-    :return 255.255.255.255
-    """
-    bin_arr = ['0' for i in range(32)]
-    for i in range(mask_int):
-        bin_arr[i] = '1'
-    tmpmask = [''.join(bin_arr[i * 8:i * 8 + 8]) for i in range(4)]
-    tmpmask = [str(int(tmpstr, 2)) for tmpstr in tmpmask]
-    return '.'.join(tmpmask)
-
-
-def num2numnum(numlist):
-    """
-    根据数字列表生成数字范围列表
-    :param numlist: [1,2,18,3,5,6,7,8,13,12,11,10]
-    :return [[1,3],[5,8],[10,13]]
-    """
-    numlist.sort()
-    numnumlist = []
-    def fun(x): return x[1] - x[0]
-    for k, g in groupby(enumerate(numlist), fun):
-        _ = [v for i, v in g]
-        if len(_) == 1:
-            numnumlist.append([_[0], _[0]])
-        else:
-            numnumlist.append([_[0], _[-1]])
-    return numnumlist
-
-
-def list_split(lst, x):
-    """
-    按指定长度拆分列表
-    :param lst: [1,2,3]
-    :param x: 1
-    :return [[1],[2],[3]]
-    """
-    return [lst[i:i+x] for i in range(0, len(lst), x)]
-
-def list_cmp(lst_1, lst_2):
-    """
-    对比两个列表 减少 遗留 新增
-    :param lst_1: [1,2,3]
-    :param lst_2: [3,4,5]
-    :return [[1,2],[3],[4,5]]
-    """
-    return [_ for _ in lst_1 if _ not in lst_2], [_ for _ in lst_1 if _ in lst_2], [_ for _ in lst_2 if _ not in lst_1]
-
-
-def dict_group(dic, lst):
-    """
-    将列表中的字典按1个或多个标题分组
-    :param dic: [{"a":"a","b":"b"},{"a":"c","b":"d"}]
-    :param lst: ["a","b"]
-    :return {'a_b':[{"a":"a","b":"b"},{"a":"c","b":"d"}]}
-    """
-    gdic = {}
-    for item in dic:
-        key = '_'.join([str(item.get(line, 'None')) for line in lst])
-        gdic.setdefault(key, [])
-        gdic[key].append(item)
-    return gdic
-
-
-def dict_cmp(dic_1, dic_2, lst):
-    """
-    对比两个列表中字典 减少 遗留 新增
-    :param dic_1: [{"a":"a","b":"b"},{"a":"c","b":"d"}]
-    :param dic_2: [{"a":"c","b":"d"},{"a":"e","b":"f"}]
-    :param lst: ["a","b"]
-    :return [[{"a":"a","b":"b"}],[{"a":"c","b":"d"}],[{"a":"e","b":"f"}]]
-    """
-    ndic_1 = dict_group(dic_1, lst)
-    ndic_2 = dict_group(dic_2, lst)
-    lst_a, lst_b, lst_c = list_cmp(list(ndic_1.keys()), list(ndic_2.keys()))
-    return [_ for k in lst_a for _ in ndic_1[k]], [_ for k in lst_b for _ in ndic_2[k]], [_ for k in lst_c for _ in ndic_2[k]]
-
-def idn2xn(domain):
-    """
-    中文域名转英文
-    :param domain: xxx.com
-    :return 英文域名
-    """
-    try:
-        return str(domain.encode('idna'), encoding='UTF-8')
-    except:
-        return 
-
-def xn2idn(domain):
-    """
-    英文域名转中文
-    :param domain: xxx.com
-    :return 中文域名
-    """
-    try:
-        return bytes(domain, encoding='UTF-8').decode('idna')
-    except:
-        return 
-
-if __name__ == '__main__':
-    pass
-
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+from itertools import groupby
+
+
+def mask2num(mask):
+    """
+    掩码转数字
+    :param mask: 255.255.255.255
+    :return 32
+    """
+    def count_bit(bin_str): return len([i for i in bin_str if i == '1'])
+    mask_splited = mask.split('.')
+    mask_count = [count_bit(bin(int(i))) for i in mask_splited]
+    return sum(mask_count)
+
+
+def num2mask(mask_int):
+    """
+    数字转掩码
+    :param mask_int: 32
+    :return 255.255.255.255
+    """
+    bin_arr = ['0' for i in range(32)]
+    for i in range(mask_int):
+        bin_arr[i] = '1'
+    tmpmask = [''.join(bin_arr[i * 8:i * 8 + 8]) for i in range(4)]
+    tmpmask = [str(int(tmpstr, 2)) for tmpstr in tmpmask]
+    return '.'.join(tmpmask)
+
+
+def num2numnum(numlist):
+    """
+    根据数字列表生成数字范围列表
+    :param numlist: [1,2,18,3,5,6,7,8,13,12,11,10]
+    :return [[1,3],[5,8],[10,13]]
+    """
+    numlist.sort()
+    numnumlist = []
+    def fun(x): return x[1] - x[0]
+    for k, g in groupby(enumerate(numlist), fun):
+        _ = [v for i, v in g]
+        if len(_) == 1:
+            numnumlist.append([_[0], _[0]])
+        else:
+            numnumlist.append([_[0], _[-1]])
+    return numnumlist
+
+
+def list_split(lst, x):
+    """
+    按指定长度拆分列表
+    :param lst: [1,2,3]
+    :param x: 1
+    :return [[1],[2],[3]]
+    """
+    return [lst[i:i+x] for i in range(0, len(lst), x)]
+
+def list_cmp(lst_1, lst_2):
+    """
+    对比两个列表 减少 遗留 新增
+    :param lst_1: [1,2,3]
+    :param lst_2: [3,4,5]
+    :return [[1,2],[3],[4,5]]
+    """
+    return [_ for _ in lst_1 if _ not in lst_2], [_ for _ in lst_1 if _ in lst_2], [_ for _ in lst_2 if _ not in lst_1]
+
+
+def dict_group(dic, lst):
+    """
+    将列表中的字典按1个或多个标题分组
+    :param dic: [{"a":"a","b":"b"},{"a":"c","b":"d"}]
+    :param lst: ["a","b"]
+    :return {'a_b':[{"a":"a","b":"b"},{"a":"c","b":"d"}]}
+    """
+    gdic = {}
+    for item in dic:
+        key = '_'.join([str(item.get(line, 'None')) for line in lst])
+        gdic.setdefault(key, [])
+        gdic[key].append(item)
+    return gdic
+
+
+def dict_cmp(dic_1, dic_2, lst):
+    """
+    对比两个列表中字典 减少 遗留 新增
+    :param dic_1: [{"a":"a","b":"b"},{"a":"c","b":"d"}]
+    :param dic_2: [{"a":"c","b":"d"},{"a":"e","b":"f"}]
+    :param lst: ["a","b"]
+    :return [[{"a":"a","b":"b"}],[{"a":"c","b":"d"}],[{"a":"e","b":"f"}]]
+    """
+    ndic_1 = dict_group(dic_1, lst)
+    ndic_2 = dict_group(dic_2, lst)
+    lst_a, lst_b, lst_c = list_cmp(list(ndic_1.keys()), list(ndic_2.keys()))
+    return [_ for k in lst_a for _ in ndic_1[k]], [_ for k in lst_b for _ in ndic_2[k]], [_ for k in lst_c for _ in ndic_2[k]]
+
+def idn2xn(domain):
+    """
+    中文域名转英文
+    :param domain: xxx.com
+    :return 英文域名
+    """
+    try:
+        return str(domain.encode('idna'), encoding='UTF-8')
+    except:
+        return 
+
+def xn2idn(domain):
+    """
+    英文域名转中文
+    :param domain: xxx.com
+    :return 中文域名
+    """
+    try:
+        return bytes(domain, encoding='UTF-8').decode('idna')
+    except:
+        return 
+
+if __name__ == '__main__':
+    pass
+
```

### Comparing `sh2d-0.9/mylib/des_help.py` & `sh2d-1.1/mylib/des_help.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from Crypto.Util.Padding import pad
-from Crypto.Cipher import DES
-import binascii
-
-
-class DES_ECB:
-
-    def __init__(self, key):
-
-        key = key.encode('utf8')
-        key = key[:8] if len(key) >= 8 else key + (8-len(key))*b'\0'
-        self.cipher = DES.new(key, DES.MODE_ECB)
-
-    def encrypt(self, text):
-        ct = self.cipher.encrypt(pad(text.encode('utf8'), 8))
-        return binascii.b2a_base64(ct).decode('utf8').strip()
-
-    def decrypt(self, text):
-        text = binascii.a2b_base64(text)
-        ct = self.cipher.decrypt(text)
-        return ct.decode('utf8').strip()
+from Crypto.Util.Padding import pad
+from Crypto.Cipher import DES
+import binascii
+
+
+class DES_ECB:
+
+    def __init__(self, key):
+
+        key = key.encode('utf8')
+        key = key[:8] if len(key) >= 8 else key + (8-len(key))*b'\0'
+        self.cipher = DES.new(key, DES.MODE_ECB)
+
+    def encrypt(self, text):
+        ct = self.cipher.encrypt(pad(text.encode('utf8'), 8))
+        return binascii.b2a_base64(ct).decode('utf8').strip()
+
+    def decrypt(self, text):
+        text = binascii.a2b_base64(text)
+        ct = self.cipher.decrypt(text)
+        return ct.decode('utf8').strip()
```

### Comparing `sh2d-0.9/mylib/dingtalk_help.py` & `sh2d-1.1/mylib/dingtalk_help.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,83 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import time
-import hmac
-import hashlib
-import base64
-import urllib.parse
-import requests
-
-
-def _sign(secret):
-    timestamp = str(round(time.time() * 1000))
-    hmac_code = hmac.new(secret.encode('utf-8'), '{}\n{}'.format(timestamp,
-                         secret).encode('utf-8'), digestmod=hashlib.sha256).digest()
-    sign = urllib.parse.quote_plus(base64.b64encode(hmac_code))
-    return timestamp, sign
-
-
-def send_text(text, token, secret="", atMobiles=[], isAtAll=False):
-    """
-    发送消息到钉钉群
-    :param text: 发送的文本消息
-    :param token: 钉钉群机器人token
-    :param secret: 钉钉群机器人secret,为关键字或IP限制时可为空
-    :param atMobiles: 要at的人的手机号列表
-    :param isAtAll: 是否@全部人 默认False
-    """
-    headers = {
-        'Content-Type': 'application/json'
-    }
-    data = {
-        "msgtype": "text",
-        "text": {
-            "content": text
-        },
-        "at": {
-            "atMobiles": atMobiles,
-            "isAtAll": isAtAll},
-    }
-    if secret:
-        timestamp, sign = _sign(secret)
-        url = "https://oapi.dingtalk.com/robot/send?access_token={}&timestamp={}&sign={}".format(
-            token, timestamp, sign)
-    else:
-        url = "https://oapi.dingtalk.com/robot/send?access_token={}".format(
-            token)
-    r = requests.post(url, json=data, headers=headers)
-    return r.json()
-
-
-def send_markdown(title, text, token, secret="", atMobiles=[], isAtAll=False):
-    """
-    发送消息到钉钉群
-    :param title: 发送的markdown标题
-    :param text: 发送的markdown内容
-    :param token: 钉钉群机器人token
-    :param secret: 钉钉群机器人secret,为关键字或IP限制时可为空
-    :param atMobiles: 要at的人的手机号列表
-    :param isAtAll: 是否@全部人 默认False
-    """
-    headers = {
-        'Content-Type': 'application/json'
-    }
-    data = {
-        "msgtype": "markdown",
-        "markdown": {
-            "title": title,
-            "text": text
-        },
-        "at": {
-            "atMobiles": atMobiles,
-            "isAtAll": isAtAll},
-    }
-    if secret:
-        timestamp, sign = _sign(secret)
-        url = "https://oapi.dingtalk.com/robot/send?access_token={}&timestamp={}&sign={}".format(
-            token, timestamp, sign)
-    else:
-        url = "https://oapi.dingtalk.com/robot/send?access_token={}".format(
-            token)
-    r = requests.post(url, json=data, headers=headers)
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import time
+import hmac
+import hashlib
+import base64
+import urllib.parse
+import requests
+
+
+def _sign(secret):
+    timestamp = str(round(time.time() * 1000))
+    hmac_code = hmac.new(secret.encode('utf-8'), '{}\n{}'.format(timestamp,
+                         secret).encode('utf-8'), digestmod=hashlib.sha256).digest()
+    sign = urllib.parse.quote_plus(base64.b64encode(hmac_code))
+    return timestamp, sign
+
+
+def send_text(text, token, secret="", atMobiles=[], isAtAll=False):
+    """
+    发送消息到钉钉群
+    :param text: 发送的文本消息
+    :param token: 钉钉群机器人token
+    :param secret: 钉钉群机器人secret,为关键字或IP限制时可为空
+    :param atMobiles: 要at的人的手机号列表
+    :param isAtAll: 是否@全部人 默认False
+    """
+    headers = {
+        'Content-Type': 'application/json'
+    }
+    data = {
+        "msgtype": "text",
+        "text": {
+            "content": text
+        },
+        "at": {
+            "atMobiles": atMobiles,
+            "isAtAll": isAtAll},
+    }
+    if secret:
+        timestamp, sign = _sign(secret)
+        url = "https://oapi.dingtalk.com/robot/send?access_token={}&timestamp={}&sign={}".format(
+            token, timestamp, sign)
+    else:
+        url = "https://oapi.dingtalk.com/robot/send?access_token={}".format(
+            token)
+    r = requests.post(url, json=data, headers=headers)
+    return r.json()
+
+
+def send_markdown(title, text, token, secret="", atMobiles=[], isAtAll=False):
+    """
+    发送消息到钉钉群
+    :param title: 发送的markdown标题
+    :param text: 发送的markdown内容
+    :param token: 钉钉群机器人token
+    :param secret: 钉钉群机器人secret,为关键字或IP限制时可为空
+    :param atMobiles: 要at的人的手机号列表
+    :param isAtAll: 是否@全部人 默认False
+    """
+    headers = {
+        'Content-Type': 'application/json'
+    }
+    data = {
+        "msgtype": "markdown",
+        "markdown": {
+            "title": title,
+            "text": text
+        },
+        "at": {
+            "atMobiles": atMobiles,
+            "isAtAll": isAtAll},
+    }
+    if secret:
+        timestamp, sign = _sign(secret)
+        url = "https://oapi.dingtalk.com/robot/send?access_token={}&timestamp={}&sign={}".format(
+            token, timestamp, sign)
+    else:
+        url = "https://oapi.dingtalk.com/robot/send?access_token={}".format(
+            token)
+    r = requests.post(url, json=data, headers=headers)
     return r.json()
```

### Comparing `sh2d-0.9/mylib/dnspython_help.py` & `sh2d-1.1/mylib/dnspython_help.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import dns.resolver
-
-
-def domain2ip(domain, dns_server=None):
-    """
-    解析域名到IP
-    :param domian: 域名
-    :param dns_server: DNS服务器
-    :return [] ip列表
-    """
-    resolver = dns.resolver.Resolver()
-
-    if dns_server is not None:
-        resolver.nameservers = [dns_server]
-    try:
-        answer = resolver.resolve(domain, 'A')
-        return [str(ip) for ip in answer]
-    except:
-        return []
-
-
-def domain2cname(domain,dns_server=None):
-    """
-    查询CNAME
-    :param domian: 域名
-    :param dns_server: DNS服务器
-    :return [] CNAME列表
-    """
-    resolver = dns.resolver.Resolver()
-
-    if dns_server is not None:
-        resolver.nameservers = [dns_server]
-    try:
-        answer = resolver.query(domain, 'CNAME')
-        return [str(_.target).strip(".").lower() for _ in answer]
-    except:
-        return []
-
-if __name__ == '__main__':
-    domain = 'www.baidu.com'
-    print(domain,domain2ip(domain),domain2cname(domain))
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import dns.resolver
+
+
+def domain2ip(domain, dns_server=None):
+    """
+    解析域名到IP
+    :param domian: 域名
+    :param dns_server: DNS服务器
+    :return [] ip列表
+    """
+    resolver = dns.resolver.Resolver()
+
+    if dns_server is not None:
+        resolver.nameservers = [dns_server]
+    try:
+        answer = resolver.resolve(domain, 'A')
+        return [str(ip) for ip in answer]
+    except:
+        return []
+
+
+def domain2cname(domain,dns_server=None):
+    """
+    查询CNAME
+    :param domian: 域名
+    :param dns_server: DNS服务器
+    :return [] CNAME列表
+    """
+    resolver = dns.resolver.Resolver()
+
+    if dns_server is not None:
+        resolver.nameservers = [dns_server]
+    try:
+        answer = resolver.query(domain, 'CNAME')
+        return [str(_.target).strip(".").lower() for _ in answer]
+    except:
+        return []
+
+if __name__ == '__main__':
+    domain = 'www.baidu.com'
+    print(domain,domain2ip(domain),domain2cname(domain))
```

### Comparing `sh2d-0.9/mylib/fofa_help.py` & `sh2d-1.1/mylib/fofa_help.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-#!/usr/bin/env python
-# -*- coding:utf-8 -*-
-
-import base64
-import requests
-
-
-def api_search(email, key, query_str, fields, size, page=1):
-    url = 'https://fofa.info/api/v1/search/all'
-    params = {
-        'email': email,
-        'key': key,
-        'qbase64': base64.b64encode(query_str.encode('utf-8')).decode('utf-8'),
-        'size': size,
-        'fields': ",".join(fields),
-        'page': page
-    }
-    rj = requests.get(url, params=params).json()
-    status = rj.get('errmsg')
-    if status:
-        if '401 Unauthorized' in status:
-            print('api或邮箱不正确!')
-        return
-    print("查询参数：{},当前第{}页,结果数：{}".format(
-        query_str, page, len(rj.get('results'))))
-    return rj.get('results')
-
-
-def fofa(email, key, query_list, fields, size=100, max_page=100, check_url=True):
-    ''' 
-    fofa 批量api查询
-    :param email eg: xxxx@qq.com
-    :param key eg: asssssssssssssssss
-    :param query_list eg: ['app="tomcat"']
-    :param fields eg: ['host','title','ip','domain','port','protocol','city']
-    '''
-    result = []
-    for query_str in query_list:
-        for page in range(1, max_page+1):
-            try:
-                res = api_search(email, key, query_str,
-                                 fields, size=size, page=page)
-            except:
-                continue
-            if res:
-                for item in res:
-                    if len(fields) == 1:
-                        _ = {fields[0]: item}
-                    else:
-                        _ = dict(zip(fields, item))
-                    _.update({'query_str': query_str})
-                    if check_url:
-                        _.update({'url': _['host'] if 'http' in _[
-                                 'host'] else "http://"+_['host']})
-                    result.append(_)
-            else:
-                break
-    return result
+#!/usr/bin/env python
+# -*- coding:utf-8 -*-
+
+import base64
+import requests
+
+
+def api_search(email, key, query_str, fields, size, page=1):
+    url = 'https://fofa.info/api/v1/search/all'
+    params = {
+        'email': email,
+        'key': key,
+        'qbase64': base64.b64encode(query_str.encode('utf-8')).decode('utf-8'),
+        'size': size,
+        'fields': ",".join(fields),
+        'page': page
+    }
+    rj = requests.get(url, params=params).json()
+    status = rj.get('errmsg')
+    if status:
+        if '401 Unauthorized' in status:
+            print('api或邮箱不正确!')
+        return
+    print("查询参数：{},当前第{}页,结果数：{}".format(
+        query_str, page, len(rj.get('results'))))
+    return rj.get('results')
+
+
+def fofa(email, key, query_list, fields, size=100, max_page=100, check_url=True):
+    ''' 
+    fofa 批量api查询
+    :param email eg: xxxx@qq.com
+    :param key eg: asssssssssssssssss
+    :param query_list eg: ['app="tomcat"']
+    :param fields eg: ['host','title','ip','domain','port','protocol','city']
+    '''
+    result = []
+    for query_str in query_list:
+        for page in range(1, max_page+1):
+            try:
+                res = api_search(email, key, query_str,
+                                 fields, size=size, page=page)
+            except:
+                continue
+            if res:
+                for item in res:
+                    if len(fields) == 1:
+                        _ = {fields[0]: item}
+                    else:
+                        _ = dict(zip(fields, item))
+                    _.update({'query_str': query_str})
+                    if check_url:
+                        _.update({'url': _['host'] if 'http' in _[
+                                 'host'] else "http://"+_['host']})
+                    result.append(_)
+            else:
+                break
+    return result
```

### Comparing `sh2d-0.9/mylib/hashlib_help.py` & `sh2d-1.1/mylib/hashlib_help.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import hashlib
-
-
-def file2md5(_file):
-    ''''
-    获取文件md5
-    :param _file: 文件路径
-    '''
-    with open(_file, 'rb') as f:
-        md5obj = hashlib.md5()
-        md5obj.update(f.read())
-        return md5obj.hexdigest()
-
-
-def str2md5(_str, encoding='utf8'):
-    ''''
-    获取字符串md5
-    :param _str: 字符串
-    '''
-    return hashlib.md5(_str.encode(encoding)).hexdigest()
-
-
-def str2sha256(_str, encoding='utf8'):
-    ''''
-    获取字符串sha256
-    :param _str: 字符串
-    '''
-    return hashlib.sha256(_str.encode(encoding)).hexdigest()
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import hashlib
+
+
+def file2md5(_file):
+    ''''
+    获取文件md5
+    :param _file: 文件路径
+    '''
+    with open(_file, 'rb') as f:
+        md5obj = hashlib.md5()
+        md5obj.update(f.read())
+        return md5obj.hexdigest()
+
+
+def str2md5(_str, encoding='utf8'):
+    ''''
+    获取字符串md5
+    :param _str: 字符串
+    '''
+    return hashlib.md5(_str.encode(encoding)).hexdigest()
+
+
+def str2sha256(_str, encoding='utf8'):
+    ''''
+    获取字符串sha256
+    :param _str: 字符串
+    '''
+    return hashlib.sha256(_str.encode(encoding)).hexdigest()
```

### Comparing `sh2d-0.9/mylib/logging_help.py` & `sh2d-1.1/mylib/logging_help.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,58 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import os
-import sys
-import time
-import logging
-
-class Logger:
-    def __init__(self, set_level="INFO",
-                 name=os.path.split(os.path.splitext(sys.argv[0])[0])[-1],
-                 log_name=time.strftime("%Y-%m-%d.log", time.localtime()),
-                 log_path=os.path.join(os.getcwd(), "logs"),
-                 use_console=True):
-        """
-        :param set_level: 日志级别["NOTSET"|"DEBUG"|"INFO"|"WARNING"|"ERROR"|"CRITICAL"]，默认为INFO
-        :param name: 日志中打印的name，默认为运行程序的name
-        :param log_name: 日志文件的名字，默认为当前时间（年-月-日.log）
-        :param log_path: 日志文件夹的路径，默认为logger.py同级目录中的log文件夹
-        :param use_console: 是否在控制台打印，默认为True
-        """
-        if not set_level:
-            set_level = self._exec_type()  # 设置set_level为None，自动获取当前运行模式
-        self.__logger = logging.getLogger(name)
-        self.setLevel(getattr(logging, set_level.upper()) if hasattr(logging, set_level.upper()) else logging.INFO)  # 设置日志级别
-        if not os.path.exists(log_path):  # 创建日志目录
-            os.makedirs(log_path)
-        formatter = logging.Formatter("%(asctime)s - %(name)s - %(funcName)s - %(levelname)s - %(message)s")
-        if not self.logger.handlers:
-            handler_list = list()
-            handler_list.append(logging.FileHandler(os.path.join(log_path, log_name), encoding="utf-8"))
-            if use_console:
-                handler_list.append(logging.StreamHandler())
-            for handler in handler_list:
-                handler.setFormatter(formatter)
-                self.addHandler(handler)
- 
-    def __getattr__(self, item):
-        return getattr(self.logger, item)
- 
-    @property
-    def logger(self):
-        return self.__logger
- 
-    @logger.setter
-    def logger(self, func):
-        self.__logger = func
- 
-    def _exec_type(self):
-        return "DEBUG" if os.environ.get("IPYTHONENABLE") else "INFO"
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import os
+import logging
+import colorlog
+
+class Logger:
+    def __init__(self, set_level="INFO",name='main',log_file=''):
+        """
+        :param set_level: 日志级别["NOTSET"|"DEBUG"|"INFO"|"WARNING"|"ERROR"|"CRITICAL"]，默认为INFO
+        :param name: 日志中打印的name
+        :param log_file: 日志文件
+        """
+
+        self.__logger = logging.getLogger(name)
+        if not set_level:
+            set_level = self._exec_type()
+        self.setLevel(getattr(logging, set_level.upper()) if hasattr(logging, set_level.upper()) else logging.INFO)
+
+
+        if log_file:
+            file_handler = logging.FileHandler(log_file,'a',encoding='utf-8')
+            file_handler.setFormatter(logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(message)s"))
+            self.__logger.addHandler(file_handler)
+
+        console_handler = logging.StreamHandler()
+        console_handler.setFormatter(self._get_color_formatter())
+        self.__logger.addHandler(console_handler)
+
+    def _get_color_formatter(self):
+        color_formatter = colorlog.ColoredFormatter(
+            "%(log_color)s%(asctime)s - %(name)s - %(levelname)s - %(message)s",
+            log_colors={
+                "DEBUG": "green",
+                "INFO": "blue",
+                "WARNING": "yellow",
+                "ERROR": "red",
+                "CRITICAL": "red,bg_white",
+            },
+            reset=True
+        )
+        return color_formatter
+ 
+    def __getattr__(self, item):
+        return getattr(self.logger, item)
+ 
+    @property
+    def logger(self):
+        return self.__logger
+ 
+    @logger.setter
+    def logger(self, func):
+        self.__logger = func
+ 
+    def _exec_type(self):
+        return "DEBUG" if os.environ.get("IPYTHONENABLE") else "INFO"
+
```

### Comparing `sh2d-0.9/mylib/nessus_help.py` & `sh2d-1.1/mylib/nessus_help.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import json
-import requests
-import time
-requests.packages.urllib3.disable_warnings()
-
-
-class NessusClient:
-
-    def __init__(self, url, accessKey, secretKey):
-
-        self.url = url
-        self.headers = {'X-ApiKeys': 'accessKey={}; secretKey={};'.format(
-            accessKey, secretKey), 'Content-Type': 'application/json', }
-
-    def connect(self, method, resource, data=None):
-        if data:
-            data = json.dumps(data)
-        r = getattr(requests, method.lower())('{0}{1}'.format(
-            self.url, resource), data=data, headers=self.headers, verify=False)
-        if r.status_code != 200:
-            print(resource, data, r.text)
-        else:
-            try:
-                return r.json()
-            except:
-                return r.text
-
-    def get_policies(self):
-        '''获取所有策略模板'''
-        data = self.connect('GET', '/editor/policy/templates')
-        return dict((p['title'], p['uuid']) for p in data['templates'])
-
-    def add_scan(self, name, targets, pid):
-        '''创建任务'''
-        scan_data = {"uuid": pid, "settings": {
-            "discovery_mode": "Port scan (all ports)", 'name': name, "text_targets": targets, }}
-        data = self.connect('POST', '/scans', scan_data)
-        return data["scan"]
-
-    def launch(self, sid):
-        '''启动扫描'''
-        data = self.connect('POST', '/scans/{}/launch'.format(sid))
-        return data["scan_uuid"]
-
-    def get_scans(self):
-        '''当前任务'''
-        data = self.connect('GET', '/scans?folder_id=3')
-        return [[i['name'],i['status'],time.strftime("%Y-%m-%d %H:%M:%S",time.localtime(i['last_modification_date']))] for i in data['scans']]
-
-if __name__ == '__main__':
-    url = 'https://127.0.0.1:8834'
-    accessKey = '71cf45723e00ddad07c226ce31047d6e18d9db9d9b3d3ebe5d81db02bfc19bd7'
-    secretKey = '42035d11f2aea714b255d14a95dfe6f3cf76e79762abbe81921c67555d7815a7'
-
-    nessus = NessusClient(url, accessKey, secretKey)
-    # policies = nessus.get_policies()
-    # scan_data = nessus.add_scan("test", "192.168.1.1",
-    #                             policies['Basic Network Scan'])
-
-    # print(nessus.launch(scan_data['id']))
-    data = nessus.get_scans()
-    print(data)
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import json
+import requests
+import time
+requests.packages.urllib3.disable_warnings()
+
+
+class NessusClient:
+
+    def __init__(self, url, accessKey, secretKey):
+
+        self.url = url
+        self.headers = {'X-ApiKeys': 'accessKey={}; secretKey={};'.format(
+            accessKey, secretKey), 'Content-Type': 'application/json', }
+
+    def connect(self, method, resource, data=None):
+        if data:
+            data = json.dumps(data)
+        r = getattr(requests, method.lower())('{0}{1}'.format(
+            self.url, resource), data=data, headers=self.headers, verify=False)
+        if r.status_code != 200:
+            print(resource, data, r.text)
+        else:
+            try:
+                return r.json()
+            except:
+                return r.text
+
+    def get_policies(self):
+        '''获取所有策略模板'''
+        data = self.connect('GET', '/editor/policy/templates')
+        return dict((p['title'], p['uuid']) for p in data['templates'])
+
+    def add_scan(self, name, targets, pid):
+        '''创建任务'''
+        scan_data = {"uuid": pid, "settings": {
+            "discovery_mode": "Port scan (all ports)", 'name': name, "text_targets": targets, }}
+        data = self.connect('POST', '/scans', scan_data)
+        return data["scan"]
+
+    def launch(self, sid):
+        '''启动扫描'''
+        data = self.connect('POST', '/scans/{}/launch'.format(sid))
+        return data["scan_uuid"]
+
+    def get_scans(self):
+        '''当前任务'''
+        data = self.connect('GET', '/scans?folder_id=3')
+        return [[i['name'],i['status'],time.strftime("%Y-%m-%d %H:%M:%S",time.localtime(i['last_modification_date']))] for i in data['scans']]
+
+if __name__ == '__main__':
+    url = 'https://127.0.0.1:8834'
+    accessKey = '71cf45723e00ddad07c226ce31047d6e18d9db9d9b3d3ebe5d81db02bfc19bd7'
+    secretKey = '42035d11f2aea714b255d14a95dfe6f3cf76e79762abbe81921c67555d7815a7'
+
+    nessus = NessusClient(url, accessKey, secretKey)
+    # policies = nessus.get_policies()
+    # scan_data = nessus.add_scan("test", "192.168.1.1",
+    #                             policies['Basic Network Scan'])
+
+    # print(nessus.launch(scan_data['id']))
+    data = nessus.get_scans()
+    print(data)
```

### Comparing `sh2d-0.9/mylib/openpyxl_help.py` & `sh2d-1.1/mylib/openpyxl_help.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,144 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-from openpyxl import load_workbook, Workbook
-
-
-class modifyXlsx():
-
-    def __init__(self, excel_file_path):
-        """
-        :param excel_file_path: 已存在的excel路径
-        """
-        self.excel_file_path = excel_file_path
-        try:
-            self.wb = load_workbook(self.excel_file_path)
-        except Exception:
-            print("{} open error".format(self.excel_file_path))
-        self.ws = self.wb.active
-
-    def get_names(self):
-        return self.wb.get_sheet_names()
-
-    def use_sheet(self, name):
-        """
-        :param name: sheet名称
-        :return bool: 操作状态 True or  None
-        """
-        try:
-            self.ws = self.wb[name]
-            return True
-        except Exception as e:
-            print("{} change {} error {}".format(
-                self.excel_file_path, name, e))
-
-    def write_cell(self, name, row_no, col_no, content):
-        """
-        修改指定单元格内容
-        :param name: sheet名称
-        :param row_no: 行号 1开始
-        :param col_no: 列号 1开始
-        :param content: 更改后的值
-        :return bool: 操作状态 True or  None
-        """
-        if (not isinstance(row_no, int)) or (not isinstance(col_no, int)) or (not self.use_sheet(name)):
-            print("{}/{}/({},{})row_no or col_no not int".format(
-                self.excel_file_path, name, row_no, col_no))
-            return
-        try:
-            self.ws.cell(row=row_no, column=col_no).value = content
-            return True
-        except Exception as e:
-            print("{}/{}/({},{})/ write_cell {} error {}".format(self.excel_file_path,
-                  name, row_no, col_no, content, e))
-
-    def read_cell(self, name, row_no, col_no):
-        """
-        读取指定单元格内容
-        :param name: sheet名称
-        :param row_no: 行号 1开始
-        :param col_no: 列号 1开始
-        :return content: 单元格内容
-        """
-        if (not isinstance(row_no, int)) or (not isinstance(col_no, int)) or (not self.use_sheet(name)):
-            print(
-                "{self.excel_file_path}/{name}/({row_no},{col_no})row_no or col_no not int")
-            return
-        try:
-            return self.ws.cell(row=row_no, column=col_no).value
-        except Exception:
-            print(
-                "{}/{}/({},{})/ read_cell error".format(self.excel_file_path, name, row_no, col_no))
-
-    def write_row(self, name, row_no, row):
-        """
-        指定位置写入行数据
-        :param name: sheet名称
-        :param row_no: 第几行
-        :param row: 多行内容 [1,2,3]
-        """
-        if (not isinstance(row_no, int)) or (not self.use_sheet(name)):
-            print(
-                "{}/{}/({})row_no or col_no not int".format(self.excel_file_path, name, row_no))
-            return
-        try:
-            for i in range(len(row)):
-                self.ws.cell(row=row_no, column=i+1).value = row[i]
-            return True
-        except Exception as e:
-            print(
-                "{}/{}/({})/ write_cell {} error{}".format(self.excel_file_path, name, row_no, row, e))
-
-    def write_rows(self, name, rows, row_no=None):
-        """
-        追加写入多行数据
-        :param name: sheet名称
-        :param rows: 多行内容 [[1,2,3],[...]]
-        :param row_no: 起始行数
-        """
-        if not self.use_sheet(name):
-            return
-        try:
-            if row_no:
-                for index, row in enumerate(rows):
-                    self.write_row(name, row_no+index, row)
-            else:
-                for row in rows:
-                    self.ws.append(row)
-            return True
-        except Exception as e:
-            print("{}/{}/rows error {}".format(self.excel_file_path, name, e))
-
-    def get_rows(self, name):
-        """
-        获取sheet数据
-        :param name: sheet名称
-        :return rows: 多行内容 [[1,2,3],[...]]
-        """
-        if not self.use_sheet(name):
-            return
-        return [[cell.value for cell in row] for row in self.ws.iter_rows()]
-
-    def save(self, excel_file_path=None):
-        if excel_file_path:
-            self.wb.save(excel_file_path)
-        else:
-            self.wb.save(self.excel_file_path)
-
-
-def write_xlsx(excle_name, **tables):
-    wb = Workbook()
-    for name in tables.keys():
-        wb.create_sheet(title=name)
-    for name in wb.sheetnames:
-        if name not in list(tables.keys()):
-            wb.remove(wb[name])
-
-    for name, rows in tables.items():
-        if not rows:
-            continue
-        for row in rows:
-            wb[name].append(row)
-    wb.save(excle_name)
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+from openpyxl import load_workbook, Workbook
+
+
+class modifyXlsx():
+
+    def __init__(self, excel_file_path):
+        """
+        :param excel_file_path: 已存在的excel路径
+        """
+        self.excel_file_path = excel_file_path
+        try:
+            self.wb = load_workbook(self.excel_file_path)
+        except Exception:
+            print("{} open error".format(self.excel_file_path))
+        self.ws = self.wb.active
+
+    def get_names(self):
+        return self.wb.get_sheet_names()
+
+    def use_sheet(self, name):
+        """
+        :param name: sheet名称
+        :return bool: 操作状态 True or  None
+        """
+        try:
+            self.ws = self.wb[name]
+            return True
+        except Exception as e:
+            print("{} change {} error {}".format(
+                self.excel_file_path, name, e))
+
+    def write_cell(self, name, row_no, col_no, content):
+        """
+        修改指定单元格内容
+        :param name: sheet名称
+        :param row_no: 行号 1开始
+        :param col_no: 列号 1开始
+        :param content: 更改后的值
+        :return bool: 操作状态 True or  None
+        """
+        if (not isinstance(row_no, int)) or (not isinstance(col_no, int)) or (not self.use_sheet(name)):
+            print("{}/{}/({},{})row_no or col_no not int".format(
+                self.excel_file_path, name, row_no, col_no))
+            return
+        try:
+            self.ws.cell(row=row_no, column=col_no).value = content
+            return True
+        except Exception as e:
+            print("{}/{}/({},{})/ write_cell {} error {}".format(self.excel_file_path,
+                  name, row_no, col_no, content, e))
+
+    def read_cell(self, name, row_no, col_no):
+        """
+        读取指定单元格内容
+        :param name: sheet名称
+        :param row_no: 行号 1开始
+        :param col_no: 列号 1开始
+        :return content: 单元格内容
+        """
+        if (not isinstance(row_no, int)) or (not isinstance(col_no, int)) or (not self.use_sheet(name)):
+            print(
+                "{self.excel_file_path}/{name}/({row_no},{col_no})row_no or col_no not int")
+            return
+        try:
+            return self.ws.cell(row=row_no, column=col_no).value
+        except Exception:
+            print(
+                "{}/{}/({},{})/ read_cell error".format(self.excel_file_path, name, row_no, col_no))
+
+    def write_row(self, name, row_no, row):
+        """
+        指定位置写入行数据
+        :param name: sheet名称
+        :param row_no: 第几行
+        :param row: 多行内容 [1,2,3]
+        """
+        if (not isinstance(row_no, int)) or (not self.use_sheet(name)):
+            print(
+                "{}/{}/({})row_no or col_no not int".format(self.excel_file_path, name, row_no))
+            return
+        try:
+            for i in range(len(row)):
+                self.ws.cell(row=row_no, column=i+1).value = row[i]
+            return True
+        except Exception as e:
+            print(
+                "{}/{}/({})/ write_cell {} error{}".format(self.excel_file_path, name, row_no, row, e))
+
+    def write_rows(self, name, rows, row_no=None):
+        """
+        追加写入多行数据
+        :param name: sheet名称
+        :param rows: 多行内容 [[1,2,3],[...]]
+        :param row_no: 起始行数
+        """
+        if not self.use_sheet(name):
+            return
+        try:
+            if row_no:
+                for index, row in enumerate(rows):
+                    self.write_row(name, row_no+index, row)
+            else:
+                for row in rows:
+                    self.ws.append(row)
+            return True
+        except Exception as e:
+            print("{}/{}/rows error {}".format(self.excel_file_path, name, e))
+
+    def get_rows(self, name):
+        """
+        获取sheet数据
+        :param name: sheet名称
+        :return rows: 多行内容 [[1,2,3],[...]]
+        """
+        if not self.use_sheet(name):
+            return
+        return [[cell.value for cell in row] for row in self.ws.iter_rows()]
+
+    def save(self, excel_file_path=None):
+        if excel_file_path:
+            self.wb.save(excel_file_path)
+        else:
+            self.wb.save(self.excel_file_path)
+
+
+def write_xlsx(excle_name, **tables):
+    wb = Workbook()
+    for name in tables.keys():
+        wb.create_sheet(title=name)
+    for name in wb.sheetnames:
+        if name not in list(tables.keys()):
+            wb.remove(wb[name])
+
+    for name, rows in tables.items():
+        if not rows:
+            continue
+        for row in rows:
+            wb[name].append(row)
+    wb.save(excle_name)
+
+
```

### Comparing `sh2d-0.9/mylib/re_help.py` & `sh2d-1.1/mylib/re_help.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,115 +1,123 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import re
-
-
-def is_ipv4(addr):
-    ''' 
-    判断是否是IPv4
-    :param addr eg: 127.0.0.1
-    :return True or False
-    '''
-    ipv4_regex = (
-        r'^(1\d{2}|2[0-4]\d|25[0-5]|[1-9]\d|[1-9])\.(1\d{2}'
-        r'|2[0-4]\d|25[0-5]|[1-9]\d|\d)\.(1\d{2}|2[0-4]\d'
-        r'|25[0-5]|[1-9]\d|\d)\.(1\d{2}|2[0-4]\d|25[0-5]|[1-9]\d|\d)$'
-    )
-    return bool(re.match(ipv4_regex, addr))
-
-
-def is_ipv6(addr):
-    ''' 
-    判断是否是IPv6
-    :param addr eg:
-    :return True or False
-    '''
-    ipv6_regex = (
-        r'(^(?:[A-F0-9]{1,4}:){7}[A-F0-9]{1,4}$)|'
-        r'(\A([0-9a-f]{1,4}:){1,1}(:[0-9a-f]{1,4}){1,6}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,2}(:[0-9a-f]{1,4}){1,5}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,3}(:[0-9a-f]{1,4}){1,4}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,4}(:[0-9a-f]{1,4}){1,3}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,5}(:[0-9a-f]{1,4}){1,2}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,6}(:[0-9a-f]{1,4}){1,1}\Z)|'
-        r'(\A(([0-9a-f]{1,4}:){1,7}|:):\Z)|(\A:(:[0-9a-f]{1,4}){1,7}\Z)|'
-        r'(\A((([0-9a-f]{1,4}:){6})(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3})\Z)|'
-        r'(\A(([0-9a-f]{1,4}:){5}[0-9a-f]{1,4}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3})\Z)|'
-        r'(\A([0-9a-f]{1,4}:){5}:[0-9a-f]{1,4}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,1}(:[0-9a-f]{1,4}){1,4}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,2}(:[0-9a-f]{1,4}){1,3}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,3}(:[0-9a-f]{1,4}){1,2}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
-        r'(\A([0-9a-f]{1,4}:){1,4}(:[0-9a-f]{1,4}){1,1}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
-        r'(\A(([0-9a-f]{1,4}:){1,5}|:):(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
-        r'(\A:(:[0-9a-f]{1,4}){1,5}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)')
-    return bool(re.match(ipv6_regex, addr))
-
-
-def is_domain(addr):
-    ''' 
-    判断是否是域名
-    :param addr eg: baidu.com
-    :return True or False
-    '''
-    domain_regex = (
-        r'^(([a-zA-Z]{1})|([a-zA-Z]{1}[a-zA-Z]{1})|'
-        r'([a-zA-Z]{1}[0-9]{1})|([0-9]{1}[a-zA-Z]{1})|'
-        r'([a-zA-Z0-9][-_.a-zA-Z0-9]{0,61}[a-zA-Z0-9]))\.'
-        r'([a-zA-Z]{2,13}|[a-zA-Z0-9-]{2,30}.[a-zA-Z]{2,3})$'
-    )
-    return bool(re.match(domain_regex, addr))
-
-
-def get_ipv4(text):
-    ''' 
-    提取IPv4
-    :param text 
-    :return []
-    '''
-    ipv4_regex = r'\b(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\b'
-    return re.findall(ipv4_regex, text)
-
-
-def get_ipv6(text):
-    ''' 
-    提取IPv6
-    :param value eg: 
-    :return []
-    '''
-    ipv6_regex = r'\b([0-9a-z]*:{1,4}){1,7}[0-9a-z]{1,4}\b'
-    return re.findall(ipv6_regex, text)
-
-
-def get_domain(text):
-    '''
-    提取domain
-    :param text 
-    :return []
-    '''
-    domain_regex = r"[0-9a-zA-Z-]+\.(?:[0-9a-zA-Z-]+\.)*[a-zA-Z]{2,6}"
-    return re.findall(domain_regex, text)
-
-def get_url(text):
-    '''
-    提取domain
-    :param text 
-    :return []
-    '''
-    url_regex = r"http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+"
-    return re.findall(url_regex, text)
-
-
-def rep_filename(text,dest=''):
-    ''' 
-    替换不能用于文件名的字符
-    :param text
-    '''
-    return re.sub(r'[\/\\\:\*\?\"\<\>\|]', dest, text)
-
-
-def rep_html(text,dest=''):
-    ''' 
-    替换html标签
-    :param text eg: 字符串
-    '''
-    return re.sub(r'<[^>]+>', dest, text)
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import re
+
+
+def is_ipv4(addr):
+    ''' 
+    判断是否是IPv4
+    :param addr eg: 127.0.0.1
+    :return True or False
+    '''
+    ipv4_regex = (
+        r'^(1\d{2}|2[0-4]\d|25[0-5]|[1-9]\d|[1-9])\.(1\d{2}'
+        r'|2[0-4]\d|25[0-5]|[1-9]\d|\d)\.(1\d{2}|2[0-4]\d'
+        r'|25[0-5]|[1-9]\d|\d)\.(1\d{2}|2[0-4]\d|25[0-5]|[1-9]\d|\d)$'
+    )
+    return bool(re.match(ipv4_regex, addr))
+
+
+def is_ipv6(addr):
+    ''' 
+    判断是否是IPv6
+    :param addr eg:
+    :return True or False
+    '''
+    ipv6_regex = (
+        r'(^(?:[A-F0-9]{1,4}:){7}[A-F0-9]{1,4}$)|'
+        r'(\A([0-9a-f]{1,4}:){1,1}(:[0-9a-f]{1,4}){1,6}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,2}(:[0-9a-f]{1,4}){1,5}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,3}(:[0-9a-f]{1,4}){1,4}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,4}(:[0-9a-f]{1,4}){1,3}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,5}(:[0-9a-f]{1,4}){1,2}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,6}(:[0-9a-f]{1,4}){1,1}\Z)|'
+        r'(\A(([0-9a-f]{1,4}:){1,7}|:):\Z)|(\A:(:[0-9a-f]{1,4}){1,7}\Z)|'
+        r'(\A((([0-9a-f]{1,4}:){6})(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3})\Z)|'
+        r'(\A(([0-9a-f]{1,4}:){5}[0-9a-f]{1,4}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3})\Z)|'
+        r'(\A([0-9a-f]{1,4}:){5}:[0-9a-f]{1,4}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,1}(:[0-9a-f]{1,4}){1,4}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,2}(:[0-9a-f]{1,4}){1,3}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,3}(:[0-9a-f]{1,4}){1,2}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
+        r'(\A([0-9a-f]{1,4}:){1,4}(:[0-9a-f]{1,4}){1,1}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
+        r'(\A(([0-9a-f]{1,4}:){1,5}|:):(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)|'
+        r'(\A:(:[0-9a-f]{1,4}){1,5}:(25[0-5]|2[0-4]\d|[0-1]?\d?\d)(\.(25[0-5]|2[0-4]\d|[0-1]?\d?\d)){3}\Z)')
+    return bool(re.match(ipv6_regex, addr))
+
+
+def is_domain(addr):
+    ''' 
+    判断是否是域名
+    :param addr eg: baidu.com
+    :return True or False
+    '''
+    domain_regex = (
+        r'^(([a-zA-Z]{1})|([a-zA-Z]{1}[a-zA-Z]{1})|'
+        r'([a-zA-Z]{1}[0-9]{1})|([0-9]{1}[a-zA-Z]{1})|'
+        r'([a-zA-Z0-9][-_.a-zA-Z0-9]{0,61}[a-zA-Z0-9]))\.'
+        r'([a-zA-Z]{2,13}|[a-zA-Z0-9-]{2,30}.[a-zA-Z]{2,3})$'
+    )
+    return bool(re.match(domain_regex, addr))
+
+
+def get_ipv4(text):
+    ''' 
+    提取IPv4
+    :param text 
+    :return []
+    '''
+    ipv4_regex = r'\b(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\b'
+    return re.findall(ipv4_regex, text)
+
+
+def get_ipv6(text):
+    ''' 
+    提取IPv6
+    :param value eg: 
+    :return []
+    '''
+    ipv6_regex = r'\b([0-9a-z]*:{1,4}){1,7}[0-9a-z]{1,4}\b'
+    return re.findall(ipv6_regex, text)
+
+def get_icp(text):
+    ''' 
+    提取ICP备案号
+    :param value eg: 
+    :return []
+    '''
+    icp_regex = r'([\u4e00-\u9fa5]ICP[备证]\d+?号(?:-\d{1,3})?)'
+    return re.findall(icp_regex, text)
+
+def get_domain(text):
+    '''
+    提取domain
+    :param text 
+    :return []
+    '''
+    domain_regex = r"[0-9a-zA-Z-]+\.(?:[0-9a-zA-Z-]+\.)*[a-zA-Z]{2,6}"
+    return re.findall(domain_regex, text)
+
+def get_url(text):
+    '''
+    提取domain
+    :param text 
+    :return []
+    '''
+    url_regex = r"http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+"
+    return re.findall(url_regex, text)
+
+
+def rep_filename(text,dest=''):
+    ''' 
+    替换不能用于文件名的字符
+    :param text
+    '''
+    return re.sub(r'[\/\\\:\*\?\"\<\>\|]', dest, text)
+
+
+def rep_html(text,dest=''):
+    ''' 
+    替换html标签
+    :param text eg: 字符串
+    '''
+    return re.sub(r'<[^>]+>', dest, text)
```

### Comparing `sh2d-0.9/mylib/weixin_help.py` & `sh2d-1.1/mylib/weixin_help.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-#!/usr/bin/env python3
-# -*- coding: UTF-8 -*-
-
-import time
-import random
-import requests
-
-
-class Weixin:
-
-    def __init__(self, token, cookie):
-        self.token = token
-        self.headers = {
-            "cookie": cookie,
-            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.0.0 Safari/537.36"
-        }
-
-    def get_fakid(self, name):
-        url = 'https://mp.weixin.qq.com/cgi-bin/searchbiz'
-        data = {
-            'action': 'search_biz',
-            'scene': 1,
-            'begin': 0,
-            'count': 10,
-            'query': name,
-            'token': self.token,
-            'lang': 'zh_CN',
-            'f': 'json',
-            'ajax': '1',
-        }
-        # 发送请求
-        rj = requests.get(url, headers=self.headers, params=data).json()
-        # 获取公众号名称、fakeid
-        wpub = {item['nickname']: item['fakeid'] for item in rj['list']}
-        return wpub.get(name)
-
-    def get_urls(self, fakeid, start_page=1, page_num=0):
-        url = 'https://mp.weixin.qq.com/cgi-bin/appmsg'
-        data = {
-            'action': 'list_ex',
-            'begin': start_page + page_num * 5, 
-            'count': '5',
-            'fakeid': fakeid,
-            'type': '9',
-            'query': '',
-            'token': self.token,
-            'lang': 'zh_CN',
-            'f': 'json',
-            'ajax': '1',
-        }
-        time.sleep(random.randint(1, 3))
-        rj = requests.get(url, headers=self.headers, params=data).json()
-        return [{'name':name,'update_time': time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(i['update_time'])), 'title':i['title'], 'link':i['link']} for i in rj['app_msg_list']]
-
-if __name__ == '__main__':
-    token = ''
-    cookie = ''
-    name = ''
-    fakeid = ''
-    wx = Weixin(token, cookie)
-    # fakeid = wx.get_fakid(name)
-    print(fakeid)
-    res = wx.get_urls(fakeid)
-    print(res)
+#!/usr/bin/env python3
+# -*- coding: UTF-8 -*-
+
+import time
+import random
+import requests
+
+
+class Weixin:
+
+    def __init__(self, token, cookie):
+        self.token = token
+        self.headers = {
+            "cookie": cookie,
+            "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/104.0.0.0 Safari/537.36"
+        }
+
+    def get_fakid(self, name):
+        url = 'https://mp.weixin.qq.com/cgi-bin/searchbiz'
+        data = {
+            'action': 'search_biz',
+            'scene': 1,
+            'begin': 0,
+            'count': 10,
+            'query': name,
+            'token': self.token,
+            'lang': 'zh_CN',
+            'f': 'json',
+            'ajax': '1',
+        }
+        # 发送请求
+        rj = requests.get(url, headers=self.headers, params=data).json()
+        # 获取公众号名称、fakeid
+        wpub = {item['nickname']: item['fakeid'] for item in rj['list']}
+        return wpub.get(name)
+
+    def get_urls(self, fakeid, start_page=1, page_num=0):
+        url = 'https://mp.weixin.qq.com/cgi-bin/appmsg'
+        data = {
+            'action': 'list_ex',
+            'begin': start_page + page_num * 5, 
+            'count': '5',
+            'fakeid': fakeid,
+            'type': '9',
+            'query': '',
+            'token': self.token,
+            'lang': 'zh_CN',
+            'f': 'json',
+            'ajax': '1',
+        }
+        time.sleep(random.randint(1, 3))
+        rj = requests.get(url, headers=self.headers, params=data).json()
+        return [{'name':name,'update_time': time.strftime("%Y-%m-%d %H:%M:%S", time.localtime(i['update_time'])), 'title':i['title'], 'link':i['link']} for i in rj['app_msg_list']]
+
+if __name__ == '__main__':
+    token = ''
+    cookie = ''
+    name = ''
+    fakeid = ''
+    wx = Weixin(token, cookie)
+    # fakeid = wx.get_fakid(name)
+    print(fakeid)
+    res = wx.get_urls(fakeid)
+    print(res)
```

### Comparing `sh2d-0.9/setup.py` & `sh2d-1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import setuptools
-
-setuptools.setup(
-    name="sh2d",
-    version="0.9",
-    author="sh2d",
-    author_email="xx@qq.com",
-    description="",
-    long_description='',
-    long_description_content_type="text/markdown",
-    url="https://github.com/",
-    packages=setuptools.find_packages(),
-    install_requires=['requests','dnspython','paramiko','pymysql','xlrd==1.2.0','xlsxwriter','zmail','xlwt','openpyxl','python-docx','docxtpl','pycryptodome','ddddocr','pyyaml'],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-)
+import setuptools
+
+setuptools.setup(
+    name="sh2d",
+    version="1.1",
+    author="sh2d",
+    author_email="xx@qq.com",
+    description="",
+    long_description='',
+    long_description_content_type="text/markdown",
+    url="https://github.com/",
+    packages=setuptools.find_packages(),
+    install_requires=['requests','dnspython','paramiko','pymysql','xlrd==1.2.0','xlsxwriter','zmail','xlwt','openpyxl','python-docx','docxtpl','pycryptodome','ddddocr','ruamel.yaml'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+)
```

### Comparing `sh2d-0.9/sh2d.egg-info/SOURCES.txt` & `sh2d-1.1/sh2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

