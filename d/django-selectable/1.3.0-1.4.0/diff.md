# Comparing `tmp/django-selectable-1.3.0.tar.gz` & `tmp/django-selectable-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-selectable-1.3.0.tar", last modified: Fri Jun 26 19:04:05 2020, max compression
+gzip compressed data, was "django-selectable-1.4.0.tar", last modified: Thu Jun 22 11:33:57 2023, max compression
```

## Comparing `django-selectable-1.3.0.tar` & `django-selectable-1.4.0.tar`

### file list

```diff
@@ -1,93 +1,92 @@
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.375334 django-selectable-1.3.0/
--rw-r--r--   0 ddinicola   (501) staff       (20)      471 2020-06-26 18:54:42.000000 django-selectable-1.3.0/AUTHORS.txt
--rw-r--r--   0 ddinicola   (501) staff       (20)     1390 2020-06-26 18:17:13.000000 django-selectable-1.3.0/LICENSE.txt
--rw-r--r--   0 ddinicola   (501) staff       (20)      176 2020-06-26 18:17:13.000000 django-selectable-1.3.0/MANIFEST.in
--rw-r--r--   0 ddinicola   (501) staff       (20)     4641 2020-06-26 19:04:05.375554 django-selectable-1.3.0/PKG-INFO
--rw-r--r--   0 ddinicola   (501) staff       (20)     2957 2020-06-26 18:54:42.000000 django-selectable-1.3.0/README.rst
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.358085 django-selectable-1.3.0/django_selectable.egg-info/
--rw-r--r--   0 ddinicola   (501) staff       (20)     4641 2020-06-26 19:04:05.000000 django-selectable-1.3.0/django_selectable.egg-info/PKG-INFO
--rw-r--r--   0 ddinicola   (501) staff       (20)     2032 2020-06-26 19:04:05.000000 django-selectable-1.3.0/django_selectable.egg-info/SOURCES.txt
--rw-r--r--   0 ddinicola   (501) staff       (20)        1 2020-06-26 19:04:05.000000 django-selectable-1.3.0/django_selectable.egg-info/dependency_links.txt
--rw-r--r--   0 ddinicola   (501) staff       (20)        1 2020-06-26 18:21:46.000000 django-selectable-1.3.0/django_selectable.egg-info/not-zip-safe
--rw-r--r--   0 ddinicola   (501) staff       (20)       11 2020-06-26 19:04:05.000000 django-selectable-1.3.0/django_selectable.egg-info/top_level.txt
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.361067 django-selectable-1.3.0/selectable/
--rw-r--r--   0 ddinicola   (501) staff       (20)      143 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/__init__.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      232 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/apps.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     5027 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/base.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      205 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/compat.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     1995 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/decorators.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      315 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/exceptions.py
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.362215 django-selectable-1.3.0/selectable/forms/
--rw-r--r--   0 ddinicola   (501) staff       (20)      113 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/forms/__init__.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     1353 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/forms/base.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     4359 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/forms/fields.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     8532 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/forms/widgets.py
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.353089 django-selectable-1.3.0/selectable/locale/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.350784 django-selectable-1.3.0/selectable/locale/cs/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.362992 django-selectable-1.3.0/selectable/locale/cs/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      602 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)      857 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.351097 django-selectable-1.3.0/selectable/locale/de/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.363616 django-selectable-1.3.0/selectable/locale/de/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      697 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)     1000 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.351426 django-selectable-1.3.0/selectable/locale/en/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.364279 django-selectable-1.3.0/selectable/locale/en/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      378 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)      764 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.351770 django-selectable-1.3.0/selectable/locale/es/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.364766 django-selectable-1.3.0/selectable/locale/es/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      721 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)      951 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.351999 django-selectable-1.3.0/selectable/locale/fr/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.365477 django-selectable-1.3.0/selectable/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      725 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)      997 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.352248 django-selectable-1.3.0/selectable/locale/it/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.366045 django-selectable-1.3.0/selectable/locale/it/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      594 2020-06-26 18:29:49.000000 django-selectable-1.3.0/selectable/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)      914 2020-06-26 18:29:49.000000 django-selectable-1.3.0/selectable/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.352634 django-selectable-1.3.0/selectable/locale/pl/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.366750 django-selectable-1.3.0/selectable/locale/pl/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      761 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)     1025 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.352884 django-selectable-1.3.0/selectable/locale/pt_BR/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.367283 django-selectable-1.3.0/selectable/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      733 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)      963 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.353277 django-selectable-1.3.0/selectable/locale/zh_CN/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.367875 django-selectable-1.3.0/selectable/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 ddinicola   (501) staff       (20)      709 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 ddinicola   (501) staff       (20)      990 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0 ddinicola   (501) staff       (20)      251 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/models.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     1275 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/registry.py
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.353575 django-selectable-1.3.0/selectable/static/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.353864 django-selectable-1.3.0/selectable/static/selectable/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.368231 django-selectable-1.3.0/selectable/static/selectable/css/
--rw-r--r--   0 ddinicola   (501) staff       (20)     1186 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/static/selectable/css/dj.selectable.css
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.368636 django-selectable-1.3.0/selectable/static/selectable/js/
--rw-r--r--   0 ddinicola   (501) staff       (20)    16114 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/static/selectable/js/jquery.dj.selectable.js
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.354249 django-selectable-1.3.0/selectable/templates/
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.369362 django-selectable-1.3.0/selectable/templates/selectable/
--rw-r--r--   0 ddinicola   (501) staff       (20)      135 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/templates/selectable/jquery-css.html
--rw-r--r--   0 ddinicola   (501) staff       (20)      227 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/templates/selectable/jquery-js.html
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.369842 django-selectable-1.3.0/selectable/templatetags/
--rwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/templatetags/__init__.py
--rwxr-xr-x   0 ddinicola   (501) staff       (20)      376 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/templatetags/selectable_tags.py
-drwxr-xr-x   0 ddinicola   (501) staff       (20)        0 2020-06-26 19:04:05.374961 django-selectable-1.3.0/selectable/tests/
--rw-r--r--   0 ddinicola   (501) staff       (20)      795 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/__init__.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     2599 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/base.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     4546 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_base.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     2936 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_decorators.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     4941 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_fields.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     2661 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_forms.py
--rw-r--r--   0 ddinicola   (501) staff       (20)    19620 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_functional.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     4775 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_templatetags.py
--rw-r--r--   0 ddinicola   (501) staff       (20)     3436 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_views.py
--rw-r--r--   0 ddinicola   (501) staff       (20)    18898 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/test_widgets.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      241 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/urls.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      225 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/tests/views.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      158 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/urls.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      307 2020-06-26 18:17:13.000000 django-selectable-1.3.0/selectable/views.py
--rw-r--r--   0 ddinicola   (501) staff       (20)      206 2020-06-26 19:04:05.376232 django-selectable-1.3.0/setup.cfg
--rwxr-xr-x   0 ddinicola   (501) staff       (20)     1603 2020-06-26 18:54:42.000000 django-selectable-1.3.0/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.501737 django-selectable-1.4.0/
+-rw-r--r--   0 jojo       (501) staff       (20)      471 2023-06-22 08:51:53.000000 django-selectable-1.4.0/AUTHORS.txt
+-rw-r--r--   0 jojo       (501) staff       (20)     1390 2023-06-22 08:51:53.000000 django-selectable-1.4.0/LICENSE.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      176 2023-06-22 08:51:53.000000 django-selectable-1.4.0/MANIFEST.in
+-rw-r--r--   0 jojo       (501) staff       (20)     3873 2023-06-22 11:33:57.502048 django-selectable-1.4.0/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2956 2023-06-22 09:14:53.000000 django-selectable-1.4.0/README.rst
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.447153 django-selectable-1.4.0/django_selectable.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)     3873 2023-06-22 11:33:57.000000 django-selectable-1.4.0/django_selectable.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2011 2023-06-22 11:33:57.000000 django-selectable-1.4.0/django_selectable.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-22 11:33:57.000000 django-selectable-1.4.0/django_selectable.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-06-22 08:56:53.000000 django-selectable-1.4.0/django_selectable.egg-info/not-zip-safe
+-rw-r--r--   0 jojo       (501) staff       (20)       11 2023-06-22 11:33:57.000000 django-selectable-1.4.0/django_selectable.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.455272 django-selectable-1.4.0/selectable/
+-rw-r--r--   0 jojo       (501) staff       (20)      143 2023-06-22 11:33:37.000000 django-selectable-1.4.0/selectable/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)      233 2023-06-22 09:05:17.000000 django-selectable-1.4.0/selectable/apps.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5031 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/base.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2000 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/decorators.py
+-rw-r--r--   0 jojo       (501) staff       (20)      315 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/exceptions.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.458806 django-selectable-1.4.0/selectable/forms/
+-rw-r--r--   0 jojo       (501) staff       (20)      137 2023-06-22 09:03:59.000000 django-selectable-1.4.0/selectable/forms/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1383 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/forms/base.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4374 2023-06-22 09:06:58.000000 django-selectable-1.4.0/selectable/forms/fields.py
+-rw-r--r--   0 jojo       (501) staff       (20)     8611 2023-06-22 09:05:18.000000 django-selectable-1.4.0/selectable/forms/widgets.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.437586 django-selectable-1.4.0/selectable/locale/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.434346 django-selectable-1.4.0/selectable/locale/cs/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.460600 django-selectable-1.4.0/selectable/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      602 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)      857 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.434656 django-selectable-1.4.0/selectable/locale/de/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.462446 django-selectable-1.4.0/selectable/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      697 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)     1000 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.434965 django-selectable-1.4.0/selectable/locale/en/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.464057 django-selectable-1.4.0/selectable/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      378 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)      764 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.435272 django-selectable-1.4.0/selectable/locale/es/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.465919 django-selectable-1.4.0/selectable/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      721 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)      951 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.435648 django-selectable-1.4.0/selectable/locale/fr/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.468186 django-selectable-1.4.0/selectable/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      725 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)      997 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.436088 django-selectable-1.4.0/selectable/locale/it/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.470129 django-selectable-1.4.0/selectable/locale/it/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      594 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)      914 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.436676 django-selectable-1.4.0/selectable/locale/pl/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.471915 django-selectable-1.4.0/selectable/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      761 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)     1025 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.437156 django-selectable-1.4.0/selectable/locale/pt_BR/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.476256 django-selectable-1.4.0/selectable/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      733 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)      963 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.437795 django-selectable-1.4.0/selectable/locale/zh_CN/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.478235 django-selectable-1.4.0/selectable/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 jojo       (501) staff       (20)      709 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 jojo       (501) staff       (20)      990 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0 jojo       (501) staff       (20)      250 2023-06-22 09:05:17.000000 django-selectable-1.4.0/selectable/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1265 2023-06-22 09:06:58.000000 django-selectable-1.4.0/selectable/registry.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.438269 django-selectable-1.4.0/selectable/static/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.438795 django-selectable-1.4.0/selectable/static/selectable/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.479007 django-selectable-1.4.0/selectable/static/selectable/css/
+-rw-r--r--   0 jojo       (501) staff       (20)     1186 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/static/selectable/css/dj.selectable.css
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.479844 django-selectable-1.4.0/selectable/static/selectable/js/
+-rw-r--r--   0 jojo       (501) staff       (20)    16114 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/static/selectable/js/jquery.dj.selectable.js
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.439276 django-selectable-1.4.0/selectable/templates/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.481854 django-selectable-1.4.0/selectable/templates/selectable/
+-rw-r--r--   0 jojo       (501) staff       (20)      135 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/templates/selectable/jquery-css.html
+-rw-r--r--   0 jojo       (501) staff       (20)      227 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/templates/selectable/jquery-js.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.483106 django-selectable-1.4.0/selectable/templatetags/
+-rwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/templatetags/__init__.py
+-rwxr-xr-x   0 jojo       (501) staff       (20)      376 2023-06-22 09:05:18.000000 django-selectable-1.4.0/selectable/templatetags/selectable_tags.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-06-22 11:33:57.500728 django-selectable-1.4.0/selectable/tests/
+-rw-r--r--   0 jojo       (501) staff       (20)      794 2023-06-22 09:05:18.000000 django-selectable-1.4.0/selectable/tests/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2630 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/tests/base.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4549 2023-06-22 09:05:18.000000 django-selectable-1.4.0/selectable/tests/test_base.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2932 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/tests/test_decorators.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5074 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/tests/test_fields.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2653 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/tests/test_forms.py
+-rw-r--r--   0 jojo       (501) staff       (20)    20094 2023-06-22 09:06:58.000000 django-selectable-1.4.0/selectable/tests/test_functional.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4985 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/tests/test_templatetags.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3428 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/tests/test_views.py
+-rw-r--r--   0 jojo       (501) staff       (20)    18922 2023-06-22 09:08:02.000000 django-selectable-1.4.0/selectable/tests/test_widgets.py
+-rw-r--r--   0 jojo       (501) staff       (20)      219 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/tests/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      225 2023-06-22 08:51:53.000000 django-selectable-1.4.0/selectable/tests/views.py
+-rw-r--r--   0 jojo       (501) staff       (20)      160 2023-06-22 09:05:20.000000 django-selectable-1.4.0/selectable/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      305 2023-06-22 09:05:18.000000 django-selectable-1.4.0/selectable/views.py
+-rw-r--r--   0 jojo       (501) staff       (20)      206 2023-06-22 11:33:57.502926 django-selectable-1.4.0/setup.cfg
+-rwxr-xr-x   0 jojo       (501) staff       (20)     1490 2023-06-22 11:33:22.000000 django-selectable-1.4.0/setup.py
```

### Comparing `django-selectable-1.3.0/LICENSE.txt` & `django-selectable-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/PKG-INFO` & `django-selectable-1.4.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,108 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-selectable
-Version: 1.3.0
+Version: 1.4.0
 Summary: Auto-complete selection widgets using Django and jQuery UI.
 Home-page: https://github.com/mlavin/django-selectable
 Author: Mark Lavin
 Author-email: markdlavin@gmail.com
 License: BSD
