# Comparing `tmp/eox-hooks-4.1.0.tar.gz` & `tmp/eox-hooks-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eox-hooks-4.1.0.tar", last modified: Wed May 10 22:12:59 2023, max compression
+gzip compressed data, was "eox-hooks-4.1.1.tar", last modified: Wed Jun 21 22:13:04 2023, max compression
```

## Comparing `eox-hooks-4.1.0.tar` & `eox-hooks-4.1.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.970454 eox-hooks-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-10 22:12:59.970454 eox-hooks-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.962454 eox-hooks-4.1.0/eox_hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/actions_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.966454 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.966454 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/course_modes_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/course_modes_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/course_modes_l_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/courses_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/courses_j_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/courses_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/enrollments_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/enrollments_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/enrollments_l_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/models_j_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/models_l_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/models_l_v1_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/course_modes.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/courses.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/enrollments.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.966454 eox-hooks-4.1.0/eox_hooks/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.970454 eox-hooks-4.1.0/eox_hooks/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_actions_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_receivers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/eox_hooks/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.962454 eox-hooks-4.1.0/eox_hooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-10 22:12:59.000000 eox-hooks-4.1.0/eox_hooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-10 22:12:59.000000 eox-hooks-4.1.0/eox_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:12:59.000000 eox-hooks-4.1.0/eox_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 22:12:59.000000 eox-hooks-4.1.0/eox_hooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 22:12:59.000000 eox-hooks-4.1.0/eox_hooks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 22:12:59.000000 eox-hooks-4.1.0/eox_hooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-10 22:12:59.000000 eox-hooks-4.1.0/eox_hooks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 22:12:59.970454 eox-hooks-4.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-05-10 22:12:59.970454 eox-hooks-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-05-10 22:12:44.000000 eox-hooks-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.156689 eox-hooks-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-21 22:13:04.156689 eox-hooks-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.144689 eox-hooks-4.1.1/eox_hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/actions_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.148689 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.152689 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/course_modes_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/course_modes_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/course_modes_l_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/courses_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/courses_j_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/courses_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/enrollments_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/enrollments_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/enrollments_l_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/models_j_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/models_l_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/models_l_v1_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/course_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/courses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/enrollments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.152689 eox-hooks-4.1.1/eox_hooks/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/settings/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.156689 eox-hooks-4.1.1/eox_hooks/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11900 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_actions_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18402 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_receivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/eox_hooks/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.148689 eox-hooks-4.1.1/eox_hooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-06-21 22:13:04.000000 eox-hooks-4.1.1/eox_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-21 22:13:04.000000 eox-hooks-4.1.1/eox_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:13:04.000000 eox-hooks-4.1.1/eox_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-21 22:13:04.000000 eox-hooks-4.1.1/eox_hooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:13:03.000000 eox-hooks-4.1.1/eox_hooks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-21 22:13:04.000000 eox-hooks-4.1.1/eox_hooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 22:13:04.000000 eox-hooks-4.1.1/eox_hooks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:13:04.156689 eox-hooks-4.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-21 22:13:04.156689 eox-hooks-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-06-21 22:12:46.000000 eox-hooks-4.1.1/setup.py
```

### Comparing `eox-hooks-4.1.0/LICENSE.txt` & `eox-hooks-4.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/PKG-INFO` & `eox-hooks-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-hooks
-Version: 4.1.0
+Version: 4.1.1
 Summary: EoxHooks
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-hooks-4.1.0/README.rst` & `eox-hooks-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/actions.py` & `eox-hooks-4.1.1/eox_hooks/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,17 +154,21 @@
 
     followup_enrollments = getattr(course, "other_course_settings", {}).get(
         "EDNX_TRIGGER_FOLLOWUP_ENROLLMENTS"
     )
 
     if not followup_enrollments:
         return
+    followup_list = []
+    for enroll in followup_enrollments:
+        if str(enrollment.course.course_key) != enroll['course_id']:
+            followup_list.append(enroll)
 
     create_enrollments_for_program.delay(
-        enrollment.user.pii.username, followup_enrollments,
+        enrollment.user.pii.username, followup_list,
     )
 
 
 def trigger_grades_assignment(**kwargs):
     """
     Custom action that propagates grades to a course component.
```

### Comparing `eox-hooks-4.1.0/eox_hooks/actions_handler.py` & `eox-hooks-4.1.1/eox_hooks/actions_handler.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/apps.py` & `eox-hooks-4.1.1/eox_hooks/apps.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/courses_j_v1.py` & `eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/courses_j_v1.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/courses_l_v1.py` & `eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/courses_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/backends/models_l_v1.py` & `eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/backends/models_l_v1.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/courses.py` & `eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/courses.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/edxapp_wrapper/models.py` & `eox-hooks-4.1.1/eox_hooks/edxapp_wrapper/models.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/receivers.py` & `eox-hooks-4.1.1/eox_hooks/receivers.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/serializers.py` & `eox-hooks-4.1.1/eox_hooks/serializers.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/settings/common.py` & `eox-hooks-4.1.1/eox_hooks/settings/common.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/settings/production.py` & `eox-hooks-4.1.1/eox_hooks/settings/production.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/settings/test.py` & `eox-hooks-4.1.1/eox_hooks/settings/test.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tasks.py` & `eox-hooks-4.1.1/eox_hooks/tasks.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_actions.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,28 +162,28 @@
 
         Expected behavior:
             - Action starts an async task that creates the other enrollments.
         """
         other_course_settings = {
             "EDNX_TRIGGER_FOLLOWUP_ENROLLMENTS": [
                 {
-                    "course_id": "course-v1:edX+DemoX+Demo_Course",
+                    "course_id": "course-v1:edX+Demo123+Demo_Course",
                 },
             ],
         }
         mock_course = MagicMock(other_course_settings=other_course_settings)
         get_course.return_value = mock_course
 
         trigger_enrollments_creation(**self.kwargs)
 
         create_enroll_task.delay.assert_called_once_with(
             "test",
             [
                 {
-                    "course_id": "course-v1:edX+DemoX+Demo_Course",
+                    "course_id": "course-v1:edX+Demo123+Demo_Course",
                 },
             ],
         )
 
 
 class TriggerGradingTest(TestCase):
     """
```

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_actions_handler.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_actions_handler.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_apps.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_apps.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_receivers.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_receivers.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_serializers.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_tasks.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_utils.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/tests/test_views.py` & `eox-hooks-4.1.1/eox_hooks/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/urls.py` & `eox-hooks-4.1.1/eox_hooks/urls.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/utils.py` & `eox-hooks-4.1.1/eox_hooks/utils.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks/views.py` & `eox-hooks-4.1.1/eox_hooks/views.py`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/eox_hooks.egg-info/PKG-INFO` & `eox-hooks-4.1.1/eox_hooks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eox-hooks
-Version: 4.1.0
+Version: 4.1.1
 Summary: EoxHooks
 Author: eduNEXT
 Author-email: contact@edunext.co
 License: AGPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
```

### Comparing `eox-hooks-4.1.0/eox_hooks.egg-info/SOURCES.txt` & `eox-hooks-4.1.1/eox_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eox-hooks-4.1.0/setup.cfg` & `eox-hooks-4.1.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 4.1.0
+current_version = 4.1.1
 commit = False
 tag = False
 
 [isort]
 default_section = THIRDPARTY
 known_first_party = eox_hooks
 include_trailing_comma = True
```

### Comparing `eox-hooks-4.1.0/setup.py` & `eox-hooks-4.1.1/setup.py`

 * *Files identical despite different names*

