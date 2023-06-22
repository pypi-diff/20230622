# Comparing `tmp/acore_server_metadata-0.4.5.tar.gz` & `tmp/acore_server_metadata-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_metadata-0.4.5.tar", last modified: Wed Jun 21 18:22:41 2023, max compression
+gzip compressed data, was "acore_server_metadata-0.5.1.tar", last modified: Thu Jun 22 16:35:01 2023, max compression
```

## Comparing `acore_server_metadata-0.4.5.tar` & `acore_server_metadata-0.5.1.tar`

### file list

```diff
@@ -1,42 +1,48 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.464861 acore_server_metadata-0.4.5/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-21 18:22:41.464722 acore_server_metadata-0.4.5/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.4.5/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.461737 acore_server_metadata-0.4.5/acore_server_metadata/
--rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.4.5/acore_server_metadata/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-21 18:22:06.000000 acore_server_metadata-0.4.5/acore_server_metadata/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      101 2023-06-15 20:16:05.000000 acore_server_metadata-0.4.5/acore_server_metadata/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.462674 acore_server_metadata-0.4.5/acore_server_metadata/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.4.5/acore_server_metadata/exc.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    27110 2023-06-21 18:19:29.000000 acore_server_metadata-0.4.5/acore_server_metadata/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.4.5/acore_server_metadata/settings.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.463312 acore_server_metadata-0.4.5/acore_server_metadata/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.4.5/acore_server_metadata/tests/mock_aws.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      155 2023-06-17 02:38:50.000000 acore_server_metadata-0.4.5/acore_server_metadata/utils.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.464056 acore_server_metadata-0.4.5/acore_server_metadata/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.4.5/acore_server_metadata/vendor/hashes.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/acore_server_metadata/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.462553 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      988 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-21 18:22:41.000000 acore_server_metadata-0.4.5/acore_server_metadata.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     3589 2023-06-21 18:22:00.000000 acore_server_metadata-0.4.5/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.4.5/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.4.5/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-21 18:22:41.464907 acore_server_metadata-0.4.5/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.4.5/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-21 18:22:41.464409 acore_server_metadata-0.4.5/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.4.5/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     5190 2023-06-17 17:52:12.000000 acore_server_metadata-0.4.5/tests/test_server.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.214875 acore_server_metadata-0.5.1/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1132 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      329 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-22 16:35:01.214724 acore_server_metadata-0.5.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5879 2023-06-19 18:57:43.000000 acore_server_metadata-0.5.1/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.209445 acore_server_metadata-0.5.1/acore_server_metadata/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      391 2023-06-16 02:28:42.000000 acore_server_metadata-0.5.1/acore_server_metadata/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-22 16:18:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      105 2023-06-22 16:18:25.000000 acore_server_metadata-0.5.1/acore_server_metadata/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.210413 acore_server_metadata-0.5.1/acore_server_metadata/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      496 2023-06-16 15:11:12.000000 acore_server_metadata-0.5.1/acore_server_metadata/exc.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      642 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/paths.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.211853 acore_server_metadata-0.5.1/acore_server_metadata/server/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-22 14:16:00.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-22 15:54:39.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    12199 2023-06-22 15:59:52.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    17224 2023-06-22 16:17:47.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/server_operation.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1665 2023-06-22 15:56:21.000000 acore_server_metadata-0.5.1/acore_server_metadata/server/server_status.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       89 2023-06-15 20:16:40.000000 acore_server_metadata-0.5.1/acore_server_metadata/settings.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.212638 acore_server_metadata-0.5.1/acore_server_metadata/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-16 01:30:10.000000 acore_server_metadata-0.5.1/acore_server_metadata/tests/mock_aws.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      479 2023-06-22 15:28:39.000000 acore_server_metadata-0.5.1/acore_server_metadata/utils.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.213645 acore_server_metadata-0.5.1/acore_server_metadata/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7553 2023-06-19 14:26:47.000000 acore_server_metadata-0.5.1/acore_server_metadata/vendor/hashes.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/acore_server_metadata/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.210288 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7028 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1187 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      242 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       22 2023-06-22 16:35:01.000000 acore_server_metadata-0.5.1/acore_server_metadata.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4218 2023-06-22 16:21:54.000000 acore_server_metadata-0.5.1/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-16 01:31:27.000000 acore_server_metadata-0.5.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       88 2023-06-19 18:46:02.000000 acore_server_metadata-0.5.1/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-22 16:35:01.214916 acore_server_metadata-0.5.1/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7570 2023-06-15 16:37:48.000000 acore_server_metadata-0.5.1/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 16:35:01.214314 acore_server_metadata-0.5.1/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1157 2023-06-19 18:53:48.000000 acore_server_metadata-0.5.1/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8010 2023-06-22 16:18:04.000000 acore_server_metadata-0.5.1/tests/test_server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      923 2023-06-22 15:33:22.000000 acore_server_metadata-0.5.1/tests/test_utils.py
```

### Comparing `acore_server_metadata-0.4.5/AUTHORS.rst` & `acore_server_metadata-0.5.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/LICENSE.txt` & `acore_server_metadata-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/PKG-INFO` & `acore_server_metadata-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_metadata
-Version: 0.4.5
+Version: 0.5.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.5#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.5/README.rst` & `acore_server_metadata-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/acore_server_metadata/paths.py` & `acore_server_metadata-0.5.1/acore_server_metadata/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/acore_server_metadata/tests/mock_aws.py` & `acore_server_metadata-0.5.1/acore_server_metadata/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/acore_server_metadata/vendor/hashes.py` & `acore_server_metadata-0.5.1/acore_server_metadata/vendor/hashes.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/acore_server_metadata/vendor/pytest_cov_helper.py` & `acore_server_metadata-0.5.1/acore_server_metadata/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/acore_server_metadata.egg-info/PKG-INFO` & `acore_server_metadata-0.5.1/acore_server_metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-metadata
-Version: 0.4.5
+Version: 0.5.1
 Summary: Azerothcore WOW server metadata for Fleet management.
 Home-page: https://github.com/MacHu-GWU/acore_server_metadata-project
-Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.4.5#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_metadata/0.5.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_metadata-0.4.5/acore_server_metadata.egg-info/SOURCES.txt` & `acore_server_metadata-0.5.1/acore_server_metadata.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -10,24 +10,29 @@
 requirements.txt
 setup.py
 acore_server_metadata/__init__.py
 acore_server_metadata/_version.py
 acore_server_metadata/api.py
 acore_server_metadata/exc.py
 acore_server_metadata/paths.py
-acore_server_metadata/server.py
 acore_server_metadata/settings.py
 acore_server_metadata/utils.py
 acore_server_metadata.egg-info/PKG-INFO
 acore_server_metadata.egg-info/SOURCES.txt
 acore_server_metadata.egg-info/dependency_links.txt
 acore_server_metadata.egg-info/requires.txt
 acore_server_metadata.egg-info/top_level.txt
 acore_server_metadata/docs/__init__.py
+acore_server_metadata/server/__init__.py
+acore_server_metadata/server/api.py
+acore_server_metadata/server/server.py
+acore_server_metadata/server/server_operation.py
+acore_server_metadata/server/server_status.py
 acore_server_metadata/tests/__init__.py
 acore_server_metadata/tests/helper.py
 acore_server_metadata/tests/mock_aws.py
 acore_server_metadata/vendor/__init__.py
 acore_server_metadata/vendor/hashes.py
 acore_server_metadata/vendor/pytest_cov_helper.py
 tests/test_api.py
-tests/test_server.py
+tests/test_server.py
+tests/test_utils.py
```

### Comparing `acore_server_metadata-0.4.5/release-history.rst` & `acore_server_metadata-0.5.1/release-history.rst`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,26 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.1 (2023-06-22)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- Now the ``acore_server_metadata.api.Server.get_server()`` method will always return a ``Server`` object. If the ec2 or rds doesn't not exists, then the ``ec2_inst`` or ``rds_inst`` attribure of the ``Server`` object will be ``None``. This behavior was returning ``None`` before.
+- Similarly the ``acore_server_metadata.api.Server.batch_get_server()`` method will always return a ``Server`` object for specific id.
+
+**Minor Improvements**
+
+- add many unit test to cover the server operations API.
+
+
 0.4.5 (2023-06-21)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug when "check=True", we didn't use the object representing the latest ec2 or rds metadata.
```

### Comparing `acore_server_metadata-0.4.5/requirements-doc.txt` & `acore_server_metadata-0.5.1/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/setup.py` & `acore_server_metadata-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `acore_server_metadata-0.4.5/tests/test_api.py` & `acore_server_metadata-0.5.1/tests/test_api.py`

 * *Files identical despite different names*

