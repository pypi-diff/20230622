# Comparing `tmp/dvp-api-1.7.0.tar.gz` & `tmp/dvp-api-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvp-api-1.7.0.tar", last modified: Tue Sep 13 07:29:51 2022, max compression
+gzip compressed data, was "dvp-api-1.8.0.tar", last modified: Thu Jun 22 07:53:24 2023, max compression
```

## Comparing `dvp-api-1.7.0.tar` & `dvp-api-1.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:29:51.369068 dvp-api-1.7.0/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    11358 2022-09-13 07:27:21.000000 dvp-api-1.7.0/LICENSE
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      140 2022-09-13 07:27:21.000000 dvp-api-1.7.0/MANIFEST.in
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1532 2022-09-13 07:29:51.369342 dvp-api-1.7.0/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      862 2022-09-13 07:27:21.000000 dvp-api-1.7.0/README.md
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:29:51.347015 dvp-api-1.7.0/dvp-api/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:29:51.351008 dvp-api-1.7.0/dvp-api/dlpx/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      145 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:29:51.351614 dvp-api-1.7.0/dvp-api/dlpx/virtualization/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      145 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:29:51.359153 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        6 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/VERSION
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      243 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/__init__.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    33674 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/common_pb2.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    63370 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/libs_pb2.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     4921 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/libs_service_pb2.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    13181 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/libs_service_pb2_grpc.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)   205607 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/platform_pb2.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    18400 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/platform_service_pb2.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    56161 2022-09-13 07:27:21.000000 dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/platform_service_pb2_grpc.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:29:51.368655 dvp-api-1.7.0/dvp-api/dvp_api.egg-info/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1532 2022-09-13 07:29:51.000000 dvp-api-1.7.0/dvp-api/dvp_api.egg-info/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      755 2022-09-13 07:29:51.000000 dvp-api-1.7.0/dvp-api/dvp_api.egg-info/SOURCES.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        1 2022-09-13 07:29:51.000000 dvp-api-1.7.0/dvp-api/dvp_api.egg-info/dependency_links.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)       16 2022-09-13 07:29:51.000000 dvp-api-1.7.0/dvp-api/dvp_api.egg-info/requires.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        5 2022-09-13 07:29:51.000000 dvp-api-1.7.0/dvp-api/dvp_api.egg-info/top_level.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      594 2022-09-13 07:29:51.370667 dvp-api-1.7.0/setup.cfg
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      557 2022-09-13 07:27:21.000000 dvp-api-1.7.0/setup.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:53:24.240311 dvp-api-1.8.0/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    11358 2023-06-22 07:47:57.000000 dvp-api-1.8.0/LICENSE
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      140 2023-06-22 07:47:57.000000 dvp-api-1.8.0/MANIFEST.in
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1532 2023-06-22 07:53:24.240492 dvp-api-1.8.0/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      862 2023-06-22 07:47:57.000000 dvp-api-1.8.0/README.md
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:53:24.224308 dvp-api-1.8.0/dvp-api/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:53:24.227285 dvp-api-1.8.0/dvp-api/dlpx/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      145 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:53:24.227969 dvp-api-1.8.0/dvp-api/dlpx/virtualization/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      145 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:53:24.237024 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        6 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/VERSION
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      243 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/__init__.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    34231 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/common_pb2.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    63370 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/libs_pb2.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     4921 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/libs_service_pb2.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    13181 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/libs_service_pb2_grpc.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)   206234 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/platform_pb2.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    18400 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/platform_service_pb2.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    56161 2023-06-22 07:47:57.000000 dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/platform_service_pb2_grpc.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:53:24.239827 dvp-api-1.8.0/dvp-api/dvp_api.egg-info/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1532 2023-06-22 07:53:24.000000 dvp-api-1.8.0/dvp-api/dvp_api.egg-info/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      755 2023-06-22 07:53:24.000000 dvp-api-1.8.0/dvp-api/dvp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        1 2023-06-22 07:53:24.000000 dvp-api-1.8.0/dvp-api/dvp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)       16 2023-06-22 07:53:24.000000 dvp-api-1.8.0/dvp-api/dvp_api.egg-info/requires.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        5 2023-06-22 07:53:24.000000 dvp-api-1.8.0/dvp-api/dvp_api.egg-info/top_level.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      594 2023-06-22 07:53:24.241289 dvp-api-1.8.0/setup.cfg
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      557 2023-06-22 07:47:57.000000 dvp-api-1.8.0/setup.py
```

### Comparing `dvp-api-1.7.0/LICENSE` & `dvp-api-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/PKG-INFO` & `dvp-api-1.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvp-api
-Version: 1.7.0
+Version: 1.8.0
 Summary: Delphix Virtualization Platform API
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: # Delphix Virtualization Platform API
         
@@ -18,11 +18,11 @@
         The software is provided “as-is” without any warranties of any kind. To the maximum extent permitted by applicable law,
         Delphix Corp. and its affiliates disclaim any liability, implied warranties, including, without limitation, any implied
         warranties of merchantability, fitness for a particular purpose and non-infringement of intellectual property rights.
 Keywords: virtualization plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dvp-api-1.7.0/README.md` & `dvp-api-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/common_pb2.py` & `dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/common_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='dlpx/virtualization/api/common.proto',
   package='com.delphix.virtualization.common',
   syntax='proto3',
   serialized_options=_b('P\001'),