-Description: django-selectable
-        ===================
-        
-        Tools and widgets for using/creating auto-complete selection widgets using Django and jQuery UI.
-        
-        .. image:: https://travis-ci.org/mlavin/django-selectable.svg?branch=master
-            :target: https://travis-ci.org/mlavin/django-selectable
-        
-        .. image:: https://codecov.io/github/mlavin/django-selectable/coverage.svg?branch=master
-            :target: https://codecov.io/github/mlavin/django-selectable?branch=master
-        
-        
-        .. note::
-        
-            This project is looking for additional maintainers to help with Django/jQuery compatibility
-            issues as well as addressing support issues/questions. If you are looking to help out
-            on this project and take a look at the open
-            `help-wanted <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Ahelp-wanted>`_
-            or `question <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Aquestion>`_
-            and see if you can contribute a fix. Be bold! If you want to take a larger role on
-            the project, please reach out on the
-            `mailing list <http://groups.google.com/group/django-selectable>`_. I'm happy to work
-            with you to get you going on an issue.
-        
-        
-        Features
-        -----------------------------------
-        
-        - Works with the latest jQuery UI Autocomplete library
-        - Auto-discovery/registration pattern for defining lookups
-        
-        
-        Installation Requirements
-        -----------------------------------
-        
-        - Python 3.6+
-        - `Django <http://www.djangoproject.com/>`_ >= 1.11
-        - `jQuery <http://jquery.com/>`_ >= 1.9, < 3.0
-        - `jQuery UI <http://jqueryui.com/>`_ >= 1.10
-        
-        To install::
-        
-            pip install django-selectable
-        
-        Next add `selectable` to your `INSTALLED_APPS` to include the related css/js::
-        
-            INSTALLED_APPS = (
-                'contrib.staticfiles',
-                # Other apps here
-                'selectable',
-            )
-        
-        The jQuery and jQuery UI libraries are not included in the distribution but must be included
-        in your templates. See the example project for an example using these libraries from the
-        Google CDN.
-        
-        Once installed you should add the urls to your root url patterns::
-        
-            urlpatterns = [
-                # Other patterns go here
-                url(r'^selectable/', include('selectable.urls')),
-            ]
-        
-        
-        Documentation
-        -----------------------------------
-        
-        Documentation for django-selectable is available on `Read The Docs <http://django-selectable.readthedocs.io/en/latest/>`_.
-        
-        
-        Additional Help/Support
-        -----------------------------------
-        
-        You can find additional help or support on the mailing list: http://groups.google.com/group/django-selectable
-        
-        
-        Contributing
-        --------------------------------------
-        
-        If you think you've found a bug or are interested in contributing to this project
-        check out our `contributing guide <http://readthedocs.org/docs/django-selectable/en/latest/contribute.html>`_.
-        
-        If you are interested in translating django-selectable into your native language
-        you can join the `Transifex project <https://www.transifex.com/projects/p/django-selectable/>`_.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE.txt
+License-File: AUTHORS.txt
+
+django-selectable
+===================
+
+Tools and widgets for using/creating auto-complete selection widgets using Django and jQuery UI.
+
+.. image:: https://travis-ci.org/mlavin/django-selectable.svg?branch=master
+    :target: https://travis-ci.org/mlavin/django-selectable
+
+.. image:: https://codecov.io/github/mlavin/django-selectable/coverage.svg?branch=master
+    :target: https://codecov.io/github/mlavin/django-selectable?branch=master
+
+
+.. note::
+
+    This project is looking for additional maintainers to help with Django/jQuery compatibility
+    issues as well as addressing support issues/questions. If you are looking to help out
+    on this project and take a look at the open
+    `help-wanted <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Ahelp-wanted>`_
+    or `question <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Aquestion>`_
+    and see if you can contribute a fix. Be bold! If you want to take a larger role on
+    the project, please reach out on the
+    `mailing list <http://groups.google.com/group/django-selectable>`_. I'm happy to work
+    with you to get you going on an issue.
+
+
+Features
+-----------------------------------
+
+- Works with the latest jQuery UI Autocomplete library
+- Auto-discovery/registration pattern for defining lookups
+
+
+Installation Requirements
+-----------------------------------
+
+- Python 3.9+
+- `Django <http://www.djangoproject.com/>`_ >= 3.2
+- `jQuery <http://jquery.com/>`_ >= 1.9, < 3.0
+- `jQuery UI <http://jqueryui.com/>`_ >= 1.10
+
+To install::
+
+    pip install django-selectable
+
+Next add `selectable` to your `INSTALLED_APPS` to include the related css/js::
+
+    INSTALLED_APPS = (
+        'contrib.staticfiles',
+        # Other apps here
+        'selectable',
+    )
+
+The jQuery and jQuery UI libraries are not included in the distribution but must be included
+in your templates. See the example project for an example using these libraries from the
+Google CDN.
+
+Once installed you should add the urls to your root url patterns::
+
+    urlpatterns = [
+        # Other patterns go here
+        url(r'^selectable/', include('selectable.urls')),
+    ]
+
+
+Documentation
+-----------------------------------
+
+Documentation for django-selectable is available on `Read The Docs <http://django-selectable.readthedocs.io/en/latest/>`_.
+
+
+Additional Help/Support
+-----------------------------------
+
+You can find additional help or support on the mailing list: http://groups.google.com/group/django-selectable
+
+
+Contributing
+--------------------------------------
+
+If you think you've found a bug or are interested in contributing to this project
+check out our `contributing guide <http://readthedocs.org/docs/django-selectable/en/latest/contribute.html>`_.
+
+If you are interested in translating django-selectable into your native language
+you can join the `Transifex project <https://www.transifex.com/projects/p/django-selectable/>`_.
```

### Comparing `django-selectable-1.3.0/README.rst` & `django-selectable-1.4.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 - Works with the latest jQuery UI Autocomplete library
 - Auto-discovery/registration pattern for defining lookups
 
 
 Installation Requirements
 -----------------------------------
 
-- Python 3.6+
-- `Django <http://www.djangoproject.com/>`_ >= 1.11
+- Python 3.9+
+- `Django <http://www.djangoproject.com/>`_ >= 3.2
 - `jQuery <http://jquery.com/>`_ >= 1.9, < 3.0
 - `jQuery UI <http://jqueryui.com/>`_ >= 1.10
 
 To install::
 
     pip install django-selectable
```

### Comparing `django-selectable-1.3.0/django_selectable.egg-info/PKG-INFO` & `django-selectable-1.4.0/django_selectable.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,110 +1,108 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: django-selectable
-Version: 1.3.0
+Version: 1.4.0
 Summary: Auto-complete selection widgets using Django and jQuery UI.
 Home-page: https://github.com/mlavin/django-selectable
 Author: Mark Lavin
 Author-email: markdlavin@gmail.com
 License: BSD
-Description: django-selectable
-        ===================
-        
-        Tools and widgets for using/creating auto-complete selection widgets using Django and jQuery UI.
-        
-        .. image:: https://travis-ci.org/mlavin/django-selectable.svg?branch=master
-            :target: https://travis-ci.org/mlavin/django-selectable
-        
-        .. image:: https://codecov.io/github/mlavin/django-selectable/coverage.svg?branch=master
-            :target: https://codecov.io/github/mlavin/django-selectable?branch=master
-        
-        
-        .. note::
-        
-            This project is looking for additional maintainers to help with Django/jQuery compatibility
-            issues as well as addressing support issues/questions. If you are looking to help out
-            on this project and take a look at the open
-            `help-wanted <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Ahelp-wanted>`_
-            or `question <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Aquestion>`_
-            and see if you can contribute a fix. Be bold! If you want to take a larger role on
-            the project, please reach out on the
-            `mailing list <http://groups.google.com/group/django-selectable>`_. I'm happy to work
-            with you to get you going on an issue.
-        
-        
-        Features
-        -----------------------------------
-        
-        - Works with the latest jQuery UI Autocomplete library
-        - Auto-discovery/registration pattern for defining lookups
-        
-        
-        Installation Requirements
-        -----------------------------------
-        
-        - Python 3.6+
-        - `Django <http://www.djangoproject.com/>`_ >= 1.11
-        - `jQuery <http://jquery.com/>`_ >= 1.9, < 3.0
-        - `jQuery UI <http://jqueryui.com/>`_ >= 1.10
-        
-        To install::
-        
-            pip install django-selectable
-        
-        Next add `selectable` to your `INSTALLED_APPS` to include the related css/js::
-        
-            INSTALLED_APPS = (
-                'contrib.staticfiles',
-                # Other apps here
-                'selectable',
-            )
-        
-        The jQuery and jQuery UI libraries are not included in the distribution but must be included
-        in your templates. See the example project for an example using these libraries from the
-        Google CDN.
-        
-        Once installed you should add the urls to your root url patterns::
-        
-            urlpatterns = [
-                # Other patterns go here
-                url(r'^selectable/', include('selectable.urls')),
-            ]
-        
-        
-        Documentation
-        -----------------------------------
-        
-        Documentation for django-selectable is available on `Read The Docs <http://django-selectable.readthedocs.io/en/latest/>`_.
-        
-        
-        Additional Help/Support
-        -----------------------------------
-        
-        You can find additional help or support on the mailing list: http://groups.google.com/group/django-selectable
-        
-        
-        Contributing
-        --------------------------------------
-        
-        If you think you've found a bug or are interested in contributing to this project
-        check out our `contributing guide <http://readthedocs.org/docs/django-selectable/en/latest/contribute.html>`_.
-        
-        If you are interested in translating django-selectable into your native language
-        you can join the `Transifex project <https://www.transifex.com/projects/p/django-selectable/>`_.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+License-File: LICENSE.txt
+License-File: AUTHORS.txt
+
+django-selectable
+===================
+
+Tools and widgets for using/creating auto-complete selection widgets using Django and jQuery UI.
+
+.. image:: https://travis-ci.org/mlavin/django-selectable.svg?branch=master
+    :target: https://travis-ci.org/mlavin/django-selectable
+
+.. image:: https://codecov.io/github/mlavin/django-selectable/coverage.svg?branch=master
+    :target: https://codecov.io/github/mlavin/django-selectable?branch=master
+
+
+.. note::
+
+    This project is looking for additional maintainers to help with Django/jQuery compatibility
+    issues as well as addressing support issues/questions. If you are looking to help out
+    on this project and take a look at the open
+    `help-wanted <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Ahelp-wanted>`_
+    or `question <https://github.com/mlavin/django-selectable/issues?q=is%3Aissue+is%3Aopen+label%3Aquestion>`_
+    and see if you can contribute a fix. Be bold! If you want to take a larger role on
+    the project, please reach out on the
+    `mailing list <http://groups.google.com/group/django-selectable>`_. I'm happy to work
+    with you to get you going on an issue.
+
+
+Features
+-----------------------------------
+
+- Works with the latest jQuery UI Autocomplete library
+- Auto-discovery/registration pattern for defining lookups
+
+
+Installation Requirements
+-----------------------------------
+
+- Python 3.9+
+- `Django <http://www.djangoproject.com/>`_ >= 3.2
+- `jQuery <http://jquery.com/>`_ >= 1.9, < 3.0
+- `jQuery UI <http://jqueryui.com/>`_ >= 1.10
+
+To install::
+
+    pip install django-selectable
+
+Next add `selectable` to your `INSTALLED_APPS` to include the related css/js::
+
+    INSTALLED_APPS = (
+        'contrib.staticfiles',
+        # Other apps here
+        'selectable',
+    )
+
+The jQuery and jQuery UI libraries are not included in the distribution but must be included
+in your templates. See the example project for an example using these libraries from the
+Google CDN.
+
+Once installed you should add the urls to your root url patterns::
+
+    urlpatterns = [
+        # Other patterns go here
+        url(r'^selectable/', include('selectable.urls')),
+    ]
+
+
+Documentation
+-----------------------------------
+
+Documentation for django-selectable is available on `Read The Docs <http://django-selectable.readthedocs.io/en/latest/>`_.
+
+
+Additional Help/Support
+-----------------------------------
+
+You can find additional help or support on the mailing list: http://groups.google.com/group/django-selectable
+
+
+Contributing
+--------------------------------------
+
+If you think you've found a bug or are interested in contributing to this project
+check out our `contributing guide <http://readthedocs.org/docs/django-selectable/en/latest/contribute.html>`_.
+
+If you are interested in translating django-selectable into your native language
+you can join the `Transifex project <https://www.transifex.com/projects/p/django-selectable/>`_.
```

### Comparing `django-selectable-1.3.0/django_selectable.egg-info/SOURCES.txt` & `django-selectable-1.4.0/django_selectable.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 django_selectable.egg-info/SOURCES.txt
 django_selectable.egg-info/dependency_links.txt
 django_selectable.egg-info/not-zip-safe
 django_selectable.egg-info/top_level.txt
 selectable/__init__.py
 selectable/apps.py
 selectable/base.py
-selectable/compat.py
 selectable/decorators.py
 selectable/exceptions.py
 selectable/models.py
 selectable/registry.py
 selectable/urls.py
 selectable/views.py
 selectable/forms/__init__.py
```

### Comparing `django-selectable-1.3.0/selectable/base.py` & `django-selectable-1.4.0/selectable/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 "Base classes for lookup creation."
 import operator
 import re
 from functools import reduce
 
 from django.conf import settings
-from django.core.paginator import Paginator, InvalidPage, EmptyPage
+from django.core.paginator import EmptyPage, InvalidPage, Paginator
+from django.db.models import Model, Q
 from django.http import JsonResponse
-from django.db.models import Q, Model
 from django.urls import reverse
 from django.utils.encoding import smart_str
 from django.utils.html import conditional_escape
 from django.utils.translation import gettext as _
 
 from .forms import BaseLookupForm
 
 __all__ = (
-    'LookupBase',
-    'ModelLookup',
+    "LookupBase",
+    "ModelLookup",
 )
 
 
-class LookupBase():
+class LookupBase:
     "Base class for all django-selectable lookups."
 
     form = BaseLookupForm
     response = JsonResponse
 
     def _name(cls):
-        app_name = cls.__module__.split('.')[-2].lower()
+        app_name = cls.__module__.split(".")[-2].lower()
         class_name = cls.__name__.lower()
-        name = '%s-%s' % (app_name, class_name)
+        name = "%s-%s" % (app_name, class_name)
         return name
+
     name = classmethod(_name)
 
     def split_term(self, term):
         """
         Split searching term into array of subterms
         that will be searched separately.
         """
         return term.split()
 
     def _url(cls):
-        return reverse('selectable-lookup', args=[cls.name()])
+        return reverse("selectable-lookup", args=[cls.name()])
+
     url = classmethod(_url)
 
     def get_query(self, request, term):
         return []
 
     def get_item_label(self, item):
         return smart_str(item)
@@ -56,68 +58,68 @@
     def get_item_value(self, item):
         return smart_str(item)
 
     def get_item(self, value):
         return value
 
     def create_item(self, value):
-        raise NotImplemented()
+        raise NotImplementedError()
 
     def format_item(self, item):
         "Construct result dictionary for the match item."
         result = {
-            'id': self.get_item_id(item),
-            'value': self.get_item_value(item),
-            'label': self.get_item_label(item),
+            "id": self.get_item_id(item),
+            "value": self.get_item_value(item),
+            "label": self.get_item_label(item),
         }
         for key in settings.SELECTABLE_ESCAPED_KEYS:
             if key in result:
                 result[key] = conditional_escape(result[key])
         return result
 
     def paginate_results(self, results, options):
         "Return a django.core.paginator.Page of results."
-        limit = options.get('limit', settings.SELECTABLE_MAX_LIMIT)
+        limit = options.get("limit", settings.SELECTABLE_MAX_LIMIT)
         paginator = Paginator(results, limit)
-        page = options.get('page', 1)
+        page = options.get("page", 1)
         try:
             results = paginator.page(page)
         except (EmptyPage, InvalidPage):
             results = paginator.page(paginator.num_pages)
         return results
 
     def results(self, request):
         "Match results to given term and return the serialized HttpResponse."
         results = {}
         form = self.form(request.GET)
         if form.is_valid():
             options = form.cleaned_data
-            term = options.get('term', '')
+            term = options.get("term", "")
             raw_data = self.get_query(request, term)
             results = self.format_results(raw_data, options)
         return self.response(results)
 
     def format_results(self, raw_data, options):
