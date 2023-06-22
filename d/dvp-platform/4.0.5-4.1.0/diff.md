# Comparing `tmp/dvp-platform-4.0.5.tar.gz` & `tmp/dvp-platform-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvp-platform-4.0.5.tar", last modified: Tue Sep 13 07:39:52 2022, max compression
+gzip compressed data, was "dvp-platform-4.1.0.tar", last modified: Thu Jun 22 07:59:01 2023, max compression
```

## Comparing `dvp-platform-4.0.5.tar` & `dvp-platform-4.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.556752 dvp-platform-4.0.5/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    11358 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/LICENSE
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      136 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/MANIFEST.in
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1274 2022-09-13 07:39:52.556934 dvp-platform-4.0.5/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      535 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/README.md
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      682 2022-09-13 07:39:52.559166 dvp-platform-4.0.5/setup.cfg
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      673 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/setup.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.383161 dvp-platform-4.0.5/src/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.383446 dvp-platform-4.0.5/src/main/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.385112 dvp-platform-4.0.5/src/main/python/
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.405512 dvp-platform-4.0.5/src/main/python/dlpx/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      124 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.411833 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      124 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/__init__.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.546388 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        6 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/VERSION
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      822 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/__init__.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     6493 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_discovery.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    36268 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_linked.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     4788 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_plugin.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    10546 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_plugin_classes.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     9656 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_upgrade.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    36562 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_virtual.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    10053 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/exceptions.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     3748 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/import_util.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     7763 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/import_validations.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)    13612 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/migration_helper.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1437 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/operation.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      332 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/util.py
--rw-r--r--   0 sourabh.jain   (503) staff       (20)      347 2022-09-13 04:50:46.000000 dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/validation_util.py
-drwxr-xr-x   0 sourabh.jain   (503) staff       (20)        0 2022-09-13 07:39:52.556289 dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1274 2022-09-13 07:39:52.000000 dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/PKG-INFO
--rw-r--r--   0 sourabh.jain   (503) staff       (20)     1273 2022-09-13 07:39:52.000000 dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/SOURCES.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        1 2022-09-13 07:39:52.000000 dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/dependency_links.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)       67 2022-09-13 07:39:52.000000 dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/requires.txt
--rw-r--r--   0 sourabh.jain   (503) staff       (20)        5 2022-09-13 07:39:52.000000 dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.374164 dvp-platform-4.1.0/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    11358 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/LICENSE
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      136 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/MANIFEST.in
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1152 2023-06-22 07:59:01.374541 dvp-platform-4.1.0/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      535 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/README.md
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      570 2023-06-22 07:59:01.375571 dvp-platform-4.1.0/setup.cfg
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      614 2023-06-22 07:09:25.000000 dvp-platform-4.1.0/setup.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.344470 dvp-platform-4.1.0/src/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.344612 dvp-platform-4.1.0/src/main/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.345450 dvp-platform-4.1.0/src/main/python/
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.350359 dvp-platform-4.1.0/src/main/python/dlpx/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      124 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.351406 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      124 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/__init__.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.369918 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        6 2023-06-22 07:09:25.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/VERSION
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      822 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/__init__.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     6493 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_discovery.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    36507 2023-06-22 07:09:25.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_linked.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     4788 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_plugin.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    10728 2023-06-22 07:09:25.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_plugin_classes.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     9656 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_upgrade.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    36562 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_virtual.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    10053 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/exceptions.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     3748 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/import_util.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     7763 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/import_validations.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)    13612 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/migration_helper.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1437 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/operation.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      332 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/util.py
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)      347 2022-09-05 09:36:54.000000 dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/validation_util.py
+drwxr-xr-x   0 vimleshmishra   (503) staff       (20)        0 2023-06-22 07:59:01.373555 dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1152 2023-06-22 07:59:01.000000 dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)     1273 2023-06-22 07:59:01.000000 dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        1 2023-06-22 07:59:01.000000 dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)       49 2023-06-22 07:59:01.000000 dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/requires.txt
+-rw-r--r--   0 vimleshmishra   (503) staff       (20)        5 2023-06-22 07:59:01.000000 dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/top_level.txt
```

### Comparing `dvp-platform-4.0.5/LICENSE` & `dvp-platform-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/PKG-INFO` & `dvp-platform-4.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dvp-platform
-Version: 4.0.5
+Version: 4.1.0
 Summary: Delphix Virtualization Platform APIs
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: **Standalone installation of this package is not supported.** Please install the [dvp](https://pypi.org/project/dvp/) package which will install this package.
         
         # Disclaimer
         
         The software is provided “as-is” without any warranties of any kind. To the maximum extent permitted by applicable law, Delphix Corp. and its affiliates disclaim any liability, implied warranties, including, without limitation, any implied warranties of merchantability, fitness for a particular purpose and non-infringement of intellectual property rights.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7, <3.9, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+Requires-Python: >=3.8, <3.9
 Description-Content-Type: text/markdown
```

### Comparing `dvp-platform-4.0.5/README.md` & `dvp-platform-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/setup.cfg` & `dvp-platform-4.1.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 home_page = https://developer.delphix.com
 summary = Delphix Virtualization Platform APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Programming Language :: Python
-	Programming Language :: Python :: 2.7
 	Programming Language :: Python :: 3.8
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 
 [options]
-requires_python = >=2.7, <=3.8, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+requires_python = >=3.8, <3.9
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/__init__.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_discovery.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_discovery.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_linked.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_linked.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,14 +108,38 @@
                 raise OperationAlreadyDefinedError(Op.LINKED_SOURCE_SIZE)
             self.source_size_impl = v.check_function(source_size_impl,
                                                      Op.LINKED_SOURCE_SIZE)
             return source_size_impl
 
         return source_size_decorator
 
+    @staticmethod
+    def _from_protobuf_remote_mount(remote_mount):
+        return Mount(remote_environment=RemoteEnvironment.from_proto(
+            remote_mount.remote_environment),
+            mount_path=remote_mount.mount_path,
+            shared_path=remote_mount.shared_path)
+
+    @staticmethod
+    def _get_mounts_from_request(request):
+        staged_mount = request.staged_source.staged_mount
+        mounts = request.staged_source.mounts
+        if mounts and len(mounts) > 0 and staged_mount and \
+                staged_mount.mount_path and len(staged_mount.mount_path) > 0 \
+                and staged_mount.remote_environment:
+            raise PluginRuntimeError(
+                'Either staged_mount or mounts can be present for staging source. '
+                'Found both staged_mount and mounts.')
+
+        if mounts and len(mounts) > 0:
+            return None, [
+                LinkedOperations._from_protobuf_remote_mount(m) for m in mounts]
+        else:
+            return LinkedOperations._from_protobuf_remote_mount(staged_mount), None
+
     def _internal_direct_pre_snapshot(self, request):
         """Pre Snapshot Wrapper for direct plugins.
 
         Executed before creating a snapshot. This plugin
         operation is run prior to creating a snapshot for a direct source.
 
         Run pre-snapshot operation for a direct source.
@@ -327,27 +351,24 @@
         #
         if not self.pre_snapshot_impl:
             raise OperationNotDefinedError(Op.LINKED_PRE_SNAPSHOT)
 
         linked_source = request.staged_source.linked_source
         staged_source_definition = (LinkedSourceDefinition.from_dict(
             json.loads(linked_source.parameters.json)))
-        staged_mount = request.staged_source.staged_mount
-        mount = Mount(remote_environment=RemoteEnvironment.from_proto(
-            staged_mount.remote_environment),
-            mount_path=staged_mount.mount_path,
-            shared_path=staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
         source_config = SourceConfigDefinition.from_dict(
             json.loads(request.source_config.parameters.json))
         snap_params = json.loads(request.snapshot_parameters.parameters.json)
         #
@@ -402,27 +423,24 @@
             return snapshot_protobuf
 
         if not self.post_snapshot_impl:
             raise OperationNotDefinedError(Op.LINKED_POST_SNAPSHOT)
 
         staged_source_definition = LinkedSourceDefinition.from_dict(
             json.loads(request.staged_source.linked_source.parameters.json))
-        mount = Mount(
-            remote_environment=RemoteEnvironment.from_proto(
-                request.staged_source.staged_mount.remote_environment),
-            mount_path=request.staged_source.staged_mount.mount_path,
-            shared_path=request.staged_source.staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=request.staged_source.linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
         source_config = SourceConfigDefinition.from_dict(
             json.loads(request.source_config.parameters.json))
         snap_params = json.loads(request.snapshot_parameters.parameters.json)
         #
@@ -476,27 +494,24 @@
         # not be called if it wasn't implemented.
         #
         if not self.start_staging_impl:
             raise OperationNotDefinedError(Op.LINKED_START_STAGING)
 
         staged_source_definition = LinkedSourceDefinition.from_dict(
             json.loads(request.staged_source.linked_source.parameters.json))
-        mount = Mount(
-            remote_environment=(RemoteEnvironment.from_proto(
-                request.staged_source.staged_mount.remote_environment)),
-            mount_path=request.staged_source.staged_mount.mount_path,
-            shared_path=request.staged_source.staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=request.staged_source.linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
         source_config = SourceConfigDefinition.from_dict(
             json.loads(request.source_config.parameters.json))
 
         self.start_staging_impl(staged_source=staged_source,
@@ -535,27 +550,24 @@
         # not be called if it wasn't implemented.
         #
         if not self.stop_staging_impl:
             raise OperationNotDefinedError(Op.LINKED_STOP_STAGING)
 
         staged_source_definition = LinkedSourceDefinition.from_dict(
             json.loads(request.staged_source.linked_source.parameters.json))
-        mount = Mount(
-            remote_environment=(RemoteEnvironment.from_proto(
-                request.staged_source.staged_mount.remote_environment)),
-            mount_path=request.staged_source.staged_mount.mount_path,
-            shared_path=request.staged_source.staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=request.staged_source.linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
         source_config = SourceConfigDefinition.from_dict(
             json.loads(request.source_config.parameters.json))
 
         self.stop_staging_impl(staged_source=staged_source,
@@ -594,27 +606,24 @@
         # not be called if it wasn't implemented.
         #
         if not self.status_impl:
             raise OperationNotDefinedError(Op.LINKED_STATUS)
 
         staged_source_definition = LinkedSourceDefinition.from_dict(
             json.loads(request.staged_source.linked_source.parameters.json))
-        mount = Mount(
-            remote_environment=(RemoteEnvironment.from_proto(
-                request.staged_source.staged_mount.remote_environment)),
-            mount_path=request.staged_source.staged_mount.mount_path,
-            shared_path=request.staged_source.staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=request.staged_source.linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
         source_config = SourceConfigDefinition.from_dict(
             json.loads(request.source_config.parameters.json))
 
         status = self.status_impl(staged_source=staged_source,
@@ -657,27 +666,24 @@
         # not be called if it wasn't implemented.
         #
         if not self.worker_impl:
             raise OperationNotDefinedError(Op.LINKED_WORKER)
 
         staged_source_definition = LinkedSourceDefinition.from_dict(
             json.loads(request.staged_source.linked_source.parameters.json))
-        mount = Mount(
-            remote_environment=(RemoteEnvironment.from_proto(
-                request.staged_source.staged_mount.remote_environment)),
-            mount_path=request.staged_source.staged_mount.mount_path,
-            shared_path=request.staged_source.staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=request.staged_source.linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
         source_config = SourceConfigDefinition.from_dict(
             json.loads(request.source_config.parameters.json))
 
         self.worker_impl(staged_source=staged_source,
@@ -708,14 +714,24 @@
            success. In case of errors, response object will contain
            PluginErrorResult.
         """
         # Reasoning for method imports are in this file's docstring.
         from generated.definitions import RepositoryDefinition
         from generated.definitions import LinkedSourceDefinition
 
+        def to_protobuf_subset_mount(subset_mount):
+            subset_mount_protobuf = common_pb2.SingleSubsetMount()
+            subset_mount_protobuf.mount_path = subset_mount.mount_path
+            subset_mount_protobuf.remote_environment.CopyFrom(
+                subset_mount.remote_environment.to_proto())
+            if subset_mount.shared_path:
+                subset_mount_protobuf.shared_path = subset_mount.shared_path
+
+            return subset_mount_protobuf
+
         def to_protobuf_single_mount(single_mount):
             if single_mount.shared_path:
                 raise PluginRuntimeError(
                     'Shared path is not supported for linked sources.')
 
             single_mount_protobuf = common_pb2.SingleEntireMount()
             single_mount_protobuf.mount_path = single_mount.mount_path
@@ -730,52 +746,51 @@
             return ownership_spec_protobuf
 
         if not self.mount_specification_impl:
             raise OperationNotDefinedError(Op.LINKED_MOUNT_SPEC)
 
         staged_source_definition = LinkedSourceDefinition.from_dict(
             json.loads(request.staged_source.linked_source.parameters.json))
-        mount = Mount(
-            remote_environment=(RemoteEnvironment.from_proto(
-                request.staged_source.staged_mount.remote_environment)),
-            mount_path=request.staged_source.staged_mount.mount_path,
-            shared_path=request.staged_source.staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=request.staged_source.linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
 
         mount_spec = self.mount_specification_impl(staged_source=staged_source,
                                                    repository=repository)
 
         # Validate that this is a MountSpecification object.
         if not isinstance(mount_spec, MountSpecification):
             raise IncorrectReturnTypeError(Op.LINKED_MOUNT_SPEC,
                                            type(mount_spec),
                                            MountSpecification)
 
-        # Only one mount is supported for linked sources.
+        staged_mount_spec_response = platform_pb2.StagedMountSpecResponse()
+
         mount_len = len(mount_spec.mounts)
-        if mount_len != 1:
+        if mount_len < 1:
             raise PluginRuntimeError(
-                'Exactly one mount must be provided for staging sources.'
-                ' Found {}'.format(mount_len))
-
-        staged_mount = to_protobuf_single_mount(mount_spec.mounts[0])
-
-        staged_mount_spec_response = platform_pb2.StagedMountSpecResponse()
-        staged_mount_spec_response.return_value.staged_mount.CopyFrom(
-            staged_mount)
+                'Mount must be provided for staging sources.'
+                ' Found {} mounts.'.format(mount_len))
+        elif mount_len > 1:
+            mounts = [to_protobuf_subset_mount(m) for m in mount_spec.mounts]
+            staged_mount_spec_response.return_value.mounts.extend(mounts)
+        else:
+            staged_mount = to_protobuf_single_mount(mount_spec.mounts[0])
+            staged_mount_spec_response.return_value.staged_mount.CopyFrom(
+                staged_mount)
 
         # Ownership spec is optional for linked sources.
         if mount_spec.ownership_specification:
             ownership_spec = to_protobuf_ownership_spec(
                 mount_spec.ownership_specification)
             staged_mount_spec_response.return_value.ownership_spec.CopyFrom(
                 ownership_spec)
@@ -808,27 +823,24 @@
         # not be called if it wasn't implemented.
         #
         if not self.source_size_impl:
             raise OperationNotDefinedError(Op.LINKED_SOURCE_SIZE)
 
         staged_source_definition = LinkedSourceDefinition.from_dict(
             json.loads(request.staged_source.linked_source.parameters.json))
-        mount = Mount(
-            remote_environment=(RemoteEnvironment.from_proto(
-                request.staged_source.staged_mount.remote_environment)),
-            mount_path=request.staged_source.staged_mount.mount_path,
-            shared_path=request.staged_source.staged_mount.shared_path)
+        staged_mount, mounts = LinkedOperations._get_mounts_from_request(request)
         staged_source = StagedSource(
             guid=request.staged_source.linked_source.guid,
             source_connection=RemoteConnection.from_proto(
                 request.staged_source.source_connection),
             parameters=staged_source_definition,
-            mount=mount,
+            mount=staged_mount,
             staged_connection=RemoteConnection.from_proto(
-                request.staged_source.staged_connection))
+                request.staged_source.staged_connection),
+            mounts=mounts)
 
         repository = RepositoryDefinition.from_dict(
             json.loads(request.repository.parameters.json))
         source_config = SourceConfigDefinition.from_dict(
             json.loads(request.source_config.parameters.json))
 
         source_size = self.source_size_impl(
```

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_plugin.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_plugin.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_plugin_classes.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_plugin_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,27 +55,28 @@
     def mounts(self):
         """list(Mount): The mounts of this VirtualSource."""
         return self._mounts
 
 
 class StagedSource(object):
     def __init__(self, guid, source_connection, parameters, mount,
-                 staged_connection):
+                 staged_connection, mounts):
 
         self._guid = guid
         if not isinstance(source_connection, RemoteConnection):
             raise IncorrectTypeError(RemoteConnection, 'source_connection',
                                      type(source_connection), RemoteConnection)
         self._source_connection = source_connection
         self._parameters = parameters
         self._mount = mount
         if not isinstance(staged_connection, RemoteConnection):
             raise IncorrectTypeError(RemoteConnection, 'staged_connection',
                                      type(staged_connection), RemoteConnection)
         self._staged_connection = staged_connection
+        self._mounts = mounts
 
     @property
     def guid(self):
         """str: The unique guid identifier for this StagedSource."""
         return self._guid
 
     @property
@@ -89,23 +90,28 @@
         """LinkedSourceDefinition: The LinkedSourceDefinition for this
         StagedSource.
         """
         return self._parameters
 
     @property
     def mount(self):
-        """MountSpecification: The MountSpecification for this StagedSource."""
+        """MountSpecification: The SingleEntireMount for this StagedSource."""
         return self._mount
 
     @property
     def staged_connection(self):
         """RemoteConnection: The RemoteConnection representing the
         staging environment for this StagedSource."""
         return self._staged_connection
 
+    @property
+    def mounts(self):
+        """list(Mount): The List of SingleSubsetMounts of this StagedSource."""
+        return self._mounts
+
 
 class DirectSource(object):
     def __init__(self, guid, connection, parameters):
         self._guid = guid
         if not isinstance(connection, RemoteConnection):
             raise IncorrectTypeError(RemoteConnection, 'connection',
                                      type(connection), RemoteConnection)
```

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_upgrade.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_upgrade.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/_virtual.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/_virtual.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/exceptions.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/exceptions.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/import_util.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/import_util.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/import_validations.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/import_validations.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/migration_helper.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/migration_helper.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dlpx/virtualization/platform/operation.py` & `dvp-platform-4.1.0/src/main/python/dlpx/virtualization/platform/operation.py`

 * *Files identical despite different names*

### Comparing `dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/PKG-INFO` & `dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: dvp-platform
-Version: 4.0.5
+Version: 4.1.0
 Summary: Delphix Virtualization Platform APIs
 Home-page: https://developer.delphix.com
 Author: Delphix
 Author-email: virtualization-plugins@delphix.com
 License: UNKNOWN
 Description: **Standalone installation of this package is not supported.** Please install the [dvp](https://pypi.org/project/dvp/) package which will install this package.
         
         # Disclaimer
         
         The software is provided “as-is” without any warranties of any kind. To the maximum extent permitted by applicable law, Delphix Corp. and its affiliates disclaim any liability, implied warranties, including, without limitation, any implied warranties of merchantability, fitness for a particular purpose and non-infringement of intellectual property rights.
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=2.7, <3.9, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
+Requires-Python: >=3.8, <3.9
 Description-Content-Type: text/markdown
```

### Comparing `dvp-platform-4.0.5/src/main/python/dvp_platform.egg-info/SOURCES.txt` & `dvp-platform-4.1.0/src/main/python/dvp_platform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

