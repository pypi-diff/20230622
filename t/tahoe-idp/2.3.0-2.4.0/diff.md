# Comparing `tmp/tahoe-idp-2.3.0.tar.gz` & `tmp/tahoe-idp-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoe-idp-2.3.0.tar", last modified: Wed Apr 19 21:14:05 2023, max compression
+gzip compressed data, was "tahoe-idp-2.4.0.tar", last modified: Thu Jun 22 20:40:46 2023, max compression
```

## Comparing `tahoe-idp-2.3.0.tar` & `tahoe-idp-2.4.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:14:05.976522 tahoe-idp-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-19 21:14:05.976522 tahoe-idp-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-19 21:14:05.976522 tahoe-idp-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:14:05.972522 tahoe-idp-2.3.0/tahoe_idp/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/magiclink_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/magiclink_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/magiclink_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/magiclink_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:14:05.976522 tahoe-idp-2.3.0/tahoe_idp/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/migrations/0002_allow_null_redirect_url.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:14:05.976522 tahoe-idp-2.3.0/tahoe_idp/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/settings/cms_production.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/settings/common_production.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/settings/lms_production.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-19 21:13:51.000000 tahoe-idp-2.3.0/tahoe_idp/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 21:14:05.976522 tahoe-idp-2.3.0/tahoe_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-04-19 21:14:05.000000 tahoe-idp-2.3.0/tahoe_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-04-19 21:14:05.000000 tahoe-idp-2.3.0/tahoe_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 21:14:05.000000 tahoe-idp-2.3.0/tahoe_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-19 21:14:05.000000 tahoe-idp-2.3.0/tahoe_idp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 21:14:05.000000 tahoe-idp-2.3.0/tahoe_idp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:40:46.279657 tahoe-idp-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-22 20:40:46.279657 tahoe-idp-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7655 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-22 20:40:46.279657 tahoe-idp-2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:40:46.275657 tahoe-idp-2.4.0/tahoe_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/magiclink_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/magiclink_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/magiclink_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/magiclink_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:40:46.279657 tahoe-idp-2.4.0/tahoe_idp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/migrations/0002_allow_null_redirect_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/receivers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:40:46.279657 tahoe-idp-2.4.0/tahoe_idp/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/settings/cms_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/settings/common_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/settings/lms_production.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-22 20:40:36.000000 tahoe-idp-2.4.0/tahoe_idp/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:40:46.279657 tahoe-idp-2.4.0/tahoe_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-06-22 20:40:46.000000 tahoe-idp-2.4.0/tahoe_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-22 20:40:46.000000 tahoe-idp-2.4.0/tahoe_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:40:46.000000 tahoe-idp-2.4.0/tahoe_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 20:40:46.000000 tahoe-idp-2.4.0/tahoe_idp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 20:40:46.000000 tahoe-idp-2.4.0/tahoe_idp.egg-info/top_level.txt
```

### Comparing `tahoe-idp-2.3.0/LICENSE` & `tahoe-idp-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/PKG-INFO` & `tahoe-idp-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoe-idp
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tahoe IdP user authentication package for Tahoe.
 Home-page: https://github.com/appsembler/tahoe-idp
 Author: Appsembler
 Author-email: ops@appsembler.com
 Project-URL: Bug Tracker, https://github.com/appsembler/tahoe-idp/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `tahoe-idp-2.3.0/README.md` & `tahoe-idp-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/setup.cfg` & `tahoe-idp-2.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/setup.py` & `tahoe-idp-2.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/api.py` & `tahoe-idp-2.4.0/tahoe_idp/api.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/backend.py` & `tahoe-idp-2.4.0/tahoe_idp/backend.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/helpers.py` & `tahoe-idp-2.4.0/tahoe_idp/helpers.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/magiclink_backends.py` & `tahoe-idp-2.4.0/tahoe_idp/magiclink_backends.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/magiclink_helpers.py` & `tahoe-idp-2.4.0/tahoe_idp/magiclink_helpers.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/magiclink_views.py` & `tahoe-idp-2.4.0/tahoe_idp/magiclink_views.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/migrations/0001_initial.py` & `tahoe-idp-2.4.0/tahoe_idp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/models.py` & `tahoe-idp-2.4.0/tahoe_idp/models.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/permissions.py` & `tahoe-idp-2.4.0/tahoe_idp/permissions.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp/settings/common_production.py` & `tahoe-idp-2.4.0/tahoe_idp/settings/common_production.py`

 * *Files identical despite different names*

### Comparing `tahoe-idp-2.3.0/tahoe_idp.egg-info/PKG-INFO` & `tahoe-idp-2.4.0/tahoe_idp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoe-idp
-Version: 2.3.0
+Version: 2.4.0
 Summary: Tahoe IdP user authentication package for Tahoe.
 Home-page: https://github.com/appsembler/tahoe-idp
 Author: Appsembler
 Author-email: ops@appsembler.com
 Project-URL: Bug Tracker, https://github.com/appsembler/tahoe-idp/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `tahoe-idp-2.3.0/tahoe_idp.egg-info/SOURCES.txt` & `tahoe-idp-2.4.0/tahoe_idp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 tahoe_idp/helpers.py
 tahoe_idp/magiclink_backends.py
 tahoe_idp/magiclink_helpers.py
 tahoe_idp/magiclink_utils.py
 tahoe_idp/magiclink_views.py
 tahoe_idp/models.py
 tahoe_idp/permissions.py
+tahoe_idp/receivers.py
 tahoe_idp/urls.py
 tahoe_idp.egg-info/PKG-INFO
 tahoe_idp.egg-info/SOURCES.txt
 tahoe_idp.egg-info/dependency_links.txt
 tahoe_idp.egg-info/entry_points.txt
 tahoe_idp.egg-info/top_level.txt
 tahoe_idp/migrations/0001_initial.py
```

