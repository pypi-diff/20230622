# Comparing `tmp/testvelikafkaclient-1.0.3.tar.gz` & `tmp/testvelikafkaclient-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testvelikafkaclient-1.0.3.tar", last modified: Thu Jun 22 09:32:45 2023, max compression
+gzip compressed data, was "testvelikafkaclient-1.0.4.tar", last modified: Thu Jun 22 09:34:29 2023, max compression
```

## Comparing `testvelikafkaclient-1.0.3.tar` & `testvelikafkaclient-1.0.4.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:32:45.842240 testvelikafkaclient-1.0.3/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1677 2023-06-22 09:32:45.842132 testvelikafkaclient-1.0.3/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-06-22 09:32:45.842270 testvelikafkaclient-1.0.3/setup.cfg
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      460 2023-06-22 09:31:56.000000 testvelikafkaclient-1.0.3/setup.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:32:45.841557 testvelikafkaclient-1.0.3/testvelikafkaclient/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       86 2023-06-22 09:25:47.000000 testvelikafkaclient-1.0.3/testvelikafkaclient/__init__.py
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       69 2023-06-22 09:32:38.000000 testvelikafkaclient-1.0.3/testvelikafkaclient/producer.py
-drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:32:45.841989 testvelikafkaclient-1.0.3/testvelikafkaclient.egg-info/
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1677 2023-06-22 09:32:45.000000 testvelikafkaclient-1.0.3/testvelikafkaclient.egg-info/PKG-INFO
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      244 2023-06-22 09:32:45.000000 testvelikafkaclient-1.0.3/testvelikafkaclient.egg-info/SOURCES.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-06-22 09:32:45.000000 testvelikafkaclient-1.0.3/testvelikafkaclient.egg-info/dependency_links.txt
--rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       20 2023-06-22 09:32:45.000000 testvelikafkaclient-1.0.3/testvelikafkaclient.egg-info/top_level.txt
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:34:29.642331 testvelikafkaclient-1.0.4/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       17 2023-06-22 09:34:15.000000 testvelikafkaclient-1.0.4/MANIFEST.in
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1677 2023-06-22 09:34:29.642227 testvelikafkaclient-1.0.4/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1477 2023-06-19 11:33:35.000000 testvelikafkaclient-1.0.4/readme.md
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       38 2023-06-22 09:34:29.642361 testvelikafkaclient-1.0.4/setup.cfg
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      460 2023-06-22 09:31:56.000000 testvelikafkaclient-1.0.4/setup.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:34:29.641485 testvelikafkaclient-1.0.4/testvelikafkaclient/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       86 2023-06-22 09:34:22.000000 testvelikafkaclient-1.0.4/testvelikafkaclient/__init__.py
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       69 2023-06-22 09:32:38.000000 testvelikafkaclient-1.0.4/testvelikafkaclient/producer.py
+drwxr-xr-x   0 konstantinedvalishvili   (501) staff       (20)        0 2023-06-22 09:34:29.642082 testvelikafkaclient-1.0.4/testvelikafkaclient.egg-info/
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)     1677 2023-06-22 09:34:29.000000 testvelikafkaclient-1.0.4/testvelikafkaclient.egg-info/PKG-INFO
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)      266 2023-06-22 09:34:29.000000 testvelikafkaclient-1.0.4/testvelikafkaclient.egg-info/SOURCES.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)        1 2023-06-22 09:34:29.000000 testvelikafkaclient-1.0.4/testvelikafkaclient.egg-info/dependency_links.txt
+-rw-r--r--   0 konstantinedvalishvili   (501) staff       (20)       20 2023-06-22 09:34:29.000000 testvelikafkaclient-1.0.4/testvelikafkaclient.egg-info/top_level.txt
```

### Comparing `testvelikafkaclient-1.0.3/PKG-INFO` & `testvelikafkaclient-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testvelikafkaclient
-Version: 1.0.3
+Version: 1.0.4
 Summary: veli kafka client <3 (demo)
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

### Comparing `testvelikafkaclient-1.0.3/testvelikafkaclient.egg-info/PKG-INFO` & `testvelikafkaclient-1.0.4/testvelikafkaclient.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testvelikafkaclient
-Version: 1.0.3
+Version: 1.0.4
 Summary: veli kafka client <3 (demo)
 Author: Konstantine
 Author-email: kdvalishvili@veli.store
 Description-Content-Type: text/markdown
 
 ### Kafka Client for VELI.STORE
```

