# Comparing `tmp/airavata-django-portal-commons-1.0.0.tar.gz` & `tmp/airavata-django-portal-commons-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airavata-django-portal-commons-1.0.0.tar", last modified: Tue Nov  1 16:43:50 2022, max compression
+gzip compressed data, was "airavata-django-portal-commons-1.0.1.tar", last modified: Thu Jun 22 15:20:06 2023, max compression
```

## Comparing `airavata-django-portal-commons-1.0.0.tar` & `airavata-django-portal-commons-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2022-11-01 16:43:50.397736 airavata-django-portal-commons-1.0.0/
--rw-r--r--   0 machrist (661619347) wheel        (0)        0 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/MANIFEST.in
--rw-r--r--   0 machrist (661619347) wheel        (0)      142 2022-11-01 16:43:50.397795 airavata-django-portal-commons-1.0.0/PKG-INFO
--rw-r--r--   0 machrist (661619347) wheel        (0)     2688 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/README.md
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2022-11-01 16:43:50.396457 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/
--rw-r--r--   0 machrist (661619347) wheel        (0)        0 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/__init__.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2022-11-01 16:43:50.397561 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/dynamic_apps/
--rw-r--r--   0 machrist (661619347) wheel        (0)     2099 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/dynamic_apps/__init__.py
--rw-r--r--   0 machrist (661619347) wheel        (0)     4129 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/dynamic_apps/context_processors.py
--rw-r--r--   0 machrist (661619347) wheel        (0)      484 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/dynamic_apps/urls.py
-drwxr-xr-x   0 machrist (661619347) wheel        (0)        0 2022-11-01 16:43:50.397000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons.egg-info/
--rw-r--r--   0 machrist (661619347) wheel        (0)      142 2022-11-01 16:43:50.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons.egg-info/PKG-INFO
--rw-r--r--   0 machrist (661619347) wheel        (0)      541 2022-11-01 16:43:50.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons.egg-info/SOURCES.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)        1 2022-11-01 16:43:50.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons.egg-info/dependency_links.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)       15 2022-11-01 16:43:50.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons.egg-info/requires.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)       31 2022-11-01 16:43:50.000000 airavata-django-portal-commons-1.0.0/airavata_django_portal_commons.egg-info/top_level.txt
--rw-r--r--   0 machrist (661619347) wheel        (0)      104 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/pyproject.toml
--rw-r--r--   0 machrist (661619347) wheel        (0)      273 2022-11-01 16:43:50.398034 airavata-django-portal-commons-1.0.0/setup.cfg
--rw-r--r--   0 machrist (661619347) wheel        (0)       38 2022-11-01 16:43:13.000000 airavata-django-portal-commons-1.0.0/setup.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.128146 airavata-django-portal-commons-1.0.1/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/MANIFEST.in
+-rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 15:20:06.128276 airavata-django-portal-commons-1.0.1/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542     3111 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/README.md
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.126188 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/__init__.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.127938 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/
+-rw-r--r--   0 machrist (661619347) 1014028542     2094 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     4129 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/context_processors.py
+-rw-r--r--   0 machrist (661619347) 1014028542      484 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/urls.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.127123 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/
+-rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542      541 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 machrist (661619347) 1014028542        1 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       34 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/requires.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       31 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/top_level.txt
+-rw-r--r--   0 machrist (661619347) 1014028542      104 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/pyproject.toml
+-rw-r--r--   0 machrist (661619347) 1014028542      374 2023-06-22 15:20:06.128699 airavata-django-portal-commons-1.0.1/setup.cfg
+-rw-r--r--   0 machrist (661619347) 1014028542       38 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/setup.py
```

### Comparing `airavata-django-portal-commons-1.0.0/README.md` & `airavata-django-portal-commons-1.0.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,21 @@
 dynamic_apps.load(INSTALLED_APPS)
 
 # (Optional) merge WEBPACK_LOADER settings from custom Django apps
 settings_module = sys.modules[__name__]
 dynamic_apps.merge_settings(settings_module)
 ```
 
+- Note: if the dynamic Django app uses WEBPACK_LOADER, keep in mind that it is
+  important that the version of
+  [django-webpack-loader](https://github.com/django-webpack/django-webpack-loader)
+  and the version of webpack-bundle-tracker be compatible. If you're using
+  django-webpack-loader prior to version 1.0 then a known good pair of versions
+  is django-webpack-loader==0.6.0 and webpack-bundle-tracker==0.4.3.
+
 2. Also add
    `'airavata_django_portal_commons.dynamic_apps.context_processors.custom_app_registry'`
    to the context_processors list:
 
 ```python
 TEMPLATES = [
     {
@@ -87,15 +94,15 @@
 
    ```
    cd /tmp/
    git clone /path/to/airavata-django-portal-commons/ -b $VERSION
    cd airavata-django-portal-commons
    python3 -m venv venv
    source venv/bin/activate
-   python3 -m pip install --upgrade build
+   python3 -m pip install --upgrade pip build
    python3 -m build
    ```
 
 5. Push to pypi.org. Optionally can push to test.pypi.org. See
    <https://packaging.python.org/tutorials/packaging-projects/> for more info.
 
    ```
```

### Comparing `airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/dynamic_apps/__init__.py` & `airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from importlib import import_module
+from importlib_metadata import entry_points
 
-from pkg_resources import iter_entry_points
 
 # AppConfig instances from custom Django apps
 CUSTOM_DJANGO_APPS = []
 
 logger = logging.getLogger(__name__)
 
 
 def load(installed_apps, entry_point_group="airavata.djangoapp"):
-    for entry_point in iter_entry_points(group=entry_point_group):
+    for entry_point in entry_points(group=entry_point_group):
         custom_app_class = entry_point.load()
         custom_app_instance = custom_app_class(
             entry_point.name, import_module(entry_point.module_name)
         )
         CUSTOM_DJANGO_APPS.append(custom_app_instance)
         # Create path to AppConfig class (otherwise the ready() method doesn't get
         # called)
```

### Comparing `airavata-django-portal-commons-1.0.0/airavata_django_portal_commons/dynamic_apps/context_processors.py` & `airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/context_processors.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-commons-1.0.0/airavata_django_portal_commons.egg-info/SOURCES.txt` & `airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