-        '''
+        """
         Returns a python structure that later gets serialized.
         raw_data
             full list of objects matching the search term
         options
             a dictionary of the given options
-        '''
+        """
         page_data = self.paginate_results(raw_data, options)
         results = {}
         meta = options.copy()
-        meta['more'] = _('Show more results')
+        meta["more"] = _("Show more results")
         if page_data and page_data.has_next():
-            meta['next_page'] = page_data.next_page_number()
+            meta["next_page"] = page_data.next_page_number()
         if page_data and page_data.has_previous():
-            meta['prev_page'] = page_data.previous_page_number()
-        results['data'] = [self.format_item(item) for item in page_data.object_list]
-        results['meta'] = meta
+            meta["prev_page"] = page_data.previous_page_number()
+        results["data"] = [self.format_item(item) for item in page_data.object_list]
+        results["meta"] = meta
         return results
 
 
 class ModelLookup(LookupBase):
     "Lookup class for easily defining lookups based on Django models."
 
     model = None
@@ -153,11 +155,11 @@
             except (ValueError, self.model.DoesNotExist):
                 item = None
         return item
 
     def create_item(self, value):
         data = {}
         if self.search_fields:
-            field_name = re.sub(r'__\w+$', '',  self.search_fields[0])
+            field_name = re.sub(r"__\w+$", "", self.search_fields[0])
             if field_name:
                 data = {field_name: value}
         return self.model(**data)
```

### Comparing `django-selectable-1.3.0/selectable/decorators.py` & `django-selectable-1.4.0/selectable/decorators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,65 @@
 "Decorators for additional lookup functionality."
 from functools import wraps
 
 from django.http import HttpResponse, HttpResponseBadRequest, HttpResponseForbidden
 
-
 __all__ = (
-    'ajax_required',
-    'login_required',
-    'staff_member_required',
+    "ajax_required",
+    "login_required",
+    "staff_member_required",
 )
 
 
 def results_decorator(func):
     """
     Helper for constructing simple decorators around Lookup.results.
 
     func is a function which takes a request as the first parameter. If func
     returns an HttpReponse it is returned otherwise the original Lookup.results
     is returned.
     """
+
     # Wrap function to maintian the original doc string, etc
     @wraps(func)
     def decorator(lookup_cls):
         # Construct a class decorator from the original function
         original = lookup_cls.results
+
         def inner(self, request):
             # Wrap lookup_cls.results by first calling func and checking the result
             result = func(request)
             if isinstance(result, HttpResponse):
                 return result
             return original(self, request)
+
         # Replace original lookup_cls.results with wrapped version
         lookup_cls.results = inner
         return lookup_cls
+
     # Return the constructed decorator
     return decorator
 
 
 @results_decorator
 def ajax_required(request):
     "Lookup decorator to require AJAX calls to the lookup view."
     if not request.is_ajax():
         return HttpResponseBadRequest()
 
 
 @results_decorator
 def login_required(request):
     "Lookup decorator to require the user to be authenticated."
-    user = getattr(request, 'user', None)
+    user = getattr(request, "user", None)
     if user is None or not user.is_authenticated:
-        return HttpResponse(status=401) # Unauthorized
+        return HttpResponse(status=401)  # Unauthorized
 
 
 @results_decorator
 def staff_member_required(request):
     "Lookup decorator to require the user is a staff member."
-    user = getattr(request, 'user', None)
+    user = getattr(request, "user", None)
     if user is None or not user.is_authenticated:
-        return HttpResponse(status=401) # Unauthorized
+        return HttpResponse(status=401)  # Unauthorized
     elif not user.is_staff:
         return HttpResponseForbidden()
```

### Comparing `django-selectable-1.3.0/selectable/forms/base.py` & `django-selectable-1.4.0/selectable/forms/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 from importlib import import_module
 
 from django import forms
 from django.conf import settings
 
-
 __all__ = (
-    'BaseLookupForm',
-    'import_lookup_class',
+    "BaseLookupForm",
+    "import_lookup_class",
 )
 
 
 class BaseLookupForm(forms.Form):
     term = forms.CharField(required=False)
     limit = forms.IntegerField(required=False, min_value=1)
     page = forms.IntegerField(required=False, min_value=1)
 
     def clean_limit(self):
         "Ensure given limit is less than default if defined"
-        limit = self.cleaned_data.get('limit', None)
-        if (settings.SELECTABLE_MAX_LIMIT is not None and
-            (not limit or limit > settings.SELECTABLE_MAX_LIMIT)):
+        limit = self.cleaned_data.get("limit", None)
+        if settings.SELECTABLE_MAX_LIMIT is not None and (
+            not limit or limit > settings.SELECTABLE_MAX_LIMIT
+        ):
             limit = settings.SELECTABLE_MAX_LIMIT
         return limit
 
     def clean_page(self):
-        "Return the first page if no page or invalid number is given."
-        return self.cleaned_data.get('page', 1) or 1
+        """
+        Return the first page if no page or invalid number is given.
+        """
+        return self.cleaned_data.get("page", 1) or 1
 
 
 def import_lookup_class(lookup_class):
     """
     Import lookup_class as a dotted base and ensure it extends LookupBase
     """
     from selectable.base import LookupBase
+
     if isinstance(lookup_class, str):
-        mod_str, cls_str = lookup_class.rsplit('.', 1)
+        mod_str, cls_str = lookup_class.rsplit(".", 1)
         mod = import_module(mod_str)
         lookup_class = getattr(mod, cls_str)
     if not issubclass(lookup_class, LookupBase):
-        raise TypeError('lookup_class must extend from selectable.base.LookupBase')
+        raise TypeError("lookup_class must extend from selectable.base.LookupBase")
     return lookup_class
```

### Comparing `django-selectable-1.3.0/selectable/forms/fields.py` & `django-selectable-1.4.0/selectable/forms/fields.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,119 +1,120 @@
 from django import forms
 from django.core.exceptions import ValidationError
 from django.core.validators import EMPTY_VALUES
-from django.utils.translation import gettext_lazy as _
 from django.db.models import Model
+from django.utils.translation import gettext_lazy as _
 
 from selectable.forms.base import import_lookup_class
-from selectable.forms.widgets import AutoCompleteSelectWidget
-from selectable.forms.widgets import AutoCompleteSelectMultipleWidget
+from selectable.forms.widgets import AutoCompleteSelectMultipleWidget, AutoCompleteSelectWidget
 
 __all__ = (
-    'AutoCompleteSelectField',
-    'AutoCompleteSelectMultipleField',
+    "AutoCompleteSelectField",
+    "AutoCompleteSelectMultipleField",
 )
 
 
 def model_vars(obj):
-    fields = dict(
-        (field.name, getattr(obj, field.name))
-        for field in obj._meta.fields
-    )
+    fields = dict((field.name, getattr(obj, field.name)) for field in obj._meta.fields)
     return fields
 
 
 class BaseAutoCompleteField(forms.Field):
-
     def has_changed(self, initial, data):
         "Detects if the data was changed. This is added in 1.6."
         # Always return False if the field is disabled since self.bound_data
         # always uses the initial value in this case.
         if self.disabled:
             return False
         if initial is None and data is None:
             return False
-        if data and not hasattr(data, '__iter__'):
+        if data and not hasattr(data, "__iter__"):
             data = self.widget.decompress(data)
         initial = self.to_python(initial)
         data = self.to_python(data)
-        if hasattr(self, '_coerce'):
+        if hasattr(self, "_coerce"):
             data = self._coerce(data)
         if isinstance(data, Model) and isinstance(initial, Model):
             return model_vars(data) != model_vars(initial)
         else:
             return data != initial
 
 
 class AutoCompleteSelectField(BaseAutoCompleteField):
     widget = AutoCompleteSelectWidget
 
     default_error_messages = {
-        'invalid_choice': _('Select a valid choice. That choice is not one of the available choices.'),
+        "invalid_choice": _(
+            "Select a valid choice. That choice is not one of the available choices."
+        ),
     }
 
     def __init__(self, lookup_class, *args, **kwargs):
         self.lookup_class = import_lookup_class(lookup_class)
-        self.allow_new = kwargs.pop('allow_new', False)
-        self.limit = kwargs.pop('limit', None)
-        widget = kwargs.get('widget', self.widget) or self.widget
+        self.allow_new = kwargs.pop("allow_new", False)
+        self.limit = kwargs.pop("limit", None)
+        widget = kwargs.get("widget", self.widget) or self.widget
         if isinstance(widget, type):
-            kwargs['widget'] = widget(lookup_class, allow_new=self.allow_new, limit=self.limit)
+            kwargs["widget"] = widget(
+                lookup_class, allow_new=self.allow_new, limit=self.limit
+            )
         super().__init__(*args, **kwargs)
 
     def to_python(self, value):
         if value in EMPTY_VALUES:
             return None
         lookup = self.lookup_class()
         if isinstance(value, list):
             # Input comes from an AutoComplete widget. It's two
             # components: text and id
             if len(value) != 2:
-                raise ValidationError(self.error_messages['invalid_choice'])
+                raise ValidationError(self.error_messages["invalid_choice"])
             label, pk = value
             if pk in EMPTY_VALUES:
                 if not self.allow_new:
                     if label:
-                        raise ValidationError(self.error_messages['invalid_choice'])
+                        raise ValidationError(self.error_messages["invalid_choice"])
                     else:
                         return None
                 if label in EMPTY_VALUES:
                     return None
                 value = lookup.create_item(label)
             else:
                 value = lookup.get_item(pk)
                 if value is None:
-                    raise ValidationError(self.error_messages['invalid_choice'])
+                    raise ValidationError(self.error_messages["invalid_choice"])
         else:
             value = lookup.get_item(value)
             if value is None:
-                raise ValidationError(self.error_messages['invalid_choice'])
+                raise ValidationError(self.error_messages["invalid_choice"])
         return value
 
 
 class AutoCompleteSelectMultipleField(BaseAutoCompleteField):
     widget = AutoCompleteSelectMultipleWidget
 
     default_error_messages = {
-        'invalid_choice': _('Select a valid choice. That choice is not one of the available choices.'),
+        "invalid_choice": _(
+            "Select a valid choice. That choice is not one of the available choices."
+        ),
     }
 
     def __init__(self, lookup_class, *args, **kwargs):
         self.lookup_class = import_lookup_class(lookup_class)
-        self.limit = kwargs.pop('limit', None)
-        widget = kwargs.get('widget', self.widget) or self.widget
+        self.limit = kwargs.pop("limit", None)
+        widget = kwargs.get("widget", self.widget) or self.widget
         if isinstance(widget, type):
-            kwargs['widget'] = widget(lookup_class, limit=self.limit)
+            kwargs["widget"] = widget(lookup_class, limit=self.limit)
         super().__init__(*args, **kwargs)
 
     def to_python(self, value):
         if value in EMPTY_VALUES:
             return []
         lookup = self.lookup_class()
         items = []
         for v in value:
             if v not in EMPTY_VALUES:
                 item = lookup.get_item(v)
                 if item is None:
-                    raise ValidationError(self.error_messages['invalid_choice'])
+                    raise ValidationError(self.error_messages["invalid_choice"])
                 items.append(item)
         return items
```

### Comparing `django-selectable-1.3.0/selectable/forms/widgets.py` & `django-selectable-1.4.0/selectable/forms/widgets.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,71 +5,68 @@
 from django.utils.encoding import force_str
 from django.utils.http import urlencode
 
 from selectable import __version__
 from selectable.forms.base import import_lookup_class
 
 __all__ = (
-    'AutoCompleteWidget',
-    'AutoCompleteSelectWidget',
-    'AutoComboboxWidget',
-    'AutoComboboxSelectWidget',
-    'AutoCompleteSelectMultipleWidget',
-    'AutoComboboxSelectMultipleWidget',
+    "AutoCompleteWidget",
+    "AutoCompleteSelectWidget",
+    "AutoComboboxWidget",
+    "AutoComboboxSelectWidget",
+    "AutoCompleteSelectMultipleWidget",
+    "AutoComboboxSelectMultipleWidget",
 )
 
 
-STATIC_PREFIX = '%sselectable/' % settings.STATIC_URL
+STATIC_PREFIX = "%sselectable/" % settings.STATIC_URL
 
 
-class SelectableMediaMixin():
-
-    class Media():
-        css = {
-            'all': ('%scss/dj.selectable.css?v=%s' % (STATIC_PREFIX, __version__),)
-        }
-        js = ('%sjs/jquery.dj.selectable.js?v=%s' % (STATIC_PREFIX, __version__),)
+class SelectableMediaMixin:
+    class Media:
+        css = {"all": ("%scss/dj.selectable.css?v=%s" % (STATIC_PREFIX, __version__),)}
+        js = ("%sjs/jquery.dj.selectable.js?v=%s" % (STATIC_PREFIX, __version__),)
 
 
 class AutoCompleteWidget(forms.TextInput, SelectableMediaMixin):
-
     def __init__(self, lookup_class, *args, **kwargs):
         self.lookup_class = import_lookup_class(lookup_class)
-        self.allow_new = kwargs.pop('allow_new', False)
-        self.qs = kwargs.pop('query_params', {})
-        self.limit = kwargs.pop('limit', None)
+        self.allow_new = kwargs.pop("allow_new", False)
+        self.qs = kwargs.pop("query_params", {})
+        self.limit = kwargs.pop("limit", None)
         super().__init__(*args, **kwargs)
 
     def update_query_parameters(self, qs_dict):
         self.qs.update(qs_dict)
 
     def build_attrs(self, base_attrs, extra_attrs=None):
         attrs = super().build_attrs(base_attrs, extra_attrs)
         url = self.lookup_class.url()
-        if self.limit and 'limit' not in self.qs:
-            self.qs['limit'] = self.limit
+        if self.limit and "limit" not in self.qs:
+            self.qs["limit"] = self.limit
         if self.qs:
-            url = '%s?%s' % (url, urlencode(self.qs))
-        if 'data-selectable-options' in attrs:
-            attrs['data-selectable-options'] = json.dumps(attrs['data-selectable-options'])
-        attrs['data-selectable-url'] = url
-        attrs['data-selectable-type'] = 'text'
-        attrs['data-selectable-allow-new'] = str(self.allow_new).lower()
+            url = "%s?%s" % (url, urlencode(self.qs))
+        if "data-selectable-options" in attrs:
+            attrs["data-selectable-options"] = json.dumps(
+                attrs["data-selectable-options"]
+            )
+        attrs["data-selectable-url"] = url
+        attrs["data-selectable-type"] = "text"
+        attrs["data-selectable-allow-new"] = str(self.allow_new).lower()
         return attrs
 
 
 class SelectableMultiWidget(forms.MultiWidget):
-
     def update_query_parameters(self, qs_dict):
         self.widgets[0].update_query_parameters(qs_dict)
 
     def decompress(self, value):
         if value:
             lookup = self.lookup_class()
-            model = getattr(self.lookup_class, 'model', None)
+            model = getattr(self.lookup_class, "model", None)
             if model and isinstance(value, model):
                 item = value
                 value = lookup.get_item_id(item)
             else:
                 item = lookup.get_item(value)
             item_value = lookup.get_item_value(item)
             return [item_value, value]
@@ -97,24 +94,26 @@
     hidden input to hold the selected id.
     """
 
     primary_widget = None
 
     def __init__(self, lookup_class, *args, **kwargs):
         self.lookup_class = import_lookup_class(lookup_class)
-        self.allow_new = kwargs.pop('allow_new', False)
-        self.limit = kwargs.pop('limit', None)
-        query_params = kwargs.pop('query_params', {})
+        self.allow_new = kwargs.pop("allow_new", False)
+        self.limit = kwargs.pop("limit", None)
+        query_params = kwargs.pop("query_params", {})
         widgets = [
             self.primary_widget(
-                lookup_class, allow_new=self.allow_new,
-                limit=self.limit, query_params=query_params,
-                attrs=kwargs.get('attrs'),
+                lookup_class,
+                allow_new=self.allow_new,
+                limit=self.limit,
+                query_params=query_params,
+                attrs=kwargs.get("attrs"),
             ),
-            forms.HiddenInput(attrs={'data-selectable-type': 'hidden'})
+            forms.HiddenInput(attrs={"data-selectable-type": "hidden"}),
         ]
         super().__init__(widgets, *args, **kwargs)
 
     def value_from_datadict(self, data, files, name):
         value = super().value_from_datadict(data, files, name)
         if not value[1]:
             compatible_postdata = self.get_compatible_postdata(data, name)
@@ -122,65 +121,61 @@
                 value[1] = compatible_postdata
         if not self.allow_new:
             return value[1]
         return value
 
 
 class AutoCompleteSelectWidget(_BaseSingleSelectWidget):
-
     primary_widget = AutoCompleteWidget
 
 
 class AutoComboboxWidget(AutoCompleteWidget, SelectableMediaMixin):
-
     def build_attrs(self, base_attrs, extra_attrs=None):
         attrs = super().build_attrs(base_attrs, extra_attrs)
-        attrs['data-selectable-type'] = 'combobox'
+        attrs["data-selectable-type"] = "combobox"
         return attrs
 
 
 class AutoComboboxSelectWidget(_BaseSingleSelectWidget):
-
     primary_widget = AutoComboboxWidget
 
 
 class LookupMultipleHiddenInput(forms.MultipleHiddenInput):
-
     def __init__(self, lookup_class, *args, **kwargs):
         self.lookup_class = import_lookup_class(lookup_class)
         super().__init__(*args, **kwargs)
 
     def get_context(self, name, value, attrs):
         lookup = self.lookup_class()
         values = self._normalize_value(value)
         values = list(values)  # force evaluation
 
         context = super().get_context(name, values, attrs)
 
         # Now override/add to what super() did:
-        subwidgets = context['widget']['subwidgets']
+        subwidgets = context["widget"]["subwidgets"]
         for widget_ctx, item in zip(subwidgets, values):
             input_value, title = self._lookup_value_and_title(lookup, item)
-            widget_ctx['value'] = input_value  # override what super() did
+            widget_ctx["value"] = input_value  # override what super() did
             if title:
-                widget_ctx['attrs']['title'] = title
+                widget_ctx["attrs"]["title"] = title
         return context
 
     def build_attrs(self, base_attrs, extra_attrs=None):
         attrs = super().build_attrs(base_attrs, extra_attrs)
-        attrs['data-selectable-type'] = 'hidden-multiple'
+        attrs["data-selectable-type"] = "hidden-multiple"
         return attrs
 
     def _normalize_value(self, value):
         if value is None:
             value = []
         return value
 
     def _lookup_value_and_title(self, lookup, v):
-        model = getattr(self.lookup_class, 'model', None)
+        model = getattr(self.lookup_class, "model", None)
         item = None
         if model and isinstance(v, model):
             item = v
             v = lookup.get_item_id(item)
         title = None
         if v:
             item = item or lookup.get_item(v)
