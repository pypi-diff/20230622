# Comparing `tmp/django_hmac_authentication-1.3.0.tar.gz` & `tmp/django_hmac_authentication-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-1.3.0.tar", last modified: Thu Jun 15 10:14:48 2023, max compression
+gzip compressed data, was "django_hmac_authentication-1.3.1.tar", last modified: Wed Jun 21 22:57:41 2023, max compression
```

## Comparing `django_hmac_authentication-1.3.0.tar` & `django_hmac_authentication-1.3.1.tar`

### file list

```diff
@@ -1,63 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.174998 django_hmac_authentication-1.3.0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-15 10:14:48.174998 django_hmac_authentication-1.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5810 2023-06-13 03:07:01.000000 django_hmac_authentication-1.3.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      722 2023-06-15 10:09:43.000000 django_hmac_authentication-1.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-15 10:14:48.174998 django_hmac_authentication-1.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.154998 django_hmac_authentication-1.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/
--rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-15 10:09:43.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/aes.py
--rw-rw-rw-   0 root         (0) root         (0)     4485 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/client_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/padding.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.162998 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6348 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2283 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-15 10:14:48.000000 django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/accounts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-05 01:42:47.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/accounts/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-06-05 01:42:47.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/models.py
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-06-05 01:42:47.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/accounts/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.166998 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3741 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1025 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      421 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_django_project/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1834 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/example_python_client.py
--rwxrwxrwx   0 root         (0) root         (0)      678 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/example_django_project/manage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-15 10:14:48.170998 django_hmac_authentication-1.3.0/src/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-15 10:14:10.000000 django_hmac_authentication-1.3.0/src/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-06-06 00:34:30.000000 django_hmac_authentication-1.3.0/src/tests/factories.py
--rw-rw-rw-   0 root         (0) root         (0)    15731 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.0/src/tests/test_authentication_api_key_secret.py
--rw-rw-rw-   0 root         (0) root         (0)     1502 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/tests/test_hmac_authorization_header_parsing.py
--rw-rw-rw-   0 root         (0) root         (0)     2356 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.0/src/tests/test_mgmt_cmd_create_hmac_for_user.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/tests/test_padding.py
--rw-rw-rw-   0 root         (0) root         (0)     3773 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.0/src/tests/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.0/src/tests/test_view_create_api_key_secret.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5810 2023-06-13 03:07:01.000000 django_hmac_authentication-1.3.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      832 2023-06-21 22:51:16.000000 django_hmac_authentication-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.190257 django_hmac_authentication-1.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.194257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/
+-rw-rw-rw-   0 root         (0) root         (0)       54 2023-06-21 22:51:16.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-06 00:58:59.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4485 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/client_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1520 2023-06-15 10:03:50.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 22:57:04.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 22:57:04.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-21 22:57:04.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-06-05 22:40:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/padding.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-05 23:55:52.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-21 22:57:41.198257 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6348 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1232 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-21 22:57:41.000000 django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/top_level.txt
```

### Comparing `django_hmac_authentication-1.3.0/LICENSE` & `django_hmac_authentication-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/PKG-INFO` & `django_hmac_authentication-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hmac_authentication
-Version: 1.3.0
+Version: 1.3.1
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

### Comparing `django_hmac_authentication-1.3.0/README.md` & `django_hmac_authentication-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/pyproject.toml` & `django_hmac_authentication-1.3.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["django_hmac_authentication*"]
+namespaces = false
+
 [project]
 name = "django_hmac_authentication"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Harisankar Krishna Swamy", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/aes.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/aes.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/exceptions.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/models.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/models.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/server_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication/views.py` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-1.3.0/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-1.3.1/src/django_hmac_authentication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-hmac-authentication
-Version: 1.3.0
+Version: 1.3.1
 Summary: Django HMAC authentication using shared secret
 Author-email: Harisankar Krishna Swamy <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

