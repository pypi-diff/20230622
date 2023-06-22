# Comparing `tmp/acore_server_config-0.3.1.tar.gz` & `tmp/acore_server_config-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acore_server_config-0.3.1.tar", last modified: Mon Jun 19 17:20:24 2023, max compression
+gzip compressed data, was "acore_server_config-0.3.2.tar", last modified: Thu Jun 22 04:14:39 2023, max compression
```

## Comparing `acore_server_config-0.3.1.tar` & `acore_server_config-0.3.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.499216 acore_server_config-0.3.1/
--rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-19 17:20:24.499072 acore_server_config-0.3.1/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.3.1/README.rst
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.495279 acore_server_config-0.3.1/acore_server_config/
--rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.3.1/acore_server_config/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-19 16:53:00.000000 acore_server_config-0.3.1/acore_server_config/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      492 2023-06-19 16:52:37.000000 acore_server_config-0.3.1/acore_server_config/api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      674 2023-06-18 03:18:29.000000 acore_server_config-0.3.1/acore_server_config/boto_ses.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.3.1/acore_server_config/compat.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.496443 acore_server_config-0.3.1/acore_server_config/config/
--rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-19 17:13:43.000000 acore_server_config-0.3.1/acore_server_config/config/__init__.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.496939 acore_server_config-0.3.1/acore_server_config/config/define/
--rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-06-19 17:13:36.000000 acore_server_config-0.3.1/acore_server_config/config/define/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.3.1/acore_server_config/config/define/main.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1370 2023-06-19 17:13:51.000000 acore_server_config-0.3.1/acore_server_config/config/define/server.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.3.1/acore_server_config/config/init.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     8011 2023-06-19 17:03:54.000000 acore_server_config-0.3.1/acore_server_config/config/loader.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.497105 acore_server_config-0.3.1/acore_server_config/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3938 2023-06-19 16:51:35.000000 acore_server_config-0.3.1/acore_server_config/in_ec2.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.3.1/acore_server_config/paths.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     1467 2023-06-17 23:09:11.000000 acore_server_config-0.3.1/acore_server_config/runtime.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.498099 acore_server_config-0.3.1/acore_server_config/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/tests/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      362 2023-06-19 16:31:24.000000 acore_server_config-0.3.1/acore_server_config/tests/dummy_config.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/tests/helper.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-19 16:26:34.000000 acore_server_config-0.3.1/acore_server_config/tests/mock_aws.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.498617 acore_server_config-0.3.1/acore_server_config/vendor/
--rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/vendor/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/acore_server_config/vendor/pytest_cov_helper.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.495984 acore_server_config-0.3.1/acore_server_config.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      285 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-19 17:20:24.000000 acore_server_config-0.3.1/acore_server_config.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)     2631 2023-06-19 16:57:27.000000 acore_server_config-0.3.1/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/requirements-automation.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.3.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-06-19 16:26:45.000000 acore_server_config-0.3.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-18 00:59:01.000000 acore_server_config-0.3.1/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-19 17:20:24.499273 acore_server_config-0.3.1/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.3.1/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-19 17:20:24.498777 acore_server_config-0.3.1/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      501 2023-06-19 16:53:17.000000 acore_server_config-0.3.1/tests/test_api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.888080 acore_server_config-0.3.2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      670 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1130 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      327 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-22 04:14:39.887931 acore_server_config-0.3.2/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4041 2023-06-18 01:42:46.000000 acore_server_config-0.3.2/README.rst
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.883260 acore_server_config-0.3.2/acore_server_config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      429 2023-06-18 01:38:46.000000 acore_server_config-0.3.2/acore_server_config/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-06-22 03:51:17.000000 acore_server_config-0.3.2/acore_server_config/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      492 2023-06-19 16:52:37.000000 acore_server_config-0.3.2/acore_server_config/api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1149 2023-06-22 03:51:05.000000 acore_server_config-0.3.2/acore_server_config/boto_ses.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      128 2023-06-16 18:25:58.000000 acore_server_config-0.3.2/acore_server_config/compat.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.884510 acore_server_config-0.3.2/acore_server_config/config/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       50 2023-06-19 17:13:43.000000 acore_server_config-0.3.2/acore_server_config/config/__init__.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.885243 acore_server_config-0.3.2/acore_server_config/config/define/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       98 2023-06-19 17:13:36.000000 acore_server_config-0.3.2/acore_server_config/config/define/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2672 2023-06-18 00:57:04.000000 acore_server_config-0.3.2/acore_server_config/config/define/main.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1565 2023-06-19 17:35:38.000000 acore_server_config-0.3.2/acore_server_config/config/define/server.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1634 2023-06-18 00:44:26.000000 acore_server_config-0.3.2/acore_server_config/config/init.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     8011 2023-06-19 17:03:54.000000 acore_server_config-0.3.2/acore_server_config/config/loader.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.885877 acore_server_config-0.3.2/acore_server_config/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3938 2023-06-19 16:51:35.000000 acore_server_config-0.3.2/acore_server_config/in_ec2.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-17 20:38:51.000000 acore_server_config-0.3.2/acore_server_config/paths.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2300 2023-06-22 03:31:06.000000 acore_server_config-0.3.2/acore_server_config/runtime.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.886959 acore_server_config-0.3.2/acore_server_config/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       58 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/tests/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      362 2023-06-19 16:31:24.000000 acore_server_config-0.3.2/acore_server_config/tests/dummy_config.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      447 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/tests/helper.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2169 2023-06-19 16:26:34.000000 acore_server_config-0.3.2/acore_server_config/tests/mock_aws.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.887480 acore_server_config-0.3.2/acore_server_config/vendor/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       25 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/vendor/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3572 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/acore_server_config/vendor/pytest_cov_helper.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.883964 acore_server_config-0.3.2/acore_server_config.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     5203 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1180 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      285 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       20 2023-06-22 04:14:39.000000 acore_server_config-0.3.2/acore_server_config.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)     2814 2023-06-22 03:52:00.000000 acore_server_config-0.3.2/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      102 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/requirements-automation.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      353 2023-06-18 01:00:08.000000 acore_server_config-0.3.2/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      563 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      188 2023-06-19 16:26:45.000000 acore_server_config-0.3.2/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      171 2023-06-22 03:48:21.000000 acore_server_config-0.3.2/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-06-22 04:14:39.888126 acore_server_config-0.3.2/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7568 2023-06-17 19:58:08.000000 acore_server_config-0.3.2/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-06-22 04:14:39.887625 acore_server_config-0.3.2/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      501 2023-06-19 16:53:17.000000 acore_server_config-0.3.2/tests/test_api.py
```

### Comparing `acore_server_config-0.3.1/AUTHORS.rst` & `acore_server_config-0.3.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/LICENSE.txt` & `acore_server_config-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/PKG-INFO` & `acore_server_config-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore_server_config
-Version: 0.3.1
+Version: 0.3.2
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.3.1/README.rst` & `acore_server_config-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config/config/define/main.py` & `acore_server_config-0.3.2/acore_server_config/config/define/main.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config/config/define/server.py` & `acore_server_config-0.3.2/acore_server_config/config/define/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,17 @@
     Per Game Server configuration.
 
     :param id: Server id, the naming convention is ``${env_name}-${server_name}``
     :param db_admin_password: the RDS admin password, we need this password
         to create the database user.
     :param db_username: the database user for game server
     :param db_password: the database password for game server