@@ -195,52 +190,53 @@
     hidden inputs to hold the selected ids.
     """
 
     primary_widget = None
 
     def __init__(self, lookup_class, *args, **kwargs):
         self.lookup_class = import_lookup_class(lookup_class)
-        self.limit = kwargs.pop('limit', None)
-        position = kwargs.pop('position', 'bottom')
+        self.limit = kwargs.pop("limit", None)
+        position = kwargs.pop("position", "bottom")
         attrs = {
-            'data-selectable-multiple': 'true',
-            'data-selectable-position': position
+            "data-selectable-multiple": "true",
+            "data-selectable-position": position,
         }
-        attrs.update(kwargs.get('attrs', {}))
-        query_params = kwargs.pop('query_params', {})
+        attrs.update(kwargs.get("attrs", {}))
+        query_params = kwargs.pop("query_params", {})
         widgets = [
             self.primary_widget(
-                lookup_class, allow_new=False,
-                limit=self.limit, query_params=query_params, attrs=attrs
+                lookup_class,
+                allow_new=False,
+                limit=self.limit,
+                query_params=query_params,
+                attrs=attrs,
             ),
-            LookupMultipleHiddenInput(lookup_class)
+            LookupMultipleHiddenInput(lookup_class),
         ]
         super().__init__(widgets, *args, **kwargs)
 
     def value_from_datadict(self, data, files, name):
-        value = self.widgets[1].value_from_datadict(data, files, name + '_1')
+        value = self.widgets[1].value_from_datadict(data, files, name + "_1")
         if not value:
             # Fall back to the compatible POST name
             value = self.get_compatible_postdata(data, name)
         return value
 
     def build_attrs(self, base_attrs, extra_attrs=None):
         attrs = super().build_attrs(base_attrs, extra_attrs)
-        if 'required' in attrs:
-            attrs.pop('required')
+        if "required" in attrs:
+            attrs.pop("required")
         return attrs
 
     def render(self, name, value, attrs=None, renderer=None):
-        if value and not hasattr(value, '__iter__'):
+        if value and not hasattr(value, "__iter__"):
             value = [value]
-        value = ['', value]
+        value = ["", value]
         return super().render(name, value, attrs, renderer)
 
 
 class AutoCompleteSelectMultipleWidget(_BaseMultipleSelectWidget):
-
     primary_widget = AutoCompleteWidget
 
 
 class AutoComboboxSelectMultipleWidget(_BaseMultipleSelectWidget):
-
     primary_widget = AutoComboboxWidget
```

### Comparing `django-selectable-1.3.0/selectable/locale/cs/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/cs/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/de/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/de/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/en/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/es/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/es/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/fr/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/fr/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/it/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/it/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/pl/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/pl/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/pt_BR/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/pt_BR/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/zh_CN/LC_MESSAGES/django.mo` & `django-selectable-1.4.0/selectable/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/locale/zh_CN/LC_MESSAGES/django.po` & `django-selectable-1.4.0/selectable/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/registry.py` & `django-selectable-1.4.0/selectable/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from django.utils.encoding import force_str
 from django.utils.module_loading import autodiscover_modules
 
 from selectable.base import LookupBase
-from selectable.exceptions import (LookupAlreadyRegistered, LookupNotRegistered,
-                                   LookupInvalid)
+from selectable.exceptions import LookupAlreadyRegistered, LookupInvalid, LookupNotRegistered
 
 
-class LookupRegistry():
-
+class LookupRegistry:
     def __init__(self):
         self._registry = {}
 
     def validate(self, lookup):
         if not issubclass(lookup, LookupBase):
-            raise LookupInvalid('Registered lookups must inherit from the LookupBase class')
+            raise LookupInvalid(
+                "Registered lookups must inherit from the LookupBase class"
+            )
 
     def register(self, lookup):
         self.validate(lookup)
         name = force_str(lookup.name())
         if name in self._registry:
-            raise LookupAlreadyRegistered('The name %s is already registered' % name)
+            raise LookupAlreadyRegistered("The name %s is already registered" % name)
         self._registry[name] = lookup
 
     def unregister(self, lookup):
         self.validate(lookup)
         name = force_str(lookup.name())
         if name not in self._registry:
-            raise LookupNotRegistered('The name %s is not registered' % name)
+            raise LookupNotRegistered("The name %s is not registered" % name)
         del self._registry[name]
 
     def get(self, key):
         return self._registry.get(key, None)
 
 
 registry = LookupRegistry()
 
 
 def autodiscover():
     # Attempt to import the app's lookups module.
-    autodiscover_modules('lookups', register_to=registry)
+    autodiscover_modules("lookups", register_to=registry)
```

### Comparing `django-selectable-1.3.0/selectable/static/selectable/css/dj.selectable.css` & `django-selectable-1.4.0/selectable/static/selectable/css/dj.selectable.css`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/static/selectable/js/jquery.dj.selectable.js` & `django-selectable-1.4.0/selectable/static/selectable/js/jquery.dj.selectable.js`

 * *Files identical despite different names*

### Comparing `django-selectable-1.3.0/selectable/tests/__init__.py` & `django-selectable-1.4.0/selectable/tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     name = models.CharField(max_length=100)
     description = models.CharField(max_length=100)
 
     def __str__(self):
         return self.name
 
     class Meta:
-        ordering = ['id']
+        ordering = ["id"]
 
 
 class OtherThing(models.Model):
     name = models.CharField(max_length=100)
     thing = models.ForeignKey(Thing, on_delete=models.CASCADE)
 
     def __str__(self):
@@ -29,11 +29,11 @@
 
     def __str__(self):
         return self.name
 
 
 class ThingLookup(ModelLookup):
     model = Thing
-    search_fields = ('name__icontains', )
+    search_fields = ("name__icontains",)
 
 
 registry.register(ThingLookup)
```

### Comparing `django-selectable-1.3.0/selectable/tests/base.py` & `django-selectable-1.4.0/selectable/tests/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 import random
 import string
 from collections import defaultdict
 
-
 from django.test import TestCase, override_settings
 from django.test.html import parse_html
 
-from . import Thing
 from ..base import ModelLookup
+from . import Thing
 
 
 def parsed_inputs(html):
     "Returns a dictionary mapping name --> node of inputs found in the HTML."
     node = parse_html(html)
     inputs = {}
-    for field in [c for c in node.children if c.name == 'input']:
-        name = dict(field.attributes)['name']
+    for field in [c for c in node.children if c.name == "input"]:
+        name = dict(field.attributes)["name"]
         current = inputs.get(name, [])
         current.append(field)
         inputs[name] = current
     return inputs
 
 
-@override_settings(ROOT_URLCONF='selectable.tests.urls')
+@override_settings(ROOT_URLCONF="selectable.tests.urls")
 class BaseSelectableTestCase(TestCase):
-
     def get_random_string(self, length=10):
-        return ''.join(random.choice(string.ascii_letters) for x in range(length))
+        return "".join(random.choice(string.ascii_letters) for x in range(length))
 
     def create_thing(self, data=None):
         data = data or {}
         defaults = {
-            'name': self.get_random_string(),
-            'description': self.get_random_string(),
+            "name": self.get_random_string(),
+            "description": self.get_random_string(),
         }
         defaults.update(data)
         return Thing.objects.create(**defaults)
 
 
 class SimpleModelLookup(ModelLookup):
     model = Thing
-    search_fields = ('name__icontains', )
+    search_fields = ("name__icontains",)
 
 
 def parsed_widget_attributes(widget):
     """
     Get a dictionary-like object containing all HTML attributes
     of the rendered widget.
 
     Lookups on this object raise ValueError if there is more than one attribute
     of the given name in the HTML, and they have different values.
     """
     # For the tests that use this, it generally doesn't matter what the value
     # is, so we supply anything.
-    rendered = widget.render('a_name', 'a_value')
+    rendered = widget.render("a_name", "a_value")
     return AttrMap(rendered)
 
 
-class AttrMap():
+class AttrMap:
     def __init__(self, html):
         dom = parse_html(html)
         self._attrs = defaultdict(set)
         self._build_attr_map(dom)
 
     def _build_attr_map(self, dom):
         for node in _walk_nodes(dom):
             if node.attributes is not None:
-                for (k, v) in node.attributes:
+                for k, v in node.attributes:
                     self._attrs[k].add(v)
 
     def __contains__(self, key):
         return key in self._attrs and len(self._attrs[key]) > 0
 
     def __getitem__(self, key):
         if key not in self:
             raise KeyError(key)
         vals = self._attrs[key]
         if len(vals) > 1:
-            raise ValueError("More than one value for attribute {0}: {1}".
-                             format(key, ", ".join(vals)))
+            raise ValueError(
+                "More than one value for attribute {0}: {1}".format(
+                    key, ", ".join(vals)
+                )
+            )
         else:
             return list(vals)[0]
 
 
 def _walk_nodes(dom):
     yield dom
     for child in dom.children:
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_base.py` & `django-selectable-1.4.0/selectable/tests/test_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,127 +3,129 @@
 from django.utils.safestring import SafeData, mark_safe
 
 from ..base import ModelLookup
 from . import Thing
 from .base import BaseSelectableTestCase, SimpleModelLookup
 
 __all__ = (
-    'ModelLookupTestCase',
-    'MultiFieldLookupTestCase',
-    'LookupEscapingTestCase',
+    "ModelLookupTestCase",
+    "MultiFieldLookupTestCase",
+    "LookupEscapingTestCase",
 )
 
 
 class ModelLookupTestCase(BaseSelectableTestCase):
     lookup_cls = SimpleModelLookup
 
     def get_lookup_instance(self):
         return self.__class__.lookup_cls()
 
     def test_get_name(self):
         name = self.__class__.lookup_cls.name()
-        self.assertEqual(name, 'tests-simplemodellookup')
+        self.assertEqual(name, "tests-simplemodellookup")
 
     def test_get_url(self):
         url = self.__class__.lookup_cls.url()
-        test_url = reverse('selectable-lookup', args=['tests-simplemodellookup'])
+        test_url = reverse("selectable-lookup", args=["tests-simplemodellookup"])
         self.assertEqual(url, test_url)
 
     def test_format_item(self):
         lookup = self.get_lookup_instance()
         thing = Thing()
         item_info = lookup.format_item(thing)
-        self.assertTrue('id' in item_info)
-        self.assertTrue('value' in item_info)
-        self.assertTrue('label' in item_info)
+        self.assertTrue("id" in item_info)
+        self.assertTrue("value" in item_info)
+        self.assertTrue("label" in item_info)
 
     def test_get_query(self):
         lookup = self.get_lookup_instance()
-        thing = self.create_thing(data={'name': 'Thing'})
-        other_thing = self.create_thing(data={'name': 'Other Thing'})
-        qs = lookup.get_query(request=None, term='other')
-        self.assertTrue(thing.pk not in qs.values_list('id', flat=True))
-        self.assertTrue(other_thing.pk in qs.values_list('id', flat=True))
+        thing = self.create_thing(data={"name": "Thing"})
+        other_thing = self.create_thing(data={"name": "Other Thing"})
+        qs = lookup.get_query(request=None, term="other")
+        self.assertTrue(thing.pk not in qs.values_list("id", flat=True))
+        self.assertTrue(other_thing.pk in qs.values_list("id", flat=True))
 
     def test_create_item(self):
         value = self.get_random_string()
         lookup = self.get_lookup_instance()
         thing = lookup.create_item(value)
         self.assertEqual(thing.__class__, Thing)
         self.assertEqual(thing.name, value)
         self.assertFalse(thing.pk)
 
     def test_get_item(self):
         lookup = self.get_lookup_instance()
-        thing = self.create_thing(data={'name': 'Thing'})
+        thing = self.create_thing(data={"name": "Thing"})
         item = lookup.get_item(thing.pk)
         self.assertEqual(thing, item)
 
     def test_format_item_escaping(self):
         "Id, value and label should be escaped."
         lookup = self.get_lookup_instance()
-        thing = self.create_thing(data={'name': 'Thing'})
+        thing = self.create_thing(data={"name": "Thing"})
         item_info = lookup.format_item(thing)
-        self.assertFalse(isinstance(item_info['id'], SafeData))
-        self.assertFalse(isinstance(item_info['value'], SafeData))
-        self.assertTrue(isinstance(item_info['label'], SafeData))
+        self.assertFalse(isinstance(item_info["id"], SafeData))
+        self.assertFalse(isinstance(item_info["value"], SafeData))
+        self.assertTrue(isinstance(item_info["label"], SafeData))
 
 
 class MultiFieldLookup(ModelLookup):
     model = Thing
-    search_fields = ('name__icontains', 'description__icontains', )
+    search_fields = (
+        "name__icontains",
+        "description__icontains",
+    )
 
 
 class MultiFieldLookupTestCase(ModelLookupTestCase):
     lookup_cls = MultiFieldLookup
 
     def test_get_name(self):
         name = self.__class__.lookup_cls.name()
-        self.assertEqual(name, 'tests-multifieldlookup')
+        self.assertEqual(name, "tests-multifieldlookup")
 
     def test_get_url(self):
         url = self.__class__.lookup_cls.url()
-        test_url = reverse('selectable-lookup', args=['tests-multifieldlookup'])
+        test_url = reverse("selectable-lookup", args=["tests-multifieldlookup"])
         self.assertEqual(url, test_url)
 
     def test_description_search(self):
         lookup = self.get_lookup_instance()
-        thing = self.create_thing(data={'description': 'Thing'})
-        other_thing = self.create_thing(data={'description': 'Other Thing'})
-        qs = lookup.get_query(request=None, term='other')
-        self.assertTrue(thing.pk not in qs.values_list('id', flat=True))
-        self.assertTrue(other_thing.pk in qs.values_list('id', flat=True))
+        thing = self.create_thing(data={"description": "Thing"})
+        other_thing = self.create_thing(data={"description": "Other Thing"})
+        qs = lookup.get_query(request=None, term="other")
+        self.assertTrue(thing.pk not in qs.values_list("id", flat=True))
+        self.assertTrue(other_thing.pk in qs.values_list("id", flat=True))
 
 
 class HTMLLookup(ModelLookup):
     model = Thing
-    search_fields = ('name__icontains', )
+    search_fields = ("name__icontains",)
 
 
 class SafeHTMLLookup(ModelLookup):
     model = Thing
-    search_fields = ('name__icontains', )
+    search_fields = ("name__icontains",)
 
     def get_item_label(self, item):
         "Mark label as safe."
         return mark_safe(item.name)
 
 
 class LookupEscapingTestCase(BaseSelectableTestCase):
-
     def test_escape_html(self):
         "HTML should be escaped by default."
         lookup = HTMLLookup()
         bad_name = "<script>alert('hacked');</script>"
         escaped_name = escape(bad_name)
-        thing = self.create_thing(data={'name': bad_name})
+        thing = self.create_thing(data={"name": bad_name})
         item_info = lookup.format_item(thing)
-        self.assertEqual(item_info['label'], escaped_name)
+        self.assertEqual(item_info["label"], escaped_name)
 
     def test_conditional_escape(self):
         "Methods should be able to mark values as safe."
         lookup = SafeHTMLLookup()
         bad_name = "<script>alert('hacked');</script>"
-        escaped_name = escape(bad_name)
-        thing = self.create_thing(data={'name': bad_name})
+        escape(bad_name)
+        thing = self.create_thing(data={"name": bad_name})
         item_info = lookup.format_item(thing)
-        self.assertEqual(item_info['label'], bad_name)
+        self.assertEqual(item_info["label"], bad_name)
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_decorators.py` & `django-selectable-1.4.0/selectable/tests/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from unittest.mock import Mock
 
 from ..decorators import ajax_required, login_required, staff_member_required
 from .base import BaseSelectableTestCase, SimpleModelLookup
 
-
 __all__ = (
-    'AjaxRequiredLookupTestCase',
-    'LoginRequiredLookupTestCase',
-    'StaffRequiredLookupTestCase',
+    "AjaxRequiredLookupTestCase",
+    "LoginRequiredLookupTestCase",
+    "StaffRequiredLookupTestCase",
 )
 
 
 class AjaxRequiredLookupTestCase(BaseSelectableTestCase):
-
     def setUp(self):
         self.lookup = ajax_required(SimpleModelLookup)()
 
     def test_ajax_call(self):
         "Ajax call should yield a successful response."
         request = Mock()
         request.is_ajax = lambda: True
@@ -28,15 +26,14 @@
         request = Mock()
         request.is_ajax = lambda: False
         response = self.lookup.results(request)
         self.assertEqual(response.status_code, 400)
 
 
 class LoginRequiredLookupTestCase(BaseSelectableTestCase):
-
     def setUp(self):
         self.lookup = login_required(SimpleModelLookup)()
 
     def test_authenicated_call(self):
         "Authenicated call should yield a successful response."
         request = Mock()
         user = Mock()
@@ -52,15 +49,14 @@
         user.is_authenticated = False
         request.user = user
         response = self.lookup.results(request)
         self.assertEqual(response.status_code, 401)
 
 
 class StaffRequiredLookupTestCase(BaseSelectableTestCase):
-
     def setUp(self):
         self.lookup = staff_member_required(SimpleModelLookup)()
 
     def test_staff_member_call(self):
         "Staff member call should yield a successful response."
         request = Mock()
         user = Mock()
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_fields.py` & `django-selectable-1.4.0/selectable/tests/test_fields.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,80 +1,83 @@
 from django import forms
 
 from selectable.forms import fields, widgets
 from selectable.tests import ThingLookup
 from selectable.tests.base import BaseSelectableTestCase
 
-
 __all__ = (
-    'AutoCompleteSelectFieldTestCase',
-    'AutoCompleteSelectMultipleFieldTestCase',
+    "AutoCompleteSelectFieldTestCase",
+    "AutoCompleteSelectMultipleFieldTestCase",
 )
 
-class FieldTestMixin():
+
+class FieldTestMixin:
     field_cls = None
     lookup_cls = None
 
     def get_field_instance(self, allow_new=False, limit=None, widget=None):
-        return self.field_cls(self.lookup_cls, allow_new=allow_new, limit=limit, widget=widget)
+        return self.field_cls(
+            self.lookup_cls, allow_new=allow_new, limit=limit, widget=widget
+        )
 
     def test_init(self):
         field = self.get_field_instance()
         self.assertEqual(field.lookup_class, self.lookup_cls)
 
     def test_init_with_limit(self):
         field = self.get_field_instance(limit=10)
         self.assertEqual(field.limit, 10)
         self.assertEqual(field.widget.limit, 10)
 
     def test_clean(self):
-        self.fail('This test has not yet been written')
+        self.fail("This test has not yet been written")
 
     def test_dotted_path(self):
         """
         Ensure lookup_class can be imported from a dotted path.
         """
-        dotted_path = '.'.join([self.lookup_cls.__module__, self.lookup_cls.__name__])
+        dotted_path = ".".join([self.lookup_cls.__module__, self.lookup_cls.__name__])
         field = self.field_cls(dotted_path)
         self.assertEqual(field.lookup_class, self.lookup_cls)
 
     def test_invalid_dotted_path(self):
         """
         An invalid lookup_class dotted path should raise an ImportError.
         """
         with self.assertRaises(ImportError):
-            self.field_cls('that.is.an.invalid.path')
+            self.field_cls("that.is.an.invalid.path")
 
     def test_dotted_path_wrong_type(self):
         """
         lookup_class must be a subclass of LookupBase.
         """
-        dotted_path = 'selectable.forms.fields.AutoCompleteSelectField'
+        dotted_path = "selectable.forms.fields.AutoCompleteSelectField"
         with self.assertRaises(TypeError):
             self.field_cls(dotted_path)
 
+
 class AutoCompleteSelectFieldTestCase(BaseSelectableTestCase, FieldTestMixin):
     field_cls = fields.AutoCompleteSelectField
     lookup_cls = ThingLookup
 
     def test_clean(self):
         thing = self.create_thing()
         field = self.get_field_instance()
         value = field.clean([thing.name, thing.id])
         self.assertEqual(thing, value)
 
     def test_new_not_allowed(self):
         field = self.get_field_instance()
         value = self.get_random_string()
-        self.assertRaises(forms.ValidationError, field.clean, [value, ''])
+        self.assertRaises(forms.ValidationError, field.clean, [value, ""])
 
     def test_new_allowed(self):
         field = self.get_field_instance(allow_new=True)
         value = self.get_random_string()
-        value = field.clean([value, ''])
+        value = field.clean([value, ""])
         self.assertTrue(isinstance(value, ThingLookup.model))
 
     def test_default_widget(self):
         field = self.get_field_instance()
         self.assertTrue(isinstance(field.widget, widgets.AutoCompleteSelectWidget))
 
     def test_alternate_widget(self):
@@ -86,15 +89,15 @@
         widget = widgets.AutoComboboxWidget(self.lookup_cls)
         field = self.get_field_instance(widget=widget)
         self.assertTrue(isinstance(field.widget, widgets.AutoComboboxWidget))
 
     def test_invalid_pk(self):
         field = self.get_field_instance()
         value = self.get_random_string()
-        self.assertRaises(forms.ValidationError, field.clean, [value, 'XXX'])
+        self.assertRaises(forms.ValidationError, field.clean, [value, "XXX"])
 
 
 class AutoCompleteSelectMultipleFieldTestCase(BaseSelectableTestCase, FieldTestMixin):
     field_cls = fields.AutoCompleteSelectMultipleField
     lookup_cls = ThingLookup
 
     def get_field_instance(self, limit=None, widget=None):
@@ -112,23 +115,33 @@
         field = self.get_field_instance()
         ids = [thing.id, other_thing.id]
         value = field.clean(ids)
         self.assertEqual([thing, other_thing], value)
 
     def test_default_widget(self):
         field = self.get_field_instance()
-        self.assertTrue(isinstance(field.widget, widgets.AutoCompleteSelectMultipleWidget))
+        self.assertTrue(
+            isinstance(field.widget, widgets.AutoCompleteSelectMultipleWidget)
+        )
 
     def test_alternate_widget(self):
         widget_cls = widgets.AutoComboboxSelectMultipleWidget
         field = self.get_field_instance(widget=widget_cls)
         self.assertTrue(isinstance(field.widget, widget_cls))
 
     def test_alternate_widget_instance(self):
         widget = widgets.AutoComboboxSelectMultipleWidget(self.lookup_cls)
         field = self.get_field_instance(widget=widget)
-        self.assertTrue(isinstance(field.widget, widgets.AutoComboboxSelectMultipleWidget))
+        self.assertTrue(
+            isinstance(field.widget, widgets.AutoComboboxSelectMultipleWidget)
+        )
 
     def test_invalid_pk(self):
         field = self.get_field_instance()
-        value = self.get_random_string()
-        self.assertRaises(forms.ValidationError, field.clean, ['XXX', ])
+        self.get_random_string()
+        self.assertRaises(
+            forms.ValidationError,
+            field.clean,
+            [
+                "XXX",
+            ],
+        )
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_forms.py` & `django-selectable-1.4.0/selectable/tests/test_forms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,86 +1,82 @@
 from ..forms import BaseLookupForm
 from .base import BaseSelectableTestCase
 
-
-__all__ = (
-    'BaseLookupFormTestCase',
-)
+__all__ = ("BaseLookupFormTestCase",)
 
 
 class BaseLookupFormTestCase(BaseSelectableTestCase):
-
     def get_valid_data(self):
         data = {
-            'term': 'foo',
-            'limit': 10,
+            "term": "foo",
+            "limit": 10,
         }
         return data
 
     def test_valid_data(self):
         data = self.get_valid_data()
         form = BaseLookupForm(data)
         self.assertTrue(form.is_valid(), "%s" % form.errors)
 
     def test_invalid_limit(self):
         """
         Test giving the form an invalid limit.
         """
 
         data = self.get_valid_data()
-        data['limit'] = 'bar'
+        data["limit"] = "bar"
         form = BaseLookupForm(data)
         self.assertFalse(form.is_valid())
 
     def test_no_limit(self):
         """
         If SELECTABLE_MAX_LIMIT is set and limit is not given then
         the form will return SELECTABLE_MAX_LIMIT.
         """
 
         with self.settings(SELECTABLE_MAX_LIMIT=25):
             data = self.get_valid_data()
-            if 'limit' in data:
-                del data['limit']
+            if "limit" in data:
+                del data["limit"]
             form = BaseLookupForm(data)
             self.assertTrue(form.is_valid(), "%s" % form.errors)
-            self.assertEqual(form.cleaned_data['limit'], 25)
+            self.assertEqual(form.cleaned_data["limit"], 25)
 
     def test_no_max_set(self):
         """
         If SELECTABLE_MAX_LIMIT is not set but given then the form
         will return the given limit.
         """
 
         with self.settings(SELECTABLE_MAX_LIMIT=None):
             data = self.get_valid_data()
             form = BaseLookupForm(data)
             self.assertTrue(form.is_valid(), "%s" % form.errors)
-            if 'limit' in data:
-                self.assertTrue(form.cleaned_data['limit'], data['limit'])
+            if "limit" in data:
+                self.assertTrue(form.cleaned_data["limit"], data["limit"])
 
     def test_no_max_set_not_given(self):
         """
         If SELECTABLE_MAX_LIMIT is not set and not given then the form
         will return no limit.
         """
 
         with self.settings(SELECTABLE_MAX_LIMIT=None):
             data = self.get_valid_data()
-            if 'limit' in data:
-                del data['limit']
+            if "limit" in data:
+                del data["limit"]
             form = BaseLookupForm(data)
             self.assertTrue(form.is_valid(), "%s" % form.errors)
-            self.assertFalse(form.cleaned_data.get('limit'))
+            self.assertFalse(form.cleaned_data.get("limit"))
 
     def test_over_limit(self):
         """
         If SELECTABLE_MAX_LIMIT is set and limit given is greater then
         the form will return SELECTABLE_MAX_LIMIT.
         """
 
         with self.settings(SELECTABLE_MAX_LIMIT=25):
             data = self.get_valid_data()
-            data['limit'] = 125
+            data["limit"] = 125
             form = BaseLookupForm(data)
             self.assertTrue(form.is_valid(), "%s" % form.errors)
-            self.assertEqual(form.cleaned_data['limit'], 25)
+            self.assertEqual(form.cleaned_data["limit"], 25)
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_functional.py` & `django-selectable-1.4.0/selectable/tests/test_functional.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,359 +1,374 @@
 """
 Larger functional tests for fields and widgets.
 """
 from django import forms
 
-from ..forms import AutoCompleteSelectField, AutoCompleteSelectMultipleField
-from ..forms import AutoCompleteSelectWidget, AutoComboboxSelectWidget
+from ..forms import (
+    AutoComboboxSelectWidget, AutoCompleteSelectField, AutoCompleteSelectMultipleField, AutoCompleteSelectWidget)
 from . import ManyThing, OtherThing, ThingLookup
 from .base import BaseSelectableTestCase
 
-
 __all__ = (
-    'FuncAutoCompleteSelectTestCase',
-    'FuncSelectModelChoiceTestCase',
-    'FuncComboboxModelChoiceTestCase',
-    'FuncManytoManyMultipleSelectTestCase',
-    'FuncFormTestCase',
+    "FuncAutoCompleteSelectTestCase",
+    "FuncSelectModelChoiceTestCase",
+    "FuncComboboxModelChoiceTestCase",
+    "FuncManytoManyMultipleSelectTestCase",
+    "FuncFormTestCase",
 )
 
 
 class OtherThingForm(forms.ModelForm):
-
     thing = AutoCompleteSelectField(lookup_class=ThingLookup)
 
     class Meta:
         model = OtherThing
-        fields = ('name', 'thing', )
+        fields = (
+            "name",
+            "thing",
+        )
 
 
 class FuncAutoCompleteSelectTestCase(BaseSelectableTestCase):
-
     def setUp(self):
         self.test_thing = self.create_thing()
 
     def test_valid_form(self):
         "Valid form using an AutoCompleteSelectField."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': self.test_thing.pk,  # Hidden input
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": self.test_thing.pk,  # Hidden input
         }
         form = OtherThingForm(data=data)
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_invalid_form_missing_selected_pk(self):
         "Invalid form using an AutoCompleteSelectField."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': '',  # Hidden input
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": "",  # Hidden input
         }
         form = OtherThingForm(data=data)
-        self.assertFalse(form.is_valid(), 'Form should not be valid')
-        self.assertFalse('name' in form.errors)
-        self.assertTrue('thing' in form.errors)
+        self.assertFalse(form.is_valid(), "Form should not be valid")
+        self.assertFalse("name" in form.errors)
+        self.assertTrue("thing" in form.errors)
 
     def test_invalid_form_missing_name(self):
         "Invalid form using an AutoCompleteSelectField."
         data = {
-            'name': '',
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': self.test_thing.pk,  # Hidden input
+            "name": "",
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": self.test_thing.pk,  # Hidden input
         }
         form = OtherThingForm(data=data)
-        self.assertFalse(form.is_valid(), 'Form should not be valid')
-        self.assertTrue('name' in form.errors)
-        self.assertFalse('thing' in form.errors)
+        self.assertFalse(form.is_valid(), "Form should not be valid")
+        self.assertTrue("name" in form.errors)
+        self.assertFalse("thing" in form.errors)
 
     def test_invalid_but_still_selected(self):
         "Invalid form should keep selected item."
         data = {
-            'name': '',
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': self.test_thing.pk,  # Hidden input
+            "name": "",
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": self.test_thing.pk,  # Hidden input
         }
         form = OtherThingForm(data=data)
-        self.assertFalse(form.is_valid(), 'Form should not be valid')
+        self.assertFalse(form.is_valid(), "Form should not be valid")
         rendered_form = form.as_p()
         # Selected text should be populated
         self.assertInHTML(
-            '''
+            """
             <input data-selectable-allow-new="false" data-selectable-type="text"
                 data-selectable-url="/selectable-tests/selectable-thinglookup/"
                 id="id_thing_0" name="thing_0" type="text" value="{}" {} />