-  serialized_pb=_b('\n$dlpx/virtualization/api/common.proto\x12!com.delphix.virtualization.common\"\x9a\x01\n\x10RemoteConnection\x12I\n\x0b\x65nvironment\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.RemoteEnvironment\x12;\n\x04user\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.RemoteUser\"q\n\x11RemoteEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\x12;\n\x04host\x18\x03 \x01(\x0b\x32-.com.delphix.virtualization.common.RemoteHost\"X\n\nRemoteHost\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\x12\x13\n\x0b\x62inary_path\x18\x03 \x01(\t\x12\x14\n\x0cscratch_path\x18\x04 \x01(\t\"-\n\nRemoteUser\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\"h\n\x0cLinkedSource\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12J\n\nparameters\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"\x9f\x01\n\x0c\x44irectSource\x12G\n\nconnection\x18\x01 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12\x46\n\rlinked_source\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.LinkedSource\"\x8e\x01\n\x11SingleEntireMount\x12P\n\x12remote_environment\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.RemoteEnvironment\x12\x12\n\nmount_path\x18\x02 \x01(\t\x12\x13\n\x0bshared_path\x18\x03 \x01(\t\"\x8e\x01\n\x11SingleSubsetMount\x12P\n\x12remote_environment\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.RemoteEnvironment\x12\x12\n\nmount_path\x18\x02 \x01(\t\x12\x13\n\x0bshared_path\x18\x03 \x01(\t\"\xc2\x02\n\x0cStagedSource\x12\x46\n\rlinked_source\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.LinkedSource\x12N\n\x11source_connection\x18\x02 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12J\n\x0cstaged_mount\x18\x03 \x01(\x0b\x32\x34.com.delphix.virtualization.common.SingleEntireMount\x12N\n\x11staged_connection\x18\x04 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\"\xf8\x01\n\rVirtualSource\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12G\n\nconnection\x18\x02 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12\x44\n\x06mounts\x18\x03 \x03(\x0b\x32\x34.com.delphix.virtualization.common.SingleSubsetMount\x12J\n\nparameters\x18\x04 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"h\n\x0cSourceConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\nparameters\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"f\n\nRepository\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\nparameters\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"V\n\x08Snapshot\x12J\n\nparameters\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"`\n\x12SnapshotParameters\x12J\n\nparameters\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"#\n\x13PluginDefinedObject\x12\x0c\n\x04json\x18\x01 \x01(\t\")\n\rOwnershipSpec\x12\x0b\n\x03uid\x18\x01 \x01(\x05\x12\x0b\n\x03gid\x18\x02 \x01(\x05\x42\x02P\x01\x62\x06proto3')
+  serialized_pb=_b('\n$dlpx/virtualization/api/common.proto\x12!com.delphix.virtualization.common\"\x9a\x01\n\x10RemoteConnection\x12I\n\x0b\x65nvironment\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.RemoteEnvironment\x12;\n\x04user\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.RemoteUser\"q\n\x11RemoteEnvironment\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\x12;\n\x04host\x18\x03 \x01(\x0b\x32-.com.delphix.virtualization.common.RemoteHost\"X\n\nRemoteHost\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\x12\x13\n\x0b\x62inary_path\x18\x03 \x01(\t\x12\x14\n\x0cscratch_path\x18\x04 \x01(\t\"-\n\nRemoteUser\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\treference\x18\x02 \x01(\t\"h\n\x0cLinkedSource\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12J\n\nparameters\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"\x9f\x01\n\x0c\x44irectSource\x12G\n\nconnection\x18\x01 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12\x46\n\rlinked_source\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.LinkedSource\"\x8e\x01\n\x11SingleEntireMount\x12P\n\x12remote_environment\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.RemoteEnvironment\x12\x12\n\nmount_path\x18\x02 \x01(\t\x12\x13\n\x0bshared_path\x18\x03 \x01(\t\"\x8e\x01\n\x11SingleSubsetMount\x12P\n\x12remote_environment\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.RemoteEnvironment\x12\x12\n\nmount_path\x18\x02 \x01(\t\x12\x13\n\x0bshared_path\x18\x03 \x01(\t\"\x88\x03\n\x0cStagedSource\x12\x46\n\rlinked_source\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.LinkedSource\x12N\n\x11source_connection\x18\x02 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12J\n\x0cstaged_mount\x18\x03 \x01(\x0b\x32\x34.com.delphix.virtualization.common.SingleEntireMount\x12N\n\x11staged_connection\x18\x04 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12\x44\n\x06mounts\x18\x05 \x03(\x0b\x32\x34.com.delphix.virtualization.common.SingleSubsetMount\"\xf8\x01\n\rVirtualSource\x12\x0c\n\x04guid\x18\x01 \x01(\t\x12G\n\nconnection\x18\x02 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12\x44\n\x06mounts\x18\x03 \x03(\x0b\x32\x34.com.delphix.virtualization.common.SingleSubsetMount\x12J\n\nparameters\x18\x04 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"h\n\x0cSourceConfig\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\nparameters\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"f\n\nRepository\x12\x0c\n\x04name\x18\x01 \x01(\t\x12J\n\nparameters\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"V\n\x08Snapshot\x12J\n\nparameters\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"`\n\x12SnapshotParameters\x12J\n\nparameters\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.common.PluginDefinedObject\"#\n\x13PluginDefinedObject\x12\x0c\n\x04json\x18\x01 \x01(\t\")\n\rOwnershipSpec\x12\x0b\n\x03uid\x18\x01 \x01(\x05\x12\x0b\n\x03gid\x18\x02 \x01(\x05\x42\x02P\x01\x62\x06proto3')
 )
 
 
 
 
 _REMOTECONNECTION = _descriptor.Descriptor(
   name='RemoteConnection',
@@ -395,28 +395,35 @@
     _descriptor.FieldDescriptor(
       name='staged_connection', full_name='com.delphix.virtualization.common.StagedSource.staged_connection', index=3,
       number=4, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='mounts', full_name='com.delphix.virtualization.common.StagedSource.mounts', index=4,
+      number=5, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1043,
-  serialized_end=1365,
+  serialized_end=1435,
 )
 
 
 _VIRTUALSOURCE = _descriptor.Descriptor(
   name='VirtualSource',
   full_name='com.delphix.virtualization.common.VirtualSource',
   filename=None,
@@ -459,16 +466,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1368,
-  serialized_end=1616,
+  serialized_start=1438,
+  serialized_end=1686,
 )
 
 
 _SOURCECONFIG = _descriptor.Descriptor(
   name='SourceConfig',
   full_name='com.delphix.virtualization.common.SourceConfig',
   filename=None,
@@ -497,16 +504,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1618,
-  serialized_end=1722,
+  serialized_start=1688,
+  serialized_end=1792,
 )
 
 
 _REPOSITORY = _descriptor.Descriptor(
   name='Repository',
   full_name='com.delphix.virtualization.common.Repository',
   filename=None,
@@ -535,16 +542,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1724,
-  serialized_end=1826,
+  serialized_start=1794,
+  serialized_end=1896,
 )
 
 
 _SNAPSHOT = _descriptor.Descriptor(
   name='Snapshot',
   full_name='com.delphix.virtualization.common.Snapshot',
   filename=None,
@@ -566,16 +573,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1828,
-  serialized_end=1914,
+  serialized_start=1898,
+  serialized_end=1984,
 )
 
 
 _SNAPSHOTPARAMETERS = _descriptor.Descriptor(
   name='SnapshotParameters',
   full_name='com.delphix.virtualization.common.SnapshotParameters',
   filename=None,
@@ -597,16 +604,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1916,
-  serialized_end=2012,
+  serialized_start=1986,
+  serialized_end=2082,
 )
 
 
 _PLUGINDEFINEDOBJECT = _descriptor.Descriptor(
   name='PluginDefinedObject',
   full_name='com.delphix.virtualization.common.PluginDefinedObject',
   filename=None,
@@ -628,16 +635,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2014,
-  serialized_end=2049,
+  serialized_start=2084,
+  serialized_end=2119,
 )
 
 
 _OWNERSHIPSPEC = _descriptor.Descriptor(
   name='OwnershipSpec',
   full_name='com.delphix.virtualization.common.OwnershipSpec',
   filename=None,
@@ -666,30 +673,31 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2051,
-  serialized_end=2092,
+  serialized_start=2121,
+  serialized_end=2162,
 )
 
 _REMOTECONNECTION.fields_by_name['environment'].message_type = _REMOTEENVIRONMENT
 _REMOTECONNECTION.fields_by_name['user'].message_type = _REMOTEUSER
 _REMOTEENVIRONMENT.fields_by_name['host'].message_type = _REMOTEHOST
 _LINKEDSOURCE.fields_by_name['parameters'].message_type = _PLUGINDEFINEDOBJECT
 _DIRECTSOURCE.fields_by_name['connection'].message_type = _REMOTECONNECTION
 _DIRECTSOURCE.fields_by_name['linked_source'].message_type = _LINKEDSOURCE
 _SINGLEENTIREMOUNT.fields_by_name['remote_environment'].message_type = _REMOTEENVIRONMENT
 _SINGLESUBSETMOUNT.fields_by_name['remote_environment'].message_type = _REMOTEENVIRONMENT
 _STAGEDSOURCE.fields_by_name['linked_source'].message_type = _LINKEDSOURCE
 _STAGEDSOURCE.fields_by_name['source_connection'].message_type = _REMOTECONNECTION
 _STAGEDSOURCE.fields_by_name['staged_mount'].message_type = _SINGLEENTIREMOUNT
 _STAGEDSOURCE.fields_by_name['staged_connection'].message_type = _REMOTECONNECTION
+_STAGEDSOURCE.fields_by_name['mounts'].message_type = _SINGLESUBSETMOUNT
 _VIRTUALSOURCE.fields_by_name['connection'].message_type = _REMOTECONNECTION
 _VIRTUALSOURCE.fields_by_name['mounts'].message_type = _SINGLESUBSETMOUNT
 _VIRTUALSOURCE.fields_by_name['parameters'].message_type = _PLUGINDEFINEDOBJECT
 _SOURCECONFIG.fields_by_name['parameters'].message_type = _PLUGINDEFINEDOBJECT
 _REPOSITORY.fields_by_name['parameters'].message_type = _PLUGINDEFINEDOBJECT
 _SNAPSHOT.fields_by_name['parameters'].message_type = _PLUGINDEFINEDOBJECT
 _SNAPSHOTPARAMETERS.fields_by_name['parameters'].message_type = _PLUGINDEFINEDOBJECT
```

### Comparing `dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/libs_pb2.py` & `dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/libs_pb2.py`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/libs_service_pb2.py` & `dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/libs_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/libs_service_pb2_grpc.py` & `dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/libs_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/platform_pb2.py` & `dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/platform_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='dlpx/virtualization/api/platform.proto',
   package='com.delphix.virtualization.platform',
   syntax='proto3',
   serialized_options=_b('P\001'),
-  serialized_pb=_b('\n&dlpx/virtualization/api/platform.proto\x12#com.delphix.virtualization.platform\x1a$dlpx/virtualization/api/common.proto\"G\n\x12GenericPluginError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x12\n\ncall_stack\x18\x03 \x01(\t\"N\n\x15UnhandledLibraryError\x12\x10\n\x08\x65rror_id\x18\x01 \x01(\r\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\ncall_stack\x18\x03 \x01(\t\"9\n\x12PluginRuntimeError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\ncall_stack\x18\x02 \x01(\t\"<\n\x15GeneratedClassesError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\ncall_stack\x18\x02 \x01(\t\"<\n\tUserError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x0e\n\x06output\x18\x03 \x01(\t\"\xd2\x03\n\x11PluginErrorResult\x12W\n\x14generic_plugin_error\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.GenericPluginErrorH\x00\x12]\n\x17unhandled_library_error\x18\x02 \x01(\x0b\x32:.com.delphix.virtualization.platform.UnhandledLibraryErrorH\x00\x12W\n\x14plugin_runtime_error\x18\x03 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.PluginRuntimeErrorH\x00\x12]\n\x17generated_classes_error\x18\x04 \x01(\x0b\x32:.com.delphix.virtualization.platform.GeneratedClassesErrorH\x00\x12\x44\n\nuser_error\x18\x05 \x01(\x0b\x32..com.delphix.virtualization.platform.UserErrorH\x00\x42\x07\n\x05\x65rror\"l\n\x1aRepositoryDiscoveryRequest\x12N\n\x11source_connection\x18\x01 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\"`\n\x19RepositoryDiscoveryResult\x12\x43\n\x0crepositories\x18\x01 \x03(\x0b\x32-.com.delphix.virtualization.common.Repository\"\xc8\x01\n\x1bRepositoryDiscoveryResponse\x12V\n\x0creturn_value\x18\x01 \x01(\x0b\x32>.com.delphix.virtualization.platform.RepositoryDiscoveryResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xb1\x01\n\x1cSourceConfigDiscoveryRequest\x12N\n\x11source_connection\x18\x01 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12\x41\n\nrepository\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\"f\n\x1bSourceConfigDiscoveryResult\x12G\n\x0esource_configs\x18\x01 \x03(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xcc\x01\n\x1dSourceConfigDiscoveryResponse\x12X\n\x0creturn_value\x18\x01 \x01(\x0b\x32@.com.delphix.virtualization.platform.SourceConfigDiscoveryResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc1\x02\n\x18\x44irectPreSnapshotRequest\x12\x46\n\rdirect_source\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.DirectSource\x12\x41\n\nrepository\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"\x19\n\x17\x44irectPreSnapshotResult\"\xc4\x01\n\x19\x44irectPreSnapshotResponse\x12T\n\x0creturn_value\x18\x01 \x01(\x0b\x32<.com.delphix.virtualization.platform.DirectPreSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc2\x02\n\x19\x44irectPostSnapshotRequest\x12\x46\n\rdirect_source\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.DirectSource\x12\x41\n\nrepository\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"Y\n\x18\x44irectPostSnapshotResult\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\"\xc6\x01\n\x1a\x44irectPostSnapshotResponse\x12U\n\x0creturn_value\x18\x01 \x01(\x0b\x32=.com.delphix.virtualization.platform.DirectPostSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xec\x01\n\x17\x44irectSourceSizeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rdirect_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.DirectSource\"/\n\x16\x44irectSourceSizeResult\x12\x15\n\rdatabase_size\x18\x01 \x01(\x04\"\xc2\x01\n\x18\x44irectSourceSizeResponse\x12S\n\x0creturn_value\x18\x01 \x01(\x0b\x32;.com.delphix.virtualization.platform.DirectSourceSizeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc1\x02\n\x18StagedPreSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"\x19\n\x17StagedPreSnapshotResult\"\xc4\x01\n\x19StagedPreSnapshotResponse\x12T\n\x0creturn_value\x18\x01 \x01(\x0b\x32<.com.delphix.virtualization.platform.StagedPreSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc2\x02\n\x19StagedPostSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"Y\n\x18StagedPostSnapshotResult\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\"\xc6\x01\n\x1aStagedPostSnapshotResponse\x12U\n\x0creturn_value\x18\x01 \x01(\x0b\x32=.com.delphix.virtualization.platform.StagedPostSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe8\x01\n\x13StartStagingRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x14\n\x12StartStagingResult\"\xba\x01\n\x14StartStagingResponse\x12O\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.StartStagingResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe7\x01\n\x12StopStagingRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x13\n\x11StopStagingResult\"\xb8\x01\n\x13StopStagingResponse\x12N\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.StopStagingResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe8\x01\n\x13StagedStatusRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x88\x01\n\x12StagedStatusResult\x12N\n\x06status\x18\x01 \x01(\x0e\x32>.com.delphix.virtualization.platform.StagedStatusResult.Status\"\"\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"\xba\x01\n\x14StagedStatusResponse\x12O\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.StagedStatusResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe8\x01\n\x13StagedWorkerRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x14\n\x12StagedWorkerResult\"\xba\x01\n\x14StagedWorkerResponse\x12O\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.StagedWorkerResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa3\x01\n\x16StagedMountSpecRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rstaged_source\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\xad\x01\n\x15StagedMountSpecResult\x12J\n\x0cstaged_mount\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.SingleEntireMount\x12H\n\x0eownership_spec\x18\x02 \x01(\x0b\x32\x30.com.delphix.virtualization.common.OwnershipSpec\"\xc0\x01\n\x17StagedMountSpecResponse\x12R\n\x0creturn_value\x18\x01 \x01(\x0b\x32:.com.delphix.virtualization.platform.StagedMountSpecResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xec\x01\n\x17StagedSourceSizeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"/\n\x16StagedSourceSizeResult\x12\x15\n\rdatabase_size\x18\x01 \x01(\x04\"\xc2\x01\n\x18StagedSourceSizeResponse\x12S\n\x0creturn_value\x18\x01 \x01(\x0b\x32;.com.delphix.virtualization.platform.StagedSourceSizeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xde\x01\n\x10\x43onfigureRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12=\n\x08snapshot\x18\x02 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"Y\n\x0f\x43onfigureResult\x12\x46\n\rsource_config\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xb4\x01\n\x11\x43onfigureResponse\x12L\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.platform.ConfigureResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xfd\x01\n\x12UnconfigureRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\x12\x12\n\ndeleteFlag\x18\x04 \x01(\x08\"\x13\n\x11UnconfigureResult\"\xb8\x01\n\x13UnconfigureResponse\x12N\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.UnconfigureResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xec\x01\n\x15VirtualCleanupRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x16\n\x14VirtualCleanupResult\"\xbe\x01\n\x16VirtualCleanupResponse\x12Q\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x39.com.delphix.virtualization.platform.VirtualCleanupResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa8\x02\n\x12ReconfigureRequest\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\x12\x41\n\nrepository\x18\x04 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\"[\n\x11ReconfigureResult\x12\x46\n\rsource_config\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xb8\x01\n\x13ReconfigureResponse\x12N\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.ReconfigureResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe3\x01\n\x0cStartRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\r\n\x0bStartResult\"\xac\x01\n\rStartResponse\x12H\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x30.com.delphix.virtualization.platform.StartResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe2\x01\n\x0bStopRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x0c\n\nStopResult\"\xaa\x01\n\x0cStopResponse\x12G\n\x0creturn_value\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.platform.StopResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xf0\x01\n\x19VirtualPreSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x1a\n\x18VirtualPreSnapshotResult\"\xc6\x01\n\x1aVirtualPreSnapshotResponse\x12U\n\x0creturn_value\x18\x01 \x01(\x0b\x32=.com.delphix.virtualization.platform.VirtualPreSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xf1\x01\n\x1aVirtualPostSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"Z\n\x19VirtualPostSnapshotResult\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\"\xc8\x01\n\x1bVirtualPostSnapshotResponse\x12V\n\x0creturn_value\x18\x01 \x01(\x0b\x32>.com.delphix.virtualization.platform.VirtualPostSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xeb\x01\n\x14VirtualStatusRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x8a\x01\n\x13VirtualStatusResult\x12O\n\x06status\x18\x01 \x01(\x0e\x32?.com.delphix.virtualization.platform.VirtualStatusResult.Status\"\"\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"\xbc\x01\n\x15VirtualStatusResponse\x12P\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x38.com.delphix.virtualization.platform.VirtualStatusResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa6\x01\n\x11InitializeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSourceJ\x04\x08\x02\x10\x03\"Z\n\x10InitializeResult\x12\x46\n\rsource_config\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xb6\x01\n\x12InitializeResponse\x12M\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x35.com.delphix.virtualization.platform.InitializeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa6\x01\n\x17VirtualMountSpecRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12H\n\x0evirtual_source\x18\x02 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\xa8\x01\n\x16VirtualMountSpecResult\x12H\n\x0eownership_spec\x18\x01 \x01(\x0b\x32\x30.com.delphix.virtualization.common.OwnershipSpec\x12\x44\n\x06mounts\x18\x02 \x03(\x0b\x32\x34.com.delphix.virtualization.common.SingleSubsetMount\"\xc2\x01\n\x18VirtualMountSpecResponse\x12S\n\x0creturn_value\x18\x01 \x01(\x0b\x32;.com.delphix.virtualization.platform.VirtualMountSpecResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xef\x01\n\x18VirtualSourceSizeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"0\n\x17VirtualSourceSizeResult\x12\x15\n\rdatabase_size\x18\x01 \x01(\x04\"\xc4\x01\n\x19VirtualSourceSizeResponse\x12T\n\x0creturn_value\x18\x01 \x01(\x0b\x32<.com.delphix.virtualization.platform.VirtualSourceSizeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\x95\x03\n\x0eUpgradeRequest\x12m\n\x16pre_upgrade_parameters\x18\x01 \x03(\x0b\x32M.com.delphix.virtualization.platform.UpgradeRequest.PreUpgradeParametersEntry\x12\x46\n\x04type\x18\x02 \x01(\x0e\x32\x38.com.delphix.virtualization.platform.UpgradeRequest.Type\x12\x15\n\rmigration_ids\x18\x03 \x03(\t\x12\x1b\n\x13lua_upgrade_version\x18\x04 \x01(\t\x1a;\n\x19PreUpgradeParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"[\n\x04Type\x12\x10\n\x0cSOURCECONFIG\x10\x00\x12\x0e\n\nREPOSITORY\x10\x01\x12\x10\n\x0cLINKEDSOURCE\x10\x02\x12\x11\n\rVIRTUALSOURCE\x10\x03\x12\x0c\n\x08SNAPSHOT\x10\x04\"\xbd\x01\n\rUpgradeResult\x12n\n\x17post_upgrade_parameters\x18\x01 \x03(\x0b\x32M.com.delphix.virtualization.platform.UpgradeResult.PostUpgradeParametersEntry\x1a<\n\x1aPostUpgradeParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb0\x01\n\x0fUpgradeResponse\x12J\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x32.com.delphix.virtualization.platform.UpgradeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06resultB\x02P\x01\x62\x06proto3')
+  serialized_pb=_b('\n&dlpx/virtualization/api/platform.proto\x12#com.delphix.virtualization.platform\x1a$dlpx/virtualization/api/common.proto\"G\n\x12GenericPluginError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x12\n\ncall_stack\x18\x03 \x01(\t\"N\n\x15UnhandledLibraryError\x12\x10\n\x08\x65rror_id\x18\x01 \x01(\r\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x12\n\ncall_stack\x18\x03 \x01(\t\"9\n\x12PluginRuntimeError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\ncall_stack\x18\x02 \x01(\t\"<\n\x15GeneratedClassesError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x12\n\ncall_stack\x18\x02 \x01(\t\"<\n\tUserError\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x0e\n\x06output\x18\x03 \x01(\t\"\xd2\x03\n\x11PluginErrorResult\x12W\n\x14generic_plugin_error\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.GenericPluginErrorH\x00\x12]\n\x17unhandled_library_error\x18\x02 \x01(\x0b\x32:.com.delphix.virtualization.platform.UnhandledLibraryErrorH\x00\x12W\n\x14plugin_runtime_error\x18\x03 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.PluginRuntimeErrorH\x00\x12]\n\x17generated_classes_error\x18\x04 \x01(\x0b\x32:.com.delphix.virtualization.platform.GeneratedClassesErrorH\x00\x12\x44\n\nuser_error\x18\x05 \x01(\x0b\x32..com.delphix.virtualization.platform.UserErrorH\x00\x42\x07\n\x05\x65rror\"l\n\x1aRepositoryDiscoveryRequest\x12N\n\x11source_connection\x18\x01 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\"`\n\x19RepositoryDiscoveryResult\x12\x43\n\x0crepositories\x18\x01 \x03(\x0b\x32-.com.delphix.virtualization.common.Repository\"\xc8\x01\n\x1bRepositoryDiscoveryResponse\x12V\n\x0creturn_value\x18\x01 \x01(\x0b\x32>.com.delphix.virtualization.platform.RepositoryDiscoveryResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xb1\x01\n\x1cSourceConfigDiscoveryRequest\x12N\n\x11source_connection\x18\x01 \x01(\x0b\x32\x33.com.delphix.virtualization.common.RemoteConnection\x12\x41\n\nrepository\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\"f\n\x1bSourceConfigDiscoveryResult\x12G\n\x0esource_configs\x18\x01 \x03(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xcc\x01\n\x1dSourceConfigDiscoveryResponse\x12X\n\x0creturn_value\x18\x01 \x01(\x0b\x32@.com.delphix.virtualization.platform.SourceConfigDiscoveryResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc1\x02\n\x18\x44irectPreSnapshotRequest\x12\x46\n\rdirect_source\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.DirectSource\x12\x41\n\nrepository\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"\x19\n\x17\x44irectPreSnapshotResult\"\xc4\x01\n\x19\x44irectPreSnapshotResponse\x12T\n\x0creturn_value\x18\x01 \x01(\x0b\x32<.com.delphix.virtualization.platform.DirectPreSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc2\x02\n\x19\x44irectPostSnapshotRequest\x12\x46\n\rdirect_source\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.DirectSource\x12\x41\n\nrepository\x18\x02 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"Y\n\x18\x44irectPostSnapshotResult\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\"\xc6\x01\n\x1a\x44irectPostSnapshotResponse\x12U\n\x0creturn_value\x18\x01 \x01(\x0b\x32=.com.delphix.virtualization.platform.DirectPostSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xec\x01\n\x17\x44irectSourceSizeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rdirect_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.DirectSource\"/\n\x16\x44irectSourceSizeResult\x12\x15\n\rdatabase_size\x18\x01 \x01(\x04\"\xc2\x01\n\x18\x44irectSourceSizeResponse\x12S\n\x0creturn_value\x18\x01 \x01(\x0b\x32;.com.delphix.virtualization.platform.DirectSourceSizeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc1\x02\n\x18StagedPreSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"\x19\n\x17StagedPreSnapshotResult\"\xc4\x01\n\x19StagedPreSnapshotResponse\x12T\n\x0creturn_value\x18\x01 \x01(\x0b\x32<.com.delphix.virtualization.platform.StagedPreSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xc2\x02\n\x19StagedPostSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\x12R\n\x13snapshot_parameters\x18\x04 \x01(\x0b\x32\x35.com.delphix.virtualization.common.SnapshotParameters\"Y\n\x18StagedPostSnapshotResult\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\"\xc6\x01\n\x1aStagedPostSnapshotResponse\x12U\n\x0creturn_value\x18\x01 \x01(\x0b\x32=.com.delphix.virtualization.platform.StagedPostSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe8\x01\n\x13StartStagingRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x14\n\x12StartStagingResult\"\xba\x01\n\x14StartStagingResponse\x12O\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.StartStagingResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe7\x01\n\x12StopStagingRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x13\n\x11StopStagingResult\"\xb8\x01\n\x13StopStagingResponse\x12N\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.StopStagingResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe8\x01\n\x13StagedStatusRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x88\x01\n\x12StagedStatusResult\x12N\n\x06status\x18\x01 \x01(\x0e\x32>.com.delphix.virtualization.platform.StagedStatusResult.Status\"\"\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"\xba\x01\n\x14StagedStatusResponse\x12O\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.StagedStatusResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe8\x01\n\x13StagedWorkerRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\x14\n\x12StagedWorkerResult\"\xba\x01\n\x14StagedWorkerResponse\x12O\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x37.com.delphix.virtualization.platform.StagedWorkerResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa3\x01\n\x16StagedMountSpecRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rstaged_source\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"\xf3\x01\n\x15StagedMountSpecResult\x12J\n\x0cstaged_mount\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.common.SingleEntireMount\x12H\n\x0eownership_spec\x18\x02 \x01(\x0b\x32\x30.com.delphix.virtualization.common.OwnershipSpec\x12\x44\n\x06mounts\x18\x03 \x03(\x0b\x32\x34.com.delphix.virtualization.common.SingleSubsetMount\"\xc0\x01\n\x17StagedMountSpecResponse\x12R\n\x0creturn_value\x18\x01 \x01(\x0b\x32:.com.delphix.virtualization.platform.StagedMountSpecResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xec\x01\n\x17StagedSourceSizeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12\x46\n\rstaged_source\x18\x03 \x01(\x0b\x32/.com.delphix.virtualization.common.StagedSource\"/\n\x16StagedSourceSizeResult\x12\x15\n\rdatabase_size\x18\x01 \x01(\x04\"\xc2\x01\n\x18StagedSourceSizeResponse\x12S\n\x0creturn_value\x18\x01 \x01(\x0b\x32;.com.delphix.virtualization.platform.StagedSourceSizeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xde\x01\n\x10\x43onfigureRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12=\n\x08snapshot\x18\x02 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"Y\n\x0f\x43onfigureResult\x12\x46\n\rsource_config\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xb4\x01\n\x11\x43onfigureResponse\x12L\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x34.com.delphix.virtualization.platform.ConfigureResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xfd\x01\n\x12UnconfigureRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\x12\x12\n\ndeleteFlag\x18\x04 \x01(\x08\"\x13\n\x11UnconfigureResult\"\xb8\x01\n\x13UnconfigureResponse\x12N\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.UnconfigureResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xec\x01\n\x15VirtualCleanupRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x16\n\x14VirtualCleanupResult\"\xbe\x01\n\x16VirtualCleanupResponse\x12Q\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x39.com.delphix.virtualization.platform.VirtualCleanupResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa8\x02\n\x12ReconfigureRequest\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\x12\x41\n\nrepository\x18\x04 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\"[\n\x11ReconfigureResult\x12\x46\n\rsource_config\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xb8\x01\n\x13ReconfigureResponse\x12N\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.ReconfigureResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe3\x01\n\x0cStartRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\r\n\x0bStartResult\"\xac\x01\n\rStartResponse\x12H\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x30.com.delphix.virtualization.platform.StartResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xe2\x01\n\x0bStopRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x0c\n\nStopResult\"\xaa\x01\n\x0cStopResponse\x12G\n\x0creturn_value\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.platform.StopResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xf0\x01\n\x19VirtualPreSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x1a\n\x18VirtualPreSnapshotResult\"\xc6\x01\n\x1aVirtualPreSnapshotResponse\x12U\n\x0creturn_value\x18\x01 \x01(\x0b\x32=.com.delphix.virtualization.platform.VirtualPreSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xf1\x01\n\x1aVirtualPostSnapshotRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"Z\n\x19VirtualPostSnapshotResult\x12=\n\x08snapshot\x18\x01 \x01(\x0b\x32+.com.delphix.virtualization.common.Snapshot\"\xc8\x01\n\x1bVirtualPostSnapshotResponse\x12V\n\x0creturn_value\x18\x01 \x01(\x0b\x32>.com.delphix.virtualization.platform.VirtualPostSnapshotResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xeb\x01\n\x14VirtualStatusRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\x8a\x01\n\x13VirtualStatusResult\x12O\n\x06status\x18\x01 \x01(\x0e\x32?.com.delphix.virtualization.platform.VirtualStatusResult.Status\"\"\n\x06Status\x12\n\n\x06\x41\x43TIVE\x10\x00\x12\x0c\n\x08INACTIVE\x10\x01\"\xbc\x01\n\x15VirtualStatusResponse\x12P\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x38.com.delphix.virtualization.platform.VirtualStatusResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa6\x01\n\x11InitializeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSourceJ\x04\x08\x02\x10\x03\"Z\n\x10InitializeResult\x12\x46\n\rsource_config\x18\x01 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\"\xb6\x01\n\x12InitializeResponse\x12M\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x35.com.delphix.virtualization.platform.InitializeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xa6\x01\n\x17VirtualMountSpecRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12H\n\x0evirtual_source\x18\x02 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"\xa8\x01\n\x16VirtualMountSpecResult\x12H\n\x0eownership_spec\x18\x01 \x01(\x0b\x32\x30.com.delphix.virtualization.common.OwnershipSpec\x12\x44\n\x06mounts\x18\x02 \x03(\x0b\x32\x34.com.delphix.virtualization.common.SingleSubsetMount\"\xc2\x01\n\x18VirtualMountSpecResponse\x12S\n\x0creturn_value\x18\x01 \x01(\x0b\x32;.com.delphix.virtualization.platform.VirtualMountSpecResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\xef\x01\n\x18VirtualSourceSizeRequest\x12\x41\n\nrepository\x18\x01 \x01(\x0b\x32-.com.delphix.virtualization.common.Repository\x12\x46\n\rsource_config\x18\x02 \x01(\x0b\x32/.com.delphix.virtualization.common.SourceConfig\x12H\n\x0evirtual_source\x18\x03 \x01(\x0b\x32\x30.com.delphix.virtualization.common.VirtualSource\"0\n\x17VirtualSourceSizeResult\x12\x15\n\rdatabase_size\x18\x01 \x01(\x04\"\xc4\x01\n\x19VirtualSourceSizeResponse\x12T\n\x0creturn_value\x18\x01 \x01(\x0b\x32<.com.delphix.virtualization.platform.VirtualSourceSizeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06result\"\x95\x03\n\x0eUpgradeRequest\x12m\n\x16pre_upgrade_parameters\x18\x01 \x03(\x0b\x32M.com.delphix.virtualization.platform.UpgradeRequest.PreUpgradeParametersEntry\x12\x46\n\x04type\x18\x02 \x01(\x0e\x32\x38.com.delphix.virtualization.platform.UpgradeRequest.Type\x12\x15\n\rmigration_ids\x18\x03 \x03(\t\x12\x1b\n\x13lua_upgrade_version\x18\x04 \x01(\t\x1a;\n\x19PreUpgradeParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"[\n\x04Type\x12\x10\n\x0cSOURCECONFIG\x10\x00\x12\x0e\n\nREPOSITORY\x10\x01\x12\x10\n\x0cLINKEDSOURCE\x10\x02\x12\x11\n\rVIRTUALSOURCE\x10\x03\x12\x0c\n\x08SNAPSHOT\x10\x04\"\xbd\x01\n\rUpgradeResult\x12n\n\x17post_upgrade_parameters\x18\x01 \x03(\x0b\x32M.com.delphix.virtualization.platform.UpgradeResult.PostUpgradeParametersEntry\x1a<\n\x1aPostUpgradeParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xb0\x01\n\x0fUpgradeResponse\x12J\n\x0creturn_value\x18\x01 \x01(\x0b\x32\x32.com.delphix.virtualization.platform.UpgradeResultH\x00\x12G\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x36.com.delphix.virtualization.platform.PluginErrorResultH\x00\x42\x08\n\x06resultB\x02P\x01\x62\x06proto3')
   ,
   dependencies=[dlpx_dot_virtualization_dot_api_dot_common__pb2.DESCRIPTOR,])
 
 
 
 _STAGEDSTATUSRESULT_STATUS = _descriptor.EnumDescriptor(
   name='Status',
@@ -95,16 +95,16 @@
     _descriptor.EnumValueDescriptor(
       name='SNAPSHOT', index=4, number=4,
       serialized_options=None,
       type=None),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=13766,
-  serialized_end=13857,
+  serialized_start=13836,
+  serialized_end=13927,
 )
 _sym_db.RegisterEnumDescriptor(_UPGRADEREQUEST_TYPE)
 
 
 _GENERICPLUGINERROR = _descriptor.Descriptor(
   name='GenericPluginError',
   full_name='com.delphix.virtualization.platform.GenericPluginError',
@@ -1693,28 +1693,35 @@
     _descriptor.FieldDescriptor(
       name='ownership_spec', full_name='com.delphix.virtualization.platform.StagedMountSpecResult.ownership_spec', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR),
+    _descriptor.FieldDescriptor(
+      name='mounts', full_name='com.delphix.virtualization.platform.StagedMountSpecResult.mounts', index=2,
+      number=3, type=11, cpp_type=10, label=3,
+      has_default_value=False, default_value=[],
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=6707,
-  serialized_end=6880,
+  serialized_end=6950,
 )
 
 
 _STAGEDMOUNTSPECRESPONSE = _descriptor.Descriptor(
   name='StagedMountSpecResponse',
   full_name='com.delphix.virtualization.platform.StagedMountSpecResponse',
   filename=None,
@@ -1746,16 +1753,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.StagedMountSpecResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=6883,
-  serialized_end=7075,
+  serialized_start=6953,
+  serialized_end=7145,
 )
 
 
 _STAGEDSOURCESIZEREQUEST = _descriptor.Descriptor(
   name='StagedSourceSizeRequest',
   full_name='com.delphix.virtualization.platform.StagedSourceSizeRequest',
   filename=None,
@@ -1791,16 +1798,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7078,
-  serialized_end=7314,
+  serialized_start=7148,
+  serialized_end=7384,
 )
 
 
 _STAGEDSOURCESIZERESULT = _descriptor.Descriptor(
   name='StagedSourceSizeResult',
   full_name='com.delphix.virtualization.platform.StagedSourceSizeResult',
   filename=None,
@@ -1822,16 +1829,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7316,
-  serialized_end=7363,
+  serialized_start=7386,
+  serialized_end=7433,
 )
 
 
 _STAGEDSOURCESIZERESPONSE = _descriptor.Descriptor(
   name='StagedSourceSizeResponse',
   full_name='com.delphix.virtualization.platform.StagedSourceSizeResponse',
   filename=None,
@@ -1863,16 +1870,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.StagedSourceSizeResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=7366,
-  serialized_end=7560,
+  serialized_start=7436,
+  serialized_end=7630,
 )
 
 
 _CONFIGUREREQUEST = _descriptor.Descriptor(
   name='ConfigureRequest',
   full_name='com.delphix.virtualization.platform.ConfigureRequest',
   filename=None,
@@ -1908,16 +1915,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7563,
-  serialized_end=7785,
+  serialized_start=7633,
+  serialized_end=7855,
 )
 
 
 _CONFIGURERESULT = _descriptor.Descriptor(
   name='ConfigureResult',
   full_name='com.delphix.virtualization.platform.ConfigureResult',
   filename=None,
@@ -1939,16 +1946,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=7787,
-  serialized_end=7876,
+  serialized_start=7857,
+  serialized_end=7946,
 )
 
 
 _CONFIGURERESPONSE = _descriptor.Descriptor(
   name='ConfigureResponse',
   full_name='com.delphix.virtualization.platform.ConfigureResponse',
   filename=None,
@@ -1980,16 +1987,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.ConfigureResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=7879,
-  serialized_end=8059,
+  serialized_start=7949,
+  serialized_end=8129,
 )
 
 
 _UNCONFIGUREREQUEST = _descriptor.Descriptor(
   name='UnconfigureRequest',
   full_name='com.delphix.virtualization.platform.UnconfigureRequest',
   filename=None,
@@ -2032,16 +2039,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8062,
-  serialized_end=8315,
+  serialized_start=8132,
+  serialized_end=8385,
 )
 
 
 _UNCONFIGURERESULT = _descriptor.Descriptor(
   name='UnconfigureResult',
   full_name='com.delphix.virtualization.platform.UnconfigureResult',
   filename=None,
@@ -2056,16 +2063,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8317,
-  serialized_end=8336,
+  serialized_start=8387,
+  serialized_end=8406,
 )
 
 
 _UNCONFIGURERESPONSE = _descriptor.Descriptor(
   name='UnconfigureResponse',
   full_name='com.delphix.virtualization.platform.UnconfigureResponse',
   filename=None,
@@ -2097,16 +2104,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.UnconfigureResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=8339,
-  serialized_end=8523,
+  serialized_start=8409,
+  serialized_end=8593,
 )
 
 
 _VIRTUALCLEANUPREQUEST = _descriptor.Descriptor(
   name='VirtualCleanupRequest',
   full_name='com.delphix.virtualization.platform.VirtualCleanupRequest',
   filename=None,
@@ -2142,16 +2149,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8526,
-  serialized_end=8762,
+  serialized_start=8596,
+  serialized_end=8832,
 )
 
 
 _VIRTUALCLEANUPRESULT = _descriptor.Descriptor(
   name='VirtualCleanupResult',
   full_name='com.delphix.virtualization.platform.VirtualCleanupResult',
   filename=None,
@@ -2166,16 +2173,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8764,
-  serialized_end=8786,
+  serialized_start=8834,
+  serialized_end=8856,
 )
 
 
 _VIRTUALCLEANUPRESPONSE = _descriptor.Descriptor(
   name='VirtualCleanupResponse',
   full_name='com.delphix.virtualization.platform.VirtualCleanupResponse',
   filename=None,
@@ -2207,16 +2214,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.VirtualCleanupResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=8789,
-  serialized_end=8979,
+  serialized_start=8859,
+  serialized_end=9049,
 )
 
 
 _RECONFIGUREREQUEST = _descriptor.Descriptor(
   name='ReconfigureRequest',
   full_name='com.delphix.virtualization.platform.ReconfigureRequest',
   filename=None,
@@ -2259,16 +2266,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=8982,
-  serialized_end=9278,
+  serialized_start=9052,
+  serialized_end=9348,
 )
 
 
 _RECONFIGURERESULT = _descriptor.Descriptor(
   name='ReconfigureResult',
   full_name='com.delphix.virtualization.platform.ReconfigureResult',
   filename=None,
@@ -2290,16 +2297,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9280,
-  serialized_end=9371,
+  serialized_start=9350,
+  serialized_end=9441,
 )
 
 
 _RECONFIGURERESPONSE = _descriptor.Descriptor(
   name='ReconfigureResponse',
   full_name='com.delphix.virtualization.platform.ReconfigureResponse',
   filename=None,
@@ -2331,16 +2338,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.ReconfigureResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=9374,
-  serialized_end=9558,
+  serialized_start=9444,
+  serialized_end=9628,
 )
 
 
 _STARTREQUEST = _descriptor.Descriptor(
   name='StartRequest',
   full_name='com.delphix.virtualization.platform.StartRequest',
   filename=None,
@@ -2376,16 +2383,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9561,
-  serialized_end=9788,
+  serialized_start=9631,
+  serialized_end=9858,
 )
 
 
 _STARTRESULT = _descriptor.Descriptor(
   name='StartResult',
   full_name='com.delphix.virtualization.platform.StartResult',
   filename=None,
@@ -2400,16 +2407,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9790,
-  serialized_end=9803,
+  serialized_start=9860,
+  serialized_end=9873,
 )
 
 
 _STARTRESPONSE = _descriptor.Descriptor(
   name='StartResponse',
   full_name='com.delphix.virtualization.platform.StartResponse',
   filename=None,
@@ -2441,16 +2448,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.StartResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=9806,
-  serialized_end=9978,
+  serialized_start=9876,
+  serialized_end=10048,
 )
 
 
 _STOPREQUEST = _descriptor.Descriptor(
   name='StopRequest',
   full_name='com.delphix.virtualization.platform.StopRequest',
   filename=None,
@@ -2486,16 +2493,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=9981,
-  serialized_end=10207,
+  serialized_start=10051,
+  serialized_end=10277,
 )
 
 
 _STOPRESULT = _descriptor.Descriptor(
   name='StopResult',
   full_name='com.delphix.virtualization.platform.StopResult',
   filename=None,
@@ -2510,16 +2517,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10209,
-  serialized_end=10221,
+  serialized_start=10279,
+  serialized_end=10291,
 )
 
 
 _STOPRESPONSE = _descriptor.Descriptor(
   name='StopResponse',
   full_name='com.delphix.virtualization.platform.StopResponse',
   filename=None,
@@ -2551,16 +2558,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.StopResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=10224,
-  serialized_end=10394,
+  serialized_start=10294,
+  serialized_end=10464,
 )
 
 
 _VIRTUALPRESNAPSHOTREQUEST = _descriptor.Descriptor(
   name='VirtualPreSnapshotRequest',
   full_name='com.delphix.virtualization.platform.VirtualPreSnapshotRequest',
   filename=None,
@@ -2596,16 +2603,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10397,
-  serialized_end=10637,
+  serialized_start=10467,
+  serialized_end=10707,
 )
 
 
 _VIRTUALPRESNAPSHOTRESULT = _descriptor.Descriptor(
   name='VirtualPreSnapshotResult',
   full_name='com.delphix.virtualization.platform.VirtualPreSnapshotResult',
   filename=None,
@@ -2620,16 +2627,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10639,
-  serialized_end=10665,
+  serialized_start=10709,
+  serialized_end=10735,
 )
 
 
 _VIRTUALPRESNAPSHOTRESPONSE = _descriptor.Descriptor(
   name='VirtualPreSnapshotResponse',
   full_name='com.delphix.virtualization.platform.VirtualPreSnapshotResponse',
   filename=None,
@@ -2661,16 +2668,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.VirtualPreSnapshotResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=10668,
-  serialized_end=10866,
+  serialized_start=10738,
+  serialized_end=10936,
 )
 
 
 _VIRTUALPOSTSNAPSHOTREQUEST = _descriptor.Descriptor(
   name='VirtualPostSnapshotRequest',
   full_name='com.delphix.virtualization.platform.VirtualPostSnapshotRequest',
   filename=None,
@@ -2706,16 +2713,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=10869,
-  serialized_end=11110,
+  serialized_start=10939,
+  serialized_end=11180,
 )
 
 
 _VIRTUALPOSTSNAPSHOTRESULT = _descriptor.Descriptor(
   name='VirtualPostSnapshotResult',
   full_name='com.delphix.virtualization.platform.VirtualPostSnapshotResult',
   filename=None,
@@ -2737,16 +2744,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11112,
-  serialized_end=11202,
+  serialized_start=11182,
+  serialized_end=11272,
 )
 
 
 _VIRTUALPOSTSNAPSHOTRESPONSE = _descriptor.Descriptor(
   name='VirtualPostSnapshotResponse',
   full_name='com.delphix.virtualization.platform.VirtualPostSnapshotResponse',
   filename=None,
@@ -2778,16 +2785,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.VirtualPostSnapshotResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=11205,
-  serialized_end=11405,
+  serialized_start=11275,
+  serialized_end=11475,
 )
 
 
 _VIRTUALSTATUSREQUEST = _descriptor.Descriptor(
   name='VirtualStatusRequest',
   full_name='com.delphix.virtualization.platform.VirtualStatusRequest',
   filename=None,
@@ -2823,16 +2830,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11408,
-  serialized_end=11643,
+  serialized_start=11478,
+  serialized_end=11713,
 )
 
 
 _VIRTUALSTATUSRESULT = _descriptor.Descriptor(
   name='VirtualStatusResult',
   full_name='com.delphix.virtualization.platform.VirtualStatusResult',
   filename=None,
@@ -2855,16 +2862,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11646,
-  serialized_end=11784,
+  serialized_start=11716,
+  serialized_end=11854,
 )
 
 
 _VIRTUALSTATUSRESPONSE = _descriptor.Descriptor(
   name='VirtualStatusResponse',
   full_name='com.delphix.virtualization.platform.VirtualStatusResponse',
   filename=None,
@@ -2896,16 +2903,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.VirtualStatusResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=11787,
-  serialized_end=11975,
+  serialized_start=11857,
+  serialized_end=12045,
 )
 
 
 _INITIALIZEREQUEST = _descriptor.Descriptor(
   name='InitializeRequest',
   full_name='com.delphix.virtualization.platform.InitializeRequest',
   filename=None,
@@ -2934,16 +2941,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=11978,
-  serialized_end=12144,
+  serialized_start=12048,
+  serialized_end=12214,
 )
 
 
 _INITIALIZERESULT = _descriptor.Descriptor(
   name='InitializeResult',
   full_name='com.delphix.virtualization.platform.InitializeResult',
   filename=None,
@@ -2965,16 +2972,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12146,
-  serialized_end=12236,
+  serialized_start=12216,
+  serialized_end=12306,
 )
 
 
 _INITIALIZERESPONSE = _descriptor.Descriptor(
   name='InitializeResponse',
   full_name='com.delphix.virtualization.platform.InitializeResponse',
   filename=None,
@@ -3006,16 +3013,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.InitializeResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=12239,
-  serialized_end=12421,
+  serialized_start=12309,
+  serialized_end=12491,
 )
 
 
 _VIRTUALMOUNTSPECREQUEST = _descriptor.Descriptor(
   name='VirtualMountSpecRequest',
   full_name='com.delphix.virtualization.platform.VirtualMountSpecRequest',
   filename=None,
@@ -3044,16 +3051,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12424,
-  serialized_end=12590,
+  serialized_start=12494,
+  serialized_end=12660,
 )
 
 
 _VIRTUALMOUNTSPECRESULT = _descriptor.Descriptor(
   name='VirtualMountSpecResult',
   full_name='com.delphix.virtualization.platform.VirtualMountSpecResult',
   filename=None,
@@ -3082,16 +3089,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12593,
-  serialized_end=12761,
+  serialized_start=12663,
+  serialized_end=12831,
 )
 
 
 _VIRTUALMOUNTSPECRESPONSE = _descriptor.Descriptor(
   name='VirtualMountSpecResponse',
   full_name='com.delphix.virtualization.platform.VirtualMountSpecResponse',
   filename=None,
@@ -3123,16 +3130,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.VirtualMountSpecResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=12764,
-  serialized_end=12958,
+  serialized_start=12834,
+  serialized_end=13028,
 )
 
 
 _VIRTUALSOURCESIZEREQUEST = _descriptor.Descriptor(
   name='VirtualSourceSizeRequest',
   full_name='com.delphix.virtualization.platform.VirtualSourceSizeRequest',
   filename=None,
@@ -3168,16 +3175,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=12961,
-  serialized_end=13200,
+  serialized_start=13031,
+  serialized_end=13270,
 )
 
 
 _VIRTUALSOURCESIZERESULT = _descriptor.Descriptor(
   name='VirtualSourceSizeResult',
   full_name='com.delphix.virtualization.platform.VirtualSourceSizeResult',
   filename=None,
@@ -3199,16 +3206,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13202,
-  serialized_end=13250,
+  serialized_start=13272,
+  serialized_end=13320,
 )
 
 
 _VIRTUALSOURCESIZERESPONSE = _descriptor.Descriptor(
   name='VirtualSourceSizeResponse',
   full_name='com.delphix.virtualization.platform.VirtualSourceSizeResponse',
   filename=None,
@@ -3240,16 +3247,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.VirtualSourceSizeResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=13253,
-  serialized_end=13449,
+  serialized_start=13323,
+  serialized_end=13519,
 )
 
 
 _UPGRADEREQUEST_PREUPGRADEPARAMETERSENTRY = _descriptor.Descriptor(
   name='PreUpgradeParametersEntry',
   full_name='com.delphix.virtualization.platform.UpgradeRequest.PreUpgradeParametersEntry',
   filename=None,
@@ -3278,16 +3285,16 @@
   ],
   serialized_options=_b('8\001'),
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13705,
-  serialized_end=13764,
+  serialized_start=13775,
+  serialized_end=13834,
 )
 
 _UPGRADEREQUEST = _descriptor.Descriptor(
   name='UpgradeRequest',
   full_name='com.delphix.virtualization.platform.UpgradeRequest',
   filename=None,
   file=DESCRIPTOR,
@@ -3330,16 +3337,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13452,
-  serialized_end=13857,
+  serialized_start=13522,
+  serialized_end=13927,
 )
 
 
 _UPGRADERESULT_POSTUPGRADEPARAMETERSENTRY = _descriptor.Descriptor(
   name='PostUpgradeParametersEntry',
   full_name='com.delphix.virtualization.platform.UpgradeResult.PostUpgradeParametersEntry',
   filename=None,
@@ -3368,16 +3375,16 @@
   ],
   serialized_options=_b('8\001'),
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13989,
-  serialized_end=14049,
+  serialized_start=14059,
+  serialized_end=14119,
 )
 
 _UPGRADERESULT = _descriptor.Descriptor(
   name='UpgradeResult',
   full_name='com.delphix.virtualization.platform.UpgradeResult',
   filename=None,
   file=DESCRIPTOR,
@@ -3398,16 +3405,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=13860,
-  serialized_end=14049,
+  serialized_start=13930,
+  serialized_end=14119,
 )
 
 
 _UPGRADERESPONSE = _descriptor.Descriptor(
   name='UpgradeResponse',
   full_name='com.delphix.virtualization.platform.UpgradeResponse',
   filename=None,
@@ -3439,16 +3446,16 @@
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
     _descriptor.OneofDescriptor(
       name='result', full_name='com.delphix.virtualization.platform.UpgradeResponse.result',
       index=0, containing_type=None, fields=[]),
   ],
-  serialized_start=14052,
-  serialized_end=14228,
+  serialized_start=14122,
+  serialized_end=14298,
 )
 
 _PLUGINERRORRESULT.fields_by_name['generic_plugin_error'].message_type = _GENERICPLUGINERROR
 _PLUGINERRORRESULT.fields_by_name['unhandled_library_error'].message_type = _UNHANDLEDLIBRARYERROR
 _PLUGINERRORRESULT.fields_by_name['plugin_runtime_error'].message_type = _PLUGINRUNTIMEERROR
 _PLUGINERRORRESULT.fields_by_name['generated_classes_error'].message_type = _GENERATEDCLASSESERROR
 _PLUGINERRORRESULT.fields_by_name['user_error'].message_type = _USERERROR
@@ -3595,14 +3602,15 @@
 _STAGEDWORKERRESPONSE.oneofs_by_name['result'].fields.append(
   _STAGEDWORKERRESPONSE.fields_by_name['error'])
 _STAGEDWORKERRESPONSE.fields_by_name['error'].containing_oneof = _STAGEDWORKERRESPONSE.oneofs_by_name['result']
 _STAGEDMOUNTSPECREQUEST.fields_by_name['repository'].message_type = dlpx_dot_virtualization_dot_api_dot_common__pb2._REPOSITORY
 _STAGEDMOUNTSPECREQUEST.fields_by_name['staged_source'].message_type = dlpx_dot_virtualization_dot_api_dot_common__pb2._STAGEDSOURCE
 _STAGEDMOUNTSPECRESULT.fields_by_name['staged_mount'].message_type = dlpx_dot_virtualization_dot_api_dot_common__pb2._SINGLEENTIREMOUNT
 _STAGEDMOUNTSPECRESULT.fields_by_name['ownership_spec'].message_type = dlpx_dot_virtualization_dot_api_dot_common__pb2._OWNERSHIPSPEC
+_STAGEDMOUNTSPECRESULT.fields_by_name['mounts'].message_type = dlpx_dot_virtualization_dot_api_dot_common__pb2._SINGLESUBSETMOUNT
 _STAGEDMOUNTSPECRESPONSE.fields_by_name['return_value'].message_type = _STAGEDMOUNTSPECRESULT
 _STAGEDMOUNTSPECRESPONSE.fields_by_name['error'].message_type = _PLUGINERRORRESULT
 _STAGEDMOUNTSPECRESPONSE.oneofs_by_name['result'].fields.append(
   _STAGEDMOUNTSPECRESPONSE.fields_by_name['return_value'])
 _STAGEDMOUNTSPECRESPONSE.fields_by_name['return_value'].containing_oneof = _STAGEDMOUNTSPECRESPONSE.oneofs_by_name['result']
 _STAGEDMOUNTSPECRESPONSE.oneofs_by_name['result'].fields.append(
   _STAGEDMOUNTSPECRESPONSE.fields_by_name['error'])
```

### Comparing `dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/platform_service_pb2.py` & `dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/platform_service_pb2.py`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/dvp-api/dlpx/virtualization/api/platform_service_pb2_grpc.py` & `dvp-api-1.8.0/dvp-api/dlpx/virtualization/api/platform_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/dvp-api/dvp_api.egg-info/PKG-INFO` & `dvp-api-1.8.0/dvp-api/dvp_api.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvp-api
-Version: 1.7.0
+Version: 1.8.0
 Summary: Delphix Virtualization Platform API
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: # Delphix Virtualization Platform API
         
@@ -18,11 +18,11 @@
         The software is provided “as-is” without any warranties of any kind. To the maximum extent permitted by applicable law,
         Delphix Corp. and its affiliates disclaim any liability, implied warranties, including, without limitation, any implied
         warranties of merchantability, fitness for a particular purpose and non-infringement of intellectual property rights.
 Keywords: virtualization plugin
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `dvp-api-1.7.0/dvp-api/dvp_api.egg-info/SOURCES.txt` & `dvp-api-1.8.0/dvp-api/dvp_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvp-api-1.7.0/setup.cfg` & `dvp-api-1.8.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [metadata]
-metadata-version = 1.2
+metadata_version = 1.2
 author = Delphix
-author-email = virtualization-plugins@delphix.com
-home-page = https://developer.delphix.com
+author_email = virtualization-plugins@delphix.com
+home_page = https://developer.delphix.com
 summary = Delphix Virtualization Platform API
-long-description = file: README.md
-long-description-content-type = text/markdown
+long_description = file: README.md
+long_description_content_type = text/markdown
 keywords = virtualization plugin
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
-	Programming Language :: Python :: 2.7
+	Programming Language :: Python :: 3.8
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
-requires-python = 2.7
+requires_python = 3.8
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dvp-api-1.7.0/setup.py` & `dvp-api-1.8.0/setup.py`

 * *Files identical despite different names*

