# Comparing `tmp/micropython-captive-dns-server-0.0.3.dev0.tar.gz` & `tmp/micropython-captive-dns-server-0.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-captive-dns-server-0.0.3.dev0.tar", last modified: Thu Jun 22 07:31:01 2023, max compression
+gzip compressed data, was "micropython-captive-dns-server-0.0.4.dev0.tar", last modified: Thu Jun 22 11:38:22 2023, max compression
```

## Comparing `micropython-captive-dns-server-0.0.3.dev0.tar` & `micropython-captive-dns-server-0.0.4.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:38:22.420632 micropython-captive-dns-server-0.0.4.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 11:38:12.000000 micropython-captive-dns-server-0.0.4.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-22 11:38:22.420632 micropython-captive-dns-server-0.0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 11:38:12.000000 micropython-captive-dns-server-0.0.4.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:38:22.420632 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:38:12.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-22 11:38:12.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-06-22 11:38:12.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:38:22.420632 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-22 11:38:22.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 11:38:22.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:38:22.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:38:22.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 11:38:22.000000 micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-22 11:38:12.000000 micropython-captive-dns-server-0.0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-22 11:38:22.420632 micropython-captive-dns-server-0.0.4.dev0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-06-22 11:38:12.000000 micropython-captive-dns-server-0.0.4.dev0/setup.py
```

### Comparing `micropython-captive-dns-server-0.0.3.dev0/LICENSE` & `micropython-captive-dns-server-0.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-captive-dns-server-0.0.3.dev0/PKG-INFO` & `micropython-captive-dns-server-0.0.4.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-captive-dns-server
-Version: 0.0.3.dev0
+Version: 0.0.4.dev0
 Summary: Micropython asyncio simplistic dns server for use with captive portals
 Author-email: Patrick McAndrew <patrick@urg.name>
 Project-URL: Homepage, https://github.com/urg/micropython-captive-dns-server
 Project-URL: Repository, https://github.com/urg/micropython-captive-dns-server
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/packet.py` & `micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server/packet.py`

 * *Files identical despite different names*

### Comparing `micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/server.py` & `micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server/server.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import usocket as socket
 import uasyncio as asyncio
-from packet import DNSPacket
+from micropython_captive_dns_server.packet import DNSPacket
 import gc
 
 
 class CaptiveDNSServer:
     async def run(self, response_ip):
         try:
             udps = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
```

### Comparing `micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/PKG-INFO` & `micropython-captive-dns-server-0.0.4.dev0/micropython_captive_dns_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-captive-dns-server
-Version: 0.0.3.dev0
+Version: 0.0.4.dev0
 Summary: Micropython asyncio simplistic dns server for use with captive portals
 Author-email: Patrick McAndrew <patrick@urg.name>
 Project-URL: Homepage, https://github.com/urg/micropython-captive-dns-server
 Project-URL: Repository, https://github.com/urg/micropython-captive-dns-server
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `micropython-captive-dns-server-0.0.3.dev0/pyproject.toml` & `micropython-captive-dns-server-0.0.4.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micropython-captive-dns-server"
-version = "0.0.3.dev"
+version = "0.0.4.dev"
 description = "Micropython asyncio simplistic dns server for use with captive portals"
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: MicroPython",
     "License :: OSI Approved :: MIT License",
@@ -24,8 +24,8 @@
 
 [project.urls]
 Homepage = "https://github.com/urg/micropython-captive-dns-server"
 Repository = "https://github.com/urg/micropython-captive-dns-server"
 
 [tool.setuptools]
 package-dir = {"" = "."}
-packages = ["micropython_captive_dns_server"]
+packages = ["micropython_captive_dns_server"]
```

### Comparing `micropython-captive-dns-server-0.0.3.dev0/setup.cfg` & `micropython-captive-dns-server-0.0.4.dev0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = "micropython-captive-dns-server"
-version = "0.0.3.dev"
+version = "0.0.4.dev"
 description = "Micropython asyncio simplistic dns server for use with captive portals"
 classifiers = 
 	Environment :: Web Environment
 	Intended Audience :: Developers
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: Implementation :: MicroPython
 	License :: OSI Approved :: MIT License
```

