# Comparing `tmp/FlowAnalyzer-0.1.5.tar.gz` & `tmp/FlowAnalyzer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowAnalyzer-0.1.5.tar", last modified: Wed Jun 21 14:12:42 2023, max compression
+gzip compressed data, was "FlowAnalyzer-0.1.6.tar", last modified: Thu Jun 22 08:47:32 2023, max compression
```

## Comparing `FlowAnalyzer-0.1.5.tar` & `FlowAnalyzer-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 14:12:42.196545 FlowAnalyzer-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-06-21 14:12:42.193653 FlowAnalyzer-0.1.5/FlowAnalyzer/
--rw-rw-rw-   0        0        0     9264 2023-06-21 14:08:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer/FlowAnalyzer.py
--rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.5/FlowAnalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 14:12:42.195544 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/
--rw-rw-rw-   0        0        0     6271 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-21 14:12:42.000000 FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     6271 2023-06-21 14:12:42.196545 FlowAnalyzer-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-21 14:12:42.196545 FlowAnalyzer-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1144 2023-06-21 14:10:34.000000 FlowAnalyzer-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:47:32.187833 FlowAnalyzer-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-06-22 08:47:32.185771 FlowAnalyzer-0.1.6/FlowAnalyzer/
+-rw-rw-rw-   0        0        0     9282 2023-06-22 08:38:34.000000 FlowAnalyzer-0.1.6/FlowAnalyzer/FlowAnalyzer.py
+-rw-rw-rw-   0        0        0       70 2023-06-16 14:40:24.000000 FlowAnalyzer-0.1.6/FlowAnalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:47:32.186766 FlowAnalyzer-0.1.6/FlowAnalyzer.egg-info/
+-rw-rw-rw-   0        0        0     6271 2023-06-22 08:47:32.000000 FlowAnalyzer-0.1.6/FlowAnalyzer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2023-06-22 08:47:32.000000 FlowAnalyzer-0.1.6/FlowAnalyzer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:47:32.000000 FlowAnalyzer-0.1.6/FlowAnalyzer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-22 08:47:32.000000 FlowAnalyzer-0.1.6/FlowAnalyzer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1080 2023-06-17 13:51:39.000000 FlowAnalyzer-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     6271 2023-06-22 08:47:32.187833 FlowAnalyzer-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5236 2023-06-20 05:17:46.000000 FlowAnalyzer-0.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:47:32.188765 FlowAnalyzer-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1144 2023-06-22 08:40:19.000000 FlowAnalyzer-0.1.6/setup.py
```

### Comparing `FlowAnalyzer-0.1.5/FlowAnalyzer/FlowAnalyzer.py` & `FlowAnalyzer-0.1.6/FlowAnalyzer/FlowAnalyzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,17 +163,17 @@
             HTTP的bytes类型，如果有Gzip数据会自动解压缩
         """
         full_request = bytes.fromhex(full_request)
         num = full_request.find(b"\r\n\r\n")
         header = full_request[:num]
         
         if full_request.endswith(b"\r\n\r\n"):
-            ret = re.findall(b'^\r\n\r\n.*?\r\n(.*)\r\n.*?\r\n\r\n$', full_request[num:], flags=re.DOTALL)
             # 判断是否有file_data，没有的话就为b""空字符串
             # 由于是多个tcp所以需要去除应该是长度的字节 不确定是不是4个字节 后期可能出现bug
-            file_data = re.sub(b"\r\n.{4}\r\n", b"", ret[0]) if ret != [] else b""
+            ret = re.findall(b'^\r\n\r\n[0-9a-f]{1,}\r\n(.*)\r\n\x30\r\n\r\n$', full_request[num:], flags=re.DOTALL)
+            file_data = re.sub(b"\r\n[0-9a-f]{1,}\r\n", b"", ret[0]) if ret != [] else b""
         else:
             file_data = full_request[num+4:]
 
         with contextlib.suppress(Exception):
             file_data = gzip.decompress(file_data)
         return header + b"\r\n\r\n" + file_data if preserve_http_headers else file_data
```

### Comparing `FlowAnalyzer-0.1.5/FlowAnalyzer.egg-info/PKG-INFO` & `FlowAnalyzer-0.1.6/FlowAnalyzer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.5
+Version: 0.1.6
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.5/LICENSE` & `FlowAnalyzer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.5/PKG-INFO` & `FlowAnalyzer-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowAnalyzer
-Version: 0.1.5
+Version: 0.1.6
 Summary: FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件
 Home-page: https://github.com/Byxs20/FlowAnalyzer
 Author: Byxs20
 Author-email: 97766819@qq.com
 License: UNKNOWN
 Description: # FlowAnalyzer
```

### Comparing `FlowAnalyzer-0.1.5/README.md` & `FlowAnalyzer-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `FlowAnalyzer-0.1.5/setup.py` & `FlowAnalyzer-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="FlowAnalyzer",
-    version="0.1.5",
+    version="0.1.6",
     description="FlowAnalyzer是一个流量分析器，用于解析和处理tshark导出的JSON数据文件",
     author="Byxs20",
     author_email="97766819@qq.com",
     packages=find_packages(exclude=["tests", "*.egg-info"]),
     package_data={
         '': ['LICENSE', 'README.md', 'setup.py'],
     },
```