+    :param authserver_conf: custom config for authserver.conf
+    :param worldserver_conf: custom config for worldserver.conf
+    :param mod_lua_engine_conf: custom config for mod_LuaEngine.conf
     """
 
     id: T.Optional[str] = dataclasses.field(default=None)
     db_admin_password: T.Optional[str] = dataclasses.field(default=None)
     db_username: T.Optional[str] = dataclasses.field(default=None)
     db_password: T.Optional[str] = dataclasses.field(default=None)
     authserver_conf: T.Dict[str, str] = dataclasses.field(default_factory=dict)
```

### Comparing `acore_server_config-0.3.1/acore_server_config/config/init.py` & `acore_server_config-0.3.2/acore_server_config/config/init.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config/config/loader.py` & `acore_server_config-0.3.2/acore_server_config/config/loader.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config/in_ec2.py` & `acore_server_config-0.3.2/acore_server_config/in_ec2.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config/paths.py` & `acore_server_config-0.3.2/acore_server_config/paths.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config/tests/mock_aws.py` & `acore_server_config-0.3.2/acore_server_config/tests/mock_aws.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config/vendor/pytest_cov_helper.py` & `acore_server_config-0.3.2/acore_server_config/vendor/pytest_cov_helper.py`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/acore_server_config.egg-info/PKG-INFO` & `acore_server_config-0.3.2/acore_server_config.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: acore-server-config
-Version: 0.3.1
+Version: 0.3.2
 Summary: Azerothcore World of Warcraft fleet of Servers configuration management.
 Home-page: https://github.com/MacHu-GWU/acore_server_config-project
-Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.1#downloads
+Download-URL: https://pypi.python.org/pypi/acore_server_config/0.3.2#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: husanhe@gmail.com
 License: MIT
 Platform: Windows
 Platform: MacOS
```

### Comparing `acore_server_config-0.3.1/acore_server_config.egg-info/SOURCES.txt` & `acore_server_config-0.3.2/acore_server_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/release-history.rst` & `acore_server_config-0.3.2/release-history.rst`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.3.2 (2023-06-21)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Minor Improvements**
+
+- add support to use this in AWS CodeBuild and AWS Lambda.
+
+
 0.3.1 (2023-06-19)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - Create two new API ``acore_server_config.api.Ec2ConfigLoader``, ``acore_server_config.api.ConfigLoader`` to replace ``acore_server_config.api.get_server``. The old api remains for backward compatibility until the next major release.
```

### Comparing `acore_server_config-0.3.1/requirements-doc.txt` & `acore_server_config-0.3.2/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `acore_server_config-0.3.1/setup.py` & `acore_server_config-0.3.2/setup.py`

 * *Files identical despite different names*

