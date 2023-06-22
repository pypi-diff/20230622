# Comparing `tmp/simple_aws_ec2-0.5.1.tar.gz` & `tmp/simple_aws_ec2-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_ec2-0.5.1.tar", last modified: Mon Jun 19 18:45:38 2023, max compression
+gzip compressed data, was "simple_aws_ec2-0.5.2.tar", last modified: Thu Jun 22 03:47:59 2023, max compression
```

## Comparing `simple_aws_ec2-0.5.1.tar` & `simple_aws_ec2-0.5.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.256548 simple_aws_ec2-0.5.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:16.000000 simple_aws_ec2-0.5.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-19 18:45:38.256381 simple_aws_ec2-0.5.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     5722 2023-06-14 19:01:43.000000 simple_aws_ec2-0.5.1/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     2825 2023-06-19 18:45:02.000000 simple_aws_ec2-0.5.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.5.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.5.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 18:45:38.256605 simple_aws_ec2-0.5.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.5.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.254222 simple_aws_ec2-0.5.1/simple_aws_ec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 18:27:29.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1389 2023-06-16 01:11:20.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.255104 simple_aws_ec2-0.5.1/simple_aws_ec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)    33502 2023-06-19 18:24:31.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/exc.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.255612 simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/waiter.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.254980 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-19 18:45:38.000000 simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 18:45:38.256030 simple_aws_ec2-0.5.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)     3114 2023-06-19 18:43:04.000000 simple_aws_ec2-0.5.1/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8301 2023-06-19 18:43:04.000000 simple_aws_ec2-0.5.1/tests/test_ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 03:47:59.850049 simple_aws_ec2-0.5.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-15 19:02:16.000000 simple_aws_ec2-0.5.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-22 03:47:59.849907 simple_aws_ec2-0.5.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5722 2023-06-14 19:01:43.000000 simple_aws_ec2-0.5.2/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3038 2023-06-22 03:47:20.000000 simple_aws_ec2-0.5.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      228 2023-06-14 13:05:19.000000 simple_aws_ec2-0.5.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       48 2023-06-14 12:12:36.000000 simple_aws_ec2-0.5.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-22 03:47:59.850102 simple_aws_ec2-0.5.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.5.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 03:47:59.847727 simple_aws_ec2-0.5.2/simple_aws_ec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-22 03:46:46.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1389 2023-06-16 01:11:20.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 03:47:59.848589 simple_aws_ec2-0.5.2/simple_aws_ec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)    34037 2023-06-22 03:46:31.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       69 2023-06-15 22:05:33.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/exc.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 03:47:59.849129 simple_aws_ec2-0.5.2/simple_aws_ec2/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-15 18:28:54.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2351 2023-06-15 18:56:04.000000 simple_aws_ec2-0.5.2/simple_aws_ec2/vendor/waiter.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 03:47:59.848460 simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6784 2023-06-22 03:47:59.000000 simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      599 2023-06-22 03:47:59.000000 simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-22 03:47:59.000000 simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      264 2023-06-22 03:47:59.000000 simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-06-22 03:47:59.000000 simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 03:47:59.849593 simple_aws_ec2-0.5.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3114 2023-06-19 18:43:04.000000 simple_aws_ec2-0.5.2/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8301 2023-06-19 18:43:04.000000 simple_aws_ec2-0.5.2/tests/test_ec2.py
```

### Comparing `simple_aws_ec2-0.5.1/AUTHORS.rst` & `simple_aws_ec2-0.5.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/LICENSE.txt` & `simple_aws_ec2-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/PKG-INFO` & `simple_aws_ec2-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple_aws_ec2
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.5.1/README.rst` & `simple_aws_ec2-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/release-history.rst` & `simple_aws_ec2-0.5.2/release-history.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.5.2 (2023-06-21)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+- add a few ec2 metadata api methods for :meth:`~simple_aws_ec2.ec2.Ec2Instance`.
+
+
 0.5.1 (2023-06-19)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - add :meth:`~simple_aws_ec2.ec2.Ec2Instance.terminate_instance` method.
```

### Comparing `simple_aws_ec2-0.5.1/requirements-doc.txt` & `simple_aws_ec2-0.5.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/setup.py` & `simple_aws_ec2-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/simple_aws_ec2/api.py` & `simple_aws_ec2-0.5.2/simple_aws_ec2/api.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/simple_aws_ec2/ec2.py` & `simple_aws_ec2-0.5.2/simple_aws_ec2/ec2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """
 Abstract dataclass for EC2 instance.
 """
 
 import typing as T
 import enum
+import json
 import dataclasses
 from datetime import datetime
 from urllib import request
 
 from func_args import resolve_kwargs, NOTHING
 from iterproxy import IterProxy
 
@@ -515,14 +516,18 @@
         return _get_metadata(name="instance-id")
 
     @classmethod
     def get_instance_type(cls) -> str:  # pragma: no cover
         return _get_metadata(name="instance-type")
 
     @classmethod
+    def get_hostname(cls) -> str:  # pragma: no cover
+        return _get_metadata(name="hostname")
+
+    @classmethod
     def get_local_hostname(cls) -> str:  # pragma: no cover
         return _get_metadata(name="local-hostname")
 
     @classmethod
     def get_local_ipv4(cls) -> str:  # pragma: no cover
         return _get_metadata(name="local-ipv4")
 
@@ -534,14 +539,26 @@
     def get_public_ipv4(cls) -> str:  # pragma: no cover
         return _get_metadata(name="public-ipv4")
 
     @classmethod
     def get_security_groups(cls) -> T.List[str]:  # pragma: no cover
         return _get_metadata(name="security-groups").splitlines()
 
+    @classmethod
+    def get_iam_info(cls) -> T.Dict[str, str]:  # pragma: no cover
+        return json.loads(_get_metadata(name="iam/info"))
+
+    @classmethod
+    def get_placement_region(cls) -> str: # pragma: no cover
+        return _get_metadata(name="placement/region")
+
+    @classmethod
+    def get_reservation_id(cls) -> str: # pragma: no cover
+        return _get_metadata(name="reservation-id")
+
 
 class Ec2InstanceIterProxy(IterProxy[Ec2Instance]):
     """
     Advanced iterator proxy for :class:`Ec2Instance`.
     """
```

### Comparing `simple_aws_ec2-0.5.1/simple_aws_ec2/vendor/waiter.py` & `simple_aws_ec2-0.5.2/simple_aws_ec2/vendor/waiter.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/PKG-INFO` & `simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: simple-aws-ec2
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.5.1#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.5.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.5.1/simple_aws_ec2.egg-info/SOURCES.txt` & `simple_aws_ec2-0.5.2/simple_aws_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/tests/test_api.py` & `simple_aws_ec2-0.5.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.5.1/tests/test_ec2.py` & `simple_aws_ec2-0.5.2/tests/test_ec2.py`

 * *Files identical despite different names*

