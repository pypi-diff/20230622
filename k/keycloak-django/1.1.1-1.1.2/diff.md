# Comparing `tmp/keycloak_django-1.1.1.tar.gz` & `tmp/keycloak_django-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak_django-1.1.1.tar", max compression
+gzip compressed data, was "keycloak_django-1.1.2.tar", max compression
```

## Comparing `keycloak_django-1.1.1.tar` & `keycloak_django-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.1.1/CHANGELOG.md
--rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.1.1/LICENSE
--rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.1.1/README.md
--rwxr-xr-x   0        0        0      971 2023-05-28 07:12:37.133036 keycloak_django-1.1.1/pyproject.toml
--rwxr-xr-x   0        0        0      114 2023-05-28 07:12:29.552892 keycloak_django-1.1.1/src/keycloak_django/__init__.py
--rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.1.1/src/keycloak_django/admin.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.1.1/src/keycloak_django/api/__init__.py
--rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.1.1/src/keycloak_django/api/apps.py
--rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.1.1/src/keycloak_django/api/urls.py
--rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.1.1/src/keycloak_django/api/viewsets.py
--rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.1.1/src/keycloak_django/apps.py
--rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.1.1/src/keycloak_django/authentication.py
--rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.1.1/src/keycloak_django/groups_permissions.py
--rwxr-xr-x   0        0        0    17614 2023-05-28 06:27:35.153651 keycloak_django-1.1.1/src/keycloak_django/keycloak.py
--rwxr-xr-x   0        0        0     7737 2023-05-28 06:57:38.923654 keycloak_django-1.1.1/src/keycloak_django/middleware.py
--rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.1.1/src/keycloak_django/migrations/0001_initial.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.1.1/src/keycloak_django/migrations/__init__.py
--rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.1.1/src/keycloak_django/models.py
--rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.1.1/src/keycloak_django/security.py
--rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.1.1/src/keycloak_django/services/__init__.py
--rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.1.1/src/keycloak_django/services/client_repository.py
--rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.1.1/src/keycloak_django/services/permission_repository.py
--rwxr-xr-x   0        0        0     3662 2023-05-28 07:12:21.675989 keycloak_django-1.1.1/src/keycloak_django/services/realm_repository.py
--rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.1.1/src/keycloak_django/services/role_repository.py
--rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.1.1/src/keycloak_django/services/user_repository.py
--rwxr-xr-x   0        0        0     1576 2023-05-28 06:57:34.486798 keycloak_django-1.1.1/src/keycloak_django/tools.py
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0       56 2023-05-05 04:43:24.284910 keycloak_django-1.1.2/CHANGELOG.md
+-rwxr-xr-x   0        0        0     1104 2023-05-05 04:43:24.575787 keycloak_django-1.1.2/LICENSE
+-rwxr-xr-x   0        0        0      129 2023-05-05 04:43:24.678171 keycloak_django-1.1.2/README.md
+-rwxr-xr-x   0        0        0      971 2023-06-21 23:07:58.558823 keycloak_django-1.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0      114 2023-06-21 23:08:15.136372 keycloak_django-1.1.2/src/keycloak_django/__init__.py
+-rwxr-xr-x   0        0        0       63 2023-05-05 04:43:24.707873 keycloak_django-1.1.2/src/keycloak_django/admin.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:24.828523 keycloak_django-1.1.2/src/keycloak_django/api/__init__.py
+-rwxr-xr-x   0        0        0      118 2023-05-05 04:43:24.739495 keycloak_django-1.1.2/src/keycloak_django/api/apps.py
+-rwxr-xr-x   0        0        0      173 2023-05-05 04:43:24.767709 keycloak_django-1.1.2/src/keycloak_django/api/urls.py
+-rwxr-xr-x   0        0        0      998 2023-05-25 02:02:25.421462 keycloak_django-1.1.2/src/keycloak_django/api/viewsets.py
+-rwxr-xr-x   0        0        0      162 2023-05-05 04:43:24.861582 keycloak_django-1.1.2/src/keycloak_django/apps.py
+-rwxr-xr-x   0        0        0      684 2023-05-05 04:43:24.891943 keycloak_django-1.1.2/src/keycloak_django/authentication.py
+-rwxr-xr-x   0        0        0     1049 2023-05-05 04:43:24.920503 keycloak_django-1.1.2/src/keycloak_django/groups_permissions.py
+-rwxr-xr-x   0        0        0    17614 2023-05-28 06:27:35.153651 keycloak_django-1.1.2/src/keycloak_django/keycloak.py
+-rwxr-xr-x   0        0        0     8042 2023-06-21 23:07:16.431582 keycloak_django-1.1.2/src/keycloak_django/middleware.py
+-rwxr-xr-x   0        0        0     2811 2023-05-25 02:01:41.767172 keycloak_django-1.1.2/src/keycloak_django/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.053856 keycloak_django-1.1.2/src/keycloak_django/migrations/__init__.py
+-rwxr-xr-x   0        0        0    11522 2023-05-25 02:03:59.088722 keycloak_django-1.1.2/src/keycloak_django/models.py
+-rwxr-xr-x   0        0        0     2899 2023-05-05 20:21:37.936996 keycloak_django-1.1.2/src/keycloak_django/security.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 04:43:25.302771 keycloak_django-1.1.2/src/keycloak_django/services/__init__.py
+-rwxr-xr-x   0        0        0     2083 2023-05-19 01:52:31.887873 keycloak_django-1.1.2/src/keycloak_django/services/client_repository.py
+-rwxr-xr-x   0        0        0     4315 2023-05-05 04:43:25.187851 keycloak_django-1.1.2/src/keycloak_django/services/permission_repository.py
+-rwxr-xr-x   0        0        0     3662 2023-05-28 07:12:21.675989 keycloak_django-1.1.2/src/keycloak_django/services/realm_repository.py
+-rwxr-xr-x   0        0        0     2005 2023-05-05 04:43:25.243733 keycloak_django-1.1.2/src/keycloak_django/services/role_repository.py
+-rwxr-xr-x   0        0        0     4322 2023-05-19 01:32:23.950903 keycloak_django-1.1.2/src/keycloak_django/services/user_repository.py
+-rwxr-xr-x   0        0        0     1906 2023-06-21 23:07:38.723575 keycloak_django-1.1.2/src/keycloak_django/tools.py
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 keycloak_django-1.1.2/PKG-INFO
```

### Comparing `keycloak_django-1.1.1/LICENSE` & `keycloak_django-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/pyproject.toml` & `keycloak_django-1.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "keycloak-django"
-version = "1.1.1"
+version = "1.1.2"
 description = "keycloak-django is Python package providing access to custom apps"
 authors = ["David Campos <dcampos@istmocenter.com>", "Arnoldo Paz <apaz@istmocenter.com>"]
 readme = "README.md"
 keywords = ["keycloak", "openid", "oidc"]
 classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `keycloak_django-1.1.1/src/keycloak_django/api/viewsets.py` & `keycloak_django-1.1.2/src/keycloak_django/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/authentication.py` & `keycloak_django-1.1.2/src/keycloak_django/authentication.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/groups_permissions.py` & `keycloak_django-1.1.2/src/keycloak_django/groups_permissions.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/keycloak.py` & `keycloak_django-1.1.2/src/keycloak_django/keycloak.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/middleware.py` & `keycloak_django-1.1.2/src/keycloak_django/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,39 +90,50 @@
             return JsonResponse({"detail": AuthenticationFailed.default_detail},
                                 status=AuthenticationFailed.status_code)
 
         UserModel = get_user_model()
 
         try:
             user = UserModel.objects.get(id=user_info['sub'])
-            user = set_profile(user=user, groups=user_groups,
-                               permissions=user_permissions, user_info=user_info)
+            user = set_profile(
+                user=user,
+                groups=user_groups,
+                permissions=user_permissions,
+                user_info=user_info,
+                attributes_fillable=self.attributes_fillable
+            )
 
             login(request, user)
         except UserModel.DoesNotExist:
             payload = {}
             for config in self.attributes_fillable:
                 if isinstance(config, tuple):
                     payload[config[0]] = user_info[config[1]]
                     continue
                 payload[config] = user_info[config]
             payload['id'] = user_info['sub']
             user = None
             if self.create_user_if_not_exist:
                 user = UserModel(**payload)
-                user = set_profile(user=user, groups=user_groups,
-                                   permissions=user_permissions, user_info=user_info)
+                user = set_profile(
+                    user=user,
+                    groups=user_groups,
+                    permissions=user_permissions,
+                    user_info=user_info,
+                    attributes_fillable=self.attributes_fillable
+                )
             if user:
                 login(request, user)
             else:
                 User = get_user_model_keycloak()
                 user = User(**payload)
                 user.groups = user_groups
                 user.permissions = user_permissions
-                fill_user_model_keycloak(user=user, user_info=user_info)
+                fill_user_model_keycloak(
+                    user=user, user_info=user_info, attributes_fillable=self.attributes_fillable)
 
         request.user = user
 
         if self.default_access == "DENY" and (not user_permissions or not user_groups):
             # User Permission Denied
             return JsonResponse({"detail": PermissionDenied.default_detail},
                                 status=PermissionDenied.status_code)
```