-            '''.format(self.test_thing.name,
-                       'required' if hasattr(form, 'use_required_attribute') else ''),
-            rendered_form
+            """.format(
+                self.test_thing.name,
+                "required" if hasattr(form, "use_required_attribute") else "",
+            ),
+            rendered_form,
         )
         # Selected pk should be populated
         self.assertInHTML(
-            '''
+            """
             <input data-selectable-type="hidden" name="thing_1" id="id_thing_1"
                 type="hidden" value="{}" {} />
-            '''.format(self.test_thing.pk,
-                       'required' if hasattr(form, 'use_required_attribute') else ''),
+            """.format(
+                self.test_thing.pk,
+                "required" if hasattr(form, "use_required_attribute") else "",
+            ),
             rendered_form,
         )
 
     def test_populate_from_model(self):
         "Populate from existing model."
-        other_thing = OtherThing.objects.create(thing=self.test_thing, name='a')
+        other_thing = OtherThing.objects.create(thing=self.test_thing, name="a")
         form = OtherThingForm(instance=other_thing)
         rendered_form = form.as_p()
         # Selected text should be populated
         self.assertInHTML(
-            '''
+            """
             <input data-selectable-allow-new="false" data-selectable-type="text"
                 data-selectable-url="/selectable-tests/selectable-thinglookup/"
                 id="id_thing_0" name="thing_0" type="text" value="{}" {} />
-            '''.format(self.test_thing.name,
-                       'required' if hasattr(form, 'use_required_attribute') else ''),
-            rendered_form
+            """.format(
+                self.test_thing.name,
+                "required" if hasattr(form, "use_required_attribute") else "",
+            ),
+            rendered_form,
         )
         # Selected pk should be populated
         self.assertInHTML(
-            '''
+            """
             <input data-selectable-type="hidden" name="thing_1" id="id_thing_1"
                 type="hidden" value="{}" {} />
-            '''.format(self.test_thing.pk,
-                       'required' if hasattr(form, 'use_required_attribute') else ''),
-            rendered_form
+            """.format(
+                self.test_thing.pk,
+                "required" if hasattr(form, "use_required_attribute") else "",
+            ),
+            rendered_form,
         )
 
 
 class SelectWidgetForm(forms.ModelForm):
-
     class Meta:
         model = OtherThing
-        fields = ('name', 'thing', )
-        widgets = {
-            'thing': AutoCompleteSelectWidget(lookup_class=ThingLookup)
-        }
+        fields = (
+            "name",
+            "thing",
+        )
+        widgets = {"thing": AutoCompleteSelectWidget(lookup_class=ThingLookup)}
 
 
 class FuncSelectModelChoiceTestCase(BaseSelectableTestCase):
     """
     Functional tests for AutoCompleteSelectWidget compatibility
     with a ModelChoiceField.
     """
 
     def setUp(self):
         self.test_thing = self.create_thing()
 
     def test_valid_form(self):
         "Valid form using an AutoCompleteSelectWidget."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': self.test_thing.pk,  # Hidden input
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": self.test_thing.pk,  # Hidden input
         }
         form = SelectWidgetForm(data=data)
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_missing_pk(self):
         "Invalid form (missing required pk) using an AutoCompleteSelectWidget."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': '',  # Hidden input missing
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": "",  # Hidden input missing
         }
         form = SelectWidgetForm(data=data)
         self.assertFalse(form.is_valid())
-        self.assertTrue('thing' in form.errors)
+        self.assertTrue("thing" in form.errors)
 
     def test_invalid_pk(self):
         "Invalid form (invalid pk value) using an AutoCompleteSelectWidget."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': 'XXX',  # Hidden input doesn't match a PK
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": "XXX",  # Hidden input doesn't match a PK
         }
         form = SelectWidgetForm(data=data)
         self.assertFalse(form.is_valid())
-        self.assertTrue('thing' in form.errors)
+        self.assertTrue("thing" in form.errors)
 
     def test_post_compatibility(self):
         """
         If new items are not allowed then the original field
         name can be included in the POST with the selected id.
         """
         data = {
-            'name': self.get_random_string(),
-            'thing': self.test_thing.pk,
+            "name": self.get_random_string(),
+            "thing": self.test_thing.pk,
         }
         form = SelectWidgetForm(data=data)
         self.assertTrue(form.is_valid(), str(form.errors))
 
 
 class ComboboxSelectWidgetForm(forms.ModelForm):
-
     class Meta:
         model = OtherThing
-        fields = ('name', 'thing', )
-        widgets = {
-            'thing': AutoComboboxSelectWidget(lookup_class=ThingLookup)
-        }
+        fields = (
+            "name",
+            "thing",
+        )
+        widgets = {"thing": AutoComboboxSelectWidget(lookup_class=ThingLookup)}
 
 
 class FuncComboboxModelChoiceTestCase(BaseSelectableTestCase):
     """
     Functional tests for AutoComboboxSelectWidget compatibility
     with a ModelChoiceField.
     """
 
     def setUp(self):
         self.test_thing = self.create_thing()
 
     def test_valid_form(self):
         "Valid form using an AutoComboboxSelectWidget."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': self.test_thing.pk,  # Hidden input
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": self.test_thing.pk,  # Hidden input
         }
         form = ComboboxSelectWidgetForm(data=data)
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_missing_pk(self):
         "Invalid form (missing required pk) using an AutoComboboxSelectWidget."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': '',  # Hidden input missing
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": "",  # Hidden input missing
         }
         form = ComboboxSelectWidgetForm(data=data)
         self.assertFalse(form.is_valid())
-        self.assertTrue('thing' in form.errors)
+        self.assertTrue("thing" in form.errors)
 
     def test_invalid_pk(self):
         "Invalid form (invalid pk value) using an AutoComboboxSelectWidget."
         data = {
-            'name': self.get_random_string(),
-            'thing_0': self.test_thing.name,  # Text input
-            'thing_1': 'XXX',  # Hidden input doesn't match a PK
+            "name": self.get_random_string(),
+            "thing_0": self.test_thing.name,  # Text input
+            "thing_1": "XXX",  # Hidden input doesn't match a PK
         }
         form = ComboboxSelectWidgetForm(data=data)
         self.assertFalse(form.is_valid())
-        self.assertTrue('thing' in form.errors)
+        self.assertTrue("thing" in form.errors)
 
     def test_post_compatibility(self):
         """
         If new items are not allowed then the original field
         name can be included in the POST with the selected id.
         """
         data = {
-            'name': self.get_random_string(),
-            'thing': self.test_thing.pk,
+            "name": self.get_random_string(),
+            "thing": self.test_thing.pk,
         }
         form = ComboboxSelectWidgetForm(data=data)
         self.assertTrue(form.is_valid(), str(form.errors))
 
 
 class ManyThingForm(forms.ModelForm):
-
     things = AutoCompleteSelectMultipleField(lookup_class=ThingLookup)
 
     class Meta:
         model = ManyThing
-        fields = ('name', 'things', )
+        fields = (
+            "name",
+            "things",
+        )
 
 
 class FuncManytoManyMultipleSelectTestCase(BaseSelectableTestCase):
     """
     Functional tests for AutoCompleteSelectMultipleField compatibility
     with a ManyToManyField.
     """
 
     def setUp(self):
         self.test_thing = self.create_thing()
 
     def test_valid_form(self):
         "Valid form using an AutoCompleteSelectMultipleField."
         data = {
-            'name': self.get_random_string(),
-            'things_0': '',  # Text input
-            'things_1': [self.test_thing.pk, ],  # Hidden inputs
+            "name": self.get_random_string(),
+            "things_0": "",  # Text input
+            "things_1": [
+                self.test_thing.pk,
+            ],  # Hidden inputs
         }
         form = ManyThingForm(data=data)
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_valid_save(self):
         "Saving data from a valid form."
         data = {
-            'name': self.get_random_string(),
-            'things_0': '',  # Text input
-            'things_1': [self.test_thing.pk, ],  # Hidden inputs
+            "name": self.get_random_string(),
+            "things_0": "",  # Text input
+            "things_1": [
+                self.test_thing.pk,
+            ],  # Hidden inputs
         }
         form = ManyThingForm(data=data)
         manything = form.save()
-        self.assertEqual(manything.name, data['name'])
+        self.assertEqual(manything.name, data["name"])
         things = manything.things.all()
         self.assertEqual(things.count(), 1)
         self.assertTrue(self.test_thing in things)
 
     def test_not_required(self):
         "Valid form where many to many is not required."
         data = {
-            'name': self.get_random_string(),
-            'things_0': '',  # Text input
-            'things_1': [],  # Hidden inputs
+            "name": self.get_random_string(),
+            "things_0": "",  # Text input
+            "things_1": [],  # Hidden inputs
         }
         form = ManyThingForm(data=data)
-        form.fields['things'].required = False
+        form.fields["things"].required = False
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_not_required_save(self):
         "Saving data when many to many is not required."
         data = {
-            'name': self.get_random_string(),
-            'things_0': '',  # Text input
-            'things_1': [],  # Hidden inputs
+            "name": self.get_random_string(),
+            "things_0": "",  # Text input
+            "things_1": [],  # Hidden inputs
         }
         form = ManyThingForm(data=data)
-        form.fields['things'].required = False
+        form.fields["things"].required = False
         manything = form.save()
-        self.assertEqual(manything.name, data['name'])
+        self.assertEqual(manything.name, data["name"])
         things = manything.things.all()
         self.assertEqual(things.count(), 0)
 
     def test_has_changed(self):
         "Populate intial data from a model."
-        manything = ManyThing.objects.create(name='Foo')
+        manything = ManyThing.objects.create(name="Foo")
         thing_1 = self.create_thing()
         manything.things.add(thing_1)
         data = {
-            'name': manything.name,
-            'things_0': '',  # Text input
-            'things_1': [thing_1.pk],  # Hidden inputs
+            "name": manything.name,
+            "things_0": "",  # Text input
+            "things_1": [thing_1.pk],  # Hidden inputs
         }
         form = ManyThingForm(data=data, instance=manything)
         self.assertFalse(form.has_changed(), str(form.changed_data))
 
     def test_post_compatibility(self):
         """
         If new items are not allowed then the original field
         name can be included in the POST with the selected ids.
         """
         data = {
-            'name': self.get_random_string(),
-            'things': [self.test_thing.pk, ],
+            "name": self.get_random_string(),
+            "things": [
+                self.test_thing.pk,
+            ],
         }
         form = ManyThingForm(data=data)
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_render_form(self):
         thing_1 = self.create_thing()
-        manything = ManyThing.objects.create(name='Foo')
+        manything = ManyThing.objects.create(name="Foo")
         manything.things.add(thing_1)
         form = ManyThingForm(instance=manything)
         rendered = form.as_p()
-        self.assertIn('title="{0}"'.format(thing_1.name),
-                      rendered)
+        self.assertIn('title="{0}"'.format(thing_1.name), rendered)
 
 
 class SimpleForm(forms.Form):
     "Non-model form usage."
     thing = AutoCompleteSelectField(lookup_class=ThingLookup)
     new_thing = AutoCompleteSelectField(lookup_class=ThingLookup, allow_new=True)
     things = AutoCompleteSelectMultipleField(lookup_class=ThingLookup)
@@ -368,98 +383,111 @@
 
     def setUp(self):
         self.test_thing = self.create_thing()
 
     def test_blank_new_item(self):
         "Regression test for #91. new_thing is required but both are blank."
         data = {
-            'thing_0': self.test_thing.name,
-            'thing_1': self.test_thing.pk,
-            'new_thing_0': '',
-            'new_thing_1': '',
-            'things_0': '',
-            'things_1': [self.test_thing.pk, ]
+            "thing_0": self.test_thing.name,
+            "thing_1": self.test_thing.pk,
+            "new_thing_0": "",
+            "new_thing_1": "",
+            "things_0": "",
+            "things_1": [
+                self.test_thing.pk,
+            ],
         }
         form = SimpleForm(data=data)
         self.assertFalse(form.is_valid())
-        self.assertTrue('new_thing' in form.errors)
+        self.assertTrue("new_thing" in form.errors)
 
     def test_has_changed_with_empty_permitted(self):
         """
         Regression test for #92. has_changed fails when there is no initial and
         allow_new=False.
         """
         data = {
-            'thing_0': '',
-            'thing_1': self.test_thing.pk,
-            'new_thing_0': self.test_thing.name,
-            'new_thing_1': self.test_thing.pk,
-            'things_0': '',
-            'things_1': [self.test_thing.pk, ]
+            "thing_0": "",
+            "thing_1": self.test_thing.pk,
+            "new_thing_0": self.test_thing.name,
+            "new_thing_1": self.test_thing.pk,
+            "things_0": "",
+            "things_1": [
+                self.test_thing.pk,
+            ],
         }
         form = SimpleForm(data=data, empty_permitted=True, use_required_attribute=False)
         self.assertTrue(form.has_changed())
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_not_changed(self):
         """
         Regression test for #92. has_changed fails when there is no initial and
         allow_new=False.
         """
         data = {
-            'thing_0': self.test_thing.name,
-            'thing_1': self.test_thing.pk,
-            'new_thing_0': self.test_thing.name,
-            'new_thing_1': self.test_thing.pk,
-            'things_0': '',
-            'things_1': [self.test_thing.pk, ]
+            "thing_0": self.test_thing.name,
+            "thing_1": self.test_thing.pk,
+            "new_thing_0": self.test_thing.name,
+            "new_thing_1": self.test_thing.pk,
+            "things_0": "",
+            "things_1": [
+                self.test_thing.pk,
+            ],
         }
         initial = {
-            'thing': self.test_thing.pk,
-            'new_thing': self.test_thing.pk,
-            'things': [self.test_thing.pk, ]
+            "thing": self.test_thing.pk,
+            "new_thing": self.test_thing.pk,
+            "things": [
+                self.test_thing.pk,
+            ],
         }
         form = SimpleForm(data=data, initial=initial)
         self.assertFalse(form.has_changed())
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_not_changed_with_empty_permitted(self):
         """
         Regression test for #92. has_changed fails when there is no initial and
         allow_new=False.
         """
         data = {
-            'thing_0': '',
-            'thing_1': '',
-            'new_thing_0': '',
-            'new_thing_1': '',
-            'things_0': '',
-            'things_1': '',
+            "thing_0": "",
+            "thing_1": "",
+            "new_thing_0": "",
+            "new_thing_1": "",
+            "things_0": "",
+            "things_1": "",
         }
         initial = {
-            'thing': '',
-            'new_thing': '',
-            'things': '',
-        }
-        form = SimpleForm(data=data, initial=initial, empty_permitted=True, use_required_attribute=False)
+            "thing": "",
+            "new_thing": "",
+            "things": "",
+        }
+        form = SimpleForm(
+            data=data,
+            initial=initial,
+            empty_permitted=True,
+            use_required_attribute=False,
+        )
         self.assertFalse(form.has_changed(), str(form.changed_data))
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_no_initial_with_empty_permitted(self):
         """
         If empty data is submitted and allowed with no initial then
         the form should not be seen as changed.
         """
         data = {
-            'thing_0': '',
-            'thing_1': '',
-            'new_thing_0': '',
-            'new_thing_1': '',
-            'things_0': '',
-            'things_1': '',
+            "thing_0": "",
+            "thing_1": "",
+            "new_thing_0": "",
+            "new_thing_1": "",
+            "things_0": "",
+            "things_1": "",
         }
         form = SimpleForm(data=data, empty_permitted=True, use_required_attribute=False)
         self.assertFalse(form.has_changed(), str(form.changed_data))
         self.assertTrue(form.is_valid(), str(form.errors))
 
     def test_no_data_with_empty_permitted(self):
         """
@@ -472,102 +500,106 @@
 
     def test_select_multiple_changed(self):
         """
         Detect changes for a multiple select input with and without
         initial data.
         """
         data = {
-            'thing_0': '',
-            'thing_1': '',
-            'new_thing_0': '',
-            'new_thing_1': '',
-            'things_0': '',
-            'things_1': [self.test_thing.pk, ]
+            "thing_0": "",
+            "thing_1": "",
+            "new_thing_0": "",
+            "new_thing_1": "",
+            "things_0": "",
+            "things_1": [
+                self.test_thing.pk,
+            ],
         }
         form = SimpleForm(data=data)
         self.assertTrue(form.has_changed())
-        self.assertTrue('things' in form.changed_data)
+        self.assertTrue("things" in form.changed_data)
 
         initial = {
-            'thing': '',
-            'new_thing': '',
-            'things': [self.test_thing.pk, ],
+            "thing": "",
+            "new_thing": "",
+            "things": [
+                self.test_thing.pk,
+            ],
         }
         form = SimpleForm(data=data, initial=initial)
         self.assertFalse(form.has_changed(), str(form.changed_data))
 
         initial = {
-            'thing': '',
-            'new_thing': '',
-            'things': [],
+            "thing": "",
+            "new_thing": "",
+            "things": [],
         }
         form = SimpleForm(data=data, initial=initial)
         self.assertTrue(form.has_changed())
-        self.assertTrue('things' in form.changed_data)
+        self.assertTrue("things" in form.changed_data)
 
     def test_single_select_changed(self):
         """
         Detect changes for a single select input with and without
         initial data.
         """
         data = {
-            'thing_0': '',
-            'thing_1': self.test_thing.pk,
-            'new_thing_0': '',
-            'new_thing_1': '',
-            'things_0': '',
-            'things_1': ''
+            "thing_0": "",
+            "thing_1": self.test_thing.pk,
+            "new_thing_0": "",
+            "new_thing_1": "",
+            "things_0": "",
+            "things_1": "",
         }
         form = SimpleForm(data=data)
         self.assertTrue(form.has_changed())
-        self.assertTrue('thing' in form.changed_data)
+        self.assertTrue("thing" in form.changed_data)
 
         initial = {
-            'thing': self.test_thing.pk,
-            'new_thing': '',
-            'things': '',
+            "thing": self.test_thing.pk,
+            "new_thing": "",
+            "things": "",
         }
         form = SimpleForm(data=data, initial=initial)
         self.assertFalse(form.has_changed(), str(form.changed_data))
 
         initial = {
-            'thing': '',
-            'new_thing': '',
-            'things': '',
+            "thing": "",
+            "new_thing": "",
+            "things": "",
         }
         form = SimpleForm(data=data, initial=initial)
         self.assertTrue(form.has_changed())
-        self.assertTrue('thing' in form.changed_data)
+        self.assertTrue("thing" in form.changed_data)
 
     def test_new_select_changed(self):
         """
         Detect changes for a single select input which allows new items
         with and without initial data.
         """
         data = {
-            'thing_0': '',
-            'thing_1': '',
-            'new_thing_0': 'Foo',
-            'new_thing_1': '',
-            'things_0': '',
-            'things_1': ''
+            "thing_0": "",
+            "thing_1": "",
+            "new_thing_0": "Foo",
+            "new_thing_1": "",
+            "things_0": "",
+            "things_1": "",
         }
         form = SimpleForm(data=data)
         self.assertTrue(form.has_changed())
-        self.assertTrue('new_thing' in form.changed_data)
+        self.assertTrue("new_thing" in form.changed_data)
 
         initial = {
-            'thing': '',
-            'new_thing': ['Foo', None],
-            'things': '',
+            "thing": "",
+            "new_thing": ["Foo", None],
+            "things": "",
         }
         form = SimpleForm(data=data, initial=initial)
         self.assertFalse(form.has_changed(), str(form.changed_data))
 
         initial = {
-            'thing': '',
-            'new_thing': '',
-            'things': '',
+            "thing": "",
+            "new_thing": "",
+            "things": "",
         }
         form = SimpleForm(data=data, initial=initial)
         self.assertTrue(form.has_changed())
-        self.assertTrue('new_thing' in form.changed_data)
+        self.assertTrue("new_thing" in form.changed_data)
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_templatetags.py` & `django-selectable-1.4.0/selectable/tests/test_templatetags.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,115 +1,132 @@
-from django.template import Template, Context
+from django.template import Context, Template
 
 from .base import BaseSelectableTestCase
 
 __all__ = (
-    'JqueryTagTestCase',
-    'ThemeTagTestCase',
+    "JqueryTagTestCase",
+    "ThemeTagTestCase",
 )
 
 
 class JqueryTagTestCase(BaseSelectableTestCase):
-
     def assertJQueryVersion(self, result, version):
         expected = "//ajax.googleapis.com/ajax/libs/jquery/%s/jquery.min.js" % version
         self.assertTrue(expected in result)
 
     def assertUIVersion(self, result, version):
         expected = "//ajax.googleapis.com/ajax/libs/jqueryui/%s/jquery-ui.js" % version
         self.assertTrue(expected in result)
 
     def test_render(self):
         "Render template tag with default versions."
         template = Template("{% load selectable_tags %}{% include_jquery_libs %}")
         context = Context({})
         result = template.render(context)
-        self.assertJQueryVersion(result, '1.12.4')
-        self.assertUIVersion(result, '1.11.4')
+        self.assertJQueryVersion(result, "1.12.4")
+        self.assertUIVersion(result, "1.11.4")
 
     def test_render_jquery_version(self):
         "Render template tag with specified jQuery version."
-        template = Template("{% load selectable_tags %}{% include_jquery_libs '1.4.3' %}")
+        template = Template(
+            "{% load selectable_tags %}{% include_jquery_libs '1.4.3' %}"
+        )
         context = Context({})
         result = template.render(context)
-        self.assertJQueryVersion(result, '1.4.3')
+        self.assertJQueryVersion(result, "1.4.3")
 
     def test_render_variable_jquery_version(self):
         "Render using jQuery version from the template context."
-        version = '1.4.3'
-        template = Template("{% load selectable_tags %}{% include_jquery_libs version %}")
-        context = Context({'version': version})
+        version = "1.4.3"
+        template = Template(
+            "{% load selectable_tags %}{% include_jquery_libs version %}"
+        )
+        context = Context({"version": version})
         result = template.render(context)
-        self.assertJQueryVersion(result, '1.4.3')
+        self.assertJQueryVersion(result, "1.4.3")
 
     def test_render_jquery_ui_version(self):
         "Render template tag with specified jQuery UI version."
-        template = Template("{% load selectable_tags %}{% include_jquery_libs '1.4.3' '1.8.13' %}")
+        template = Template(
+            "{% load selectable_tags %}{% include_jquery_libs '1.4.3' '1.8.13' %}"
+        )
         context = Context({})
         result = template.render(context)
-        self.assertUIVersion(result, '1.8.13')
+        self.assertUIVersion(result, "1.8.13")
 
     def test_render_variable_jquery_ui_version(self):
         "Render using jQuery UI version from the template context."
-        version = '1.8.13'
-        template = Template("{% load selectable_tags %}{% include_jquery_libs '1.4.3' version %}")
-        context = Context({'version': version})
+        version = "1.8.13"
+        template = Template(
+            "{% load selectable_tags %}{% include_jquery_libs '1.4.3' version %}"
+        )
+        context = Context({"version": version})
         result = template.render(context)
-        self.assertUIVersion(result, '1.8.13')
+        self.assertUIVersion(result, "1.8.13")
 
     def test_render_no_jquery(self):
         "Render template tag without jQuery."
         template = Template("{% load selectable_tags %}{% include_jquery_libs '' %}")
         context = Context({})
         result = template.render(context)
-        self.assertTrue('jquery.min.js' not in result)
+        self.assertTrue("jquery.min.js" not in result)
 
     def test_render_no_jquery_ui(self):
         "Render template tag without jQuery UI."
-        template = Template("{% load selectable_tags %}{% include_jquery_libs '1.7.2' '' %}")
+        template = Template(
+            "{% load selectable_tags %}{% include_jquery_libs '1.7.2' '' %}"
+        )
         context = Context({})
         result = template.render(context)
-        self.assertTrue('jquery-ui.js' not in result)
+        self.assertTrue("jquery-ui.js" not in result)
 
 
 class ThemeTagTestCase(BaseSelectableTestCase):
-
     def assertUICSS(self, result, theme, version):
-        expected = "//ajax.googleapis.com/ajax/libs/jqueryui/%s/themes/%s/jquery-ui.css" % (version, theme)
+        expected = (
+            "//ajax.googleapis.com/ajax/libs/jqueryui/%s/themes/%s/jquery-ui.css"
+            % (version, theme)
+        )
         self.assertTrue(expected in result)
 
     def test_render(self):
         "Render template tag with default settings."
         template = Template("{% load selectable_tags %}{% include_ui_theme %}")
         context = Context({})
         result = template.render(context)
-        self.assertUICSS(result, 'smoothness', '1.11.4')
+        self.assertUICSS(result, "smoothness", "1.11.4")
 
     def test_render_version(self):
         "Render template tag with alternate version."
-        template = Template("{% load selectable_tags %}{% include_ui_theme 'base' '1.8.13' %}")
+        template = Template(
+            "{% load selectable_tags %}{% include_ui_theme 'base' '1.8.13' %}"
+        )
         context = Context({})
         result = template.render(context)
-        self.assertUICSS(result, 'base', '1.8.13')
+        self.assertUICSS(result, "base", "1.8.13")
 
     def test_variable_version(self):
         "Render using version from content variable."
-        version = '1.8.13'
-        template = Template("{% load selectable_tags %}{% include_ui_theme 'base' version %}")
-        context = Context({'version': version})
+        version = "1.8.13"
+        template = Template(
+            "{% load selectable_tags %}{% include_ui_theme 'base' version %}"
+        )
+        context = Context({"version": version})
         result = template.render(context)
-        self.assertUICSS(result, 'base', version)
+        self.assertUICSS(result, "base", version)
 
     def test_render_theme(self):
         "Render template tag with alternate theme."
-        template = Template("{% load selectable_tags %}{% include_ui_theme 'ui-lightness' %}")
+        template = Template(
+            "{% load selectable_tags %}{% include_ui_theme 'ui-lightness' %}"
+        )
         context = Context({})
         result = template.render(context)
-        self.assertUICSS(result, 'ui-lightness', '1.11.4')
+        self.assertUICSS(result, "ui-lightness", "1.11.4")
 
     def test_variable_theme(self):
         "Render using theme from content variable."
-        theme = 'ui-lightness'
+        theme = "ui-lightness"
         template = Template("{% load selectable_tags %}{% include_ui_theme theme %}")
-        context = Context({'theme': theme})
+        context = Context({"theme": theme})
         result = template.render(context)
-        self.assertUICSS(result, theme, '1.11.4')
+        self.assertUICSS(result, theme, "1.11.4")
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_views.py` & `django-selectable-1.4.0/selectable/tests/test_views.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,91 +1,87 @@
 import json
 
 from django.conf import settings
-from django.urls import reverse
 from django.test import override_settings
+from django.urls import reverse
 
 from . import ThingLookup
 from .base import BaseSelectableTestCase
 
-
-__all__ = (
-    'SelectableViewTest',
-)
+__all__ = ("SelectableViewTest",)
 
 
 @override_settings(SELECTABLE_MAX_LIMIT=25)
 class SelectableViewTest(BaseSelectableTestCase):
-
     def setUp(self):
         super().setUp()
         self.url = ThingLookup.url()
         self.lookup = ThingLookup()
         self.thing = self.create_thing()
         self.other_thing = self.create_thing()
 
     def test_response_type(self):
         response = self.client.get(self.url)
-        self.assertEqual(response['Content-Type'], 'application/json')
+        self.assertEqual(response["Content-Type"], "application/json")
 
     def test_response_keys(self):
         response = self.client.get(self.url)
-        data = json.loads(response.content.decode('utf-8'))
-        for result in data.get('data'):
-            self.assertTrue('id' in result)
-            self.assertTrue('value' in result)
-            self.assertTrue('label' in result)
+        data = json.loads(response.content.decode("utf-8"))
+        for result in data.get("data"):
+            self.assertTrue("id" in result)
+            self.assertTrue("value" in result)
+            self.assertTrue("label" in result)
 
     def test_no_term_lookup(self):
         data = {}
         response = self.client.get(self.url, data)
-        data = json.loads(response.content.decode('utf-8'))
+        data = json.loads(response.content.decode("utf-8"))
         self.assertEqual(len(data), 2)
 
     def test_simple_term_lookup(self):
-        data = {'term': self.thing.name}
+        data = {"term": self.thing.name}
         response = self.client.get(self.url, data)
-        data = json.loads(response.content.decode('utf-8'))
+        data = json.loads(response.content.decode("utf-8"))
         self.assertEqual(len(data), 2)
-        self.assertEqual(len(data.get('data')), 1)
+        self.assertEqual(len(data.get("data")), 1)
 
     def test_unknown_lookup(self):
-        unknown_url = reverse('selectable-lookup', args=["XXXXXXX"])
+        unknown_url = reverse("selectable-lookup", args=["XXXXXXX"])
         response = self.client.get(unknown_url)
         self.assertEqual(response.status_code, 404)
 
     def test_basic_limit(self):
         for i in range(settings.SELECTABLE_MAX_LIMIT):
-            self.create_thing(data={'name': 'Thing%s' % i})
+            self.create_thing(data={"name": "Thing%s" % i})
         response = self.client.get(self.url)
-        data = json.loads(response.content.decode('utf-8'))
-        self.assertEqual(len(data.get('data')), settings.SELECTABLE_MAX_LIMIT)
-        meta = data.get('meta')
-        self.assertTrue('next_page' in meta)
+        data = json.loads(response.content.decode("utf-8"))
+        self.assertEqual(len(data.get("data")), settings.SELECTABLE_MAX_LIMIT)
+        meta = data.get("meta")
+        self.assertTrue("next_page" in meta)
 
     def test_get_next_page(self):
         for i in range(settings.SELECTABLE_MAX_LIMIT * 2):
-            self.create_thing(data={'name': 'Thing%s' % i})
-        data = {'term': 'Thing', 'page': 2}
+            self.create_thing(data={"name": "Thing%s" % i})
+        data = {"term": "Thing", "page": 2}
         response = self.client.get(self.url, data)
-        data = json.loads(response.content.decode('utf-8'))
-        self.assertEqual(len(data.get('data')), settings.SELECTABLE_MAX_LIMIT)
+        data = json.loads(response.content.decode("utf-8"))
+        self.assertEqual(len(data.get("data")), settings.SELECTABLE_MAX_LIMIT)
         # No next page
-        meta = data.get('meta')
-        self.assertFalse('next_page' in meta)
+        meta = data.get("meta")
+        self.assertFalse("next_page" in meta)
 
     def test_request_more_than_max(self):
         for i in range(settings.SELECTABLE_MAX_LIMIT):
-            self.create_thing(data={'name': 'Thing%s' % i})
-        data = {'term': '', 'limit': settings.SELECTABLE_MAX_LIMIT * 2}
+            self.create_thing(data={"name": "Thing%s" % i})
+        data = {"term": "", "limit": settings.SELECTABLE_MAX_LIMIT * 2}
         response = self.client.get(self.url)
-        data = json.loads(response.content.decode('utf-8'))
-        self.assertEqual(len(data.get('data')), settings.SELECTABLE_MAX_LIMIT)
+        data = json.loads(response.content.decode("utf-8"))
+        self.assertEqual(len(data.get("data")), settings.SELECTABLE_MAX_LIMIT)
 
     def test_request_less_than_max(self):
         for i in range(settings.SELECTABLE_MAX_LIMIT):
-            self.create_thing(data={'name': 'Thing%s' % i})
+            self.create_thing(data={"name": "Thing%s" % i})
         new_limit = settings.SELECTABLE_MAX_LIMIT // 2
-        data = {'term': '', 'limit': new_limit}
+        data = {"term": "", "limit": new_limit}
         response = self.client.get(self.url, data)
-        data = json.loads(response.content.decode('utf-8'))
-        self.assertEqual(len(data.get('data')), new_limit)
+        data = json.loads(response.content.decode("utf-8"))
+        self.assertEqual(len(data.get("data")), new_limit)
```

### Comparing `django-selectable-1.3.0/selectable/tests/test_widgets.py` & `django-selectable-1.4.0/selectable/tests/test_widgets.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,107 +1,109 @@
 import json
 
 from django import forms
 from django.utils.http import urlencode
+from urllib.parse import urlparse
 
-from . import Thing, ThingLookup
-from ..compat import urlparse
 from ..forms import widgets
+from . import Thing, ThingLookup
 from .base import BaseSelectableTestCase, parsed_inputs, parsed_widget_attributes
 
 __all__ = (
-    'AutoCompleteWidgetTestCase',
-    'AutoCompleteSelectWidgetTestCase',
-    'AutoComboboxWidgetTestCase',
-    'AutoComboboxSelectWidgetTestCase',
-    'AutoCompleteSelectMultipleWidgetTestCase',
-    'AutoComboboxSelectMultipleWidgetTestCase',
+    "AutoCompleteWidgetTestCase",
+    "AutoCompleteSelectWidgetTestCase",
+    "AutoComboboxWidgetTestCase",
+    "AutoComboboxSelectWidgetTestCase",
+    "AutoCompleteSelectMultipleWidgetTestCase",
+    "AutoComboboxSelectMultipleWidgetTestCase",
 )
 
 
-class WidgetTestMixin():
+class WidgetTestMixin:
     widget_cls = None
     lookup_cls = None
 
     def get_widget_instance(self, **kwargs):
         return self.__class__.widget_cls(self.__class__.lookup_cls, **kwargs)
 
     def test_init(self):
         widget = self.get_widget_instance()
         self.assertEqual(widget.lookup_class, self.__class__.lookup_cls)
 
     def test_dotted_path(self):
         """
         Ensure lookup_class can be imported from a dotted path.
         """
-        dotted_path = '.'.join([self.__class__.lookup_cls.__module__, self.__class__.lookup_cls.__name__])
+        dotted_path = ".".join(
+            [self.__class__.lookup_cls.__module__, self.__class__.lookup_cls.__name__]
+        )
         widget = self.__class__.widget_cls(dotted_path)
         self.assertEqual(widget.lookup_class, self.__class__.lookup_cls)
 
     def test_invalid_dotted_path(self):
         """
         An invalid lookup_class dotted path should raise an ImportError.
         """
         with self.assertRaises(ImportError):
-            self.__class__.widget_cls('that.is.an.invalid.path')
+            self.__class__.widget_cls("that.is.an.invalid.path")
 
     def test_dotted_path_wrong_type(self):
         """
         lookup_class must be a subclass of LookupBase.
         """
-        dotted_path = 'selectable.forms.widgets.AutoCompleteWidget'
+        dotted_path = "selectable.forms.widgets.AutoCompleteWidget"
         with self.assertRaises(TypeError):
             self.__class__.widget_cls(dotted_path)
 
 
 class AutoCompleteWidgetTestCase(BaseSelectableTestCase, WidgetTestMixin):
     widget_cls = widgets.AutoCompleteWidget
     lookup_cls = ThingLookup
 
     def test_rendered_attrs(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget)
-        self.assertTrue('data-selectable-url' in attrs)
-        self.assertTrue('data-selectable-type' in attrs)
-        self.assertTrue('data-selectable-allow-new' in attrs)
+        self.assertTrue("data-selectable-url" in attrs)
+        self.assertTrue("data-selectable-type" in attrs)
+        self.assertTrue("data-selectable-allow-new" in attrs)
 
     def test_update_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance()
         widget.update_query_parameters(params)
         attrs = parsed_widget_attributes(widget)
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_limit_parameter(self):
         widget = self.get_widget_instance(limit=10)
         attrs = parsed_widget_attributes(widget)
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
-        self.assertTrue('limit=10' in query)
+        self.assertTrue("limit=10" in query)
 
     def test_initial_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance(query_params=params)
         attrs = parsed_widget_attributes(widget)
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_build_selectable_options(self):
         "Serialize selectable options as json in data attribute."
-        options = {'autoFocus': True}
-        widget = self.get_widget_instance(attrs={'data-selectable-options': options})
+        options = {"autoFocus": True}
+        widget = self.get_widget_instance(attrs={"data-selectable-options": options})
         attrs = parsed_widget_attributes(widget)
-        self.assertTrue('data-selectable-options' in attrs)
-        self.assertEqual(attrs['data-selectable-options'], json.dumps(options))
+        self.assertTrue("data-selectable-options" in attrs)
+        self.assertEqual(attrs["data-selectable-options"], json.dumps(options))
 
 
 class AutoCompleteSelectWidgetTestCase(BaseSelectableTestCase, WidgetTestMixin):
     widget_cls = widgets.AutoCompleteSelectWidget
     lookup_cls = ThingLookup
 
     def test_has_complete_widget(self):
@@ -111,105 +113,105 @@
     def test_has_hidden_widget(self):
         widget = self.get_widget_instance()
         self.assertEqual(widget.widgets[1].__class__, forms.HiddenInput)
 
     def test_hidden_type(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget.widgets[1])
-        self.assertTrue('data-selectable-type' in attrs)
-        self.assertEqual(attrs['data-selectable-type'], 'hidden')
+        self.assertTrue("data-selectable-type" in attrs)
+        self.assertEqual(attrs["data-selectable-type"], "hidden")
 
     def test_update_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance()
         widget.update_query_parameters(params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_limit_parameter(self):
         widget = self.get_widget_instance(limit=10)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
-        self.assertTrue('limit=10' in query)
+        self.assertTrue("limit=10" in query)
 
     def test_initial_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance(query_params=params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_build_selectable_options(self):
         "Serialize selectable options as json in data attribute."
-        options = {'autoFocus': True}
-        widget = self.get_widget_instance(attrs={'data-selectable-options': options})
+        options = {"autoFocus": True}
+        widget = self.get_widget_instance(attrs={"data-selectable-options": options})
         attrs = parsed_widget_attributes(widget.widgets[0])
-        self.assertTrue('data-selectable-options' in attrs)
-        self.assertEqual(attrs['data-selectable-options'], json.dumps(options))
+        self.assertTrue("data-selectable-options" in attrs)
+        self.assertEqual(attrs["data-selectable-options"], json.dumps(options))
 
     def test_postdata_compatible_with_select(self):
         "Checks postdata for values that a select widget would generate."
-        postdata = {'fruit': '1'}
+        postdata = {"fruit": "1"}
         widget = self.get_widget_instance()
-        widget_val = widget.value_from_datadict(postdata, [], 'fruit')
-        self.assertEqual(widget_val, '1')
+        widget_val = widget.value_from_datadict(postdata, [], "fruit")
+        self.assertEqual(widget_val, "1")
 
 
 class AutoComboboxWidgetTestCase(BaseSelectableTestCase, WidgetTestMixin):
     widget_cls = widgets.AutoComboboxWidget
     lookup_cls = ThingLookup
 
     def test_rendered_attrs(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget)
-        self.assertTrue('data-selectable-url' in attrs)
-        self.assertTrue('data-selectable-type' in attrs)
-        self.assertTrue('data-selectable-allow-new' in attrs)
+        self.assertTrue("data-selectable-url" in attrs)
+        self.assertTrue("data-selectable-type" in attrs)
+        self.assertTrue("data-selectable-allow-new" in attrs)
 
     def test_update_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance()
         widget.update_query_parameters(params)
         attrs = parsed_widget_attributes(widget)
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_limit_parameter(self):
         widget = self.get_widget_instance(limit=10)
         attrs = parsed_widget_attributes(widget)
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
-        self.assertTrue('limit=10' in query)
+        self.assertTrue("limit=10" in query)
 
     def test_initial_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance(query_params=params)
         attrs = parsed_widget_attributes(widget)
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_build_selectable_options(self):
         "Serialize selectable options as json in data attribute."
-        options = {'autoFocus': True}
-        widget = self.get_widget_instance(attrs={'data-selectable-options': options})
+        options = {"autoFocus": True}
+        widget = self.get_widget_instance(attrs={"data-selectable-options": options})
         attrs = parsed_widget_attributes(widget)
-        self.assertTrue('data-selectable-options' in attrs)
-        self.assertEqual(attrs['data-selectable-options'], json.dumps(options))
+        self.assertTrue("data-selectable-options" in attrs)
+        self.assertEqual(attrs["data-selectable-options"], json.dumps(options))
 
 
 class AutoComboboxSelectWidgetTestCase(BaseSelectableTestCase, WidgetTestMixin):
     widget_cls = widgets.AutoComboboxSelectWidget
     lookup_cls = ThingLookup
 
     def test_has_complete_widget(self):
@@ -219,245 +221,245 @@
     def test_has_hidden_widget(self):
         widget = self.get_widget_instance()
         self.assertEqual(widget.widgets[1].__class__, forms.HiddenInput)
 
     def test_hidden_type(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget.widgets[1])
-        self.assertTrue('data-selectable-type' in attrs)
-        self.assertEqual(attrs['data-selectable-type'], 'hidden')
+        self.assertTrue("data-selectable-type" in attrs)
+        self.assertEqual(attrs["data-selectable-type"], "hidden")
 
     def test_update_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance()
         widget.update_query_parameters(params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_limit_parameter(self):
         widget = self.get_widget_instance(limit=10)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
-        self.assertTrue('limit=10' in query)
+        self.assertTrue("limit=10" in query)
 
     def test_initial_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance(query_params=params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_build_selectable_options(self):
         "Serialize selectable options as json in data attribute."
-        options = {'autoFocus': True}
-        widget = self.get_widget_instance(attrs={'data-selectable-options': options})
+        options = {"autoFocus": True}
+        widget = self.get_widget_instance(attrs={"data-selectable-options": options})
         attrs = parsed_widget_attributes(widget.widgets[0])
-        self.assertTrue('data-selectable-options' in attrs)
-        self.assertEqual(attrs['data-selectable-options'], json.dumps(options))
+        self.assertTrue("data-selectable-options" in attrs)
+        self.assertEqual(attrs["data-selectable-options"], json.dumps(options))
 
 
 class AutoCompleteSelectMultipleWidgetTestCase(BaseSelectableTestCase, WidgetTestMixin):
     widget_cls = widgets.AutoCompleteSelectMultipleWidget
     lookup_cls = ThingLookup
 
     def test_has_complete_widget(self):
         widget = self.get_widget_instance()
         self.assertEqual(widget.widgets[0].__class__, widgets.AutoCompleteWidget)
 
     def test_multiple_attr(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget.widgets[0])
-        self.assertTrue('data-selectable-multiple' in attrs)
-        self.assertEqual(attrs['data-selectable-multiple'], 'true')
+        self.assertTrue("data-selectable-multiple" in attrs)
+        self.assertEqual(attrs["data-selectable-multiple"], "true")
 
     def test_has_hidden_widget(self):
         widget = self.get_widget_instance()
         self.assertEqual(widget.widgets[1].__class__, widgets.LookupMultipleHiddenInput)
 
     def test_hidden_type(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget.widgets[1])
-        self.assertTrue('data-selectable-type' in attrs)
-        self.assertEqual(attrs['data-selectable-type'], 'hidden-multiple')
+        self.assertTrue("data-selectable-type" in attrs)
+        self.assertEqual(attrs["data-selectable-type"], "hidden-multiple")
 
     def test_render_single(self):
         widget = self.get_widget_instance()
         val = 4
-        rendered_value = widget.render('field_name', val)
+        rendered_value = widget.render("field_name", val)
         inputs = parsed_inputs(rendered_value)
-        field = inputs['field_name_1'][0]
+        field = inputs["field_name_1"][0]
         attributes = dict(field.attributes)
-        self.assertEqual(attributes['data-selectable-type'], 'hidden-multiple')
-        self.assertEqual(attributes['type'], 'hidden')
-        self.assertEqual(int(attributes['value']), val)
+        self.assertEqual(attributes["data-selectable-type"], "hidden-multiple")
+        self.assertEqual(attributes["type"], "hidden")
+        self.assertEqual(int(attributes["value"]), val)
 
     def test_render_list(self):
         widget = self.get_widget_instance()
         list_val = [8, 5]
-        rendered_value = widget.render('field_name', list_val)
+        rendered_value = widget.render("field_name", list_val)
         inputs = parsed_inputs(rendered_value)
         found_values = []
-        for field in inputs['field_name_1']:
+        for field in inputs["field_name_1"]:
             attributes = dict(field.attributes)
-            self.assertEqual(attributes['data-selectable-type'], 'hidden-multiple')
-            self.assertEqual(attributes['type'], 'hidden')
-            found_values.append(int(attributes['value']))
+            self.assertEqual(attributes["data-selectable-type"], "hidden-multiple")
+            self.assertEqual(attributes["type"], "hidden")
+            found_values.append(int(attributes["value"]))
         self.assertListEqual(found_values, list_val)
 
     def test_render_qs(self):
         widget = self.get_widget_instance()
         t1 = self.create_thing()
         t2 = self.create_thing()
         qs_val = Thing.objects.filter(pk__in=[t1.pk, t2.pk])
-        rendered_value = widget.render('field_name', qs_val)
+        rendered_value = widget.render("field_name", qs_val)
         inputs = parsed_inputs(rendered_value)
         found_values = []
         found_titles = []
-        for field in inputs['field_name_1']:
+        for field in inputs["field_name_1"]:
             attributes = dict(field.attributes)
-            self.assertEqual(attributes['data-selectable-type'], 'hidden-multiple')
-            self.assertEqual(attributes['type'], 'hidden')
-            found_titles.append(attributes['title'])
-            found_values.append(attributes['value'])
+            self.assertEqual(attributes["data-selectable-type"], "hidden-multiple")
+            self.assertEqual(attributes["type"], "hidden")
+            found_titles.append(attributes["title"])
+            found_values.append(attributes["value"])
         self.assertListEqual(found_values, [str(t1.pk), str(t2.pk)])
         self.assertListEqual(found_titles, [t1.name, t2.name])
 
     def test_update_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance()
         widget.update_query_parameters(params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_limit_parameter(self):
         widget = self.get_widget_instance(limit=10)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
-        self.assertTrue('limit=10' in query)
+        self.assertTrue("limit=10" in query)
 
     def test_initial_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance(query_params=params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_build_selectable_options(self):
         "Serialize selectable options as json in data attribute."
-        options = {'autoFocus': True}
-        widget = self.get_widget_instance(attrs={'data-selectable-options': options})
+        options = {"autoFocus": True}
+        widget = self.get_widget_instance(attrs={"data-selectable-options": options})
         attrs = parsed_widget_attributes(widget.widgets[0])
-        self.assertTrue('data-selectable-options' in attrs)
-        self.assertEqual(attrs['data-selectable-options'], json.dumps(options))
+        self.assertTrue("data-selectable-options" in attrs)
+        self.assertEqual(attrs["data-selectable-options"], json.dumps(options))
 
 
 class AutoComboboxSelectMultipleWidgetTestCase(BaseSelectableTestCase, WidgetTestMixin):
     widget_cls = widgets.AutoComboboxSelectMultipleWidget
     lookup_cls = ThingLookup
 
     def test_has_complete_widget(self):
         widget = self.get_widget_instance()
         self.assertEqual(widget.widgets[0].__class__, widgets.AutoComboboxWidget)
 
     def test_multiple_attr(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget.widgets[0])
-        self.assertTrue('data-selectable-multiple' in attrs)
-        self.assertEqual(attrs['data-selectable-multiple'], 'true')
+        self.assertTrue("data-selectable-multiple" in attrs)
+        self.assertEqual(attrs["data-selectable-multiple"], "true")
 
     def test_has_hidden_widget(self):
         widget = self.get_widget_instance()
         self.assertEqual(widget.widgets[1].__class__, widgets.LookupMultipleHiddenInput)
 
     def test_hidden_type(self):
         widget = self.get_widget_instance()
         attrs = parsed_widget_attributes(widget.widgets[1])
-        self.assertTrue('data-selectable-type' in attrs)
-        self.assertEqual(attrs['data-selectable-type'], 'hidden-multiple')
+        self.assertTrue("data-selectable-type" in attrs)
+        self.assertEqual(attrs["data-selectable-type"], "hidden-multiple")
 
     def test_render_single(self):
         widget = self.get_widget_instance()
         val = 4
-        rendered_value = widget.render('field_name', val)
+        rendered_value = widget.render("field_name", val)
         inputs = parsed_inputs(rendered_value)
-        field = inputs['field_name_1'][0]
+        field = inputs["field_name_1"][0]
         attributes = dict(field.attributes)
-        self.assertEqual(attributes['data-selectable-type'], 'hidden-multiple')
-        self.assertEqual(attributes['type'], 'hidden')
-        self.assertEqual(attributes['value'], str(val))
+        self.assertEqual(attributes["data-selectable-type"], "hidden-multiple")
+        self.assertEqual(attributes["type"], "hidden")
+        self.assertEqual(attributes["value"], str(val))
 
     def test_render_list(self):
         widget = self.get_widget_instance()
         list_val = [8, 5]
-        rendered_value = widget.render('field_name', list_val)
+        rendered_value = widget.render("field_name", list_val)
         inputs = parsed_inputs(rendered_value)
         found_values = []
-        for field in inputs['field_name_1']:
+        for field in inputs["field_name_1"]:
             attributes = dict(field.attributes)
-            self.assertEqual(attributes['data-selectable-type'], 'hidden-multiple')
-            self.assertEqual(attributes['type'], 'hidden')
-            found_values.append(int(attributes['value']))
+            self.assertEqual(attributes["data-selectable-type"], "hidden-multiple")
+            self.assertEqual(attributes["type"], "hidden")
+            found_values.append(int(attributes["value"]))
         self.assertListEqual(found_values, list_val)
 
     def test_render_qs(self):
         widget = self.get_widget_instance()
         t1 = self.create_thing()
         t2 = self.create_thing()
         qs_val = Thing.objects.filter(pk__in=[t1.pk, t2.pk])
-        rendered_value = widget.render('field_name', qs_val)
+        rendered_value = widget.render("field_name", qs_val)
         inputs = parsed_inputs(rendered_value)
         found_values = []
-        for field in inputs['field_name_1']:
+        for field in inputs["field_name_1"]:
             attributes = dict(field.attributes)
-            self.assertEqual(attributes['data-selectable-type'], 'hidden-multiple')
-            self.assertEqual(attributes['type'], 'hidden')
-            found_values.append(int(attributes['value']))
+            self.assertEqual(attributes["data-selectable-type"], "hidden-multiple")
+            self.assertEqual(attributes["type"], "hidden")
+            found_values.append(int(attributes["value"]))
         self.assertListEqual(found_values, [t1.pk, t2.pk])
 
     def test_update_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance()
         widget.update_query_parameters(params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_limit_parameter(self):
         widget = self.get_widget_instance(limit=10)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
-        self.assertTrue('limit=10' in query)
+        self.assertTrue("limit=10" in query)
 
     def test_initial_query_parameters(self):
-        params = {'active': 1}
+        params = {"active": 1}
         widget = self.get_widget_instance(query_params=params)
         attrs = parsed_widget_attributes(widget.widgets[0])
-        url = attrs['data-selectable-url']
+        url = attrs["data-selectable-url"]
         parse = urlparse(url)
         query = parse.query
         self.assertEqual(query, urlencode(params))
 
     def test_build_selectable_options(self):
         "Serialize selectable options as json in data attribute."
-        options = {'autoFocus': True}
-        widget = self.get_widget_instance(attrs={'data-selectable-options': options})
+        options = {"autoFocus": True}
+        widget = self.get_widget_instance(attrs={"data-selectable-options": options})
         attrs = parsed_widget_attributes(widget.widgets[0])
-        self.assertTrue('data-selectable-options' in attrs)
-        self.assertEqual(attrs['data-selectable-options'], json.dumps(options))
+        self.assertTrue("data-selectable-options" in attrs)
+        self.assertEqual(attrs["data-selectable-options"], json.dumps(options))
```

### Comparing `django-selectable-1.3.0/setup.py` & `django-selectable-1.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,25 +23,22 @@
     url='https://github.com/mlavin/django-selectable',
     license='BSD',
     description=' '.join(__import__('selectable').__doc__.splitlines()).strip(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Framework :: Django',
-        'Framework :: Django :: 1.11',
-        'Framework :: Django :: 2.0',
-        'Framework :: Django :: 2.1',
-        'Framework :: Django :: 2.2',
-        'Framework :: Django :: 3.0',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.2',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
     ],
     long_description=read_file('README.rst'),
     test_suite="runtests.runtests",
     zip_safe=False,  # because we're including media that Django needs
 )
```

