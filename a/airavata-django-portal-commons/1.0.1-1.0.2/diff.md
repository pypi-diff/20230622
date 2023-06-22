# Comparing `tmp/airavata-django-portal-commons-1.0.1.tar.gz` & `tmp/airavata-django-portal-commons-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airavata-django-portal-commons-1.0.1.tar", last modified: Thu Jun 22 15:20:06 2023, max compression
+gzip compressed data, was "airavata-django-portal-commons-1.0.2.tar", last modified: Thu Jun 22 16:56:27 2023, max compression
```

## Comparing `airavata-django-portal-commons-1.0.1.tar` & `airavata-django-portal-commons-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.128146 airavata-django-portal-commons-1.0.1/
--rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/MANIFEST.in
--rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 15:20:06.128276 airavata-django-portal-commons-1.0.1/PKG-INFO
--rw-r--r--   0 machrist (661619347) 1014028542     3111 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/README.md
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.126188 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/
--rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/__init__.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.127938 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/
--rw-r--r--   0 machrist (661619347) 1014028542     2094 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/__init__.py
--rw-r--r--   0 machrist (661619347) 1014028542     4129 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/context_processors.py
--rw-r--r--   0 machrist (661619347) 1014028542      484 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/urls.py
-drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 15:20:06.127123 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/
--rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/PKG-INFO
--rw-r--r--   0 machrist (661619347) 1014028542      541 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/SOURCES.txt
--rw-r--r--   0 machrist (661619347) 1014028542        1 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/dependency_links.txt
--rw-r--r--   0 machrist (661619347) 1014028542       34 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/requires.txt
--rw-r--r--   0 machrist (661619347) 1014028542       31 2023-06-22 15:20:06.000000 airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/top_level.txt
--rw-r--r--   0 machrist (661619347) 1014028542      104 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/pyproject.toml
--rw-r--r--   0 machrist (661619347) 1014028542      374 2023-06-22 15:20:06.128699 airavata-django-portal-commons-1.0.1/setup.cfg
--rw-r--r--   0 machrist (661619347) 1014028542       38 2023-06-22 15:16:25.000000 airavata-django-portal-commons-1.0.1/setup.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.537011 airavata-django-portal-commons-1.0.2/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/MANIFEST.in
+-rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 16:56:27.537073 airavata-django-portal-commons-1.0.2/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542     3111 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/README.md
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.535435 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/
+-rw-r--r--   0 machrist (661619347) 1014028542        0 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/__init__.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.536779 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/
+-rw-r--r--   0 machrist (661619347) 1014028542     2094 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/__init__.py
+-rw-r--r--   0 machrist (661619347) 1014028542     4129 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/context_processors.py
+-rw-r--r--   0 machrist (661619347) 1014028542      484 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/urls.py
+drwxr-xr-x   0 machrist (661619347) 1014028542        0 2023-06-22 16:56:27.536113 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/
+-rw-r--r--   0 machrist (661619347) 1014028542     3294 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/PKG-INFO
+-rw-r--r--   0 machrist (661619347) 1014028542      541 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 machrist (661619347) 1014028542        1 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       26 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/requires.txt
+-rw-r--r--   0 machrist (661619347) 1014028542       31 2023-06-22 16:56:27.000000 airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/top_level.txt
+-rw-r--r--   0 machrist (661619347) 1014028542      104 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/pyproject.toml
+-rw-r--r--   0 machrist (661619347) 1014028542      362 2023-06-22 16:56:27.537352 airavata-django-portal-commons-1.0.2/setup.cfg
+-rw-r--r--   0 machrist (661619347) 1014028542       38 2023-06-22 16:55:49.000000 airavata-django-portal-commons-1.0.2/setup.py
```

### Comparing `airavata-django-portal-commons-1.0.1/PKG-INFO` & `airavata-django-portal-commons-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-commons
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities for working with dynamically loaded Django apps.
 Description-Content-Type: text/markdown
 
 # Airavata Django Portal Commons
 
 Utilities for working with dynamically loaded Django apps.
```

### Comparing `airavata-django-portal-commons-1.0.1/README.md` & `airavata-django-portal-commons-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/__init__.py` & `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/__init__.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-commons-1.0.1/airavata_django_portal_commons/dynamic_apps/context_processors.py` & `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons/dynamic_apps/context_processors.py`

 * *Files identical despite different names*

### Comparing `airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/PKG-INFO` & `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airavata-django-portal-commons
-Version: 1.0.1
+Version: 1.0.2
 Summary: Utilities for working with dynamically loaded Django apps.
 Description-Content-Type: text/markdown
 
 # Airavata Django Portal Commons
 
 Utilities for working with dynamically loaded Django apps.
```

### Comparing `airavata-django-portal-commons-1.0.1/airavata_django_portal_commons.egg-info/SOURCES.txt` & `airavata-django-portal-commons-1.0.2/airavata_django_portal_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