### Comparing `keycloak_django-1.1.1/src/keycloak_django/migrations/0001_initial.py` & `keycloak_django-1.1.2/src/keycloak_django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/models.py` & `keycloak_django-1.1.2/src/keycloak_django/models.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/security.py` & `keycloak_django-1.1.2/src/keycloak_django/security.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/services/client_repository.py` & `keycloak_django-1.1.2/src/keycloak_django/services/client_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/services/permission_repository.py` & `keycloak_django-1.1.2/src/keycloak_django/services/permission_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/services/realm_repository.py` & `keycloak_django-1.1.2/src/keycloak_django/services/realm_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/services/role_repository.py` & `keycloak_django-1.1.2/src/keycloak_django/services/role_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/services/user_repository.py` & `keycloak_django-1.1.2/src/keycloak_django/services/user_repository.py`

 * *Files identical despite different names*

### Comparing `keycloak_django-1.1.1/src/keycloak_django/tools.py` & `keycloak_django-1.1.2/src/keycloak_django/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,34 +2,40 @@
 from django.conf import settings
 from django.contrib.auth.models import Permission, Group
 from django.apps import apps as django_apps
 from django.core.exceptions import ImproperlyConfigured
 from django.utils import timezone
 
 
-def set_profile(user, groups: List[Group], permissions: List[Permission], user_info=None):
+def set_profile(user, groups: List[Group], permissions: List[Permission], user_info=None, attributes_fillable: List[str] = []):
     user.last_login = timezone.now()
     user.groups = groups
     user.permissions = permissions
     if user_info:
-        user = fill_user_model_keycloak(user=user, user_info=user_info)
+        user = fill_user_model_keycloak(
+            user=user, user_info=user_info, attributes_fillable=attributes_fillable)
     user.save()
     return user
 
 
-def fill_user_model_keycloak(user, user_info):
+def fill_user_model_keycloak(user, user_info, attributes_fillable):
     """
     Return the User Keycloak model that is active in this project.
     """
-    if hasattr(user, 'is_superuser'):
-        user.is_superuser = user_info.get('is_superuser', False)
-    if hasattr(user, 'is_staff'):
-        user.is_staff = user_info.get('is_staff', True)
-    if hasattr(user, 'realm_name'):
-        user.realm_name = user_info.get('realm_name', 'master')
+    # if hasattr(user, 'is_superuser'):
+    #     user.is_superuser = user_info.get('is_superuser', False)
+    # if hasattr(user, 'is_staff'):
+    #     user.is_staff = user_info.get('is_staff', True)
+    # if hasattr(user, 'realm_name'):
+    #     user.realm_name = user_info.get('realm_name', 'master')
+    for config in attributes_fillable:
+        if isinstance(config, tuple):
+            setattr(user, config[0], user_info[config[1]])
+            continue
+        setattr(user, config, user_info[config])
     return user
 
 
 def get_user_model_keycloak():
     """
     Return the User Keycloak model that is active in this project.
     """
```

### Comparing `keycloak_django-1.1.1/PKG-INFO` & `keycloak_django-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-django
-Version: 1.1.1
+Version: 1.1.2
 Summary: keycloak-django is Python package providing access to custom apps
 Keywords: keycloak,openid,oidc
 Author: David Campos
 Author-email: dcampos@istmocenter.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

