# Comparing `tmp/micropython-captive-dns-server-0.0.2.dev0.tar.gz` & `tmp/micropython-captive-dns-server-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropython-captive-dns-server-0.0.2.dev0.tar", last modified: Sun Jun 18 11:38:48 2023, max compression
+gzip compressed data, was "micropython-captive-dns-server-0.0.3.dev0.tar", last modified: Thu Jun 22 07:31:01 2023, max compression
```

## Comparing `micropython-captive-dns-server-0.0.2.dev0.tar` & `micropython-captive-dns-server-0.0.3.dev0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:38:48.755262 micropython-captive-dns-server-0.0.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-18 11:38:40.000000 micropython-captive-dns-server-0.0.2.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-18 11:38:48.755262 micropython-captive-dns-server-0.0.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-18 11:38:40.000000 micropython-captive-dns-server-0.0.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:38:48.755262 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 11:38:40.000000 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-18 11:38:40.000000 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server/packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-18 11:38:40.000000 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 11:38:48.755262 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-18 11:38:48.000000 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-18 11:38:48.000000 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 11:38:48.000000 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-18 11:38:48.000000 micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-18 11:38:40.000000 micropython-captive-dns-server-0.0.2.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 11:38:48.755262 micropython-captive-dns-server-0.0.2.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10576 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 07:31:01.000000 micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-22 07:31:01.477126 micropython-captive-dns-server-0.0.3.dev0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-06-22 07:30:53.000000 micropython-captive-dns-server-0.0.3.dev0/setup.py
```

### Comparing `micropython-captive-dns-server-0.0.2.dev0/LICENSE` & `micropython-captive-dns-server-0.0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropython-captive-dns-server-0.0.2.dev0/PKG-INFO` & `micropython-captive-dns-server-0.0.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-captive-dns-server
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Micropython asyncio simplistic dns server for use with captive portals
 Author-email: Patrick McAndrew <patrick@urg.name>
 Project-URL: Homepage, https://github.com/urg/micropython-captive-dns-server
 Project-URL: Repository, https://github.com/urg/micropython-captive-dns-server
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server/packet.py` & `micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/packet.py`

 * *Files identical despite different names*

### Comparing `micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server/server.py` & `micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server/server.py`

 * *Files identical despite different names*

### Comparing `micropython-captive-dns-server-0.0.2.dev0/micropython_captive_dns_server.egg-info/PKG-INFO` & `micropython-captive-dns-server-0.0.3.dev0/micropython_captive_dns_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropython-captive-dns-server
-Version: 0.0.2.dev0
+Version: 0.0.3.dev0
 Summary: Micropython asyncio simplistic dns server for use with captive portals
 Author-email: Patrick McAndrew <patrick@urg.name>
 Project-URL: Homepage, https://github.com/urg/micropython-captive-dns-server
 Project-URL: Repository, https://github.com/urg/micropython-captive-dns-server
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `micropython-captive-dns-server-0.0.2.dev0/pyproject.toml` & `micropython-captive-dns-server-0.0.3.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "micropython-captive-dns-server"
-version = "0.0.2.dev"
+version = "0.0.3.dev"
 description = "Micropython asyncio simplistic dns server for use with captive portals"
 classifiers = [
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: Implementation :: MicroPython",
     "License :: OSI Approved :: MIT License",
```

