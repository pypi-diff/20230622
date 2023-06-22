# Comparing `tmp/fastposter-1.4.3.tar.gz` & `tmp/fastposter-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastposter-1.4.3.tar", last modified: Wed Feb 22 16:30:14 2023, max compression
+gzip compressed data, was "fastposter-1.5.0.tar", last modified: Thu Jun 22 12:51:09 2023, max compression
```

## Comparing `fastposter-1.4.3.tar` & `fastposter-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-02-22 16:30:14.572099 fastposter-1.4.3/
--rw-r--r--   0 thomas     (501) staff       (20)     1071 2023-02-19 14:38:51.000000 fastposter-1.4.3/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)      565 2023-02-22 16:30:14.571627 fastposter-1.4.3/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      100 2023-02-08 15:51:24.000000 fastposter-1.4.3/README.md
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-02-22 16:30:14.569024 fastposter-1.4.3/fastposter/
--rw-r--r--   0 thomas     (501) staff       (20)      122 2023-02-19 14:19:36.000000 fastposter-1.4.3/fastposter/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      312 2023-02-22 16:30:08.000000 fastposter-1.4.3/fastposter/__version__.py
--rw-r--r--   0 thomas     (501) staff       (20)     7786 2023-02-22 16:29:50.000000 fastposter-1.4.3/fastposter/fastposter.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-02-22 16:30:14.571165 fastposter-1.4.3/fastposter.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)      565 2023-02-22 16:30:14.000000 fastposter-1.4.3/fastposter.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      269 2023-02-22 16:30:14.000000 fastposter-1.4.3/fastposter.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-02-22 16:30:14.000000 fastposter-1.4.3/fastposter.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       17 2023-02-22 16:30:14.000000 fastposter-1.4.3/fastposter.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)       11 2023-02-22 16:30:14.000000 fastposter-1.4.3/fastposter.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)       38 2023-02-22 16:30:14.572210 fastposter-1.4.3/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)      772 2023-02-22 16:30:02.000000 fastposter-1.4.3/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-22 12:51:09.549681 fastposter-1.5.0/
+-rw-r--r--   0 thomas     (501) staff       (20)     1071 2023-02-19 14:38:51.000000 fastposter-1.5.0/LICENSE
+-rw-r--r--   0 thomas     (501) staff       (20)      541 2023-06-22 12:51:09.549391 fastposter-1.5.0/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      100 2023-02-08 15:51:24.000000 fastposter-1.5.0/README.md
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-22 12:51:09.547210 fastposter-1.5.0/fastposter/
+-rw-r--r--   0 thomas     (501) staff       (20)      122 2023-02-19 14:19:36.000000 fastposter-1.5.0/fastposter/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      312 2023-06-22 12:38:17.000000 fastposter-1.5.0/fastposter/__version__.py
+-rw-r--r--   0 thomas     (501) staff       (20)     7806 2023-06-22 12:38:17.000000 fastposter-1.5.0/fastposter/fastposter.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-22 12:51:09.548953 fastposter-1.5.0/fastposter.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)      541 2023-06-22 12:51:09.000000 fastposter-1.5.0/fastposter.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      269 2023-06-22 12:51:09.000000 fastposter-1.5.0/fastposter.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-06-22 12:51:09.000000 fastposter-1.5.0/fastposter.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       17 2023-06-22 12:51:09.000000 fastposter-1.5.0/fastposter.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       11 2023-06-22 12:51:09.000000 fastposter-1.5.0/fastposter.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       38 2023-06-22 12:51:09.549794 fastposter-1.5.0/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)      772 2023-06-22 12:38:51.000000 fastposter-1.5.0/setup.py
```

### Comparing `fastposter-1.4.3/LICENSE` & `fastposter-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastposter-1.4.3/PKG-INFO` & `fastposter-1.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: fastposter
-Version: 1.4.3
+Version: 1.5.0
 Summary: A Python client for fastposter cloud
 Home-page: https://github.com/psoho/fastposter-client-python
 Author: Alex
 Author-email: service@fastposter.net
 License: MIT License (MIT)
 Project-URL: Documentation, https://cloud.fastposter.net/doc/guide/
 Project-URL: Source, https://github.com/psoho/fastposter-client-python
-Description: # fastposter 让海报开发更简单
-        
-        云服务开发文档 https://cloud.fastposter.net/doc/guide/
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# fastposter 让海报开发更简单
+
+云服务开发文档 https://cloud.fastposter.net/doc/guide/
```

### Comparing `fastposter-1.4.3/fastposter/fastposter.py` & `fastposter-1.5.0/fastposter/fastposter.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 client.buildPoster("ced9b1*****d494c", params=params, b64=True).b64String()
             """
             print(text)
             return
         return self.bytes.decode('utf-8')
 
 
+@DeprecationWarning
 class CloudClient:
     """
     海报云服务客户端
     """
 
     seq = 1
```

### Comparing `fastposter-1.4.3/fastposter.egg-info/PKG-INFO` & `fastposter-1.5.0/fastposter.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: fastposter
-Version: 1.4.3
+Version: 1.5.0
 Summary: A Python client for fastposter cloud
 Home-page: https://github.com/psoho/fastposter-client-python
 Author: Alex
 Author-email: service@fastposter.net
 License: MIT License (MIT)
 Project-URL: Documentation, https://cloud.fastposter.net/doc/guide/
 Project-URL: Source, https://github.com/psoho/fastposter-client-python
-Description: # fastposter 让海报开发更简单
-        
-        云服务开发文档 https://cloud.fastposter.net/doc/guide/
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# fastposter 让海报开发更简单
+
+云服务开发文档 https://cloud.fastposter.net/doc/guide/
```

### Comparing `fastposter-1.4.3/setup.py` & `fastposter-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fastposter',
-    version="1.4.3",
+    version="1.5.0",
     description='A Python client for fastposter cloud',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Alex',
     author_email='service@fastposter.net',
     license='MIT License (MIT)',
     url='https://github.com/psoho/fastposter-client-python',
```

